# Comparing `tmp/cdpcli-beta-0.9.89.tar.gz` & `tmp/cdpcli-beta-0.9.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.89.tar", last modified: Wed Jun 14 22:47:31 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.90.tar", last modified: Thu Jun 22 06:18:25 2023, max compression
```

## Comparing `cdpcli-beta-0.9.89.tar` & `cdpcli-beta-0.9.90.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-06-14 22:47:26.000000 cdpcli-beta-0.9.89/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   148743 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   104375 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193260 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   177206 2023-06-14 22:47:26.000000 cdpcli-beta-0.9.89/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.508536 cdpcli-beta-0.9.89/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.508536 cdpcli-beta-0.9.89/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.466169 cdpcli-beta-0.9.90/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-22 06:18:25.466169 cdpcli-beta-0.9.90/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.466169 cdpcli-beta-0.9.90/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-22 06:18:25.466169 cdpcli-beta-0.9.90/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-22 06:18:20.000000 cdpcli-beta-0.9.90/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-06-22 06:18:20.000000 cdpcli-beta-0.9.90/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   150970 2023-06-22 06:18:22.000000 cdpcli-beta-0.9.90/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   105695 2023-06-22 06:18:21.000000 cdpcli-beta-0.9.90/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-22 06:18:22.000000 cdpcli-beta-0.9.90/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-22 06:18:21.000000 cdpcli-beta-0.9.90/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193413 2023-06-22 06:18:21.000000 cdpcli-beta-0.9.90/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   181044 2023-06-22 06:18:20.000000 cdpcli-beta-0.9.90/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-22 06:18:22.000000 cdpcli-beta-0.9.90/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-22 06:18:21.000000 cdpcli-beta-0.9.90/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.454169 cdpcli-beta-0.9.90/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    73060 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-22 06:18:23.000000 cdpcli-beta-0.9.90/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.446169 cdpcli-beta-0.9.90/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.458169 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-22 06:18:24.000000 cdpcli-beta-0.9.90/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-22 06:18:25.466169 cdpcli-beta-0.9.90/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.446169 cdpcli-beta-0.9.90/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.462169 cdpcli-beta-0.9.90/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.462169 cdpcli-beta-0.9.90/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.462169 cdpcli-beta-0.9.90/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.462169 cdpcli-beta-0.9.90/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:18:25.462169 cdpcli-beta-0.9.90/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-22 06:07:05.000000 cdpcli-beta-0.9.90/versioneer.py
```

### Comparing `cdpcli-beta-0.9.89/LICENSE.txt` & `cdpcli-beta-0.9.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.90/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/PKG-INFO` & `cdpcli-beta-0.9.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.89
+Version: 0.9.90
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.89/README.md` & `cdpcli-beta-0.9.90/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/__init__.py` & `cdpcli-beta-0.9.90/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/argparser.py` & `cdpcli-beta-0.9.90/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/argprocess.py` & `cdpcli-beta-0.9.90/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/arguments.py` & `cdpcli-beta-0.9.90/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/auth.py` & `cdpcli-beta-0.9.90/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.90/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/clicommand.py` & `cdpcli-beta-0.9.90/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/clidriver.py` & `cdpcli-beta-0.9.90/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/client.py` & `cdpcli-beta-0.9.90/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/compat.py` & `cdpcli-beta-0.9.90/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/completer.py` & `cdpcli-beta-0.9.90/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/config.py` & `cdpcli-beta-0.9.90/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/configloader.py` & `cdpcli-beta-0.9.90/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/credentials.py` & `cdpcli-beta-0.9.90/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.90/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/cli.json` & `cdpcli-beta-0.9.90/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/datahub/datahub.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1418,14 +1418,24 @@
         type: string
         description: The name of the instance group where the given instance is located.
       instances:
         type: array
         items:
           $ref: '#/definitions/Instance'
         description: List of instances in this instance group.
+      subnetIds:
+        type: array
+        items:
+          type: string
+        description: The list of subnet IDs in case of multi-availability zone setup
+      availabilityZones:
+        type: array
+        items:
+          type: string
+        description: List of availability zones that this instance group is associated with.
   StartClusterVerticalScalingRequest:
     type: object
     description: The request object for Data Hub vertical scaling.
     required:
       - datahub
       - group
       - instanceTemplate
@@ -1478,14 +1488,59 @@
         description: The public IP of the given instance.
       fqdn:
         type: string
         description: The FQDN of the instance.
       status:
         type: string
         description: The status of the instance. This includes information like whether the instance is being provisioned, stopped, decommissioning failures etc.
+      statusReason:
+        type: string
+        description: The reason for the current status of this instance.
+      sshPort:
+        type: integer
+        format: int32
+        description: The SSH port for the instance.
+      clouderaManagerServer:
+        type: boolean
+        description: Whether the instance has Cloudera Manager deployed or not.
+      instanceGroup:
+        type: string
+        description: The name of the instance group this instance belongs to.
+      attachedVolumes:
+        type: array
+        description: List of volumes attached to this instance.
+        items:
+          $ref: '#/definitions/AttachedVolumeDetail'
+      availabilityZone:
+        type: string
+        description: The availability zone of the instance.
+      instanceVmType:
+        type: string
+        description: The VM type of the instance. Supported values depend on the cloud platform.
+      rackId:
+        type: string
+        description: The rack ID of the instance in Cloudera Manager.
+      subnetId:
+        type: string
+        description: The subnet ID of the instance.
+  AttachedVolumeDetail:
+    type: object
+    description: The attached volume configuration.
+    properties:
+      count:
+        type: integer
+        format: int32
+        description: The number of volumes.
+      volumeType:
+        type: string
+        description: The type of volumes.
+      size:
+        type: integer
+        format: int32
+        description: The size of each volume in GB.
   Endpoints:
     type: object
     description: Object which holds the exposed endpoints for the given cluster.
     required:
       - endpoints
     properties:
       endpoints:
@@ -2286,14 +2341,19 @@
         description: The names or CRNs of the recipes that would be applied to the instance group.
       recoveryMode:
         type: string
         description: Recovery mode for the instance group.
       volumeEncryption:
         $ref: '#/definitions/VolumeEncryptionRequest'
         description: The volume encryption settings. This setting does not apply to Azure which always encrypts volumes.
+      subnetIds:
+        type: array
+        items:
+          type: string
+        description: The list of subnet IDs in case of multi-availability zone setup. Specifying this field overrides the datahub level subnet ID setup for the multi-availability zone configuration.
   AzureInstanceGroupRequest:
     type: object
     description: Configurations for instance group
     required:
       - nodeCount
       - instanceGroupName
       - instanceGroupType
@@ -4066,14 +4126,17 @@
         description: Checks the eligibility of an image to upgrade but do not perform the upgrade.
       showAvailableImages:
         type: boolean
         description: Returns the list of images that are eligible for the upgrade.
       showLatestAvailableImagePerRuntime:
         type: boolean
         description: Returns the latest image that is eligible for the upgrade for each runtime version with at least one available upgrade candidate.
+      rollingUpgradeEnabled:
+        type: boolean
+        description: Enables the ability to perform rolling runtime upgrade.
   UpgradeClusterResponse:
     type: object
     description: Response object for upgrade datahub request.
     properties:
       current:
         $ref: '#/definitions/ImageInfo'
         description: Information about the current image.
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1058,14 +1058,19 @@
         type: string
         description: The name of the instance group.
       instances:
         type: array
         items:
           $ref: '#/definitions/Instance'
         description: List of instances in this instance group.
+      availabilityZones:
+        type: array
+        items:
+          type: string
+        description: List of availability zones that this instance group is associated with.
   Instance:
     type: object
     description: Object which holds some details of an instance for the given cluster.
     required:
       - id
       - state
     properties:
@@ -1090,20 +1095,40 @@
       publicIp:
         type: string
         description: The public IP of the given instance.
       sshPort:
         type: integer
         format: int32
         description: The SSH port for the instance.
+      clouderaManagerServer:
+        type: boolean
+        description: Whether the instance has Cloudera Manager deployed or not.
       instanceGroup:
         type: string
         description: The name of the instance group this instance belongs to.
       instanceTypeVal:
         $ref: '#/definitions/DatalakeInstanceType'
         description: The instance type.
+      attachedVolumes:
+        type: array
+        description: List of volumes attached to this instance.
+        items:
+          $ref: '#/definitions/AttachedVolumeDetail'
+      availabilityZone:
+        type: string
+        description: The availability zone of the instance.
+      instanceVmType:
+        type: string
+        description: The VM type of the instance. Supported values depend on the cloud platform.
+      rackId:
+        type: string
+        description: The rack ID of the instance in Cloudera Manager.
+      subnetId:
+        type: string
+        description: The subnet ID of the instance.
   DatalakeInstanceStatus:
     type: string
     description: The status of the instance.
     enum:
       - REQUESTED
       - FAILED
       - CREATED
@@ -1122,14 +1147,29 @@
   DatalakeInstanceType:
     type: string
     description: The type of the instance.
     enum:
       - GATEWAY
       - GATEWAY_PRIMARY
       - CORE
+  AttachedVolumeDetail:
+    type: object
+    description: The attached volume configuration.
+    properties:
+      count:
+        type: integer
+        format: int32
+        description: The number of volumes.
+      volumeType:
+        type: string
+        description: The type of volumes.
+      size:
+        type: integer
+        format: int32
+        description: The size of each volume in GB.
   Endpoints:
     type: object
     description: Object which holds the exposed endpoints for the given cluster.
     required:
       - endpoints
     properties:
       endpoints:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/dw/dw.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1926,14 +1926,17 @@
         type: array
         items:
           type: string
         description: List of IP address CIDRs to whitelist for workload access.
       usePrivateLoadBalancer:
         type: boolean
         description: Set up load balancer with private IP address. In AWS it is created in private subnets. In Azure an internal load balancer gets created. Make sure there is connectivity between your client network and the network (VPC/VNet) where CDW environment is deployed.
+      usePublicWorkerNode:
+        type: boolean
+        description: Set up worker node with public IP address. In AWS it is created in public subnets.
       enableStorageRoles:
         type: boolean
         description: Enable Storage Roles
         default: false
         x-form-factors: public
         x-entitlement: CDW_STORAGE_ROLES
       customRegistryOptions:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/environments/environments.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1525,14 +1525,36 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/UpdateOrchestratorStateResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/environments2/updateProxyConfig:
+    post:
+      summary: Updates the proxy config of the given environment.
+      description: Updates the proxy config of the given environment.
+      operationId: updateProxyConfig
+      x-mutating: true
+      x-entitlement: CDP_ENVIRONMENT_EDIT_PROXY_CONFIG
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateProxyConfigRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateProxyConfigResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
@@ -3884,15 +3906,15 @@
           type: string
         description: The recipes for the FreeIPA cluster.
       instanceType:
         type: string
         description: Custom instance type of FreeIPA instances.
       multiAz:
         type: boolean
-        description: Flag which marks that the freeIPA will be deployed in a multi-availability zone way or not.
+        description: Flag which marks that the FreeIPA will be deployed in a multi-availability zone way or not.
   AzureFreeIpaCreationRequest:
     description: Request object for creating FreeIPA in the environment.
     type: object
     properties:
       instanceCountByGroup:
         type: integer
         format: int32
@@ -3920,17 +3942,14 @@
         description: The recipes for the FreeIPA cluster.
       instanceType:
         type: string
         description: Custom instance type of FreeIPA instances.
   FreeIpaImageRequest:
     description: Request object for FreeIPA image.
     type: object
-    required:
-      - catalog
-      - id
     properties:
       catalog:
         type: string
         description: Image catalog to use for FreeIPA image selection.
         x-no-paramfile: true
       id:
         type: string
@@ -3981,14 +4000,84 @@
         items:
           type: string
       recipes:
         type: array
         description: The recipes for the FreeIPA cluster.
         items:
           type: string
+      instances:
+        type: array
+        description: The instances of the FreeIPA cluster.
+        uniqueItems: true
+        items:
+          $ref: '#/definitions/FreeIpaInstance'
+  FreeIpaInstance:
+    type: object
+    description: Object for a FreeIPA instance providing specific information about the instance.
+    properties:
+      availabilityZone:
+        type: string
+        description: The availability zone of the instance.
+      discoveryFQDN:
+        type: string
+        description: The fully qualified domain name of the instance in the service discovery cluster.
+      instanceId:
+        type: string
+        description: The instance ID for the instance.
+      instanceGroup:
+        type: string
+        description: The instance group that contains the instance.
+      instanceStatus:
+        type: string
+        description: The status of the instance.
+      instanceStatusReason:
+        type: string
+        description: The status reason for the instance.
+      instanceType:
+        type: string
+        description: The type of the instance (either GATEWAY or GATEWAY_PRIMARY).
+      instanceVmType:
+        type: string
+        description: The VM type of the instance. Supported values depend on the cloud platform.
+      lifeCycle:
+        type: string
+        description: The life cycle type for the instance (either NORMAL or SPOT).
+      privateIP:
+        type: string
+        description: The private IP of the instance.
+      publicIP:
+        type: string
+        description: The public IP of the instance.
+      sshPort:
+        type: integer
+        format: int32
+        description: The SSH port of the instance.
+      subnetId:
+        type: string
+        description: The subnet ID of the instance.
+      attachedVolumes:
+        type: array
+        description: List of volumes attached to this instance.
+        items:
+          $ref: '#/definitions/AttachedVolumeDetail'
+  AttachedVolumeDetail:
+    type: object
+    description: The attached volume configuration.
+    properties:
+      count:
+        type: integer
+        format: int32
+        description: The number of volumes.
+      volumeType:
+        type: string
+        description: The type of volumes.
+      size:
+        type: integer
+        format: int32
+        description: The size of each volume in GB.
   ProxyConfig:
     type: object
     description: A proxy config object.
     required:
       - proxyConfigName
       - crn
       - protocol
@@ -4890,14 +4979,32 @@
     properties:
       environment:
         type: string
         description: The name or CRN of the environment.
   RotateSaltPasswordResponse:
     type: object
     description: Response object for rotating SaltStack user password on FreeIPA instances.
+  UpdateProxyConfigRequest:
+    type: object
+    description: Request object for updating the proxy config of the given environment.
+    required:
+      - environment
+    properties:
+      environment:
+        type: string
+        description: The name or CRN of the environment.
+      proxyConfigName:
+        type: string
+        description: The name of the new proxy config for the environment. Either this or the remove proxy flag has to be given.
+      removeProxy:
+        type: boolean
+        description: Flag to indicate that the current proxy config should be removed for the environment. Either this or a proxy config name has to be given.
+  UpdateProxyConfigResponse:
+    type: object
+    description: Response object for updating the proxy config of the given environment.
   UpdateOrchestratorStateRequest:
     type: object
     description: Request object for running orchestrator engine state update on the FreeIPA cluster.
     required:
       - environment
     properties:
       environment:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/opdb/opdb.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -704,14 +704,39 @@
     properties:
       key:
         type: string
         description: Key
       value:
         type: string
         description: Value
+  InstanceGroupType:
+    type: string
+    description: "InstanceGroup Type.\n `WORKER` - WORKER value of the InstanceGroup name. `LEADER` - LEADER value of the InstanceGroup name. `MASTER` - MASTER value of the InstanceGroup name. `GATEWAY` - GATEWAY value of the InstanceGroup name. `STRONGMETA` - STRONGMETA value of the InstanceGroup name. `EDGE` - EDGE value of the InstanceGroup name."
+    enum:
+      - WORKER
+      - LEADER
+      - MASTER
+      - GATEWAY
+      - STRONGMETA
+      - EDGE
+  CustomRecipe:
+    type: object
+    description: Describe a custom recipe.
+    required:
+      - names
+      - instanceGroup
+    properties:
+      names:
+        type: array
+        items:
+          type: string
+        description: Name of the recipe.
+      instanceGroup:
+        description: Instance group to apply the recipe to.
+        $ref: '#/definitions/InstanceGroupType'
   CreateDatabaseRequest:
     type: object
     description: A request to create the database
     required:
       - environmentName
       - databaseName
     properties:
@@ -768,14 +793,19 @@
         description: Disable OAuth Bearer (JWT) authentication scheme.
       enableRegionCanary:
         type: boolean
         description: To enable the region canary for the database.
       scaleType:
         description: Optional tags to choose one of the predefined cluster sizes.
         $ref: '#/definitions/ScaleType'
+      recipes:
+        type: array
+        items:
+          $ref: '#/definitions/CustomRecipe'
+        description: Custom recipes for the database.
   VolumeType:
     type: string
     description: "Volume Type.\n `HDD` - Hard disk drives (HDD) volume type. Default is HDD. `SSD` - Solid disk drives (SSD) volume type."
     enum:
       - HDD
       - SSD
   AttachedStorageForWorkers:
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.90/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.89
+  version: 0.9.90
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.89/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.90/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.90/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/doc/style.py` & `cdpcli-beta-0.9.90/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/docs.py` & `cdpcli-beta-0.9.90/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/endpoint.py` & `cdpcli-beta-0.9.90/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.90/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.90/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.90/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.90/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.90/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/exceptions.py` & `cdpcli-beta-0.9.90/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.90/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/formatter.py` & `cdpcli-beta-0.9.90/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/help.py` & `cdpcli-beta-0.9.90/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/loader.py` & `cdpcli-beta-0.9.90/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/main.py` & `cdpcli-beta-0.9.90/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/model.py` & `cdpcli-beta-0.9.90/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/paginate.py` & `cdpcli-beta-0.9.90/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/paramfile.py` & `cdpcli-beta-0.9.90/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.90/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/parser.py` & `cdpcli-beta-0.9.90/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.90/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/schema.py` & `cdpcli-beta-0.9.90/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/serialize.py` & `cdpcli-beta-0.9.90/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/shorthand.py` & `cdpcli-beta-0.9.90/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/signers.py` & `cdpcli-beta-0.9.90/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/table.py` & `cdpcli-beta-0.9.90/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/text.py` & `cdpcli-beta-0.9.90/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/textwriter.py` & `cdpcli-beta-0.9.90/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.90/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/translate.py` & `cdpcli-beta-0.9.90/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/utils.py` & `cdpcli-beta-0.9.90/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli/validate.py` & `cdpcli-beta-0.9.90/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.90/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.89
+Version: 0.9.90
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.89/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.90/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/setup.py` & `cdpcli-beta-0.9.90/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/setup_common.py` & `cdpcli-beta-0.9.90/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/__init__.py` & `cdpcli-beta-0.9.90/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.90/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.90/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.90/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.90/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_auth.py` & `cdpcli-beta-0.9.90/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.90/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_client.py` & `cdpcli-beta-0.9.90/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_completer.py` & `cdpcli-beta-0.9.90/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.90/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_docs.py` & `cdpcli-beta-0.9.90/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.90/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_help.py` & `cdpcli-beta-0.9.90/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.90/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_model.py` & `cdpcli-beta-0.9.90/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.90/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.90/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.90/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.90/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.90/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_signers.py` & `cdpcli-beta-0.9.90/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.90/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_utils.py` & `cdpcli-beta-0.9.90/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/tests/unit/test_validate.py` & `cdpcli-beta-0.9.90/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.89/versioneer.py` & `cdpcli-beta-0.9.90/versioneer.py`

 * *Files identical despite different names*

