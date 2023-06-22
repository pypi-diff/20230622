# Comparing `tmp/cdpcli-0.9.9.tar.gz` & `tmp/cdpcli-0.9.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdpcli-0.9.9.tar", last modified: Wed Apr  8 03:44:24 2020, max compression
+gzip compressed data, was "cdpcli-0.9.90.tar", last modified: Thu Jun 22 06:16:30 2023, max compression
```

## Comparing `cdpcli-0.9.9.tar` & `cdpcli-0.9.90.tar`

### file list

```diff
@@ -1,227 +1,183 @@
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    49425 2020-04-08 03:37:47.000000 cdpcli-0.9.9/NOTICES.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2309 2020-04-08 03:37:47.000000 cdpcli-0.9.9/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    68612 2020-04-08 03:37:47.000000 cdpcli-0.9.9/versioneer.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli.egg-info/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)       85 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)        1 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1343 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (114) jenkins    (118)       13 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      144 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7594 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11358 2020-04-08 03:37:47.000000 cdpcli-0.9.9/LICENSE.txt
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1343 2020-04-08 03:44:24.000000 cdpcli-0.9.9/PKG-INFO
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2517 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/exceptions.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    16810 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/adapters.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)   308434 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/cacert.pem
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      820 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/hooks.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5415 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/api.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4374 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/exceptions.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4507 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9326 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11628 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/six.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     8935 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ordered_dict.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)       74 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3778 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      460 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2281 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/filepost.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9011 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/connection.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    10037 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/ssl_.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9544 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/timeout.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5836 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/url.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9924 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/retry.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3293 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/connection.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      566 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/response.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2089 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/request.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      486 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9406 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/poolmanager.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    16459 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/response.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5833 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/fields.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5751 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/request.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    30319 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/connectionpool.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2055 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    10428 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/_collections.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3187 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/escprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    45972 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euckrfreq.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1902 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/charsetprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1674 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euctwprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1967 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcsgroupprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2318 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/codingstatemachine.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11318 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langhebrewmodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    17725 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langcyrillicmodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6840 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/universaldetector.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1684 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/big5prober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7839 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/escsm.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/utf8prober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9226 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/chardistribution.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    82594 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/big5freq.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    19348 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/jpcntx.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12784 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langbulgarianmodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    47315 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/jisfreq.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1675 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euckrprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    19590 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcssm.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    36011 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/gb2312freq.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12536 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langhungarianmodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    34872 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euctwfreq.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1782 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/cp949prober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1333 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/constants.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2504 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/chardetect.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sjisprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3291 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sbcsgroupprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3787 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/charsetgroupprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11275 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langthaimodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    13359 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/hebrewprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3678 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/eucjpprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1157 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/compat.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1679 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/gb2312prober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1295 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5232 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/latin1prober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4793 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sbcharsetprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12628 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langgreekmodel.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3268 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcharsetprober.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)       62 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    17191 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/cookies.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    24250 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/sessions.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2977 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/structures.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      613 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/certs.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6794 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/auth.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    29176 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/models.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3200 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/status_codes.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    21334 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/utils.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1469 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/compat.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1861 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    27344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6261 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/exceptions.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    16363 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      497 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/_version.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3837 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    17092 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/commands.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9335 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11071 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2641 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      971 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3749 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4854 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/set.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6203 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5432 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1357 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11436 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/credentials.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      771 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/main.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9950 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/validate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    20401 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/client.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    20750 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/clidriver.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/doc/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    10699 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7269 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1857 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/_examples.rst
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1936 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1193 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      560 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      862 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/_description.rst
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/dataeng/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2137 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/examples/dataeng/submit-jobs.rst
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3401 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11896 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6963 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    14764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/table.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    16344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/model.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    22915 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    13740 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    13421 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9313 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     8353 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    10239 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/endpoint.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4389 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/text.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7949 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7604 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    20851 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/textwriter.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3437 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     7334 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/help.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9323 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6528 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/compat.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    94175 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/iam/iam.yaml
--rw-rw-r--   0 jenkins    (114) jenkins    (118)       73 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/aliases.yaml
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1002 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/data/_retry.json
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    22237 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    29396 2020-04-08 03:44:20.000000 cdpcli-0.9.9/cdpcli/data/ml/ml.yaml
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2070 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    57881 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    50828 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/datahub/datahub.yaml
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     9211 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6456 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1207 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5732 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2241 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3377 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4824 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    16301 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2433 2020-04-08 03:37:47.000000 cdpcli-0.9.9/setup.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     1815 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5370 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3807 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    10918 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11649 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      732 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    13191 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6143 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5696 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_set.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     5637 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     8304 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3412 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6671 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12035 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11015 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6829 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     6354 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11859 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2663 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12543 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    14273 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    22467 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    18652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    14551 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     3116 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4603 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    12725 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     2642 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    11124 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     8860 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)    13775 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)     4162 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/__init__.py
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      314 2020-04-08 03:44:24.000000 cdpcli-0.9.9/setup.cfg
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      308 2020-04-08 03:37:47.000000 cdpcli-0.9.9/MANIFEST.in
--rw-rw-r--   0 jenkins    (114) jenkins    (118)      451 2020-04-08 03:37:47.000000 cdpcli-0.9.9/README.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.054955 cdpcli-0.9.90/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-22 06:06:23.000000 cdpcli-0.9.90/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-22 06:06:23.000000 cdpcli-0.9.90/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-22 06:06:23.000000 cdpcli-0.9.90/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-06-22 06:16:30.054955 cdpcli-0.9.90/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-22 06:06:23.000000 cdpcli-0.9.90/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.054955 cdpcli-0.9.90/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-22 06:16:30.054955 cdpcli-0.9.90/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      222 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15591 2023-06-22 06:16:25.000000 cdpcli-0.9.90/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   144916 2023-06-22 06:16:27.000000 cdpcli-0.9.90/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   102676 2023-06-22 06:16:26.000000 cdpcli-0.9.90/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-22 06:16:26.000000 cdpcli-0.9.90/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-22 06:16:26.000000 cdpcli-0.9.90/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193413 2023-06-22 06:16:25.000000 cdpcli-0.9.90/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   165510 2023-06-22 06:16:25.000000 cdpcli-0.9.90/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   132904 2023-06-22 06:16:27.000000 cdpcli-0.9.90/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-06-22 06:16:25.000000 cdpcli-0.9.90/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56809 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    24469 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        6 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.038955 cdpcli-0.9.90/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-22 06:16:28.000000 cdpcli-0.9.90/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.042955 cdpcli-0.9.90/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.022955 cdpcli-0.9.90/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.042955 cdpcli-0.9.90/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.042955 cdpcli-0.9.90/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.042955 cdpcli-0.9.90/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.042955 cdpcli-0.9.90/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.046955 cdpcli-0.9.90/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.046955 cdpcli-0.9.90/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.046955 cdpcli-0.9.90/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-22 06:06:23.000000 cdpcli-0.9.90/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.034955 cdpcli-0.9.90/cdpcli.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4214 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-22 06:16:29.000000 cdpcli-0.9.90/cdpcli.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-22 06:16:30.054955 cdpcli-0.9.90/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1414 2023-06-22 06:06:23.000000 cdpcli-0.9.90/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-22 06:06:23.000000 cdpcli-0.9.90/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.026955 cdpcli-0.9.90/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.050955 cdpcli-0.9.90/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.050955 cdpcli-0.9.90/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.050955 cdpcli-0.9.90/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.054955 cdpcli-0.9.90/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:16:30.054955 cdpcli-0.9.90/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-22 06:06:23.000000 cdpcli-0.9.90/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-22 06:06:23.000000 cdpcli-0.9.90/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdpcli-0.9.9/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-0.9.90/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/versioneer.py` & `cdpcli-0.9.90/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,23 +558,23 @@
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
         f = open(versionfile_abs, "r")
         for line in f.readlines():
             if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
+                mo = re.search('=\\s*"(.*)"', line)
                 if mo:
                     keywords["refnames"] = mo.group(1)
             if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
+                mo = re.search('=\\s*"(.*)"', line)
                 if mo:
                     keywords["full"] = mo.group(1)
             if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
+                mo = re.search('=\\s*"(.*)"', line)
                 if mo:
                     keywords["date"] = mo.group(1)
         f.close()
     except EnvironmentError:
         pass
     return keywords
 
@@ -607,15 +607,15 @@
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search('\\d', r)])
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
@@ -683,15 +683,15 @@
     if dirty:
         git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search('^(.+)-(\\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
```

### Comparing `cdpcli-0.9.9/LICENSE.txt` & `cdpcli-0.9.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/response.py` & `cdpcli-0.9.90/cdpcli/table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,466 +1,411 @@
-try:
-    import http.client as httplib
-except ImportError:
-    import httplib
-import zlib
-import io
-from socket import timeout as SocketTimeout
-
-from ._collections import HTTPHeaderDict
-from .exceptions import (
-    ProtocolError, DecodeError, ReadTimeoutError, ResponseNotChunked
-)
-from .packages.six import string_types as basestring, binary_type, PY3
-from .connection import HTTPException, BaseSSLError
-from .util.response import is_fp_closed
-
-
-class DeflateDecoder(object):
-
-    def __init__(self):
-        self._first_try = True
-        self._data = binary_type()
-        self._obj = zlib.decompressobj()
-
-    def __getattr__(self, name):
-        return getattr(self._obj, name)
-
-    def decompress(self, data):
-        if not data:
-            return data
-
-        if not self._first_try:
-            return self._obj.decompress(data)
-
-        self._data += data
-        try:
-            return self._obj.decompress(data)
-        except zlib.error:
-            self._first_try = False
-            self._obj = zlib.decompressobj(-zlib.MAX_WBITS)
-            try:
-                return self.decompress(self._data)
-            finally:
-                self._data = None
-
-
-class GzipDecoder(object):
-
-    def __init__(self):
-        self._obj = zlib.decompressobj(16 + zlib.MAX_WBITS)
-
-    def __getattr__(self, name):
-        return getattr(self._obj, name)
+# Copyright 2012-2013 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+#
+# Modifications made by Cloudera are:
+#     Copyright (c) 2016 Cloudera, Inc. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License"). You
+# may not use this file except in compliance with the License. A copy of
+# the License is located at
+#
+#     http://aws.amazon.com/apache2.0/
+#
+# or in the "license" file accompanying this file. This file is
+# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
+# ANY KIND, either express or implied. See the License for the specific
+# language governing permissions and limitations under the License.
+
+import os
+import struct
+import sys
+
+from cdpcli.compat import six
+import colorama
+
+
+def determine_terminal_width(default_width=80):
+    # If we can't detect the terminal width, the default_width is returned.
+    try:
+        from termios import TIOCGWINSZ
+        from fcntl import ioctl
+    except ImportError:
+        return default_width
+    try:
+        height, width = struct.unpack('hhhh', ioctl(sys.stdout,
+                                                    TIOCGWINSZ, '\000' * 8))[0:2]
+    except Exception:
+        return default_width
+    else:
+        return width
+
+
+def is_a_tty():
+    try:
+        return os.isatty(sys.stdout.fileno())
+    except Exception:
+        return False
 
-    def decompress(self, data):
-        if not data:
-            return data
-        return self._obj.decompress(data)
 
+def center_text(text, length=80, left_edge='|', right_edge='|',
+                text_length=None):
+    """Center text with specified edge chars.
+
+    You can pass in the length of the text as an arg, otherwise it is computed
+    automatically for you.  This can allow you to center a string not based
+    on it's literal length (useful if you're using ANSI codes).
+    """
+    # postcondition: len(returned_text) == length
+    if text_length is None:
+        text_length = len(text)
+    output = []
+    char_start = (length // 2) - (text_length // 2) - 1
+    output.append(left_edge + ' ' * char_start + text)
+    length_so_far = len(left_edge) + char_start + text_length
+    right_side_spaces = length - len(right_edge) - length_so_far
+    output.append(' ' * right_side_spaces)
+    output.append(right_edge)
+    final = ''.join(output)
+    return final
+
+
+def align_left(text, length, left_edge='|', right_edge='|', text_length=None,
+               left_padding=2):
+    """Left align text."""
+    # postcondition: len(returned_text) == length
+    if text_length is None:
+        text_length = len(text)
+    computed_length = (
+        text_length + left_padding + len(left_edge) + len(right_edge))
+    if length - computed_length >= 0:
+        padding = left_padding
+    else:
+        padding = 0
+    output = []
+    length_so_far = 0
+    output.append(left_edge)
+    length_so_far += len(left_edge)
+    output.append(' ' * padding)
+    length_so_far += padding
+    output.append(text)
+    length_so_far += text_length
+    output.append(' ' * (length - length_so_far - len(right_edge)))
+    output.append(right_edge)
+    return ''.join(output)
+
+
+def convert_to_vertical_table(sections):
+    # Any section that only has a single row is
+    # inverted, so:
+    # header1 | header2 | header3
+    # val1    | val2    | val2
+    #
+    # becomes:
+    #
+    # header1 | val1
+    # header2 | val2
+    # header3 | val3
+    for i, section in enumerate(sections):
+        if len(section.rows) == 1 and section.headers:
+            headers = section.headers
+            new_section = Section()
+            new_section.title = section.title
+            new_section.indent_level = section.indent_level
+            for header, element in zip(headers, section.rows[0]):
+                new_section.add_row([header, element])
+            sections[i] = new_section
+
+
+class IndentedStream(object):
+    def __init__(self, stream, indent_level, left_indent_char='|',
+                 right_indent_char='|'):
+        self._stream = stream
+        self._indent_level = indent_level
+        self._left_indent_char = left_indent_char
+        self._right_indent_char = right_indent_char
+
+    def write(self, text):
+        self._stream.write(self._left_indent_char * self._indent_level)
+        if text.endswith('\n'):
+            self._stream.write(text[:-1])
+            self._stream.write(self._right_indent_char * self._indent_level)
+            self._stream.write('\n')
+        else:
+            self._stream.write(text)
 
-def _get_decoder(mode):
-    if mode == 'gzip':
-        return GzipDecoder()
+    def __getattr__(self, attr):
+        return getattr(self._stream, attr)
 
-    return DeflateDecoder()
 
+class Styler(object):
+    def style_title(self, text):
+        return text
 
-class HTTPResponse(io.IOBase):
-    """
-    HTTP Response container.
+    def style_header_column(self, text):
+        return text
 
-    Backwards-compatible to httplib's HTTPResponse but the response ``body`` is
-    loaded and decoded on-demand when the ``data`` property is accessed.  This
-    class is also compatible with the Python standard library's :mod:`io`
-    module, and can hence be treated as a readable object in the context of that
-    framework.
-
-    Extra parameters for behaviour not present in httplib.HTTPResponse:
-
-    :param preload_content:
-        If True, the response's body will be preloaded during construction.
-
-    :param decode_content:
-        If True, attempts to decode specific content-encoding's based on headers
-        (like 'gzip' and 'deflate') will be skipped and raw data will be used
-        instead.
-
-    :param original_response:
-        When this HTTPResponse wrapper is generated from an httplib.HTTPResponse
-        object, it's convenient to include the original for debug purposes. It's
-        otherwise unused.
-    """
+    def style_row_element(self, text):
+        return text
 
-    CONTENT_DECODERS = ['gzip', 'deflate']
-    REDIRECT_STATUSES = [301, 302, 303, 307, 308]
+    def style_indentation_char(self, text):
+        return text
 
-    def __init__(self, body='', headers=None, status=0, version=0, reason=None,
-                 strict=0, preload_content=True, decode_content=True,
-                 original_response=None, pool=None, connection=None):
 
-        if isinstance(headers, HTTPHeaderDict):
-            self.headers = headers
+class ColorizedStyler(Styler):
+    def __init__(self):
+        # `autoreset` allows us to not have to sent reset sequences for every
+        # string. `strip` lets us preserve color when redirecting.
+        colorama.init(autoreset=True, strip=False)
+
+    def style_title(self, text):
+        # Originally bold + underline
+        return text
+
+    def style_header_column(self, text):
+        # Originally underline
+        return text
+
+    def style_row_element(self, text):
+        return (colorama.Style.BRIGHT + colorama.Fore.BLUE +
+                text + colorama.Style.RESET_ALL)
+
+    def style_indentation_char(self, text):
+        return (colorama.Style.DIM + colorama.Fore.YELLOW +
+                text + colorama.Style.RESET_ALL)
+
+
+class MultiTable(object):
+    def __init__(self, terminal_width=None, initial_section=True,
+                 column_separator='|', terminal=None,
+                 styler=None, auto_reformat=True):
+        self._auto_reformat = auto_reformat
+        if initial_section:
+            self._current_section = Section()
+            self._sections = [self._current_section]
         else:
-            self.headers = HTTPHeaderDict(headers)
-        self.status = status
-        self.version = version
-        self.reason = reason
-        self.strict = strict
-        self.decode_content = decode_content
-
-        self._decoder = None
-        self._body = None
-        self._fp = None
-        self._original_response = original_response
-        self._fp_bytes_read = 0
-
-        if body and isinstance(body, (basestring, binary_type)):
-            self._body = body
-
-        self._pool = pool
-        self._connection = connection
-
-        if hasattr(body, 'read'):
-            self._fp = body
-
-        # Are we using the chunked-style of transfer encoding?
-        self.chunked = False
-        self.chunk_left = None
-        tr_enc = self.headers.get('transfer-encoding', '').lower()
-        # Don't incur the penalty of creating a list and then discarding it
-        encodings = (enc.strip() for enc in tr_enc.split(","))
-        if "chunked" in encodings:
-            self.chunked = True
-
-        # We certainly don't want to preload content when the response is chunked.
-        if not self.chunked and preload_content and not self._body:
-            self._body = self.read(decode_content=decode_content)
-
-    def get_redirect_location(self):
-        """
-        Should we redirect and where to?
-
-        :returns: Truthy redirect location string if we got a redirect status
-            code and valid location. ``None`` if redirect status and no
-            location. ``False`` if not a redirect status code.
-        """
-        if self.status in self.REDIRECT_STATUSES:
-            return self.headers.get('location')
-
-        return False
+            self._current_section = None
+            self._sections = []
+        if styler is None:
+            # Move out to factory.
+            if is_a_tty():
+                self._styler = ColorizedStyler()
+            else:
+                self._styler = Styler()
+        else:
+            self._styler = styler
+        self._rendering_index = 0
+        self._column_separator = column_separator
+        if terminal_width is None:
+            self._terminal_width = determine_terminal_width()
+
+    def add_title(self, title):
+        self._current_section.add_title(title)
+
+    def add_row_header(self, headers):
+        self._current_section.add_header(headers)
+
+    def add_row(self, row_elements):
+        self._current_section.add_row(row_elements)
+
+    def new_section(self, title, indent_level=0):
+        self._current_section = Section()
+        self._sections.append(self._current_section)
+        self._current_section.add_title(title)
+        self._current_section.indent_level = indent_level
+
+    def render(self, stream):
+        max_width = self._calculate_max_width()
+        should_convert_table = self._determine_conversion_needed(max_width)
+        if should_convert_table:
+            convert_to_vertical_table(self._sections)
+            max_width = self._calculate_max_width()
+        stream.write('-' * max_width + '\n')
+        for section in self._sections:
+            self._render_section(section, max_width, stream)
+
+    def _determine_conversion_needed(self, max_width):
+        # If we don't know the width of the controlling terminal,
+        # then we don't try to resize the table.
+        if max_width > self._terminal_width:
+            return self._auto_reformat
+
+    def _calculate_max_width(self):
+        max_width = max(s.total_width(padding=4, with_border=True,
+                                      outer_padding=s.indent_level)
+                        for s in self._sections)
+        return max_width
+
+    def _render_section(self, section, max_width, stream):
+        stream = IndentedStream(stream, section.indent_level,
+                                self._styler.style_indentation_char('|'),
+                                self._styler.style_indentation_char('|'))
+        max_width -= (section.indent_level * 2)
+        self._render_title(section, max_width, stream)
+        self._render_column_titles(section, max_width, stream)
+        self._render_rows(section, max_width, stream)
+
+    def _render_title(self, section, max_width, stream):
+        # The title consists of:
+        # title        :  |   This is the title      |
+        # bottom_border:  ----------------------------
+        if section.title:
+            title = self._styler.style_title(section.title)
+            stream.write(center_text(title, max_width, '|', '|',
+                                     len(section.title)) + '\n')
+            if not section.headers and not section.rows:
+                stream.write('+%s+' % ('-' * (max_width - 2)) + '\n')
 
-    def release_conn(self):
-        if not self._pool or not self._connection:
+    def _render_column_titles(self, section, max_width, stream):
+        if not section.headers:
             return
+        # In order to render the column titles we need to know
+        # the width of each of the columns.
+        widths = section.calculate_column_widths(padding=4,
+                                                 max_width=max_width)
+        # TODO: Built a list instead of +=, it's more efficient.
+        current = ''
+        length_so_far = 0
+        # The first cell needs both left and right edges '|  foo  |'
+        # while subsequent cells only need right edges '  foo  |'.
+        first = True
+        for width, header in zip(widths, section.headers):
+            stylized_header = self._styler.style_header_column(header)
+            if first:
+                left_edge = '|'
+                first = False
+            else:
+                left_edge = ''
+            current += center_text(text=stylized_header, length=width,
+                                   left_edge=left_edge, right_edge='|',
+                                   text_length=len(header))
+            length_so_far += width
+        self._write_line_break(stream, widths)
+        stream.write(current + '\n')
+
+    def _write_line_break(self, stream, widths):
+        # Write out something like:
+        # +-------+---------+---------+
+        parts = []
+        first = True
+        for width in widths:
+            if first:
+                parts.append('+%s+' % ('-' * (width - 2)))
+                first = False
+            else:
+                parts.append('%s+' % ('-' * (width - 1)))
+        parts.append('\n')
+        stream.write(''.join(parts))
 
-        self._pool._put_conn(self._connection)
-        self._connection = None
-
-    @property
-    def data(self):
-        # For backwords-compat with earlier urllib3 0.4 and earlier.
-        if self._body:
-            return self._body
-
-        if self._fp:
-            return self.read(cache_content=True)
-
-    def tell(self):
-        """
-        Obtain the number of bytes pulled over the wire so far. May differ from
-        the amount of content returned by :meth:``HTTPResponse.read`` if bytes
-        are encoded on the wire (e.g, compressed).
-        """
-        return self._fp_bytes_read
-
-    def _init_decoder(self):
-        """
-        Set-up the _decoder attribute if necessar.
-        """
-        # Note: content-encoding value should be case-insensitive, per RFC 7230
-        # Section 3.2
-        content_encoding = self.headers.get('content-encoding', '').lower()
-        if self._decoder is None and content_encoding in self.CONTENT_DECODERS:
-            self._decoder = _get_decoder(content_encoding)
-
-    def _decode(self, data, decode_content, flush_decoder):
-        """
-        Decode the data passed in and potentially flush the decoder.
-        """
-        try:
-            if decode_content and self._decoder:
-                data = self._decoder.decompress(data)
-        except (IOError, zlib.error) as e:
-            content_encoding = self.headers.get('content-encoding', '').lower()
-            raise DecodeError(
-                "Received response with content-encoding: %s, but "
-                "failed to decode it." % content_encoding, e)
-
-        if flush_decoder and decode_content and self._decoder:
-            buf = self._decoder.decompress(binary_type())
-            data += buf + self._decoder.flush()
-
-        return data
-
-    def read(self, amt=None, decode_content=None, cache_content=False):
-        """
-        Similar to :meth:`httplib.HTTPResponse.read`, but with two additional
-        parameters: ``decode_content`` and ``cache_content``.
-
-        :param amt:
-            How much of the content to read. If specified, caching is skipped
-            because it doesn't make sense to cache partial content as the full
-            response.
-
-        :param decode_content:
-            If True, will attempt to decode the body based on the
-            'content-encoding' header.
-
-        :param cache_content:
-            If True, will save the returned data such that the same result is
-            returned despite of the state of the underlying file object. This
-            is useful if you want the ``.data`` property to continue working
-            after having ``.read()`` the file object. (Overridden if ``amt`` is
-            set.)
-        """
-        self._init_decoder()
-        if decode_content is None:
-            decode_content = self.decode_content
-
-        if self._fp is None:
+    def _render_rows(self, section, max_width, stream):
+        if not section.rows:
             return
-
-        flush_decoder = False
-
-        try:
-            try:
-                if amt is None:
-                    # cStringIO doesn't like amt=None
-                    data = self._fp.read()
-                    flush_decoder = True
+        widths = section.calculate_column_widths(padding=4,
+                                                 max_width=max_width)
+        if not widths:
+            return
+        self._write_line_break(stream, widths)
+        for row in section.rows:
+            # TODO: Built the string in a list then join instead of using +=,
+            # it's more efficient.
+            current = ''
+            length_so_far = 0
+            first = True
+            for width, element in zip(widths, row):
+                if first:
+                    left_edge = '|'
+                    first = False
                 else:
-                    cache_content = False
-                    data = self._fp.read(amt)
-                    if amt != 0 and not data:  # Platform-specific: Buggy versions of Python.
-                        # Close the connection when no data is returned
-                        #
-                        # This is redundant to what httplib/http.client _should_
-                        # already do.  However, versions of python released before
-                        # December 15, 2012 (http://bugs.python.org/issue16298) do
-                        # not properly close the connection in all cases. There is
-                        # no harm in redundantly calling close.
-                        self._fp.close()
-                        flush_decoder = True
-
-            except SocketTimeout:
-                # FIXME: Ideally we'd like to include the url in the ReadTimeoutError but
-                # there is yet no clean way to get at it from this context.
-                raise ReadTimeoutError(self._pool, None, 'Read timed out.')
-
-            except BaseSSLError as e:
-                # FIXME: Is there a better way to differentiate between SSLErrors?
-                if 'read operation timed out' not in str(e):  # Defensive:
-                    # This shouldn't happen but just in case we're missing an edge
-                    # case, let's avoid swallowing SSL errors.
-                    raise
-
-                raise ReadTimeoutError(self._pool, None, 'Read timed out.')
-
-            except HTTPException as e:
-                # This includes IncompleteRead.
-                raise ProtocolError('Connection broken: %r' % e, e)
-
-            self._fp_bytes_read += len(data)
-
-            data = self._decode(data, decode_content, flush_decoder)
-
-            if cache_content:
-                self._body = data
-
-            return data
-
-        finally:
-            if self._original_response and self._original_response.isclosed():
-                self.release_conn()
-
-    def stream(self, amt=2**16, decode_content=None):
-        """
-        A generator wrapper for the read() method. A call will block until
-        ``amt`` bytes have been read from the connection or until the
-        connection is closed.
-
-        :param amt:
-            How much of the content to read. The generator will return up to
-            much data per iteration, but may return less. This is particularly
-            likely when using compressed data. However, the empty string will
-            never be returned.
-
-        :param decode_content:
-            If True, will attempt to decode the body based on the
-            'content-encoding' header.
-        """
-        if self.chunked:
-            for line in self.read_chunked(amt, decode_content=decode_content):
-                yield line
-        else:
-            while not is_fp_closed(self._fp):
-                data = self.read(amt=amt, decode_content=decode_content)
+                    left_edge = ''
+                stylized = self._styler.style_row_element(element)
+                current += align_left(text=stylized, length=width,
+                                      left_edge=left_edge,
+                                      right_edge=self._column_separator,
+                                      text_length=len(element))
+                length_so_far += width
+            stream.write(current + '\n')
+        self._write_line_break(stream, widths)
 
-                if data:
-                    yield data
 
-    @classmethod
-    def from_httplib(ResponseCls, r, **response_kw):
-        """
-        Given an :class:`httplib.HTTPResponse` instance ``r``, return a
-        corresponding :class:`urllib3.response.HTTPResponse` object.
-
-        Remaining parameters are passed to the HTTPResponse constructor, along
-        with ``original_response=r``.
-        """
-        headers = r.msg
-        if not isinstance(headers, HTTPHeaderDict):
-            if PY3: # Python 3
-                headers = HTTPHeaderDict(headers.items())
-            else: # Python 2
-                headers = HTTPHeaderDict.from_httplib(headers)
-
-        # HTTPResponse objects in Python 3 don't have a .strict attribute
-        strict = getattr(r, 'strict', 0)
-        resp = ResponseCls(body=r,
-                           headers=headers,
-                           status=r.status,
-                           version=r.version,
-                           reason=r.reason,
-                           strict=strict,
-                           original_response=r,
-                           **response_kw)
-        return resp
-
-    # Backwards-compatibility methods for httplib.HTTPResponse
-    def getheaders(self):
-        return self.headers
-
-    def getheader(self, name, default=None):
-        return self.headers.get(name, default)
-
-    # Overrides from io.IOBase
-    def close(self):
-        if not self.closed:
-            self._fp.close()
-
-    @property
-    def closed(self):
-        if self._fp is None:
-            return True
-        elif hasattr(self._fp, 'closed'):
-            return self._fp.closed
-        elif hasattr(self._fp, 'isclosed'):  # Python 2
-            return self._fp.isclosed()
-        else:
-            return True
-
-    def fileno(self):
-        if self._fp is None:
-            raise IOError("HTTPResponse has no file to get a fileno from")
-        elif hasattr(self._fp, "fileno"):
-            return self._fp.fileno()
+class Section(object):
+    def __init__(self):
+        self.title = ''
+        self.headers = []
+        self.rows = []
+        self.indent_level = 0
+        self._num_cols = None
+        self._max_widths = []
+
+    def __repr__(self):
+        return ("Section(title=%s, headers=%s, indent_level=%s, num_rows=%s)" %
+                (self.title, self.headers, self.indent_level, len(self.rows)))
+
+    def calculate_column_widths(self, padding=0, max_width=None):
+        # postcondition: sum(widths) == max_width
+        unscaled_widths = [w + padding for w in self._max_widths]
+        if max_width is None:
+            return unscaled_widths
+        if not unscaled_widths:
+            return unscaled_widths
         else:
-            raise IOError("The file-like object this HTTPResponse is wrapped "
-                          "around has no file descriptor")
-
-    def flush(self):
-        if self._fp is not None and hasattr(self._fp, 'flush'):
-            return self._fp.flush()
-
-    def readable(self):
-        # This method is required for `io` module compatibility.
-        return True
-
-    def readinto(self, b):
-        # This method is required for `io` module compatibility.
-        temp = self.read(len(b))
-        if len(temp) == 0:
-            return 0
+            # Compute scale factor for max_width.
+            scale_factor = max_width / float(sum(unscaled_widths))
+            scaled = [int(round(scale_factor * w)) for w in unscaled_widths]
+            # Once we've scaled the columns, we may be slightly over/under
+            # the amount we need so we have to adjust the columns.
+            off_by = sum(scaled) - max_width
+            while off_by != 0:
+                iter_order = range(len(scaled))
+                if off_by < 0:
+                    iter_order = reversed(iter_order)
+                for i in iter_order:
+                    if off_by > 0:
+                        scaled[i] -= 1
+                        off_by -= 1
+                    else:
+                        scaled[i] += 1
+                        off_by += 1
+                    if off_by == 0:
+                        break
+            return scaled
+
+    def total_width(self, padding=0, with_border=False, outer_padding=0):
+        total = 0
+        # One char on each side == 2 chars total to the width.
+        border_padding = 2
+        for w in self.calculate_column_widths():
+            total += w + padding
+        if with_border:
+            total += border_padding
+        total += outer_padding + outer_padding
+        return max(len(self.title) + border_padding + outer_padding +
+                   outer_padding, total)
+
+    def add_title(self, title):
+        self.title = title
+
+    def add_header(self, headers):
+        self._update_max_widths(headers)
+        if self._num_cols is None:
+            self._num_cols = len(headers)
+        self.headers = self._format_headers(headers)
+
+    def _format_headers(self, headers):
+        return headers
+
+    def add_row(self, row):
+        if self._num_cols is None:
+            self._num_cols = len(row)
+        if len(row) != self._num_cols:
+            raise ValueError("Row should have %s elements, instead "
+                             "it has %s" % (self._num_cols, len(row)))
+        row = self._format_row(row)
+        self.rows.append(row)
+        self._update_max_widths(row)
+
+    def _format_row(self, row):
+        return [six.text_type(r) for r in row]
+
+    def _update_max_widths(self, row):
+        if not self._max_widths:
+            self._max_widths = [len(el) for el in row]
         else:
-            b[:len(temp)] = temp
-            return len(temp)
-
-    def _update_chunk_length(self):
-        # First, we'll figure out length of a chunk and then
-        # we'll try to read it from socket.
-        if self.chunk_left is not None:
-            return
-        line = self._fp.fp.readline()
-        line = line.split(b';', 1)[0]
-        try:
-            self.chunk_left = int(line, 16)
-        except ValueError:
-            # Invalid chunked protocol response, abort.
-            self.close()
-            raise httplib.IncompleteRead(line)
-
-    def _handle_chunk(self, amt):
-        returned_chunk = None
-        if amt is None:
-            chunk = self._fp._safe_read(self.chunk_left)
-            returned_chunk = chunk
-            self._fp._safe_read(2)  # Toss the CRLF at the end of the chunk.
-            self.chunk_left = None
-        elif amt < self.chunk_left:
-            value = self._fp._safe_read(amt)
-            self.chunk_left = self.chunk_left - amt
-            returned_chunk = value
-        elif amt == self.chunk_left:
-            value = self._fp._safe_read(amt)
-            self._fp._safe_read(2)  # Toss the CRLF at the end of the chunk.
-            self.chunk_left = None
-            returned_chunk = value
-        else:  # amt > self.chunk_left
-            returned_chunk = self._fp._safe_read(self.chunk_left)
-            self._fp._safe_read(2)  # Toss the CRLF at the end of the chunk.
-            self.chunk_left = None
-        return returned_chunk
-
-    def read_chunked(self, amt=None, decode_content=None):
-        """
-        Similar to :meth:`HTTPResponse.read`, but with an additional
-        parameter: ``decode_content``.
-
-        :param decode_content:
-            If True, will attempt to decode the body based on the
-            'content-encoding' header.
-        """
-        self._init_decoder()
-        # FIXME: Rewrite this method and make it a class with a better structured logic.
-        if not self.chunked:
-            raise ResponseNotChunked("Response is not chunked. "
-                "Header 'transfer-encoding: chunked' is missing.")
-
-        if self._original_response and self._original_response._method.upper() == 'HEAD':
-            # Don't bother reading the body of a HEAD request.
-            # FIXME: Can we do this somehow without accessing private httplib _method?
-            self._original_response.close()
-            return
-
-        while True:
-            self._update_chunk_length()
-            if self.chunk_left == 0:
-                break
-            chunk = self._handle_chunk(amt)
-            yield self._decode(chunk, decode_content=decode_content,
-                               flush_decoder=True)
-
-        # Chunk content ends with \r\n: discard it.
-        while True:
-            line = self._fp.fp.readline()
-            if not line:
-                # Some sites may not end with '\r\n'.
-                break
-            if line == b'\r\n':
-                break
-
-        # We read everything; close the "file".
-        if self._original_response:
-            self._original_response.close()
-        self.release_conn()
+            for i, el in enumerate(row):
+                self._max_widths[i] = max(len(el), self._max_widths[i])
```

### Comparing `cdpcli-0.9.9/cdpcli/thirdparty/requests/utils.py` & `cdpcli-0.9.90/cdpcli/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,707 +1,537 @@
-# -*- coding: utf-8 -*-
+# Copyright 2012-2013 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+#
+# Modifications made by Cloudera are:
+#     Copyright (c) 2016 Cloudera, Inc. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License"). You
+# may not use this file except in compliance with the License. A copy of
+# the License is located at
+#
+#     http://aws.amazon.com/apache2.0/
+#
+# or in the "license" file accompanying this file. This file is
+# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
+# ANY KIND, either express or implied. See the License for the specific
+# language governing permissions and limitations under the License.
 
-"""
-requests.utils
-~~~~~~~~~~~~~~
-
-This module provides utility functions that are used within Requests
-that are also useful for external consumption.
-
-"""
-
-import cgi
-import codecs
-import collections
-import io
+import copy
 import os
-import platform
-import re
-import sys
-import socket
-import struct
-import warnings
-
-from . import __version__
-from . import certs
-from .compat import parse_http_list as _parse_list_header
-from .compat import (quote, urlparse, bytes, str, OrderedDict, unquote, is_py2,
-                     builtin_str, getproxies, proxy_bypass, urlunparse,
-                     basestring)
-from .cookies import RequestsCookieJar, cookiejar_from_dict
-from .structures import CaseInsensitiveDict
-from .exceptions import InvalidURL
-
-_hush_pyflakes = (RequestsCookieJar,)
-
-NETRC_FILES = ('.netrc', '_netrc')
-
-DEFAULT_CA_BUNDLE_PATH = certs.where()
-
-
-def dict_to_sequence(d):
-    """Returns an internal sequence dictionary update."""
+import uuid
 
-    if hasattr(d, 'items'):
-        d = d.items()
-
-    return d
-
-
-def super_len(o):
-    if hasattr(o, '__len__'):
-        return len(o)
-
-    if hasattr(o, 'len'):
-        return o.len
-
-    if hasattr(o, 'fileno'):
-        try:
-            fileno = o.fileno()
-        except io.UnsupportedOperation:
-            pass
+from cdpcli import credentials, DEFAULT_PROFILE_NAME
+from cdpcli import xform_name
+from cdpcli.auth import AccessTokenAuth
+from cdpcli.auth import ECDSAv1Auth
+from cdpcli.auth import Ed25519v1Auth
+from cdpcli.auth import RSAv1Auth
+from cdpcli.cdprequest import prepare_request_dict
+from cdpcli.configloader import load_config, raw_config_parse
+from cdpcli.endpoint import DEFAULT_TIMEOUT
+from cdpcli.exceptions import ClientError, ConfigNotFound, ProfileNotFound
+from cdpcli.exceptions import OperationNotPageableError
+from cdpcli.model import ServiceModel
+from cdpcli.paginate import Paginator
+from cdpcli.serialize import create_serializer
+from cdpcli.signers import RequestSigner
+from cdpcli.utils import get_service_module_name
+
+ALTUS_REQUEST_ID_HEADER = 'x-altus-request-id'
+CDP_REQUEST_ID_HEADER = 'x-cdp-request-id'
+
+
+class ClientCreator(object):
+
+    def __init__(self,
+                 loader,
+                 context,
+                 endpoint_creator,
+                 user_agent_header,
+                 response_parser_factory,
+                 retryhandler):
+        self._loader = loader
+        self._context = context
+        self._endpoint_creator = endpoint_creator
+        self._user_agent_header = user_agent_header
+        self._response_parser_factory = response_parser_factory
+        self._retryhandler = retryhandler
+
+    @property
+    def context(self):
+        return self._context
+
+    def create_client(self,
+                      service_name,
+                      explicit_endpoint_url,
+                      region,
+                      tls_verification,
+                      credentials,
+                      client_config=None):
+        service_model = self._load_service_model(service_name)
+        cls = self._create_client_class(service_name, service_model)
+        client_args = self._get_client_args(service_model,
+                                            explicit_endpoint_url,
+                                            region,
+                                            tls_verification,
+                                            credentials,
+                                            client_config)
+        return cls(**client_args)
+
+    def _load_service_model(self, service_name):
+        service_data = self._loader.load_service_data(service_name)
+        return ServiceModel(service_data, service_name=service_name)
+
+    def _create_client_class(self, service_name, service_model):
+        class_attributes = self._create_methods(service_model)
+        py_name_to_operation_name = self._create_name_mapping(service_model)
+        class_attributes['_PY_TO_OP_NAME'] = py_name_to_operation_name
+        bases = [BaseClient]
+        class_name = get_service_module_name(service_model)
+        cls = type(str(class_name), tuple(bases), class_attributes)
+        return cls
+
+    def _get_client_args(self,
+                         service_model,
+                         explicit_endpoint_url,
+                         region,
+                         tls_verification,
+                         credentials,
+                         client_config):
+        """Get keyword arguments for constructing a client object.
+        """
+        serializer = create_serializer()
+        if client_config is not None:
+            connect_timeout = client_config.connect_timeout
+            if connect_timeout <= 0:
+                connect_timeout = None
+            read_timeout = client_config.read_timeout
+            if read_timeout <= 0:
+                read_timeout = None
         else:
-            return os.fstat(fileno).st_size
-
-    if hasattr(o, 'getvalue'):
-        # e.g. BytesIO, cStringIO.StringIO
-        return len(o.getvalue())
-
-
-def get_netrc_auth(url):
-    """Returns the Requests tuple auth for a given url from netrc."""
+            connect_timeout = DEFAULT_TIMEOUT
+            read_timeout = DEFAULT_TIMEOUT
+        endpoint = self._endpoint_creator.create_endpoint(
+            service_model,
+            explicit_endpoint_url,
+            self._context.get_scoped_config(),
+            region,
+            self._response_parser_factory,
+            tls_verification,
+            (connect_timeout, read_timeout),
+            self._retryhandler)
+        if AccessTokenAuth.is_access_token(credentials.access_token):
+            auth_method = AccessTokenAuth.AUTH_METHOD_NAME
+        elif Ed25519v1Auth.detect_private_key(credentials.private_key):
+            auth_method = Ed25519v1Auth.AUTH_METHOD_NAME
+        elif ECDSAv1Auth.detect_private_key(credentials.private_key):
+            auth_method = ECDSAv1Auth.AUTH_METHOD_NAME
+        else:
+            auth_method = RSAv1Auth.AUTH_METHOD_NAME
+        additional_headers = dict()
+        request_headers_string = self._context.get_scoped_config().get(
+            'request_headers', '')
+        for header_string in request_headers_string.split(','):
+            header_string = header_string.strip()
+            if header_string == '':
+                continue
+            name, value = header_string.split('=', 1)
+            if value == 'generate::uuid':
+                value = str(uuid.uuid4())
+            additional_headers[name] = value
+        signer = RequestSigner(auth_method, credentials)
+        return {
+            'serializer': serializer,
+            'service_model': service_model,
+            'endpoint': endpoint,
+            'loader': self._loader,
+            'user_agent_header': self._user_agent_header,
+            'additional_headers': additional_headers,
+            'request_signer': signer
+        }
+
+    def _create_methods(self, service_model):
+        op_dict = {}
+        for operation_name in service_model.operation_names:
+            py_operation_name = xform_name(operation_name)
+            op_dict[py_operation_name] = self._create_api_method(
+                py_operation_name, operation_name, service_model)
+        return op_dict
+
+    def _create_name_mapping(self, service_model):
+        mapping = {}
+        for operation_name in service_model.operation_names:
+            py_operation_name = xform_name(operation_name)
+            mapping[py_operation_name] = operation_name
+        return mapping
+
+    def _create_api_method(self, py_operation_name, operation_name, service_model):
+        def _api_call(self, *args, **kwargs):
+            if args:
+                raise TypeError(
+                    "%s() only accepts keyword arguments." % py_operation_name)
+            http, parsed_response = self.make_api_call(operation_name, kwargs)
+            return parsed_response
+
+        _api_call.__name__ = str(py_operation_name)
+        return _api_call
+
+
+class BaseClient(object):
+
+    # This is actually reassigned with the py->op_name mapping when the client
+    # creator creates the subclass.  This value is used because calls such as
+    # client.get_paginator('list_objects') use the snake_case name, but we need
+    # to know the ListObjects form. The xform_name() function does the forward
+    # mapping for ListObjects->list_objects conversion, but this holds the
+    # reverse mapping.
+    _PY_TO_OP_NAME = {}
+
+    def __init__(self,
+                 serializer,
+                 endpoint,
+                 service_model,
+                 loader,
+                 user_agent_header,
+                 additional_headers,
+                 request_signer):
+        self._serializer = serializer
+        self._endpoint = endpoint
+        self._loader = loader
+        self._user_agent_header = user_agent_header
+        self._additional_headers = additional_headers
+        self._request_signer = request_signer
+        self.meta = ClientMeta(service_model, endpoint.host, self._PY_TO_OP_NAME)
+
+    def can_paginate(self, operation_name):
+        actual_operation_name = self._PY_TO_OP_NAME[operation_name]
+        return self._service_model.operation_model(actual_operation_name).can_paginate
+
+    def get_paginator(self, operation_name):
+        if not self.can_paginate(operation_name):
+            raise OperationNotPageableError(operation_name=operation_name)
+        actual_operation_name = self._PY_TO_OP_NAME[operation_name]
+        operation_model = self._service_model.operation_model(actual_operation_name)
+        method = getattr(self, operation_name)
+        return Paginator(method, operation_model)
+
+    @property
+    def _service_model(self):
+        return self.meta.service_model
+
+    def make_api_call(self, operation_name, api_params,
+                      allow_redirects=True):
+        operation_model = self._service_model.operation_model(operation_name)
+        request_dict = self._serializer.serialize_to_request(api_params, operation_model)
+        return self._make_request(operation_name, operation_model, request_dict,
+                                  allow_redirects)
+
+    def make_request(self, operation_name,
+                     method, url_path, headers, body,
+                     allow_redirects=True):
+        operation_model = self._service_model.operation_model(operation_name)
+        request_dict = {
+            'url_path': url_path,
+            'method': method,
+            'headers': headers,
+            'body': body
+        }
+        return self._make_request(operation_name, operation_model, request_dict,
+                                  allow_redirects)
+
+    def raise_error(self, operation_name, http, parsed_response):
+        request_id = http.headers.get(ALTUS_REQUEST_ID_HEADER) \
+            if ALTUS_REQUEST_ID_HEADER in http.headers \
+            else http.headers.get(CDP_REQUEST_ID_HEADER, 'Unknown')
+        raise ClientError(
+            parsed_response,
+            operation_name,
+            self._service_model.service_name,
+            http.status_code,
+            request_id)
+
+    def _make_request(self, operation_name, operation_model, request_dict,
+                      allow_redirects):
+        prepare_request_dict(request_dict,
+                             endpoint_url=self._endpoint.host,
+                             user_agent_header=self._user_agent_header,
+                             additional_headers=self._additional_headers)
+        http, parsed_response = self._endpoint.make_request(
+            operation_model, request_dict, self._request_signer,
+            allow_redirects=allow_redirects)
+        if allow_redirects and http.status_code >= 300:
+            self.raise_error(operation_name, http, parsed_response)
+        elif not allow_redirects and http.status_code >= 400:
+            self.raise_error(operation_name, http, parsed_response)
+        else:
+            return http, parsed_response
 
-    try:
-        from netrc import netrc, NetrcParseError
 
-        netrc_path = None
+class ClientMeta(object):
 
-        for f in NETRC_FILES:
+    def __init__(self, service_model, endpoint_url, method_to_api_mapping):
+        self._service_model = service_model
+        self._endpoint_url = endpoint_url
+        self._method_to_api_mapping = method_to_api_mapping
+
+    @property
+    def service_model(self):
+        return self._service_model
+
+    @property
+    def endpoint_url(self):
+        return self._endpoint_url
+
+    @property
+    def method_to_api_mapping(self):
+        return self._method_to_api_mapping
+
+
+class Context(object):
+    """
+    The Context object exposes configuration information and credentials into a
+    single, easy-to-use object.
+
+    """
+
+    #: A default dictionary that maps the logical names for context variables
+    #: to the specific environment variables and configuration file names
+    #: that contain the values for these variables.
+    #: When creating a new Context object, you can pass in your own dictionary
+    #: to remap the logical names or to add new logical names.  You can then
+    #: get the current value for these variables by using the
+    #: ``get_config_variable`` method of the :class:`Context` #: class.
+    #: These form the keys of the dictionary.  The values in the dictionary
+    #: are tuples of (<config_name>, <environment variable>, <default value>,
+    #: <conversion func>).
+    #: The conversion func is a function that takes the configuration value
+    #: as an argument and returns the converted value.  If this value is
+    #: None, then the configuration value is returned unmodified.  This
+    #: conversion function can be used to type convert config values to
+    #: values other than the default values of strings.
+    #: The ``profile`` and ``config_file`` variables should always have a
+    #: None value for the first entry in the tuple because it doesn't make
+    #: sense to look inside the config file for the location of the config
+    #: file or for the default profile to use.
+    #: The ``config_name`` is the name to look for in the configuration file,
+    #: the ``env var`` is the OS environment variable (``os.environ``) to
+    #: use, and ``default_value`` is the value to use if no value is otherwise
+    #: found.
+    CONTEXT_VARIABLES = {
+        # logical:  config_file, env_var, default_value, conversion_func
+        'profile': (None, ['CDP_DEFAULT_PROFILE', 'CDP_PROFILE'], None, None),
+        'config_file': (None, 'CDP_CONFIG_FILE', '~/.cdp/config', None),
+        'ca_bundle': ('ca_bundle', 'CDP_CA_BUNDLE', None, None),
+        'api_versions': ('api_versions', None, {}, None),
+        # This is the legacy json configuration file
+        'auth_config': (None, None, None, None),
+        # This is the shared credentials file.
+        'credentials_file': (None, 'CDP_SHARED_CREDENTIALS_FILE',
+                             '~/.cdp/credentials', None),
+        'cdp_region': ('cdp_region', None, None, None),
+        'cdp_endpoint_url': ('cdp_endpoint_url', None, None, None),
+        'endpoint_url': ('endpoint_url', None, None, None),
+        'form_factor': ('form_factor', None, None, None),
+    }
+
+    def __init__(self, profile=None):
+        self.context_var_map = copy.copy(self.CONTEXT_VARIABLES)
+        # The _profile attribute is just used to cache the value
+        # of the current profile to avoid going through the normal
+        # config lookup process each access time.
+        self._profile = None
+        self._config = None
+        self._profile_map = None
+        # This is a dict that stores per context specific config variable
+        # overrides via set_config_variable().
+        self._context_instance_vars = {}
+        if profile is not None:
+            self._context_instance_vars['profile'] = profile
+        self._client_config = None
+
+    @property
+    def profile(self):
+        """
+        Returns the profile if one was set. Can be None.
+        """
+        if self._profile is None:
+            profile = self.get_config_variable('profile')
+            self._profile = profile
+        return self._profile
+
+    @property
+    def effective_profile(self):
+        """
+        Returns the effective profile, cannot be None. If no profile was
+        set the default profile is returned.
+        """
+        profile_name = self.profile
+        if profile_name is None:
+            profile_name = DEFAULT_PROFILE_NAME
+        return profile_name
+
+    @property
+    def full_config(self):
+        """Return the parsed config file.
+        The ``get_config`` method returns the config associated with the
+        specified profile.  This property returns the contents of the
+        **entire** config file.
+        """
+        if self._config is None:
             try:
-                loc = os.path.expanduser('~/{0}'.format(f))
-            except KeyError:
-                # os.path.expanduser can fail when $HOME is undefined and
-                # getpwuid fails. See http://bugs.python.org/issue20164 &
-                # https://github.com/kennethreitz/requests/issues/1846
-                return
-
-            if os.path.exists(loc):
-                netrc_path = loc
-                break
-
-        # Abort early if there isn't one.
-        if netrc_path is None:
-            return
-
-        ri = urlparse(url)
-
-        # Strip port numbers from netloc
-        host = ri.netloc.split(':')[0]
-
-        try:
-            _netrc = netrc(netrc_path).authenticators(host)
-            if _netrc:
-                # Return with login / password
-                login_i = (0 if _netrc[0] else 1)
-                return (_netrc[login_i], _netrc[2])
-        except (NetrcParseError, IOError):
-            # If there was a parsing error or a permissions issue reading the file,
-            # we'll just skip netrc auth
-            pass
-
-    # AppEngine hackiness.
-    except (ImportError, AttributeError):
-        pass
-
-
-def guess_filename(obj):
-    """Tries to guess the filename of the given object."""
-    name = getattr(obj, 'name', None)
-    if (name and isinstance(name, basestring) and name[0] != '<' and
-            name[-1] != '>'):
-        return os.path.basename(name)
-
-
-def from_key_val_list(value):
-    """Take an object and test to see if it can be represented as a
-    dictionary. Unless it can not be represented as such, return an
-    OrderedDict, e.g.,
-
-    ::
-
-        >>> from_key_val_list([('key', 'val')])
-        OrderedDict([('key', 'val')])
-        >>> from_key_val_list('string')
-        ValueError: need more than 1 value to unpack
-        >>> from_key_val_list({'key': 'val'})
-        OrderedDict([('key', 'val')])
-    """
-    if value is None:
-        return None
-
-    if isinstance(value, (str, bytes, bool, int)):
-        raise ValueError('cannot encode objects that are not 2-tuples')
-
-    return OrderedDict(value)
-
-
-def to_key_val_list(value):
-    """Take an object and test to see if it can be represented as a
-    dictionary. If it can be, return a list of tuples, e.g.,
-
-    ::
-
-        >>> to_key_val_list([('key', 'val')])
-        [('key', 'val')]
-        >>> to_key_val_list({'key': 'val'})
-        [('key', 'val')]
-        >>> to_key_val_list('string')
-        ValueError: cannot encode objects that are not 2-tuples.
-    """
-    if value is None:
-        return None
-
-    if isinstance(value, (str, bytes, bool, int)):
-        raise ValueError('cannot encode objects that are not 2-tuples')
-
-    if isinstance(value, collections.Mapping):
-        value = value.items()
-
-    return list(value)
-
-
-# From mitsuhiko/werkzeug (used with permission).
-def parse_list_header(value):
-    """Parse lists as described by RFC 2068 Section 2.
-
-    In particular, parse comma-separated lists where the elements of
-    the list may include quoted-strings.  A quoted-string could
-    contain a comma.  A non-quoted string could have quotes in the
-    middle.  Quotes are removed automatically after parsing.
-
-    It basically works like :func:`parse_set_header` just that items
-    may appear multiple times and case sensitivity is preserved.
-
-    The return value is a standard :class:`list`:
-
-    >>> parse_list_header('token, "quoted value"')
-    ['token', 'quoted value']
-
-    To create a header from the :class:`list` again, use the
-    :func:`dump_header` function.
-
-    :param value: a string with a list header.
-    :return: :class:`list`
-    """
-    result = []
-    for item in _parse_list_header(value):
-        if item[:1] == item[-1:] == '"':
-            item = unquote_header_value(item[1:-1])
-        result.append(item)
-    return result
-
-
-# From mitsuhiko/werkzeug (used with permission).
-def parse_dict_header(value):
-    """Parse lists of key, value pairs as described by RFC 2068 Section 2 and
-    convert them into a python dict:
-
-    >>> d = parse_dict_header('foo="is a fish", bar="as well"')
-    >>> type(d) is dict
-    True
-    >>> sorted(d.items())
-    [('bar', 'as well'), ('foo', 'is a fish')]
-
-    If there is no value for a key it will be `None`:
-
-    >>> parse_dict_header('key_without_value')
-    {'key_without_value': None}
-
-    To create a header from the :class:`dict` again, use the
-    :func:`dump_header` function.
-
-    :param value: a string with a dict header.
-    :return: :class:`dict`
-    """
-    result = {}
-    for item in _parse_list_header(value):
-        if '=' not in item:
-            result[item] = None
-            continue
-        name, value = item.split('=', 1)
-        if value[:1] == value[-1:] == '"':
-            value = unquote_header_value(value[1:-1])
-        result[name] = value
-    return result
-
-
-# From mitsuhiko/werkzeug (used with permission).
-def unquote_header_value(value, is_filename=False):
-    r"""Unquotes a header value.  (Reversal of :func:`quote_header_value`).
-    This does not use the real unquoting but what browsers are actually
-    using for quoting.
-
-    :param value: the header value to unquote.
-    """
-    if value and value[0] == value[-1] == '"':
-        # this is not the real unquoting, but fixing this so that the
-        # RFC is met will result in bugs with internet explorer and
-        # probably some other browsers as well.  IE for example is
-        # uploading files with "C:\foo\bar.txt" as filename
-        value = value[1:-1]
-
-        # if this is a filename and the starting characters look like
-        # a UNC path, then just return the value without quotes.  Using the
-        # replace sequence below on a UNC path has the effect of turning
-        # the leading double slash into a single slash and then
-        # _fix_ie_filename() doesn't work correctly.  See #458.
-        if not is_filename or value[:2] != '\\\\':
-            return value.replace('\\\\', '\\').replace('\\"', '"')
-    return value
-
-
-def dict_from_cookiejar(cj):
-    """Returns a key/value dictionary from a CookieJar.
-
-    :param cj: CookieJar object to extract cookies from.
-    """
-
-    cookie_dict = {}
-
-    for cookie in cj:
-        cookie_dict[cookie.name] = cookie.value
-
-    return cookie_dict
-
-
-def add_dict_to_cookiejar(cj, cookie_dict):
-    """Returns a CookieJar from a key/value dictionary.
-
-    :param cj: CookieJar to insert cookies into.
-    :param cookie_dict: Dict of key/values to insert into CookieJar.
-    """
-
-    cj2 = cookiejar_from_dict(cookie_dict)
-    cj.update(cj2)
-    return cj
-
-
-def get_encodings_from_content(content):
-    """Returns encodings from given content string.
-
-    :param content: bytestring to extract encodings from.
-    """
-    warnings.warn((
-        'In requests 3.0, get_encodings_from_content will be removed. For '
-        'more information, please see the discussion on issue #2266. (This'
-        ' warning should only appear once.)'),
-        DeprecationWarning)
-
-    charset_re = re.compile(r'<meta.*?charset=["\']*(.+?)["\'>]', flags=re.I)
-    pragma_re = re.compile(r'<meta.*?content=["\']*;?charset=(.+?)["\'>]', flags=re.I)
-    xml_re = re.compile(r'^<\?xml.*?encoding=["\']*(.+?)["\'>]')
-
-    return (charset_re.findall(content) +
-            pragma_re.findall(content) +
-            xml_re.findall(content))
-
-
-def get_encoding_from_headers(headers):
-    """Returns encodings from given HTTP Header Dict.
-
-    :param headers: dictionary to extract encoding from.
-    """
-
-    content_type = headers.get('content-type')
-
-    if not content_type:
-        return None
-
-    content_type, params = cgi.parse_header(content_type)
-
-    if 'charset' in params:
-        return params['charset'].strip("'\"")
-
-    if 'text' in content_type:
-        return 'ISO-8859-1'
-
-
-def stream_decode_response_unicode(iterator, r):
-    """Stream decodes a iterator."""
-
-    if r.encoding is None:
-        for item in iterator:
-            yield item
-        return
-
-    decoder = codecs.getincrementaldecoder(r.encoding)(errors='replace')
-    for chunk in iterator:
-        rv = decoder.decode(chunk)
-        if rv:
-            yield rv
-    rv = decoder.decode(b'', final=True)
-    if rv:
-        yield rv
-
-
-def iter_slices(string, slice_length):
-    """Iterate over slices of a string."""
-    pos = 0
-    while pos < len(string):
-        yield string[pos:pos + slice_length]
-        pos += slice_length
-
-
-def get_unicode_from_response(r):
-    """Returns the requested content back in unicode.
-
-    :param r: Response object to get unicode content from.
-
-    Tried:
-
-    1. charset from content-type
-    2. fall back and replace all unicode characters
-
-    """
-    warnings.warn((
-        'In requests 3.0, get_unicode_from_response will be removed. For '
-        'more information, please see the discussion on issue #2266. (This'
-        ' warning should only appear once.)'),
-        DeprecationWarning)
-
-    tried_encodings = []
-
-    # Try charset from content-type
-    encoding = get_encoding_from_headers(r.headers)
-
-    if encoding:
-        try:
-            return str(r.content, encoding)
-        except UnicodeError:
-            tried_encodings.append(encoding)
-
-    # Fall back:
-    try:
-        return str(r.content, encoding, errors='replace')
-    except TypeError:
-        return r.content
-
-
-# The unreserved URI characters (RFC 3986)
-UNRESERVED_SET = frozenset(
-    "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
-    + "0123456789-._~")
-
-
-def unquote_unreserved(uri):
-    """Un-escape any percent-escape sequences in a URI that are unreserved
-    characters. This leaves all reserved, illegal and non-ASCII bytes encoded.
-    """
-    parts = uri.split('%')
-    for i in range(1, len(parts)):
-        h = parts[i][0:2]
-        if len(h) == 2 and h.isalnum():
+                config_file = self.get_config_variable('config_file')
+                self._config = load_config(config_file)
+            except ConfigNotFound:
+                self._config = {'profiles': {}}
             try:
-                c = chr(int(h, 16))
-            except ValueError:
-                raise InvalidURL("Invalid percent-escape sequence: '%s'" % h)
-
-            if c in UNRESERVED_SET:
-                parts[i] = c + parts[i][2:]
-            else:
-                parts[i] = '%' + parts[i]
-        else:
-            parts[i] = '%' + parts[i]
-    return ''.join(parts)
-
-
-def requote_uri(uri):
-    """Re-quote the given URI.
-
-    This function passes the given URI through an unquote/quote cycle to
-    ensure that it is fully and consistently quoted.
-    """
-    safe_with_percent = "!#$%&'()*+,/:;=?@[]~"
-    safe_without_percent = "!#$&'()*+,/:;=?@[]~"
-    try:
-        # Unquote only the unreserved characters
-        # Then quote only illegal characters (do not quote reserved,
-        # unreserved, or '%')
-        return quote(unquote_unreserved(uri), safe=safe_with_percent)
-    except InvalidURL:
-        # We couldn't unquote the given URI, so let's try quoting it, but
-        # there may be unquoted '%'s in the URI. We need to make sure they're
-        # properly quoted so they do not cause issues elsewhere.
-        return quote(uri, safe=safe_without_percent)
-
-
-def address_in_network(ip, net):
-    """
-    This function allows you to check if on IP belongs to a network subnet
-    Example: returns True if ip = 192.168.1.1 and net = 192.168.1.0/24
-             returns False if ip = 192.168.1.1 and net = 192.168.100.0/24
-    """
-    ipaddr = struct.unpack('=L', socket.inet_aton(ip))[0]
-    netaddr, bits = net.split('/')
-    netmask = struct.unpack('=L', socket.inet_aton(dotted_netmask(int(bits))))[0]
-    network = struct.unpack('=L', socket.inet_aton(netaddr))[0] & netmask
-    return (ipaddr & netmask) == (network & netmask)
-
-
-def dotted_netmask(mask):
-    """
-    Converts mask from /xx format to xxx.xxx.xxx.xxx
-    Example: if mask is 24 function returns 255.255.255.0
-    """
-    bits = 0xffffffff ^ (1 << 32 - mask) - 1
-    return socket.inet_ntoa(struct.pack('>I', bits))
-
-
-def is_ipv4_address(string_ip):
-    try:
-        socket.inet_aton(string_ip)
-    except socket.error:
+                # Now we need to inject the profiles from the
+                # credentials file.  We don't actually need the values
+                # in the creds file, only the profile names so that we
+                # can validate the user is not referring to a nonexistent
+                # profile.
+                cred_file = self.get_config_variable('credentials_file')
+                cred_profiles = raw_config_parse(cred_file)
+                for profile in cred_profiles:
+                    cred_vars = cred_profiles[profile]
+                    if profile not in self._config['profiles']:
+                        self._config['profiles'][profile] = cred_vars
+                    else:
+                        self._config['profiles'][profile].update(cred_vars)
+            except ConfigNotFound:
+                pass
+        return self._config
+
+    def _build_profile_map(self):
+        # This will build the profile map if it has not been created,
+        # otherwise it will return the cached value.  The profile map
+        # is a list of profile names, to the config values for the profile.
+        if self._profile_map is None:
+            self._profile_map = self.full_config['profiles']
+        return self._profile_map
+
+    def get_config_variable(self, logical_name,
+                            methods=('instance', 'env', 'config')):
+        """
+        Retrieve the value associated with the specified logical_name
+        from the environment or the config file.  Values found in the
+        environment variable take precedence of values found in the
+        config file.  If no value can be found, a None will be returned.
+
+        :type logical_name: str
+        :param logical_name: The logical name of the context variable
+            you want to retrieve.  This name will be mapped to the
+            appropriate environment variable name for this context as
+            well as the appropriate config file entry.
+
+        :type methods: tuple
+        :param methods: Defines which methods will be used to find
+            the variable value.  By default, all available methods
+            are tried but you can limit which methods are used
+            by supplying a different value to this parameter.
+            Valid choices are: instance|env|config
+
+        :returns: value of variable or None if not defined.
+
+        """
+        # Handle all the short circuit special cases first.
+        if logical_name not in self.context_var_map:
+            return
+        # Do the actual lookups.  We need to handle
+        # 'instance', 'env', and 'config' locations, in that order.
+        value = None
+        var_config = self.context_var_map[logical_name]
+        if self._found_in_instance_vars(methods, logical_name):
+            return self._context_instance_vars[logical_name]
+        elif self._found_in_env(methods, var_config):
+            value = self._retrieve_from_env(var_config[1], os.environ)
+        elif self._found_in_config_file(methods, var_config):
+            value = self.get_scoped_config()[var_config[0]]
+        if value is None:
+            value = var_config[2]
+        if var_config[3] is not None:
+            value = var_config[3](value)
+        return value
+
+    def _found_in_instance_vars(self, methods, logical_name):
+        if 'instance' in methods:
+            return logical_name in self._context_instance_vars
         return False
-    return True
 
-
-def is_valid_cidr(string_network):
-    """Very simple check of the cidr format in no_proxy variable"""
-    if string_network.count('/') == 1:
-        try:
-            mask = int(string_network.split('/')[1])
-        except ValueError:
-            return False
-
-        if mask < 1 or mask > 32:
-            return False
-
-        try:
-            socket.inet_aton(string_network.split('/')[0])
-        except socket.error:
-            return False
-    else:
+    def _found_in_env(self, methods, var_config):
+        return (
+            'env' in methods and
+            var_config[1] is not None and
+            self._retrieve_from_env(var_config[1], os.environ) is not None)
+
+    def _found_in_config_file(self, methods, var_config):
+        if 'config' in methods and var_config[0] is not None:
+            return var_config[0] in self.get_scoped_config()
         return False
-    return True
-
-
-def should_bypass_proxies(url):
-    """
-    Returns whether we should bypass proxies or not.
-    """
-    get_proxy = lambda k: os.environ.get(k) or os.environ.get(k.upper())
-
-    # First check whether no_proxy is defined. If it is, check that the URL
-    # we're getting isn't in the no_proxy list.
-    no_proxy = get_proxy('no_proxy')
-    netloc = urlparse(url).netloc
-
-    if no_proxy:
-        # We need to check whether we match here. We need to see if we match
-        # the end of the netloc, both with and without the port.
-        no_proxy = no_proxy.replace(' ', '').split(',')
-
-        ip = netloc.split(':')[0]
-        if is_ipv4_address(ip):
-            for proxy_ip in no_proxy:
-                if is_valid_cidr(proxy_ip):
-                    if address_in_network(ip, proxy_ip):
-                        return True
-        else:
-            for host in no_proxy:
-                if netloc.endswith(host) or netloc.split(':')[0].endswith(host):
-                    # The URL does match something in no_proxy, so we don't want
-                    # to apply the proxies on this URL.
-                    return True
-
-    # If the system proxy settings indicate that this URL should be bypassed,
-    # don't proxy.
-    # The proxy_bypass function is incredibly buggy on OS X in early versions
-    # of Python 2.6, so allow this call to fail. Only catch the specific
-    # exceptions we've seen, though: this call failing in other ways can reveal
-    # legitimate problems.
-    try:
-        bypass = proxy_bypass(netloc)
-    except (TypeError, socket.gaierror):
-        bypass = False
-
-    if bypass:
-        return True
-
-    return False
-
-def get_environ_proxies(url):
-    """Return a dict of environment proxies."""
-    if should_bypass_proxies(url):
-        return {}
-    else:
-        return getproxies()
-
-
-def default_user_agent(name="python-requests"):
-    """Return a string representing the default user agent."""
-    _implementation = platform.python_implementation()
-
-    if _implementation == 'CPython':
-        _implementation_version = platform.python_version()
-    elif _implementation == 'PyPy':
-        _implementation_version = '%s.%s.%s' % (sys.pypy_version_info.major,
-                                                sys.pypy_version_info.minor,
-                                                sys.pypy_version_info.micro)
-        if sys.pypy_version_info.releaselevel != 'final':
-            _implementation_version = ''.join([_implementation_version, sys.pypy_version_info.releaselevel])
-    elif _implementation == 'Jython':
-        _implementation_version = platform.python_version()  # Complete Guess
-    elif _implementation == 'IronPython':
-        _implementation_version = platform.python_version()  # Complete Guess
-    else:
-        _implementation_version = 'Unknown'
-
-    try:
-        p_system = platform.system()
-        p_release = platform.release()
-    except IOError:
-        p_system = 'Unknown'
-        p_release = 'Unknown'
-
-    return " ".join(['%s/%s' % (name, __version__),
-                     '%s/%s' % (_implementation, _implementation_version),
-                     '%s/%s' % (p_system, p_release)])
-
-
-def default_headers():
-    return CaseInsensitiveDict({
-        'User-Agent': default_user_agent(),
-        'Accept-Encoding': ', '.join(('gzip', 'deflate')),
-        'Accept': '*/*',
-        'Connection': 'keep-alive',
-    })
-
-
-def parse_header_links(value):
-    """Return a dict of parsed link headers proxies.
-
-    i.e. Link: <http:/.../front.jpeg>; rel=front; type="image/jpeg",<http://.../back.jpeg>; rel=back;type="image/jpeg"
-
-    """
-
-    links = []
 
-    replace_chars = " '\""
-
-    for val in re.split(", *<", value):
-        try:
-            url, params = val.split(";", 1)
-        except ValueError:
-            url, params = val, ''
-
-        link = {}
-
-        link["url"] = url.strip("<> '\"")
-
-        for param in params.split(";"):
-            try:
-                key, value = param.split("=")
-            except ValueError:
-                break
-
-            link[key.strip(replace_chars)] = value.strip(replace_chars)
-
-        links.append(link)
-
-    return links
-
-
-# Null bytes; no need to recreate these on each call to guess_json_utf
-_null = '\x00'.encode('ascii')  # encoding to ASCII for Python 3
-_null2 = _null * 2
-_null3 = _null * 3
-
-
-def guess_json_utf(data):
-    # JSON always starts with two ASCII characters, so detection is as
-    # easy as counting the nulls and from their location and count
-    # determine the encoding. Also detect a BOM, if present.
-    sample = data[:4]
-    if sample in (codecs.BOM_UTF32_LE, codecs.BOM32_BE):
-        return 'utf-32'     # BOM included
-    if sample[:3] == codecs.BOM_UTF8:
-        return 'utf-8-sig'  # BOM included, MS style (discouraged)
-    if sample[:2] in (codecs.BOM_UTF16_LE, codecs.BOM_UTF16_BE):
-        return 'utf-16'     # BOM included
-    nullcount = sample.count(_null)
-    if nullcount == 0:
-        return 'utf-8'
-    if nullcount == 2:
-        if sample[::2] == _null2:   # 1st and 3rd are null
-            return 'utf-16-be'
-        if sample[1::2] == _null2:  # 2nd and 4th are null
-            return 'utf-16-le'
-        # Did not detect 2 valid UTF-16 ascii-range characters
-    if nullcount == 3:
-        if sample[:3] == _null3:
-            return 'utf-32-be'
-        if sample[1:] == _null3:
-            return 'utf-32-le'
-        # Did not detect a valid UTF-32 ascii-range character
-    return None
-
-
-def prepend_scheme_if_needed(url, new_scheme):
-    '''Given a URL that may or may not have a scheme, prepend the given scheme.
-    Does not replace a present scheme with the one provided as an argument.'''
-    scheme, netloc, path, params, query, fragment = urlparse(url, new_scheme)
-
-    # urlparse is a finicky beast, and sometimes decides that there isn't a
-    # netloc present. Assume that it's being over-cautious, and switch netloc
-    # and path if urlparse decided there was no netloc.
-    if not netloc:
-        netloc, path = path, netloc
-
-    return urlunparse((scheme, netloc, path, params, query, fragment))
-
-
-def get_auth_from_url(url):
-    """Given a url with authentication components, extract them into a tuple of
-    username,password."""
-    parsed = urlparse(url)
-
-    try:
-        auth = (unquote(parsed.username), unquote(parsed.password))
-    except (AttributeError, TypeError):
-        auth = ('', '')
-
-    return auth
-
-
-def to_native_string(string, encoding='ascii'):
-    """
-    Given a string object, regardless of type, returns a representation of that
-    string in the native string type, encoding and decoding where necessary.
-    This assumes ASCII unless told otherwise.
-    """
-    out = None
+    def _retrieve_from_env(self, names, environ):
+        # We need to handle the case where names is either
+        # a single value or a list of variables.
+        if not isinstance(names, list):
+            names = [names]
+        for name in names:
+            if name in environ:
+                return environ[name]
+        return None
 
-    if isinstance(string, builtin_str):
-        out = string
-    else:
-        if is_py2:
-            out = string.encode(encoding)
+    def get_scoped_config(self):
+        """
+        Returns the config values from the config file scoped to the current
+        profile.
+
+        The configuration data is loaded **only** from the config file.
+        It does not resolve variables based on different locations
+        (e.g. first from the context instance, then from environment
+        variables, then from the config file).  If you want this lookup
+        behavior, use the ``get_config_variable`` method instead.
+
+        Note that this configuration is specific to a single profile (the
+        ``profile`` session variable).
+
+        If the ``profile`` session variable is set and the profile does
+        not exist in the config file, a ``ProfileNotFound`` exception
+        will be raised.
+        """
+        profile_name = self.get_config_variable('profile')
+        profile_map = self._build_profile_map()
+        # If a profile is not explicitly set return the default
+        # profile config or an empty config dict if we don't have
+        # a default profile.
+        if profile_name is None:
+            return profile_map.get('default', {})
+        elif profile_name not in profile_map:
+            # Otherwise if they specified a profile, it has to
+            # exist (even if it's the default profile) otherwise
+            # we complain.
+            raise ProfileNotFound(profile=profile_name)
         else:
-            out = string.decode(encoding)
-
-    return out
-
-
-def urldefragauth(url):
-    """
-    Given a url remove the fragment and the authentication part
-    """
-    scheme, netloc, path, params, query, fragment = urlparse(url)
-
-    # see func:`prepend_scheme_if_needed`
-    if not netloc:
-        netloc, path = path, netloc
+            return profile_map[profile_name]
 
-    netloc = netloc.rsplit('@', 1)[-1]
+    def set_config_variable(self, logical_name, value):
+        """Set a configuration variable to a specific value.
 
-    return urlunparse((scheme, netloc, path, params, query, ''))
+        By using this method, you can override the normal lookup
+        process used in ``get_config_variable`` by explicitly setting
+        a value.  Subsequent calls to ``get_config_variable`` will
+        use the ``value``.  This gives you per-session specific
+        configuration values.
+        ::
+            >>> # Assume logical name 'foo' maps to env var 'FOO'
+            >>> os.environ['FOO'] = 'myvalue'
+            >>> s.get_config_variable('foo')
+            'myvalue'
+            >>> s.set_config_variable('foo', 'othervalue')
+            >>> s.get_config_variable('foo')
+            'othervalue'
+        """
+        self._context_instance_vars[logical_name] = value
+
+    def get_credentials(self, parsed_globals=None):
+        """
+        Return the :class:`botocore.credential.Credential` object
+        associated with this session.
+        """
+        resolver = credentials.create_credential_resolver(self, parsed_globals)
+        return resolver.load_credentials()
```

### Comparing `cdpcli-0.9.9/cdpcli/thirdparty/six.py` & `cdpcli-0.9.90/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/exceptions.py` & `cdpcli-0.9.90/cdpcli/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -70,17 +70,25 @@
         msg = self.MSG_TEMPLATE.format(
             error_code=error_response['error'].get('code', 'Unknown'),
             error_message=error_response['error'].get('message', 'Unknown'),
             operation_name=operation_name,
             service_name=service_name,
             http_status_code=http_status_code,
             request_id=request_id)
+        msg = self.cleanup_error_msg(msg)
         super(ClientError, self).__init__(msg)
+        self.http_status_code = http_status_code
         self.response = error_response
 
+    def cleanup_error_msg(self, msg):
+        msg = msg.replace('&quot;', '"').replace("&#39;", "'")\
+            .replace("/&lt;", "<").replace("&gt;", ">")
+
+        return msg
+
 
 class UnseekableStreamError(CdpCLIError):
     """
     Need to seek a stream, but stream does not support seeking.
     """
     fmt = ('Need to rewind the stream {stream_object}, but stream '
            'is not seekable.')
@@ -117,15 +125,15 @@
     fmt = 'Signature version is not supported: {signature_version}'
 
 
 class NoCredentialsError(CdpCLIError):
     """
     No credentials could be found.
     """
-    fmt = 'Unable to locate CDP credentials'
+    fmt = 'Unable to locate CDP credentials: {err_msg}.'
 
 
 class UnknownCredentialError(CdpCLIError):
     """
     Tried to insert before/after an unregistered credential type.
     """
     fmt = 'Credential named {name} not found.'
@@ -182,14 +190,22 @@
 class ConfigParseError(CdpCLIError):
     """
     The configuration file could not be parsed.
     """
     fmt = 'Unable to parse config file: {path}'
 
 
+class InvalidConfiguredFormFactor(CdpCLIError):
+    """
+    The configured form factor is not a valid value.
+    """
+    fmt = ('The configured form factor {form_factor} is invalid. '
+           'Valid values are: {valid_form_factors}')
+
+
 class ClusterTerminatingError(CdpCLIError):
 
     """
     The cluster is terminating or has already terminated.
     """
     fmt = 'Cluster {cluster_name} is terminating.'
 
@@ -236,7 +252,92 @@
 
 class WrongPuttyKeyError(CdpCLIError):
 
     """
     A wrong key has been used with a compatible program.
     """
     fmt = 'Key file file format is incorrect. Putty expects a ppk file.'
+
+
+class MissingArgumentError(CdpCLIError):
+
+    """
+    The following argument is required.
+    """
+    fmt = 'The following argument is required: {arg_name}.'
+
+
+class InteractiveLoginError(CdpCLIError):
+
+    """
+    Login failed.
+    """
+    fmt = 'Login failed: {err_msg}.'
+
+
+class WrongSvcFormFactorError(CdpCLIError):
+
+    """
+    The service does not work under the current form factor.
+    """
+    fmt = ('The command {service_name} is not available under the {form_factor}'
+           ' CDP form factor. It is only available for these form factors: '
+           '{service_form_factors}. Check that your profile configuration '
+           'specifies the correct form factor, or that the endpoint URL in '
+           'profile configuration or on the command line points to the correct '
+           'control plane.')
+
+
+class WrongOpFormFactorError(CdpCLIError):
+
+    """
+    The operation does not work under the current form factor.
+    """
+    fmt = ('The subcommand {operation_name} under the command {service_name} is '
+           'not available under the {form_factor} CDP form factor. It is only '
+           'available for these form factors: {operation_form_factors}. Check '
+           'that your profile configuration or explicit endpoint URL points to '
+           'the correct control plane.')
+
+
+class WrongArgFormFactorError(CdpCLIError):
+
+    """
+    The argument does not work under the current form factor.
+    """
+    fmt = ('The argument {arg_name} is not available under the {form_factor} '
+           'CDP form factor. It is only available for these form factors: '
+           '{arg_form_factors}. Check that your profile configuration '
+           'or explicit endpoint URL points to the correct control plane.')
+
+
+class ExtensionImportError(CdpCLIError):
+
+    """
+    Failed to import CLI extension.
+    """
+    fmt = 'Failed to import CLI extension \'{ext_name}\': {err}.'
+
+
+class WorkloadServiceDiscoveryError(CdpCLIError):
+
+    """
+    The workload service-discovery failed.
+    """
+    fmt = 'Workload service-discovery error: {err_msg}.'
+
+
+class RedirectExtensionError(CdpCLIError):
+
+    """
+    The redirect extension failed.
+    """
+    fmt = 'The redirect extension failed: {err_msg}.'
+
+
+class DfExtensionError(CdpCLIError):
+
+    """
+    The DF extension failed.
+    """
+    fmt = ('The DF extension failed: {err_msg} '
+           'Service name: {service_name}, operation name: {operation_name}')
```

### Comparing `cdpcli-0.9.9/cdpcli/cdprequest.py` & `cdpcli-0.9.90/cdpcli/cdprequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
 from cdpcli.compat import HTTPHeaders
 from cdpcli.compat import HTTPResponse
 from cdpcli.compat import six
 from cdpcli.compat import urlsplit
 from cdpcli.compat import urlunsplit
 from cdpcli.exceptions import UnseekableStreamError
-from cdpcli.thirdparty.requests import models
-from cdpcli.thirdparty.requests.packages.urllib3.connection import HTTPConnection
-from cdpcli.thirdparty.requests.packages.urllib3.connection import VerifiedHTTPSConnection  # noqa
-from cdpcli.thirdparty.requests.packages.urllib3.connectionpool import HTTPConnectionPool   # noqa
-from cdpcli.thirdparty.requests.packages.urllib3.connectionpool import HTTPSConnectionPool  # noqa
-from cdpcli.thirdparty.requests.sessions import REDIRECT_STATI
+from cdpcli.utils import is_absolute_url
+from requests import models
+from requests.sessions import REDIRECT_STATI
+from urllib3.connection import HTTPConnection
+from urllib3.connection import VerifiedHTTPSConnection  # noqa
+from urllib3.connectionpool import HTTPConnectionPool   # noqa
+from urllib3.connectionpool import HTTPSConnectionPool  # noqa
 
 
 def _urljoin(endpoint_url, url_path):
     p = urlsplit(endpoint_url)
     # <part>   - <index>
     # scheme   - p[0]
     # netloc   - p[1]
@@ -62,15 +63,19 @@
         additional_headers):
     r = request_dict
     headers = r['headers']
     for name, value in additional_headers.items():
         headers[name] = value
     if user_agent_header is not None:
         headers['User-Agent'] = user_agent_header
-    r['url'] = _urljoin(endpoint_url, r['url_path'])
+    url_path = r['url_path']
+    if is_absolute_url(url_path):
+        r['url'] = url_path
+    else:
+        r['url'] = _urljoin(endpoint_url, url_path)
 
 
 def create_request_object(request_dict):
     return CdpRequest(method=request_dict['method'],
                       url=request_dict['url'],
                       data=request_dict['body'],
                       headers=request_dict['headers'])
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/cliinputjson.py` & `cdpcli-0.9.90/cdpcli/extensions/cliinputjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,42 +43,42 @@
     }
 
     def __init__(self, operation_model):
         super(CliInputJSONArgument, self).__init__()
         self._operation_model = operation_model
 
     def invoke(self,
-               client,
-               operation_name,
+               client_creator,
+               operation_model,
                parameters,
                parsed_args,
                parsed_globals):
-        return self.add_to_call_parameters(parameters, parsed_args)
+        return self.add_to_call_parameters(parameters, parsed_args, parsed_globals)
 
-    def add_to_call_parameters(self, call_parameters, parsed_args):
+    def add_to_call_parameters(self, call_parameters, parsed_args, parsed_globals):
 
         # Check if ``--cli-input-json`` was specified in the command line.
         input_json = getattr(parsed_args, 'cli_input_json', None)
         if input_json is not None:
             # Retrieve the JSON from the file if needed.
-            retrieved_json = get_paramfile(input_json)
+            retrieved_json = get_paramfile(input_json, parsed_globals)
             # Nothing was retrieved from the file. So assume the argument
             # is already a JSON string.
             if retrieved_json is None:
                 retrieved_json = input_json
             try:
                 # Try to load the JSON string into a python dictionary
                 input_data = json.loads(retrieved_json)
             except ValueError as e:
                 raise ParamError(
                     self.name, "Invalid JSON: %s\nJSON received: %s"
                                % (e, retrieved_json))
             # We run the ParamFileVisitor over the input data to resolve any
             # paramfile references in it.
-            input_data = ParamFileVisitor().visit(
+            input_data = ParamFileVisitor(parsed_globals).visit(
                 input_data, self._operation_model.input_shape)
             # Add the members from the input JSON to the call parameters.
             self._update_call_parameters(call_parameters, input_data)
         return True
 
     def _update_call_parameters(self, call_parameters, input_data):
         for input_key in input_data.keys():
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-0.9.90/cdpcli/extensions/generatecliskeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     }
 
     def __init__(self, operation_model):
         super(GenerateCliSkeletonArgument, self).__init__()
         self._operation_model = operation_model
 
     def invoke(self,
-               client,
-               operation_name,
+               client_creator,
+               operation_model,
                parameters,
                parsed_args,
                parsed_globals):
         return self._generate_json_skeleton(parsed_args)
 
     def _generate_json_skeleton(self, parsed_args):
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/commands.py` & `cdpcli-0.9.90/cdpcli/extensions/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,29 +139,29 @@
     def __call__(self, client_creator, args, parsed_globals):
         # args is the remaining unparsed args.
         # We might be able to parse these args so we need to create
         # an arg parser and parse them.
         self._subcommand_table = self._build_subcommand_table()
         self._arg_table = self._build_arg_table()
         self._handle_override_required_args(args)
-        parser = ArgTableArgParser(self.arg_table, self.subcommand_table)
+        parser = ArgTableArgParser(self.arg_table, command_table=self.subcommand_table)
         parsed_args, remaining = parser.parse_known_args(args)
 
         # Unpack arguments
         for key, value in vars(parsed_args).items():
             cli_argument = None
 
             # Convert the name to use dashes instead of underscore
             # as these are how the parameters are stored in the
             # `arg_table`.
             xformed = key.replace('_', '-')
             if xformed in self.arg_table:
                 cli_argument = self.arg_table[xformed]
 
-            value = unpack_argument(cli_argument, value)
+            value = unpack_argument(cli_argument, value, parsed_globals)
 
             # If this parameter has a schema defined, then allow plugins
             # a chance to process and override its value.
             if self._should_allow_override(cli_argument, value):
                 # Unpack the argument, which is a string, into the
                 # correct Python type (dict, list, etc)
                 value = unpack_cli_arg(cli_argument, value)
@@ -297,16 +297,16 @@
     @lineage.setter
     def lineage(self, value):
         self._lineage = value
 
 
 class BasicDocHandler(OperationDocumentGenerator):
 
-    def __init__(self, help_command):
-        super(BasicDocHandler, self).__init__(help_command)
+    def __init__(self, help_command, show_hidden=False):
+        super(BasicDocHandler, self).__init__(help_command, show_hidden=show_hidden)
         self.doc = help_command.doc
 
     def build_translation_map(self):
         return {}
 
     def doc_description(self, help_command, **kwargs):
         self.doc.style.h2('Description')
@@ -439,9 +439,10 @@
         else:
             return value
 
     def __call__(self, client_creator, args, parsed_globals):
         # Now generate all of the events for a Provider document.
         # We pass ourselves along so that we can, in turn, get passed
         # to all event handlers.
-        generate_doc(self.GeneratorClass(self), self)
+        generate_doc(self.GeneratorClass(self, show_hidden=parsed_globals.deprecated),
+                     self)
         self.renderer.render(self.doc.getvalue())
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/paginate.py` & `cdpcli-0.9.90/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/extensions/writer.py` & `cdpcli-0.9.90/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/extensions/arguments.py` & `cdpcli-0.9.90/cdpcli/extensions/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         # Set all ``Argument`` objects in ``argument_table`` to not required
         # if this argument's name is present in the command line.
         if name_in_cmdline in args:
             for arg_name in argument_table.keys():
                 argument_table[arg_name].required = False
 
     def invoke(self,
-               client,
-               operation_name,
+               client_creator,
+               operation_model,
                parameters,
                parsed_args,
                parsed_globals):
         """
         Invokes the argument handler. Returns 'True' if other operation call
         handlers should be invoked after it, 'False' to indicate that no other
         invocations should be made.
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/__init__.py` & `cdpcli-0.9.90/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/extensions/configure/get.py` & `cdpcli-0.9.90/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/extensions/configure/set.py` & `cdpcli-0.9.90/cdpcli/extensions/configure/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 import os
 
 from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME
+from cdpcli import CDP_ACCESS_TOKEN_KEY_NAME
 from cdpcli import CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli import DEFAULT_PROFILE_NAME
 from cdpcli.extensions.commands import BasicCommand
 from cdpcli.extensions.writer import ConfigFileWriter
 
 from . import PREDEFINED_SECTION_NAMES
 
@@ -40,14 +41,15 @@
          'action': 'store',
          'no_paramfile': True,  # To disable the default paramfile behavior
          'cli_type_name': 'string', 'positional_arg': True},
     ]
     # Any variables specified in this list will be written to
     # the ~/.cdp/credentials file instead of ~/.cdp/config.
     _WRITE_TO_CREDS_FILE = [CDP_ACCESS_KEY_ID_KEY_NAME,
+                            CDP_ACCESS_TOKEN_KEY_NAME,
                             CDP_PRIVATE_KEY_KEY_NAME]
 
     def __init__(self, config_writer=None):
         super(ConfigureSetCommand, self).__init__()
         if config_writer is None:
             config_writer = ConfigFileWriter()
         self._config_writer = config_writer
@@ -96,14 +98,17 @@
                     value = {parts[1]: value}
             elif len(parts) == 2:
                 # Otherwise it's something like "set preview.service true"
                 # of something in the [plugin] section.
                 section, varname = parts
         config_filename = os.path.expanduser(
             context.get_config_variable('config_file'))
+        if varname == CDP_PRIVATE_KEY_KEY_NAME:
+            # V3/ECDSA private key has '\n' in the string.
+            value = value.replace('\n', '\\n')
         updated_config = {'__section__': section, varname: value}
         if varname in self._WRITE_TO_CREDS_FILE:
             config_filename = os.path.expanduser(
                 context.get_config_variable('credentials_file'))
             section_name = updated_config['__section__']
             if section_name.startswith('profile '):
                 updated_config['__section__'] = section_name[8:]
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/configure/configure.py` & `cdpcli-0.9.90/cdpcli/extensions/configure/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
+                   CDP_ACCESS_TOKEN_KEY_NAME, \
+                   CDP_PRIVATE_KEY_KEY_NAME, \
+                   CDP_REGION_KEY_NAME
 from cdpcli.compat import compat_input
 from cdpcli.endpoint import EndpointResolver
 from cdpcli.exceptions import ProfileNotFound
 from cdpcli.extensions.commands import BasicCommand
 from cdpcli.extensions.configure import CREDENTIAL_FILE_COMMENT
 from cdpcli.extensions.configure.get import ConfigureGetCommand
 from cdpcli.extensions.configure.list import ConfigureListCommand
@@ -51,37 +54,35 @@
 
 
 class ConfigureCommand(BasicCommand):
     NAME = 'configure'
     DESCRIPTION = BasicCommand.FROM_FILE()
     SYNOPSIS = ('cdp configure [--profile profile-name]')
     EXAMPLES = (
-        'To create a new configuration::\n'
+        'To create a new default configuration for CDP Public Cloud::\n'
         '\n'
         '    $ cdp configure\n'
         '    CDP Access Key ID [None]: accesskey\n'
         '    CDP Private Key [None]: privatekey\n'
-        '\n'
-        'To update just the access key id::\n'
-        '\n'
-        '    $ cdp configure\n'
-        '    CDP Access Key ID [***]:\n'
-        '    CDP Private Key [****]:\n'
+        '    CDP Endpoint URL (blank for public cloud) [None]:\n'
     )
     SUBCOMMANDS = [
         {'name': 'list', 'command_class': ConfigureListCommand},
         {'name': 'get', 'command_class': ConfigureGetCommand},
         {'name': 'set', 'command_class': ConfigureSetCommand},
     ]
 
     # If you want to add new values to prompt, update this list here.
     VALUES_TO_PROMPT = [
-        # (logical_name, config_name, prompt_text)
+        # (config_name, prompt_text)
         (CDP_ACCESS_KEY_ID_KEY_NAME, "CDP Access Key ID"),
-        (CDP_PRIVATE_KEY_KEY_NAME, "CDP Private Key")
+        (CDP_PRIVATE_KEY_KEY_NAME, "CDP Private Key"),
+        (CDP_REGION_KEY_NAME, "CDP Region"),
+        (EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME,
+         "CDP Endpoint URL (blank for public cloud)")
     ]
 
     def __init__(self, prompter=None, config_writer=None):
         super(ConfigureCommand, self).__init__()
         if prompter is None:
             prompter = InteractivePrompter()
         self._prompter = prompter
@@ -102,43 +103,38 @@
         for config_name, prompt_text in self.VALUES_TO_PROMPT:
             current_value = config.get(config_name)
             new_value = self._prompter.get_value(current_value, config_name,
                                                  prompt_text)
             if new_value is not None and new_value != current_value:
                 new_values[config_name] = new_value
 
-        if parsed_globals.endpoint_url is not None:
-            new_values[EndpointResolver.ENDPOINT_URL_KEY_NAME] = \
-                parsed_globals.endpoint_url
-
-        if parsed_globals.cdp_endpoint_url is not None:
-            new_values[EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME] = \
-                parsed_globals.cdp_endpoint_url
-
         config_filename = os.path.expanduser(
             context.get_config_variable('config_file'))
         if new_values:
             self._write_out_creds_file_values(context,
                                               new_values,
                                               parsed_globals.profile)
             if parsed_globals.profile is not None:
                 new_values['__section__'] = (
                     'profile %s' % parsed_globals.profile)
             self._config_writer.update_config(new_values, config_filename)
 
     def _write_out_creds_file_values(self, context, new_values, profile_name):
-        # The access_key/private_key are now *always* written to the shared
+        # The access_key/private_key/access_token are now *always* written to the shared
         # credentials file (~/.cdp/credentials).
         credential_file_values = {}
         if CDP_ACCESS_KEY_ID_KEY_NAME in new_values:
             credential_file_values[CDP_ACCESS_KEY_ID_KEY_NAME] = new_values.pop(
                 CDP_ACCESS_KEY_ID_KEY_NAME)
         if CDP_PRIVATE_KEY_KEY_NAME in new_values:
             credential_file_values[CDP_PRIVATE_KEY_KEY_NAME] = new_values.pop(
                 CDP_PRIVATE_KEY_KEY_NAME)
+        if CDP_ACCESS_TOKEN_KEY_NAME in new_values:
+            credential_file_values[CDP_ACCESS_TOKEN_KEY_NAME] = new_values.pop(
+                CDP_ACCESS_TOKEN_KEY_NAME)
         if credential_file_values:
             if profile_name is not None:
                 credential_file_values['__section__'] = profile_name
             shared_credentials_filename = os.path.expanduser(
                 context.get_config_variable('credentials_file'))
             self._config_writer.update_config(
                 credential_file_values,
```

### Comparing `cdpcli-0.9.9/cdpcli/extensions/configure/list.py` & `cdpcli-0.9.90/cdpcli/extensions/configure/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,72 +11,94 @@
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 import sys
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME,\
+    CDP_ENDPOINT_URL_KEY_NAME,\
+    CDP_PRIVATE_KEY_KEY_NAME,\
+    CDP_REGION_KEY_NAME,\
+    ENDPOINT_URL_KEY_NAME,\
+    FORM_FACTOR_KEY_NAME
 from cdpcli.extensions.commands import BasicCommand
 
 from . import ConfigValue, NOT_SET
 
 
 class ConfigureListCommand(BasicCommand):
     NAME = 'list'
     DESCRIPTION = (
-        'List the CDP CLI configuration data.  This command will '
-        'show you the current configuration data.  For each configuration '
-        'item, it will show you the value, where the configuration value '
-        'was retrieved, and the configuration variable name.  For example, '
-        'if you provide the CDP access key in an environment variable, this '
-        'command will show you the key information you\'ve configured, '
-        'it will tell you that this value came from an environment '
-        'variable, and it will tell you the name of the environment '
-        'variable.\n'
+        'List CDP CLI configuration data. Each configuration item\'s name, '
+        'value, source type, and source location are listed. For example, if '
+        'you provide the CDP access key in an environment variable, this '
+        'command will list the access key value and its source as the '
+        'environment.\n'
     )
     SYNOPSIS = 'cdp configure list [--profile profile-name]'
     EXAMPLES = (
         'To show your current configuration values::\n'
         '\n'
         '  $ cdp configure list\n'
-        '        Name                    Value             Type    Location\n'
-        '        ----                    -----             ----    --------\n'
-        '     profile                <not set>             None    None\n'
-        '  access_key     ****************ABCD      config_file    ~/.cdp/config\n'
-        '  private_key    ****************ABCD      config_file    ~/.cdp/config\n'
+        '                Name                Value'
+        '              Source Type    Source\n'
+        '                ----                -----'
+        '              -----------    ------\n'
+        '             profile            <not set>'
+        '                     None    None\n'
+        '   cdp_access_key_id ****************ABCD  shared-credentials-file\n'
+        '     cdp_private_key ****************EFGH  shared-credentials-file\n'
+        '    cdp_endpoint_url            <not set>'
+        '                     None    None\n'
+        '        endpoint_url            <not set>'
+        '                     None    None\n'
+        '         form_factor            <not set>'
+        '                     None    None\n'
         '\n'
     )
 
     def __init__(self, stream=sys.stdout):
         super(ConfigureListCommand, self).__init__()
         self._stream = stream
 
     def _run_main(self, client_creator, args, parsed_globals):
         context = client_creator.context
 
-        self._display_config_value(ConfigValue('Value', 'Type', 'Location'),
+        self._display_config_value(ConfigValue('Value', 'Source Type', 'Source'),
                                    'Name')
-        self._display_config_value(ConfigValue('-----', '----', '--------'),
+        self._display_config_value(ConfigValue('-----', '-----------', '------'),
                                    '----')
 
         if context.profile is not None:
             profile = ConfigValue(context.profile, 'manual', '--profile')
         else:
             profile = self._lookup_config(context, 'profile')
         self._display_config_value(profile, 'profile')
 
         access_key, private_key = self._lookup_credentials(context)
-        self._display_config_value(access_key, 'access_key')
-        self._display_config_value(private_key, 'private_key')
+        self._display_config_value(access_key, CDP_ACCESS_KEY_ID_KEY_NAME)
+        self._display_config_value(private_key, CDP_PRIVATE_KEY_KEY_NAME)
+
+        self._display_config_value(self._lookup_config(context, CDP_REGION_KEY_NAME),
+                                   CDP_REGION_KEY_NAME)
+        self._display_config_value(self._lookup_config(context,
+                                                       CDP_ENDPOINT_URL_KEY_NAME),
+                                   CDP_ENDPOINT_URL_KEY_NAME)
+        self._display_config_value(self._lookup_config(context, ENDPOINT_URL_KEY_NAME),
+                                   ENDPOINT_URL_KEY_NAME)
+        self._display_config_value(self._lookup_config(context, FORM_FACTOR_KEY_NAME),
+                                   FORM_FACTOR_KEY_NAME)
 
     def _display_config_value(self, config_value, config_name):
-        self._stream.write('%10s %24s %16s    %s\n' % (
-            config_name, config_value.value, config_value.config_type,
-            config_value.config_variable))
+        truncated_value = (config_value.value[:27] + '...')\
+            if len(config_value.value) > 30 else config_value.value
+        self._stream.write('%20s %30s %24s    %s\n' % (
+            config_name, truncated_value, config_value.source_type,
+            config_value.source))
 
     def _lookup_credentials(self, context):
         # First try it with _lookup_config.  It's possible
         # that we don't find credentials this way.
         access_key = self._lookup_config(context, CDP_ACCESS_KEY_ID_KEY_NAME)
         if access_key.value is not NOT_SET:
             private_key = self._lookup_config(context, CDP_PRIVATE_KEY_KEY_NAME)
```

### Comparing `cdpcli-0.9.9/cdpcli/credentials.py` & `cdpcli-0.9.90/cdpcli/credentials.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,45 +14,55 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from collections import namedtuple
 import logging
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
+                   CDP_ACCESS_TOKEN_KEY_NAME, \
+                   CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli.auth import AccessTokenAuth
 from cdpcli.auth import Ed25519v1Auth
 import cdpcli.compat
 from cdpcli.compat import json
 from cdpcli.configloader import raw_config_parse
 from cdpcli.exceptions import ConfigNotFound
 from cdpcli.exceptions import MalformedCredentialsError
 from cdpcli.exceptions import NoCredentialsError
 from cdpcli.exceptions import PartialCredentialsError
 from cdpcli.exceptions import UnknownCredentialError
 
 LOG = logging.getLogger('cdpcli.credentials')
 ReadOnlyCredentials = namedtuple('ReadOnlyCredentials',
-                                 ['access_key_id', 'private_key', 'method'])
+                                 ['access_key_id',
+                                  'private_key',
+                                  'access_token',
+                                  'method'])
 ACCESS_KEY_ID = 'access_key_id'
 PRIVATE_KEY = 'private_key'
+ACCESS_TOKEN = 'access_token'
 
 
-def create_credential_resolver(context):
+def create_credential_resolver(context, parsed_globals=None):
     """Create a default credential resolver.
 
     This creates a pre-configured credential resolver
     that includes the default lookup chain for
     credentials.
+
+    :param parsed_globals: CLI input parameters which might contain an access-token.
     """
     profile_name = context.effective_profile
     auth_file = context.get_config_variable('auth_config')
     shared_credential_file = context.get_config_variable('credentials_file')
 
     env_provider = EnvProvider()
     providers = [
+        ParamsProvider(parsed_globals),
         env_provider,
         AuthConfigFile(auth_file),
         SharedCredentialProvider(
             creds_filename=shared_credential_file,
             profile_name=profile_name
         ),
     ]
@@ -79,37 +89,44 @@
         LOG.debug('Skipping environment variable credential check because '
                   'profile name was explicitly set.')
 
     resolver = CredentialResolver(providers=providers)
     return resolver
 
 
-def get_credentials(context):
-    resolver = create_credential_resolver(context)
+def get_credentials(context, parsed_globals=None):
+    resolver = create_credential_resolver(context, parsed_globals)
     return resolver.load_credentials()
 
 
 class Credentials(object):
     """
     Holds the credentials needed to authenticate requests.
     """
 
-    def __init__(self, access_key_id, private_key, method):
+    def __init__(self,
+                 access_key_id=None,
+                 private_key=None,
+                 access_token=None,
+                 method=None):
         self.access_key_id = access_key_id
         self.private_key = private_key
+        self.access_token = access_token
         self.method = method
         self._normalize()
 
     def _normalize(self):
         self.access_key_id = cdpcli.compat.ensure_unicode(self.access_key_id)
         self.private_key = cdpcli.compat.ensure_unicode(self.private_key)
+        self.access_token = cdpcli.compat.ensure_unicode(self.access_token)
 
     def get_frozen_credentials(self):
         return ReadOnlyCredentials(self.access_key_id,
                                    self.private_key,
+                                   self.access_token,
                                    self.method)
 
 
 class CredentialProvider(object):
 
     # Implementations must provide a method.
     METHOD = None
@@ -121,21 +138,25 @@
         found = []
         for key_name in key_names:
             try:
                 found.append(mapping[key_name])
             except KeyError:
                 raise PartialCredentialsError(provider=self.METHOD,
                                               cred_var=key_name)
-        return found
+        if len(found) == 1:  # found access-token, returns a single-value string.
+            return found[0]
+        else:  # found access-key-id and private-key, returns a tuple.
+            return found
 
 
 class EnvProvider(CredentialProvider):
     METHOD = 'env'
     ACCESS_KEY_ID_ENV_VAR = 'CDP_ACCESS_KEY_ID'
     PRIVATE_KEY_ENV_VAR = 'CDP_PRIVATE_KEY'
+    ACCESS_TOKEN_ENV_VAR = 'CDP_ACCESS_TOKEN'
 
     def __init__(self, environ=None, mapping=None):
         super(EnvProvider, self).__init__()
         if environ is None:
             environ = os.environ
         self.environ = environ
         self._mapping = self._build_mapping(mapping)
@@ -143,19 +164,22 @@
     def _build_mapping(self, mapping):
         # Mapping of variable name to env var name.
         var_mapping = {}
         if mapping is None:
             # Use the class var default.
             var_mapping[ACCESS_KEY_ID] = self.ACCESS_KEY_ID_ENV_VAR
             var_mapping[PRIVATE_KEY] = self.PRIVATE_KEY_ENV_VAR
+            var_mapping[ACCESS_TOKEN] = self.ACCESS_TOKEN_ENV_VAR
         else:
             var_mapping[ACCESS_KEY_ID] = mapping.get(
                 ACCESS_KEY_ID, self.ACCESS_KEY_ID_ENV_VAR)
             var_mapping[PRIVATE_KEY] = mapping.get(
                 PRIVATE_KEY, self.PRIVATE_KEY_ENV_VAR)
+            var_mapping[ACCESS_TOKEN] = mapping.get(
+                ACCESS_TOKEN, self.ACCESS_TOKEN_ENV_VAR)
         return var_mapping
 
     def load(self):
         """
         Search for credentials in explicit environment variables.
         """
         if self._mapping[ACCESS_KEY_ID] in self.environ:
@@ -167,19 +191,30 @@
             # For compatibility, assume the PRIVATE_KEY is a path to a file
             # containing the key. Only if there is no file, should the value
             # be checked to see if it's an actual key.
             if not os.path.isfile(private_key):
                 if Ed25519v1Auth.detect_private_key(private_key):
                     private_key_value = private_key
                 else:
-                    LOG.debug("Private key at %s does not exist!" % private_key)
-                    raise NoCredentialsError()
+                    raise NoCredentialsError(
+                        err_msg='Private key file {} does not exist'.format(private_key))
             else:
                 private_key_value = open(private_key).read()
-            return Credentials(access_key_id, private_key_value,
+            return Credentials(access_key_id=access_key_id,
+                               private_key=private_key_value,
+                               method=self.METHOD)
+        elif self._mapping[ACCESS_TOKEN] in self.environ:
+            access_token = self._extract_creds_from_mapping(
+                self.environ, self._mapping[ACCESS_TOKEN])
+            LOG.info('Found access token in environment variables.')
+            if not AccessTokenAuth.is_access_token(access_token):
+                LOG.debug('Invalid access token {}'.format(access_token))
+                raise NoCredentialsError(
+                    err_msg='Invalid access token (see debug log for value)')
+            return Credentials(access_token=access_token,
                                method=self.METHOD)
         else:
             return None
 
 
 class CredentialResolver(object):
 
@@ -230,22 +265,33 @@
             raise UnknownCredentialError(name=name)
 
     def load_credentials(self):
         """
         Goes through the credentials chain, returning the first ``Credentials``
         that could be loaded.
         """
+
+        # Grab this during the scan in case no credentials are available.
+        creds_expanded_path = None
+
         # First provider to return a non-None response wins.
         for provider in self.providers:
             LOG.debug("Looking for credentials via: %s", provider.METHOD)
+            if isinstance(provider, SharedCredentialProvider):
+                creds_expanded_path = provider.get_creds_expanded_path()
             creds = provider.load()
             if creds is not None:
                 return creds
 
-        raise NoCredentialsError()
+        err_msg = "No credentials found anywhere in chain"
+        if creds_expanded_path:
+            err_msg += ". The shared credentials file should be stored at {}"\
+                .format(creds_expanded_path)
+
+        raise NoCredentialsError(err_msg=err_msg)
 
 
 class AuthConfigFile(CredentialProvider):
     METHOD = 'auth_config_file'
 
     def __init__(self, conf):
         super(AuthConfigFile, self).__init__()
@@ -255,56 +301,102 @@
         """
         load the credential from the json configuration file.
         """
         if self._conf is None:
             return None
 
         if not os.path.isfile(self._conf):
-            LOG.debug("Conf file at %s does not exist!" % self._conf)
-            raise NoCredentialsError()
+            raise NoCredentialsError(
+                err_msg="Config file {} not found".format(self._conf))
         try:
             conf = json.loads(open(self._conf).read())
         except Exception:
             LOG.debug("Could not read conf: %s", exc_info=True)
             return None
 
-        if ACCESS_KEY_ID not in conf:
+        if ACCESS_KEY_ID in conf or PRIVATE_KEY in conf:
+            LOG.debug('Found credentials for key: %s in configuration file.',
+                      conf[ACCESS_KEY_ID])
+            access_key_id, private_key = self._extract_creds_from_mapping(
+                conf,
+                ACCESS_KEY_ID,
+                PRIVATE_KEY)
+            return Credentials(access_key_id=access_key_id,
+                               private_key=private_key,
+                               method=self.METHOD)
+        elif ACCESS_TOKEN in conf:
+            LOG.debug('Found access-token in configuration file.')
+            access_token = self._extract_creds_from_mapping(conf, ACCESS_TOKEN)
+            return Credentials(access_token=access_token,
+                               method=self.METHOD)
+        else:
+            cred_vars = '%s or %s' % (ACCESS_KEY_ID, ACCESS_TOKEN)
             LOG.debug('Auth config file is missing required key %s',
-                      ACCESS_KEY_ID)
+                      cred_vars)
             raise MalformedCredentialsError(provider=self.METHOD,
-                                            cred_var=ACCESS_KEY_ID)
-
-        LOG.debug('Found credentials for key: %s in configuration file.',
-                  conf[ACCESS_KEY_ID])
-        access_key_id, private_key = self._extract_creds_from_mapping(
-            conf,
-            ACCESS_KEY_ID,
-            PRIVATE_KEY)
-        return Credentials(access_key_id, private_key, self.METHOD)
+                                            cred_var=cred_vars)
 
 
 class SharedCredentialProvider(CredentialProvider):
     METHOD = 'shared-credentials-file'
 
     def __init__(self, creds_filename, profile_name):
         self._creds_filename = creds_filename
+        self._creds_expanded_path = os.path.expanduser(creds_filename)
         self._profile_name = profile_name
 
+    def get_creds_expanded_path(self):
+        return self._creds_expanded_path
+
     def load(self):
         try:
             available_creds = raw_config_parse(self._creds_filename)
         except ConfigNotFound:
-            LOG.debug("Credentials file at %s does not exist!" % self._creds_filename)
+            LOG.debug("Shared credentials file {} not found".format(self._creds_filename))
             return None
         if self._profile_name in available_creds:
             config = available_creds[self._profile_name]
-            access_key_id, private_key = self._extract_creds_from_mapping(
-                config, CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME)
-            # We store the private key in the credentials file as a one-line
-            # value in which the newlines in the PEM file are replaced with
-            # '\n'. We need to replace them back as the RawConfigParser we use
-            # does not do it for us. Note that if the value in the configuration
-            # IS a PEM formatted value this is a no-op.
-            private_key = private_key.replace('\\n', '\n')
-            LOG.info("Found credentials in shared credentials file: %s",
-                     self._creds_filename)
-            return Credentials(access_key_id, private_key, method=self.METHOD)
+
+            if CDP_ACCESS_KEY_ID_KEY_NAME in config or \
+                    CDP_PRIVATE_KEY_KEY_NAME in config:
+                access_key_id, private_key = self._extract_creds_from_mapping(
+                    config, CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME)
+                # We store the private key in the credentials file as a one-line
+                # value in which the newlines in the PEM file are replaced with
+                # '\n'. We need to replace them back as the RawConfigParser we use
+                # does not do it for us. Note that if the value in the configuration
+                # IS a PEM formatted value this is a no-op.
+                private_key = private_key.replace('\\n', '\n')
+                LOG.info("Found credentials in shared credentials file: %s",
+                         self._creds_filename)
+                return Credentials(access_key_id=access_key_id,
+                                   private_key=private_key,
+                                   method=self.METHOD)
+            elif CDP_ACCESS_TOKEN_KEY_NAME in config:
+                access_token = self._extract_creds_from_mapping(
+                    config, CDP_ACCESS_TOKEN_KEY_NAME)
+                LOG.info("Found access-token in shared credentials file: %s",
+                         self._creds_filename)
+                return Credentials(access_token=access_token,
+                                   method=self.METHOD)
+            else:
+                return None
+
+
+class ParamsProvider(CredentialProvider):
+    """
+    Support for access-token parameter only.
+    """
+
+    METHOD = 'params'
+
+    def __init__(self, params):
+        if params is None:
+            self._access_token = None
+        else:
+            self._access_token = getattr(params, 'access_token', None)
+
+    def load(self):
+        if bool(self._access_token):
+            return Credentials(access_token=self._access_token,
+                               method=self.METHOD)
+        return None
```

### Comparing `cdpcli-0.9.9/cdpcli/main.py` & `cdpcli-0.9.90/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/validate.py` & `cdpcli-0.9.90/cdpcli/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
+import base64
 import datetime
 import decimal
 
 from cdpcli.compat import six
 from cdpcli.exceptions import ParamValidationError
 from cdpcli.utils import parse_to_aware_datetime
 
@@ -134,14 +135,17 @@
                                min_allowed, max_allowed))
         elif error_type == 'invalid length':
             min_allowed = additional['valid_range'][0]
             max_allowed = additional['valid_range'][1]
             return ('Invalid length for parameter %s, value: %s, valid range: '
                     '%s-%s' % (name, additional['param'],
                                min_allowed, max_allowed))
+        elif error_type == 'invalid base64':
+            return 'Invalid base64 value for parameter %s, error: %s' \
+                % (name, additional['error'])
 
     def _get_name(self, name):
         if not name:
             return 'input'
         elif name.startswith('.'):
             return name[1:]
         else:
@@ -222,14 +226,25 @@
         # to a datetime.
         is_valid_type = self._type_check_datetime(param)
         if not is_valid_type:
             valid_type_names = [six.text_type(datetime), 'timestamp-string']
             errors.report(name, 'invalid type', param=param,
                           valid_types=valid_type_names)
 
+    @type_check(valid_types=(bytes, bytearray, six.string_types))
+    def _validate_blob(self, param, shape, errors, name):
+        if isinstance(param, six.string_types):
+            try:
+                bytes = base64.b64decode(param)
+                length_check(name, len(bytes), shape, 'invalid length', errors)
+            except Exception as err:
+                errors.report(name, 'invalid base64', error=err)
+        else:
+            length_check(name, len(param), shape, 'invalid length', errors)
+
     def _type_check_datetime(self, value):
         try:
             parse_to_aware_datetime(value)
             return True
         except (TypeError, ValueError, AttributeError):
             # Yes, dateutil can sometimes raise an AttributeError when parsing
             # timestamps.
```

### Comparing `cdpcli-0.9.9/cdpcli/doc/style.py` & `cdpcli-0.9.90/cdpcli/doc/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,19 @@
             self.end_bold()
 
     def ref(self, title, link=None):
         if link is None:
             link = title
         self.doc.write(':doc:`%s <%s>`' % (title, link))
 
+    def simple_field(self, field_name, field_value):
+        self.new_paragraph()
+        self.doc.write(':%s: %s' % (field_name, field_value))
+        self.new_paragraph()
+
     def _heading(self, s, border_char):
         border = border_char * len(s)
         self.new_paragraph()
         self.doc.write('%s\n%s\n%s' % (border, s, border))
         self.new_paragraph()
 
     def h1(self, s):
```

### Comparing `cdpcli-0.9.9/cdpcli/doc/restdoc.py` & `cdpcli-0.9.90/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/doc/docstringparser.py` & `cdpcli-0.9.90/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-0.9.90/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/examples/configure/get/_description.rst` & `cdpcli-0.9.90/cdpcli/examples/configure/get/_description.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 An unqualified configuration name refers to a name that is not scoped to a
 specific section in the configuration file.  Sections are specified by
 separating parts with the ``"."`` character (``section.config-name``).  An
 unqualified name will be scoped to the current profile.  For example,
 ``cdp configure get cdp_access_key_id`` will retrieve the ``cdp_access_key_id``
 from the current profile,  or the ``default`` profile if no profile is
 specified.  You can still provide a ``--profile`` argument to the ``cdp
-configure get`` command.  For example, ``cdp configure get region --profile
+configure get`` command.  For example, ``cdp configure get cdp_region --profile
 testing`` will print the region value for the ``testing`` profile.
 
 
 Qualified Names
 ---------------
 
 A qualified name is a name that has at least one ``"."`` character in the name.
```

### Comparing `cdpcli-0.9.9/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-0.9.90/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/examples/configure/set/_description.rst` & `cdpcli-0.9.90/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/serialize.py` & `cdpcli-0.9.90/cdpcli/serialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,40 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
+import base64
+
 from cdpcli import validate
 from cdpcli.compat import json
 from cdpcli.compat import OrderedDict
+from cdpcli.compat import six
 
 
 def create_serializer():
     serializer = Serializer()
     validator = validate.ParamValidator()
     return validate.ParamValidationDecorator(validator, serializer)
 
 
 class Serializer(object):
     DEFAULT_ENCODING = 'utf-8'
 
+    def _get_base64(self, value):
+        # Returns the base64-encoded version of value, handling
+        # both strings and bytes. The returned value is a string
+        # via the default encoding.
+        if isinstance(value, six.string_types):
+            value = value.encode(self.DEFAULT_ENCODING)
+        return base64.b64encode(value).strip().decode(
+            self.DEFAULT_ENCODING)
+
     def serialize_to_request(self, parameters, operation_model):
         # Don't serialize any parameter with a None value.
         filtered_parameters = OrderedDict(
             (k, v) for k, v in parameters.items() if v is not None)
 
         serialized = {}
         serialized['method'] = operation_model.http['method']
@@ -73,9 +85,20 @@
             # JSON list serialization is the only case where we aren't setting
             # a key on a dict.  We handle this by using a __current__ key on a
             # wrapper dict to serialize each list item before appending it to
             # the serialized list.
             self._serialize(wrapper, array_item, shape.member, "__current__")
             array_obj.append(wrapper["__current__"])
 
+    def _serialize_type_blob(self, serialized, value, shape, key):
+        # Blob args must be base64 encoded.
+        # If value type is string/text, it is already base64 encoded, verified
+        # in validate.py.
+        # Use isinstance(six.string_types) because a string could be either str
+        # or unicode in python2.
+        if isinstance(value, six.string_types):
+            serialized[key] = value
+        else:
+            serialized[key] = self._get_base64(value)
+
     def _default_serialize(self, serialized, value, shape, key):
         serialized[key] = value
```

### Comparing `cdpcli-0.9.9/cdpcli/retryhandler.py` & `cdpcli-0.9.90/cdpcli/retryhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import functools
 import logging
 
 from cdpcli.exceptions import EndpointConnectionError
-from cdpcli.thirdparty.requests import ConnectionError, Timeout
-from cdpcli.thirdparty.requests.packages.urllib3.exceptions \
-    import ClosedPoolError
+from requests import ConnectionError, Timeout
+from urllib3.exceptions import ClosedPoolError
 
 
 LOG = logging.getLogger('cdpcli.retryhandler')
 # The only supported error for now is GENERAL_CONNECTION_ERROR
 # which maps to requests generic ConnectionError.  If we're able
 # to get more specific exceptions from requests we can update
 # this mapping with more specific exceptions.
```

### Comparing `cdpcli-0.9.9/cdpcli/paginate.py` & `cdpcli-0.9.90/cdpcli/paginate.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,17 +100,25 @@
             # advance to the next page
             self._op_kwargs[self._input_token_key] = \
                 previous_next_token = next_token
 
     # builds a full operation result object by iterating over pages which are
     # fetched using multiple requests to service
     def build_full_result(self):
+        first_response = True
         result = {}
         # iterate over service responses, one response per page of results
         for response in self:
+            if first_response:
+                result = copy(response)
+                if self._result_key in result:
+                    del result[self._result_key]
+                if self._output_token_key in result:
+                    del result[self._output_token_key]
+                first_response = False
             response_value = response.get(self._result_key, None)
             if response_value is None:
                 continue
             existing_value = result.get(self._result_key, None)
             if existing_value is None:
                 result[self._result_key] = copy(response_value)
             elif isinstance(response_value, list):
```

### Comparing `cdpcli-0.9.9/cdpcli/table.py` & `cdpcli-0.9.90/cdpcli/shorthand.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,402 +10,389 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import os
-import struct
-import sys
-
-from cdpcli.compat import six
-import colorama
-
-
-def determine_terminal_width(default_width=80):
-    # If we can't detect the terminal width, the default_width is returned.
-    try:
-        from termios import TIOCGWINSZ
-        from fcntl import ioctl
-    except ImportError:
-        return default_width
-    try:
-        height, width = struct.unpack('hhhh', ioctl(sys.stdout,
-                                                    TIOCGWINSZ, '\000' * 8))[0:2]
-    except Exception:
-        return default_width
-    else:
-        return width
-
-
-def is_a_tty():
-    try:
-        return os.isatty(sys.stdout.fileno())
-    except Exception:
-        return False
-
-
-def center_text(text, length=80, left_edge='|', right_edge='|',
-                text_length=None):
-    """Center text with specified edge chars.
-
-    You can pass in the length of the text as an arg, otherwise it is computed
-    automatically for you.  This can allow you to center a string not based
-    on it's literal length (useful if you're using ANSI codes).
-    """
-    # postcondition: len(returned_text) == length
-    if text_length is None:
-        text_length = len(text)
-    output = []
-    char_start = (length // 2) - (text_length // 2) - 1
-    output.append(left_edge + ' ' * char_start + text)
-    length_so_far = len(left_edge) + char_start + text_length
-    right_side_spaces = length - len(right_edge) - length_so_far
-    output.append(' ' * right_side_spaces)
-    output.append(right_edge)
-    final = ''.join(output)
-    return final
-
-
-def align_left(text, length, left_edge='|', right_edge='|', text_length=None,
-               left_padding=2):
-    """Left align text."""
-    # postcondition: len(returned_text) == length
-    if text_length is None:
-        text_length = len(text)
-    computed_length = (
-        text_length + left_padding + len(left_edge) + len(right_edge))
-    if length - computed_length >= 0:
-        padding = left_padding
-    else:
-        padding = 0
-    output = []
-    length_so_far = 0
-    output.append(left_edge)
-    length_so_far += len(left_edge)
-    output.append(' ' * padding)
-    length_so_far += padding
-    output.append(text)
-    length_so_far += text_length
-    output.append(' ' * (length - length_so_far - len(right_edge)))
-    output.append(right_edge)
-    return ''.join(output)
-
-
-def convert_to_vertical_table(sections):
-    # Any section that only has a single row is
-    # inverted, so:
-    # header1 | header2 | header3
-    # val1    | val2    | val2
-    #
-    # becomes:
-    #
-    # header1 | val1
-    # header2 | val2
-    # header3 | val3
-    for i, section in enumerate(sections):
-        if len(section.rows) == 1 and section.headers:
-            headers = section.headers
-            new_section = Section()
-            new_section.title = section.title
-            new_section.indent_level = section.indent_level
-            for header, element in zip(headers, section.rows[0]):
-                new_section.add_row([header, element])
-            sections[i] = new_section
-
-
-class IndentedStream(object):
-    def __init__(self, stream, indent_level, left_indent_char='|',
-                 right_indent_char='|'):
-        self._stream = stream
-        self._indent_level = indent_level
-        self._left_indent_char = left_indent_char
-        self._right_indent_char = right_indent_char
-
-    def write(self, text):
-        self._stream.write(self._left_indent_char * self._indent_level)
-        if text.endswith('\n'):
-            self._stream.write(text[:-1])
-            self._stream.write(self._right_indent_char * self._indent_level)
-            self._stream.write('\n')
-        else:
-            self._stream.write(text)
+import logging
+import re
+import string
+
+LOG = logging.getLogger('cdpcli.shorthand')
+_EOF = object()
+
+
+class _NamedRegex(object):
+    def __init__(self, name, regex_str):
+        self.name = name
+        self.regex = re.compile(regex_str, re.UNICODE)
+
+    def match(self, value):
+        return self.regex.match(value)
+
+
+class ShorthandParseError(Exception):
+    def __init__(self, value, expected, actual, index):
+        self.value = value
+        self.expected = expected
+        self.actual = actual
+        self.index = index
+        msg = self._construct_msg()
+        super(ShorthandParseError, self).__init__(msg)
+
+    def _construct_msg(self):
+        consumed, remaining, num_spaces = self.value, '', self.index
+        if '\n' in self.value[:self.index]:
+            # If there's newlines in the consumed expression, we want
+            # to make sure we're only counting the spaces
+            # from the last newline:
+            # foo=bar,\n
+            # bar==baz
+            #     ^
+            last_newline = self.value[:self.index].rindex('\n')
+            num_spaces = self.index - last_newline - 1
+        if '\n' in self.value[self.index:]:
+            # If there's newline in the remaining, divide value
+            # into consumed and remainig
+            # foo==bar,\n
+            #     ^
+            # bar=baz
+            next_newline = self.index + self.value[self.index:].index('\n')
+            consumed = self.value[:next_newline]
+            remaining = self.value[next_newline:]
+        msg = (
+            "Expected: '%s', received: '%s' for input:\n"
+            "%s\n"
+            "%s"
+            "%s"
+        ) % (self.expected, self.actual, consumed,
+             ' ' * num_spaces + '^', remaining)
+        return msg
+
+
+class ShorthandParser(object):
+    """Parses shorthand syntax in the CLI.
 
-    def __getattr__(self, attr):
-        return getattr(self._stream, attr)
+    Note that this parser does not rely on any JSON models to control
+    how to parse the shorthand syntax.
 
+    """
 
-class Styler(object):
-    def style_title(self, text):
-        return text
+    _SINGLE_QUOTED = _NamedRegex('singled quoted', r'\'(?:\\\\|\\\'|[^\'])*\'')
+    _DOUBLE_QUOTED = _NamedRegex('double quoted', r'"(?:\\\\|\\"|[^"])*"')
+    _START_WORD = u'\\!\\#-&\\(-\\+\\--\\<\\>-Z\\\\-z\u007c-\uffff'
+    _FIRST_FOLLOW_CHARS = u'\\s\\!\\#-&\\(-\\+\\--\\\\\\^-\\|~-\uffff'
+    _SECOND_FOLLOW_CHARS = u'\\s\\!\\#-&\\(-\\+\\--\\<\\>-\uffff'
+    _ESCAPED_COMMA = '(\\\\,)'
+    _FIRST_VALUE = _NamedRegex(
+        'first',
+        u'({escaped_comma}|[{start_word}])'
+        u'({escaped_comma}|[{follow_chars}])*'.format(
+            escaped_comma=_ESCAPED_COMMA,
+            start_word=_START_WORD,
+            follow_chars=_FIRST_FOLLOW_CHARS,
+        ))
+    _SECOND_VALUE = _NamedRegex(
+        'second',
+        u'({escaped_comma}|[{start_word}])'
+        u'({escaped_comma}|[{follow_chars}])*'.format(
+            escaped_comma=_ESCAPED_COMMA,
+            start_word=_START_WORD,
+            follow_chars=_SECOND_FOLLOW_CHARS,
+        ))
 
-    def style_header_column(self, text):
-        return text
+    def __init__(self):
+        self._tokens = []
 
-    def style_row_element(self, text):
-        return text
+    def parse(self, value):
+        """Parse shorthand syntax.
 
-    def style_indentation_char(self, text):
-        return text
+        For example::
 
+            parser = ShorthandParser()
+            parser.parse('a=b')  # {'a': 'b'}
+            parser.parse('a=b,c')  # {'a': ['b', 'c']}
+
+        :tpye value: str
+        :param value: Any value that needs to be parsed.
+
+        :return: Parsed value, which will be a dictionary.
+        """
+        self._input_value = value
+        self._index = 0
+        return self._parameter()
+
+    def _parameter(self):
+        # parameter = keyval *("," keyval)
+        params = {}
+        params.update(self._keyval())
+        while self._index < len(self._input_value):
+            self._expect(',', consume_whitespace=True)
+            keyval = self._keyval()
+            for key in keyval.keys():
+                if key in params:
+                    LOG.warn('A value for the key "%s" was given more than '
+                             'once. Only the last value listed will be used. '
+                             'Separate multiple sets of key-value pairs with '
+                             'spaces.', key)
+            params.update(keyval)
+        return params
+
+    def _keyval(self):
+        # keyval = key "=" [values]
+        key = self._key()
+        self._expect('=', consume_whitespace=True)
+        values = self._values()
+        return {key: values}
+
+    def _key(self):
+        # key = 1*(alpha / %x30-39 / %x5f / %x2e)  ; [a-zA-Z0-9\-_.]
+        valid_chars = string.ascii_letters + string.digits + '-_.'
+        start = self._index
+        while not self._at_eof():
+            if self._current() not in valid_chars:
+                break
+            self._index += 1
+        return self._input_value[start:self._index]
+
+    def _values(self):
+        # values = csv-list / explicit-list / hash-literal
+        if self._at_eof():
+            return ''
+        elif self._current() == '[':
+            return self._explicit_list()
+        elif self._current() == '{':
+            return self._hash_literal()
+        else:
+            return self._csv_value()
 
-class ColorizedStyler(Styler):
-    def __init__(self):
-        # autoreset allows us to not have to sent
-        # reset sequences for every string.
-        colorama.init(autoreset=True)
-
-    def style_title(self, text):
-        # Originally bold + underline
-        return text
-
-    def style_header_column(self, text):
-        # Originally underline
-        return text
-
-    def style_row_element(self, text):
-        return (colorama.Style.BRIGHT + colorama.Fore.BLUE +
-                text + colorama.Style.RESET_ALL)
-
-    def style_indentation_char(self, text):
-        return (colorama.Style.DIM + colorama.Fore.YELLOW +
-                text + colorama.Style.RESET_ALL)
-
-
-class MultiTable(object):
-    def __init__(self, terminal_width=None, initial_section=True,
-                 column_separator='|', terminal=None,
-                 styler=None, auto_reformat=True):
-        self._auto_reformat = auto_reformat
-        if initial_section:
-            self._current_section = Section()
-            self._sections = [self._current_section]
+    def _csv_value(self):
+        # Supports either:
+        # foo=bar     -> 'bar'
+        #     ^
+        # foo=bar,baz -> ['bar', 'baz']
+        #     ^
+        first_value = self._first_value()
+        self._consume_whitespace()
+        if self._at_eof() or self._input_value[self._index] != ',':
+            return first_value
+        self._expect(',', consume_whitespace=True)
+        csv_list = [first_value]
+        # Try to parse remaining list values.
+        # It's possible we don't parse anything:
+        # a=b,c=d
+        #     ^-here
+        # In the case above, we'll hit the ShorthandParser,
+        # backtrack to the comma, and return a single scalar
+        # value 'b'.
+        while True:
+            try:
+                current = self._second_value()
+                self._consume_whitespace()
+                if self._at_eof():
+                    csv_list.append(current)
+                    break
+                self._expect(',', consume_whitespace=True)
+                csv_list.append(current)
+            except ShorthandParseError:
+                # Backtrack to the previous comma.
+                # This can happen when we reach this case:
+                # foo=a,b,c=d,e=f
+                #     ^-start
+                # foo=a,b,c=d,e=f
+                #          ^-error, "expected ',' received '='
+                # foo=a,b,c=d,e=f
+                #        ^-backtrack to here.
+                if self._at_eof():
+                    raise
+                self._backtrack_to(',')
+                break
+        if len(csv_list) == 1:
+            # Then this was a foo=bar case, so we expect
+            # this to parse to a scalar value 'bar', i.e
+            # {"foo": "bar"} instead of {"bar": ["bar"]}
+            return first_value
+        return csv_list
+
+    def _value(self):
+        result = self._FIRST_VALUE.match(self._input_value[self._index:])
+        if result is not None:
+            consumed = self._consume_matched_regex(result)
+            return consumed.replace('\\,', ',').rstrip()
+        return ''
+
+    def _explicit_list(self):
+        # explicit-list = "[" [value *(",' value)] "]"
+        self._expect('[', consume_whitespace=True)
+        values = []
+        while self._current() != ']':
+            val = self._explicit_values()
+            values.append(val)
+            self._consume_whitespace()
+            if self._current() != ']':
+                self._expect(',')
+                self._consume_whitespace()
+        self._expect(']')
+        return values
+
+    def _explicit_values(self):
+        # values = csv-list / explicit-list / hash-literal
+        if self._current() == '[':
+            return self._explicit_list()
+        elif self._current() == '{':
+            return self._hash_literal()
         else:
-            self._current_section = None
-            self._sections = []
-        if styler is None:
-            # Move out to factory.
-            if is_a_tty():
-                self._styler = ColorizedStyler()
-            else:
-                self._styler = Styler()
+            return self._first_value()
+
+    def _hash_literal(self):
+        self._expect('{', consume_whitespace=True)
+        keyvals = {}
+        while self._current() != '}':
+            key = self._key()
+            self._expect('=', consume_whitespace=True)
+            v = self._explicit_values()
+            self._consume_whitespace()
+            if self._current() != '}':
+                self._expect(',')
+                self._consume_whitespace()
+            keyvals[key] = v
+        self._expect('}')
+        return keyvals
+
+    def _first_value(self):
+        # first-value = value / single-quoted-val / double-quoted-val
+        if self._current() == "'":
+            return self._single_quoted_value()
+        elif self._current() == '"':
+            return self._double_quoted_value()
+        return self._value()
+
+    def _single_quoted_value(self):
+        # single-quoted-value = %x27 *(val-escaped-single) %x27
+        # val-escaped-single  = %x20-26 / %x28-7F / escaped-escape /
+        #                       (escape single-quote)
+        return self._consume_quoted(self._SINGLE_QUOTED, escaped_char="'")
+
+    def _consume_quoted(self, regex, escaped_char=None):
+        value = self._must_consume_regex(regex)[1:-1]
+        if escaped_char is not None:
+            value = value.replace("\\%s" % escaped_char, escaped_char)
+            value = value.replace("\\\\", "\\")
+        return value
+
+    def _double_quoted_value(self):
+        return self._consume_quoted(self._DOUBLE_QUOTED, escaped_char='"')
+
+    def _second_value(self):
+        if self._current() == "'":
+            return self._single_quoted_value()
+        elif self._current() == '"':
+            return self._double_quoted_value()
         else:
-            self._styler = styler
-        self._rendering_index = 0
-        self._column_separator = column_separator
-        if terminal_width is None:
-            self._terminal_width = determine_terminal_width()
-
-    def add_title(self, title):
-        self._current_section.add_title(title)
-
-    def add_row_header(self, headers):
-        self._current_section.add_header(headers)
-
-    def add_row(self, row_elements):
-        self._current_section.add_row(row_elements)
-
-    def new_section(self, title, indent_level=0):
-        self._current_section = Section()
-        self._sections.append(self._current_section)
-        self._current_section.add_title(title)
-        self._current_section.indent_level = indent_level
-
-    def render(self, stream):
-        max_width = self._calculate_max_width()
-        should_convert_table = self._determine_conversion_needed(max_width)
-        if should_convert_table:
-            convert_to_vertical_table(self._sections)
-            max_width = self._calculate_max_width()
-        stream.write('-' * max_width + '\n')
-        for section in self._sections:
-            self._render_section(section, max_width, stream)
-
-    def _determine_conversion_needed(self, max_width):
-        # If we don't know the width of the controlling terminal,
-        # then we don't try to resize the table.
-        if max_width > self._terminal_width:
-            return self._auto_reformat
-
-    def _calculate_max_width(self):
-        max_width = max(s.total_width(padding=4, with_border=True,
-                                      outer_padding=s.indent_level)
-                        for s in self._sections)
-        return max_width
-
-    def _render_section(self, section, max_width, stream):
-        stream = IndentedStream(stream, section.indent_level,
-                                self._styler.style_indentation_char('|'),
-                                self._styler.style_indentation_char('|'))
-        max_width -= (section.indent_level * 2)
-        self._render_title(section, max_width, stream)
-        self._render_column_titles(section, max_width, stream)
-        self._render_rows(section, max_width, stream)
-
-    def _render_title(self, section, max_width, stream):
-        # The title consists of:
-        # title        :  |   This is the title      |
-        # bottom_border:  ----------------------------
-        if section.title:
-            title = self._styler.style_title(section.title)
-            stream.write(center_text(title, max_width, '|', '|',
-                                     len(section.title)) + '\n')
-            if not section.headers and not section.rows:
-                stream.write('+%s+' % ('-' * (max_width - 2)) + '\n')
+            consumed = self._must_consume_regex(self._SECOND_VALUE)
+            return consumed.replace('\\,', ',').rstrip()
+
+    def _expect(self, char, consume_whitespace=False):
+        if consume_whitespace:
+            self._consume_whitespace()
+        if self._index >= len(self._input_value):
+            raise ShorthandParseError(self._input_value, char,
+                                      'EOF', self._index)
+        actual = self._input_value[self._index]
+        if actual != char:
+            raise ShorthandParseError(self._input_value, char,
+                                      actual, self._index)
+        self._index += 1
+        if consume_whitespace:
+            self._consume_whitespace()
+
+    def _must_consume_regex(self, regex):
+        result = regex.match(self._input_value[self._index:])
+        if result is not None:
+            return self._consume_matched_regex(result)
+        raise ShorthandParseError(self._input_value, '<%s>' % regex.name,
+                                  '<none>', self._index)
+
+    def _consume_matched_regex(self, result):
+        start, end = result.span()
+        v = self._input_value[self._index+start:self._index+end]
+        self._index += (end - start)
+        return v
+
+    def _current(self):
+        # If the index is at the end of the input value,
+        # then _EOF will be returned.
+        if self._index < len(self._input_value):
+            return self._input_value[self._index]
+        return _EOF
+
+    def _at_eof(self):
+        return self._index >= len(self._input_value)
+
+    def _backtrack_to(self, char):
+        while self._index >= 0 and self._input_value[self._index] != char:
+            self._index -= 1
+
+    def _consume_whitespace(self):
+        while self._current() != _EOF and self._current() in string.whitespace:
+            self._index += 1
+
+
+class ModelVisitor(object):
+    def visit(self, params, model):
+        self._visit({}, model, '', params)
+
+    def _visit(self, parent, shape, name, value):
+        method = getattr(self, '_visit_%s' % shape.type_name,
+                         self._visit_scalar)
+        method(parent, shape, name, value)
 
-    def _render_column_titles(self, section, max_width, stream):
-        if not section.headers:
+    def _visit_object(self, parent, shape, name, value):
+        if not isinstance(value, dict):
             return
-        # In order to render the column titles we need to know
-        # the width of each of the columns.
-        widths = section.calculate_column_widths(padding=4,
-                                                 max_width=max_width)
-        # TODO: Built a list instead of +=, it's more efficient.
-        current = ''
-        length_so_far = 0
-        # The first cell needs both left and right edges '|  foo  |'
-        # while subsequent cells only need right edges '  foo  |'.
-        first = True
-        for width, header in zip(widths, section.headers):
-            stylized_header = self._styler.style_header_column(header)
-            if first:
-                left_edge = '|'
-                first = False
-            else:
-                left_edge = ''
-            current += center_text(text=stylized_header, length=width,
-                                   left_edge=left_edge, right_edge='|',
-                                   text_length=len(header))
-            length_so_far += width
-        self._write_line_break(stream, widths)
-        stream.write(current + '\n')
-
-    def _write_line_break(self, stream, widths):
-        # Write out something like:
-        # +-------+---------+---------+
-        parts = []
-        first = True
-        for width in widths:
-            if first:
-                parts.append('+%s+' % ('-' * (width - 2)))
-                first = False
-            else:
-                parts.append('%s+' % ('-' * (width - 1)))
-        parts.append('\n')
-        stream.write(''.join(parts))
+        for member_name, member_shape in shape.members.items():
+            self._visit(value, member_shape, member_name,
+                        value.get(member_name))
 
-    def _render_rows(self, section, max_width, stream):
-        if not section.rows:
+    def _visit_map(self, parent, shape, name, value):
+        if not isinstance(value, dict):
             return
-        widths = section.calculate_column_widths(padding=4,
-                                                 max_width=max_width)
-        if not widths:
+        for k, v in value.items():
+            self._visit(value, shape.value, k, v)
+
+    def _visit_array(self, parent, shape, name, value):
+        if not isinstance(value, list):
             return
-        self._write_line_break(stream, widths)
-        for row in section.rows:
-            # TODO: Built the string in a list then join instead of using +=,
-            # it's more efficient.
-            current = ''
-            length_so_far = 0
-            first = True
-            for width, element in zip(widths, row):
-                if first:
-                    left_edge = '|'
-                    first = False
-                else:
-                    left_edge = ''
-                stylized = self._styler.style_row_element(element)
-                current += align_left(text=stylized, length=width,
-                                      left_edge=left_edge,
-                                      right_edge=self._column_separator,
-                                      text_length=len(element))
-                length_so_far += width
-            stream.write(current + '\n')
-        self._write_line_break(stream, widths)
+        for i, element in enumerate(value):
+            self._visit(value, shape.member, i, element)
 
+    def _visit_scalar(self, parent, shape, name, value):
+        pass
 
-class Section(object):
-    def __init__(self):
-        self.title = ''
-        self.headers = []
-        self.rows = []
-        self.indent_level = 0
-        self._num_cols = None
-        self._max_widths = []
-
-    def __repr__(self):
-        return ("Section(title=%s, headers=%s, indent_level=%s, num_rows=%s)" %
-                (self.title, self.headers, self.indent_level, len(self.rows)))
-
-    def calculate_column_widths(self, padding=0, max_width=None):
-        # postcondition: sum(widths) == max_width
-        unscaled_widths = [w + padding for w in self._max_widths]
-        if max_width is None:
-            return unscaled_widths
-        if not unscaled_widths:
-            return unscaled_widths
-        else:
-            # Compute scale factor for max_width.
-            scale_factor = max_width / float(sum(unscaled_widths))
-            scaled = [int(round(scale_factor * w)) for w in unscaled_widths]
-            # Once we've scaled the columns, we may be slightly over/under
-            # the amount we need so we have to adjust the columns.
-            off_by = sum(scaled) - max_width
-            while off_by != 0:
-                iter_order = range(len(scaled))
-                if off_by < 0:
-                    iter_order = reversed(iter_order)
-                for i in iter_order:
-                    if off_by > 0:
-                        scaled[i] -= 1
-                        off_by -= 1
-                    else:
-                        scaled[i] += 1
-                        off_by += 1
-                    if off_by == 0:
-                        break
-            return scaled
-
-    def total_width(self, padding=0, with_border=False, outer_padding=0):
-        total = 0
-        # One char on each side == 2 chars total to the width.
-        border_padding = 2
-        for w in self.calculate_column_widths():
-            total += w + padding
-        if with_border:
-            total += border_padding
-        total += outer_padding + outer_padding
-        return max(len(self.title) + border_padding + outer_padding +
-                   outer_padding, total)
-
-    def add_title(self, title):
-        self.title = title
-
-    def add_header(self, headers):
-        self._update_max_widths(headers)
-        if self._num_cols is None:
-            self._num_cols = len(headers)
-        self.headers = self._format_headers(headers)
-
-    def _format_headers(self, headers):
-        return headers
-
-    def add_row(self, row):
-        if self._num_cols is None:
-            self._num_cols = len(row)
-        if len(row) != self._num_cols:
-            raise ValueError("Row should have %s elements, instead "
-                             "it has %s" % (self._num_cols, len(row)))
-        row = self._format_row(row)
-        self.rows.append(row)
-        self._update_max_widths(row)
-
-    def _format_row(self, row):
-        return [six.text_type(r) for r in row]
-
-    def _update_max_widths(self, row):
-        if not self._max_widths:
-            self._max_widths = [len(el) for el in row]
+
+class BackCompatVisitor(ModelVisitor):
+    def _visit_array(self, parent, shape, name, value):
+        if not isinstance(value, list):
+            # Convert a -> [a] because they specified
+            # "foo=bar", but "bar" should really be ["bar"].
+            if value is not None:
+                parent[name] = [value]
         else:
-            for i, el in enumerate(row):
-                self._max_widths[i] = max(len(el), self._max_widths[i])
+            return super(BackCompatVisitor, self)._visit_array(
+                parent, shape, name, value)
+
+    def _visit_scalar(self, parent, shape, name, value):
+        if value is None:
+            return
+        type_name = shape.type_name
+        if type_name in ['integer', 'long']:
+            parent[name] = int(value)
+        elif type_name in ['double', 'float']:
+            parent[name] = float(value)
+        elif type_name == 'boolean':
+            # We want to make sure we only set a value
+            # only if "true"/"false" is specified.
+            if value.lower() == 'true':
+                parent[name] = True
+            elif value.lower() == 'false':
+                parent[name] = False
```

### Comparing `cdpcli-0.9.9/cdpcli/model.py` & `cdpcli-0.9.90/cdpcli/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 
 def _get_shape_type(shape_data):
     shape_type = shape_data['type']
     if shape_type == 'string':
         if shape_data.get('format', None) == 'date-time':
             return 'datetime'
+        if shape_data.get('format', None) == 'byte':
+            return 'blob'
     if shape_type == 'number':
         return shape_data.get('format')
     if shape_type == 'object':
         if ADDITIONAL_PROPERTIES in shape_data:
             return 'map'
     return shape_type
 
@@ -106,26 +108,31 @@
         return self._shape_data.get('x-paging-page-size', False)
 
     @CachedProperty
     def is_no_paramfile(self):
         return self._shape_data.get('x-no-paramfile', False)
 
     @CachedProperty
-    def is_undocumented(self):
+    def is_deprecated(self):
         return self._shape_data.get('x-deprecated', False)
 
+    @CachedProperty
+    def form_factors(self):
+        if "x-form-factors" in self._shape_data:
+            return self._shape_data['x-form-factors'].split(',')
+        return None
+
     def _get_shape(self, name, shape_data):
         if REF_KEY in shape_data:
             # Reference value type
             # $ref: '#/definitions/SomeObject'
             return self._shape_resolver.resolve_shape_ref(name,
                                                           shape_data[REF_KEY])
         elif TYPE_KEY in shape_data:
-            # Explicit value type
-            # type: SomeShapeType
+            # Explicit value type, e.g., SomeShapeType
             return self._shape_resolver.get_shape(name, shape_data)
         else:
             raise InvalidShapeError("Unknown %s content: %s"
                                     % shape_data, self.name)
 
 
 class ObjectShape(Shape):
@@ -161,14 +168,18 @@
 
 class StringShape(Shape):
     @CachedProperty
     def enum(self):
         return self._shape_data.get('enum', [])
 
     @CachedProperty
+    def deprecated_enum_values(self):
+        return self._shape_data.get('x-deprecated-enum-values', [])
+
+    @CachedProperty
     def supported_options(self):
         return self._shape_data.get('x-supported-options', [])
 
 
 class ShapeResolver(object):
 
     def __init__(self, definitions):
@@ -185,15 +196,16 @@
                 shape_cls = ArrayShape
             elif shape_type == 'string':
                 shape_cls = StringShape
             elif shape_type in ['integer',
                                 'float',
                                 'double',
                                 'boolean',
-                                'datetime']:
+                                'datetime',
+                                'blob']:
                 shape_cls = Shape
             else:
                 raise InvalidShapeError("Unknown shape type: %s" % shape_type)
         except KeyError:
             raise InvalidShapeError("Shape is missing required key 'type': %s"
                                     % (shape_data))
         return shape_cls(name, shape_data, self)
@@ -230,20 +242,25 @@
         return self._name
 
     @property
     def service_model(self):
         return self._service_model
 
     @CachedProperty
+    def summary(self):
+        return self._operation_data["summary"]
+
+    @CachedProperty
     def documentation(self):
         return self._operation_data["description"]
 
     @CachedProperty
     def can_paginate(self):
-        return self._operation_data.get("x-paginates", False)
+        # A valid paginating operation always has x-paging-default-max-items
+        return "x-paging-default-max-items" in self._operation_data
 
     @CachedProperty
     def paging_input_token(self):
         if self.can_paginate:
             for name, shape in self.input_shape.members.items():
                 if shape.is_paging_input_token:
                     return name
@@ -276,22 +293,42 @@
     @CachedProperty
     def paging_default_max_items(self):
         if self.can_paginate:
             return int(self._operation_data.get("x-paging-default-max-items"))
         return None
 
     @CachedProperty
+    def is_deprecated(self):
+        return self._operation_data.get('x-deprecated', False)
+
+    @CachedProperty
+    def form_factors(self):
+        if "x-form-factors" in self._operation_data:
+            return self._operation_data['x-form-factors'].split(',')
+        return None
+
+    @CachedProperty
+    def extensions(self):
+        if "x-extensions" in self._operation_data:
+            return self._operation_data['x-extensions'].split(',')
+        return None
+
+    @CachedProperty
     def input_shape(self):
         return self._service_model.resolve_shape_ref(
             "input", self._operation_data['parameters'][0]['schema'][REF_KEY])
 
     @CachedProperty
     def output_shape(self):
-        return self._service_model.resolve_shape_ref(
-            "output", self._operation_data['responses'][200]['schema'][REF_KEY])
+        if '200' in self._operation_data['responses']:
+            return self._service_model.resolve_shape_ref(
+                "output", self._operation_data['responses']['200']['schema'][REF_KEY])
+        else:
+            return self._service_model.resolve_shape_ref(
+                "output", self._operation_data['responses'][200]['schema'][REF_KEY])
 
 
 class ServiceModel(object):
 
     def __init__(self, service_data, service_name):
         self._service_data = service_data
         self._service_name = service_name
@@ -299,50 +336,76 @@
         self._shape_resolver = ShapeResolver(service_data.get('definitions', {}))
 
     @CachedProperty
     def service_name(self):
         return self._service_name
 
     @CachedProperty
+    def service_version(self):
+        return self._service_data["info"]["version"]
+
+    @CachedProperty
+    def service_title(self):
+        return self._service_data["info"]["title"]
+
+    @CachedProperty
     def documentation(self):
         return self._service_data["info"]["description"]
 
     @instance_cache
     def operation_model(self, operation_name):
         for request_uri in self._service_data["paths"]:
             for http_method in self._service_data["paths"][request_uri]:
                 operation_data = self._service_data["paths"][request_uri][http_method]
                 if operation_data["operationId"] == operation_name:
                     return OperationModel(operation_data,
                                           self,
                                           operation_name,
                                           http_method,
                                           request_uri)
+                if operation_data.get("x-alt-operation-id", None) == operation_name:
+                    operation_data = operation_data.copy()
+                    operation_data["x-deprecated"] = True
+                    return OperationModel(operation_data,
+                                          self,
+                                          operation_name,
+                                          http_method,
+                                          request_uri)
         raise OperationNotFoundError(operation_name)
 
     @CachedProperty
     def operation_names(self):
         operation_names = []
         for path in self._service_data["paths"]:
             for operation in self._service_data["paths"][path]:
-                operation_names.append(
-                    self._service_data["paths"][path][operation]["operationId"])
+                operation_data = self._service_data["paths"][path][operation]
+                operation_names.append(operation_data["operationId"])
+                if "x-alt-operation-id" in operation_data:
+                    operation_names.append(operation_data["x-alt-operation-id"])
         return operation_names
 
     def resolve_shape_ref(self, name, shape_ref):
         return self._shape_resolver.resolve_shape_ref(name, shape_ref)
 
     @CachedProperty
     def endpoint_name(self):
         return self._service_data["x-endpoint-name"]
 
     @CachedProperty
+    def endpoint_prefix(self):
+        return self._service_data.get("x-endpoint-prefix", 'api')
+
+    @CachedProperty
     def products(self):
         return self._service_data.get("x-products", "ALTUS").split(',')
 
+    @CachedProperty
+    def form_factors(self):
+        return self._service_data.get("x-form-factors", "public").split(',')
+
 
 class DenormalizedStructureBuilder(object):
     """Build a StructureShape from a denormalized model.
 
     This is a convenience builder class that makes it easy to construct
     ``StructureShape``s based on a denormalized model.
 
@@ -400,15 +463,16 @@
         elif shape_type == LIST_TYPE:
             shapes[shape_name] = self._build_array(model, shapes)
         elif shape_type in ['string',
                             'integer',
                             'float',
                             'double',
                             'boolean',
-                            'datetime']:
+                            'datetime',
+                            'blob']:
             shapes[shape_name] = self._build_scalar(model)
         else:
             raise InvalidShapeError("Unknown shape type: %s" % model['type'])
 
     def _build_object(self, model, shapes):
         members = OrderedDict()
         shape = self._build_initial_shape(model)
@@ -438,14 +502,16 @@
         shape = {
             'type': model['type'],
         }
         if 'documentation' in model:
             shape['documentation'] = model['documentation']
         if 'enum' in model:
             shape['enum'] = model['enum']
+        if 'x-deprecated-enum-values' in model:
+            shape['x-deprecated-enum-values'] = model['x-deprecated-enum-values']
         if 'x-supported-options' in model:
             shape['x-supported-options'] = model['x-supported-options']
         if 'x-no-paramfile' in model:
             shape['x-no-paramfile'] = model['x-no-paramfile']
         return shape
 
     def _build_scalar(self, model):
```

### Comparing `cdpcli-0.9.9/cdpcli/docs.py` & `cdpcli-0.9.90/cdpcli/docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,65 +16,79 @@
 
 import os
 
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli import SCALAR_TYPES
+from cdpcli import VERSION
 from cdpcli import xform_name
 from cdpcli.argprocess import ParamShorthandDocGen
 from cdpcli.extensions.paginate import add_paging_description
 from cdpcli.model import StringShape
 
 
-def _is_argument_hidden(argument):
-    if getattr(argument, '_UNDOCUMENTED', False):
+MANUAL_SECTION = '1'
+MANUAL_GROUP = 'CDP CLI'
+
+
+def _is_hidden(item):
+    if getattr(item, '_UNDOCUMENTED', False):
+        return True
+    if getattr(item, 'is_deprecated', False):
         return True
     return False
 
 
 def generate_doc(generator, help_command):
     generator.doc_title(help_command)
+    generator.doc_docinfo(help_command)
     generator.doc_description(help_command)
     generator.doc_synopsis_start(help_command)
     if help_command.arg_table:
         for arg_name in help_command.arg_table:
             generator.doc_synopsis_option(arg_name, help_command)
     generator.doc_synopsis_end(help_command)
     generator.doc_options_start(help_command)
     if help_command.arg_table:
         for arg_name in help_command.arg_table:
-            if _is_argument_hidden(help_command.arg_table[arg_name]):
+            if not generator.show_hidden and \
+               _is_hidden(help_command.arg_table[arg_name]):
                 continue
+            generator.doc_option_start(arg_name, help_command)
             generator.doc_option(arg_name, help_command)
             generator.doc_option_example(arg_name, help_command)
+            generator.doc_option_form_factors(arg_name, help_command)
+            generator.doc_option_end(arg_name, help_command)
     generator.doc_options_end(help_command)
     generator.doc_subitems_start(help_command)
     if help_command.command_table:
         for command_name in sorted(help_command.command_table.keys()):
-            if hasattr(help_command.command_table[command_name],
-                       '_UNDOCUMENTED'):
+            if not generator.show_hidden and \
+               _is_hidden(help_command.command_table[command_name]):
                 continue
             generator.doc_subitem(command_name, help_command)
     generator.doc_subitems_end(help_command)
     generator.doc_examples(help_command)
     generator.doc_output(help_command)
+    generator.doc_form_factors(help_command)
     generator.doc_relateditems_start(help_command)
     if help_command.related_items:
         for related_item in sorted(help_command.related_items):
             generator.doc_relateditem(help_command, related_item)
 
 
 class CLIDocumentGenerator(object):
 
-    def __init__(self, help_command):
+    def __init__(self, help_command, show_hidden=False):
         self.help_command = help_command
         self.help_command.doc.translation_map = self.build_translation_map()
         self._arg_groups = self._build_arg_table_groups(help_command)
         self._documented_arg_groups = []
+        self.show_hidden = show_hidden
 
     def _build_arg_table_groups(self, help_command):
         arg_groups = {}
         for name, arg in help_command.arg_table.items():
             if arg.group_name is not None:
                 arg_groups.setdefault(arg.group_name, []).append(arg)
         return arg_groups
@@ -89,14 +103,17 @@
         doc.style.new_paragraph()
         reference = help_command.command_lineage.replace('.', ' ')
         if reference != 'cdp':
             reference = 'cdp ' + reference
         doc.writeln('.. _cli:%s:' % reference)
         doc.style.h1(help_command.name)
 
+    def doc_docinfo(self, help_command):
+        pass
+
     def doc_description(self, help_command):
         doc = help_command.doc
         doc.style.h2('Description')
         doc.include_doc_string(help_command.description)
         doc.style.new_paragraph()
 
     def doc_synopsis_start(self, help_command):
@@ -105,24 +122,26 @@
         doc.style.h2('Synopsis')
         doc.style.start_codeblock()
         doc.writeln('%s' % help_command.name)
 
     def doc_synopsis_option(self, arg_name, help_command):
         doc = help_command.doc
         argument = help_command.arg_table[arg_name]
-        if _is_argument_hidden(argument):
+        if not self.show_hidden and _is_hidden(argument):
             return
         if argument.group_name in self._arg_groups:
             if argument.group_name in self._documented_arg_groups:
                 # This arg is already documented so we can move on.
                 return
             option_str = ' | '.join(
                 [a.cli_name for a in
                  self._arg_groups[argument.group_name]])
             self._documented_arg_groups.append(argument.group_name)
+        elif argument.cli_type_name == 'blob':
+            option_str = '%s <blob>' % argument.cli_name
         else:
             option_str = '%s <value>' % argument.cli_name
         if not argument.required:
             option_str = '[%s]' % option_str
         doc.writeln('%s' % option_str)
 
     def doc_synopsis_end(self, help_command):
@@ -130,90 +149,63 @@
         doc.style.end_codeblock()
         # Reset the documented arg groups for other sections
         # that may document args (the detailed docs following
         # the synopsis).
         self._documented_arg_groups = []
 
     def doc_options_start(self, help_command):
-        doc = help_command.doc
-        doc.style.h2('Options')
-        if not help_command.arg_table:
-            doc.write('*None*\n')
+        pass
 
-    def doc_options_end(self, help_command):
+    def doc_option_start(self, arg_name, help_command):
         pass
 
     def doc_option(self, arg_name, help_command):
-        doc = help_command.doc
-        argument = help_command.arg_table[arg_name]
-        if _is_argument_hidden(argument):
-            return
-        if argument.group_name in self._arg_groups:
-            if argument.group_name in self._documented_arg_groups:
-                # This arg is already documented so we can move on.
-                return
-            name = ' | '.join(
-                ['``%s``' % a.cli_name for a in
-                 self._arg_groups[argument.group_name]])
-            self._documented_arg_groups.append(argument.group_name)
-        else:
-            name = '``%s``' % argument.cli_name
-        doc.write('%s (%s)\n' % (name, argument.cli_type_name))
-        doc.style.indent()
-        doc.include_doc_string(argument.documentation)
-        self._document_enums(argument, doc)
-        doc.style.dedent()
-        doc.style.new_paragraph()
+        pass
 
     def doc_option_example(self, arg_name, help_command):
         pass
 
+    def doc_option_form_factors(self, arg_name, help_command):
+        pass
+
+    def doc_option_end(self, arg_name, help_command):
+        pass
+
+    def doc_options_end(self, help_command):
+        pass
+
     def doc_relateditems_start(self, help_command):
         if help_command.related_items:
             doc = help_command.doc
             doc.style.h2('See Also')
 
     def doc_relateditem(self, help_command, related_item):
         doc = help_command.doc
         doc.write('* ')
         doc.style.sphinx_reference_label(
             label='cli:%s' % related_item,
             text=related_item
         )
         doc.write('\n')
 
-    def _document_enums(self, argument, doc):
-        if hasattr(argument, 'argument_model'):
-            model = argument.argument_model
-            if isinstance(model, StringShape):
-                if model.enum:
-                    self._write_possible_values(doc, model.enum)
-                if model.supported_options:
-                    self._write_possible_values(doc, model.supported_options)
-
-    def _write_possible_values(self, doc, possible_values):
-        doc.style.new_paragraph()
-        doc.write('Possible values:')
-        doc.style.start_ul()
-        for value in possible_values:
-            doc.style.li('``%s``' % value)
-        doc.style.end_ul()
-
     def doc_subitems_start(self, help_command):
         pass
 
     def doc_subitems_end(self, help_command):
         pass
 
     def doc_examples(self, help_command):
         pass
 
     def doc_output(self, help_command):
         pass
 
+    def doc_form_factors(self, help_command):
+        pass
+
 
 class ProviderDocumentGenerator(CLIDocumentGenerator):
 
     def doc_synopsis_start(self, help_command):
         doc = help_command.doc
         doc.style.h2('Synopsis')
         doc.style.codeblock(help_command.synopsis)
@@ -226,35 +218,52 @@
         doc = help_command.doc
         doc.style.new_paragraph()
 
     def doc_options_start(self, help_command):
         doc = help_command.doc
         doc.style.h2('Options')
 
+    def doc_option_start(self, arg_name, help_command):
+        pass
+
     def doc_option(self, arg_name, help_command):
         doc = help_command.doc
         argument = help_command.arg_table[arg_name]
         doc.writeln('``%s`` (%s)' % (argument.cli_name,
                                      argument.cli_type_name))
         doc.include_doc_string(argument.documentation)
         if argument.choices:
             doc.style.start_ul()
             for choice in argument.choices:
                 doc.style.li(choice)
             doc.style.end_ul()
 
+    def doc_option_example(self, arg_name, help_command):
+        pass
+
+    def doc_option_form_factors(self, arg_name, help_command):
+        pass
+
+    def doc_option_end(self, arg_name, help_command):
+        pass
+
+    def doc_options_end(self, help_command):
+        pass
+
     def doc_subitems_start(self, help_command):
         doc = help_command.doc
-        doc.style.h2('Available Services')
+        doc.style.h2('Available Commands')
         doc.style.toctree()
 
     def doc_subitem(self, command_name, help_command):
         doc = help_command.doc
+        command = help_command.command_table[command_name]
+        is_deprecated = ' (deprecated)' if _is_hidden(command) else ''
         file_name = '%s/index' % command_name
-        doc.style.tocitem(command_name, file_name=file_name)
+        doc.style.tocitem(command_name + is_deprecated, file_name=file_name)
 
 
 class ServiceDocumentGenerator(CLIDocumentGenerator):
 
     def build_translation_map(self):
         d = {}
         service_model = self.help_command.obj
@@ -272,47 +281,70 @@
     def doc_synopsis_end(self, help_command):
         pass
 
     # A service document has no option section.
     def doc_options_start(self, help_command):
         pass
 
+    def doc_option_start(self, arg_name, help_command):
+        pass
+
     def doc_option(self, arg_name, help_command):
         pass
 
     def doc_option_example(self, arg_name, help_command):
         pass
 
+    def doc_option_form_factors(self, arg_name, help_command):
+        pass
+
+    def doc_option_end(self, arg_name, help_command):
+        pass
+
     def doc_options_end(self, help_command):
         pass
 
+    def doc_docinfo(self, help_command):
+        doc = help_command.doc
+        service_model = help_command.obj
+        doc.style.simple_field('subtitle', service_model.service_title)
+        service_version = service_model.service_version
+        # Goes away once each service has its own version number
+        if service_version == '__API_VERSION__':
+            service_version = VERSION
+        doc.style.simple_field('version', service_version)
+        if help_command.include_man_fields:
+            doc.style.simple_field('manual_section', MANUAL_SECTION)
+            doc.style.simple_field('manual_group', MANUAL_GROUP)
+
     def doc_description(self, help_command):
         doc = help_command.doc
         service_model = help_command.obj
         doc.style.h2('Description')
         # TODO: need a documentation attribute.
         doc.include_doc_string(service_model.documentation)
 
     def doc_subitems_start(self, help_command):
         doc = help_command.doc
-        doc.style.h2('Available Commands')
+        doc.style.h2('Available Subcommands')
         doc.style.toctree()
 
     def doc_subitem(self, command_name, help_command):
         doc = help_command.doc
         subcommand = help_command.command_table[command_name]
+        is_deprecated = ' (deprecated)' if _is_hidden(subcommand) else ''
         subcommand_table = getattr(subcommand, 'subcommand_table', {})
         # If the subcommand table has commands in it,
         # direct the subitem to the command's index because
         # it has more subcommands to be documented.
         if (len(subcommand_table) > 0):
             file_name = '%s/index' % command_name
-            doc.style.tocitem(command_name, file_name=file_name)
+            doc.style.tocitem(command_name + is_deprecated, file_name=file_name)
         else:
-            doc.style.tocitem(command_name)
+            doc.style.tocitem(command_name + is_deprecated)
 
 
 class OperationDocumentGenerator(CLIDocumentGenerator):
 
     def build_translation_map(self):
         operation_model = self.help_command.obj
         d = {}
@@ -334,27 +366,48 @@
                         d[argument_name] = cli_name
                 else:
                     d[argument_name] = cli_name
         for operation_name in operation_model.service_model.operation_names:
             d[operation_name] = xform_name(operation_name, '-')
         return d
 
+    def doc_docinfo(self, help_command):
+        doc = help_command.doc
+        operation_model = help_command.obj
+        # Internal commands like "configure" may lack these (see BasicDocHandler)
+        if hasattr(operation_model, 'summary'):
+            doc.style.simple_field('subtitle', operation_model.summary)
+        if hasattr(operation_model, 'service_model') and\
+                hasattr(operation_model.service_model, 'service_version'):
+            service_version = operation_model.service_model.service_version
+            # Goes away once each service has its own version number
+            if service_version == '__API_VERSION__':
+                service_version = VERSION
+            doc.style.simple_field('version', service_version)
+        if help_command.include_man_fields:
+            doc.style.simple_field('manual_section', MANUAL_SECTION)
+            doc.style.simple_field('manual_group', MANUAL_GROUP)
+
     def doc_description(self, help_command):
         doc = help_command.doc
         operation_model = help_command.obj
         doc.style.h2('Description')
         doc.include_doc_string(operation_model.documentation)
         add_paging_description(help_command)
 
     def _json_example_value_name(self, argument_model, include_enum_values=True):
         # If include_enum_values is True, then the valid enum values
         # are included as the sample JSON value.
         if isinstance(argument_model, StringShape):
             if argument_model.enum and include_enum_values:
                 choices = argument_model.enum
+                if not self.show_hidden and argument_model.deprecated_enum_values:
+                    choices = [item
+                               for item in choices
+                               if item not in argument_model.deprecated_enum_values]
                 return '|'.join(['"%s"' % c for c in choices])
             elif argument_model.supported_options and include_enum_values:
                 choices = argument_model.supported_options
                 return '|'.join(['"%s"' % c for c in choices])
             else:
                 return '"string"'
         elif argument_model.type_name == 'boolean':
@@ -446,18 +499,57 @@
                 if need_comma:
                     doc.write(',')
                     doc.style.new_line()
                 doc.write('"%s": ' % member_name)
                 self._json_example(doc, member_model, stack)
                 need_comma = True
 
+    def doc_options_start(self, help_command):
+        doc = help_command.doc
+        doc.style.h2('Options')
+        if not help_command.arg_table:
+            doc.write('*None*\n')
+
+    def doc_option_start(self, arg_name, help_command):
+        pass
+
+    def doc_option(self, arg_name, help_command):
+        doc = help_command.doc
+        argument = help_command.arg_table[arg_name]
+        is_deprecated = ''
+        if _is_hidden(argument):
+            if not self.show_hidden:
+                return
+            else:
+                is_deprecated = ' (deprecated)'
+        if argument.group_name in self._arg_groups:
+            if argument.group_name in self._documented_arg_groups:
+                # This arg is already documented so we can move on.
+                return
+            name = ' | '.join(
+                ['``%s``' % a.cli_name for a in
+                 self._arg_groups[argument.group_name]])
+        else:
+            name = '``%s``' % argument.cli_name
+        doc.write('%s (%s)%s\n' % (name, argument.cli_type_name, is_deprecated))
+        doc.style.indent()
+        doc.style.new_paragraph()
+        doc.include_doc_string(argument.documentation)
+        self._document_enums(argument, doc)
+        if hasattr(argument.argument_model, 'members'):
+            doc.style.new_paragraph()
+            for member_name, member_shape in argument.argument_model.members.items():
+                self.doc_member(doc, member_name, member_shape, stack=[])
+        doc.style.dedent()
+        doc.style.new_paragraph()
+
     def doc_option_example(self, arg_name, help_command):
         doc = help_command.doc
         cli_argument = help_command.arg_table[arg_name]
-        if _is_argument_hidden(cli_argument):
+        if not self.show_hidden and _is_hidden(cli_argument):
             return
         if cli_argument.group_name in self._arg_groups:
             if cli_argument.group_name in self._documented_arg_groups:
                 # Args with group_names (boolean args) don't
                 # need to generate example syntax.
                 return
         argument_model = cli_argument.argument_model
@@ -491,85 +583,154 @@
             doc.write('Syntax')
             doc.style.start_codeblock()
             example_type = self._json_example_value_name(
                 member, include_enum_values=False)
             doc.write('%s %s ...' % (example_type, example_type))
             if isinstance(member, StringShape):
                 if member.enum:
-                    self._write_possible_values(doc, member.enum)
+                    enum_values = member.enum
+                    if not self.show_hidden and member.deprecated_enum_values:
+                        enum_values = [v for v in enum_values
+                                       if v not in member.deprecated_enum_values]
+                    self._write_possible_values(doc, enum_values)
                 if member.supported_options:
                     self._write_possible_values(doc, member.supported_options)
             doc.style.end_codeblock()
             doc.style.new_paragraph()
         elif cli_argument.cli_type_name not in SCALAR_TYPES:
             doc.style.new_paragraph()
             doc.write('JSON Syntax')
             doc.style.start_codeblock()
             self._json_example(doc, argument_model, stack=[])
             doc.style.end_codeblock()
             doc.style.new_paragraph()
 
-    def _write_possible_values(self, doc, possible_values):
-        doc.style.new_paragraph()
-        doc.write("Possible values:\n")
-        for value in possible_values:
-            doc.write("    %s\n" % value)
-        doc.write("\n")
+    def doc_option_form_factors(self, arg_name, help_command):
+        doc = help_command.doc
+        argument = help_command.arg_table[arg_name]
+        if not self.show_hidden and _is_hidden(argument):
+            return
+        if argument.group_name in self._arg_groups:
+            if argument.group_name in self._documented_arg_groups:
+                # This arg is already documented so we can move on.
+                return
+        if argument.argument_model.form_factors is not None:
+            self._write_form_factors(doc, argument.argument_model.form_factors)
+
+    def doc_option_end(self, arg_name, help_command):
+        argument = help_command.arg_table[arg_name]
+        if argument.group_name in self._arg_groups:
+            if argument.group_name in self._documented_arg_groups:
+                # This arg is already documented so we can move on.
+                return
+            self._documented_arg_groups.append(argument.group_name)
+
+    def doc_options_end(self, help_command):
+        pass
 
     def doc_output(self, help_command):
         doc = help_command.doc
         doc.style.h2('Output')
         operation_model = help_command.obj
         output_shape = operation_model.output_shape
         if output_shape is None:
             doc.write('None')
         else:
             for member_name, member_shape in output_shape.members.items():
-                self._doc_member_for_output(doc, member_name, member_shape, stack=[])
+                self.doc_member(doc, member_name, member_shape, stack=[])
+
+    def doc_examples(self, help_command):
+        operation = help_command.command_lineage.replace('.', os.path.sep)
+        doc_path = os.path.dirname(os.path.abspath(__file__))
+        doc_path = os.path.join(doc_path, 'examples')
+        doc_path = os.path.join(doc_path, operation) + '.rst'
+        if os.path.isfile(doc_path):
+            help_command.doc.style.h2('Examples')
+            fp = open(doc_path)
+            for line in fp.readlines():
+                help_command.doc.write(line)
+
+    def doc_form_factors(self, help_command):
+        operation_model = help_command.obj
+        form_factors = getattr(operation_model, 'form_factors', None)
+        if not form_factors:
+            service_model = getattr(operation_model, 'service_model', None)
+            if service_model:
+                form_factors = getattr(service_model, 'form_factors', None)
+        if form_factors:
+            doc = help_command.doc
+            doc.style.h2('Form Factors')
+            doc.write(', '.join(form_factors))
+            doc.style.new_paragraph()
 
-    def _doc_member_for_output(self, doc, member_name, member_shape, stack):
+    def doc_member(self, doc, member_name, member_shape, stack):
         if member_shape.name in stack:
             # Document the recursion once, otherwise just
             # note the fact that it's recursive and return.
             if stack.count(member_shape.name) > 1:
                 if member_shape.type_name == OBJECT_TYPE:
                     doc.write('( ... recursive ... )')
                 return
         stack.append(member_shape.name)
         try:
-            self._do_doc_member_for_output(doc, member_name,
-                                           member_shape, stack)
+            self._do_doc_member(doc, member_name,
+                                member_shape, stack)
         finally:
             stack.pop()
 
-    def _do_doc_member_for_output(self, doc, member_name, member_shape, stack):
+    def _do_doc_member(self, doc, member_name, member_shape, stack):
+        is_deprecated = ''
+        if _is_hidden(member_shape):
+            if not self.show_hidden:
+                return
+            else:
+                is_deprecated = ' (deprecated)'
         docs = member_shape.documentation
         if member_name:
-            doc.write('%s -> (%s)' % (member_name, member_shape.type_name))
+            doc.write('%s -> (%s)%s' %
+                      (member_name, member_shape.type_name, is_deprecated))
         else:
-            doc.write('(%s)' % member_shape.type_name)
+            doc.write('(%s)%s' % member_shape.type_name, is_deprecated)
         doc.style.indent()
         doc.style.new_paragraph()
         doc.include_doc_string(docs)
+        if member_shape.form_factors is not None:
+            self._write_form_factors(doc, member_shape.form_factors)
         doc.style.new_paragraph()
         member_type_name = member_shape.type_name
         if member_type_name == OBJECT_TYPE:
             for sub_name, sub_shape in member_shape.members.items():
-                self._doc_member_for_output(doc, sub_name, sub_shape, stack)
+                self.doc_member(doc, sub_name, sub_shape, stack)
         elif member_type_name == LIST_TYPE:
-            self._doc_member_for_output(doc, '', member_shape.member, stack)
+            self.doc_member(doc, 'item', member_shape.member, stack)
         elif member_type_name == MAP_TYPE:
-            self._doc_member_for_output(doc, 'key', member_shape.key, stack)
-            self._doc_member_for_output(doc, 'value', member_shape.value, stack)
+            self.doc_member(doc, 'key', member_shape.key, stack)
+            self.doc_member(doc, 'value', member_shape.value, stack)
         doc.style.dedent()
         doc.style.new_paragraph()
 
-    def doc_examples(self, help_command):
-        operation = help_command.command_lineage.replace('.', os.path.sep)
-        doc_path = os.path.dirname(os.path.abspath(__file__))
-        doc_path = os.path.join(doc_path, 'examples')
-        doc_path = os.path.join(doc_path, operation) + '.rst'
-        if os.path.isfile(doc_path):
-            help_command.doc.style.h2('Examples')
-            fp = open(doc_path)
-            for line in fp.readlines():
-                help_command.doc.write(line)
+    def _document_enums(self, argument, doc):
+        if hasattr(argument, 'argument_model'):
+            model = argument.argument_model
+            if isinstance(model, StringShape):
+                if model.enum:
+                    enum_values = model.enum
+                    if not self.show_hidden and model.deprecated_enum_values:
+                        enum_values = [v for v in enum_values
+                                       if v not in model.deprecated_enum_values]
+                    self._write_possible_values(doc, enum_values)
+                if model.supported_options:
+                    self._write_possible_values(doc, model.supported_options)
+
+    def _write_possible_values(self, doc, possible_values):
+        doc.style.new_paragraph()
+        doc.write('Possible values:')
+        doc.style.start_ul()
+        for value in possible_values:
+            doc.style.li('``%s``' % value)
+        doc.style.end_ul()
+
+    def _write_form_factors(self, doc, form_factors):
+        doc.style.new_paragraph()
+        doc.write('Form Factors: ')
+        doc.write(', '.join(form_factors))
+        doc.style.new_paragraph()
```

### Comparing `cdpcli-0.9.9/cdpcli/arguments.py` & `cdpcli-0.9.90/cdpcli/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         if serialized_name is None:
             serialized_name = name
         self._serialized_name = serialized_name
         self.argument_model = argument_model
         self._required = is_required
         self._operation_model = operation_model
         self.no_paramfile = no_paramfile
-        self._UNDOCUMENTED = self.argument_model.is_undocumented
+        self._UNDOCUMENTED = self.argument_model.is_deprecated
 
     @property
     def py_name(self):
         return self._name.replace('-', '_')
 
     @property
     def required(self):
```

### Comparing `cdpcli-0.9.9/cdpcli/loader.py` & `cdpcli-0.9.90/cdpcli/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     # returns a list of actual existing directories among search paths
     def _potential_locations(self):
         for path in self._search_paths:
             if os.path.isdir(path):
                 yield path
 
     # lists potential service names in a given search path
-    # which is obtained by sallow listing of subdirectories
+    # which is obtained by shallow listing of subdirectories
     def _potential_services(self, path):
         for child in os.listdir(path):
             full_path = os.path.join(path, child)
             if os.path.isdir(full_path):
                 yield (child, full_path)
 
     def _load_builtin_aliases(self):
```

### Comparing `cdpcli-0.9.9/cdpcli/configloader.py` & `cdpcli-0.9.90/cdpcli/configloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
+import configparser
 import copy
 import os
 import shlex
 
 from cdpcli.exceptions import ConfigNotFound, ConfigParseError
-from six.moves import configparser
 
 
 def multi_file_load_config(*filenames):
     """Load and combine multiple INI configs with profiles.
 
     This function will take a list of filesnames and return
     a single dictionary that represents the merging of the loaded
```

### Comparing `cdpcli-0.9.9/cdpcli/text.py` & `cdpcli-0.9.90/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/translate.py` & `cdpcli-0.9.90/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/auth.py` & `cdpcli-0.9.90/cdpcli/auth.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from base64 import b64decode, urlsafe_b64encode
 from email.utils import formatdate
+import hashlib
 import logging
 
 from asn1crypto import keys, pem
 from cdpcli.compat import json
 from cdpcli.compat import OrderedDict
 from cdpcli.compat import urlsplit
 from cdpcli.exceptions import NoCredentialsError
+from ecdsa import SigningKey
+from ecdsa.util import sigencode_der
 from pure25519 import eddsa
 import rsa
 
 
 LOG = logging.getLogger('cdpcli.auth')
 
 
@@ -89,15 +92,16 @@
     def _get_signature(self, method, split, headers):
         string_to_sign = self._canonical_string(method, split, headers)
         LOG.debug('StringToSign:\n%s', string_to_sign)
         return self._sign_string(string_to_sign)
 
     def add_auth(self, request):
         if self.credentials is None:
-            raise NoCredentialsError
+            raise NoCredentialsError(
+                err_msg='Credentials not available for request signing')
         LOG.debug("Calculating signature using %s." % self.auth_method)
         LOG.debug('HTTP request method: %s', request.method)
         split = urlsplit(request.url)
         signature = self._get_signature(request.method,
                                         split,
                                         request.headers)
         self._inject_signature(request, signature)
@@ -194,11 +198,100 @@
             LOG.debug(message, exc_info=True)
             raise Exception(message)
         # We sign the hash.
         signature = rsa.sign(string_to_sign.encode('utf-8'), key, 'SHA-256')
         return signature
 
 
+class ECDSAv1Auth(V1Signer):
+    """
+    ECDSA signing with a SHA-512 hash returning a base64 encoded signature.
+    """
+    AUTH_METHOD_NAME = 'ecdsav1'
+
+    def __init__(self, credentials):
+        super(ECDSAv1Auth, self).__init__(credentials, self.AUTH_METHOD_NAME)
+
+    @staticmethod
+    def _parse_private_key(private_key, error_message="Failed to import private key."):
+        """
+        Parse the ECDSA private key.
+        :param private_key: The private key.
+        :return: The SigningKey.
+        :raise: Exception if the private key can not be parsed.
+        """
+        try:
+            # We expect the private key to be a PKCS8 pem formatted string.
+            pem_bytes = private_key.encode('utf-8')
+            if pem.detect(pem_bytes):
+                _, _, der_bytes = pem.unarmor(pem_bytes)
+                # In PKCS8 the key is wrapped in a container that describes it
+                info = keys.PrivateKeyInfo.load(der_bytes, strict=True)
+                # Directly unwrap the private key. The asn1crypto library stopped
+                # offering an API call for this in their 1.0.0 release but their
+                # official answer of using a separate native-code-dependent
+                # library to do one line of work is unreasonable. Of course, this
+                # line might break in the future...
+                unwrapped = info['private_key'].parsed
+                # The unwrapped key is equivalent to pkcs1 contents
+                return SigningKey.from_der(unwrapped.dump())
+            else:
+                raise Exception('Not a PEM file')
+        except Exception:
+            LOG.debug(error_message, exc_info=True)
+            raise Exception(error_message)
+
+    @staticmethod
+    def detect_private_key(private_key):
+        """
+        Try to see if the private key is an ECDSA key by parsing it.
+        :param private_key: The key to check.
+        :return: True if the key is an ECDSA key, False otherwise.
+        """
+        try:
+            ECDSAv1Auth._parse_private_key(private_key)
+            return True
+        except Exception:
+            return False
+
+    def _raw_sign_string(self, string_to_sign):
+        """
+        Sign the supplied string using the credentials and return the raw signature.
+        :param string_to_sign: String to sign
+        :return: Raw signature as string
+        """
+        sk = ECDSAv1Auth._parse_private_key(
+            self.credentials.private_key,
+            self.ERROR_MESSAGE % self.credentials.method)
+        # Sign the hash.
+        signature = sk.sign_deterministic(
+            string_to_sign.encode('utf-8'),
+            hashfunc=hashlib.sha512,
+            sigencode=sigencode_der)
+        return signature
+
+
+class AccessTokenAuth:
+    AUTH_METHOD_NAME = 'access_token'
+
+    def __init__(self, credentials):
+        self._credentials = credentials
+
+    def add_auth(self, request):
+        if self._credentials is None:
+            raise NoCredentialsError(
+                err_msg='Credentials not available for request signing')
+        if 'Authorization' in request.headers:
+            raise Exception("Authorization found in headers!")
+        request.headers['Authorization'] = self._credentials.access_token
+
+    @classmethod
+    def is_access_token(cls, access_token):
+        return bool(access_token)
+
+
 AUTH_TYPE_MAPS = {
+    ECDSAv1Auth.AUTH_METHOD_NAME: ECDSAv1Auth,
     Ed25519v1Auth.AUTH_METHOD_NAME: Ed25519v1Auth,
     RSAv1Auth.AUTH_METHOD_NAME: RSAv1Auth,
+    AccessTokenAuth.AUTH_METHOD_NAME: AccessTokenAuth
 }
```

### Comparing `cdpcli-0.9.9/cdpcli/argparser.py` & `cdpcli-0.9.90/cdpcli/argparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,36 +13,24 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import argparse
 from difflib import get_close_matches
 import logging
+import os
 import sys
 
 from cdpcli import ARGPARSE_DASH_ENCODING
 from cdpcli.compat import six
 
 
 LOG = logging.getLogger('cdpcli.argparser')
 
 
-HELP_BLURB = (
-    "To see help text, you can run:\n"
-    "\n"
-    "  cdp help\n"
-    "  cdp <command> help\n"
-    "  cdp <command> <subcommand> help\n"
-)
-USAGE = (
-    "cdp [options] <command> <subcommand> [<subcommand> ...] [parameters]\n"
-    "%s" % HELP_BLURB
-)
-
-
 class CLIArgParser(argparse.ArgumentParser):
     Formatter = argparse.RawTextHelpFormatter
 
     # When displaying invalid choice error messages, this controls how many
     # options to show per line.
     ChoicesPerLine = 2
 
@@ -50,19 +38,21 @@
         """
         It's probably not a great idea to override a "hidden" method but the default
         behavior is pretty ugly and there doesn't seem to be any other way to change
         it.
         """
         # converted value must be one of the choices (if specified)
         if action.choices is not None and value not in action.choices:
+            choice_max_len = len(max(action.choices, key=len))
+            column_width = max(choice_max_len, 40)
             msg = ['Invalid choice, valid choices are:\n']
             for i in range(len(action.choices))[::self.ChoicesPerLine]:
                 current = []
                 for choice in action.choices[i:i + self.ChoicesPerLine]:
-                    current.append('%-40s' % choice)
+                    current.append(('%-' + str(column_width) + 's') % choice)
                 msg.append(' | '.join(current))
             possible = get_close_matches(value, action.choices, cutoff=0.8)
             if possible:
                 extra = ['\n\nInvalid choice: %r, maybe you meant:\n' % value]
                 for word in possible:
                     extra.append('  * %s' % word)
                 msg.extend(extra)
@@ -120,16 +110,17 @@
                  description,
                  argument_table):
         super(MainArgParser, self).__init__(
             formatter_class=self.Formatter,
             add_help=False,
             conflict_handler='resolve',
             description=description,
-            usage=USAGE)
+            allow_abbrev=False)
         self._build(command_table, version_string, argument_table)
+        self._command_table = command_table
 
     def _create_choice_help(self, choices):
         help_str = ''
         for choice in sorted(choices):
             help_str += '* %s\n' % choice
         return help_str
 
@@ -139,54 +130,75 @@
             argument.add_to_parser(self)
         self.add_argument('--version',
                           action="version",
                           version=version_string,
                           help='Display the version of this tool')
         self.add_argument('command', choices=list(command_table.keys()))
 
+    def parse_known_args(self, args, namespace=None):
+        """
+        Parses normally, but also adds the command_table to the parsed
+        arguments, so that commands like refdoc may access it. This is a hack.
+        """
+        parsed, remaining = super(MainArgParser, self).parse_known_args(args, namespace)
+        setattr(parsed, 'command_table', self._command_table)
+        return parsed, remaining
+
 
 class ArgTableArgParser(CLIArgParser):
 
-    def __init__(self, argument_table, command_table=None):
+    def __init__(self, argument_table, service_name=None, operation_name=None,
+                 command_table=None):
         # command_table is an optional subcommand_table.  If it's passed
         # in, then we'll update the argparse to parse a 'subcommand' argument
         # and populate the choices field with the command table keys.
+        if service_name and operation_name:
+            progString = "{} {} {}".format(os.path.basename(sys.argv[0]), service_name,
+                                           operation_name)
+        else:
+            progString = os.path.basename(sys.argv[0])
         super(ArgTableArgParser, self).__init__(
+            prog=progString,
             formatter_class=self.Formatter,
             add_help=False,
-            usage=USAGE,
             conflict_handler='resolve')
         if command_table is None:
             command_table = {}
         self._build(argument_table, command_table)
 
     def _build(self, argument_table, command_table):
         for arg_name in argument_table:
             argument = argument_table[arg_name]
             argument.add_to_parser(self)
         if command_table:
             self.add_argument('subcommand', choices=list(command_table.keys()),
                               nargs='?')
 
     def parse_known_args(self, args, namespace=None):
-        if len(args) == 1 and args[0] == 'help':
+        if len(args) == 1 and (args[0] == 'help' or args[0] == '--help'):
             namespace = argparse.Namespace()
             namespace.help = 'help'
             return namespace, []
         else:
             return super(ArgTableArgParser, self).parse_known_args(
                 args, namespace)
 
 
 class ServiceArgParser(CLIArgParser):
 
     def __init__(self, operations_table, service_name):
         super(ServiceArgParser, self).__init__(
+            prog="{} {}".format(os.path.basename(sys.argv[0]), service_name),
             formatter_class=argparse.RawTextHelpFormatter,
             add_help=False,
-            conflict_handler='resolve',
-            usage=USAGE)
+            conflict_handler='resolve')
         self._build(operations_table)
         self._service_name = service_name
 
     def _build(self, operations_table):
         self.add_argument('operation', choices=list(operations_table.keys()))
+
+    def parse_known_args(self, args, namespace=None):
+        if len(args) == 0 or (len(args) == 1 and args[0] == '--help'):
+            args = ['help']
+        return super(ServiceArgParser, self).parse_known_args(
+            args, namespace)
```

### Comparing `cdpcli-0.9.9/cdpcli/textwriter.py` & `cdpcli-0.9.90/cdpcli/textwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,14 +766,20 @@
         raise nodes.SkipNode
 
     def visit_raw(self, node):
         if 'text' in node.get('format', '').split():
             self.body.append(node.astext())
         raise nodes.SkipNode
 
+    def visit_docinfo(self, node):
+        raise nodes.SkipNode
+
+    def visit_version(self, node):
+        raise nodes.SkipNode
+
     def _visit_admonition(self, node):
         self.new_state(2)
 
     def _make_depart_admonition(name):
         def depart_admonition(self, node):
             self.end_state(first=name.capitalize() + ': ')
         return depart_admonition
```

### Comparing `cdpcli-0.9.9/cdpcli/help.py` & `cdpcli-0.9.90/cdpcli/help.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # language governing permissions and limitations under the License.
 
 import os
 import platform
 import shlex
 from subprocess import PIPE
 from subprocess import Popen
+import sys
 
 from cdpcli.argparser import ArgTableArgParser
 from cdpcli.argprocess import ParamShorthand
 from cdpcli.doc.restdoc import ReSTDocument
 from cdpcli.docs import generate_doc
 from cdpcli.docs import OperationDocumentGenerator
 from cdpcli.docs import ProviderDocumentGenerator
@@ -41,15 +42,33 @@
     """
     if platform.system() == 'Windows':
         return WindowsHelpRenderer()
     else:
         return PosixHelpRenderer()
 
 
+class NullRenderer(object):
+    """
+    A renderer that does not render anything. Use this when the goal is only
+    to populate the help command's doc object.
+    """
+
+    def render(self, contents):
+        pass
+
+
 class PagingHelpRenderer(object):
+    """
+    Interface for a help renderer.
+    The renderer is responsible for displaying the help content on
+    a particular platform.
+    """
+    def __init__(self, output_stream=sys.stdout):
+        self.output_stream = output_stream
+
     PAGER = None
 
     def get_pager_cmdline(self):
         pager = self.PAGER
         if 'MANPAGER' in os.environ:
             pager = os.environ['MANPAGER']
         elif 'PAGER' in os.environ:
@@ -77,20 +96,23 @@
 
 
 class PosixHelpRenderer(PagingHelpRenderer):
     PAGER = 'less -R'
 
     def _convert_doc_content(self, contents):
         man_contents = publish_string(contents, writer=manpage.Writer())
-        if not self._exists_on_path('groff'):
-            raise ExecutableNotFoundError(executable_name='groff')
-        cmdline = ['groff', '-man', '-T', 'ascii']
+        if self._exists_on_path('groff'):
+            cmdline = ['groff', '-m', 'man', '-T', 'ascii']
+        elif self._exists_on_path('mandoc'):
+            cmdline = ['mandoc', '-T', 'ascii']
+        else:
+            raise ExecutableNotFoundError(executable_name='groff or mandoc')
         p3 = self._popen(cmdline, stdin=PIPE, stdout=PIPE, stderr=PIPE)
-        groff_output = p3.communicate(input=man_contents)[0]
-        return groff_output
+        output = p3.communicate(input=man_contents)[0]
+        return output
 
     def _send_output_to_pager(self, output):
         cmdline = self.get_pager_cmdline()
         with ignore_ctrl_c():
             # We can't rely on the KeyboardInterrupt from
             # the CLIDriver being caught because when we
             # send the output to a pager it will use various
@@ -128,22 +150,23 @@
         kwargs['shell'] = True
         return Popen(*args, **kwargs)
 
 
 class HelpCommand(object):
     GeneratorClass = None
 
-    def __init__(self, obj, command_table, arg_table):
+    def __init__(self, obj, command_table, arg_table, include_man_fields=True):
         self.obj = obj
         if command_table is None:
             command_table = {}
         self.command_table = command_table
         if arg_table is None:
             arg_table = {}
         self.arg_table = arg_table
+        self.include_man_fields = include_man_fields
         self._subcommand_table = {}
         self._related_items = []
         self.renderer = get_renderer()
         self.doc = ReSTDocument(target='man')
 
     @property
     def command_lineage(self):
@@ -159,21 +182,22 @@
 
     @property
     def related_items(self):
         return self._related_items
 
     def __call__(self, client_creator, args, parsed_globals):
         if args:
-            subcommand_parser = ArgTableArgParser({}, self.subcommand_table)
+            subcommand_parser = ArgTableArgParser({}, command_table=self.subcommand_table)
             parsed, remaining = subcommand_parser.parse_known_args(args)
             if getattr(parsed, 'subcommand', None) is not None:
                 return self.subcommand_table[parsed.subcommand](remaining,
                                                                 parsed_globals)
 
-        generate_doc(self.GeneratorClass(self), self)
+        show_deprecated = parsed_globals.deprecated
+        generate_doc(self.GeneratorClass(self, show_hidden=show_deprecated), self)
         self.renderer.render(self.doc.getvalue())
 
 
 class ProviderHelpCommand(HelpCommand):
     GeneratorClass = ProviderDocumentGenerator
 
     def __init__(self, command_table, arg_table, description, synopsis, usage):
```

### Comparing `cdpcli-0.9.9/cdpcli/utils.py` & `cdpcli-0.9.90/cdpcli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,34 +13,63 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import contextlib
 import datetime
 import functools
+import importlib
 import re
 import signal
+import urllib.parse as urlparse
 
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli.compat import compat_tzlocal
 from cdpcli.compat import OrderedDict
 import dateutil.parser
 from dateutil.tz import tzutc
 
 # These are chars that do not need to be urlencoded based on rfc2986, section 2.3.
 SAFE_CHARS = '-._~'
 
 
+def import_module(module_name):
+    try:
+        return importlib.import_module(module_name)
+    except ImportError:
+        return None
+
+
+def get_extension_registers(name):
+    module = import_module('cdpcli.extensions.%s.register' % name)
+    if module is None:
+        module = import_module('cdpcli.extensions.%s' % name)
+    if module is None:
+        return None, None
+
+    register = getattr(module, 'register', None)
+    if register is not None:
+        return register, None
+
+    register_ext = getattr(module, 'register_extension', None)
+    register_cmd = getattr(module, 'register_command', None)
+    return register_ext, register_cmd
+
+
+def is_absolute_url(url):
+    return bool(urlparse.urlparse(url).netloc)
+
+
 def get_service_module_name(service_model):
     name = service_model.service_name
     name = name.replace('Cloudera', '')
     name = name.replace('CDP', '')
-    name = re.sub('\W+', '', name)
+    name = re.sub('\\W+', '', name)
     return name
 
 
 def json_encoder(obj):
     """JSON encoder that formats datetimes as ISO8601 format."""
     if isinstance(obj, datetime.datetime):
         return obj.isoformat()
@@ -86,14 +115,15 @@
             cache_key = (func_name, args, kwarg_items)
         result = self._instance_cache.get(cache_key)
         if result is not None:
             return result
         result = func(self, *args, **kwargs)
         self._instance_cache[cache_key] = result
         return result
+
     return _cache_guard
 
 
 def parse_timestamp(value):
     """Parse a timestamp into a datetime object.
 
     Supported formats:
@@ -187,15 +217,15 @@
     if dt.tzinfo is None:
         if default_timezone is None:
             default_timezone = tzutc()
         dt = dt.replace(tzinfo=default_timezone)
     d = dt.replace(tzinfo=None) - dt.utcoffset() - epoch
     if hasattr(d, "total_seconds"):
         return d.total_seconds()  # Works in Python 2.7+
-    return (d.microseconds + (d.seconds + d.days * 24 * 3600) * 10**6) / 10**6
+    return (d.microseconds + (d.seconds + d.days * 24 * 3600) * 10 ** 6) / 10 ** 6
 
 
 class ArgumentGenerator(object):
     """Generate sample input based on a shape model.
 
     This class contains a ``generate_skeleton`` method that will take
     an input shape (created from ``cdpcli.model``) and generate
@@ -217,14 +247,15 @@
         ddb = clidriver.get_service_model('dataeng')
         arg_gen = ArgumentGenerator()
         sample_input = arg_gen.generate_skeleton(
             ddb.operation_model('createAWSCluster').input_shape)
         print("Sample input for dataeng.createAWSCluster: %s" % sample_input)
 
     """
+
     def __init__(self):
         pass
 
     def generate_skeleton(self, shape):
         if shape.type_name == OBJECT_TYPE:
             return self._generate_type_object(shape)
         elif shape.type_name == LIST_TYPE:
@@ -237,14 +268,16 @@
             return 0
         elif shape.type_name in ['float', 'double']:
             return 0.0
         elif shape.type_name == 'boolean':
             return True
         elif shape.type_name == 'datetime':
             return '2002-10-02T13:00:00+00:00'
+        elif shape.type_name == 'blob':
+            return ''
         else:
             raise Exception("Unknown shape type: %s" % shape.type_name)
 
     def _generate_type_object(self, shape):
         skeleton = OrderedDict()
         for member_name, member_shape in shape.members.items():
             skeleton[member_name] = self.generate_skeleton(member_shape)
```

### Comparing `cdpcli-0.9.9/cdpcli/compat.py` & `cdpcli-0.9.90/cdpcli/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         # That way consumers can just call get_stdout_text_writer() and write
         # unicode to the returned stream.  Note that get_stdout_text_writer
         # just returns sys.stdout in the PY3 section above because python3
         # handles this.
         return codecs.getwriter(locale.getpreferredencoding())(sys.stdout)
 
     def ensure_unicode(s, encoding='utf-8', errors='strict'):
+        if s is None:
+            return None
         if isinstance(s, six.text_type):
             return s
         return unicode(s, encoding, errors)  # noqa
 
     def compat_open(filename, mode='r', encoding=None):
         # See docstring for compat_open in the PY3 section above.
         if 'b' not in mode:
```

### Comparing `cdpcli-0.9.9/cdpcli/data/iam/iam.yaml` & `cdpcli-0.9.90/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,2731 +1,2479 @@
+x-generated: Automatically generated by protocols script. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: iam
-x-products: ALTUS,CDP
-x-altus-releases: PUBLIC
+x-endpoint-name: dfworkload
+x-products: CDP
+x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.1-SNAPSHOT
-  title: Cloudera IAM Service
+  description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
+  version: 0.9.90
+  title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
-  description: Cloudera Altus IAM is a web service that you can use to manage users and user permissions under your Altus account.
+  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
+tags:
+  - name: CDFLocalRPCAPIVersion1
 paths:
-  /iam/getUser:
+  /dfx/api/rpc-v1/custom-nar-configurations/create-custom-nar-configuration:
     post:
-      summary: Gets information on a user.
-      description: Gets information on a user. If no user name is specified. The user name is determined from the access key used to make the request.
-      operationId: getUser
+      summary: Create the custom NAR configuration.
+      description: Create the custom NAR configuration.
+      operationId: createCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Create Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/GetUserRequest'
+            $ref: '#/definitions/CreateCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetUserResponse'
+            $ref: '#/definitions/CreateCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listUsers:
+  /dfx/api/rpc-v1/custom-nar-configurations/delete-custom-nar-configuration:
     post:
-      summary: Lists users.
-      description: Lists users.
-      operationId: listUsers
-      x-right: iam/listUsers
-      x-paginates: true
-      x-paging-default-max-items: 100
+      summary: Deletes an orphaned custom NAR configuration.
+      description: Deletes an orphaned custom NAR configuration.
+      operationId: deleteCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Delete Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/ListUsersRequest'
+            $ref: '#/definitions/DeleteCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListUsersResponse'
+            $ref: '#/definitions/DeleteCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/createUser:
+  /dfx/api/rpc-v1/custom-nar-configurations/get-custom-nar-configuration:
     post:
-      summary: Creates a user in Altus.
-      description: Creates a user in Altus.
-      operationId: createUser
-      x-right: iam/createUser
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
+      summary: Get a custom NAR configuration.
+      description: Get a custom NAR configuration.
+      operationId: getCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/CreateUserRequest'
+            $ref: '#/definitions/GetCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateUserResponse'
+            $ref: '#/definitions/GetCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/createUserAccessKey:
+  /dfx/api/rpc-v1/custom-nar-configurations/get-default-custom-nar-configuration:
     post:
-      summary: Creates a new access key for a user.
-      description: Creates a new access key for a user.
-      operationId: createUserAccessKey
+      summary: Get the default custom NAR configuration.
+      description: Get the default custom NAR configuration.
+      operationId: getDefaultCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Default Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/CreateUserAccessKeyRequest'
+            $ref: '#/definitions/GetDefaultCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateUserAccessKeyResponse'
+            $ref: '#/definitions/GetDefaultCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/createMachineUserAccessKey:
+  /dfx/api/rpc-v1/custom-nar-configurations/update-custom-nar-configuration:
     post:
-      summary: Creates a new access key for a machine user.
-      description: Creates a new access key for a machine user.
-      operationId: createMachineUserAccessKey
+      summary: Update the custom NAR configuration.
+      description: Update the custom NAR configuration.
+      operationId: updateCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Update Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/CreateMachineUserAccessKeyRequest'
+            $ref: '#/definitions/UpdateCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateMachineUserAccessKeyResponse'
+            $ref: '#/definitions/UpdateCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/deleteAccessKey:
+  /dfx/api/rpc-v1/custom-nar-configurations/validate-custom-nar-configuration:
     post:
-      summary: Deletes an access key.
-      description: Deletes an access key.
-      operationId: deleteAccessKey
+      summary: Validates the custom NAR configuration.
+      description: Validates the custom NAR configuration.
+      operationId: validateCustomNarConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Validate Custom NAR Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/DeleteAccessKeyRequest'
+            $ref: '#/definitions/ValidateCustomNarConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteAccessKeyResponse'
+            $ref: '#/definitions/ValidateCustomNarConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/updateAccessKey:
+  /dfx/api/rpc-v1/deployments/abort-asset-update-request:
     post:
-      summary: Updates an access key.
-      description: Updates an access key.
-      operationId: updateAccessKey
+      summary: Aborts asset update request.
+      description: Aborts an asset update request for a given deployment.
+      operationId: abortAssetUpdateRequest
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Abort Asset Update Request
           required: true
           schema:
-            $ref: '#/definitions/UpdateAccessKeyRequest'
+            $ref: '#/definitions/AbortAssetUpdateRequestRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpdateAccessKeyResponse'
+            $ref: '#/definitions/AbortAssetUpdateRequestResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/getAccessKey:
+  /dfx/api/rpc-v1/deployments/abort-deployment-request:
     post:
-      summary: Gets information on an access key.
-      description: Gets information on an access key. If no access key ID is specified. Information on the access key used to make the request is returned.
-      operationId: getAccessKey
-      x-right: iam/getAccessKey
+      summary: Aborts a deployment request.
+      description: Aborts a deployment request.
+      operationId: abortDeploymentRequest
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Abort Deployment Request
           required: true
           schema:
-            $ref: '#/definitions/GetAccessKeyRequest'
+            $ref: '#/definitions/AbortDeploymentRequestRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetAccessKeyResponse'
+            $ref: '#/definitions/AbortDeploymentRequestResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listAccessKeys:
+  /dfx/api/rpc-v1/deployments/cancel-nifi-version-update:
     post:
-      summary: Lists access keys.
-      description: Lists access keys.
-      operationId: listAccessKeys
-      x-right: iam/listAccessKeys
-      x-paginates: true
-      x-paging-default-max-items: 100
+      summary: Cancels a NiFi version update for a deployment.
+      description: Cancels a NiFi version update for a deployment.
+      operationId: cancelNifiVersionUpdate
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Cancel NiFi Version Update
           required: true
           schema:
-            $ref: '#/definitions/ListAccessKeysRequest'
+            $ref: '#/definitions/CancelNifiVersionUpdateRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListAccessKeysResponse'
+            $ref: '#/definitions/CancelNifiVersionUpdateResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listRoles:
+  /dfx/api/rpc-v1/deployments/create-asset-update-request:
     post:
-      summary: Lists all the available roles.
-      description: Lists all the available roles. Roles grant rights to users via policies that are attached to the roles.
-      operationId: listRoles
-      x-right: iam/listRoles
+      summary: Create asset update request.
+      description: Create an update request for modifying the assets of a given deployment.
+      operationId: createAssetUpdateRequest
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Create Asset Update Request
           required: true
           schema:
-            $ref: '#/definitions/ListRolesRequest'
+            $ref: '#/definitions/CreateAssetUpdateRequestRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListRolesResponse'
+            $ref: '#/definitions/CreateAssetUpdateRequestResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listResourceRoles:
+  /dfx/api/rpc-v1/deployments/create-deployment:
     post:
-      summary: Lists all the available resource roles.
-      description: Lists all the available reource roles. Resource roles grants rights over certain resources.
-      operationId: listResourceRoles
-      x-right: iam/listResourceRoles
+      summary: Creates a deployment.
+      description: Creates a deployment.
+      operationId: createDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Create Deployment Request
           required: true
           schema:
-            $ref: '#/definitions/ListResourceRolesRequest'
+            $ref: '#/definitions/CreateDeploymentRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListResourceRolesResponse'
+            $ref: '#/definitions/CreateDeploymentResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/assignUserRole:
+  /dfx/api/rpc-v1/deployments/get-deployment-configuration:
     post:
-      summary: Assign a role to a user.
-      description: Assign a role to a user. If the role is already assigned to the user the request will fail.
-      operationId: assignUserRole
-      x-right: iam/assignRole
+      summary: Retrieves the deployment configuration.
+      description: Retrieves the deployment configuration.
+      operationId: getDeploymentConfiguration
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Deployment Configuration Request
           required: true
           schema:
-            $ref: '#/definitions/AssignUserRoleRequest'
+            $ref: '#/definitions/GetDeploymentConfigurationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/AssignUserRoleResponse'
+            $ref: '#/definitions/GetDeploymentConfigurationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/unassignUserRole:
+  /dfx/api/rpc-v1/deployments/get-deployment-configuration-metadata:
     post:
-      summary: Unassign a role from a user.
-      description: Unassign a role from a user. If the role is not currently assigned to the user the request will fail.
-      operationId: unassignUserRole
-      x-right: iam/unassignRole
+      summary: Retrieves the deployment configuration metadata.
+      description: Retrieves the deployment configuration metadata.
+      operationId: getDeploymentConfigurationMetadata
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Deployment Configuration Metadata Request
           required: true
           schema:
-            $ref: '#/definitions/UnassignUserRoleRequest'
+            $ref: '#/definitions/GetDeploymentConfigurationMetadataRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UnassignUserRoleResponse'
+            $ref: '#/definitions/GetDeploymentConfigurationMetadataResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/assignUserResourceRole:
+  /dfx/api/rpc-v1/deployments/get-deployment-request-details:
     post:
-      summary: Assign a resource role to a user.
-      description: Assign a resource role to a user. If the resource role is already assigned to the user the request will fail.
-      operationId: assignUserResourceRole
-      x-right: iam/assignResourceRole
+      summary: Retrieves deployment request details.
+      description: Retrieves deployment request details.
+      operationId: getDeploymentRequestDetails
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Deployment Request details
           required: true
           schema:
-            $ref: '#/definitions/AssignUserResourceRoleRequest'
+            $ref: '#/definitions/GetDeploymentRequestDetailsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/AssignUserResourceRoleResponse'
+            $ref: '#/definitions/GetDeploymentRequestDetailsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/unassignUserResourceRole:
+  /dfx/api/rpc-v1/deployments/terminate-deployment:
     post:
-      summary: Unassign a resource role from a user.
-      description: Unassign a resource role from a user. If the resource role is not currently assigned to the user the request will fail.
-      operationId: unassignUserResourceRole
-      x-right: iam/unassignResourceRole
+      summary: Terminates a deployment.
+      description: Initiates the termination of a deployment.
+      operationId: terminateDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Terminate Deployment Request
           required: true
           schema:
-            $ref: '#/definitions/UnassignUserResourceRoleRequest'
+            $ref: '#/definitions/TerminateDeploymentRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UnassignUserResourceRoleResponse'
+            $ref: '#/definitions/TerminateDeploymentResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listUserAssignedRoles:
+  /dfx/api/rpc-v1/deployments/transition-flow:
     post:
-      summary: Lists the user's assigned roles.
-      description: Lists the user's assigned roles.
-      operationId: listUserAssignedRoles
-      x-right: iam/listAssignedRoles
+      summary: Transitions a flow.
+      description: Transitions the NiFi flow of a deployment to the specified state.
+      operationId: transitionFlow
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Transition Flow
           required: true
           schema:
-            $ref: '#/definitions/ListUserAssignedRolesRequest'
+            $ref: '#/definitions/TransitionFlowRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListUserAssignedRolesResponse'
+            $ref: '#/definitions/TransitionFlowResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/listUserAssignedResourceRoles:
+  /dfx/api/rpc-v1/deployments/update-deployment:
     post:
-      summary: Lists a user's assigned resource roles.
-      description: Lists a user's assigned resource roles.
-      operationId: listUserAssignedResourceRoles
-      x-right: iam/listAssignedResourceRoles
+      summary: Updates a deployment.
+      description: Updates a deployment.
+      operationId: updateDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload,df
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Update Deployment Request
           required: true
           schema:
-            $ref: '#/definitions/ListUserAssignedResourceRolesRequest'
+            $ref: '#/definitions/UpdateDeploymentRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListUserAssignedResourceRolesResponse'
+            $ref: '#/definitions/UpdateDeploymentResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/assignMachineUserRole:
+  /dfx/api/rpc-v1/deployments/update-nifi-version:
     post:
-      summary: Assign a role to a machine user.
-      description: Assign a role to a machine user. If the role is already assigned to the machine user the request will fail.
-      operationId: assignMachineUserRole
-      x-right: iam/assignRole
+      summary: Updates the NiFi version of a deployment.
+      description: Initiates the process of updating the NiFi version of a deployment.
+      operationId: updateNifiVersion
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Update NiFi Version
           required: true
           schema:
-            $ref: '#/definitions/AssignMachineUserRoleRequest'
+            $ref: '#/definitions/UpdateNifiVersionRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/AssignMachineUserRoleResponse'
+            $ref: '#/definitions/UpdateNifiVersionResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/unassignMachineUserRole:
+  /dfx/api/rpc-v1/deployments/upload-asset:
     post:
-      summary: Unassign a role from a machine user.
-      description: Unassign a role from a machine user. If the role is not currently assigned to the machine user the request will fail.
-      operationId: unassignMachineUserRole
-      x-right: iam/unassignRole
+      summary: Upload an asset.
+      description: Uploads an asset for a deployment request or asset update request.
+      operationId: uploadAsset
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload,df
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Upload Asset
           required: true
           schema:
-            $ref: '#/definitions/UnassignMachineUserRoleRequest'
+            $ref: '#/definitions/UploadAssetRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UnassignMachineUserRoleResponse'
+            $ref: '#/definitions/UploadAssetResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/assignMachineUserResourceRole:
+  /dfx/api/rpc-v1/environments/list-nifi-versions:
     post:
-      summary: Assign a resource role to a machine user.
-      description: Assign a resource role to a machine user. If the resource role is already assigned to the machine user the request will fail.
-      operationId: assignMachineUserResourceRole
-      x-right: iam/assignResourceRole
+      summary: Lists all supported NiFi versions.
+      description: Lists all supported NiFi versions.
+      operationId: listNifiVersions
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: List NiFi Versions Request
           required: true
           schema:
-            $ref: '#/definitions/AssignMachineUserResourceRoleRequest'
+            $ref: '#/definitions/ListNifiVersionsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/AssignMachineUserResourceRoleResponse'
+            $ref: '#/definitions/ListNifiVersionsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /iam/unassignMachineUserResourceRole:
+  /dfx/api/rpc-v1/inbound-connection-endpoint-certificates/download-client-certificate-encoded:
     post:
-      summary: Unassign a resource role from a machine user.
-      description: Unassign a resource role from a machine user. If the resource role is not currently assigned to the machine user the request will fail.
-      operationId: unassignMachineUserResourceRole
-      x-right: iam/unassignResourceRole
+      summary: Get Inbound Connection Endpoint Client Certificate (in PEM encoding)
+      description: Get Inbound Connection Endpoint Client Certificate (in PEM encoding)
+      operationId: getClientCertificateEncoded
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Inbound Connection Endpoint client's certificate request
           required: true
           schema:
-            $ref: '#/definitions/UnassignMachineUserResourceRoleRequest'
+            $ref: '#/definitions/InboundConnectionEndpointClientCertificateRequest'
       responses:
         200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/UnassignMachineUserResourceRoleResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listMachineUserAssignedRoles:
-    post:
-      summary: Lists the machine user's assigned roles.
-      description: Lists the machine user's assigned roles.
-      operationId: listMachineUserAssignedRoles
-      x-right: iam/listAssignedRoles
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListMachineUserAssignedRolesRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListMachineUserAssignedRolesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listMachineUserAssignedResourceRoles:
-    post:
-      summary: Lists a machine user's assigned resource roles.
-      description: Lists a machine user's assigned resource roles.
-      operationId: listMachineUserAssignedResourceRoles
-      x-right: iam/listAssignedResourceRoles
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListMachineUserAssignedResourceRolesRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListMachineUserAssignedResourceRolesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listResourceAssignees:
-    post:
-      summary: List the resource assignees and their respective resource roles for the resource.
-      description: List the resource assignees and their respective resource roles for the resource.
-      operationId: listResourceAssignees
-      x-right: iam/listResourceAssignees
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListResourceAssigneesRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListResourceAssigneesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/createMachineUser:
-    post:
-      summary: Create a machine user.
-      description: Creates a machine user in the account. A machine user can be used to access Altus API. A machine user can have access keys associated with it and can be assigned roles and resource roles. A machine user cannot login to the Altus console.
-      operationId: createMachineUser
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/CreateMachineUserRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/CreateMachineUserResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listMachineUsers:
-    post:
-      summary: Lists machine users.
-      description: Lists machine users in the account.
-      operationId: listMachineUsers
-      x-right: iam/listMachineUsers
-      x-paginates: true
-      x-paging-default-max-items: 100
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListMachineUsersRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListMachineUsersResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/deleteMachineUser:
-    post:
-      summary: Delete a machine user.
-      description: Deletes a machine user previously created in the account.
-      operationId: deleteMachineUser
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/DeleteMachineUserRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/DeleteMachineUserResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/createSamlProvider:
-    post:
-      summary: Creates a SAML provider in Altus.
-      description: Creates a SAML provider in Altus.
-      operationId: createSamlProvider
-      x-right: iam/createSamlProvider
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/CreateSamlProviderRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/CreateSamlProviderResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/deleteSamlProvider:
-    post:
-      summary: Deletes a SAML provider in Altus account.
-      description: Deletes a SAML provider in Altus account.
-      operationId: deleteSamlProvider
-      x-right: iam/deleteSamlProvider
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/DeleteSamlProviderRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/DeleteSamlProviderResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listSamlProviders:
-    post:
-      summary: Lists SAML providers in Altus account.
-      description: Lists SAML providers in Altus account.
-      operationId: listSamlProviders
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
-      x-right: iam/listSamlProviders
-      parameters:
-        - name: input
-          in: body
-          required: true
+          description: Expected response to a valid inboundConnectionEndpointClientCertificateRequest.
           schema:
-            $ref: '#/definitions/ListSamlProvidersRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListSamlProvidersResponse'
+            $ref: '#/definitions/InboundConnectionEndpointClientCertificateResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/updateSamlProvider:
+  /dfx/api/rpc-v1/inbound-connection-endpoint-certificates/download-client-private-key-encoded:
     post:
-      summary: Updates a SAML provider in Altus.
-      description: Updates a SAML provider in Altus.
-      operationId: updateSamlProvider
-      x-right: iam/updateSamlProvider
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
+      summary: Get Inbound Connection Endpoint Client's Private Key (in PEM encoding)
+      description: Get Inbound Connection Endpoint Client's Private Key (in PEM encoding)
+      operationId: getClientPrivateKeyEncoded
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Get Inbound Connection Endpoint client's private key request
           required: true
           schema:
-            $ref: '#/definitions/UpdateSamlProviderRequest'
+            $ref: '#/definitions/InboundConnectionEndpointClientPrivateKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpdateSamlProviderResponse'
+            $ref: '#/definitions/InboundConnectionEndpointClientPrivateKeyResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/enableClouderaSSOLogin:
+  /dfx/api/rpc-v1/inbound-connection-endpoints/create-inbound-connection-endpoint:
     post:
-      summary: Enables interactive login using Cloudera SSO for this account.
-      description: Enables interactive login using Cloudera SSO for this account. This is a no-op if login using Cloudera SSO are already enabled.
-      operationId: enableClouderaSSOLogin
-      x-right: iam/manageClouderaSSOLogin
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
+      summary: Create Inbound Connection Endpoint
+      description: Create Inbound Connection Endpoint
+      operationId: createInboundConnectionEndpoint
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Create Inbound Connection Endpoint request
           required: true
           schema:
-            $ref: '#/definitions/EnableClouderaSSOLoginRequest'
+            $ref: '#/definitions/CreateInboundConnectionEndpointRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/EnableClouderaSSOLoginResponse'
+            $ref: '#/definitions/CreateInboundConnectionEndpointResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/disableClouderaSSOLogin:
+  /dfx/api/rpc-v1/inbound-connection-endpoints/delete-inbound-connection-endpoint:
     post:
-      summary: Disables interactive login using Cloudera SSO for this account.
-      description: Disables interactive login using Cloudera SSO for this account. When disabled, only users who are designated account administrators will be able to use Cloudera SSO to interactively login to the Altus account. All other users will only be able to interactively login using SAML providers defined for the account. This is a no-op if login using Cloudera SSO are already disabled.
-      operationId: disableClouderaSSOLogin
-      x-right: iam/manageClouderaSSOLogin
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
+      summary: Delete Inbound Connection Endpoint
+      description: Delete Inbound Connection Endpoint
+      operationId: deleteInboundConnectionEndpoint
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Delete Inbound Connection Endpoint request
           required: true
           schema:
-            $ref: '#/definitions/DisableClouderaSSOLoginRequest'
+            $ref: '#/definitions/DeleteInboundConnectionEndpointRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DisableClouderaSSOLoginResponse'
+            $ref: '#/definitions/DeleteInboundConnectionEndpointResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/getAccount:
+  /dfx/api/rpc-v1/inbound-connection-endpoints/describe-inbound-connection-endpoint:
     post:
-      summary: Retrieves information about the Altus account.
-      description: Retrieves information about the Altus account.
-      operationId: getAccount
-      x-entitlement: IDENTITY_FEDERATION
-      x-right: iam/getAccount
-      x-no-compatibility-guarantee: true
+      summary: Describe Inbound Connection Endpoint
+      description: Describe Inbound Connection Endpoint
+      operationId: describeInboundConnectionEndpoint
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: Describe Inbound Connection Endpoint request
           required: true
           schema:
-            $ref: '#/definitions/GetAccountRequest'
+            $ref: '#/definitions/DescribeInboundConnectionEndpointRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetAccountResponse'
+            $ref: '#/definitions/DescribeInboundConnectionEndpointResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/createGroup:
+  /dfx/api/rpc-v1/inbound-connection-endpoints/list-inbound-connection-endpoints:
     post:
-      summary: Create a group.
-      description: Create a group. A group is a named collection of users and machine users. Roles and resource roles can be assigned to a group impacting all members of the group.
-      operationId: createGroup
-      x-right: iam/createGroup
+      summary: List Inbound Connection Endpoints
+      description: List Inbound Connection Endpoints
+      operationId: listInboundConnectionEndpoints
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: input
+          description: List Inbound Connection Endpoints request
           required: true
           schema:
-            $ref: '#/definitions/CreateGroupRequest'
+            $ref: '#/definitions/ListInboundConnectionEndpointsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateGroupResponse'
+            $ref: '#/definitions/ListInboundConnectionEndpointsResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/deleteGroup:
+  /dfx/api/rpc-v1/inbound-connection-endpoints/renew-certificates:
     post:
-      summary: Delete a group.
-      description: Delete a group.
-      operationId: deleteGroup
-      x-right: iam/deleteGroup
+      summary: Renew Inbound Connection Endpoint certificates
+      description: Submits a request for renewal of Inbound Connection Endpoint certificates
+      operationId: renewInboundConnectionEndpointCertificates
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
       parameters:
-        - name: input
-          in: body
+        - in: body
+          name: body
+          description: Inbound connection endpoint certificates renewal request
           required: true
           schema:
-            $ref: '#/definitions/DeleteGroupRequest'
+            $ref: '#/definitions/RenewInboundConnectionEndpointCertificateRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteGroupResponse'
+            $ref: '#/definitions/RenewInboundConnectionEndpointCertificateResponse'
         default:
           description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroups:
-    post:
-      summary: Lists groups.
-      description: Lists groups. If no group names are specified, the call lists all groups.
-      operationId: listGroups
-      x-right: iam/listGroups
-      x-paginates: true
-      x-paging-default-max-items: 100
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupsRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupsResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/updateGroup:
-    post:
-      summary: Update a group.
-      description: Update a group.
-      operationId: updateGroup
-      x-right: iam/updateGroup
-      x-no-compatibility-guarantee: true
-      x-entitlement: IDENTITY_FEDERATION
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/UpdateGroupRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/UpdateGroupResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/addUserToGroup:
-    post:
-      summary: Add a user to a group.
-      description: Add a user to group.
-      operationId: addUserToGroup
-      x-right: iam/addMemberToGroup
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/AddUserToGroupRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/AddUserToGroupResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/addMachineUserToGroup:
-    post:
-      summary: Add a machine user to group.
-      description: Add a machine user to a group.
-      operationId: addMachineUserToGroup
-      x-right: iam/addMemberToGroup
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/AddMachineUserToGroupRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/AddMachineUserToGroupResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/removeUserFromGroup:
-    post:
-      summary: Remove a user from a group.
-      description: Remove a user from a group.
-      operationId: removeUserFromGroup
-      x-right: iam/removeMemberFromGroup
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/RemoveUserFromGroupRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/RemoveUserFromGroupResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/removeMachineUserFromGroup:
-    post:
-      summary: Remove a machine user from a group.
-      description: Remove a machine user from a group.
-      operationId: removeMachineUserFromGroup
-      x-right: iam/removeMemberFromGroup
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/RemoveMachineUserFromGroupRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/RemoveMachineUserFromGroupResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroupMembers:
-    post:
-      summary: List the members of a group.
-      description: List the members of a group.
-      operationId: listGroupMembers
-      x-right: iam/listGroupMembers
-      x-paginates: true
-      x-paging-default-max-items: 100
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupMembersRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupMembersResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroupsForUser:
-    post:
-      summary: List the groups that the user belongs to.
-      description: List the groups that the user belongs to.
-      operationId: listGroupsForUser
-      x-right: iam/listGroupsForActor
-      x-paginates: true
-      x-paging-default-max-items: 100
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupsForUserRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupsForUserResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroupsForMachineUser:
-    post:
-      summary: List the groups that the machine user belongs to.
-      description: List the groups that the machine user belongs to.
-      operationId: listGroupsForMachineUser
-      x-right: iam/listGroupsForActor
-      x-paginates: true
-      x-paging-default-max-items: 100
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupsForMachineUserRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupsForMachineUserResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/assignGroupRole:
-    post:
-      summary: Assign a role to a group.
-      description: Assign a role to a group. If the role is already assigned to the group the request will fail.
-      operationId: assignGroupRole
-      x-right: iam/assignRole
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/AssignGroupRoleRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/AssignGroupRoleResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/unassignGroupRole:
-    post:
-      summary: Unassign a role from a group.
-      description: Unassign a role from a group. If the role is not currently assigned to the group the request will fail.
-      operationId: unassignGroupRole
-      x-right: iam/unassignRole
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/UnassignGroupRoleRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/UnassignGroupRoleResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/assignGroupResourceRole:
-    post:
-      summary: Assign a resource role to a group.
-      description: Assign a resource role to a group. If the resource role is already assigned to the group the request will fail.
-      operationId: assignGroupResourceRole
-      x-right: iam/assignResourceRole
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/AssignGroupResourceRoleRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/AssignGroupResourceRoleResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/unassignGroupResourceRole:
-    post:
-      summary: Unassign a resource role from a group.
-      description: Unassign a resource role from a group. If the resource role is not currently assigned to the group the request will fail.
-      operationId: unassignGroupResourceRole
-      x-right: iam/unassignResourceRole
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/UnassignGroupResourceRoleRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/UnassignGroupResourceRoleResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroupAssignedRoles:
-    post:
-      summary: Lists the group's assigned roles.
-      description: Lists the group's assigned roles.
-      operationId: listGroupAssignedRoles
-      x-right: iam/listAssignedRoles
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupAssignedRolesRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupAssignedRolesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/listGroupAssignedResourceRoles:
-    post:
-      summary: Lists a group's assigned resource roles.
-      description: Lists a group's assigned resource roles.
-      operationId: listGroupAssignedResourceRoles
-      x-right: iam/listAssignedResourceRoles
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListGroupAssignedResourceRolesRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListGroupAssignedResourceRolesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/setWorkloadPassword:
-    post:
-      summary: Set the workload password for an actor.
-      description: Set the workload password for an actor. This will be the actor's password in all Environments they have access to, including Environments they are given access to after setting the password. The password plaintext is not kept.
-      operationId: setWorkloadPassword
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/SetWorkloadPasswordRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/SetWorkloadPasswordResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /iam/setWorkloadPasswordPolicy:
-    post:
-      summary: Set the workload password policy for the account.
-      description: Set the workload password for the account. Changes to the workload password policy only affect passwords that are set after the policy has been updated. By default, passwords never expire.
-      operationId: setWorkloadPasswordPolicy
-      x-no-compatibility-guarantee: true
-      x-right: iam/setWorkloadPasswordPolicy
-      x-entitlement: WORKLOAD_PASSWORD_POLICY
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/SetWorkloadPasswordPolicyRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/SetWorkloadPasswordPolicyResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
 definitions:
-  Error:
+  AbortAssetUpdateRequestRequest:
     type: object
-    description: An object returned on an error.
+    description: Request object for aborting an asset update request
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - assetUpdateRequestCrn
+      - deploymentCrn
     properties:
-      code:
+      environmentCrn:
         type: string
-        description: The error code.
-      message:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        description: The error message.
-  WorkloadPasswordPolicy:
+        description: The deployment crn.
+      assetUpdateRequestCrn:
+        type: string
+        description: The CRN of the asset update request
+  AbortAssetUpdateRequestResponse:
     type: object
-    description: Information about the workload password policy for an account.
-    x-no-compatibility-guarantee: true
+    description: Response object for aborting an asset update request
+    x-workload: true
+    x-client-only: true
+  AbortDeploymentRequestRequest:
+    type: object
+    description: Request object for abort deployment request.
+    x-workload: true
+    x-client-only: true
     required:
-      - maxPasswordLifetimeDays
+      - environmentCrn
+      - deploymentRequestCrn
     properties:
-      maxPasswordLifetimeDays:
-        type: integer
-        format: int32
-        description: The max lifetime, in days, of the password. If '0' passwords never expire.
-  Account:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentRequestCrn:
+        type: string
+        description: The deployment request crn.
+  AbortDeploymentRequestResponse:
+    type: object
+    description: Response object for aborting a deployment request.
+    x-workload: true
+    x-client-only: true
+  AlertFrequencyTolerance:
     type: object
-    description: Information about a Cloudera Altus account.
-    x-no-compatibility-guarantee: true
+    description: The alert frequency tolerance unit choices, including a default
+    x-workload: true
+    x-client-only: true
     required:
-      - clouderaSSOLoginEnabled
-      - workloadPasswordPolicy
+      - units
     properties:
-      clouderaSSOLoginEnabled:
-        type: boolean
-        description: Whether interactive login using Cloudera SSO is enabled.
-      workloadPasswordPolicy:
-        x-no-compatibility-guarantee: true
-        $ref: '#/definitions/WorkloadPasswordPolicy'
-        description: The workload password policy object.
-  User:
+      units:
+        type: array
+        description: The legal alert frequency values
+        items:
+          $ref: '#/definitions/AlertFrequencyUnit'
+      defaultUnitId:
+        type: string
+        description: The default alert frequency ID to use as the default chooser value
+  AlertFrequencyUnit:
     type: object
-    description: Information about a Cloudera Altus user.
+    description: The alert frequency unit to use in KPI tolerances and metrics
+    x-workload: true
+    x-client-only: true
     required:
-      - userId
-      - crn
-      - email
-      - firstName
-      - lastName
-      - creationDate
-      - accountAdmin
-      - identityProviderCrn
-    x-limits:
-      - scope: account
-        value: 100
-        doc: The maximum number of users that can be created in an account.
+      - id
+      - label
     properties:
-      userId:
+      id:
         type: string
-        description: The stable, unique identifier of the user.
-      crn:
+        description: The id of the frequency unit
+        enum:
+          - SECONDS
+          - MINUTES
+          - HOURS
+          - DAYS
+      label:
         type: string
-        description: The CRN of the user.
-      email:
+        description: The user-friendly label of the frequency unit
+      abbreviation:
         type: string
-        description: The user's email address.
-      firstName:
+        description: The abbreviation for frequency unit
+  AssetReference:
+    type: object
+    description: A reference to an asset used in a flow parameter
+    x-workload: true
+    x-client-only: true
+    properties:
+      name:
         type: string
-        description: The user's first name.
-      lastName:
+        description: The name of the asset
+      path:
         type: string
-        description: The user's last name.
-      creationDate:
+        description: The path of the asset
+      version:
         type: string
-        format: date-time
-        description: The date when this user record was created.
-      accountAdmin:
+        description: The version of the asset
+      environmentProvided:
         type: boolean
-        description: Whether the user is an administrator of their Altus account.
-      identityProviderCrn:
-        type: string
-        x-no-compatibility-guarantee: true
-        description: The identity provider that the user belongs to. It can be "Cloudera-Default", "Cloudera-Administration", or a customer defined IdP.
-      lastInteractiveLogin:
-        type: string
-        format: date-time
-        description: The date of the user's last interactive login.
-      workloadUsername:
-        type: string
-        description: The username used in all the workload clusters of the user.
-        x-no-compatibility-guarantee: true
-  MachineUser:
+        description: Whether or not the asset is provided automatically by the environment. If true, the asset cannot removed or replaced.
+  CancelNifiVersionUpdateRequest:
     type: object
-    description: Information about a Cloudera Altus machine user.
+    description: Request object for cancelling a NiFi version update for a deployment.
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
-      - crn
-      - creationDate
-    x-limits:
-      - scope: account
-        value: 100
-        doc: The maximum number of machine users that can be created in an account.
+      - environmentCrn
+      - deploymentCrn
     properties:
-      machineUserName:
-        type: string
-        description: The machine user name.
-      crn:
-        type: string
-        description: The CRN of the user.
-      creationDate:
+      environmentCrn:
         type: string
-        format: date-time
-        description: The date when this machine user record was created.
-      workloadUsername:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        description: The username used in all the workload clusters of the machine user.
-        x-no-compatibility-guarantee: true
-  AccessKey:
+        description: The deployment crn.
+  CancelNifiVersionUpdateResponse:
     type: object
-    description: Information about a Cloudera Altus access key.
-    required:
-      - accessKeyId
-      - crn
-      - actorCrn
-      - creationDate
-    x-limits:
-      - scope: account
-        value: 200
-        doc: The maximum number of access keys that can be created in an account.
+    description: Response object for cancelling a NiFi version update for a deployment.
+    x-workload: true
+    x-client-only: true
     properties:
-      accessKeyId:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  ClusterSize:
+    type: object
+    description: Cluster scaling parameters
+    x-workload: true
+    x-client-only: true
+    properties:
+      name:
         type: string
-        description: The ID of the access key.
-      crn:
+        description: The name of this Cluster Size
+      text:
         type: string
-        description: The CRN of the access key.
-      actorCrn:
+        description: The text (i.e., the human readable name) for this Cluster Size
+      coresPerNode:
+        type: integer
+        format: int32
+        description: The number of CPU Cores per node
+      heapSize:
+        type: number
+        format: double
+        description: The heap size
+      enabled:
+        type: boolean
+        description: Flag to signal whether this ClusterSize is enabled
+      memoryLimit:
+        type: number
+        format: double
+        description: The memory limit
+  ConfiguredAlert:
+    type: object
+    description: An alert configuration that specifies a configured frequency with lower and/or upper thresholds
+    x-workload: true
+    x-client-only: true
+    properties:
+      thresholdMoreThan:
+        description: The optional moreThan threshold that should trigger an alert; at least one of thresholdMoreThan and thresholdLessThan is required
+        $ref: '#/definitions/ConfiguredAlertThreshold'
+      thresholdLessThan:
+        description: The optional lessThan threshold that should trigger an alert
+        $ref: '#/definitions/ConfiguredAlertThreshold'
+      frequencyTolerance:
+        description: The configured alert frequency tolerance for the KPI
+        $ref: '#/definitions/ConfiguredAlertFrequencyTolerance'
+  ConfiguredAlertFrequencyTolerance:
+    type: object
+    description: An alert configuration frequency tolerance for measuring an amount of time and unit for alert triggering
+    x-workload: true
+    x-client-only: true
+    required:
+      - unit
+      - value
+    properties:
+      unit:
+        description: The unit of time controlling how long a metric value can persist outside its boundaries before an alert is generated
+        $ref: '#/definitions/AlertFrequencyUnit'
+      value:
+        type: number
+        format: double
+        description: The amount of time, associated with the given unit, a metric value can persist outside its boundaries before an alert is generated
+  ConfiguredAlertThreshold:
+    type: object
+    description: A configured alert threshold to pair together a statistical unit and value
+    x-workload: true
+    x-client-only: true
+    required:
+      - unitId
+      - value
+    properties:
+      unitId:
+        type: string
+        description: The identifier of the alert threshold unit to associate with the given threshold value
+      value:
+        type: number
+        format: double
+        description: The threshold value whose triggering causes an alert
+  ConfiguredKpi:
+    type: object
+    description: An instantiated KPI specifying a metric on which to alert
+    x-workload: true
+    x-client-only: true
+    required:
+      - metricId
+    properties:
+      metricId:
         type: string
-        description: The CRN of the actor with which this access key is associated.
-      creationDate:
+        description: The id of the associated metric
+      id:
         type: string
-        format: date-time
-        description: The date when the access key was created.
-      status:
+        description: The id of the KPI; used only when viewing and editing existing KPIs
+      metricComponentType:
         type: string
-        description: The status of an access key.
+        description: The component type of the associated metric
         enum:
-          - ACTIVE
-          - INACTIVE
-      type:
+          - SYSTEM
+          - NIFI_FLOW
+          - NIFI_PROCESSOR
+          - NIFI_PROCESS_GROUP
+          - NIFI_CONNECTION
+      alert:
+        description: The alert specification for the associated metric
+        $ref: '#/definitions/ConfiguredAlert'
+      componentId:
         type: string
-        description: The type of an access key.
-        enum:
-          - V1
-          - V2
-      lastUsage:
-        $ref: '#/definitions/AccessKeyLastUsage'
-        description: Information on the last time this access key was used.
-  AccessKeyLastUsage:
+        description: The optional process group ID, processor ID, or connection ID. This is a composite ID containing a chain of process group IDs representing the component's full ancestry
+  CreateAssetUpdateRequestRequest:
     type: object
-    description: Information on the last time an access key was used.
+    description: Request object for creating an asset update request
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
     properties:
-      lastUsageDate:
+      environmentCrn:
         type: string
-        format: date-time
-        description: The date when the access key was last used.
-      serviceName:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        description: The name of the service with which this access key was most recently used.
-  PolicyStatement:
-    type: object
-    description: A policy statement is a list of rights and zero or more resources on which the rights are granted.
-    required:
-      - rights
-      - resources
-    properties:
-      rights:
-        type: array
-        items:
-          type: string
-        description: The list of rights in the policy statement.
-      resources:
-        type: array
-        items:
-          type: string
-        description: The resources on which the rights are granted.
-  Policy:
+        description: The deployment crn.
+  CreateAssetUpdateRequestResponse:
     type: object
-    description: A policy contains a list of one or more policy statements.
-    required:
-      - crn
-      - policyStatements
+    description: Response object for creating an asset update request
+    x-workload: true
+    x-client-only: true
     properties:
-      crn:
+      assetUpdateRequestCrn:
         type: string
-        description: The policy crn.
-      policyStatements:
-        type: array
-        items:
-          $ref: '#/definitions/PolicyStatement'
-        description: The policy statements.
-  ResourceRole:
+        description: The CRN of the created asset update request
+  CreateCustomNarConfigurationRequest:
     type: object
-    description: Information about a resource role. A resource role is a role that grants a collection of rights to a user on resources.
+    description: Request object for creating a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - crn
-      - rights
+      - environmentCrn
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      crn:
+      environmentCrn:
         type: string
-        description: The CRN of the resource role.
-      rights:
-        type: array
-        items:
-          type: string
-        description: The rights granted by this role.
-  Role:
-    type: object
-    description: Information about a role.
-    required:
-      - crn
-      - policies
-    properties:
-      crn:
+        description: The CRN of an environment to execute the command.
+      username:
         type: string
-        description: The role's CRN.
-      policies:
-        type: array
-        items:
-          $ref: '#/definitions/Policy'
-        description: The list of policies that belong to the role. Cannot be empty.
-  ResourceAssignment:
-    type: object
-    description: Information about a resource assignment.
-    required:
-      - resourceCrn
-      - resourceRoleCrn
-    properties:
-      resourceCrn:
+        description: The username used to access the storage location
+      password:
         type: string
-        description: The assigned resource's CRN.
-      resourceRoleCrn:
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The assigned resource role CRN.
-  ResourceAssignee:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of the configuration
+  CreateCustomNarConfigurationResponse:
     type: object
-    description: Information about the resource role assignee for the resource.
+    description: Response for creating a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - assigneeCrn
-      - resourceRoleCrn
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      assigneeCrn:
+      username:
         type: string
-        description: The CRN of the assignee.
-      resourceRoleCrn:
+        description: The username used to access the storage location
+      password:
         type: string
-        description: The assigned resource role CRN.
-  Group:
-    type: object
-    description: Information about a group.
-    required:
-      - groupName
-      - crn
-      - creationDate
-    properties:
-      groupName:
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The group name.
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of the configuration
       crn:
         type: string
-        description: The CRN of the group.
-      creationDate:
-        type: string
-        format: date-time
-        description: The date when this group record was created.
-      syncMembershipOnUserLogin:
-        x-no-compatibility-guarantee: true
-        type: boolean
-        description: Whether group membership is synced when a user logs in. The default is to sync group membership.
-  SamlProvider:
+        description: The CRN of the custom NAR configuration to update.
+  CreateDeploymentRequest:
     type: object
-    description: Information used to connect an Altus account to an external identity provider.
-    x-no-compatibility-guarantee: true
-    required:
-      - crn
-      - creationDate
-      - samlProviderName
-      - samlProviderId
-      - syncGroupsOnLogin
+    description: Request object to create a deployment.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - clusterSizeName
+      - configurationVersion
+      - deploymentRequestCrn
+      - name
     properties:
-      crn:
-        type: string
-        description: CRN of the SAML provider in Altus.
-        x-no-compatibility-guarantee: true
-      creationDate:
-        type: string
-        format: date-time
-        description: The date when this SAML provider record was created.
-        x-no-compatibility-guarantee: true
-      samlProviderName:
+      environmentCrn:
         type: string
-        description: Name of the SAML provider.
-      samlProviderId:
+        description: The CRN of an environment to execute the command.
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of this configuration
+      name:
         type: string
-        description: The unique ID of the saml provider.
-      syncGroupsOnLogin:
-        type: boolean
-        description: Whether users federated with this SAML provider will have their group membership synchronized. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion.
-      samlMetadataDocument:
+        description: The name of the deployment
+      clusterSizeName:
         type: string
-        description: The original metadata that was passed while creating the SAML provider connector. This field will not be set for listSamlProviders API response.
-  GetUserRequest:
-    type: object
-    description: Request object for a get user request.
-    properties:
-      userId:
+        description: The size of the cluster to deploy
+        enum:
+          - EXTRA_SMALL
+          - SMALL
+          - MEDIUM
+          - LARGE
+      deploymentRequestCrn:
         type: string
-        description: The ID of the user to get information about. If it is not included, it defaults to the user making the request.
-  GetUserResponse:
-    type: object
-    description: Response object for a get user request.
-    required:
-      - user
-    properties:
-      user:
-        $ref: '#/definitions/User'
-        description: Information about the user.
-  ListUsersRequest:
-    type: object
-    description: Request object for a list users request.
-    properties:
-      userIds:
+        description: The CRN of the deployment request.
+      parameterGroups:
         type: array
+        description: The list of flow parameter groups
         items:
-          type: string
-        description: The user IDs or CRNs of the users.
-      pageSize:
+          $ref: '#/definitions/FlowParameterGroup'
+      autoScalingEnabled:
+        type: boolean
+        description: Specifies that auto-scaling should be enabled.
+      autoScaleMinNodes:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The minimum number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is true.
+      autoScaleMaxNodes:
+        type: integer
+        format: int32
+        description: The maximum number of nodes that the cluster should scale to. May only be specified when autoScalingEnabled is true.
+      staticNodeCount:
+        type: integer
+        format: int32
+        description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
+      kpis:
+        type: array
+        description: The list of configured KPIs
+        items:
+          $ref: '#/definitions/ConfiguredKpi'
+      cfmNifiVersion:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListUsersResponse:
-    type: object
-    description: Response object for a list users request.
-    required:
-      - users
-    properties:
-      users:
+        description: The CFM NiFi version associated with the deployment
+      autoStartFlow:
+        type: boolean
+        description: Indicates whether or not the flow should be started during deployment creation
+      inboundHostname:
+        type: string
+        description: The FQDN of inbound hostname or just the prefix part
+      listenComponents:
         type: array
+        description: Listen components port and protocol data
         items:
-          $ref: '#/definitions/User'
-        x-paging-result: true
-        description: The users.
-      nextToken:
+          $ref: '#/definitions/ListenComponent'
+      customNarConfigurationCrn:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  CreateUserAccessKeyRequest:
+        description: The CRN of the custom NAR configuration.
+  CreateDeploymentResponse:
     type: object
-    description: Request object for a create user access key request.
+    description: Response object from creating a deployment.
+    x-workload: true
+    x-client-only: true
     properties:
-      user:
-        type: string
-        description: The ID or CRN of the user to whom this access key will be associated. If it is not included, it defaults to the user making the request.
-      type:
-        type: string
-        description: The version of an access key to create. Default is V2. Use V1 for compatibility with old CLI (< 1.6)  and SDK (< 1.3) releases.
-        enum:
-          - V1
-          - V2
-  CreateUserAccessKeyResponse:
-    type: object
-    description: Response object for a create user access key request.
-    required:
-      - accessKey
-      - privateKey
-    properties:
-      accessKey:
-        $ref: '#/definitions/AccessKey'
-        description: The access key that was created.
-      privateKey:
-        type: string
-        description: The private key associated with this access key. This string is the contents of a PEM file containing a PKCS#8 private key.
-        x-sensitive: true
-  CreateMachineUserAccessKeyRequest:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  CreateInboundConnectionEndpointRequest:
     type: object
-    description: Request object for a create machine user access key request.
-    required:
-      - machineUserName
+    description: Request object that contains FQDN for the Inbound Connection Endpoint to create
+    x-workload: true
+    x-client-only: true
     properties:
-      machineUserName:
-        type: string
-        description: The name or CRN of the machine user to whom this access key will be associated.
-      type:
+      environmentCrn:
         type: string
-        description: The version of an access key to create. Default is V2. Use V1 for compatibility with old CLI (< 1.6)  and SDK (< 1.3) releases.
-        enum:
-          - V1
-          - V2
-  CreateMachineUserAccessKeyResponse:
-    type: object
-    description: Response object for a create machine user access key request.
-    required:
-      - accessKey
-      - privateKey
-    properties:
-      accessKey:
-        $ref: '#/definitions/AccessKey'
-        description: The access key that was created.
-      privateKey:
+        description: The CRN of an environment to execute the command.
+      hostname:
         type: string
-        description: The private key associated with this access key. This string is the contents of a PEM file containing a PKCS#8 private key.
-        x-sensitive: true
-  DeleteAccessKeyRequest:
-    type: object
-    description: Request object for a delete access key request.
+        description: Fully qualified domain name
     required:
-      - accessKeyId
-    properties:
-      accessKeyId:
-        type: string
-        description: The ID of the access key.
-  DeleteAccessKeyResponse:
+      - environmentCrn
+  CreateInboundConnectionEndpointResponse:
     type: object
-    description: Response object for a delete access key request.
-  UpdateAccessKeyRequest:
+    description: Response object returned during Inbound Connection Endpoint creation
+    x-workload: true
+    x-client-only: true
+    properties:
+      inboundConnectionEndpointSummary:
+        description: Data that describes the Inbound Connection Endpoint.
+        $ref: '#/definitions/InboundConnectionEndpointSummary'
+  DeleteCustomNarConfigurationRequest:
     type: object
-    description: Request object for an update access key request.
+    description: Request object for deleting a custom NAR configuration by CRN.
+    x-workload: true
+    x-client-only: true
     required:
-      - accessKeyId
-      - status
+      - environmentCrn
+      - configurationVersion
+      - customNarConfigurationCrn
     properties:
-      accessKeyId:
+      environmentCrn:
         type: string
-        description: The ID of the access key to update.
-      status:
+        description: The CRN of an environment to execute the command.
+      customNarConfigurationCrn:
         type: string
-        description: The status to assign to the access key.
-        enum:
-          - ACTIVE
-          - INACTIVE
-  UpdateAccessKeyResponse:
+        description: The CRN of the custom NAR configuration to delete.
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of the configuration
+  DeleteCustomNarConfigurationResponse:
     type: object
-    description: Response object for an update access key request.
+    description: Response object for deleting a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - accessKey
-    properties:
-      accessKey:
-        $ref: '#/definitions/AccessKey'
-        description: The access key that was updated.
-  GetAccessKeyRequest:
-    type: object
-    description: Request object for a get access key request.
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      accessKeyId:
+      username:
+        type: string
+        description: The username used to access the storage location
+      password:
+        type: string
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The ID of the access key to get information about. If it is not included, it defaults to the access key used to make the request.
-  GetAccessKeyResponse:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of the configuration
+      crn:
+        type: string
+        description: The CRN of the custom NAR configuration to update.
+  DeleteInboundConnectionEndpointRequest:
     type: object
-    description: Response object for a get access key request.
+    description: Request object that contains the identifier of the Inbound Connection Endpoint to delete
+    x-workload: true
+    x-client-only: true
     required:
-      - accessKey
+      - environmentCrn
+      - crn
     properties:
-      accessKey:
-        $ref: '#/definitions/AccessKey'
-        description: Information about the access key.
-  ListAccessKeysRequest:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      crn:
+        type: string
+        description: The CRN of the Inbound Connection Endpoint
+  DeleteInboundConnectionEndpointResponse:
+    type: object
+    description: Response object returned during deletion of an Inbound Connection Endpoint
+    x-workload: true
+    x-client-only: true
+  DeploymentConfiguration:
     type: object
-    description: Request object for a list access keys request.
+    description: Provides all of the configuration that dictates how a flow should be deployed
+    x-workload: true
+    x-client-only: true
+    required:
+      - configurationVersion
     properties:
-      accessKeyIds:
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of this configuration
+      parameterGroups:
         type: array
+        description: The list of flow parameter groups
         items:
-          type: string
-        description: The access key IDs or CRNs of the access keys.
-      pageSize:
+          $ref: '#/definitions/FlowParameterGroup'
+      autoScalingEnabled:
+        type: boolean
+        description: Specifies that auto-scaling should be enabled.
+      autoScaleMinNodes:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
-        type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListAccessKeysResponse:
-    type: object
-    description: Response object for a list access keys request.
-    required:
-      - accessKeys
-    properties:
-      accessKeys:
+        description: The minimum number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is true.
+      autoScaleMaxNodes:
+        type: integer
+        format: int32
+        description: The maximum number of nodes that the cluster should scale to. May only be specified when autoScalingEnabled is true.
+      staticNodeCount:
+        type: integer
+        format: int32
+        description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
+      kpis:
         type: array
+        description: The list of configured KPIs
         items:
-          $ref: '#/definitions/AccessKey'
-        x-paging-result: true
-        description: The access keys.
-      nextToken:
+          $ref: '#/definitions/ConfiguredKpi'
+      deploymentId:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  CreateSamlProviderRequest:
-    type: object
-    description: Request object for creating SAML provider request.
-    x-no-compatibility-guarantee: true
-    required:
-      - samlProviderName
-      - samlMetadataDocument
-    properties:
-      samlProviderName:
+        description: The id of the deployment.
+      deploymentCrn:
+        type: string
+        description: The CRN of the deployment.
+      name:
         type: string
-        description: The name of SAML provider. The name must be unique, must have a maximum of 128 characters, and must contain only alphanumeric characters, "-" and "_". Names are are not case-sensitive.
-      samlMetadataDocument:
+        description: The name of the deployment
+      cfmNifiVersion:
         type: string
-        description: SAML metadata document XML file. Length of meta data document cannot be more than 200 KB (200,000 bytes).
-        maxLength: 200000
-      syncGroupsOnLogin:
+        description: The CFM NiFi version associated with the deployment
+      autoStartFlow:
         type: boolean
-        description: Whether to sync group information for users federated with this SAML provider. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion. The default is to synchronize group membership.
-  CreateSamlProviderResponse:
-    type: object
-    description: Response object for a creating SAML provider request.
-    x-no-compatibility-guarantee: true
-    required:
-      - samlProvider
-    properties:
-      samlProvider:
-        $ref: '#/definitions/SamlProvider'
-        description: The SAML provider.
-  DeleteSamlProviderRequest:
-    type: object
-    description: Request object for deleting SAML provider request.
-    x-no-compatibility-guarantee: true
-    properties:
-      samlProviderName:
+        description: Indicates whether or not the flow should be started during deployment creation
+      clusterSizeName:
         type: string
-        description: The name or CRN of the SAML provider to delete.
-  DeleteSamlProviderResponse:
-    type: object
-    description: Response object for delete SAML provider request.
-    x-no-compatibility-guarantee: true
-  ListSamlProvidersRequest:
-    type: object
-    description: Request object for a list SAML providers request.
-    x-no-compatibility-guarantee: true
-    properties:
-      samlProviderNames:
+        description: The size of the cluster to deploy
+        enum:
+          - EXTRA_SMALL
+          - SMALL
+          - MEDIUM
+          - LARGE
+      parametersDirty:
+        type: boolean
+        description: Indicates whether or not all current parameter values have successfully been applied to NiFi
+        readOnly: true
+      kpisDirty:
+        type: boolean
+        description: Indicates whether or not the current KPIs have successfully been deployed as alert rules
+        readOnly: true
+      sizingAndScalingDirty:
+        type: boolean
+        description: Indicates whether or not the current sizing and scaling configuration has been successfully applied in Kubernetes
+        readOnly: true
+      lastUpdatedByUsername:
+        type: string
+        description: The username of the last person to update the deployment configuration
+        readOnly: true
+      inboundHostname:
+        type: string
+        description: The inbound hostname
+      listenComponents:
         type: array
-        description: The SAML providers names or CRNs to retrieve. If empty all SAML providers will be returned.
+        description: Listen components port and protocol data
         items:
-          type: string
-          description: The SAML providers names or CRNs to retrieve. If empty all SAML providers will be returned.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
-        type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListSamlProvidersResponse:
+          $ref: '#/definitions/ListenComponent'
+  DeploymentStatus:
     type: object
-    description: Response object for a list SAML providers request.
-    x-no-compatibility-guarantee: true
+    description: The state and state message associated with a deployment
+    x-workload: true
+    x-client-only: true
     required:
-      - samlProviders
+      - detailedState
+      - state
     properties:
-      samlProviders:
-        type: array
-        items:
-          $ref: '#/definitions/SamlProvider'
-        x-paging-result: true
-        description: The SAML providers.
-      nextToken:
+      detailedState:
+        type: string
+        description: The detailed state that the deployment is currently in
+        enum:
+          - GOOD_HEALTH
+          - FAILED_TO_SUSPEND
+          - FAILED_TO_UPDATE_NIFI_VERSION
+          - FAILED_TO_START
+          - FAILED_TO_RESTART
+          - SUSPENDED
+          - FAILED_TO_DEPLOY
+          - FAILED_TO_IMPORT
+          - FAILED_TO_UPDATE
+          - FAILED_TO_TERMINATE
+          - NEW
+          - CREATING_NODES
+          - DEPLOYING_ASSETS
+          - DEPLOYING_FLOW_DEFINITION
+          - IMPORTING_FLOW
+          - STARTING_FLOW
+          - SUSPENDING_FLOW
+          - UPDATING
+          - UPDATING_NIFI_VERSION
+          - CANCELLING_NIFI_VERSION_UPDATE
+          - RESTARTING
+          - TERMINATING
+          - CANCEL_REQUESTED
+          - STOPPED
+          - UNKNOWN
+          - UPGRADING
+          - FAILED_TO_UPGRADE
+          - ROLLING_BACK
+          - KPI_OUT_OF_RANGE
+          - CANNOT_AUTOSCALE
+          - DEPLOYMENT_DISCONNECTED
+          - UNUSED_LOGICAL_BAD_HEALTH
+          - AT_CAPACITY
+          - SDX_OUTPUT_CHANGED
+          - METRICS_UNAVAILABLE
+          - METERING_WARNING
+          - METERING_OFFLINE
+          - CERTIFICATE_RENEWED
+          - NOT_HEALTHY
+      state:
+        type: string
+        description: The state that the deployment is currently in
+        enum:
+          - DEPLOYING
+          - GOOD_HEALTH
+          - CONCERNING_HEALTH
+          - BAD_HEALTH
+          - IMPORTING_FLOW
+          - STARTING_FLOW
+          - SUSPENDING_FLOW
+          - SUSPENDED
+          - UPDATING
+          - TERMINATING
+          - RESTARTING
+          - UPGRADING
+          - ROLLING_BACK
+          - STOPPED
+          - UNKNOWN
+      message:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  UpdateSamlProviderRequest:
+        description: Detail message relating to the current status of the deployment
+  DescribeInboundConnectionEndpointRequest:
     type: object
-    description: Request object for an updating SAML provider request.
-    x-no-compatibility-guarantee: true
+    description: Request object that contains the identifier of the Inbound Connection Endpoint to describe
+    x-workload: true
+    x-client-only: true
     required:
-      - samlProviderName
+      - environmentCrn
+      - crn
     properties:
-      samlProviderName:
+      environmentCrn:
         type: string
-        description: The name or CRN of SAML provider to update.
-      samlMetadataDocument:
+        description: The CRN of an environment to execute the command.
+      crn:
         type: string
-        description: SAML metadata document XML file. Length of meta data document cannot be more than 200 KB (200,000 bytes). Can be omitted if no update is required.
-        maxLength: 200000
-      syncGroupsOnLogin:
-        type: boolean
-        description: Whether to sync group information for users federated with this SAML provider. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion. The default is to synchronize group membership. Can be omitted if no update is required.
-  UpdateSamlProviderResponse:
+        description: The CRN of the Inbound Connection Endpoint
+  DescribeInboundConnectionEndpointResponse:
     type: object
-    description: Response object for an updating SAML provider request.
-    x-no-compatibility-guarantee: true
-    required:
-      - samlProvider
+    description: Response object that describes an Inbound Connection Endpoint
+    x-workload: true
+    x-client-only: true
     properties:
-      samlProvider:
-        $ref: '#/definitions/SamlProvider'
-        description: The SAML provider.
-  ListRolesRequest:
+      inboundConnectionEndpointSummary:
+        description: Data that describes the Inbound Connection Endpoint.
+        $ref: '#/definitions/InboundConnectionEndpointSummary'
+  EnvCloudRegion:
     type: object
-    description: Request object for a list roles request.
+    description: A cloud region
+    x-workload: true
+    x-client-only: true
     properties:
-      roleNames:
-        type: array
-        items:
-          type: string
-        description: The roles names or CRNs to retrieve. If empty all roles will be returned.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+      name:
+        type: string
+        description: Name of the cloud region
+      displayName:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListRolesResponse:
+        description: Display-friendly name of the cloud region
+  Error:
     type: object
-    description: Response object for a list roles request.
-    required:
-      - roles
+    description: An object returned on an error.
+    x-workload: true
+    x-client-only: true
     properties:
-      roles:
-        type: array
-        items:
-          $ref: '#/definitions/Role'
-        x-paging-result: true
-        description: The list of roles in the account.
-      nextToken:
+      code:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListResourceRolesRequest:
+        description: The error code.
+      message:
+        type: string
+        description: The error message.
+  FlowParameter:
     type: object
-    description: Request object for a list resource roles request.
+    description: A flow parameter
+    x-workload: true
+    x-client-only: true
     properties:
-      resourceRoleNames:
+      name:
+        type: string
+        description: The name of the parameter
+      description:
+        type: string
+        description: The description of the param
+      value:
+        type: string
+        description: The value of the parameter
+        x-no-paramfile: true
+      sensitive:
+        type: boolean
+        description: Whether or not the parameter value is sensitive
+      type:
+        type: string
+        description: The type of parameter. Possibly TEXT, FILE, FILES, DIRECTORY
+        enum:
+          - TEXT
+          - FILE
+          - FILES
+      assetReferences:
         type: array
+        description: The list of referenced assets.
         items:
-          type: string
-        description: The resource roles CRNs to retrieve. If empty all resource roles will be returned.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
-        type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListResourceRolesResponse:
+          $ref: '#/definitions/AssetReference'
+  FlowParameterGroup:
     type: object
-    description: Response object for a list resource roles request.
-    required:
-      - resourceRoles
+    description: A flow parameter group
+    x-workload: true
+    x-client-only: true
     properties:
-      resourceRoles:
+      name:
+        type: string
+        description: The name of the parameter group
+      parameters:
         type: array
+        description: The parameters in the group
         items:
-          $ref: '#/definitions/ResourceRole'
-        x-paging-result: true
-        description: The list of resource roles. Cannot be empty.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  AssignUserRoleRequest:
+          $ref: '#/definitions/FlowParameter'
+  GetCustomNarConfigurationRequest:
     type: object
-    description: Request object for an assign user role request.
-    required:
-      - user
-      - role
+    description: Request object for retrieving a custom NAR configuration by CRN.
+    x-workload: true
+    x-client-only: true
     properties:
-      user:
+      environmentCrn:
         type: string
-        description: The user the role is assigned to. Can be the user's CRN or id.
-      role:
+        description: The CRN of an environment to execute the command.
+      customNarConfigurationCrn:
         type: string
-        description: The role to assign to the user. Can be the role's CRN or name.
-  AssignUserRoleResponse:
-    type: object
-    description: Response object for an assign user role request.
-  UnassignUserRoleRequest:
+        description: The CRN of the custom NAR configuration to retrieve.
+    required:
+      - environmentCrn
+  GetCustomNarConfigurationResponse:
     type: object
-    description: Request object for an unassign user role request.
+    description: Response object for retrieving a custom NAR configuration by CRN.
+    x-workload: true
+    x-client-only: true
     required:
-      - user
-      - role
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      user:
+      username:
+        type: string
+        description: The username used to access the storage location
+      password:
         type: string
-        description: The user to unassigned the roles from. Can be the user CRN or id.
-      role:
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The role to unassigned from the user. Can be the role's CRN or name.
-  UnassignUserRoleResponse:
-    type: object
-    description: Response object for an unassign user role request.
-  AssignUserResourceRoleRequest:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of the configuration
+      crn:
+        type: string
+        description: The CRN of the custom NAR configuration to update.
+  GetDefaultCustomNarConfigurationRequest:
     type: object
-    description: Request object for an assign user resource role request.
+    description: Request object for retrieving the default custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - user
-      - resourceRoleCrn
-      - resourceCrn
+      - environmentCrn
     properties:
-      user:
-        type: string
-        description: The user to assign the resource role to. Can be the user's CRN or id.
-      resourceRoleCrn:
-        type: string
-        description: The CRN of the resource role to assign to the user.
-      resourceCrn:
+      environmentCrn:
         type: string
-        description: The resource for which the resource role rights are granted.
-  AssignUserResourceRoleResponse:
+        description: The CRN of an environment to execute the command.
+  GetDefaultCustomNarConfigurationResponse:
     type: object
-    description: Response object for an assign user resource role request.
-  UnassignUserResourceRoleRequest:
-    type: object
-    description: Request object for an unassign user role request.
+    description: Response object for retrieving the default custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - user
-      - resourceRoleCrn
-      - resourceCrn
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      user:
-        type: string
-        description: The user to unassign the resource role from.
-      resourceRoleCrn:
+      username:
         type: string
-        description: The CRN of the resource role to unassigned from the user.
-      resourceCrn:
+        description: The username used to access the storage location
+      password:
         type: string
-        description: The CRN of the resource for which the resource role rights will be unassigned.
-  UnassignUserResourceRoleResponse:
-    type: object
-    description: Response object for an unassign user role request.
-  ListUserAssignedRolesRequest:
-    type: object
-    description: Request object for a list user assigned roles request.
-    properties:
-      user:
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The user to list the assigned roles for. Can be the user's CRN or id. If it is not included, it defaults to the user making the request.
-      pageSize:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The version of the configuration
+      crn:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListUserAssignedRolesResponse:
+        description: The CRN of the custom NAR configuration to update.
+  GetDeploymentConfigurationMetadataRequest:
     type: object
-    description: Response object for a list user assigned roles request.
+    description: Request object for retrieving deployment configuration metadata.
+    x-workload: true
+    x-client-only: true
     required:
-      - roleCrns
-    properties:
-      roleCrns:
-        type: array
-        items:
-          type: string
-        x-paging-result: true
-        description: The role CRNs assigned to the user.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListUserAssignedResourceRolesRequest:
-    type: object
-    description: Request object for a list user assigned resource roles request.
+      - environmentCrn
+      - deploymentCrn
     properties:
-      user:
+      environmentCrn:
         type: string
-        description: The user to list the assigned roles for. Can be the user's CRN or id. If it is not included, it defaults to the user making the request.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListUserAssignedResourceRolesResponse:
+        description: The deployment crn.
+  GetDeploymentConfigurationMetadataResponse:
     type: object
-    description: Response object for a list user assigned roles request.
-    required:
-      - resourceAssignments
+    description: Response object for retrieving deployment configuration metadata request.
+    x-workload: true
+    x-client-only: true
     properties:
-      resourceAssignments:
-        type: array
-        items:
-          $ref: '#/definitions/ResourceAssignment'
-        x-paging-result: true
-        description: The user's resource assignments.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  AssignMachineUserRoleRequest:
+      deploymentConfigurationMetadata:
+        description: The deployment configuration metadata.
+        $ref: '#/definitions/RpcDeploymentConfigurationMetadata'
+  GetDeploymentConfigurationRequest:
     type: object
-    description: Request object for an assign machine user role request.
+    description: Request object for retrieving deployment configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
-      - role
+      - environmentCrn
+      - deploymentCrn
     properties:
-      machineUserName:
+      environmentCrn:
         type: string
-        description: The machine user the role is assigned to. Can be the machine user's name or CRN.
-      role:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        description: The role to assign to the machine user. Can be the role's name or CRN.
-  AssignMachineUserRoleResponse:
+        description: The deployment crn.
+  GetDeploymentConfigurationResponse:
     type: object
-    description: Response object for an assign machine user role request.
-  UnassignMachineUserRoleRequest:
+    description: Response object for retrieving deployment configuration request.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deploymentConfiguration:
+        description: The deployment configuration.
+        $ref: '#/definitions/DeploymentConfiguration'
+  GetDeploymentRequestDetailsRequest:
     type: object
-    description: Request object for an unassign machine user role request.
+    description: Request object for retrieving deployment request details.
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
-      - role
+      - environmentCrn
+      - deploymentRequestCrn
     properties:
-      machineUserName:
+      environmentCrn:
         type: string
-        description: The machine user to unassigned the roles from. Can be the machine user's name or CRN.
-      role:
+        description: The CRN of an environment to execute the command.
+      deploymentRequestCrn:
         type: string
-        description: The role to unassigned from the user. Can be the role's name or CRN.
-  UnassignMachineUserRoleResponse:
+        description: The deployment request crn.
+  GetDeploymentRequestDetailsResponse:
     type: object
-    description: Response object for an unassign machine user role request.
-  AssignMachineUserResourceRoleRequest:
+    description: Response object for retrieving deployment request details request.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deploymentConfigurationMetadata:
+        description: The deployment configuration metadata.
+        $ref: '#/definitions/RpcDeploymentConfigurationMetadata'
+  InboundConnectionEndpointCertificateSummary:
     type: object
-    description: Request object for an assign machine user resource role request.
-    required:
-      - machineUserName
-      - resourceRoleCrn
-      - resourceCrn
+    description: Inbound Connection Endpoint Certificate Summary
+    x-workload: true
+    x-client-only: true
     properties:
-      machineUserName:
-        type: string
-        description: The machine user to assign the resource role to. Can be the user's name or CRN.
-      resourceRoleCrn:
+      expiration:
+        type: integer
+        format: int64
+        description: The timestamp of when the Inbound Connection Endpoint Certificate expires
+        readOnly: true
+      certificateType:
         type: string
-        description: The CRN of the resource role to assign to the machine user.
-      resourceCrn:
+        description: The type of the Inbound Connection Endpoint Certificate
+        readOnly: true
+        enum:
+          - CLIENT_ENTITY
+          - CLIENT_CA
+          - SERVER_ENTITY
+      state:
         type: string
-        description: The resource for which the resource role rights are granted.
-  AssignMachineUserResourceRoleResponse:
-    type: object
-    description: Response object for an assign machine user resource role request.
-  UnassignMachineUserResourceRoleRequest:
-    type: object
-    description: Request object for an unassign machine user role request.
-    required:
-      - machineUserName
-      - resourceRoleCrn
-      - resourceCrn
+        description: The state of the Inbound Connection Endpoint Certificate
+        readOnly: true
+        enum:
+          - PROVISIONING
+          - CURRENT
+          - EXPIRED
+          - RENEWING
+          - RENEWAL_FAILED
+      statusMessage:
+        type: string
+        description: The status message of the Inbound Connection Endpoint Certificate
+        readOnly: true
+  InboundConnectionEndpointClientCertificateRequest:
+    type: object
+    description: Request object to retrieve Inbound Connection Endpoint client's certificate.
+    x-workload: true
+    x-client-only: true
     properties:
-      machineUserName:
+      environmentCrn:
         type: string
-        description: The machine user to unassign the resource role from.
-      resourceRoleCrn:
+        description: The CRN of an environment to execute the command.
+      id:
         type: string
-        description: The CRN of the resource role to unassigned from the machine user.
-      resourceCrn:
+        description: The Inbound Connection Endpoint identifier. Deprecated. Use 'crn' instead
+        x-deprecated: true
+      crn:
         type: string
-        description: The CRN of the resource for which the resource role rights will be unassigned.
-  UnassignMachineUserResourceRoleResponse:
-    type: object
-    description: Response object for an unassign machine user role request.
-  ListMachineUserAssignedRolesRequest:
-    type: object
-    description: Request object for a list machine user assigned roles request.
+        description: The CRN of the Inbound Connection Endpoint
     required:
-      - machineUserName
-    properties:
-      machineUserName:
-        type: string
-        description: The machine user to list the assigned roles for. Can be the machine user's name or CRN.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
-        type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListMachineUserAssignedRolesResponse:
+      - environmentCrn
+  InboundConnectionEndpointClientCertificateResponse:
     type: object
-    description: Response object for a list machine user assigned roles request.
-    required:
-      - roleCrns
+    description: Response object that contains the client's certificate.
+    x-workload: true
+    x-client-only: true
     properties:
-      roleCrns:
-        type: array
-        items:
-          type: string
-        x-paging-result: true
-        description: The role CRNs assigned to the user.
-      nextToken:
+      certificate:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListMachineUserAssignedResourceRolesRequest:
+        description: The client's encoded certificate.
+        readOnly: true
+  InboundConnectionEndpointClientPrivateKeyRequest:
     type: object
-    description: Request object for a list machine user assigned resource roles request.
-    required:
-      - machineUserName
+    description: Request object to retrieve Inbound Connection Endpoint client's private key.
+    x-workload: true
+    x-client-only: true
     properties:
-      machineUserName:
+      environmentCrn:
         type: string
-        description: The machine user to list the assigned resource roles for. Can be the machine user's name or CRN.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The CRN of an environment to execute the command.
+      id:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListMachineUserAssignedResourceRolesResponse:
-    type: object
-    description: Response object for a list machine user assigned roles request.
+        description: The Inbound Connection Endpoint identifier. Deprecated. Use 'crn' instead
+        x-deprecated: true
+      crn:
+        type: string
+        description: The CRN of the Inbound Connection Endpoint
     required:
-      - resourceAssignments
+      - environmentCrn
+  InboundConnectionEndpointClientPrivateKeyResponse:
+    type: object
+    description: Response object that contains the client's private key.
+    x-workload: true
+    x-client-only: true
     properties:
-      resourceAssignments:
+      privateKey:
+        type: string
+        description: The client's encoded private key.
+        readOnly: true
+  InboundConnectionEndpointSummary:
+    type: object
+    description: Inbound Connection Endpoint Summary
+    x-workload: true
+    x-client-only: true
+    properties:
+      fullyQualifiedDomainName:
+        type: string
+        description: The FQDN of the inbound connection hostname
+        readOnly: true
+      state:
+        type: string
+        description: State of the Inbound Connection Endpoint
+        readOnly: true
+        enum:
+          - UNASSIGNED
+          - ASSIGNED
+          - PROVISIONING_CERTIFICATES
+          - RENEWING_CERTIFICATES
+          - READY
+          - FAILED
+      deploymentCrn:
+        type: string
+        description: The CRN of the deployment the hostname is assigned to
+        readOnly: true
+      crn:
+        type: string
+        description: The CRN of the Inbound Connection Endpoint
+        readOnly: true
+      certificateSummaries:
         type: array
+        description: The summaries of certificates associated with the Inbound Connection Endpoint
+        readOnly: true
+        uniqueItems: true
         items:
-          $ref: '#/definitions/ResourceAssignment'
-        x-paging-result: true
-        description: The user's resource assignments.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListResourceAssigneesRequest:
+          $ref: '#/definitions/InboundConnectionEndpointCertificateSummary'
+  KpiContextGroup:
     type: object
-    description: Request object for a list resource assignees request.
+    description: Captures the use of a KPI in the context of a process group
+    x-workload: true
+    x-client-only: true
     required:
-      - resourceCrn
+      - id
+      - name
     properties:
-      resourceCrn:
+      id:
         type: string
-        description: The resource CRN for which to list the assignees.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The id of the containing process group
+      name:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListResourceAssigneesResponse:
+        description: The name of the containing process group
+      scopeComponents:
+        type: array
+        description: The scope components of the group
+        items:
+          $ref: '#/definitions/KpiScopeComponent'
+  KpiMetaData:
     type: object
-    description: Response object for a list resource assignees request.
+    description: A template for instantiating KPIs
+    x-workload: true
+    x-client-only: true
     required:
-      - resourceAssignees
+      - alertFrequencyTolerance
+      - kpiScopes
+      - unitTypes
     properties:
-      resourceAssignees:
+      kpiScopes:
         type: array
+        description: The KPI scope meta data list, one per MetricComponentType.
         items:
-          $ref: '#/definitions/ResourceAssignee'
-        x-paging-result: true
-        description: List of resource assignees and their respective resource roles for the resource.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  CreateMachineUserRequest:
+          $ref: '#/definitions/KpiScopeMetaData'
+      unitTypes:
+        type: object
+        description: The entire tree of legal unit types for all metrics.
+        additionalProperties:
+          type: array
+          items:
+            $ref: '#/definitions/KpiUnit'
+      alertFrequencyTolerance:
+        description: The alert frequency tolerance shared by all metrics.
+        $ref: '#/definitions/AlertFrequencyTolerance'
+  KpiScopeComponent:
     type: object
-    description: Request object for create machine user request.
+    description: Provides scoping when defining KPIs
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
+      - id
+      - name
     properties:
-      machineUserName:
+      id:
+        type: string
+        description: The internal id of the scope, for example the connection ID
+      name:
         type: string
-        description: The name to use for the new machine user. The name should be an alpha numeric string, including '-' and '_', no longer than 128 characters long. Only one machine user with this name can be exist at a given time in an account.
-  CreateMachineUserResponse:
+        description: The child name to show in the hierarchical chooser
+  KpiScopeMetaData:
     type: object
-    description: Response object for create machine user request.
+    description: Provides scoping meta data for use during KPI creation
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUser
+      - label
+      - metricTypes
+      - type
     properties:
-      machineUser:
-        $ref: '#/definitions/MachineUser'
-        description: Information about the machine user.
-  ListMachineUsersRequest:
-    type: object
-    description: Request object for a list machine users request.
-    properties:
-      machineUserNames:
+      type:
+        type: string
+        description: The type of the scope
+        enum:
+          - SYSTEM
+          - NIFI_FLOW
+          - NIFI_PROCESSOR
+          - NIFI_PROCESS_GROUP
+          - NIFI_CONNECTION
+      metricTypes:
         type: array
+        description: The available metric types for the chosen scope type
         items:
-          type: string
-        description: The machine user names or CRNs of the macihne users. If not provided all machine users for the account are retrieved.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+          $ref: '#/definitions/KpiScopeMetricType'
+      label:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListMachineUsersResponse:
-    type: object
-    description: Response object for a list machine users request.
-    required:
-      - machineUsers
-    properties:
-      machineUsers:
+        description: The label to use for the chosen scope type
+      contextGroups:
         type: array
+        description: The context identifiers for the chosen scope type
         items:
-          $ref: '#/definitions/MachineUser'
-        x-paging-result: true
-        description: The machine users.
-      nextToken:
+          $ref: '#/definitions/KpiContextGroup'
+      contextLabel:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  DeleteMachineUserRequest:
+        description: The label to use for the context identifier, which depends on scope type.
+  KpiScopeMetricType:
     type: object
-    description: Request object for delete machine user request.
+    description: Provides the legal metric types for an owning scope
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
+      - defaultUnitId
+      - id
+      - label
+      - unitTypeKey
     properties:
-      machineUserName:
+      id:
         type: string
-        description: The name or CRN of the machine user to delete.
-  DeleteMachineUserResponse:
-    type: object
-    description: Response object for delete machine user request.
-  CreateGroupRequest:
+        description: The internal id of the metric type
+      label:
+        type: string
+        description: The user-visible label of the metric type
+      unitTypeKey:
+        type: string
+        description: The unit type key for this metric
+        enum:
+          - DURATION
+          - RATIO
+          - SIZE
+          - RATE
+          - COUNT
+      defaultUnitId:
+        type: string
+        description: The default unitId for this metric
+      description:
+        type: string
+        description: The user-visible description of the metric type
+  KpiUnit:
+    type: object
+    description: Captures the legal units for a metric, a means to avoid large numbers either before or after a decimal point
+    x-workload: true
+    x-client-only: true
+    required:
+      - factor
+      - id
+      - label
+    properties:
+      id:
+        type: string
+        description: The internal ID of the unit
+      label:
+        type: string
+        description: The user-visible label of the unit
+      factor:
+        type: integer
+        format: int64
+        description: The conversion factor to use to normalize values with this unit into a common unit
+  ListInboundConnectionEndpointsRequest:
     type: object
-    description: Request object for create group request.
+    description: Request object to use to list Inbound Connection Endpoints
+    x-workload: true
+    x-client-only: true
     required:
-      - groupName
+      - environmentCrn
     properties:
-      groupName:
+      environmentCrn:
         type: string
-        description: The name of the group. This name must be unique, must have a maximum of 32 characters, and must contain only alphanumeric characters, "-" and "_". Also, the first character of the name must be alphabetic or an underscore. Names are are not case-sensitive. The group named administrators is reserved.
-      syncMembershipOnUserLogin:
-        x-no-compatibility-guarantee: true
-        type: boolean
-        description: Whether group membership is synced when a user logs in. The default is to sync group membership.
-  CreateGroupResponse:
+        description: The CRN of an environment to execute the command.
+  ListInboundConnectionEndpointsResponse:
     type: object
-    description: Response object for create group request.
-    required:
-      - group
+    description: Response object that contains a list of Inbound Connection Endpoints
+    x-workload: true
+    x-client-only: true
     properties:
-      group:
-        $ref: '#/definitions/Group'
-        description: Information about the group.
-  DeleteGroupRequest:
+      inboundConnectionEndpoints:
+        type: array
+        description: A list of Inbound Connection Endpoints.
+        readOnly: true
+        items:
+          $ref: '#/definitions/InboundConnectionEndpointSummary'
+  ListNifiVersionsRequest:
     type: object
-    description: Request object for delete group request.
+    description: Request object for listing the supported NiFi versions.
+    x-workload: true
+    x-client-only: true
     required:
-      - groupName
+      - environmentCrn
     properties:
-      groupName:
+      environmentCrn:
         type: string
-        description: The name or CRN of the group to delete.
-  DeleteGroupResponse:
-    type: object
-    description: Response object for delete group request.
-  ListGroupsRequest:
+        description: The CRN of an environment to execute the command.
+  ListNifiVersionsResponse:
     type: object
-    description: Request object for a list groups request.
+    description: Response object for listing the supported NiFi versions.
+    x-workload: true
+    x-client-only: true
     properties:
-      groupNames:
+      nifiVersions:
         type: array
+        description: A list of supported NiFi versions.
         items:
           type: string
-        description: The group names or CRNs of the groups. If not provided, all groups in the account are retrieved.
-      pageSize:
-        type: integer
-        format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
-        type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupsResponse:
+  ListenComponent:
     type: object
-    description: Response object for a list groups request.
+    description: Provides subset of metadata of a Listen* component
+    x-workload: true
+    x-client-only: true
     required:
-      - groups
+      - protocol
     properties:
-      groups:
-        type: array
-        items:
-          $ref: '#/definitions/Group'
-        x-paging-result: true
-        description: The list of groups.
-      nextToken:
+      protocol:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  UpdateGroupRequest:
-    type: object
-    description: Request object for update group request.
-    x-no-compatibility-guarantee: true
-    required:
-      - groupName
-    properties:
-      groupName:
+        description: Inbound protocol
+        enum:
+          - TCP
+          - UDP
+      listenComponentType:
         type: string
-        description: The name or CRN of the group to update.
-      syncMembershipOnUserLogin:
-        type: boolean
-        description: Whether group membership is synced when a user logs in. Can be omitted if no update is required.
-  UpdateGroupResponse:
-    type: object
-    description: Response object for update group request.
-    x-no-compatibility-guarantee: true
-    required:
-      - group
-    properties:
-      group:
-        $ref: '#/definitions/Group'
-        description: Information about the updated group.
-  AddUserToGroupRequest:
-    type: object
-    description: Request object for an add user to group request.
+        description: Listen component type
+        readOnly: true
+        enum:
+          - ListenHTTP
+          - ListenFTP
+          - ListenSyslog
+          - ListenRELP
+          - ListenTCP
+          - ListenUDP
+          - ListenTCPRecord
+          - ListenUDPRecord
+          - ListenGRPC
+          - ListenSMTP
+          - ListenBeats
+          - ListenLumberjack
+          - ListenWebSocket
+          - HandleHttpRequest
+      port:
+        type: string
+        description: Inbound port
+  RenewInboundConnectionEndpointCertificateRequest:
+    type: object
+    description: Request object to renew Inbound Connection Endpoint certificate(s)
+    x-workload: true
+    x-client-only: true
     required:
-      - userId
-      - groupName
+      - environmentCrn
+      - crn
     properties:
-      userId:
+      environmentCrn:
         type: string
-        description: The ID or CRN of the user to add to the group.
-      groupName:
+        description: The CRN of an environment to execute the command.
+      crn:
         type: string
-        description: The name or CRN of the group to add the user to.
-  AddUserToGroupResponse:
-    type: object
-    description: Response object for an add user to group request.
-  AddMachineUserToGroupRequest:
+        description: The CRN of the Inbound Connection Endpoint
+      renewServerCertificate:
+        type: boolean
+        description: Whether to renew Inbound Connection Endpoint's server certificate
+      renewClientCertificates:
+        type: boolean
+        description: Whether to renew Inbound Connection Endpoint's client certificates
+      revokeClientCertificates:
+        type: boolean
+        description: Whether to revoke existing Inbound Connection Endpoint's client certificates
+  RenewInboundConnectionEndpointCertificateResponse:
     type: object
-    description: Request object for an add machine user to group request.
+    description: Response object for Inbound Connection Endpoint certificate renewal request
+    x-workload: true
+    x-client-only: true
+  RpcDeployment:
+    type: object
+    description: Provides details about a deployment.
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
-      - groupName
+      - name
+      - service
+      - status
     properties:
-      machineUserName:
+      name:
         type: string
-        description: The name or CRN of the machine user to add to the group.
-      groupName:
+        description: The name of the deployment
+      status:
+        description: The status of the deployment
+        $ref: '#/definitions/DeploymentStatus'
+      service:
+        description: Simple information about the DataFlow service of the deployment
+        $ref: '#/definitions/ServiceMeta'
+      crn:
         type: string
-        description: The name or CRN of the group to add the machine user to.
-  AddMachineUserToGroupResponse:
-    type: object
-    description: Response object for add machine user to group request.
-  RemoveUserFromGroupRequest:
-    type: object
-    description: Request object for a remove user from group request.
-    required:
-      - userId
-      - groupName
-    properties:
-      userId:
+        description: The CRN of the deployment
+      activeInfoAlertCount:
+        type: integer
+        format: int64
+        description: Current count of active alerts classified as an info
+      activeWarningAlertCount:
+        type: integer
+        format: int64
+        description: Current count of active alerts classified as a warning
+      activeErrorAlertCount:
+        type: integer
+        format: int64
+        description: Current count of active alerts classified as an error
+      created:
+        type: integer
+        format: int64
+        description: Timestamp of the creation of the deployment
+      updated:
+        type: integer
+        format: int64
+        description: Timestamp of the last time the deployment was modified
+      validActions:
+        type: array
+        description: Valid actions that can be applied to the deployment in its current state
+        uniqueItems: true
+        items:
+          type: string
+          enum:
+            - VIEW_NIFI
+            - START_FLOW
+            - SUSPEND_FLOW
+            - EDIT
+            - CANCEL_CREATE
+            - TERMINATE
+            - VIEW_METRICS
+            - UPDATE_NIFI_VERSION
+            - CANCEL_NIFI_VERSION_UPDATE
+            - RESTART_DEPLOYMENT
+            - MANAGE_DEPLOYMENT
+      nifiUrl:
         type: string
-        description: The ID or CRN of the user to remove from the group.
-      groupName:
+        description: The url to open the deployed flow in NiFi
+      clusterSize:
         type: string
-        description: The name or CRN of the group to remove the user from.
-  RemoveUserFromGroupResponse:
-    type: object
-    description: Response object for a remove user from group request.
-  RemoveMachineUserFromGroupRequest:
-    type: object
-    description: Request object for a remove machine user from group request.
-    required:
-      - machineUserName
-      - groupName
-    properties:
-      machineUserName:
+        description: The initial size of the deployment
+        enum:
+          - EXTRA_SMALL
+          - SMALL
+          - MEDIUM
+          - LARGE
+      coresPerNode:
+        type: integer
+        format: int32
+        description: The number of cores per node for the deployment
+      heapSize:
+        type: number
+        format: double
+        description: The heap size for the deployment
+      autoscalingEnabled:
+        type: boolean
+        description: Whether or not autoscaling is enabled for this deployment
+      autoscaleMinNodes:
+        type: integer
+        format: int32
+        description: The minimum number of nodes that the deployment will allocate; can only be used when autoscalingEnabled is true
+      autoscaleMaxNodes:
+        type: integer
+        format: int32
+        description: The maximum number of nodes that the deployment can scale up to; can only be used when autoscalingEnabled is true
+      staticNodeCount:
+        type: integer
+        format: int32
+        description: The static number of nodes of the deployment; can only be used when autoscalingEnabled is false
+      flowName:
         type: string
-        description: The name or CRN of the machine user to add to the group.
-      groupName:
+        description: The name of the flow
+      flowVersion:
+        type: integer
+        format: int32
+        description: The version of the flow
+      flowVersionCrn:
         type: string
-        description: The name or CRN of the group to remove the machine user from.
-  RemoveMachineUserFromGroupResponse:
-    type: object
-    description: Response object for a remove machine user from group request.
-  ListGroupMembersRequest:
-    type: object
-    description: Request object for a list group members request.
-    required:
-      - groupName
-    properties:
-      groupName:
+        description: The deployment's current flow version CRN
+      flowCrn:
         type: string
-        description: The name or CRN of the group to list the membership of.
-      pageSize:
+        description: The deployment's current flow CRN
+      artifactTypeName:
+        type: string
+        description: The type of artifact of the flow
+      currentNodeCount:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The current node count
+      deployedByUsername:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupMembersResponse:
-    type: object
-    description: Response object for a list group members request.
-    required:
-      - memberCrns
-    properties:
-      memberCrns:
-        type: array
-        items:
-          type: string
-        description: The list of group members.
-        x-paging-result: true
-      nextToken:
+        description: The username of the person who deployed the flow
+      deployedByName:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListGroupsForUserRequest:
-    type: object
-    description: Request object for a list groups for user request.
-    required:
-      - userId
-    properties:
-      userId:
+        description: The name of the person who deployed the flow
+      dfxLocalUrl:
         type: string
-        description: The ID or CRN of the user to list the groups of.
-      pageSize:
+        description: Base URL to the CDF Local instance running this deployment
+      configurationVersion:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The current version of the deployment's configuration
+      lastUpdatedByUsername:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupsForUserResponse:
-    type: object
-    description: Response object for a list groups for user request.
-    required:
-      - groupCrns
-    properties:
-      groupCrns:
-        type: array
-        items:
-          type: string
-        x-paging-result: true
-        description: The list of groups.
-      nextToken:
+        description: The username of the last person to update the deployment
+      cfmNifiVersion:
+        type: string
+        description: The CFM NiFi version associated with the deployment
+      memoryLimit:
+        type: number
+        format: double
+        description: The memory limit of the deployment
+      inboundConnectionEndpointId:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListGroupsForMachineUserRequest:
+        description: The ID of Inbound Connection Endpoint assigned to the deployment
+      testSession:
+        type: boolean
+        description: Indicates this deployment was created as a test session for designing a flow
+      flowDesignerId:
+        type: string
+        description: The ID of the flow design for a test session deployment.
+      customNarConfigurationId:
+        type: string
+        description: The identifier of the custom NAR configuration, if used.
+  RpcDeploymentConfigurationMetadata:
     type: object
-    description: Request object for a list groups for machine user request.
+    description: Provides details about the deployment and all of the different configuration items that are available.
+    x-workload: true
+    x-client-only: true
     required:
-      - machineUserName
+      - flowCrn
+      - flowName
+      - flowVersion
+      - flowVersionCrn
+      - requiresEnvironmentSslContextService
+      - service
     properties:
-      machineUserName:
+      flowCrn:
         type: string
-        description: The name or CRN of the machine user to list the groups of.
-      pageSize:
+        description: The CRN of the flow to deploy
+      flowName:
+        type: string
+        description: The name of the flow to deploy
+      flowVersion:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The version of the flow to deploy
+      flowVersionCrn:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupsForMachineUserResponse:
-    type: object
-    description: Response object for a list groups for machine user request.
-    required:
-      - groupCrns
-    properties:
-      groupCrns:
+        description: The CRN for the flow version
+      service:
+        description: Simple information about the DataFlow service of the deployment
+        $ref: '#/definitions/ServiceMeta'
+      requiresEnvironmentSslContextService:
+        type: boolean
+        description: A flag indicating if the flow requires an Environment specific SSLContextService
+        readOnly: true
+      artifactTypeName:
+        type: string
+        description: The type of the artifact of the flow.
+        readOnly: true
+      parameterGroups:
         type: array
+        description: The list of flow parameter groups
         items:
-          type: string
-        x-paging-result: true
-        description: The list of groups.
-      nextToken:
-        type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  AssignGroupRoleRequest:
+          $ref: '#/definitions/FlowParameterGroup'
+      kpiMetaData:
+        description: The KPI meta data
+        $ref: '#/definitions/KpiMetaData'
+      clusterSizingOptions:
+        type: array
+        description: The options that are available for determining the size of the deployed cluster
+        items:
+          $ref: '#/definitions/ClusterSize'
+  ServiceMeta:
     type: object
-    description: Request object for an assign group role request.
+    description: The meta information about a DataFlow service.
+    x-workload: true
+    x-client-only: true
     required:
-      - groupName
-      - role
+      - cloudPlatform
+      - crn
+      - environmentCrn
+      - name
+      - region
     properties:
-      groupName:
+      crn:
         type: string
-        description: The group to which the role is assigned to. Can be the group name or CRN.
-      role:
+        description: The CRN of the DataFlow service
+      name:
         type: string
-        description: The role being assigned to the group. Can be the role's CRN or name.
-  AssignGroupRoleResponse:
-    type: object
-    description: Response object for an assign group role request.
-  UnassignGroupRoleRequest:
-    type: object
-    description: Request object for an unassign group role request.
-    required:
-      - groupName
-      - role
-    properties:
-      groupName:
+        description: The name of the DataFlow service
+      cloudPlatform:
         type: string
-        description: The group to unassign the role from. Can be the group name or CRN.
-      role:
-        type: string
-        description: The role to unassign from the group. Can be the role's CRN or name.
-  UnassignGroupRoleResponse:
-    type: object
-    description: Response object for an unassign group role request.
-  AssignGroupResourceRoleRequest:
-    type: object
-    description: Request object for an assign group resource role request.
-    required:
-      - groupName
-      - resourceRoleCrn
-      - resourceCrn
-    properties:
-      groupName:
+        description: The cloudPlatform flag of the DataFlow service
+        enum:
+          - AWS
+          - AZURE
+          - YARN
+          - YCLOUD
+          - GCP
+          - OPENSTACK
+          - LOCAL_K8S
+          - MOCK
+      region:
+        description: The region of the DataFlow service
+        $ref: '#/definitions/EnvCloudRegion'
+      environmentCrn:
+        type: string
+        description: Crn of associated CDP environment
+  TerminateDeploymentRequest:
+    type: object
+    description: Request object to terminate a deployment.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+  TerminateDeploymentResponse:
+    type: object
+    description: Response object for terminating a deployment request.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  TransitionFlowRequest:
+    type: object
+    description: Request object for transitioning the state of the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+      - flowState
+    properties:
+      environmentCrn:
         type: string
-        description: The group to assign the resource role to. Can be the group's name or CRN.
-      resourceRoleCrn:
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
         type: string
-        description: The CRN of the resource role being assigned to the group.
-      resourceCrn:
+        description: The deployment crn.
+      flowState:
         type: string
-        description: The resource for which the resource role rights are granted.
-  AssignGroupResourceRoleResponse:
-    type: object
-    description: Response object for an assign group resource role request.
-  UnassignGroupResourceRoleRequest:
-    type: object
-    description: Request object for an unassign group resource role request.
+        description: The desired state of the NiFi flow
+        enum:
+          - STARTED
+          - SUSPENDED
+  TransitionFlowResponse:
+    type: object
+    description: Response object for transitioning the state of the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  UpdateCustomNarConfigurationRequest:
+    type: object
+    description: Request object to update a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - groupName
-      - resourceRoleCrn
-      - resourceCrn
+      - environmentCrn
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      groupName:
+      environmentCrn:
         type: string
-        description: The group to unassign the resource role from.
-      resourceRoleCrn:
+        description: The CRN of an environment to execute the command.
+      username:
         type: string
-        description: The CRN of the resource role to unassign from the group.
-      resourceCrn:
+        description: The username used to access the storage location
+      password:
         type: string
-        description: The CRN of the resource for which the resource role rights will be unassigned.
-  UnassignGroupResourceRoleResponse:
-    type: object
-    description: Response object for an unassign group role request.
-  ListGroupAssignedRolesRequest:
-    type: object
-    description: Request object for a list group assigned roles request.
-    required:
-      - groupName
-    properties:
-      groupName:
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The group to list the assigned roles for. Can be the group's name or CRN.
-      pageSize:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The version of the configuration
+      crn:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupAssignedRolesResponse:
+        description: The CRN of the custom NAR configuration to update.
+  UpdateCustomNarConfigurationResponse:
     type: object
-    description: Response object for a list group assigned roles request.
+    description: Response object for updating a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
-      - roleCrns
+      - configurationVersion
+      - password
+      - storageLocation
+      - username
     properties:
-      roleCrns:
-        type: array
-        items:
-          type: string
-        x-paging-result: true
-        description: The role CRNs assigned to the group.
-      nextToken:
+      username:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  ListGroupAssignedResourceRolesRequest:
-    type: object
-    description: Request object for a list group assigned resource roles request.
-    required:
-      - groupName
-    properties:
-      groupName:
+        description: The username used to access the storage location
+      password:
+        type: string
+        description: The password used to access the storage location
+      storageLocation:
         type: string
-        description: The group to list the assigned resource roles for. Can be the group's name or CRN.
-      pageSize:
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
         type: integer
         format: int32
-        minimum: 1
-        maximum: 100
-        x-paging-page-size: true
-        description: The size of each page.
-      startingToken:
+        description: The version of the configuration
+      crn:
         type: string
-        x-paging-input-token: true
-        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
-  ListGroupAssignedResourceRolesResponse:
+        description: The CRN of the custom NAR configuration to update.
+  UpdateDeploymentRequest:
     type: object
-    description: Response object for a list group assigned resource roles request.
+    description: Provides all of the configuration that dictates how a flow should be deployed
+    x-workload: true
+    x-client-only: true
     required:
-      - resourceAssignments
+      - environmentCrn
+      - configurationVersion
+      - deploymentCrn
     properties:
-      resourceAssignments:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of this configuration
+      deploymentCrn:
+        type: string
+        description: The CRN of the existing deployment to be updated.
+      parameterGroups:
+        type: array
+        description: The list of flow parameter groups
+        items:
+          $ref: '#/definitions/FlowParameterGroup'
+      autoScalingEnabled:
+        type: boolean
+        description: Specifies that auto-scaling should be enabled.
+      autoScaleMinNodes:
+        type: integer
+        format: int32
+        description: The minimum number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is true.
+      autoScaleMaxNodes:
+        type: integer
+        format: int32
+        description: The maximum number of nodes that the cluster should scale to. May only be specified when autoScalingEnabled is true.
+      staticNodeCount:
+        type: integer
+        format: int32
+        description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
+      kpis:
         type: array
+        description: The list of configured KPIs
         items:
-          $ref: '#/definitions/ResourceAssignment'
-        x-paging-result: true
-        description: The group's resource assignments.
-      nextToken:
+          $ref: '#/definitions/ConfiguredKpi'
+      assetUpdateRequestCrn:
         type: string
-        x-paging-output-token: true
-        description: The token to use when requesting the next set of results. If not present, there are no additional results.
-  EnableClouderaSSOLoginRequest:
-    type: object
-    description: Request object for an enable Cloudera SSO login request.
-    x-no-compatibility-guarantee: true
-  EnableClouderaSSOLoginResponse:
-    type: object
-    description: Response object for an enable Cloudera SSO login request.
-    x-no-compatibility-guarantee: true
-  DisableClouderaSSOLoginRequest:
+        description: The CRN of the asset update request. Required when updating assets of an existing deployment.
+  UpdateDeploymentResponse:
     type: object
-    description: Request object for a disable Cloudera SSO login request.
-    x-no-compatibility-guarantee: true
-  DisableClouderaSSOLoginResponse:
-    type: object
-    description: Response object for a disable Cloudera SSO login request.
-    x-no-compatibility-guarantee: true
-  GetAccountRequest:
-    type: object
-    description: Request object for a get account request.
-    x-no-compatibility-guarantee: true
-  GetAccountResponse:
+    description: Response object from updating a deployment.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deploymentConfiguration:
+        description: The deployment configuration.
+        $ref: '#/definitions/DeploymentConfiguration'
+  UpdateNifiVersionRequest:
     type: object
-    description: Response object for a get account response.
-    x-no-compatibility-guarantee: true
+    description: Request object for updating the NiFi version of a deployment.
+    x-workload: true
+    x-client-only: true
     required:
-      - account
+      - environmentCrn
+      - cfmNifiVersion
+      - deploymentCrn
     properties:
-      account:
-        $ref: '#/definitions/Account'
-        description: The account object.
-  CreateUserRequest:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+      cfmNifiVersion:
+        type: string
+        description: The NiFi version to which to update the deployment.
+  UpdateNifiVersionResponse:
     type: object
-    description: Request object for creating user request.
-    x-no-compatibility-guarantee: true
+    description: Response object for updating the NiFi version of a deployment.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  UploadAssetRequest:
+    type: object
+    description: Request object for uploading an asset
+    x-workload: true
+    x-client-only: true
     required:
-      - samlProviderName
-      - identityProviderUserId
-      - email
+      - environmentCrn
+      - filePath
+      - parameterGroup
+      - parameterName
     properties:
-      samlProviderName:
+      environmentCrn:
         type: string
-        description: The name or CRN of the SAML provider the user will use for login.
-      identityProviderUserId:
+        description: The CRN of an environment to execute the command.
+      parameterGroup:
         type: string
-        description: The identity provider user id for the user. This ID must match the NameId attribute value that will be passed for the user in the SAML response using the associated SAML provider.
-      email:
+        description: The name of the parameter group
+      parameterName:
         type: string
-        description: The email address for the user. Used for display purposes only.
-      groups:
-        type: array
-        items:
-          type: string
-        description: The list of groups the user belongs to. The groups will be created if they do not exist.
-      firstName:
+        description: The name of the parameter within the parameter group
+      filePath:
+        type: string
+        description: The full local path to the file being uploaded
+      deploymentRequestCrn:
         type: string
-        description: The user first name.
-      lastName:
+        description: The CRN of the deployment request. Required during initial deployment.
+      deploymentName:
         type: string
-        description: The user last name.
-  CreateUserResponse:
+        description: The name of the deployment. Required during initial deployment.
+      assetUpdateRequestCrn:
+        type: string
+        description: The CRN of the asset update request. Required when updating assets of an existing deployment.
+  UploadAssetResponse:
     type: object
-    description: Response object for a create user request.
-    x-no-compatibility-guarantee: true
-    required:
-      - user
-    properties:
-      user:
-        $ref: '#/definitions/User'
-        description: Information about the user.
-  SetWorkloadPasswordRequest:
+    description: Response for uploading an asset.
+    x-workload: true
+    x-client-only: true
+  ValidateCustomNarConfigurationRequest:
     type: object
-    description: Request object for a set workload password request.
+    description: Request object for validating a custom NAR configuration.
+    x-workload: true
+    x-client-only: true
     required:
+      - environmentCrn
+      - configurationVersion
       - password
+      - storageLocation
+      - username
     properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      username:
+        type: string
+        description: The username used to access the storage location
       password:
         type: string
-        description: The password value to set
-        x-sensitive: true
-  SetWorkloadPasswordResponse:
-    type: object
-    description: Response object for a set workload password request.
-  SetWorkloadPasswordPolicyRequest:
-    type: object
-    description: Request object for a set workload password policy request.
-    x-no-compatibility-guarantee: true
-    properties:
-      maxPasswordLifetimeDays:
+        description: The password used to access the storage location
+      storageLocation:
+        type: string
+        description: The storage location, such as an S3 bucket or ADLS container
+      configurationVersion:
         type: integer
         format: int32
-        minimum: 0
-        description: The max lifetime of passwords, in days. If set to '0' passwords never expires.
-  SetWorkloadPasswordPolicyResponse:
+        description: The version of the configuration
+  ValidateCustomNarConfigurationResponse:
     type: object
-    description: Response object for a set workload password policy request.
-    x-no-compatibility-guarantee: true
+    description: Response object for validating custom NAR configuration.
+    x-workload: true
+    x-client-only: true
```

### Comparing `cdpcli-0.9.9/cdpcli/data/_retry.json` & `cdpcli-0.9.90/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/data/datalake/datalake.yaml` & `cdpcli-0.9.90/cdpcli/data/opdb/opdb.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,721 +1,779 @@
+x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: datalake
-x-interface-model: cdp
+x-endpoint-name: opdb
 x-products: CDP
+x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.1-SNAPSHOT
-  title: Cloudera Datalake Service
+  version: 0.9.90
+  title: Operational Database service
   license:
     name: Apache 2.0
-  description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
+  description: Interact with the Cloudera Operational Database service
+  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/datalake/createAWSDatalake:
+  /api/v1/opdb/collectDiagnostics:
     post:
-      summary: Creates an AWS datalake.
-      description: Creates an AWS datalake.
-      operationId: createAWSDatalake
+      summary: Collect diagnostic data bundles from the database
+      description: returns details of running command
+      operationId: collectDiagnostics
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAWSDatalakeRequest'
+            $ref: '#/definitions/CollectDiagnosticsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAWSDatalakeResponse'
+            $ref: '#/definitions/CollectDiagnosticsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/createAzureDatalake:
+      x-mutating: false
+  /api/v1/opdb/createDatabase:
     post:
-      summary: Creates an Azure datalake.
-      description: Creates an Azure datalake.
-      operationId: createAzureDatalake
+      summary: Create opDb
+      description: Create a operational database in a environment
+      operationId: createDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAzureDatalakeRequest'
+            $ref: '#/definitions/CreateDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAzureDatalakeResponse'
+            $ref: '#/definitions/CreateDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/listDatalakes:
+      x-mutating: true
+  /api/v1/opdb/describeClientConnectivity:
     post:
-      summary: Lists datalakes.
-      description: Lists datalakes.
-      operationId: listDatalakes
+      summary: Returns client connectivity details
+      description: Returns details to enable programmatic client connectivity for a database
+      operationId: describeClientConnectivity
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListDatalakesRequest'
+            $ref: '#/definitions/DescribeClientConnectivityRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListDatalakesResponse'
+            $ref: '#/definitions/DescribeClientConnectivityResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/deleteDatalake:
+      x-mutating: false
+  /api/v1/opdb/describeDatabase:
     post:
-      summary: Deletes a datalake.
-      description: Deletes a datalake.
-      operationId: deleteDatalake
+      summary: Describe a opDb
+      description: Details about the operational database
+      operationId: describeDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteDatalakeRequest'
+            $ref: '#/definitions/DescribeDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteDatalakeResponse'
+            $ref: '#/definitions/DescribeDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/describeDatalake:
+      x-mutating: false
+  /api/v1/opdb/describeUpgradeDatabase:
     post:
-      summary: Describes a datalake.
-      description: Describes a datalake.
-      operationId: describeDatalake
+      summary: Describes the upgrade availability.
+      description: Describes the upgrade availability for an operational database.
+      operationId: describeUpgradeDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeDatalakeRequest'
+            $ref: '#/definitions/DescribeUpgradeDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeDatalakeResponse'
+            $ref: '#/definitions/DescribeUpgradeDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/repairDatalake:
+      x-mutating: false
+  /api/v1/opdb/dropDatabase:
     post:
-      summary: Repairs a datalake.
-      description: Repairs a datalake.
-      operationId: repairDatalake
+      summary: drop a opDb
+      description: drop the operational database
+      operationId: dropDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RepairDatalakeRequest'
+            $ref: '#/definitions/DropDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RepairDatalakeResponse'
+            $ref: '#/definitions/DropDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getClusterServiceStatus:
+      x-mutating: true
+  /api/v1/opdb/listDatabases:
     post:
-      summary: Get cluster service status.
-      description: Gets the status of the services in a cluster.
-      operationId: getClusterServiceStatus
+      summary: List all opDbs in an environment
+      description: Fetch a list of all operational databases in an environment
+      operationId: listDatabases
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetClusterServiceStatusRequest'
+            $ref: '#/definitions/ListDatabasesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetClusterServiceStatusResponse'
+            $ref: '#/definitions/ListDatabasesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getClusterHostStatus:
+      x-mutating: false
+  /api/v1/opdb/listDiagnostics:
     post:
-      summary: Get cluster host status.
-      description: Gets the status of the hosts in a cluster.
-      operationId: getClusterHostStatus
+      summary: List all diagnostics associated to the database
+      description: returns list of diagnostics collections
+      operationId: listDiagnostics
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetClusterHostStatusRequest'
+            $ref: '#/definitions/ListDiagnosticsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetClusterHostStatusResponse'
+            $ref: '#/definitions/ListDiagnosticsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/upgradeDatalake:
+      x-mutating: false
+  /api/v1/opdb/listSupportedEnvironments:
     post:
-      summary: Upgrade cluster OS.
-      description: Upgrades the datalake cluster to the latest images.
-      operationId: upgradeDatalake
+      summary: List of environments available for the database creation
+      description: Fetches a list of environments available for the database creation
+      operationId: listSupportedEnvironments
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpgradeDatalakeRequest'
+            $ref: '#/definitions/ListSupportedEnvironmentsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpgradeDatalakeResponse'
+            $ref: '#/definitions/ListSupportedEnvironmentsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/checkDatalakeUpgradeOptions:
+      x-mutating: false
+  /api/v1/opdb/startDatabase:
     post:
-      summary: Check upgrade options.
-      description: Checks for upgrade options.
-      operationId: checkDatalakeUpgradeOptions
+      summary: Starts the database
+      description: Starts a previously stopped database
+      operationId: startDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CheckDatalakeUpgradeOptionsRequest'
+            $ref: '#/definitions/StartDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CheckDatalakeUpgradeOptionsResponse'
+            $ref: '#/definitions/StartDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/startDatalake:
+      x-mutating: true
+  /api/v1/opdb/stopDatabase:
     post:
-      summary: Start Datalake
-      description: Starts a stopped Datalake
-      operationId: startDatalake
+      summary: Stops the database
+      description: Stops a running database
+      operationId: stopDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StartDatalakeRequest'
+            $ref: '#/definitions/StopDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StartDatalakeResponse'
+            $ref: '#/definitions/StopDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/stopDatalake:
+      x-mutating: true
+  /api/v1/opdb/upgradeDatabase:
     post:
-      summary: Stop Datalake
-      description: Stops a running Datalake
-      operationId: stopDatalake
+      summary: Upgrades the database.
+      description: Upgrades an operational database in an environment to a given runtime.
+      operationId: upgradeDatabase
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StopDatalakeRequest'
+            $ref: '#/definitions/UpgradeDatabaseRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StopDatalakeResponse'
+            $ref: '#/definitions/UpgradeDatabaseResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+      x-mutating: true
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  ClouderaManagerDetails:
+  DiagnosticsBundle:
     type: object
-    description: Cloudera Manager details.
-    required:
-      - version
-      - clouderaManagerRepositoryURL
+    description: Describe a diagnostics bundle
     properties:
-      version:
+      id:
+        type: string
+        description: Identifier for each bundle collection
+      crn:
+        type: string
+        description: The object on which diagnostics was collected
+      startTime:
         type: string
-        description: Cloudera Manager version.
-      clouderaManagerRepositoryURL:
+        format: date-time
+        description: Start time
+      endTime:
         type: string
-        description: Cloudera Manager repository URL.
-      clouderaManagerServerURL:
+        format: date-time
+        description: The end time, if the command is finished.
+      status:
         type: string
-        description: Cloudera Manager server URL.
-  ProductVersion:
+        description: A status of the diagnostics collection process
+      result:
+        type: string
+        description: If this is a download, a link to the download location of the bundle
+  CollectDiagnosticsRequest:
     type: object
-    description: Product version.
+    description: Enables starting collection of the diagnostics. This is an asynchronous API and not expected to block.
     required:
-      - name
-      - version
+      - environmentName
+      - databaseName
+      - endTime
     properties:
-      name:
+      environmentName:
         type: string
-        description: The name of the product.
-      version:
+        description: The name of the environment
+      databaseName:
         type: string
-        description: The version of the product.
-  AWSConfiguration:
-    type: object
-    description: AWS configuration.
-    properties:
-      instanceProfile:
+        description: The name of the database
+      endTime:
+        type: string
+        description: The end time (in ISO 8601 format) of the period to collection statistics for.
+      startTime:
         type: string
-        description: The instance profile used for the ID Broker instance.
-  AzureConfiguration:
+        description: The start time (in ISO 8601 format) of the period to collection statistics for.
+  CollectDiagnosticsResponse:
     type: object
-    description: Azure configuration.
+    description: Information about diagnostic bundle generation
     properties:
-      managedIdentity:
-        type: string
-        description: The managed identity used for the ID Broker instance.
-  DatalakeDetails:
+      diagnosticsBundle:
+        description: Details of requested diagnostic bundle collection
+        $ref: '#/definitions/DiagnosticsBundle'
+  ListDiagnosticsRequest:
     type: object
-    description: Details about a datalake
+    description: Lists the in-progress diagnostic bundle operations.
     required:
-      - datalakeName
-      - crn
+      - environmentName
+      - databaseName
     properties:
-      crn:
-        type: string
-        description: The CRN of the datalake.
-      datalakeName:
-        type: string
-        description: The name of the datalake.
-      status:
-        type: string
-        description: The status of the datalake.
-      environmentCrn:
-        type: string
-        description: The CRN of the environment.
-      credentialCrn:
-        type: string
-        description: The CRN of credentials.
-      cloudPlatform:
+      environmentName:
         type: string
-        description: The cloud platform.
-      creationDate:
+        description: The name of the environment
+      databaseName:
         type: string
-        format: date-time
-        description: The date when the datalake was created.
-      clouderaManager:
-        $ref: '#/definitions/ClouderaManagerDetails'
-        description: The Cloudera Manager details.
-      productVersions:
+        description: The name of the database
+  ListDiagnosticsResponse:
+    type: object
+    description: The list of in-progress diagnostic bundle operations
+    properties:
+      diagnosticsBundles:
         type: array
         items:
-          $ref: '#/definitions/ProductVersion'
-        description: The product versions.
-      region:
-        type: string
-        description: The region of the datalake.
-      statusReason:
-        type: string
-        description: The reason for the status of the datalake.
-      awsConfiguration:
-        $ref: '#/definitions/AWSConfiguration'
-        description: The AWS configuration.
-      azureConfiguration:
-        $ref: '#/definitions/AzureConfiguration'
-        description: The Azure configuration.
-  Datalake:
+          $ref: '#/definitions/DiagnosticsBundle'
+        description: List of diagnostics operations
+  CreateDatabaseRequest:
     type: object
-    description: Information about a datalake.
+    description: A request to create the database
     required:
-      - datalakeName
-      - crn
+      - environmentName
+      - databaseName
     properties:
-      datalakeName:
-        type: string
-        description: The name of the datalake.
-      crn:
-        type: string
-        description: The CRN of the datalake.
-      status:
+      environmentName:
         type: string
-        description: The status of the datalake.
-      environmentCrn:
+        description: environment name
+      databaseName:
         type: string
-        description: The CRN of the environment.
-      creationDate:
-        type: string
-        format: date-time
-        description: The date when the datalake was created.
-      statusReason:
-        type: string
-        description: The reason for the status of the datalake.
-  DatalakeResourceTagRequest:
+        description: database name
+  CreateDatabaseResponse:
     type: object
-    description: Tag for a datalake resource.
+    description: A response which gives status of the database creation
     required:
-      - key
-      - value
+      - databaseDetails
     properties:
-      key:
-        type: string
-        description: The key of tag.
-      value:
-        type: string
-        description: The value of the tag.
-  AWSConfigurationRequest:
+      databaseDetails:
+        description: Details of the Database created
+        $ref: '#/definitions/DatabaseDetails'
+  DropDatabaseRequest:
     type: object
-    description: Request object for AWS configuration.
+    description: A request to drop the database
     required:
-      - instanceProfile
-      - storageBucketLocation
+      - environmentName
+      - databaseName
     properties:
-      instanceProfile:
+      environmentName:
         type: string
-        description: The ARN of an IAM instance profile.
-      storageBucketLocation:
+        description: environment name
+      databaseName:
         type: string
-        description: The location of the S3 bucket to be used as storage. The location has to start with s3a:// followed by the bucket name.
-  AzureConfigurationRequest:
+        description: database name
+  DropDatabaseResponse:
     type: object
-    description: Request object for Azure configuration.
-    required:
-      - managedIdentity
-      - storageLocation
+    description: A response which gives status of the database deletion
     properties:
-      managedIdentity:
-        type: string
-        description: The managed identity to use. The assumer should have Virtual Machine Contributor and Managed Identity Operator roles on subscription level.
-      storageLocation:
-        type: string
-        description: The storage location to use. The location has to be in the following format abfs://filesystem@storage-account-name.dfs.core.windows.net. The filesystem must already exist and the storage account must be StorageV2.
-  CreateAWSDatalakeRequest:
+      status:
+        description: status of delete database request
+        $ref: '#/definitions/StatusType'
+  ListSupportedEnvironmentsRequest:
+    type: object
+    description: A request to get a list of available environments
+  Environment:
     type: object
-    description: Request object for create AWS datalake request.
+    description: Details of the environment
     required:
-      - datalakeName
-      - environmentName
+      - crn
+      - name
     properties:
-      datalakeName:
+      crn:
         type: string
-        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
-        minLength: 5
-        maxLength: 100
-      environmentName:
+        description: The crn of the environment
+      name:
         type: string
-        description: The environment name or CRN.
-      cloudProviderConfiguration:
-        $ref: '#/definitions/AWSConfigurationRequest'
-        description: AWS configuration.
-      tags:
+        description: The name of the environment
+  ListSupportedEnvironmentsResponse:
+    type: object
+    description: A response which contains a list of available environments
+    properties:
+      environments:
         type: array
-        description: Tags to be added to Datalake related resources.
         items:
-          $ref: '#/definitions/DatalakeResourceTagRequest'
-      scale:
+          $ref: '#/definitions/Environment'
+        description: The crn of the environment
+  StatusType:
+    type: string
+    description: status of the database
+    enum:
+      - REQUESTED
+      - CREATE_IN_PROGRESS
+      - AVAILABLE
+      - UPDATE_IN_PROGRESS
+      - UPDATE_REQUESTED
+      - UPDATE_FAILED
+      - CREATE_FAILED
+      - ENABLE_SECURITY_FAILED
+      - PRE_DELETE_IN_PROGRESS
+      - DELETE_IN_PROGRESS
+      - DELETE_FAILED
+      - DELETE_COMPLETED
+      - STOPPED
+      - STOP_REQUESTED
+      - START_REQUESTED
+      - STOP_IN_PROGRESS
+      - START_IN_PROGRESS
+      - START_FAILED
+      - STOP_FAILED
+      - WAIT_FOR_SYNC
+      - MAINTENANCE_MODE_ENABLED
+      - REQUESTING
+      - MISSING
+      - BACKUP_IN_PROGRESS
+      - BACKUP_FAILED
+      - BACKUP_FINISHED
+      - RESTORE_IN_PROGRESS
+      - RESTORE_FAILED
+      - RESTORE_FINISHED
+      - DELETED_ON_PROVIDER_SIDE
+      - AMBIGUOUS
+      - EXTERNAL_DATABASE_CREATION_IN_PROGRESS
+      - EXTERNAL_DATABASE_CREATION_FAILED
+      - EXTERNAL_DATABASE_DELETION_IN_PROGRESS
+      - EXTERNAL_DATABASE_DELETION_FINISHED
+      - EXTERNAL_DATABASE_DELETION_FAILED
+      - UNKNOWN
+      - EXTERNAL_DATABASE_START_IN_PROGRESS
+      - EXTERNAL_DATABASE_START_FINISHED
+      - EXTERNAL_DATABASE_START_FAILED
+      - EXTERNAL_DATABASE_STOP_IN_PROGRESS
+      - EXTERNAL_DATABASE_STOP_FINISHED
+      - EXTERNAL_DATABASE_STOP_FAILED
+      - LOAD_BALANCER_UPDATE_IN_PROGRESS
+      - LOAD_BALANCER_UPDATE_FINISHED
+      - LOAD_BALANCER_UPDATE_FAILED
+      - UNREACHABLE
+      - NODE_FAILURE
+      - RECOVERY_IN_PROGRESS
+      - RECOVERY_REQUESTED
+      - RECOVERY_FAILED
+  ListDatabasesRequest:
+    type: object
+    description: A request to list databases
+    properties:
+      environmentName:
         type: string
-        description: The scale of the datalake.
-  CreateAWSDatalakeResponse:
+        description: name of the environment
+  ListDatabasesResponse:
     type: object
-    description: Response object for create AWS datalake request.
+    description: A list of databases in response
     required:
-      - datalake
+      - databases
     properties:
-      datalake:
-        $ref: '#/definitions/Datalake'
-        description: The datalake.
-  CreateAzureDatalakeRequest:
+      databases:
+        type: array
+        items:
+          $ref: '#/definitions/DatabaseDetails'
+        description: The details of the database
+  DatabaseDetails:
     type: object
-    description: Request object for create Azure datalake request.
+    description: Details of the databases.
     required:
-      - datalakeName
-      - environmentName
+      - databaseName
+      - environmentCrn
+      - crn
+      - creationDate
     properties:
-      datalakeName:
+      databaseName:
         type: string
-        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
-        minLength: 5
-        maxLength: 100
+        description: The name of the database.
+      environmentCrn:
+        type: string
+        description: environment crn
+      crn:
+        type: string
+        description: database crn
+      creationDate:
+        type: string
+        format: date-time
+        description: The creation time of the database
+      status:
+        description: Status of the database creation
+        $ref: '#/definitions/StatusType'
+      creatorCrn:
+        type: string
+        description: Crn of the creator
+      dbVersion:
+        type: string
+        description: Database version
+      hueEndpoint:
+        type: string
+        description: Hue endpoint
       environmentName:
         type: string
-        description: The environment name or CRN.
-      cloudProviderConfiguration:
-        $ref: '#/definitions/AzureConfigurationRequest'
-        description: Azure configuration.
-      tags:
-        type: array
-        description: Tags to be added to Datalake related resources.
-        items:
-          $ref: '#/definitions/DatalakeResourceTagRequest'
-      scale:
+        description: Environment name
+      storageLocation:
+        type: string
+        description: HBase cloud storage location
+      internalName:
         type: string
-        description: The scale of the datalake.
-  CreateAzureDatalakeResponse:
+        description: Internal cluster name for this database
+  DescribeDatabaseRequest:
     type: object
-    description: Response object for create Azure datalake request.
+    description: request to get details of the database in a particular environment
     required:
-      - datalake
-    properties:
-      datalake:
-        $ref: '#/definitions/Datalake'
-        description: The datalake.
-  ListDatalakesRequest:
-    type: object
-    description: Request object for list datalakes request.
+      - environmentName
+      - databaseName
     properties:
       environmentName:
         type: string
-        description: The name or CRN of the environment for which the datalakes will be listed.
-      datalakeName:
+        description: The name of the environment.
+      databaseName:
         type: string
-        description: The name or CRN of the datalake for which details are requested.
-  ListDatalakesResponse:
+        description: The name of the database.
+  DescribeDatabaseResponse:
     type: object
-    description: Response object for list datalakes request.
-    required:
-      - datalakes
+    description: Details of the database.
     properties:
-      datalakes:
-        type: array
-        items:
-          $ref: '#/definitions/Datalake'
-        description: The datalakes.
-  DeleteDatalakeRequest:
+      databaseDetails:
+        description: The details of the database.
+        $ref: '#/definitions/DatabaseDetails'
+  StartDatabaseRequest:
     type: object
-    description: Request object for delete datalake request.
+    description: Start the database.
     required:
-      - datalakeName
+      - environmentName
+      - databaseName
     properties:
-      datalakeName:
+      environmentName:
         type: string
-        description: The name or CRN of the datalake to be deleted.
-      force:
-        type: boolean
-        description: Whether the datalake should be force deleted. This option can be used when cluster deletion fails. This removes the entry from Cloudera Datalake service. Any lingering resources have to be deleted from the cloud provider manually. The default is false.
-  DeleteDatalakeResponse:
+        description: The name of the environment
+      databaseName:
+        type: string
+        description: The name of the database.
+  StartDatabaseResponse:
     type: object
-    description: Response object for delete datalake request.
-  DescribeDatalakeRequest:
+    description: A response from starting the database.
+    properties:
+      wasStarted:
+        type: boolean
+        description: True if the database start request accepted
+      previousStatus:
+        description: The status of the database prior to the start request.
+        $ref: '#/definitions/StatusType'
+  StopDatabaseRequest:
     type: object
-    description: Request object for describe datalake request.
+    description: Stop the database.
     required:
-      - datalakeName
+      - environmentName
+      - databaseName
     properties:
-      datalakeName:
+      environmentName:
+        type: string
+        description: The name of the environment
+      databaseName:
         type: string
-        description: The name or CRN of the datalake.
-  DescribeDatalakeResponse:
+        description: The name of the database.
+  StopDatabaseResponse:
     type: object
-    description: Response object for describe datalake request.
-    required:
-      - datalake
+    description: A response from stopping the database.
     properties:
-      datalake:
-        $ref: '#/definitions/DatalakeDetails'
-        description: The datalake.
-  RepairDatalakeRequest:
+      wasStopped:
+        type: boolean
+        description: True if the database stop request accepted
+      previousStatus:
+        description: The status of the database prior to the stop request.
+        $ref: '#/definitions/StatusType'
+  DescribeClientConnectivityRequest:
     type: object
-    description: Request object for repair datalake request.
+    description: A request for client API connectivity to a database.
     required:
-      - datalakeName
-      - instanceGroupName
+      - environmentName
+      - databaseName
     properties:
-      datalakeName:
+      environmentName:
         type: string
-        description: The name or CRN of the datalake.
-      instanceGroupName:
+        description: The name of the environment
+      databaseName:
         type: string
-        description: The instance group where the failed instances will be repaired.
-  RepairDatalakeResponse:
-    type: object
-    description: Response object for repair datalake request.
-  GetClusterServiceStatusRequest:
+        description: The name of the database
+  KerberosConfiguration:
     type: object
-    description: Request object to get service status.
-    required:
-      - clusterName
+    description: Configuration information to enable Kerberos authentication
     properties:
-      clusterName:
+      kdcHost:
+        type: string
+        description: The hostname of the KDC
+      realm:
         type: string
-        description: The name or CRN of the cluster.
-  GetClusterServiceStatusResponse:
+        description: The Kerberos realm
+      krb5Conf:
+        type: string
+        description: A base64-encoded krb5.conf file
+  Kind:
+    type: string
+    description: "A categorization of a connector to describe how it is broadly used.\n `LIBRARY` - A client library or API which user's code invokes `JDBC` - A JDBC driver `SERVICE` - A Service URL `ENVIRONMENT` - An environment to use to run other commands and tools `ODBC` - An ODBC driver"
+    enum:
+      - LIBRARY
+      - JDBC
+      - SERVICE
+      - ENVIRONMENT
+  DependencyManagement:
     type: object
-    description: Response object to get service status.
-    required:
-      - services
+    description: Information about dependencies necessary to use a connector.
     properties:
-      services:
-        type: array
-        items:
-          $ref: '#/definitions/ServiceStatus'
-        description: The cluster services health.
-  ServiceStatus:
+      mavenUrl:
+        type: string
+        description: The URL of a Maven repository containing the client JARs.
+  ClientConfigurationDetails:
     type: object
-    description: Information about a cluster service.
+    description: A URL which holds information necessary to configure a Connector.
     properties:
-      type:
-        type: string
-        description: The service type.
-      state:
+      name:
         type: string
-        description: The service state.
-      healthSummary:
+        description: The name of this configuration
+      url:
         type: string
-        description: The service health summary.
-      healthChecks:
-        type: array
-        items:
-          $ref: '#/definitions/HealthCheck'
-        description: The service health checks.
-  HealthCheck:
+        description: The URL from which to fetch the configuration
+  ConnectorConfiguration:
     type: object
-    description: The result of a health check.
+    description: Runtime details necessary to use a connector.
     properties:
-      name:
+      clientConfigurationDetails:
+        type: array
+        items:
+          $ref: '#/definitions/ClientConfigurationDetails'
+        description: Configuration information required to use a Connector
+      jdbcUrl:
         type: string
-        description: The name of service health check.
-      summary:
+        description: A base JDBC URL if the connector is a JDBC driver.
+      serviceUrl:
         type: string
-        description: The service health check summary.
-  GetClusterHostStatusRequest:
+        description: A base service URL
+  Connector:
     type: object
-    description: Request object to get host status.
-    required:
-      - clusterName
+    description: Information to use to connect to a database via some mechanism.
     properties:
-      clusterName:
+      name:
         type: string
-        description: The name or CRN of the cluster.
-  GetClusterHostStatusResponse:
+        description: The name of the API/Library this connector represents.
+      version:
+        type: string
+        description: The version of the connector.
+      kind:
+        description: A categorization of this connector.
+        $ref: '#/definitions/Kind'
+      dependencies:
+        description: Software dependency information necessary to use the connector.
+        $ref: '#/definitions/DependencyManagement'
+      configuration:
+        description: Runtime details required to use the connector.
+        $ref: '#/definitions/ConnectorConfiguration'
+      requiresKerberos:
+        type: boolean
+        description: True if the connector requires Kerberos to authenticate.
+  DescribeClientConnectivityResponse:
     type: object
-    description: Response object for getting host status.
-    required:
-      - hosts
+    description: A response with client API connectivity to a database.
     properties:
-      hosts:
+      connectors:
         type: array
         items:
-          $ref: '#/definitions/HostStatus'
-        description: The cluster hosts status.
-  HostStatus:
+          $ref: '#/definitions/Connector'
+        description: Available connectors for this database
+      kerberosConfiguration:
+        description: Kerberos configuration information
+        $ref: '#/definitions/KerberosConfiguration'
+  UpgradeDatabaseRequest:
     type: object
-    description: Information about cluster host status.
+    description: Asynchronous request to upgrade the CDP Runtime for a database.
     properties:
-      hostid:
+      environment:
         type: string
-        description: Unique identifier of the cluster host given by Cloudera Manager.
-      hostname:
+        description: The name or CRN of the environment.
+      database:
         type: string
-        description: The cluster hostname.
-      healthSummary:
+        description: The name or CRN of the database.
+      runtime:
         type: string
-        description: The host health summary.
-  UpgradeDatalakeRequest:
+        description: The CDP Runtime version to upgrade to.
+      osUpgradeOnly:
+        type: boolean
+        description: Only perform an Operating System upgrade.
+  UpgradeDatabaseResponse:
     type: object
-    description: Request object to upgrade datalake.
-    required:
-      - datalakeName
+    description: Response with the reason whether upgrade request is accepted or why it is not possible.
     properties:
-      datalakeName:
+      statusReason:
         type: string
-        description: The name or CRN of the datalake.
-  UpgradeDatalakeResponse:
-    type: object
-    description: Response object for upgrade datalake request.
-  CheckDatalakeUpgradeOptionsRequest:
+        description: The reason whether upgrade request is accepted or why it is not possible.
+  DescribeUpgradeDatabaseRequest:
     type: object
-    description: Request object to check datalake upgrade options.
+    description: Request to describe the upgrade availability of CDP Runtime and Operating System for a database.
     required:
-      - datalakeName
+      - environment
+      - database
     properties:
-      datalakeName:
+      environment:
         type: string
-        description: The name or CRN of the datalake.
-  CheckDatalakeUpgradeOptionsResponse:
-    type: object
-    description: Response object to check datalake upgrade options.
-    required:
-      - current
-    properties:
-      current:
-        $ref: '#/definitions/ImageInfo'
-        description: Details of the image, that datalake is currently uses.
-      upgrade:
-        $ref: '#/definitions/ImageInfo'
-        description: Details of the image, that datalake can be upgraded to.
-  StartDatalakeRequest:
-    type: object
-    description: Request object to start a datalake.
-    required:
-      - datalakeName
-    properties:
-      datalakeName:
+        description: The name or CRN of the environment.
+      database:
         type: string
-        description: The name or CRN of the datalake.
-  StartDatalakeResponse:
+        description: The name or CRN of the database.
+  DescribeUpgradeDatabaseResponse:
     type: object
-    description: Response object of starting a datalake.
-  StopDatalakeRequest:
-    type: object
-    description: Request object to stop a datalake.
-    required:
-      - datalakeName
+    description: Response with upgrade availability of CDP Runtime and Operating System for a database.
     properties:
-      datalakeName:
+      statusReason:
         type: string
-        description: The name or CRN of the datalakeName.
-  StopDatalakeResponse:
-    type: object
-    description: Response object of stopping a datalake.
-  ImageInfo:
+        description: The reason whether upgrade request is accepted or why it is not possible.
+      currentComponentVersion:
+        description: Versions of currently deployed CDP runtime and operating system.
+        $ref: '#/definitions/ComponentsVersion'
+      availableComponentVersions:
+        type: array
+        items:
+          $ref: '#/definitions/ComponentsVersion'
+        description: List of available versions for upgrade.
+      isOSUpgradeAvailable:
+        type: boolean
+        description: Is an OS upgrade available.
+      isRuntimeUpgradeAvailable:
+        type: boolean
+        description: Is a CDP Runtime upgrade available.
+  ComponentsVersion:
     type: object
-    description: Basic information about an image.
+    description: Versions of the CDP runtime and Operating system components.
     properties:
-      imageName:
+      cm:
+        type: string
+        description: Version of Cloudera Manager.
+      cdp:
         type: string
-        description: The name of the image.
-      imageId:
+        description: CDP Runtime version.
+      os:
         type: string
-        description: The id of the image.
-      imageCatalogName:
+        description: Operation System name and version.
+      osPatchLevel:
         type: string
-        description: Name of the image catalog, the image is from.
-      created:
-        type: integer
-        format: int64
-        description: Image creation timestamp
+        description: Operation System patch level.
+x-audit: true
```

### Comparing `cdpcli-0.9.9/cdpcli/data/ml/ml.yaml` & `cdpcli-0.9.90/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,221 +1,212 @@
-x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: ml
+x-endpoint-name: replicationmanager
 x-products: CDP
+x-form-factors: public
 x-cdp-releases: PUBLIC
+x-audit: true
 info:
-  version: 0.1-SNAPSHOT
-  title: Cloudera Machine Learning
+  version: 0.9.90
+  title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
-  description: Install and manage Cloudera Machine Learning applications.
+  description: Create and manage replication policies using Cloudera Replication Manager.
+  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/ml/createWorkspace:
+  /api/v1/replicationmanager/listClusters:
     post:
-      summary: Create a Cloudera Machine Learning workspace.
-      description: Provision a Kubernetes cluster and install the Cloudera Machine Learning application in it.
-      operationId: createWorkspace
+      summary: Lists all clusters.
+      description: Provides a detailed list of all available clusters.
+      operationId: listClusters
+      x-mutating: false
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateWorkspaceRequest'
+            $ref: '#/definitions/ListClustersRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/CreateWorkspaceResponse'
+            $ref: '#/definitions/ListClustersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/deleteWorkspace:
+  /api/v1/replicationmanager/listClusterServiceStatuses:
     post:
-      summary: Delete Cloudera Machine Learning Workspace.
-      description: Deletes a Cloudera Machine Learning workspace.
-      operationId: deleteWorkspace
+      summary: Lists Cluster Service Statuses.
+      description: Provides a list of cluster service (e.g. HDFS, Hive, YARN, etc.) statuses.
+      operationId: listClusterServiceStatuses
+      x-mutating: false
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteWorkspaceRequest'
+            $ref: '#/definitions/ListClusterServiceStatusesRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteWorkspaceResponse'
+            $ref: '#/definitions/ListClusterServiceStatusesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/describeWorkspace:
+  /api/v1/replicationmanager/listAllCredentials:
     post:
-      summary: Describe Cloudera Machine Learning Workspace.
-      description: Describes a Cloudera Machine Learning workspace.
-      operationId: describeWorkspace
+      summary: Lists Cloud Credentials.
+      description: Provides a detailed list of cloud credentials across all available clusters.
+      operationId: listAllCredentials
+      x-mutating: false
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeWorkspaceRequest'
+            $ref: '#/definitions/ListAllCredentialsRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeWorkspaceResponse'
+            $ref: '#/definitions/ListAllCredentialsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/getAuditEvents:
+  /api/v1/replicationmanager/getCredentials:
     post:
-      summary: Gets all the events belong to a workspace crn.
-      description: Gets all the events belong to a workspace crn.
-      operationId: getAuditEvents
+      summary: Get Cloud Credentials from a Cluster.
+      description: Returns cloud credentials on a specific cluster.
+      operationId: getCredentials
+      x-mutating: false
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetAuditEventsRequest'
+            $ref: '#/definitions/GetCredentialsRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/GetAuditEventsResponse'
+            $ref: '#/definitions/GetCredentialsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/getLatestWorkspaceVersion:
+  /api/v1/replicationmanager/listPolicies:
     post:
-      summary: GetLatestWorkspaceVersion Cloudera Machine Learning Workspace.
-      description: Retrieves the latest version that Cloudera Machine Learning deploys to workspaces.
-      operationId: getLatestWorkspaceVersion
+      summary: Get All Replication Policies.
+      description: Provides a list of all replication policies across all available clusters.
+      operationId: listPolicies
+      x-mutating: false
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetLatestWorkspaceVersionRequest'
+            $ref: '#/definitions/ListPoliciesRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/GetLatestWorkspaceVersionResponse'
+            $ref: '#/definitions/ListPoliciesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/getLogs:
+  /api/v1/replicationmanager/deletePolicy:
     post:
-      summary: Gets all the logs belong to a request id.
-      description: Gets all the logs belong to a request id.
-      operationId: getLogs
+      summary: Delete Replication Policy.
+      description: Permanently deletes a specific replication policy.
+      operationId: deletePolicy
+      x-mutating: true
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetLogsRequest'
+            $ref: '#/definitions/DeletePolicyRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/GetLogsResponse'
+            $ref: '#/definitions/DeletePolicyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/grantWorkspaceAccess:
+  /api/v1/replicationmanager/createPolicy:
     post:
-      summary: GrantWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Grants an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: grantWorkspaceAccess
+      summary: Create a Replication Policy.
+      description: Creates a new replication policy with the given name on a specific cluster.
+      operationId: createPolicy
+      x-mutating: true
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GrantWorkspaceAccessRequest'
+            $ref: '#/definitions/CreatePolicyRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/GrantWorkspaceAccessResponse'
+            $ref: '#/definitions/CreatePolicyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/listWorkspaces:
+  /api/v1/replicationmanager/suspendPolicy:
     post:
-      summary: List Cloudera Machine Learning workspaces.
-      description: List Cloudera Machine Learning workspaces.
-      operationId: listWorkspaces
+      summary: Stop all replication tasks defined by the policy.
+      description: Stops all replication tasks defined by the policy. Replication will resume after activating the policy.
+      operationId: suspendPolicy
+      x-mutating: true
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListWorkspacesRequest'
+            $ref: '#/definitions/SuspendPolicyRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/ListWorkspacesResponse'
+            $ref: '#/definitions/SuspendPolicyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/ml/revokeWorkspaceAccess:
+  /api/v1/replicationmanager/activatePolicy:
     post:
-      summary: RevokeWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Revokes an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: revokeWorkspaceAccess
+      summary: Resume all replication tasks defined by the policy.
+      description: Resumes all replication tasks defined by the policy if the policy is currently suspended.
+      operationId: activatePolicy
+      x-mutating: true
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RevokeWorkspaceAccessRequest'
+            $ref: '#/definitions/ActivatePolicyRequest'
       responses:
         200:
-          description: Expected response to a valid request.
+          description: Describes a successful response to a valid request.
           schema:
-            $ref: '#/definitions/RevokeWorkspaceAccessResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /api/v1/ml/upgradeWorkspace:
-    post:
-      summary: Upgrade Cloudera Machine Learning workspace.
-      description: Upgrades a Cloudera Machine Learning workspace to the latest available version.
-      operationId: upgradeWorkspace
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/UpgradeWorkspaceRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/UpgradeWorkspaceResponse'
+            $ref: '#/definitions/ActivatePolicyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
@@ -223,662 +214,875 @@
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  RootVolume:
+  ListClustersRequest:
     type: object
-    description: Configuration for instance root device volume
+    description: Request to list clusters.
+  ListClustersResponse:
+    type: object
+    description: Response object for list clusters request.
     required:
-      - size
+      - unreachableClusters
+      - clusters
     properties:
-      size:
-        type: integer
-        format: int64
-        description: The volume size in GB.
-  GetLogsRequest:
+      unreachableClusters:
+        description: List of errors for unreachable clusters.
+        type: array
+        items:
+          $ref: '#/definitions/ApiError'
+      clusters:
+        type: array
+        description: List of clusters.
+        items:
+          $ref: '#/definitions/Cluster'
+  ListClusterServiceStatusesRequest:
+    type: object
+    description: Request object to list cluster statuses.
+  ListClusterServiceStatusesResponse:
+    type: object
+    description: Response object for listing of cluster statuses.
+    properties:
+      statuses:
+        type: array
+        description: List of statuses by cluster.
+        items:
+          $ref: '#/definitions/ClusterServiceStatuses'
+  ListAllCredentialsRequest:
+    type: object
+    description: Request object for listing all cloud credentials on all clusters.
+  ListAllCredentialsResponse:
+    type: object
+    description: Response object for list credentials request.
+    required:
+      - unreachableClusters
+      - credentials
+    properties:
+      unreachableClusters:
+        description: List of errors for unreachable clusters.
+        type: array
+        items:
+          $ref: '#/definitions/ApiError'
+      credentials:
+        description: List of credentials by cluster.
+        type: array
+        items:
+          $ref: '#/definitions/CredentialsResponse'
+  GetCredentialsRequest:
     type: object
-    description: GetLogsRequestfor getting logs for a request ID.
+    description: Request object to retrieve specific cloud credentials.
     required:
-      - workspaceCrn
-      - requestID
+      - clusterCrn
     properties:
-      workspaceCrn:
+      clusterCrn:
+        description: CRN of the cluster where the credential is.
         type: string
-        description: WorkspaceCrn the requestID belongs to.
-      requestID:
+      credentialName:
+        description: Name of the credential. If both name and Id are specified, the Id is considered.
         type: string
-        description: Unique Key to identify a set of logs.
-      fetchAll:
-        type: boolean
-        description: Flag to fetch all logs.
-      pageSize:
-        type: integer
-        format: int32
-        description: Limit the number of logs.
-      offset:
-        type: integer
-        format: int32
-        description: offset from which the logs should be fetched.
-  GetLogsResponse:
+      credentialId:
+        description: Id of the credential. If both name and Id are specified, the Id is considered.
+        type: string
+  GetCredentialsResponse:
     type: object
-    description: GetLogsResponse contains all the logs for a given request id.
-    required:
-      - auditLogs
+    description: Response for credential request.
     properties:
-      auditLogs:
-        description: Contains all the logs for a given request id.
-        $ref: '#/definitions/AuditLogs'
-  AuditLogs:
+      credentials:
+        type: array
+        description: List of credentials.
+        items:
+          $ref: '#/definitions/CredentialDetails'
+  ListPoliciesRequest:
     type: object
-    description: AuditLogs contains all the logs for a given request id.
+    description: Request object for listing all policies.
+  ListPoliciesResponse:
+    type: object
+    description: Response object for a list policies request.
     required:
-      - requestID
-      - count
-      - logs
+      - unreachableClusters
+      - policyErrors
+      - policies
     properties:
-      requestID:
-        type: string
-        description: The request ID associated with a long-running operation to fetch the logs for.
-      count:
-        type: integer
-        format: int32
-        description: Total number of logs associated with the request id.
-      logs:
+      unreachableClusters:
+        description: List of errors for unreachable clusters.
+        type: array
+        items:
+          $ref: '#/definitions/ApiError'
+      policyErrors:
+        description: List of policy errors.
+        type: array
+        items:
+          $ref: '#/definitions/ApiError'
+      policies:
+        description: List of policies.
         type: array
         items:
-          $ref: '#/definitions/AuditLog'
-        description: Contains all the logs for a given request id.
-  AuditLog:
+          $ref: '#/definitions/Policy'
+  DeletePolicyRequest:
     type: object
-    description: Audit log represents an individual log.
+    description: Delete a replication policy.
     required:
-      - createdDate
-      - log
+      - clusterCrn
+      - policyName
     properties:
-      createdDate:
+      clusterCrn:
         type: string
-        format: date-time
-        description: Time at which the log is created.
-      log:
+        description: CRN of the cluster where the policy is.
+      policyName:
         type: string
-        description: Log description.
-  GetAuditEventsRequest:
+        description: Policy name to delete.
+  DeletePolicyResponse:
+    type: object
+    description: Response object for deletePolicy.
+  CreatePolicyRequest:
     type: object
-    description: GetAuditEventsRequest to get all audit events for a given workspace crn.
+    description: Create a replication policy.
     required:
-      - workspaceCrn
+      - clusterCrn
+      - policyName
+      - policyDefinition
     properties:
-      workspaceCrn:
+      clusterCrn:
         type: string
-        description: Workspace crn for which audit events to be fetched.
-  GetAuditEventsResponse:
+        description: CRN of the cluster where the policy will be created.
+      policyName:
+        type: string
+        description: Name of the new policy.
+      policyDefinition:
+        description: Policy definition.
+        $ref: '#/definitions/PolicyDefinition'
+  CreatePolicyResponse:
+    type: object
+    description: Response object for createPolicy.
+  SuspendPolicyRequest:
     type: object
-    description: GetAuditEventsResponse containes all the audit events for a given workspace crn.
+    description: Suspend a replication policy.
     required:
-      - auditEvents
+      - clusterCrn
+      - policyName
     properties:
-      auditEvents:
-        description: Contains all the audit events for a given workspace crn.
-        $ref: '#/definitions/AuditEvents'
-  AuditEvents:
+      clusterCrn:
+        type: string
+        description: CRN of the cluster where the policy is.
+      policyName:
+        type: string
+        description: Policy name to suspend.
+  SuspendPolicyResponse:
     type: object
-    description: AuditEvents contains all the audit events for a given workspace crn.
+    description: Response object for suspendPolicy.
+  ActivatePolicyRequest:
+    type: object
+    description: Activate a replication policy.
     required:
-      - workspaceCrn
-      - events
+      - clusterCrn
+      - policyName
     properties:
-      workspaceCrn:
+      clusterCrn:
         type: string
-        description: Workspace crn unique for the set of audit events.
-      events:
-        type: array
-        items:
-          $ref: '#/definitions/AuditEvent'
-        description: AuditEvent belong to the workspace crn.
-  AuditEvent:
+        description: CRN of the cluster where the policy is.
+      policyName:
+        type: string
+        description: Policy name to resume.
+  ActivatePolicyResponse:
     type: object
-    description: Audit event descibes an performed or performing in a given workspace.
+    description: Response object for resumePolicy.
+  ApiError:
+    type: object
+    description: API error.
     required:
-      - workspaceCrn
-      - userCrn
-      - requestID
-      - action
-      - createdDate
+      - code
+      - message
+      - status
     properties:
-      workspaceCrn:
-        type: string
-        description: Workspace crn where the event observed.
-      userCrn:
+      code:
+        type: integer
+        format: int32
+        description: Error code.
+      message:
+        description: Error message.
         type: string
-        description: UserCrn to track which user has caused the event.
-      requestID:
+      status:
+        description: Error status.
         type: string
-        description: Unique request ID to keep track of event.
-      action:
+      clusterUrl:
         type: string
-        description: Action the user has generated.
-      createdDate:
+        description: Cluster URL.
+      requestId:
+        description: Request ID.
         type: string
-        format: date-time
-        description: Time at creation of event.
-  Autoscaling:
+  ClusterServiceStatuses:
     type: object
-    description: Configuration for instance auto scaling.
+    description: Describes the status of services running on a cluster.
     required:
-      - minInstances
-      - maxInstances
+      - clusterCrn
+      - serviceStatuses
     properties:
-      minInstances:
-        type: integer
-        format: int32
-        description: The minimum number of instance for auto scaling.
-      maxInstances:
-        type: integer
-        format: int32
-        description: The maximum number of instance for auto scaling.
-      enabled:
-        type: boolean
-        description: The boolean flag to enable the auto scaling.
-  InstanceGroup:
+      clusterCrn:
+        description: Cluster CRN.
+        type: string
+      serviceStatuses:
+        description: List of service statuses.
+        type: array
+        items:
+          $ref: '#/definitions/ServiceInfo'
+  Cluster:
     type: object
-    description: Contains the necessary info for an instance group.
+    description: Describes a Datalake, Datahub or Classic cluster.
     required:
-      - instanceType
+      - crn
+      - name
+      - dataCenter
+      - clusterType
+      - replicationEngineType
+      - clusterManagerType
+      - clusterManagerUrl
+      - clusterUrl
     properties:
-      instanceType:
-        type: string
-        description: The cloud provider instance type for the node instance.
-      instanceTier:
+      crn:
+        description: Cluster CRN.
         type: string
-        description: The tier of the instance i.e. on-demand/spot.
-      instanceCount:
-        type: integer
-        format: int32
-        description: The initial number of instance node.
       name:
+        description: Cluster name.
         type: string
-        description: The unique name of the instance group.
-      ingressRules:
-        type: array
-        items:
-          type: string
-        description: The networking rules for the ingress.
-      rootVolume:
-        description: The root volume of the instance.
-        $ref: '#/definitions/RootVolume'
-      autoscaling:
-        description: The auto scaling configuration.
-        $ref: '#/definitions/Autoscaling'
-  WorkspaceInstanceGroup:
-    type: object
-    description: Instance group information to show in workspace details.
-    required:
-      - instanceType
-      - instanceCount
-      - instanceGroupName
-      - minInstances
-      - maxInstances
-      - instances
-      - tags
-    properties:
-      instanceType:
+      dataCenter:
+        description: Cluster data center.
         type: string
-        description: The cloud provider instance type for the node instance.
-      instanceCount:
-        type: integer
-        format: int32
-        description: The initial number of instance node.
-      instanceGroupName:
+      clusterType:
+        description: Cluster type.
         type: string
-        description: The unique name of the instance group.
-      minInstances:
-        type: integer
-        format: int32
-        description: The minimum number of instances that can be deployed to this instance group. If the value is 0, the group might be empty.
-      maxInstances:
+        enum:
+          - CLASSIC
+          - SDX
+          - DISTROX
+      replicationEngineType:
+        description: Replication engine type.
+        type: string
+        enum:
+          - CM
+          - DLM_ENGINE
+      clusterManagerType:
+        description: Cluster Manager type.
+        type: string
+        enum:
+          - CLOUDERA_MANAGER
+          - AMBARI
+      clusterManagerUrl:
+        description: Cluster Manager URL.
+        type: string
+      clusterUrl:
+        description: Cluster URL.
+        type: string
+      totalHosts:
+        description: Total hosts on the cluster.
         type: integer
         format: int32
-        description: The maximum number of instances that can be deployed to this instance group.
-      instances:
-        type: array
-        items:
-          $ref: '#/definitions/Instance'
-        description: Instances in the instance group.
-      tags:
-        type: array
-        items:
-          $ref: '#/definitions/Tag'
-        description: Tags are key/value pairs that are applied to all tag-able resources deployed in the workspace's cloud environment.
-  Instance:
-    type: object
-    description: Represents each instance in an instance group.
-    required:
-      - instanceId
-      - availabilityZone
+      location:
+        description: Cluster location.
+        $ref: '#/definitions/Location'
+      stackCrn:
+        description: Stack CRN.
+        type: string
+      description:
+        description: Cluster description.
+        type: string
+      stackMajorVersion:
+        description: Stack major version.
+        type: string
+      stackVersion:
+        description: Stack version.
+        type: string
+      uuid:
+        description: Cluster UUID from Cloudera Manager if the cluster has CM backend.
+        type: string
+      environmentCrn:
+        description: CRN of the cluster's environment.
+        type: string
+      knoxUrl:
+        description: Knox URL if the cluster was registered with one, null otherwise.
+        type: string
+      cloudAccountProvider:
+        description: Cloud account provider.
+        type: string
+        enum:
+          - AWS
+          - ADLS
+          - WASB
+          - ABFS
+          - GCS
+      cmName:
+        description: Cloudera Manager name.
+        type: string
+      codProperties:
+        description: Additional properties for operational databases.
+        $ref: '#/definitions/CodProperties'
+  Location:
+    type: object
+    description: Location object.
+    required:
+      - id
+      - country
+      - city
+      - latitude
+      - longitude
     properties:
-      instanceId:
+      id:
+        description: Location ID.
+        type: integer
+        format: int64
+      country:
+        description: Country.
         type: string
-        description: Unique instance Id generated by the cloud provider.
-      availabilityZone:
+      city:
+        description: City.
         type: string
-        description: Availability zone the instance belongs to.
-  Tag:
+      latitude:
+        description: Latitude.
+        type: number
+        format: double
+      longitude:
+        description: Longitude.
+        type: number
+        format: double
+  CodProperties:
     type: object
-    description: Contains a single tag entry associated with a workspace.
-    required:
-      - key
-      - value
+    description: Additional properties for operational databases.
     properties:
-      key:
-        type: string
-        description: The name for the tag.
-      value:
+      operationalDatabaseName:
+        description: Name of the corresponding operational database..
         type: string
-        description: The value for the tag.
-  ProvisionTag:
+  CustomConfigs:
     type: object
-    description: Contains a single tag entry that will be configured on cloud resources associated with a workspace.
+    description: Custom key/value configurations.
     required:
-      - key
+      - name
       - value
+      - confidential
     properties:
-      key:
+      name:
+        description: Name.
         type: string
-        description: The name for the tag.
       value:
+        description: Value.
         type: string
-        description: The value for the tag.
-  ProvisionK8sRequest:
-    type: object
-    description: Request object for workspace provision.
-    required:
-      - instanceGroups
-      - environmentName
-    properties:
-      instanceGroups:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroup'
-        description: The instance groups.
-      environmentName:
-        type: string
-        description: The environment for the workspace to create.
-      tags:
-        type: array
-        items:
-          $ref: '#/definitions/ProvisionTag'
-        description: Tags to add to the cloud provider resources created. This is in addition to any tags added by Cloudera.
-  CreateWorkspaceRequest:
+      confidential:
+        description: Whether the value is confidential.
+        type: boolean
+  CredentialsResponse:
     type: object
-    description: Request object for the CreateWorkspace method.
+    description: Response object for cloud credentials.
     required:
-      - environmentName
-      - workspaceName
-      - usePublicLoadBalancer
-      - disableTLS
+      - clusterCrn
+      - clusterUrl
+      - replicationEngineType
+      - credentials
     properties:
-      environmentName:
+      clusterCrn:
+        description: Cluster CRN.
         type: string
-        description: The environment for the workspace to create.
-      workspaceName:
+      clusterUrl:
+        description: Cluster URL.
         type: string
-        description: The name of the workspace to create.
-      usePublicLoadBalancer:
-        type: boolean
-        description: The boolean flag to request public load balancer. By default private load balancer is used.
-      disableTLS:
-        type: boolean
-        description: The boolean flag to disable TLS setup for workspace. By default the TLS is enabled.
-      provisionK8sRequest:
-        description: The request for Kubernetes workspace provision.
-        $ref: '#/definitions/ProvisionK8sRequest'
-      enableMonitoring:
-        type: boolean
-        description: The boolean flag is used to enable mlonitoring. By default monitoring is disabled.
-      existingNFS:
+      replicationEngineType:
+        description: Replication engine type.
         type: string
-        description: Optionally use an existing NFS by providing the hostname and desired path (Azure and Private Cloud only).
-      loadBalancerIPWhitelists:
-        type: array
-        items:
-          type: string
-        description: The whitelist of ips for loadBalancer.
-  CreateWorkspaceResponse:
-    type: object
-    description: Response object for the CreateWorkspace method.
-  ListWorkspacesRequest:
+        enum:
+          - CM
+          - DLMENGINE
+      credentials:
+        description: Cloud credentials.
+        $ref: '#/definitions/CredentialCollection'
+  CredentialCollection:
     type: object
-    description: Request object for the ListWorkspaces method.
-  ListWorkspacesResponse:
-    type: object
-    description: Response object for the ListWorkspaces method.
+    description: Cloud Credentials listing.
+    required:
+      - totalResults
+      - results
+      - credentials
     properties:
-      workspaces:
+      totalResults:
+        description: Total number cloud credentials.
+        type: integer
+        format: int64
+      results:
+        description: Number of cloud credentials in the response.
+        type: integer
+        format: int64
+      credentials:
+        description: Cloud credential details.
         type: array
         items:
-          $ref: '#/definitions/WorkspaceSummary'
-        description: The list of workspaces.
-  WorkspaceSummary:
+          $ref: '#/definitions/CredentialDetails'
+  CredentialDetails:
     type: object
-    description: A Cloudera Machine Learning workspace which includes the deployed configuration details.
+    description: Cloud credential details for by-name or by-id cloud credential request.
     required:
-      - instanceName
-      - environmentName
-      - instanceStatus
-      - instanceUrl
-      - environmentCrn
-      - crn
-      - k8sClusterName
-      - creatorCrn
-      - version
-      - httpsEnabled
-      - filesystemID
-      - cloudPlatform
-      - monitoringEnabled
-    properties:
-      instanceName:
-        type: string
-        description: The name of the workspace.
-      environmentName:
-        type: string
-        description: The name of the workspace's environment.
-      instanceStatus:
-        type: string
-        description: The workspace's current status.
-      instanceUrl:
-        type: string
-        description: URL of the workspace's user interface.
-      environmentCrn:
-        type: string
-        description: CRN of the environment.
-      crn:
-        type: string
-        description: The CRN of the workspace.
-      k8sClusterName:
+      - id
+      - name
+      - provider
+      - authType
+      - creationTime
+      - lastModifiedTime
+    properties:
+      id:
+        description: Credential id.
         type: string
-        description: The Kubernetes cluster name.
-      creatorCrn:
+      name:
+        description: Credential name.
         type: string
-        description: The CRN of the creator of the workspace.
-      version:
+      provider:
+        description: Credential provider.
         type: string
-        description: The version of Cloudera Machine Learning that was installed on the workspace.
-      httpsEnabled:
-        type: boolean
-        description: Indicates if HTTPs communication was enabled on this workspace when provisioned.
-      filesystemID:
+      authType:
+        description: Authentication type.
         type: string
-        description: A filesystem ID referencing the filesystem that was created on the cloud provider environment that this workspace uses.
-      cloudPlatform:
-        type: string
-        description: The cloud platform of the environment that was used to create this workspace.
-      monitoringEnabled:
-        type: boolean
-        description: If usage monitoring is enabled or not on this workspace.
-      loadBalancerIPWhitelists:
-        type: array
-        items:
-          type: string
-        description: The whitelist of ips for loadBalancer.
-      creationDate:
+      creationTime:
+        description: Creation time.
         type: string
         format: date-time
-        description: Creation date of workspace.
-      failureMessage:
+      lastModifiedTime:
+        description: Last modified time.
         type: string
-        description: Failure message from the most recent failure that has occurred during workspace provisioning.
-      healthInfoLists:
+        format: date-time
+      configs:
+        description: Configurations.
+        type: object
+        additionalProperties:
+          type: string
+      customConfigs:
+        description: Custom configurations.
         type: array
         items:
-          $ref: '#/definitions/HealthInfo'
-        description: The health info information of the workspace.
-  Workspace:
+          $ref: '#/definitions/CustomConfigs'
+  ServiceInfo:
     type: object
-    description: A ML workspace, which includes the cluster and storage.
+    description: Service status definition.
     required:
-      - instanceName
-      - environmentName
-      - instanceStatus
-      - instanceUrl
-      - environmentCrn
-      - crn
-      - k8sClusterName
-      - creatorCrn
-      - version
-      - httpsEnabled
-      - endpointPublicAccess
-      - filesystemID
-      - tags
-      - instanceGroups
-      - cloudPlatform
-      - monitoringEnabled
-    properties:
-      instanceName:
-        type: string
-        description: The name of the workspace.
-      environmentName:
-        type: string
-        description: The name of the workspace's environment.
-      instanceStatus:
-        type: string
-        description: The workspace's current status.
-      instanceUrl:
+      - serviceName
+      - status
+    properties:
+      serviceName:
+        description: Service name.
         type: string
-        description: URL of the workspace's user interface.
-      environmentCrn:
+      status:
+        description: Service status.
         type: string
-        description: CRN of the environment.
-      crn:
+  Policy:
+    type: object
+    description: Replication policy definition.
+    required:
+      - policyId
+      - name
+      - type
+      - status
+      - frequency
+      - endTime
+      - jobs
+      - report
+    properties:
+      policyId:
+        description: Policy id.
         type: string
-        description: The CRN of the workspace.
-      k8sClusterName:
+      name:
+        description: Policy name.
         type: string
-        description: The Kubernetes cluster name.
-      creatorCrn:
+      type:
+        description: Policy type.
         type: string
-        description: The CRN of the creator of the workspace.
-      version:
+      status:
+        description: Current status of the policy.
         type: string
-        description: The version of Cloudera Machine Learning that was installed on the workspace.
-      httpsEnabled:
-        type: boolean
-        description: To Display if Https is enabled or not.
-      endpointPublicAccess:
-        type: boolean
-        description: To check if the cluster is publicly accessible or not.
-      filesystemID:
+      frequency:
+        description: Frequency in seconds when the policy runs.
+        type: integer
+        format: int64
+      endTime:
+        description: End time of policy run or when it repeats.
         type: string
-        description: filesystemID used by the workspace
-      tags:
+        format: date-time
+      jobs:
+        description: List of policy runs.
         type: array
         items:
-          $ref: '#/definitions/Tag'
-        description: Tags provided by the user at the time of workspace creation.
-      instanceGroups:
+          $ref: '#/definitions/PolicyInstanceResponse'
+      report:
+        description: Policy report.
+        $ref: '#/definitions/PolicyReport'
+      description:
+        description: Policy description.
+        type: string
+      executionType:
+        description: Policy execution type.
+        type: string
+      sourceDataset:
+        description: Source dataset of replication.
         type: array
         items:
-          $ref: '#/definitions/WorkspaceInstanceGroup'
-        description: The instance groups.
-      cloudPlatform:
-        type: string
-        description: The cloud platform of the environment that was used to create this workspace.
-      monitoringEnabled:
-        type: boolean
-        description: If usage monitoring is enabled or not on this workspace.
-      loadBalancerIPWhitelists:
+          type: string
+      targetDataset:
+        description: Target dataset of replication.
         type: array
         items:
           type: string
-        description: IP whitelist for loadBalancer.
-      creationDate:
+      creationTime:
+        description: Policy creation time.
         type: string
         format: date-time
-        description: Creation date of workspace.
-      healthInfoLists:
+      startTime:
+        description: Policy start time.
+        type: string
+        format: date-time
+      sourceCluster:
+        description: Source cluster of replication.
+        type: string
+      sourceClusterCrn:
+        description: CRN of the source cluster.
+        type: string
+      targetCluster:
+        description: Target cluster of replication if not cloud.
+        type: string
+      targetClusterCrn:
+        description: CRN of the target cluster.
+        type: string
+      customProperties:
+        description: Custom replication properties.
+        type: object
+        additionalProperties:
+          type: string
+      plugins:
+        description: Plugins.
         type: array
+        x-default: null
         items:
-          $ref: '#/definitions/HealthInfo'
-        description: The health info information of the workspace.
-      failureMessage:
+          type: string
+      nextRun:
+        description: Next expected run of the policy.
         type: string
-        description: Failure message from the most recent failure that has occurred during workspace provisioning.
-  UpgradeWorkspaceRequest:
+      target:
+        description: Replication target details.
+        $ref: '#/definitions/TargetDetails'
+  PolicyInstanceResponse:
     type: object
-    description: Request object for the UpgradeWorkspace method.
+    description: Policy execution details.
+    required:
+      - id
+      - policyId
+      - status
+      - startTime
     properties:
-      environmentName:
+      id:
+        description: Policy instance command id.
         type: string
-        description: The environment of the workspace.
-      workspaceName:
+      policyId:
+        description: Policy id.
         type: string
-        description: The name of the workspace.
-      mlVersion:
+      status:
+        description: Policy command status.
         type: string
-        description: The version of workspace to upgrade to.
-      workspaceCrn:
+      startTime:
+        description: Command start time.
         type: string
-        description: The CRN of the workspace. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  UpgradeWorkspaceResponse:
-    type: object
-    description: Response object for the UpgradeWorkspace method.
-  DescribeWorkspaceRequest:
-    type: object
-    description: Request object for the DescribeWorkspace method.
-    properties:
-      environmentName:
+        format: date-time
+      endTime:
+        description: Command end time.
         type: string
-        description: The environment for the workspace to describe.
-      workspaceName:
+        format: date-time
+      trackingInfo:
+        description: JSON data to track polciy status.
+        type: string
+      message:
+        description: Output of the policy command.
         type: string
-        description: The name of the workspace to describe.
-      workspaceCrn:
+      jobType:
+        description: Job type.
         type: string
-        description: The CRN of the workspace to describe. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  DescribeWorkspaceResponse:
+      totalSteps:
+        description: Total number of steps.
+        type: integer
+        format: int32
+      completedSteps:
+        description: Number of completed steps.
+        type: integer
+        format: int32
+  PolicyReportDetails:
     type: object
-    description: Response object for the DescribeWorkspace method.
+    description: Policy report details.
     required:
-      - workspace
+      - status
+      - endTime
+    properties:
+      status:
+        description: Status of the command.
+        type: string
+      endTime:
+        description: End time.
+        type: string
+        format: date-time
+  PolicyReport:
+    type: object
+    description: Policy report.
     properties:
-      workspace:
-        description: The workspace.
-        $ref: '#/definitions/Workspace'
-  DeleteWorkspaceRequest:
+      lastSucceededInstance:
+        description: Last successful instance.
+        $ref: '#/definitions/PolicyReportDetails'
+      lastFailedInstance:
+        description: Last failed instance.
+        $ref: '#/definitions/PolicyReportDetails'
+  TargetDetails:
     type: object
-    description: Request object for the DeleteWorkspace method.
+    description: Target details.
     required:
-      - force
-      - removeStorage
+      - environmentCrn
     properties:
-      force:
-        type: boolean
-        description: Force delete a workspace even if errors occur during deletion. Force delete removes the guarantee that resources in your cloud account will be cleaned up.
-      removeStorage:
-        type: boolean
-        description: The remove storage flag indicates weather to keep the backing workspace filesystem storage or remove it during delete.
-      environmentName:
-        type: string
-        description: The environment for the workspace to delete.
-      workspaceName:
+      environmentCrn:
+        description: Target's environment CRN.
         type: string
-        description: The name of the workspace to delete.
-      workspaceCrn:
+      warehouseCrn:
+        description: Target's warehouse CRN.
         type: string
-        description: The CRN of the workspace to delete. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  DeleteWorkspaceResponse:
+  PolicyDefinition:
     type: object
-    description: Response object for the DeleteWorkspace method.
-  GrantWorkspaceAccessRequest:
-    type: object
-    description: Request object for the GrantWorkspaceAccess method.
+    description: Policy creation request definition.
+    required:
+      - name
+      - type
+      - sourceDataset
+      - frequencyInSec
     properties:
-      arn:
+      name:
+        description: Name of the new policy.
         type: string
-        description: 'The aws user ARN to grant access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
-        x-deprecated: true
-      environmentName:
+      type:
+        description: Policy replication type.
         type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
+        enum:
+          - FS
+          - HIVE
+          - HBASE
+      sourceDataset:
+        description: Source dataset to replicate.
+        $ref: '#/definitions/SourceDataset'
+      frequencyInSec:
+        description: Policy's frequency in seconds.
+        type: integer
+        format: int64
+      targetDataset:
+        description: Dataset to replicate to.
         type: string
-        description: The name of the workspace to grant access to.
-      workspaceCrn:
+      cloudCredential:
+        description: Cloud credentials to use if replicating to Cloud.
         type: string
-        description: The CRN of the workspace to grant access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-      identifier:
+      sourceCluster:
+        description: 'Name of source cluster in the format: "dataCenterName$cluster name", for example "DC-Europe$My Source 42.'
         type: string
-        description: The cloud provider user id which will be granted access to the workspace's kubernetes cluster.
-  GrantWorkspaceAccessResponse:
-    type: object
-    description: Response object for the GrantWorkspaceAccess method.
-    required:
-      - kubeconfig
-    properties:
-      kubeconfig:
+      targetCluster:
+        description: 'Name of destination cluster in the format: "dataCenterName$cluster name", for example "DC-US$My Destination 17".'
         type: string
-        description: The Kubernetes config file
-  RevokeWorkspaceAccessRequest:
-    type: object
-    description: Request object for the RevokeWorkspace method.
-    properties:
-      arn:
+      startTime:
+        description: Start time.
         type: string
-        description: 'The aws user ARN to revoke access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
-        x-deprecated: true
-      environmentName:
+        format: date-time
+      endTime:
+        description: End time.
         type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
+        format: date-time
+      distcpMaxMaps:
+        description: Maximum Map jobs to use for replication.
+        type: integer
+        format: int64
+      distcpMapBandwidth:
+        description: Maximum bandwidth to use for replication.
+        type: integer
+        format: int64
+      queueName:
+        description: YARN queue name if not default.
+        type: string
+      tdeSameKey:
+        description: TDE same key.
+        type: boolean
+      description:
+        description: Description of the policy.
+        type: string
+      enableSnapshotBasedReplication:
+        description: Enable snapshot based replication.
+        type: boolean
+      cloudEncryptionAlgorithm:
+        description: The type of cloud encryption algorithm. Can be used only for HDP/Ambari managed clusters. Supported values are AES256,SSE-KMS.
         type: string
-        description: The name of the workspace to revoke access to.
-      workspaceCrn:
+      cloudEncryptionKey:
+        description: Cloud encryption key.
         type: string
-        description: The CRN of the workspace to revoke access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-      identifier:
+      plugins:
+        description: Plugins.
+        type: array
+        x-default: null
+        items:
+          type: string
+      hiveExternalTableBaseDirectory:
+        description: Hive external table base directory.
         type: string
-        description: The cloud provider user id which will be granted access to the workspace's kubernetes cluster.
-  RevokeWorkspaceAccessResponse:
+      cmPolicySubmitUser:
+        description: CM policy submit user.
+        $ref: '#/definitions/CmPolicySubmitUser'
+  SourceDataset:
+    type: object
+    description: Extra properties for the source dataset.
+    properties:
+      hdfsArguments:
+        description: HDFS arguments for HDFS and Hive replication.
+        $ref: '#/definitions/HdfsArguments'
+      hiveArguments:
+        description: Arguments for Hive replication, null if HDFS replication.
+        $ref: '#/definitions/HiveArguments'
+  HdfsArguments:
+    type: object
+    description: Extra properties for HDFS.
+    properties:
+      path:
+        description: HDFS path. Mandatory for HDFS policies, otherwise optional.
+        type: string
+      replicationStrategy:
+        description: Replication strategy.
+        type: string
+        enum:
+          - DYNAMIC
+          - STATIC
+      mapReduceService:
+        description: Name of the mapreduce service.
+        type: string
+      logPath:
+        description: Job log path.
+        type: string
+      errorHandling:
+        description: Error handling strategy.
+        $ref: '#/definitions/ErrorHandling'
+      preserve:
+        description: Properties to preserve.
+        $ref: '#/definitions/Preserve'
+      deletePolicy:
+        description: Deletion behavior.
+        type: string
+        enum:
+          - KEEP_DELETED_FILES
+          - DELETE_TO_TRASH
+          - DELETE_PERMANENTLY
+      alert:
+        description: Alerting behavior.
+        $ref: '#/definitions/Alert'
+      exclusionFilters:
+        description: Exclusion filters in glob format.
+        type: array
+        x-default: null
+        items:
+          type: string
+  ErrorHandling:
     type: object
-    description: Response object for the RevokeWorkspaceAccess method.
-  GetLatestWorkspaceVersionRequest:
+    description: Error handling behavior.
+    required:
+      - skipChecksumChecks
+      - skipListingChecksumChecks
+      - abortOnError
+      - abortOnSnapshotDiffFailures
+    properties:
+      skipChecksumChecks:
+        description: Skip checksum checks.
+        type: boolean
+      skipListingChecksumChecks:
+        description: Skip checksum checks for copy-listing.
+        type: boolean
+      abortOnError:
+        description: Abort policy on error.
+        type: boolean
+      abortOnSnapshotDiffFailures:
+        description: Abort policy if there are snapshot diff failures.
+        type: boolean
+  Preserve:
     type: object
-    description: Request object for GetLatestWorkspaceVersion.
-  GetLatestWorkspaceVersionResponse:
+    description: Properties to preserve after replication.
+    required:
+      - blockSize
+      - replicationCount
+      - permissions
+      - extendedAttributes
+    properties:
+      blockSize:
+        description: Block size.
+        type: boolean
+      replicationCount:
+        description: Replication count.
+        type: boolean
+      permissions:
+        description: Permissions.
+        type: boolean
+      extendedAttributes:
+        description: Extended attributes.
+        type: boolean
+  Alert:
     type: object
-    description: Response object for GetLatestWorkspaceVersion.
+    description: Cloudera Manager alerting behavior.
     required:
-      - version
+      - onFailure
+      - onStart
+      - onSuccess
+      - onAbort
     properties:
-      version:
-        type: string
-        description: The latest version of a workspace that is used when deploying Cloudera Machine Learning workspaces.
-  HealthInfo:
+      onFailure:
+        description: Alert on failure.
+        type: boolean
+      onStart:
+        description: Alert on start.
+        type: boolean
+      onSuccess:
+        description: ALert on success.
+        type: boolean
+      onAbort:
+        description: Alert on abort.
+        type: boolean
+  HiveArguments:
     type: object
-    description: Healthinfo object contains the health information of a resource.
+    description: Hive replication arguments.
+    properties:
+      databasesAndTables:
+        description: Scope of the replication.
+        type: array
+        items:
+          $ref: '#/definitions/HiveDatabaseAndTables'
+      sentryPermissions:
+        description: Include or exclude Sentry permissions.
+        type: string
+        enum:
+          - INCLUDE
+          - EXCLUDE
+      skipUrlPermissions:
+        description: Skip URL permissions.
+        type: boolean
+      numThreads:
+        description: Number of threads to use during replication.
+        type: integer
+        format: int64
+  HiveDatabaseAndTables:
+    type: object
+    description: Hive replication scope.
     required:
-      - resourceName
-      - isHealthy
-      - updatedAt
-      - message
-      - details
+      - database
     properties:
-      resourceName:
+      database:
+        description: Database to replicate.
         type: string
-        description: The resource name being checked.
-      isHealthy:
-        type: boolean
-        description: The boolean that indicates the health status.
-      updatedAt:
+      tablesIncludeRegex:
+        description: Regex to match included tables.
         type: string
-        format: date-time
-        description: The unix timestamp for the heartbeat.
-      message:
+      tablesExcludeRegex:
+        description: Regex to match excluded tables.
+        type: string
+  CmPolicySubmitUser:
+    type: object
+    description: CM Policy submit user.
+    properties:
+      userName:
+        description: Username.
+        type: string
+      sourceUser:
+        description: Source user.
         type: string
-        description: The message to show for the health info.
-      details:
-        type: array
-        items:
-          type: string
-        description: The detail of the health info.
```

### Comparing `cdpcli-0.9.9/cdpcli/data/environments/environments.yaml` & `cdpcli-0.9.90/cdpcli/data/ml/ml.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,1646 +1,1676 @@
+x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: environments2
-x-display-name: environments
+x-endpoint-name: ml
 x-products: CDP
+x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.1-SNAPSHOT
-  title: Cloudera Environments Service
+  version: 0.9.90
+  title: Cloudera Machine Learning
   license:
     name: Apache 2.0
-  description: Cloudera Environments Service is a web service that manages cloud provider access.
+  description: Install and manage Cloudera Machine Learning applications.
+  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/environments2/createAWSEnvironment:
+  /api/v1/ml/backupWorkspace:
     post:
-      summary: Creates a new AWS environment by providing the cloud provider access and network information. A FreeIPA server will be automatically provisioned when an environment is created.
-      description: Creates a new AWS environment.
-      operationId: createAWSEnvironment
+      summary: Backup a workspace.
+      description: Backup a workspace.
+      operationId: backupWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAWSEnvironmentRequest'
+            $ref: '#/definitions/BackupWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAWSEnvironmentResponse'
+            $ref: '#/definitions/BackupWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/createAzureEnvironment:
+      x-mutating: true
+  /api/v1/ml/createWorkspace:
     post:
-      summary: Creates a new Azure environment by providing the cloud provider access and network information. A FreeIPA server will be automatically provisioned when an environment is created.
-      description: Creates a new Azure environment.
-      operationId: createAzureEnvironment
+      summary: Create a Cloudera Machine Learning workspace.
+      description: Provision a Kubernetes cluster and install the Cloudera Machine Learning application in it.
+      operationId: createWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAzureEnvironmentRequest'
+            $ref: '#/definitions/CreateWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAzureEnvironmentResponse'
+            $ref: '#/definitions/CreateWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/createAWSCredential:
+      x-mutating: true
+  /api/v1/ml/deleteBackup:
     post:
-      summary: Creates a new AWS credential that can be attatched to an environment. The credential is used for authorization to provision resources such as compute instances within your cloud provider account.
-      description: Creates a new AWS credential.
-      operationId: createAWSCredential
+      summary: Deletes a backup snapshot.
+      description: Deletes a Cloudera Machine Learning workspace backup.
+      operationId: deleteBackup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAWSCredentialRequest'
+            $ref: '#/definitions/DeleteBackupRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAWSCredentialResponse'
+            $ref: '#/definitions/DeleteBackupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/createAzureCredential:
+      x-mutating: true
+  /api/v1/ml/deleteInstanceGroup:
     post:
-      summary: Creates a new Azure credential that can be attatched to an environment. The credential is used for authorization to provision resources such as compute instances within your cloud provider account.
-      description: Creates a new Azure credential.
-      operationId: createAzureCredential
+      summary: Deletes an instance group from the cluster.
+      description: Deletes an instance group from a Cloudera Machine Learning workspace.
+      operationId: deleteInstanceGroup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAzureCredentialRequest'
+            $ref: '#/definitions/DeleteInstanceGroupRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAzureCredentialResponse'
+            $ref: '#/definitions/DeleteInstanceGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/changeEnvironmentCredential:
+      x-mutating: true
+  /api/v1/ml/deleteWorkspace:
     post:
-      summary: Changes the credential for an environment.
-      description: Changes the credential for an environment.
-      operationId: changeEnvironmentCredential
+      summary: Delete Cloudera Machine Learning Workspace.
+      description: Deletes a Cloudera Machine Learning workspace.
+      operationId: deleteWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ChangeEnvironmentCredentialRequest'
+            $ref: '#/definitions/DeleteWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ChangeEnvironmentCredentialResponse'
+            $ref: '#/definitions/DeleteWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/deleteEnvironment:
+      x-mutating: true
+  /api/v1/ml/describeWorkspace:
     post:
-      summary: Deletes an environment.
-      description: Deletes an environment.
-      operationId: deleteEnvironment
+      summary: Describe Cloudera Machine Learning Workspace.
+      description: Describes a Cloudera Machine Learning workspace.
+      operationId: describeWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteEnvironmentRequest'
+            $ref: '#/definitions/DescribeWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteEnvironmentResponse'
+            $ref: '#/definitions/DescribeWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/deleteCredential:
+      x-mutating: false
+  /api/v1/ml/getAuditEvents:
     post:
-      summary: Deletes a credential.
-      description: Deletes a credential.
-      operationId: deleteCredential
+      summary: Gets all the events belong to a workspace crn.
+      description: Gets all the events belong to a workspace crn.
+      operationId: getAuditEvents
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteCredentialRequest'
+            $ref: '#/definitions/GetAuditEventsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteCredentialResponse'
+            $ref: '#/definitions/GetAuditEventsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/listEnvironments:
+      x-mutating: false
+  /api/v1/ml/getKubeconfig:
     post:
-      summary: Lists environments.
-      description: Lists environments.
-      operationId: listEnvironments
+      summary: ListWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Lists users that can perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: getKubeconfig
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListEnvironmentsRequest'
+            $ref: '#/definitions/GetKubeconfigRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListEnvironmentsResponse'
+            $ref: '#/definitions/GetKubeconfigResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/listCredentials:
+      x-mutating: false
+  /api/v1/ml/getLatestWorkspaceVersion:
     post:
-      summary: Lists credentials.
-      description: Lists credentials.
-      operationId: listCredentials
+      summary: GetLatestWorkspaceVersion Cloudera Machine Learning Workspace.
+      description: Retrieves the latest version that Cloudera Machine Learning deploys to workspaces.
+      operationId: getLatestWorkspaceVersion
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListCredentialsRequest'
+            $ref: '#/definitions/GetLatestWorkspaceVersionRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListCredentialsResponse'
+            $ref: '#/definitions/GetLatestWorkspaceVersionResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/describeEnvironment:
+      x-mutating: false
+  /api/v1/ml/getLogs:
     post:
-      summary: Describes an environment.
-      description: Describes an environment.
-      operationId: describeEnvironment
+      summary: Gets all the logs belong to a request id.
+      description: Gets all the logs belong to a request id.
+      operationId: getLogs
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeEnvironmentRequest'
+            $ref: '#/definitions/GetLogsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeEnvironmentResponse'
+            $ref: '#/definitions/GetLogsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/syncAllUsers:
+      x-mutating: false
+  /api/v1/ml/grantWorkspaceAccess:
     post:
-      summary: Synchronizes environments with all users and groups state with CDP.
-      description: Synchronizes environments with all users and groups state with CDP.
-      operationId: syncAllUsers
+      summary: GrantWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Grants an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: grantWorkspaceAccess
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SyncAllUsersRequest'
+            $ref: '#/definitions/GrantWorkspaceAccessRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SyncAllUsersResponse'
+            $ref: '#/definitions/GrantWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/syncUser:
+      x-mutating: true
+  /api/v1/ml/listWorkspaceAccess:
     post:
-      summary: Synchronizes environments with single user to the FreeIPA servers.
-      description: Synchronizes environments with single user to the FreeIPA servers.
-      operationId: syncUser
+      summary: ListWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Lists users that can perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: listWorkspaceAccess
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SyncUserRequest'
+            $ref: '#/definitions/ListWorkspaceAccessRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SyncUserResponse'
+            $ref: '#/definitions/ListWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/syncStatus:
+      x-mutating: false
+  /api/v1/ml/listWorkspaceBackups:
     post:
-      summary: Returns status of the sync operation for the operation id.
-      description: Returns status of the sync operation for the operation id. Operation Id should be one of the previously request sync operation.
-      operationId: syncStatus
+      summary: List backup snapshots of a workspace.
+      description: List backup snapshots of a workspace.
+      operationId: listWorkspaceBackups
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SyncStatusRequest'
+            $ref: '#/definitions/ListWorkspaceBackupsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SyncStatusResponse'
+            $ref: '#/definitions/ListWorkspaceBackupsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/setPassword:
+      x-mutating: false
+  /api/v1/ml/listWorkspaces:
     post:
-      summary: Sets workload user's password and updates into all environments.
-      description: Sets workload user's password and updates into all environments if there is no environment CRN passed or, if environment CRNs list is provided, then password is reset only for that environment. Password must be of min 8 characters and no more then 64 characters and should be combination of UPPER Case, lower case, digits and special characters.
-      operationId: setPassword
+      summary: List Cloudera Machine Learning workspaces.
+      description: List Cloudera Machine Learning workspaces.
+      operationId: listWorkspaces
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SetPasswordRequest'
+            $ref: '#/definitions/ListWorkspacesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SetPasswordResponse'
+            $ref: '#/definitions/ListWorkspacesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/getRootCertificate:
+      x-skip-auditing: true
+  /api/v1/ml/modifyClusterInstanceGroup:
     post:
-      summary: This API provides contents of public certificate for an environment.
-      description: This API provides the contents of the root public certificate for an environment. The contents are a base64 encoded blob between -----BEGIN CERTIFICATE----- and -----END CERTIFICATE-----. This certificate can be imported by end users to establish trust with environment resources.
-      operationId: getRootCertificate
+      summary: Modify Cloudera Machine Learning workspace cluster instance group.
+      description: Modify a Cloudera Machine Learning workspace cluster instance group.
+      operationId: modifyClusterInstanceGroup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetRootCertificateRequest'
+            $ref: '#/definitions/ModifyClusterInstanceGroupRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetRootCertificateResponse'
+            $ref: '#/definitions/ModifyClusterInstanceGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/getIdBrokerMappings:
+      x-mutating: true
+  /api/v1/ml/modifyClusterSecurity:
     post:
-      summary: Gets all ID Broker mappings for an environment.
-      description: Gets all ID Broker mappings for an environment.
-      operationId: getIdBrokerMappings
+      summary: Modify Cloudera Machine Learning workspace cluster security.
+      description: Modify a Cloudera Machine Learning workspace cluster security.
+      operationId: modifyClusterSecurity
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetIdBrokerMappingsRequest'
+            $ref: '#/definitions/ModifyClusterSecurityRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetIdBrokerMappingsResponse'
+            $ref: '#/definitions/ModifyClusterSecurityResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/setIdBrokerMappings:
+      x-mutating: true
+  /api/v1/ml/modifyWorkspaceLoadBalancer:
     post:
-      summary: Sets all ID Broker mappings for an environment.
-      description: Sets all ID Broker mappings for an environment. Overwrites all existing mappings.
-      operationId: setIdBrokerMappings
+      summary: Modify Cloudera Machine Learning workspace loadbalancer.
+      description: Modify a Cloudera Machine Learning workspace loadbalancer.
+      operationId: modifyWorkspaceLoadBalancer
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SetIdBrokerMappingsRequest'
+            $ref: '#/definitions/ModifyWorkspaceLoadBalancerRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SetIdBrokerMappingsResponse'
+            $ref: '#/definitions/ModifyWorkspaceLoadBalancerResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/syncIdBrokerMappings:
+      x-mutating: true
+  /api/v1/ml/requestWorkflowCancellation:
     post:
-      summary: Syncs all ID Broker mappings for an environment.
-      description: Syncs all ID Broker mappings to all datalake clusters in an environment.
-      operationId: syncIdBrokerMappings
+      summary: Request a workflow cancellation.
+      description: Request a long running workflow cancellation by resource ID and workflow type.
+      operationId: requestWorkflowCancellation
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SyncIdBrokerMappingsRequest'
+            $ref: '#/definitions/RequestWorkflowCancellationRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SyncIdBrokerMappingsResponse'
+            $ref: '#/definitions/RequestWorkflowCancellationResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/getIdBrokerMappingsSyncStatus:
+      x-mutating: true
+  /api/v1/ml/restoreWorkspace:
     post:
-      summary: Gets ID Broker mappings sync status.
-      description: Gets the status of the most recent ID Broker mappings sync operation, if any.
-      operationId: getIdBrokerMappingsSyncStatus
+      summary: Restore a Cloudera Machine Learning workspace.
+      description: Create a new workspace based on an existing workspace backup snapshot.
+      operationId: restoreWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetIdBrokerMappingsSyncStatusRequest'
+            $ref: '#/definitions/RestoreWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetIdBrokerMappingsSyncStatusResponse'
+            $ref: '#/definitions/RestoreWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/startEnvironment:
+      x-mutating: true
+  /api/v1/ml/resumeWorkspace:
     post:
-      summary: Start an environment.
-      description: Start an environment.
-      operationId: startEnvironment
+      summary: Resume Cloudera Machine Learning workspace.
+      description: Resume a Cloudera Machine Learnings workspace.
+      operationId: resumeWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StartEnvironmentRequest'
+            $ref: '#/definitions/ResumeWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StartEnvironmentResponse'
+            $ref: '#/definitions/ResumeWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/stopEnvironment:
+      x-mutating: true
+  /api/v1/ml/revokeWorkspaceAccess:
     post:
-      summary: Stop an environment.
-      description: Stop an environment.
-      operationId: stopEnvironment
+      summary: RevokeWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Revokes an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: revokeWorkspaceAccess
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StopEnvironmentRequest'
+            $ref: '#/definitions/RevokeWorkspaceAccessRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StopEnvironmentResponse'
+            $ref: '#/definitions/RevokeWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/getFreeipaStatus:
+      x-mutating: true
+  /api/v1/ml/suspendWorkspace:
     post:
-      summary: Get the status of the FreeIPA services
-      description: Gets the status of the FreeIPA nodes services and connectivity.
-      operationId: getFreeipaStatus
+      summary: Suspend Cloudera Machine Learning workspace.
+      description: Suspend a Cloudera Machine Learning workspace.
+      operationId: suspendWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetFreeipaStatusRequest'
+            $ref: '#/definitions/SuspendWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetFreeipaStatusResponse'
+            $ref: '#/definitions/SuspendWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/environments2/repairFreeipa:
+      x-mutating: true
+  /api/v1/ml/upgradeWorkspace:
     post:
-      summary: Repairs the FreeIPA nodes.
-      description: Repairs the FreeIPA nodes if they are in a non working state.
-      operationId: repairFreeipa
+      summary: Upgrade Cloudera Machine Learning workspace.
+      description: Upgrades a Cloudera Machine Learning workspace to the latest available version.
+      operationId: upgradeWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RepairFreeipaRequest'
+            $ref: '#/definitions/UpgradeWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RepairFreeipaResponse'
+            $ref: '#/definitions/UpgradeWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+      x-mutating: true
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  CreateAWSCredentialResponse:
+  RootVolume:
     type: object
-    description: Response object for a create AWS credential request.
+    description: Configuration for instance root device volume.
     required:
-      - credential
+      - size
     properties:
-      credential:
-        description: The credential object.
-        $ref: '#/definitions/Credential'
-  CreateAWSCredentialRequest:
+      size:
+        type: integer
+        format: int64
+        description: The volume size in GB.
+  GetLogsRequest:
     type: object
-    description: Request object for a create AWS credential request.
+    description: GetLogsRequestfor getting logs for a request ID.
     required:
-      - credentialName
-      - roleArn
+      - workspaceCrn
+      - requestID
     properties:
-      credentialName:
+      workspaceCrn:
         type: string
-        description: The name of the credential.
-      roleArn:
+        description: WorkspaceCrn the requestID belongs to.
+      requestID:
         type: string
-        description: The ARN of the delegated access role.
-      description:
-        type: string
-        description: A description for the credential.
-  CreateAzureCredentialRequest:
+        description: Unique Key to identify a set of logs.
+      fetchAll:
+        type: boolean
+        description: Flag to fetch all logs.
+      pageSize:
+        type: integer
+        format: int32
+        description: Limit the number of logs.
+      offset:
+        type: integer
+        format: int32
+        description: offset from which the logs should be fetched.
+  GetLogsResponse:
+    type: object
+    description: GetLogsResponse contains all the logs for a given request id.
+    required:
+      - auditLogs
+    properties:
+      auditLogs:
+        description: Contains all the logs for a given request id.
+        $ref: '#/definitions/AuditLogs'
+  AuditLogs:
     type: object
-    description: Request object for a create Azure credential request.
+    description: AuditLogs contains all the logs for a given request id.
     required:
-      - credentialName
-      - subscriptionId
-      - tenantId
-      - appBased
+      - requestID
+      - count
+      - logs
     properties:
-      credentialName:
+      requestID:
         type: string
-        description: The name of the credential.
-      subscriptionId:
+        description: The request ID associated with a long-running operation to fetch the logs for.
+      count:
+        type: integer
+        format: int32
+        description: Total number of logs associated with the request id.
+      logs:
+        type: array
+        items:
+          $ref: '#/definitions/AuditLog'
+        description: Contains all the logs for a given request id.
+  AuditLog:
+    type: object
+    description: Audit log represents an individual log.
+    required:
+      - createdDate
+      - log
+    properties:
+      createdDate:
         type: string
-        description: The Azure subscription ID.
-      tenantId:
+        format: date-time
+        description: Time at which the log is created.
+      log:
         type: string
-        description: The Azure AD tenant ID for the Azure subscription.
-      appBased:
-        type: object
-        description: Additional configurations needed for app-based authentication.
-        required:
-          - applicationId
-          - secretKey
-        properties:
-          applicationId:
-            type: string
-            description: The id of the application registered in Azure.
-          secretKey:
-            type: string
-            x-sensitive: true
-            description: The client secret key (also referred to as application password) for the registered application.
-      description:
+        description: Log description.
+  GetAuditEventsRequest:
+    type: object
+    description: GetAuditEventsRequest to get all audit events for a given workspace crn.
+    required:
+      - workspaceCrn
+    properties:
+      workspaceCrn:
         type: string
-        description: A description for the credential.
-  CreateAzureCredentialResponse:
+        description: Workspace crn for which audit events to be fetched.
+  GetAuditEventsResponse:
     type: object
-    description: Response object for a create Azure credential request.
+    description: GetAuditEventsResponse containes all the audit events for a given workspace crn.
     required:
-      - credential
+      - auditEvents
     properties:
-      credential:
-        description: The credential object.
-        $ref: '#/definitions/Credential'
-  Credential:
+      auditEvents:
+        description: Contains all the audit events for a given workspace crn.
+        $ref: '#/definitions/AuditEvents'
+  AuditEvents:
     type: object
-    description: A credential object.
+    description: AuditEvents contains all the audit events for a given workspace crn.
     required:
-      - credentialName
-      - crn
-      - cloudPlatform
+      - workspaceCrn
+      - events
     properties:
-      credentialName:
+      workspaceCrn:
         type: string
-        description: The name of the credential.
-      crn:
+        description: Workspace crn unique for the set of audit events.
+      events:
+        type: array
+        items:
+          $ref: '#/definitions/AuditEvent'
+        description: AuditEvent belong to the workspace crn.
+  AuditEvent:
+    type: object
+    description: Audit event descibes an performed or performing in a given workspace.
+    required:
+      - workspaceCrn
+      - userCrn
+      - requestID
+      - action
+      - createdDate
+    properties:
+      workspaceCrn:
         type: string
-        description: The CRN of the credential.
-      cloudPlatform:
+        description: Workspace crn where the event observed.
+      userCrn:
+        type: string
+        description: UserCrn to track which user has caused the event.
+      requestID:
+        type: string
+        description: Unique request ID to keep track of event.
+      action:
         type: string
-        description: The cloud provider.
-      description:
+        description: Action the user has generated.
+      createdDate:
         type: string
-        description: A description for the credential.
-  CreateAWSEnvironmentRequest:
+        format: date-time
+        description: Time at creation of event.
+  Autoscaling:
     type: object
-    description: Request object for a create AWS environment request.
+    description: Configuration for instance auto scaling.
     required:
-      - environmentName
-      - credentialName
-      - region
-      - securityAccess
-      - authentication
-      - logStorage
+      - minInstances
+      - maxInstances
     properties:
-      environmentName:
-        type: string
-        description: The name of the environment. Must contain only lowercase letters, numbers and hyphens.
-      credentialName:
-        type: string
-        description: Name of the credential to use for the environment.
-      region:
+      minInstances:
+        type: integer
+        format: int32
+        description: The minimum number of instance for auto scaling.
+      maxInstances:
+        type: integer
+        format: int32
+        description: The maximum number of instance for auto scaling.
+      enabled:
+        type: boolean
+        description: The boolean flag to enable the auto scaling.
+  InstanceGroup:
+    type: object
+    description: Contains the necessary info for an instance group.
+    required:
+      - instanceType
+    properties:
+      instanceType:
         type: string
-        description: The region of the environment.
-      securityAccess:
-        description: Security control for FreeIPA and Datalake deployment.
-        $ref: '#/definitions/SecurityAccessRequest'
-      authentication:
-        description: SSH authentication information for accessing cluster node instances. Users with access to this authentication information have root level access to the Data Lake and Data Hub cluster instances.
-        $ref: '#/definitions/AuthenticationRequest'
-      logStorage:
-        description: AWS storage configuration for cluster and audit logs.
-        $ref: '#/definitions/AwsLogStorageRequest'
-      networkCidr:
+        description: The cloud provider instance type for the node instance.
+      instanceTier:
         type: string
-        description: The network CIDR. This will create a VPC along with subnets in multiple Availability Zones.
-      vpcId:
+        description: The tier of the instance i.e. on-demand/spot.
+      instanceCount:
+        type: integer
+        format: int32
+        description: The initial number of instance node.
+      name:
         type: string
-        description: The Amazon VPC ID. Mutually exclusive with networkCidr.
-      subnetIds:
+        description: The unique name of the instance group.
+      ingressRules:
         type: array
-        description: One or more subnet ids within the VPC. Mutually exclusive with networkCidr.
-        uniqueItems: true
         items:
           type: string
-      s3GuardTableName:
+        description: The networking rules for the ingress.
+      rootVolume:
+        description: The root volume of the instance.
+        $ref: '#/definitions/RootVolume'
+      autoscaling:
+        description: The auto scaling configuration.
+        $ref: '#/definitions/Autoscaling'
+  WorkspaceInstanceGroup:
+    type: object
+    description: Instance group information to show in workspace details.
+    required:
+      - instanceType
+      - instanceCount
+      - instanceGroupName
+      - minInstances
+      - maxInstances
+      - instances
+      - tags
+    properties:
+      instanceType:
         type: string
-        description: The name for the DynamoDB table backing S3Guard.
-      description:
+        description: The cloud provider instance type for the node instance.
+      instanceCount:
+        type: integer
+        format: int32
+        description: The initial number of instance node.
+      instanceGroupName:
         type: string
-        description: An description of the environment.
-      freeIpa:
-        $ref: '#/definitions/AWSFreeIpaCreationRequest'
-        description: The FreeIPA creation request for the environment
+        description: The unique name of the instance group.
+      minInstances:
+        type: integer
+        format: int32
+        description: The minimum number of instances that can be deployed to this instance group. If the value is 0, the group might be empty.
+      maxInstances:
+        type: integer
+        format: int32
+        description: The maximum number of instances that can be deployed to this instance group.
+      instances:
+        type: array
+        items:
+          $ref: '#/definitions/Instance'
+        description: Instances in the instance group.
       tags:
         type: array
-        description: Tags associated with the resources.
         items:
-          $ref: '#/definitions/TagRequest'
-  AwsLogStorageRequest:
+          $ref: '#/definitions/Tag'
+        description: Tags are key/value pairs that are applied to all tag-able resources deployed in the workspace's cloud environment.
+  Instance:
     type: object
+    description: Represents each instance in an instance group.
     required:
-      - storageLocationBase
-      - instanceProfile
-    description: AWS storage configuration for cluster and audit logs.
+      - instanceId
+      - availabilityZone
     properties:
-      storageLocationBase:
+      instanceId:
         type: string
-        description: The base location to store logs in S3. This should be an s3a:// url.
-      instanceProfile:
+        description: Unique instance Id generated by the cloud provider.
+      availabilityZone:
         type: string
-        description: The AWS instance profile that which contains the necessary permissions to access the S3 storage location.
-  AzureLogStorageRequest:
+        description: Availability zone the instance belongs to.
+  Tag:
     type: object
-    description: Azure storage configuration for cluster and audit logs.
+    description: Contains a single tag entry associated with a workspace.
     required:
-      - storageLocationBase
-      - managedIdentity
+      - key
+      - value
     properties:
-      storageLocationBase:
+      key:
         type: string
-        description: The storage location to use. The location has to be in the following format abfs://filesystem@storage-account-name.dfs.core.windows.net. The filesystem must already exist and the storage account must be StorageV2.
-      managedIdentity:
+        description: The name for the tag.
+      value:
         type: string
-        description: The managed identity associated with the logger. This identity should have Storage Blob Data Contributor role on the given storage account.
-  LogStorage:
+        description: The value for the tag.
+  ProvisionTag:
     type: object
-    description: Storage configuration for cluster and audit logs.
+    description: Contains a single tag entry that will be configured on cloud resources associated with a workspace.
     required:
-      - enabled
-    properties:
-      enabled:
-        type: boolean
-        description: Whether external log storage is enabled.
-      awsDetails:
-        type: object
-        description: AWS-specific log storage configuration information.
-        properties:
-          storageLocationBase:
-            type: string
-            description: The base location to store logs in S3. This should be an s3a:// url.
-          instanceProfile:
-            type: string
-            description: The AWS instance profile that which contains the necessary permissions to access the S3 storage location.
-      azureDetails:
-        type: object
-        description: Azure-specific log storage configuration information.
-        properties:
-          storageLocationBase:
-            type: string
-            description: The storage location to use. The location has to be in the following format abfs://filesystem@storage-account-name.dfs.core.windows.net.
-          managedIdentity:
-            type: string
-            description: The managed identity associated with the logger. This identity should have Storage Blob Data Contributor role on the given storage account.
-  SecurityAccessRequest:
-    type: object
-    description: Security control configuration for FreeIPA and Datalake deployment. Choosing a CIDR will automatically create security groups. Alternatively existing security groups can be specified.
-    properties:
-      cidr:
-        type: string
-        description: CIDR range which is allowed for inbound traffic. Either IPv4 or IPv6 is allowed.
-      securityGroupIdForKnox:
-        type: string
-        description: Security group where Knox-enabled hosts are placed. Mutually exclusive with cidr.
-      defaultSecurityGroupId:
-        type: string
-        description: Security group where all other hosts are placed. Mutually exclusive with cidr.
-  SecurityAccess:
-    type: object
-    description: Security control configuration for FreeIPA and Datalake deployment.
+      - key
+      - value
     properties:
-      cidr:
-        type: string
-        description: CIDR range which is allowed for inbound traffic. Either IPv4 or IPv6 is allowed.
-      securityGroupIdForKnox:
+      key:
         type: string
-        description: Security group where Knox-enabled hosts are placed.
-      defaultSecurityGroupId:
+        description: The name for the tag.
+      value:
         type: string
-        description: Security group where all other hosts are placed.
-  CreateAWSEnvironmentResponse:
-    type: object
-    description: Response object for a create AWS environment request.
-    required:
-      - environment
-    properties:
-      environment:
-        $ref: '#/definitions/Environment'
-        description: Created environment object.
-  CreateAzureEnvironmentResponse:
+        description: The value for the tag.
+  ProvisionK8sRequest:
     type: object
-    description: Response object for a create Azure environment request.
+    description: Request object for workspace provision.
     required:
-      - environment
-    properties:
-      environment:
-        $ref: '#/definitions/Environment'
-        description: Created environment object.
-  ListEnvironmentsRequest:
-    type: object
-    description: Request object for a list environments request.
-  ListEnvironmentsResponse:
-    type: object
-    description: Response object for a list environments request.
-    required:
-      - environments
+      - instanceGroups
+      - environmentName
     properties:
-      environments:
+      instanceGroups:
         type: array
         items:
-          $ref: '#/definitions/EnvironmentSummary'
-        description: The environment.
-  ListCredentialsRequest:
+          $ref: '#/definitions/InstanceGroup'
+        description: The instance groups.
+      environmentName:
+        type: string
+        description: The name of the environment for the workspace to create.
+      tags:
+        type: array
+        items:
+          $ref: '#/definitions/ProvisionTag'
+        description: Tags to add to the cloud provider resources created. This is in addition to any tags added by Cloudera.
+      network:
+        description: The overlay network for an AWS Kubernetes cluster's CNI.
+        $ref: '#/definitions/OverlayNetwork'
+  OverlayNetwork:
     type: object
-    description: Request object for a list credentials request.
+    description: Contains the information about overlay network.
     properties:
-      credentialName:
+      plugin:
         type: string
-        description: An optional credential name to search by.
-  ListCredentialsResponse:
+        description: 'The plugin specifies specific cni vendor, ex: calico, weave etc.'
+      topology:
+        description: The options for overlay topology.
+        $ref: '#/definitions/Topology'
+  Topology:
     type: object
-    description: Response object for a list credentials request.
-    required:
-      - credentials
+    description: Contains the information about topology.
     properties:
-      credentials:
+      subnets:
         type: array
         items:
-          $ref: '#/definitions/Credential'
-        description: The credentials.
-  CreateAzureEnvironmentRequest:
+          type: string
+        description: The options for subnets.
+  ExistingDatabaseConfig:
+    type: object
+    description: Configurations for bringing an existing database for model metrics
+    properties:
+      existingDatabaseHost:
+        type: string
+        description: Optionally provide a Postgresql database host to export model metrics to.
+      existingDatabasePort:
+        type: string
+        description: Optionally provide a Postgresql database port to export model metrics to.
+      existingDatabaseName:
+        type: string
+        description: Optionally provide a Postgresql database name to export model metrics to.
+      existingDatabaseUser:
+        type: string
+        description: Optionally provide a Postgresql database user to use when exporting model metrics.
+      existingDatabasePassword:
+        type: string
+        description: Optionally provide a Postgresql database password to use when exporting model metrics.
+        x-sensitive: true
+  CreateWorkspaceRequest:
     type: object
-    description: Request object for a create Azure environment request.
+    description: Request object for the CreateWorkspace method.
     required:
       - environmentName
-      - credentialName
-      - region
-      - publicKey
-      - securityAccess
-      - usePublicIp
-      - logStorage
+      - workspaceName
     properties:
       environmentName:
         type: string
-        description: The name of the environment. Must contain only lowercase letters, numbers and hyphens.
-      credentialName:
+        description: The environment for the workspace to create.
+      workspaceName:
         type: string
-        description: Name of the credential to use for the environment.
-      region:
+        description: The name of the workspace to create.
+      usePublicLoadBalancer:
+        type: boolean
+        description: The boolean flag to request public load balancer. By default, private load balancer is used.
+      disableTLS:
+        type: boolean
+        description: The boolean flag to disable TLS setup for workspace. By default, the TLS is enabled.
+      provisionK8sRequest:
+        description: The request for Kubernetes workspace provision. Required in public cloud.
+        $ref: '#/definitions/ProvisionK8sRequest'
+      enableMonitoring:
+        type: boolean
+        description: The boolean flag is used to enable monitoring. By default, monitoring is disabled.
+      enableGovernance:
+        type: boolean
+        description: Enables Cloudera Machine Learning governance by integrating with Cloudera Atlas. By default, this flag is disabled.
+      existingNFS:
         type: string
-        description: The region of the environment.
-      publicKey:
+        description: Optionally use an existing NFS by providing the hostname and desired path (Azure and Private Cloud only).
+      loadBalancerIPWhitelists:
+        type: array
+        items:
+          type: string
+        description: The whitelist of IPs for load balancer.
+      nfsVersion:
         type: string
-        description: Public SSH key string. The associated private key can be used to get root-level access to the Data Lake instance and Data Hub cluster instances.
-      securityAccess:
-        description: Security control for FreeIPA and Datalake deployment.
-        $ref: '#/definitions/SecurityAccessRequest'
-      usePublicIp:
-        type: boolean
-        description: Whether to associate public ip's to the resources within the network.
-      logStorage:
-        description: Azure storage configuration for cluster and audit logs.
-        $ref: '#/definitions/AzureLogStorageRequest'
-      existingNetworkParams:
-        description: Parameters needed to use an existing VNet and Subnets.
-        $ref: '#/definitions/ExistingAzureNetworkRequest'
-      newNetworkParams:
-        type: object
-        description: Parameteres needed to automatically create VNet and Subnets.
-        required:
-          - networkCidr
-        properties:
-          networkCidr:
-            type: string
-            description: The range of private IPv4 addresses that resources will use under the created VNet.
-      description:
-        type: string
-        description: An description of the environment.
-      freeIpa:
-        $ref: '#/definitions/AzureFreeIpaCreationRequest'
-        description: The FreeIPA creation request for the environment
-      tags:
+        description: The NFS Protocol version of the NFS server we are using for Azure and Private Cloud.
+      enableModelMetrics:
+        type: boolean
+        description: Enables the model metrics service for exporting metrics for models to a metrics store.
+      existingDatabaseConfig:
+        description: Optional configurations for an existing Postgres to export model metrics to.
+        $ref: '#/definitions/ExistingDatabaseConfig'
+      whitelistAuthorizedIPRanges:
+        type: boolean
+        description: Whether to whitelist only 'authorizedIPRanges' given or all public IPs.
+      authorizedIPRanges:
+        type: array
+        items:
+          type: string
+        description: The whitelist of CIDR blocks which can access the API server.
+      skipValidation:
+        type: boolean
+        description: Skip pre-flight validations if requested
+      subnetsForLoadBalancers:
         type: array
-        description: Tags associated with the resources.
         items:
-          $ref: '#/definitions/TagRequest'
-  ExistingAzureNetworkRequest:
+          type: string
+        description: The list of subnets used for the load balancer that CML creates.
+      staticSubdomain:
+        type: string
+        description: The static subdomain to be used for the workspace.
+      cdswMigrationMode:
+        type: string
+        description: Toggle for cdsw migration preflight validation
+      outboundTypes:
+        type: array
+        items:
+          $ref: '#/definitions/OutboundTypes'
+        description: Outbound Types provided for the workspace.
+  OutboundTypes:
+    type: string
+    description: List of possible Outbound types.
+    enum:
+      - UNKNOWN
+      - OUTBOUND_TYPE_UDR
+  RestoreWorkspaceRequest:
+    type: object
+    description: Request object for RestoreWorkspace method.
+    properties:
+      newWorkspaceParameters:
+        description: The parameters required for a new Cloudera Machine Learning workspace.
+        $ref: '#/definitions/CreateWorkspaceRequest'
+      backupCrn:
+        type: string
+        description: The CRN of the backup snapshot to used for restoring.
+      useStaticSubdomain:
+        type: boolean
+        description: A boolean value to check if subdomain must be used or not.
+      restoreJobTimeoutMinutes:
+        type: integer
+        format: int32
+        description: The timeout to restore the backup snapshots, in minutes.
+  CreateWorkspaceResponse:
     type: object
-    description: Request object for creating an Azure environment using existing VNet and subnets.
-    required:
-      - networkId
-      - resourceGroupName
-      - subnetIds
+    description: Response object for the CreateWorkspace method.
+  RestoreWorkspaceResponse:
+    type: object
+    description: Response object for the RestoreWorkspace method.
     properties:
-      networkId:
-        type: string
-        description: The id of the Azure VNet.
-      resourceGroupName:
+      workspaceCrn:
         type: string
-        description: The name of the resource group associated with the VNet.
-      subnetIds:
+        description: The CRN of the Cloudera Machine Learning workspace being provisioned.
+  ListWorkspacesRequest:
+    type: object
+    description: Request object for the ListWorkspaces method.
+    properties:
+      queryOptions:
         type: array
-        description: One or more subnet ids within the VNet.
-        uniqueItems: true
         items:
           type: string
-  ChangeEnvironmentCredentialRequest:
+        description: Additional query options.
+  ListWorkspacesResponse:
     type: object
-    description: Request object for a change environment credentials request.
-    required:
-      - environmentName
-      - credentialName
+    description: Response object for the ListWorkspaces method.
+    properties:
+      workspaces:
+        type: array
+        items:
+          $ref: '#/definitions/WorkspaceSummary'
+        description: The list of workspaces.
+  ListWorkspaceBackupsQueryOptions:
+    type: object
+    description: Query options object for ListWorkspaceBackups method.
+    properties:
+      expandEnvironmentMetadata:
+        type: boolean
+        description: When set to true, will return the metadata of the environment where the backed-up workspace is/was present.
+  ListWorkspaceBackupsRequest:
+    type: object
+    description: Request object for ListWorkspaceBackups method.
     properties:
       environmentName:
         type: string
-        description: The name or CRN of the environment.
-      credentialName:
+        description: The environment for the workspace to list backups for.
+      workspaceName:
         type: string
-        description: The credential name to set for the environment. This must be a credential that already exists.
-  ChangeEnvironmentCredentialResponse:
+        description: The name of the workspace to list backups for.
+      workspaceCrn:
+        type: string
+        description: The CRN of the workspace to list backups for. If this field is specified, environmentName and workspaceName are ignored.
+      queryOptions:
+        description: Additional query options to enhance/mutate the API response.
+        $ref: '#/definitions/ListWorkspaceBackupsQueryOptions'
+  BackupDetail:
     type: object
-    description: Response object for a change environment credentials request.
-    required:
-      - environment
+    description: Backup Detail response object for listing backups.
     properties:
-      environment:
-        $ref: '#/definitions/EnvironmentSummary'
-        description: The environment summary.
-  DescribeEnvironmentRequest:
+      backupCrn:
+        type: string
+        description: The CRN of the backup snapshot.
+      backupName:
+        type: string
+        description: The name of the backup snapshot.
+      createdAt:
+        type: string
+        format: date-time
+        description: The creation time of the backup snapshot.
+      creatorCrn:
+        type: string
+        description: The CRN of the creator.
+      workspaceVersionAtBackup:
+        type: string
+        description: The version of the backed-up workspace at the time of backup.
+      backupStatus:
+        type: string
+        description: The status of the backup.
+  ListWorkspaceBackupsResponse:
     type: object
-    description: Request object for a describe environment request.
-    required:
-      - environmentName
+    description: Response object for ListWorkspaceBackups method.
     properties:
-      environmentName:
+      backups:
+        type: array
+        items:
+          $ref: '#/definitions/BackupDetail'
+        description: The list of backups along with their details.
+  UpgradeState:
+    type: object
+    description: Response object for the workspace summary.
+    properties:
+      state:
         type: string
-        description: The names or CRN of the environment.
-  DescribeEnvironmentResponse:
+        description: The current upgrade state of the workspace.
+      reason:
+        type: string
+        description: The reason for the current state.
+  BackupMetadata:
     type: object
-    description: Response object for a describe environment request.
-    required:
-      - environment
+    description: Backup metadata response object for the workspace summary.
     properties:
-      environment:
-        $ref: '#/definitions/Environment'
-        description: The environment.
-  EnvironmentSummary:
+      backupVaultName:
+        type: string
+        description: The backup vault name.
+      lastSuccessfulBackupTime:
+        type: string
+        format: date-time
+        description: The time when the last successful backup was taken.
+      isSuccessfulBackupAvailable:
+        type: boolean
+        description: Whether successful backups are available for the workspace.
+      lastBackupStatus:
+        type: string
+        description: The status of the last backup initiated.
+      numberOfAvailableBackups:
+        type: integer
+        format: int64
+        description: The number of backups available.
+  WorkspaceSummary:
     type: object
-    description: The environment summary.
+    description: A Cloudera Machine Learning workspace which includes the deployed configuration details.
     required:
+      - instanceName
       - environmentName
+      - instanceStatus
+      - instanceUrl
+      - environmentCrn
       - crn
-      - status
-      - region
+      - k8sClusterName
+      - creatorCrn
+      - version
+      - httpsEnabled
+      - filesystemID
       - cloudPlatform
-      - credentialName
+      - monitoringEnabled
     properties:
+      instanceName:
+        type: string
+        description: The name of the workspace.
       environmentName:
         type: string
-        description: Name of the environment.
-      crn:
+        description: The name of the workspace's environment.
+      instanceStatus:
+        type: string
+        description: The workspace's current status.
+      instanceUrl:
+        type: string
+        description: URL of the workspace's user interface.
+      environmentCrn:
         type: string
         description: CRN of the environment.
-      status:
+      crn:
         type: string
-        description: Status of the environment,
-      region:
+        description: The CRN of the workspace.
+      k8sClusterName:
         type: string
-        description: Region of the environment.
+        description: The Kubernetes cluster name.
+      creatorCrn:
+        type: string
+        description: The CRN of the creator of the workspace.
+      version:
+        type: string
+        description: The version of Cloudera Machine Learning that was installed on the workspace.
+      httpsEnabled:
+        type: boolean
+        description: Indicates if HTTPs communication was enabled on this workspace when provisioned.
+      filesystemID:
+        type: string
+        description: A filesystem ID referencing the filesystem that was created on the cloud provider environment that this workspace uses.
       cloudPlatform:
         type: string
-        description: Cloud platform of the environment.
-      credentialName:
+        description: The cloud platform of the environment that was used to create this workspace.
+      monitoringEnabled:
+        type: boolean
+        description: If usage monitoring is enabled or not on this workspace.
+      loadBalancerIPWhitelists:
+        type: array
+        items:
+          type: string
+        description: The whitelist of IPs for load balancer.
+      creationDate:
         type: string
-        description: Name of the credential of the environment. Must contain only lowercase letters, numbers and hyphens.
-      description:
+        format: date-time
+        description: Creation date of workspace.
+      failureMessage:
         type: string
-        description: Description of the environment.
-  Environment:
+        description: Failure message from the most recent failure that has occurred during workspace provisioning.
+      healthInfoLists:
+        type: array
+        items:
+          $ref: '#/definitions/HealthInfo'
+        description: The health info information of the workspace.
+      upgradeState:
+        description: The upgrade state contains the workspace upgrade information.
+        $ref: '#/definitions/UpgradeState'
+      nfsVersion:
+        type: string
+        description: NFS Version of the filesystem.
+      backupMetadata:
+        description: The Backup Metadata for the workspace.
+        $ref: '#/definitions/BackupMetadata'
+      clusterID:
+        type: string
+        description: The Cluster ID for the workspace.
+      isPrivate:
+        type: boolean
+        description: The value to indicate if the cluster is private or not.
+  Workspace:
     type: object
-    description: The environment.
+    description: A ML workspace, which includes the cluster and storage.
     required:
+      - instanceName
       - environmentName
+      - instanceStatus
+      - instanceUrl
+      - environmentCrn
       - crn
-      - status
-      - region
+      - k8sClusterName
+      - creatorCrn
+      - version
+      - httpsEnabled
+      - endpointPublicAccess
+      - filesystemID
+      - tags
+      - instanceGroups
       - cloudPlatform
-      - credentialName
-      - network
-      - logStorage
+      - monitoringEnabled
     properties:
+      instanceName:
+        type: string
+        description: The name of the workspace.
       environmentName:
         type: string
-        description: Name of the environment.
-      crn:
+        description: The name of the workspace's environment.
+      instanceStatus:
         type: string
-        description: CRN of the environment.
-      status:
+        description: The workspace's current status.
+      instanceUrl:
         type: string
-        description: Status of the environment.
-      region:
+        description: URL of the workspace's user interface.
+      environmentCrn:
         type: string
-        description: Region of the environment.
-      cloudPlatform:
+        description: CRN of the environment.
+      crn:
         type: string
-        description: Cloud platform of the environment.
-      credentialName:
+        description: The CRN of the workspace.
+      k8sClusterName:
         type: string
-        description: Name of the credential of the environment.
-      network:
-        description: Network related specifics of the environment.
-        $ref: '#/definitions/Network'
-      logStorage:
-        description: Storage configuration for cluster and audit logs.
-        $ref: '#/definitions/LogStorage'
-      authentication:
-        description: SSH key for accessing cluster node instances.
-        $ref: '#/definitions/Authentication'
-      securityAccess:
-        description: Security control for FreeIPA and Datalake deployment.
-        $ref: '#/definitions/SecurityAccess'
-      description:
+        description: The Kubernetes cluster name.
+      creatorCrn:
         type: string
-        description: Description of the environment
-      statusReason:
+        description: The CRN of the creator of the workspace.
+      version:
         type: string
-        description: The status reason.
-      awsDetails:
-        type: object
-        description: AWS-specific environment configuration information.
-        properties:
-          s3GuardTableName:
-            type: string
-            description: The name for the DynamoDB table backing S3Guard.
-  AuthenticationRequest:
-    type: object
-    description: Additional SSH key authentication configuration for accessing cluster node.
-    properties:
-      publicKey:
+        description: The version of Cloudera Machine Learning that was installed on the workspace.
+      httpsEnabled:
+        type: boolean
+        description: To Display if Https is enabled or not.
+      endpointPublicAccess:
+        type: boolean
+        description: To check if the cluster is publicly accessible or not.
+      filesystemID:
         type: string
-        description: Public SSH key string. Mutually exclusive with publicKeyId.
-      publicKeyId:
+        description: filesystemID used by the workspace
+      tags:
+        type: array
+        items:
+          $ref: '#/definitions/Tag'
+        description: Tags provided by the user at the time of workspace creation.
+      instanceGroups:
+        type: array
+        items:
+          $ref: '#/definitions/WorkspaceInstanceGroup'
+        description: The instance groups.
+      cloudPlatform:
         type: string
-        description: Public SSH key ID already registered in the cloud provider. Mutually exclusive with publicKey.
-  Authentication:
-    type: object
-    description: Additional SSH key authentication configuration for accessing cluster node instances.
-    properties:
-      publicKey:
+        description: The cloud platform of the environment that was used to create this workspace.
+      monitoringEnabled:
+        type: boolean
+        description: If usage monitoring is enabled or not on this workspace.
+      loadBalancerIPWhitelists:
+        type: array
+        items:
+          type: string
+        description: IP whitelist for loadBalancer.
+      creationDate:
         type: string
-        description: SSH Public key string.
-      publicKeyId:
+        format: date-time
+        description: Creation date of workspace.
+      healthInfoLists:
+        type: array
+        items:
+          $ref: '#/definitions/HealthInfo'
+        description: The health info information of the workspace.
+      failureMessage:
         type: string
-        description: Public SSH key ID already registered in the cloud provider.
-      loginUserName:
+        description: Failure message from the most recent failure that has occurred during workspace provisioning.
+      clusterBaseDomain:
         type: string
-        description: The SSH user name created on the nodes for SSH access.
-  Network:
-    type: object
-    description: The network.
-    required:
-      - networkName
-      - subnetIds
-    properties:
-      networkName:
+        description: The basedomain of the cluster.
+      modelMetricsEnabled:
+        type: boolean
+        description: Whether model metrics is enabled.
+      governanceEnabled:
+        type: boolean
+        description: Whether governance is enabled.
+      subnets:
+        type: array
+        items:
+          type: string
+        description: The subnets of the workspace.
+      whitelistAuthorizedIPRanges:
+        type: boolean
+        description: Whether to whitelist only 'authorizedIPRanges' given or all public IPs.
+      authorizedIPRanges:
+        type: array
+        items:
+          type: string
+        description: The whitelist of CIDR blocks which can access the API server.
+      nfsVersion:
         type: string
-        description: Name of the network
-      subnetIds:
+        description: NFS Version of the filesystem.
+      subnetsForLoadBalancers:
         type: array
-        description: Subnet ids of the network.
-        uniqueItems: true
         items:
           type: string
-      aws:
-        description: AWS network parameters.
-        $ref: '#/definitions/NetworkAwsParams'
-      azure:
-        description: Azure network parameters.
-        $ref: '#/definitions/NetworkAzureParams'
-      networkCidr:
-        type: string
-        description: The range of private IPv4 addresses that resources will use under this network.
-      subnetMetadata:
-        type: object
-        description: Additional subnet metadata of the network.
-        additionalProperties:
-          description: The subnet information.
-          $ref: '#/definitions/CloudSubnet'
-  CloudSubnet:
+        description: The list of subnets used for the load balancer that CML creates.
+      upgradeState:
+        description: The upgrade state contains the workspace upgrade information.
+        $ref: '#/definitions/UpgradeState'
+      backupMetadata:
+        description: The Backup MetaData for this Workspace
+        $ref: '#/definitions/BackupMetadata'
+      clusterID:
+        type: string
+        description: The Cluster ID for the workspace.
+      isPrivate:
+        type: boolean
+        description: The value to indicate if the cluster is private or not.
+  UpgradeWorkspaceRequest:
     type: object
-    description: Information about a cloud provider subnet.
+    description: Request object for the UpgradeWorkspace method.
     properties:
-      subnetId:
-        description: The id of the subnet.
+      environmentName:
         type: string
-      subnetName:
-        description: The name of the subnet.
+        description: The environment of the workspace.
+      workspaceName:
         type: string
-      availabilityZone:
-        description: The availability zone of the subnet.
+        description: The name of the workspace.
+      mlVersion:
         type: string
-      cidr:
-        description: The CIDR IP range of the subnet.
+        description: The version of workspace to upgrade to. (Deprecated).
+        x-deprecated: true
+      workspaceCrn:
         type: string
-  NetworkAwsParams:
+        description: The CRN of the workspace. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  UpgradeWorkspaceResponse:
     type: object
-    description: AWS network parameters.
-    required:
-      - vpcId
-    properties:
-      vpcId:
-        type: string
-        description: VPC ids of the specified networks.
-  NetworkAzureParams:
+    description: Response object for the UpgradeWorkspace method.
+  DescribeWorkspaceRequest:
     type: object
-    description: Azure network parameters.
-    required:
-      - networkId
-      - resourceGroupName
-      - usePublicIp
+    description: Request object for the DescribeWorkspace method.
     properties:
-      networkId:
+      environmentName:
         type: string
-        description: The id of the Azure VNet.
-      resourceGroupName:
+        description: The environment for the workspace to describe.
+      workspaceName:
         type: string
-        description: The name of the resource group associated with the VNet.
-      usePublicIp:
-        type: boolean
-        description: Whether to associate public ip's to the resources within the network.
-  DeleteEnvironmentRequest:
-    type: object
-    description: Request object for a delete environment request.
-    required:
-      - environmentName
-    properties:
-      environmentName:
+        description: The name of the workspace to describe.
+      workspaceCrn:
         type: string
-        description: The name or CRN of the environment.
-  DeleteEnvironmentResponse:
-    type: object
-    description: Response object for a delete environment request.
-  StartEnvironmentRequest:
+        description: The CRN of the workspace to describe. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  DescribeWorkspaceResponse:
     type: object
-    description: Request object for a start environment request.
+    description: Response object for the DescribeWorkspace method.
     required:
-      - environmentName
+      - workspace
     properties:
-      environmentName:
-        type: string
-        description: The name or CRN of the environment.
-  StartEnvironmentResponse:
+      workspace:
+        description: The workspace.
+        $ref: '#/definitions/Workspace'
+  DeleteInstanceGroupRequest:
     type: object
-    description: Response object for a start environment request.
-  StopEnvironmentRequest:
-    type: object
-    description: Request object for a stop environment request.
+    description: Request object for the DeleteInstanceGroup method.
     required:
-      - environmentName
+      - workspaceCrn
+      - instanceGroupName
     properties:
-      environmentName:
+      workspaceCrn:
         type: string
-        description: The name or CRN of the environment.
-  StopEnvironmentResponse:
-    type: object
-    description: Response object for a stop environment request.
-  DeleteCredentialRequest:
-    type: object
-    description: Request object for a delete credential request.
-    required:
-      - credentialName
-    properties:
-      credentialName:
+        description: The CRN of the workspace from which instance group is to be deleted.
+      instanceGroupName:
         type: string
-        description: The name or CRN of the credential.
-  DeleteCredentialResponse:
-    type: object
-    description: Response object for a delete credential request.
-  SyncAllUsersRequest:
+        description: The instance group that we want to delete from the workspace.
+  DeleteInstanceGroupResponse:
     type: object
-    description: Request object for a All Users and Groups Sync.
-    properties:
-      environmentNames:
-        type: array
-        description: List of environments to be synced. If not present, all environments will be synced.
-        items:
-          type: string
-  SyncAllUsersResponse:
+    description: Response object for the DeleteInstanceGroup method.
+  DeleteWorkspaceRequest:
     type: object
-    description: All Users and Groups Sync Response Object
+    description: Request object for the DeleteWorkspace method.
     required:
-      - operationId
+      - force
     properties:
-      operationId:
-        type: string
-        description: UUID of the request for this operation. This Id can be used for geting status on the operation.
-      operationType:
-        description: Operation type, set password or user sync
-        $ref: '#/definitions/OperationType'
-      status:
-        description: Status of this operation. Status can be one of these values (REQUESTED, RUNNING, COMPLETED, FAILED, REJECTED, TIMEDOUT)
-        $ref: '#/definitions/SyncStatus'
-      success:
-        type: array
-        description: List of sync operation details for all succeeded environments.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      failure:
-        type: array
-        description: List of sync operation details for all failed envs.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      error:
+      force:
+        type: boolean
+        description: Force delete a workspace even if errors occur during deletion. Force delete removes the guarantee that resources in your cloud account will be cleaned up.
+      removeStorage:
+        type: boolean
+        description: The remove storage flag indicates weather to keep the backing workspace filesystem storage or remove it during delete.
+      environmentName:
         type: string
-        description: If there is any error associated.
-      startTime:
+        description: The environment for the workspace to delete.
+      workspaceName:
         type: string
-        description: Sync operation start timestamp.
-      endTime:
+        description: The name of the workspace to delete.
+      workspaceCrn:
         type: string
-        description: Sync operation end timestamp.
-  SyncUserRequest:
+        description: The CRN of the workspace to delete. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  DeleteWorkspaceResponse:
     type: object
-    description: Request Object for single user sync operation.
-  SyncUserResponse:
+    description: Response object for the DeleteWorkspace method.
+  GrantWorkspaceAccessRequest:
     type: object
-    description: Response Object for single user sync operation.
-    required:
-      - operationId
+    description: Request object for the GrantWorkspaceAccess method.
     properties:
-      operationId:
+      arn:
         type: string
-        description: UUID of the request for this operation. This Id can be used for geting status on the operation.
-      operationType:
-        description: Operation type, set password or user sync
-        $ref: '#/definitions/OperationType'
-      status:
-        description: Status of this operation. Status can be one of these values (REQUESTED, RUNNING, COMPLETED, FAILED, REJECTED, TIMEDOUT)
-        $ref: '#/definitions/SyncStatus'
-      success:
-        type: array
-        description: List of sync operation details for all succeeded environments.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      failure:
-        type: array
-        description: List of sync operation details for all failed envs.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      error:
+        description: 'The aws user ARN to grant access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
+        x-deprecated: true
+      environmentName:
+        type: string
+        description: The environment that the workspace is a member of.
+      workspaceName:
         type: string
-        description: If there is any error associated.
-      startTime:
+        description: The name of the workspace to grant access to.
+      workspaceCrn:
         type: string
-        description: Sync operation start timestamp.
-      endTime:
+        description: The CRN of the workspace to grant access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+      identifier:
         type: string
-        description: Sync operation end timestamp.
-  SetPasswordRequest:
+        description: The cloud provider user id which will be granted access to the workspace's Kubernetes cluster.
+  GrantWorkspaceAccessResponse:
     type: object
-    description: Request object for set password request.
+    description: Response object for the GrantWorkspaceAccess method.
     required:
-      - password
+      - kubeconfig
     properties:
-      password:
+      kubeconfig:
         type: string
-        description: password field.
+        description: The Kubernetes config file
         x-sensitive: true
-      environmentCRNs:
-        type: array
-        description: Optional list of environment CRNs. Only the passed environments user's password will be affected. If this field is not present, all environments will be affected.
-        items:
-          type: string
-  SetPasswordResponse:
+  RevokeWorkspaceAccessRequest:
     type: object
-    description: Response object for set password request.
-    required:
-      - operationId
+    description: Request object for the RevokeWorkspace method.
     properties:
-      operationId:
+      arn:
         type: string
-        description: UUID of the request for this operation. This Id can be used for geting status on the operation.
-      operationType:
-        description: Operation type, set password or user sync
-        $ref: '#/definitions/OperationType'
-      status:
-        description: Status of this operation. Status can be one of these values (REQUESTED, RUNNING, COMPLETED, FAILED, REJECTED, TIMEDOUT)
-        $ref: '#/definitions/SyncStatus'
-      success:
-        type: array
-        description: List of sync operation details for all succeeded environments.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      failure:
-        type: array
-        description: List of sync operation details for all failed envs.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      error:
+        description: 'The aws user ARN to revoke access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
+        x-deprecated: true
+      environmentName:
         type: string
-        description: If there is any error associated.
-      startTime:
+        description: The environment that the workspace is a member of.
+      workspaceName:
         type: string
-        description: Sync operation start timestamp.
-      endTime:
+        description: The name of the workspace to revoke access to.
+      workspaceCrn:
         type: string
-        description: Sync operation end timestamp.
-  SyncStatusRequest:
+        description: The CRN of the workspace to revoke access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+      identifier:
+        type: string
+        description: The cloud provider user id which will be granted access to the workspace's Kubernetes cluster.
+  RevokeWorkspaceAccessResponse:
     type: object
-    description: Request object for Sync Status.
-    required:
-      - operationId
+    description: Response object for the RevokeWorkspaceAccess method.
+  ListWorkspaceAccessRequest:
+    type: object
+    description: Request object for the ListWorkspace method.
     properties:
-      operationId:
+      environmentName:
+        type: string
+        description: The environment that the workspace is a member of.
+      workspaceName:
+        type: string
+        description: The name of the workspace to list access.
+      workspaceCrn:
         type: string
-        description: operationId for the previously requested sync operation for user sync or password.
-  SyncStatusResponse:
+        description: The CRN of the workspace to list access. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  ListWorkspaceAccessResponse:
     type: object
-    description: Response object for Sync Operation.
+    description: Response object for the ListWorkspaceAccess method.
     required:
-      - operationId
+      - users
     properties:
-      operationId:
-        type: string
-        description: UUID of the request for this operation. This Id can be used for geting status on the operation.
-      operationType:
-        description: Operation type, set password or user sync
-        $ref: '#/definitions/OperationType'
-      status:
-        description: Status of this operation. Status can be one of these values (REQUESTED, RUNNING, COMPLETED, FAILED, REJECTED, TIMEDOUT)
-        $ref: '#/definitions/SyncStatus'
-      success:
-        type: array
-        description: List of sync operation details for all succeeded environments.
-        items:
-          $ref: '#/definitions/SyncOperationDetails'
-      failure:
+      users:
         type: array
-        description: List of sync operation details for all failed envs.
         items:
-          $ref: '#/definitions/SyncOperationDetails'
-      error:
+          type: string
+          x-sensitive: true
+        description: The list of users that have access.
+        x-sensitive: true
+  GetKubeconfigRequest:
+    type: object
+    description: Request object for the GetKubeconfig method.
+    properties:
+      environmentName:
         type: string
-        description: If there is any error associated.
-      startTime:
+        description: The environment that the workspace is a member of.
+      workspaceName:
         type: string
-        description: Sync operation start timestamp.
-      endTime:
+        description: The name of the workspace to list access.
+      workspaceCrn:
         type: string
-        description: Sync operation end timestamp.
-  GetRootCertificateRequest:
+        description: The CRN of the workspace to list access.
+  GetKubeconfigResponse:
     type: object
-    description: Request object for obtaining public certificate of an environment.
+    description: Response object for the GetKubeconfig method.
     required:
-      - environmentName
+      - kubeconfig
     properties:
-      environmentName:
+      kubeconfig:
         type: string
-        description: The name or CRN of the environment.
-  GetRootCertificateResponse:
+        description: The list of users that have access.
+        x-sensitive: true
+  GetLatestWorkspaceVersionRequest:
     type: object
-    description: Response object with base64 encoded contents of the public certificate for an environment.
-    properties:
-      contents:
-        type: string
-        description: Contents of a certificate.
-  GetIdBrokerMappingsRequest:
+    description: Request object for GetLatestWorkspaceVersion.
+  GetLatestWorkspaceVersionResponse:
     type: object
-    description: Request object for getting ID Broker mappings for an environment.
+    description: Response object for GetLatestWorkspaceVersion.
     required:
-      - environmentName
+      - version
     properties:
-      environmentName:
+      version:
         type: string
-        description: The name or CRN of the environment.
-  GetIdBrokerMappingsResponse:
+        description: The latest version of a workspace that is used when deploying Cloudera Machine Learning workspaces.
+  HealthInfo:
     type: object
-    description: Response object for getting ID Broker mappings for an environment.
+    description: Healthinfo object contains the health information of a resource.
     required:
-      - mappingsVersion
-      - dataAccessRole
-      - rangerAuditRole
+      - resourceName
+      - isHealthy
+      - updatedAt
+      - message
+      - details
     properties:
-      mappingsVersion:
-        type: integer
-        format: int64
-        description: The version of the mappings.
-      dataAccessRole:
+      resourceName:
         type: string
-        description: The cloud provider role to which data access services will be mapped (e.g. an ARN in AWS, a Resource ID in Azure).
-      rangerAuditRole:
+        description: The resource name being checked.
+      isHealthy:
+        type: boolean
+        description: The boolean that indicates the health status.
+      updatedAt:
         type: string
-        description: The cloud provider role to which services that write to Ranger audit logs will be mapped (e.g. an ARN in AWS, a Resource ID in Azure). Note that some data access services also write to Ranger audit logs; such services will be mapped to the dataAccessRole, not the rangerAuditRole.
-      baselineRole:
+        format: date-time
+        description: The timestamp for the heartbeat.
+      message:
         type: string
-        description: Deprecated. Please use rangerAuditRole instead.
-        x-deprecated: true
-      mappings:
+        description: The message to show for the health info.
+      details:
         type: array
-        description: ID Broker mappings for individual actors and groups. Does not include mappings for data access services. May be empty if no individual mappings are needed.
         items:
-          $ref: '#/definitions/IdBrokerMapping'
-  SetIdBrokerMappingsRequest:
+          type: string
+        description: The detail of the health info.
+  ModifyClusterInstanceGroupRequest:
     type: object
-    description: Request object for setting ID Broker mappings for an environment. Overwrites all existing mappings.
+    description: Request object for ModifyClusterInstanceGroup.
     required:
-      - environmentName
-      - dataAccessRole
+      - workspaceCrn
+      - instanceGroupName
+      - min
+      - max
+      - instanceType
     properties:
-      environmentName:
-        type: string
-        description: The name or CRN of the environment.
-      dataAccessRole:
+      workspaceCrn:
         type: string
-        description: The cloud provider role to which data access services will be mapped (e.g. an ARN in AWS, a Resource ID in Azure).
-      rangerAuditRole:
+        description: The CRN of the workspace cluster to modify.
+      instanceGroupName:
         type: string
-        description: The cloud provider role to which services that write to Ranger audit logs will be mapped (e.g. an ARN in AWS, a Resource ID in Azure). Note that some data access services also write to Ranger audit logs; such services will be mapped to the dataAccessRole, not the rangerAuditRole. ``THIS PARAMETER IS REQUIRED.``
-      baselineRole:
+        description: The name of the instance group of the workspace cluster to modify.
+      min:
+        type: integer
+        format: int32
+        description: The desired autoscaling min of the workspace cluster instance group.
+      max:
+        type: integer
+        format: int32
+        description: The desired autoscaling min of the workspace cluster instance group.
+      instanceType:
         type: string
-        description: Deprecated. Please use rangerAuditRole instead.
-        x-deprecated: true
-      mappings:
-        type: array
-        description: ID Broker mappings for individual actors and groups. Does not include mappings for data access services. If omitted or set to an empty list, you must also specify the ``--set-empty-mappings`` option, to confirm that you want to remove any existing individual mappings.
-        items:
-          $ref: '#/definitions/IdBrokerMappingRequest'
-      setEmptyMappings:
-        type: boolean
-        default: false
-        description: Whether to install an empty set of individual mappings, deleting any existing mappings. The ``--set-empty-mappings`` option is required if ``--mappings`` is omitted or if its value is an empty list, and disallowed otherwise.
-  SetIdBrokerMappingsResponse:
+        description: The desired instance type of the workspace cluster instance group.
+  ModifyClusterInstanceGroupResponse:
+    type: object
+    description: Response object for ModifyClusterInstanceGroup.
+  ModifyClusterSecurityRequest:
     type: object
-    description: Response object for setting ID Broker mappings for an environment.
+    description: Request object for ModifyClusterSecurity.
     required:
-      - mappingsVersion
-      - dataAccessRole
-      - rangerAuditRole
+      - workspaceCrn
+      - allowlistAuthorizedIPRanges
+      - authorizedIPRanges
     properties:
-      mappingsVersion:
-        type: integer
-        format: int64
-        description: The version of the mappings.
-      dataAccessRole:
-        type: string
-        description: The cloud provider role to which data access services will be mapped (e.g. an ARN in AWS, a Resource ID in Azure).
-      rangerAuditRole:
-        type: string
-        description: The cloud provider role to which services that write to Ranger audit logs will be mapped (e.g. an ARN in AWS, a Resource ID in Azure). Note that some data access services also write to Ranger audit logs; such services will be mapped to the dataAccessRole, not the rangerAuditRole.
-      baselineRole:
+      workspaceCrn:
         type: string
-        description: Deprecated. Please use rangerAuditRole instead.
-        x-deprecated: true
-      mappings:
+        description: The CRN of the workspace cluster to modify.
+      allowlistAuthorizedIPRanges:
+        type: boolean
+        description: Whether to allow only authorized IP ranges given or all public IPs.
+      authorizedIPRanges:
         type: array
-        description: ID Broker mappings for individual actors and groups. Does not include mappings for data access services. May be empty if no individual mappings are needed.
         items:
-          $ref: '#/definitions/IdBrokerMapping'
-  SyncIdBrokerMappingsRequest:
+          type: string
+        description: The allowlist of CIDR blocks which can access the API server.
+  ModifyClusterSecurityResponse:
     type: object
-    description: Request object for synchronizing ID Broker mappings for an environment.
+    description: Response object for ModifyClusterSecurity.
+  ModifyWorkspaceLoadBalancerRequest:
+    type: object
+    description: Request object for ModifyWorkspaceLoadBalancer.
     required:
-      - environmentName
+      - workspaceCrn
+      - loadBalancerIPAllowLists
     properties:
-      environmentName:
+      workspaceCrn:
         type: string
-        description: The name or CRN of the environment.
-  SyncIdBrokerMappingsResponse:
+        description: The CRN of the workspace cluster to modify.
+      loadBalancerIPAllowLists:
+        type: array
+        items:
+          type: string
+        description: The allowlist of CIDR blocks which can access the loadbalancer.
+  ModifyWorkspaceLoadBalancerResponse:
     type: object
-    description: Response object for synchronizing ID Broker mappings for an environment.
-  GetIdBrokerMappingsSyncStatusRequest:
+    description: Response object for ModifyWorkspaceLoadBalancer.
+  SuspendWorkspaceRequest:
     type: object
-    description: Request object for getting ID Broker mappings sync status.
+    description: Request object for SuspendWorkspace.
     required:
-      - environmentName
+      - workspaceCrn
     properties:
-      environmentName:
+      workspaceCrn:
         type: string
-        description: The name or CRN of the environment.
-  GetIdBrokerMappingsSyncStatusResponse:
+        description: The CRN of the workspace to suspend.
+  SuspendWorkspaceResponse:
     type: object
-    description: Response object for getting ID Broker mappings sync status.
-    required:
-      - syncNeeded
-      - globalStatus
-      - statuses
-    properties:
-      syncNeeded:
-        type: boolean
-        description: Whether a sync is needed to bring in-cluster mappings up-to-date.
-      globalStatus:
-        description: The overall mappings sync status for all datalake clusters in the environment.
-        $ref: '#/definitions/SyncStatus'
-      statuses:
-        type: object
-        description: Map of datalake cluster CRN to mappings sync status for each datalake cluster in the environment.
-        additionalProperties:
-          description: ID Broker sync status.
-          $ref: '#/definitions/IdBrokerSyncStatus'
-  IdBrokerMapping:
+    description: Response object for SuspendWorkspace.
+  ResumeWorkspaceRequest:
     type: object
-    description: A mapping of an actor or group to a cloud provider role.
+    description: Request object for ResumeWorkspace.
     required:
-      - accessorCrn
-      - role
+      - workspaceCrn
     properties:
-      accessorCrn:
-        type: string
-        description: The CRN of the actor or group.
-      role:
+      workspaceCrn:
         type: string
-        description: The cloud provider role (e.g., ARN in AWS, Resource ID in Azure) to which the actor or group is mapped.
-  IdBrokerMappingRequest:
+        description: The CRN of the workspace to resume.
+  ResumeWorkspaceResponse:
     type: object
-    description: A mapping of an actor or group to a cloud provider role, used in request objects.
-    required:
-      - accessorCrn
-      - role
-    properties:
-      accessorCrn:
-        type: string
-        description: The CRN of the actor or group.
-      role:
-        type: string
-        description: The cloud provider role (e.g., ARN in AWS, Resource ID in Azure) to which the actor or group is mapped.
-  IdBrokerSyncStatus:
+    description: Response object for ResumeWorkspace.
+  BackupWorkspaceRequest:
     type: object
-    description: Status of an ID Broker mappings sync operation.
+    description: The request object for workspace backup.
     required:
-      - status
+      - workspaceCrn
+      - backupName
     properties:
-      status:
-        description: The mappings sync summary status.
-        $ref: '#/definitions/SyncStatus'
-      startDate:
+      workspaceCrn:
         type: string
-        format: date-time
-        description: The date when the mappings sync started executing. Omitted if status is NEVER_RUN.
-      endDate:
-        type: string
-        format: date-time
-        description: The date when the mappings sync completed or was terminated. Omitted if status is NEVER_RUN or RUNNING.
-      errorDetail:
+        description: CRN of the workspace to backup.
+      backupName:
         type: string
-        description: The detail of the error. Omitted if status is not FAILED.
-  SyncOperationDetails:
+        description: Backup name.
+      backupJobTimeoutMinutes:
+        type: integer
+        format: int32
+        description: The timeout(in minutes) to use for the execution of the backup jobs.
+      skipValidation:
+        type: boolean
+        description: Skip pre-flight validations if requested.
+  BackupWorkspaceResponse:
     type: object
-    description: Details object of the sync operation for success or falure.
-    required:
-      - environmentCrn
+    description: The response object for workspace backup.
     properties:
-      environmentCrn:
-        description: environment crn.
+      backupCrn:
         type: string
-      message:
+        description: CRN of the backup generated.
+      vaultName:
         type: string
-        description: The detail of the success or failure.
-  SyncStatus:
-    type: string
-    description: Status of a sync operation.
-    enum:
-      - NEVER_RUN
-      - REQUESTED
-      - REJECTED
-      - RUNNING
-      - COMPLETED
-      - FAILED
-      - TIMEDOUT
-  OperationType:
-    type: string
-    description: Operation Type.
-    enum:
-      - SET_PASSWORD
-      - USER_SYNC
-  GetFreeipaStatusRequest:
+        description: Name of the vault where backup related volumes are stored.
+  DeleteBackupRequest:
     type: object
-    description: Request object for getting the status of the FreeIPA servers.
+    description: The request object for DeleteBackup operation.
     required:
-      - environmentName
+      - backupCrn
     properties:
-      environmentName:
+      backupCrn:
         type: string
-        description: The environment name or CRN of the FreeIPA to repair
-  FreeIPANodeStatus:
+        description: The CRN of the backup to be deleted.
+      skipValidation:
+        type: boolean
+        description: Skip pre-flight validations if requested.
+  DeleteBackupResponse:
     type: object
-    description: The status and issues of an individual FreeIPA node.
-    required:
-      - hostname
-      - status
+    description: The response object for DeleteBackup operation.
     properties:
-      hostname:
-        type: string
-        description: The hostname of the ipa instance.
-      status:
-        type: string
-        description: The status of the individual node
-        enum:
-          - REQUESTED
-          - CREATED
-          - UNREGISTERED
-          - REGISTERED
-          - DECOMMISSIONED
-          - TERMINATED
-          - DELETED_ON_PROVIDER_SIDE
-          - FAILED
-          - STOPPED
-          - REBOOTING
-          - UNREACHABLE
-      issues:
-        type: array
-        description: A list of issues the node is having
-        items:
-          type: string
-  GetFreeipaStatusResponse:
+      workflowId:
+        type: string
+        description: The ID of the delete-backup workflow.
+  WorkflowMetadata:
     type: object
-    description: The overall status of the FreeIPA cluster.
-    required:
-      - environmentCrn
-      - environmentName
-      - status
-      - instances
+    description: The workflow metadata.
     properties:
-      environmentCrn:
+      resourceId:
         type: string
-        description: The CRN of the environment
-      environmentName:
+        description: The unique identifier of the resource.
+      workflowIndex:
+        type: integer
+        format: int64
+        description: The workflow index. Monotonically increases for each subsequent workflow for a resource.
+      workflowType:
         type: string
-        description: The name of the Environment
-      status:
+        description: The workflow type.
+      workflowId:
         type: string
-        description: The overall status of the FreeIPA cluster
-        enum:
-          - REQUESTED
-          - CREATE_IN_PROGRESS
-          - AVAILABLE
-          - STACK_AVAILABLE
-          - UPDATE_IN_PROGRESS
-          - UPDATE_REQUESTED
-          - UPDATE_FAILED
-          - CREATE_FAILED
-          - DELETE_IN_PROGRESS
-          - DELETE_FAILED
-          - DELETE_COMPLETED
-          - STOPPED
-          - STOP_REQUESTED
-          - START_REQUESTED
-          - STOP_IN_PROGRESS
-          - START_IN_PROGRESS
-          - START_FAILED
-          - STOP_FAILED
-          - WAIT_FOR_SYNC
-          - MAINTENANCE_MODE_ENABLED
-          - UNREACHABLE
-          - UNHEALTHY
-          - DELETED_ON_PROVIDER_SIDE
-          - UNKNOWN
-      instances:
-        type: object
-        description: Status of individual nodes in the FreeIPA cluster
-        additionalProperties:
-          description: An Individual Node Status
-          $ref: '#/definitions/FreeIPANodeStatus'
-  RepairFreeipaRequest:
-    type: object
-    description: Request object for repairing the FreeIPA servers.
-    required:
-      - environmentName
-    properties:
-      environmentName:
+        description: The workflow identifier.
+      lastKnownStatus:
         type: string
-        description: The environment name or CRN of the FreeIPA to repair
-      force:
-        type: boolean
-        description: Force the repair even if the status if the FreeIPA nodes are good.
-        default: false
-      instances:
-        type: array
-        items:
-          type: string
-        description: The instance Ids to repair. If not provided then all instances are looked at for repair.
-  RepairFreeipaResponse:
-    type: object
-    description: Response object for an FreeIPA repair request.
-  AWSFreeIpaCreationRequest:
-    description: Request object for creating FreeIPA in the environment.
-    type: object
-    properties:
-      instanceCountByGroup:
-        type: integer
-        format: int32
-        description: The number of FreeIPA instances to create per group when creating FreeIPA in the environment
-  AzureFreeIpaCreationRequest:
-    description: Request object for creating FreeIPA in the environment.
+        description: The last known status of the workflow.
+  RequestWorkflowCancellationRequest:
     type: object
+    description: Request object for RequestWorkflowCancellation.
     properties:
-      instanceCountByGroup:
-        type: integer
-        format: int32
-        description: The number of FreeIPA instances to create per group when creating FreeIPA in the environment
-  TagRequest:
-    description: A label that can be attached to some resources.
-    type: object
-    required:
-      - key
-      - value
-    properties:
-      key:
+      resourceId:
         type: string
-        description: The tag's name.
-      value:
+        description: The unique identifier of the resource.
+      workflowType:
         type: string
-        description: The associated value of the tag.
+        description: The workflow type.
+  RequestWorkflowCancellationResponse:
+    type: object
+    description: Response object for RequestWorkflowCancellation.
+    properties:
+      workflowMetadata:
+        type: array
+        items:
+          $ref: '#/definitions/WorkflowMetadata'
+        description: The list of workflow metedata for cancelled workflows.
+x-audit: true
```

### Comparing `cdpcli-0.9.9/cdpcli/formatter.py` & `cdpcli-0.9.90/cdpcli/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,19 @@
 
     def _format_response(self, command_name, response, stream):
         # For operations that have no response body (e.g. s3 put-object)
         # the response will be an empty string.  We don't want to print
         # that out to the user but other "falsey" values like an empty
         # dictionary should be printed.
         if response != {}:
+            ensure_ascii = self._args.ensure_ascii
+            if ensure_ascii is None:
+                ensure_ascii = False
             json.dump(response, stream, indent=4, default=json_encoder,
-                      ensure_ascii=False)
+                      ensure_ascii=ensure_ascii)
             stream.write('\n')
 
 
 class TableFormatter(FullyBufferedFormatter):
     """Pretty print a table from a given response.
 
     The table formatter is able to take any generic response
```

### Comparing `cdpcli-0.9.9/cdpcli/completer.py` & `cdpcli-0.9.90/cdpcli/completer.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,21 +72,22 @@
         if current_arg != subcmd_name and current_arg.startswith('-'):
             return self._find_possible_options(current_arg, opts, subcmd_help)
         return []
 
     def _complete_option(self, option_name):
         if option_name == '--endpoint-url':
             return []
-        if option_name == '--cdp-endpoint-url':
-            return []
-        if option_name == '--output':
-            cli_data = self.driver.session.get_data('cli')
-            return cli_data['options']['output']['choices']
         if option_name == '--profile':
-            return self.driver.session.available_profiles
+            return []
+        cli_data_options = getattr(self.driver, '_cli_data', {}).get('options', {})
+        enum_option_names = ['--' + name
+                             for name, option in cli_data_options.items()
+                             if 'choices' in option]
+        if option_name in enum_option_names:
+            return cli_data_options[option_name.lstrip('-')]['choices']
         return []
 
     def _complete_provider(self, current_arg, opts):
         if current_arg.startswith('-'):
             return self._find_possible_options(current_arg, opts)
         elif current_arg == 'cdp':
             return self._get_documented_completions(
```

### Comparing `cdpcli-0.9.9/cdpcli/clicommand.py` & `cdpcli-0.9.90/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/schema.py` & `cdpcli-0.9.90/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/cdpcli/signers.py` & `cdpcli-0.9.90/cdpcli/signers.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,12 +48,12 @@
         cls = cdpcli.auth.AUTH_TYPE_MAPS.get(signature_version)
         if cls is None:
             raise UnknownSignatureVersionError(
                 signature_version=signature_version)
         # If there's no credentials provided (i.e credentials is None),
         # then we'll pass a value of "None" over to the auth classes,
         # which already handle the cases where no credentials have
-        # been provided.
+        # been provided (by failing ...).
         frozen_credentials = self._credentials.get_frozen_credentials()
         kwargs['credentials'] = frozen_credentials
         auth = cls(**kwargs)
         return auth
```

### Comparing `cdpcli-0.9.9/cdpcli/__init__.py` & `cdpcli-0.9.90/cdpcli/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,21 +16,30 @@
 
 import os
 import re
 
 from ._version import get_versions
 
 
+# Retrieve the version number from versioneer's code.
 __version__ = get_versions()['version']
 del get_versions
 
 VERSION = __version__
 
 CDPCLI_ROOT = os.path.dirname(os.path.abspath(__file__))
 
+# Read in the release file and update the advertised version with it if it's
+# not the default / PUBLIC release.
+_release_file_path = os.path.normpath("{0}/data/release.txt".format(CDPCLI_ROOT))
+with open(_release_file_path) as releaseFile:
+    RELEASE = releaseFile.readline()
+
+if RELEASE != 'PUBLIC':
+    VERSION += ' (%s)' % RELEASE
 
 # Used to specify anonymous (unsigned) request signature
 UNSIGNED = object()
 
 
 SCALAR_TYPES = set(['string',
                     'float',
@@ -52,14 +61,19 @@
 COMPLEX_TYPES = set([OBJECT_TYPE,
                      LIST_TYPE,
                      MAP_TYPE])
 
 DEFAULT_PROFILE_NAME = 'default'
 CDP_ACCESS_KEY_ID_KEY_NAME = 'cdp_access_key_id'
 CDP_PRIVATE_KEY_KEY_NAME = 'cdp_private_key'
+CDP_ACCESS_TOKEN_KEY_NAME = 'cdp_access_token'
+CDP_REGION_KEY_NAME = 'cdp_region'
+CDP_ENDPOINT_URL_KEY_NAME = 'cdp_endpoint_url'
+ENDPOINT_URL_KEY_NAME = 'endpoint_url'
+FORM_FACTOR_KEY_NAME = 'form_factor'
 # Python argparse has a bug in which '-' are not parsed correctly if they appear
 # as values for other arguments, see: http://bugs.python.org/issue9334 for more
 # details. This defines special encoding for dash that we will "decode" and
 # replace with a dash. The reason we are using \\ is that there is a non zero
 # chance that customers can discover this themselves.
 ARGPARSE_DASH_ENCODING = '\\-'
```

### Comparing `cdpcli-0.9.9/cdpcli/paramfile.py` & `cdpcli-0.9.90/cdpcli/paramfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 #
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
+
 import os
 
 from cdpcli.compat import compat_open
 from cdpcli.compat import six
-from cdpcli.thirdparty import requests
+import requests
 
 
 class ResourceLoadingError(Exception):
     pass
 
 
-def get_paramfile(path):
+def get_paramfile(path, parsed_globals):
     """Load parameter based on a resource URI.
 
     It is possible to pass parameters to operations by referring
     to files or URI's.  If such a reference is detected, this
     function attempts to retrieve the data from the file or URI
     and returns it.  If there are any errors or if the ``path``
     does not appear to refer to a file or URI, a ``None`` is
@@ -36,36 +37,44 @@
 
     """
     data = None
     if isinstance(path, six.string_types):
         for prefix, function_spec in PREFIX_MAP.items():
             if path.startswith(prefix):
                 function, kwargs = function_spec
+                kwargs['parsed_globals'] = parsed_globals
                 data = function(prefix, path, **kwargs)
     return data
 
 
-def get_file(prefix, path, mode):
+def get_file(prefix, path, mode, parsed_globals):
     file_path = os.path.expandvars(os.path.expanduser(path[len(prefix):]))
     try:
         with compat_open(file_path, mode) as f:
             return f.read()
     except UnicodeDecodeError:
         raise ResourceLoadingError(
             'Unable to load paramfile (%s), text contents could '
             'not be decoded.  If this is a binary file, please use the '
             'fileb:// prefix instead of the file:// prefix.' % file_path)
     except (OSError, IOError) as e:
         raise ResourceLoadingError('Unable to load paramfile %s: %s' % (
             path, e))
 
 
-def get_uri(prefix, uri):
+def get_uri(prefix, uri, parsed_globals):
     try:
-        r = requests.get(uri)
+        # The TLS verification value can be a boolean or a CA_BUNDLE path. This
+        # is a little odd, but ultimately comes from the python HTTP requests
+        # library we're using.
+        tls_verification = getattr(parsed_globals, 'verify_tls', True)
+        ca_bundle = getattr(parsed_globals, 'ca_bundle', None)
+        if tls_verification and ca_bundle is not None:
+            tls_verification = ca_bundle
+        r = requests.get(uri, verify=tls_verification)
         if r.status_code == 200:
             return r.text
         else:
             raise ResourceLoadingError(
                 "received non 200 status code of %s" % (
                     r.status_code))
     except Exception as e:
@@ -77,14 +86,17 @@
     'fileb://': (get_file, {'mode': 'rb'}),
     'http://': (get_uri, {}),
     'https://': (get_uri, {}),
 }
 
 
 class ParamFileVisitor(object):
+    def __init__(self, parsed_globals):
+        self._parsed_globals = parsed_globals
+
     """
     This visitor's visit method will walk the input params object of the input
     shape, visiting all fields and recursing through complex fields. Any string
     field encountered will get paramfile resolution unless it is marked in the
     model as being x-no-paramfile.
     """
 
@@ -123,22 +135,34 @@
     def _visit_float(self, param, shape, name):
         return param
 
     def _visit_double(self, param, shape, name):
         return param
 
     def _visit_string(self, param, shape, name):
+        if not getattr(self._parsed_globals, 'expand_param', True):
+            return param
         if shape.is_no_paramfile:
             return param
-        override = get_paramfile(param)
+        override = get_paramfile(param, self._parsed_globals)
         if override is not None:
             return override
         return param
 
     def _visit_array(self, param, shape, name):
         visited = []
         for i, item in enumerate(param):
             visited.append(self._visit(item, shape.member, '%s[%s]' % (name, i)))
         return visited
 
     def _visit_datetime(self, param, shape, name):
         return param
+
+    def _visit_blob(self, param, shape, name):
+        if not getattr(self._parsed_globals, 'expand_param', True):
+            return param
+        if shape.is_no_paramfile:
+            return param
+        override = get_paramfile(param, self._parsed_globals)
+        if override is not None:
+            return override
+        return param
```

### Comparing `cdpcli-0.9.9/cdpcli/argprocess.py` & `cdpcli-0.9.90/cdpcli/argprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import os
-
 from cdpcli import COMPLEX_TYPES
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli import SCALAR_TYPES
 from cdpcli import shorthand
 from cdpcli.compat import json
@@ -58,33 +56,35 @@
         super(ParamUnknownKeyError, self).__init__(full_message)
 
 
 class TooComplexError(Exception):
     pass
 
 
-def unpack_argument(cli_argument, value):
-    override = uri_param(cli_argument, value)
+def unpack_argument(cli_argument, value, parsed_globals):
+    override = uri_param(cli_argument, value, parsed_globals)
     if override is not None:
         value = override
     return value
 
 
-def uri_param(cli_argument, value):
-    if getattr(cli_argument, 'no_paramfile', None):
+def uri_param(cli_argument, value, parsed_globals):
+    if not getattr(parsed_globals, 'expand_param', True):
+        return
+    elif getattr(cli_argument, 'no_paramfile', None):
         return
     else:
-        return _check_for_uri_param(cli_argument, value)
+        return _check_for_uri_param(cli_argument, value, parsed_globals)
 
 
-def _check_for_uri_param(param, value):
+def _check_for_uri_param(param, value, parsed_globals):
     if isinstance(value, list) and len(value) == 1:
         value = value[0]
     try:
-        return get_paramfile(value)
+        return get_paramfile(value, parsed_globals)
     except ResourceLoadingError as e:
         raise ParamError(param.cli_name, six.text_type(e))
 
 
 def unpack_cli_arg(cli_argument, value):
     """
     Parses and unpacks the encoded string command line parameter
@@ -156,22 +156,14 @@
     # Note the cli_name is used strictly for error reporting.  It's
     # not required to use unpack_scalar_cli_arg
     if argument_model.type_name == 'integer' or argument_model.type_name == 'long':
         return int(value)
     elif argument_model.type_name == 'float' or argument_model.type_name == 'double':
         # TODO: losing precision on double types
         return float(value)
-    elif argument_model.type_name == 'blob' and \
-            argument_model.serialization.get('streaming'):
-        file_path = os.path.expandvars(value)
-        file_path = os.path.expanduser(file_path)
-        if not os.path.isfile(file_path):
-            msg = 'Blob values must be a path to a file.'
-            raise ParamError(cli_name, msg)
-        return open(file_path, 'rb')
     elif argument_model.type_name == 'boolean':
         if isinstance(value, six.string_types) and value.lower() == 'false':
             return False
         return bool(value)
     else:
         return value
 
@@ -335,15 +327,16 @@
 
         # Otherwise we fall back to the normal docgen for shorthand
         # syntax.
         stack = []
         try:
             if argument_model.type_name == LIST_TYPE:
                 argument_model = argument_model.member
-                return self._shorthand_docs(argument_model, stack) + ' ...'
+                return self._shorthand_docs(argument_model, stack) + \
+                    ' ... (separate items with spaces)'
             else:
                 return self._shorthand_docs(argument_model, stack)
         except TooComplexError:
             return ''
 
     def _handle_special_cases(self, cli_name, model):
         if model.type_name == LIST_TYPE and \
```

### Comparing `cdpcli-0.9.9/tests/unit/cdp/__init__.py` & `cdpcli-0.9.90/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-0.9.90/tests/unit/extensions/test_cliinputjson.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,78 +62,90 @@
         add_cli_input_json(self.operation_model, argument_table)
         arg_handler = argument_table['cli-input-json']
         self.assertIsNotNone(arg_handler)
         self.assertTrue(isinstance(arg_handler, CliInputJSONArgument))
 
     def test_add_to_call_parameters_no_file(self):
         parsed_args = mock.Mock()
+        parsed_globals = mock.Mock()
         # Make the value a JSON string
         parsed_args.cli_input_json = self.input_json
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file(self):
         parsed_args = mock.Mock()
+        parsed_globals = mock.Mock()
         # Make the value a file with JSON located inside.
         parsed_args.cli_input_json = 'file://' + self.temp_file
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file_from_visitor(self):
         temp_file1 = os.path.join(self.temp_dir, 'foo.json')
         with open(temp_file1, 'w') as f:
             f.write("baz")
         temp_file1 = _make_file_uri(temp_file1)
         temp_file2 = os.path.join(self.temp_dir, 'bar.json')
         with open(temp_file2, 'w') as f:
             f.write('{"A": "foo", "B": "file://%s"}' % temp_file1)
         temp_file2 = _make_file_uri(temp_file2)
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = 'file://' + temp_file2
+        parsed_globals = mock.Mock()
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'baz'})
 
     def test_add_to_call_parameters_bad_json(self):
         parsed_args = mock.Mock()
         # Create a bad JSON input
         parsed_args.cli_input_json = self.input_json + ','
+        parsed_globals = mock.Mock()
         call_parameters = {}
         with self.assertRaises(ParamError):
             self.argument.add_to_call_parameters(
                 call_parameters=call_parameters,
-                parsed_args=parsed_args
+                parsed_args=parsed_args,
+                parsed_globals=parsed_globals
             )
 
     def test_add_to_call_parameters_no_clobber(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = self.input_json
+        parsed_globals = mock.Mock()
         # The value for ``A`` should not be clobbered by the input JSON
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         self.assertEqual(call_parameters, {'A': 'baz', 'B': 'bar'})
 
     def test_no_add_to_call_parameters(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = None
+        parsed_globals = mock.Mock()
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args
+            parsed_args=parsed_args,
+            parsed_globals=parsed_globals
         )
         # Nothing should have been added to the call parameters because
         # ``cli_input_json`` is not in the ``parsed_args``
         self.assertEqual(call_parameters, {'A': 'baz'})
```

### Comparing `cdpcli-0.9.9/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-0.9.90/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/extensions/test_paginate.py` & `cdpcli-0.9.90/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/extensions/test_writer.py` & `cdpcli-0.9.90/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/extensions/__init__.py` & `cdpcli-0.9.90/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/extensions/configure/test_configure.py` & `cdpcli-0.9.90/tests/unit/extensions/configure/test_configure.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
+                   CDP_PRIVATE_KEY_KEY_NAME, \
+                   CDP_REGION_KEY_NAME
 from cdpcli.compat import six
 from cdpcli.endpoint import EndpointResolver
 from cdpcli.extensions.configure import configure
 from cdpcli.extensions.configure import ConfigValue
 from cdpcli.extensions.configure import CREDENTIAL_FILE_COMMENT
 from cdpcli.extensions.configure import NOT_SET
 import mock
@@ -30,17 +32,18 @@
 
 class TestConfigureCommand(unittest.TestCase):
 
     def setUp(self):
         self.writer = mock.Mock()
         self.global_args = mock.Mock()
         self.global_args.profile = None
-        self.global_args.endpoint_url = None
-        self.global_args.cdp_endpoint_url = None
-        self.precanned = PrecannedPrompter(value='new_value')
+        self.precanned = PrecannedPrompter(access_key_id='new_access_key_id',
+                                           private_key='new_private_key',
+                                           cdp_region=None,
+                                           cdp_endpoint_url=None)
         self.context = FakeContext({'config_file': 'myconfigfile'})
         self.configure = configure.ConfigureCommand(prompter=self.precanned,
                                                     config_writer=self.writer)
 
     def assert_credentials_file_updated_with(self,
                                              new_values,
                                              config_file_comment=None):
@@ -52,80 +55,59 @@
                                    expected_creds_file,
                                    config_file_comment=config_file_comment))
 
     def test_configure_command_sends_values_to_writer(self):
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Credentials are always written to the shared credentials file.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
 
         # Non-credentials config is written to the config file.
         self.writer.update_config.assert_called_with(
             {}, 'myconfigfile')
 
-    def test_configure_command_with_endpoint_url(self):
-        self.global_args.endpoint_url = "http://foo.com"
-        self.configure(self.context, args=[], parsed_globals=self.global_args)
-        # Credentials are always written to the shared credentials file.
-        self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
-            config_file_comment=CREDENTIAL_FILE_COMMENT)
-
-        # Non-credentials config is written to the config file.
-        self.writer.update_config.assert_called_with(
-            {EndpointResolver.ENDPOINT_URL_KEY_NAME: "http://foo.com"}, 'myconfigfile')
-
-    def test_configure_command_with_cdp_endpoint_url(self):
-        self.global_args.cdp_endpoint_url = "http://foo.com"
-        self.configure(self.context, args=[], parsed_globals=self.global_args)
-        # Credentials are always written to the shared credentials file.
-        self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
-            config_file_comment=CREDENTIAL_FILE_COMMENT)
-
-        # Non-credentials config is written to the config file.
-        self.writer.update_config.assert_called_with(
-            {EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://foo.com"},
-            'myconfigfile')
-
-    def test_configure_command_with_both_endpoint_urls(self):
-        self.global_args.endpoint_url = "http://foo.com"
-        self.global_args.cdp_endpoint_url = "http://bar.com"
+    def test_configure_command_with_new_values(self):
+        self.precanned = PrecannedPrompter(access_key_id='new_access_key_id',
+                                           private_key='new_private_key',
+                                           cdp_region='us-west-2',
+                                           cdp_endpoint_url='http://foo.com')
+        self.configure = configure.ConfigureCommand(prompter=self.precanned,
+                                                    config_writer=self.writer)
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Credentials are always written to the shared credentials file.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
 
         # Non-credentials config is written to the config file.
         self.writer.update_config.assert_called_with(
-            {EndpointResolver.ENDPOINT_URL_KEY_NAME: "http://foo.com",
-             EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://bar.com"},
+            {CDP_REGION_KEY_NAME: "us-west-2",
+             EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://foo.com"},
             'myconfigfile')
 
     def test_same_values_are_not_changed(self):
         # If the user enters the same value as the current value, we don't need
         # to write anything to the config.
         self.configure = configure.ConfigureCommand(prompter=EchoPrompter(),
                                                     config_writer=self.writer)
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         self.assertFalse(self.writer.update_config.called)
 
     def test_none_values_are_not_changed(self):
         # If a user hits enter, this will result in a None value which means
         # don't change the existing values.  In this case, we don't need
         # to write anything out to the config.
-        user_presses_enter = None
-        precanned = PrecannedPrompter(value=user_presses_enter)
-        self.configure = configure.ConfigureCommand(prompter=precanned,
+        self.precanned = PrecannedPrompter(access_key_id=None,
+                                           private_key=None,
+                                           cdp_region=None,
+                                           cdp_endpoint_url=None)
+        self.configure = configure.ConfigureCommand(prompter=self.precanned,
                                                     config_writer=self.writer)
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         self.assertFalse(self.writer.update_config.called)
 
     def test_create_configure_cmd(self):
         self.configure = configure.ConfigureCommand()
         self.assertIsInstance(self.configure, configure.ConfigureCommand)
@@ -133,16 +115,16 @@
     def test_section_name_can_be_changed_for_profiles(self):
         # If the user specifies "--profile myname" we need to write
         # this out to the [profile myname] section.
         self.global_args.profile = 'myname'
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Note the __section__ key name.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value',
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key',
              '__section__': 'myname'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
         self.writer.update_config.assert_called_with(
             {'__section__': 'profile myname'}, 'myconfigfile')
 
     def test_context_says_profile_does_not_exist(self):
         # Whenever you try to get a config value from botocore,
@@ -152,16 +134,16 @@
         context = FakeContext({'config_file': 'myconfigfile'},
                               profile_does_not_exist=True)
         self.configure = configure.ConfigureCommand(prompter=self.precanned,
                                                     config_writer=self.writer)
         self.global_args.profile = 'profile-does-not-exist'
         self.configure(context, args=[], parsed_globals=self.global_args)
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_value',
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key',
              '__section__': 'profile-does-not-exist'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
         self.writer.update_config.assert_called_with(
             {'__section__': 'profile profile-does-not-exist'}, 'myconfigfile')
 
 
 class TestInteractivePrompter(unittest.TestCase):
@@ -213,15 +195,15 @@
         self.assertRegexpMatches(prompt_text, r'\[\*\*\*\*.*\]')
 
     def test_non_secret_keys_are_not_masked(self):
         prompter = configure.InteractivePrompter()
         prompter.get_value(
             current_value='mycurrentvalue', config_name='not_a_secret_key',
             prompt_text='Enter value')
-        # We should also not display the entire priate key.
+        # We should display the entire non-secret key.
         prompt_text = self.stdout.getvalue()
         self.assertIn('mycurrentvalue', prompt_text)
         self.assertRegexpMatches(prompt_text, r'\[mycurrentvalue\]')
 
     def test_user_hits_enter_returns_none(self):
         # If a user hits enter, then raw_input returns the empty string.
         self.mock_raw_input.return_value = ''
@@ -270,27 +252,30 @@
         self.assertEqual(no_config.value, NOT_SET)
         no_config.mask_value()
         self.assertEqual(no_config.value, NOT_SET)
 
 
 class PrecannedPrompter(object):
 
-    def __init__(self, value):
-        self._value = value
+    def __init__(self, access_key_id, private_key, cdp_region, cdp_endpoint_url):
+        self._access_key_id = access_key_id
+        self._private_key = private_key
+        self._cdp_region = cdp_region
+        self._cdp_endpoint_url = cdp_endpoint_url
 
-    def get_value(self, current_value, logical_name, prompt_text=''):
-        return self._value
+    def get_value(self, current_value, config_name, prompt_text=''):
+        if config_name == CDP_ACCESS_KEY_ID_KEY_NAME:
+            return self._access_key_id
+        elif config_name == CDP_PRIVATE_KEY_KEY_NAME:
+            return self._private_key
+        elif config_name == CDP_REGION_KEY_NAME:
+            return self._cdp_region
+        elif config_name == EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME:
+            return self._cdp_endpoint_url
+        else:
+            return None
 
 
 class EchoPrompter(object):
 
-    def get_value(self, current_value, logical_name, prompt_text=''):
-        return current_value
-
-
-class KeyValuePrompter(object):
-
-    def __init__(self, mapping):
-        self.mapping = mapping
-
     def get_value(self, current_value, config_name, prompt_text=''):
-        return self.mapping.get(prompt_text)
+        return current_value
```

### Comparing `cdpcli-0.9.9/tests/unit/extensions/configure/test_list.py` & `cdpcli-0.9.90/tests/unit/extensions/configure/test_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,132 +10,147 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
+                   CDP_PRIVATE_KEY_KEY_NAME, \
+                   CDP_REGION_KEY_NAME
 from cdpcli.compat import six
 from cdpcli.extensions.configure.list import ConfigureListCommand
 import mock
 from tests import unittest
 from tests.unit import FakeContext
 
 
 class TestConfigureListCommand(unittest.TestCase):
 
     def test_configure_list_command_nothing_set(self):
         # Test the case where the user only wants to change a single_value.
         context = FakeContext(
             all_variables={'config_file': '/config/location'})
         context.full_config = {
-            'profiles': {'default': {'region': 'CDP_REGION'}}}
+            'profiles': {'default': {}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
-        self.assertRegexpMatches(rendered, 'profile\s+<not set>')
-        self.assertRegexpMatches(rendered, 'access_key\s+<not set>')
-        self.assertRegexpMatches(rendered, 'private_key\s+<not set>')
+        self.assertRegexpMatches(rendered, 'profile\\s+<not set>')
+        self.assertRegexpMatches(rendered, 'cdp_region\\s+<not set>')
+        self.assertRegexpMatches(rendered, 'cdp_access_key_id\\s+<not set>')
+        self.assertRegexpMatches(rendered, 'cdp_private_key\\s+<not set>')
 
     def test_configure_from_env(self):
         env_vars = {
             'profile': 'myprofilename'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             environment_vars=env_vars)
         context.context_var_map = {'profile': (None, "PROFILE_ENV_VAR")}
         context.full_config = {
-            'profiles': {'default': {'region': 'CDP_REGION'}}}
+            'profiles': {'default': {}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\s+myprofilename\s+env\s+PROFILE_ENV_VAR')
+            rendered, 'profile\\s+myprofilename\\s+env\\s+PROFILE_ENV_VAR')
 
     def test_configure_from_config_file(self):
-        # this is not a known configuration so this is ignored.
         config_file_vars = {
+            # this is not a known configuration so this is ignored.
             'foo': 'bar',
+            CDP_REGION_KEY_NAME: 'eu-1',
             CDP_ACCESS_KEY_ID_KEY_NAME: 'key_id',
             CDP_PRIVATE_KEY_KEY_NAME: 'mysecretkey'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             config_file_vars=config_file_vars)
-        context.context_var_map = {'region': ('region', "CDP_REGION")}
+        context.context_var_map = {'region': ()}
         context.full_config = {
-            'profiles': {'default': {'region': 'CDP_REGION'}}}
+            'profiles': {'default': {}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\s+<not set>\s+None\s+None')
+            rendered, 'profile\\s+<not set>\\s+None\\s+None')
         self.assertRegexpMatches(
-            rendered, r'access_key\s+\*+y_id\s+config-file')
+            rendered, 'cdp_region\\s+eu-1\\s+config-file')
         self.assertRegexpMatches(
-            rendered, r'private_key\s+\*+tkey\s+config-file')
+            rendered, 'cdp_access_key_id\\s+\\*+y_id\\s+config-file')
+        self.assertRegexpMatches(
+            rendered, 'cdp_private_key\\s+\\*+tkey\\s+config-file')
 
     def test_configure_from_multiple_sources(self):
         # Here the profile is from an env var, the
         # region is from the config file, and the credentials
         # are from an iam-role.
         env_vars = {
             'profile': 'myprofilename'
         }
+        config_file_vars = {
+            CDP_REGION_KEY_NAME: 'eu-1'
+        }
         credentials = mock.Mock()
         credentials.access_key_id = 'access_key'
         credentials.private_key = 'private_key'
+        credentials.access_token = None
         credentials.method = 'foobar'
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             environment_vars=env_vars,
-            config_file_vars={},
+            config_file_vars=config_file_vars,
             credentials=credentials)
         context.context_var_map = {
-            'region': ('region', 'CDP_REGION'),
             'profile': ('profile', 'CDP_DEFAULT_PROFILE')}
         context.full_config = {
-            'profiles': {'default': {'region': 'CDP_REGION'}}}
+            'profiles': {'default': {}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         # The profile came from an env var.
         self.assertRegexpMatches(
-            rendered, 'profile\s+myprofilename\s+env\s+CDP_DEFAULT_PROFILE')
+            rendered, 'profile\\s+myprofilename\\s+env\\s+CDP_DEFAULT_PROFILE')
+        # The cdp_region came from config file.
+        self.assertRegexpMatches(
+            rendered, 'cdp_region\\s+eu-1\\s+config-file')
         # The credentials came from 'foobar'.  Note how we're
         # also checking that the access_key/private_key are masked
         # with '*' chars except for the last 4 chars.
         self.assertRegexpMatches(
-            rendered, r'access_key\s+\*+_key\s+foobar')
+            rendered, r'cdp_access_key_id\s+\*+_key\s+foobar')
         self.assertRegexpMatches(
-            rendered, r'private_key\s+\*+_key\s+foobar')
+            rendered, r'cdp_private_key\s+\*+_key\s+foobar')
 
     def test_profile_set_in_context(self):
-        # this is not a known configuration so this is ignored.
         config_file_vars = {
+            # this is not a known configuration so this is ignored.
             'foo': 'bar',
+            CDP_REGION_KEY_NAME: 'eu-1',
             CDP_ACCESS_KEY_ID_KEY_NAME: 'key_id',
             CDP_PRIVATE_KEY_KEY_NAME: 'mysecretkey'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             config_file_vars=config_file_vars)
         context.profile = 'dev'
-        context.context_var_map = {'region': ('region', "CDP_REGION")}
+        context.context_var_map = {}
         context.full_config = {
-            'profiles': {'dev': {'region': 'CDP_REGION'}}}
+            'profiles': {'dev': {}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\s+dev\s+manual\s+--profile')
+            rendered, 'profile\\s+dev\\s+manual\\s+--profile')
+        self.assertRegexpMatches(
+            rendered, 'cdp_region\\s+eu-1\\s+config-file')
         self.assertRegexpMatches(
-            rendered, r'access_key\s+\*+y_id\s+config-file')
+            rendered, r'cdp_access_key_id\s+\*+y_id\s+config-file')
         self.assertRegexpMatches(
-            rendered, r'private_key\s+\*+tkey\s+config-file')
+            rendered, r'cdp_private_key\s+\*+tkey\s+config-file')
```

### Comparing `cdpcli-0.9.9/tests/unit/extensions/configure/test_set.py` & `cdpcli-0.9.90/tests/unit/extensions/configure/test_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
+                   CDP_ACCESS_TOKEN_KEY_NAME, \
+                   CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.extensions.configure.set import ConfigureSetCommand
 import mock
 from tests import unittest
 from tests.unit import FakeContext
 
 
 class TestConfigureSetCommand(unittest.TestCase):
@@ -112,15 +114,33 @@
         set_command(self.context,
                     args=[CDP_PRIVATE_KEY_KEY_NAME, 'foo'],
                     parsed_globals=None)
         self.config_writer.update_config.assert_called_with(
             {'__section__': 'default',
              CDP_PRIVATE_KEY_KEY_NAME: 'foo'}, self.fake_credentials_filename)
 
+    def test_access_token_written_to_shared_credentials_file(self):
+        set_command = ConfigureSetCommand(self.config_writer)
+        set_command(self.context,
+                    args=[CDP_ACCESS_TOKEN_KEY_NAME, 'foo'],
+                    parsed_globals=None)
+        self.config_writer.update_config.assert_called_with(
+            {'__section__': 'default',
+             CDP_ACCESS_TOKEN_KEY_NAME: 'foo'}, self.fake_credentials_filename)
+
     def test_access_key_written_to_shared_credentials_file_profile(self):
         set_command = ConfigureSetCommand(self.config_writer)
         set_command(self.context,
                     args=['profile.foo.cdp_access_key_id', 'bar'],
                     parsed_globals=None)
         self.config_writer.update_config.assert_called_with(
             {'__section__': 'foo',
              CDP_ACCESS_KEY_ID_KEY_NAME: 'bar'}, self.fake_credentials_filename)
+
+    def test_configure_set_command_access_key_v3(self):
+        set_command = ConfigureSetCommand(self.config_writer)
+        set_command(self.context,
+                    args=[CDP_PRIVATE_KEY_KEY_NAME, 'foo\nbar'],
+                    parsed_globals=None)
+        self.config_writer.update_config.assert_called_with(
+            {'__section__': 'default',
+             CDP_PRIVATE_KEY_KEY_NAME: 'foo\\nbar'}, self.fake_credentials_filename)
```

### Comparing `cdpcli-0.9.9/tests/unit/extensions/configure/test_get.py` & `cdpcli-0.9.90/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/test_auth.py` & `cdpcli-0.9.90/tests/unit/test_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,27 +21,32 @@
 from cdpcli.compat import HTTPHeaders
 from cdpcli.compat import json
 from cdpcli.compat import urlsplit
 import cdpcli.credentials
 from cdpcli.exceptions import NoCredentialsError
 import mock
 from tests import unittest
-from tests.unit import ED25519_KEY, RSA_KEY
+from tests.unit import ECDSA_KEY, ED25519_KEY, RSA_KEY
 
 
 EXPECTED_RSA_SIG = \
     'VLlOczaMiHdAHfW7-0axYWAxpFPqHR2sR22XRh98AlVTBjj8QJTModpzNUQxb1N0F94pMP6U' \
     'BI-flm-rl3vHJaRBfcWbaDglD02YcuqD87CmOIpZ6Z3TUTbkOcxTsMSkgOaPqQkO1p49WRl3' \
     'P_v3Q9z5y6Mh7ZDbQeonQcagKhoIYQnCXYrEmAAHhTGwuxanuAsPu2y8svUBKNd9fXZ7stQ0' \
     'Pom2J2aQZnegBM6I_QJICP7ZEd0Roga0AcGoL1OsZo_fANkUV9eUvtw8CfTw11G2c1YS__pq' \
     'PVuW4iPSYONoUN5NrL6x3RtGOea0Xo__9B5ki0_TLsYMyhF37it6qA=='
 
 EXPECTED_ED25519_SIG = \
     'et_Ueu_w3QuQbqvDdwy9aT8HLzsXBdJfRRRHe4fEK_RZ-qR-xvM35XG8J8q-YMz70GunK82JoSt5ztz0lAuCBg=='  # noqa
 
+EXPECTED_ECDSA_SIG = \
+    'MIGIAkIBPOgngVp4-uyWzLTCKcsCBeYezoedjN-Tj2KI78aIn6huJEJwG-6ZiVcEyO-mI1wN' \
+    'tbVu7H-iQDMPFKyBdpezjxYCQgEY32q1WTQUPHj_JNYN33QhCMPjJHIaBcHTdMp0SO3iVzLD' \
+    'Xi1MmHoMGsIYnUq3Q8Y1Z5JiyFr0NO6XzfnrF_OYCQ=='
+
 
 class BaseTestWithFixedDate(unittest.TestCase):
     def setUp(self):
         self.datetime_patch = mock.patch('cdpcli.auth.datetime')
         self.datetime_mock = self.datetime_patch.start()
         self.fixed_date = datetime.datetime(2014, 3, 10, 17, 2, 55, 0)
         self.datetime_mock.datetime.utcnow.return_value = self.fixed_date
@@ -60,17 +65,17 @@
 
 class TestRSAV1(unittest.TestCase):
     maxDiff = None
 
     def setUp(self):
         access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
         self.credentials = cdpcli.credentials.Credentials(
-            access_key_id,
-            RSA_KEY,
-            'test')
+            access_key_id=access_key_id,
+            private_key=RSA_KEY,
+            method='test')
         self.rsav1 = cdpcli.auth.RSAv1Auth(self.credentials)
         self.date_mock = mock.patch('cdpcli.auth.formatdate')
         self.formatdate = self.date_mock.start()
         self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
 
     def tearDown(self):
         self.date_mock.stop()
@@ -155,17 +160,17 @@
     """
     We're not retesting aspects that are identical to what RSA tests cover
     """
 
     def setUp(self):
         access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
         self.credentials = cdpcli.credentials.Credentials(
-            access_key_id,
-            ED25519_KEY,
-            'test')
+            access_key_id=access_key_id,
+            private_key=ED25519_KEY,
+            method='test')
         self.ed25519v1 = cdpcli.auth.Ed25519v1Auth(self.credentials)
         self.date_mock = mock.patch('cdpcli.auth.formatdate')
         self.formatdate = self.date_mock.start()
         self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
 
     def tearDown(self):
         self.date_mock.stop()
@@ -199,7 +204,86 @@
 
         json_metadata = json.loads(
             urlsafe_b64decode(metadata.encode('utf-8')).decode('utf-8'))
         self.assertEqual(self.credentials.access_key_id,
                          json_metadata['access_key_id'])
         self.assertEqual("ed25519v1",
                          json_metadata['auth_method'])
+
+
+class TestECDSAV1(unittest.TestCase):
+    """
+    We're not retesting aspects that are identical to what RSA tests cover
+    """
+
+    def setUp(self):
+        access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
+        self.credentials = cdpcli.credentials.Credentials(
+            access_key_id=access_key_id,
+            private_key=ECDSA_KEY,
+            method='test')
+        self.ecdsav1 = cdpcli.auth.ECDSAv1Auth(self.credentials)
+        self.date_mock = mock.patch('cdpcli.auth.formatdate')
+        self.formatdate = self.date_mock.start()
+        self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
+
+    def tearDown(self):
+        self.date_mock.stop()
+
+    def test_no_credentials_raises_error(self):
+        ecdsav1 = cdpcli.auth.ECDSAv1Auth(None)
+        with self.assertRaises(NoCredentialsError):
+            ecdsav1.add_auth("pass someting")
+
+    def test_put(self):
+        http_headers = HTTPHeaders.from_dict({})
+        split = urlsplit('/foo/bar')
+        cs = self.ecdsav1._canonical_string('PUT', split, http_headers)
+        expected_canonical = "PUT\n\nThu, 17 Nov 2005 18:49:58 GMT\n/foo/bar\necdsav1"
+        self.assertEqual(expected_canonical, cs)
+        sig = self.ecdsav1._get_signature('PUT', split, HTTPHeaders.from_dict({}))
+        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
+
+    def test_auth_header_string(self):
+        http_headers = HTTPHeaders.from_dict({})
+        split = urlsplit('/foo/bar')
+        sig = self.ecdsav1._get_signature('PUT', split, http_headers)
+        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
+
+        auth_header_string = self.ecdsav1._get_signature_header(sig)
+        expected_metadata = 'eyJhY2Nlc3Nfa2V5X2lkIjogIkFCQ0QtRUZHSC1JSktMLU1O' \
+                            'T1AtUVJTVCIsICJhdXRoX21ldGhvZCI6ICJlY2RzYXYxIn0='
+        metadata, sig = auth_header_string.split(".")
+        self.assertEqual(expected_metadata, metadata)
+        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
+
+        json_metadata = json.loads(
+            urlsafe_b64decode(metadata.encode('utf-8')).decode('utf-8'))
+        self.assertEqual(self.credentials.access_key_id, json_metadata['access_key_id'])
+        self.assertEqual("ecdsav1", json_metadata['auth_method'])
+
+
+class TestAccessToken(unittest.TestCase):
+    def test_no_credentials_raises_error(self):
+        access_token_auth = cdpcli.auth.AccessTokenAuth(None)
+        with self.assertRaises(NoCredentialsError):
+            access_token_auth.add_auth("pass something")
+
+    def test_auth_header_string(self):
+        access_token = 'Bearer ABC.DEF'
+        credentials = cdpcli.credentials.Credentials(
+            access_token=access_token,
+            method='test')
+        access_token_auth = cdpcli.auth.AccessTokenAuth(credentials)
+
+        request = CdpRequest()
+        request.headers['Content-Type'] = 'text/html'
+        request.method = 'PUT'
+        request.url = 'https://altus.cloudera.com/service/op'
+
+        access_token_auth.add_auth(request)
+        self.assertEqual(request.headers['Authorization'], access_token)
+
+    def test_is_access_token(self):
+        self.assertFalse(cdpcli.auth.AccessTokenAuth.is_access_token(None))
+        self.assertFalse(cdpcli.auth.AccessTokenAuth.is_access_token(''))
+        self.assertTrue(cdpcli.auth.AccessTokenAuth.is_access_token('Bearer A.B'))
```

### Comparing `cdpcli-0.9.9/tests/unit/test_loaders.py` & `cdpcli-0.9.90/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/test_protocol.py` & `cdpcli-0.9.90/tests/unit/test_protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import datetime
 import os
+import sys
 
 from cdpcli.compat import json
 from cdpcli.compat import six
 from cdpcli.exceptions import ParamValidationError
 from cdpcli.model import ServiceModel
 from cdpcli.parser import ResponseParserFactory
 from cdpcli.serialize import create_serializer
@@ -95,14 +96,38 @@
                                 'crn': 'test-crn-1'},
                                {'name': 'test-name-2',
                                 'crn': 'test-crn-1'}]
         operation_model = self.service_model.operation_model('arrayOfObjects')
         request = self.serializer.serialize_to_request(params, operation_model)
         self._validate_request(request, '/directors/arrayOfObjects', params)
 
+    if sys.version_info.major >= 3:  # bytes is introduced in python3
+        def test_blob_param_bytes(self):
+            params = {}
+            params['data'] = b'Hello World'
+            operation_model = self.service_model.operation_model('blobObject')
+            request = self.serializer.serialize_to_request(params, operation_model)
+            params['data'] = 'SGVsbG8gV29ybGQ='
+            self._validate_request(request, '/directors/blobObject', params)
+
+    def test_blob_param_bytearray(self):
+        params = {}
+        params['data'] = bytearray(b'Hello World')
+        operation_model = self.service_model.operation_model('blobObject')
+        request = self.serializer.serialize_to_request(params, operation_model)
+        params['data'] = 'SGVsbG8gV29ybGQ='
+        self._validate_request(request, '/directors/blobObject', params)
+
+    def test_blob_param_base64(self):
+        params = {}
+        params['data'] = 'SGVsbG8gV29ybGQ='
+        operation_model = self.service_model.operation_model('blobObject')
+        request = self.serializer.serialize_to_request(params, operation_model)
+        self._validate_request(request, '/directors/blobObject', params)
+
 
 class TestParser(unittest.TestCase):
 
     def setUp(self):
         self.model = yaml.safe_load(open(os.path.join(PROTOCOL_DIR, 'service.yaml')))
         self.service_model = ServiceModel(self.model, 'servicename')
         self.parser = ResponseParserFactory().create_parser()
@@ -119,14 +144,36 @@
         body['code'] = code
         body['message'] = message
         response = {}
         response["status_code"] = 301
         response["body"] = json.dumps(body).encode(UTF8)
         return response
 
+    def _create_error_response_2(self, messages):
+        body = {}
+        body['errorMessages'] = messages
+        response = {}
+        response["status_code"] = 401
+        response["body"] = json.dumps(body).encode(UTF8)
+        return response
+
+    def _create_error_response_3(self, message):
+        body = {}
+        body['error'] = message
+        response = {}
+        response["status_code"] = 400
+        response["body"] = json.dumps(body).encode(UTF8)
+        return response
+
+    def _create_error_response_4(self, message):
+        response = {}
+        response["status_code"] = 409
+        response["body"] = message.encode(UTF8)
+        return response
+
     def _assert_same(self, v1, v2, path=""):
         if type(v1) is dict:
             for k in v1.keys():
                 self.assertTrue(k in v2)
                 self._assert_same(v1[k], v2[k])
             for k in v2.keys():
                 self.assertTrue(k in v1)
@@ -243,7 +290,43 @@
     def test_error(self):
         response = self._create_error_response(
             "YouMessedUpException",
             "You, sir, have messed up.")
         operation_model = self.service_model.operation_model('createDirector')
         parsed_response = self.parser.parse(response, operation_model.output_shape)
         self._validate_error_response(response, parsed_response)
+
+    def test_error_2(self):
+        response = self._create_error_response_2([
+            "YouMessedUpException",
+            "You, sir, have messed up."])
+        operation_model = self.service_model.operation_model('createDirector')
+        parsed_response = self.parser.parse(response, operation_model.output_shape)
+        self.assertEquals({
+            'error': {
+                'code': '',
+                'message': 'YouMessedUpException You, sir, have messed up.'}},
+            parsed_response)
+
+    def test_error_3(self):
+        response = self._create_error_response_3(
+            "YouMessedUpException "
+            "You, sir, have messed up.")
+        operation_model = self.service_model.operation_model('createDirector')
+        parsed_response = self.parser.parse(response, operation_model.output_shape)
+        self.assertEquals({
+            'error': {
+                'code': '',
+                'message': 'YouMessedUpException You, sir, have messed up.'}},
+            parsed_response)
+
+    def test_error_4(self):
+        response = self._create_error_response_4(
+            "YouMessedUpException "
+            "You, sir, have messed up.")
+        operation_model = self.service_model.operation_model('createDirector')
+        parsed_response = self.parser.parse(response, operation_model.output_shape)
+        self.assertEquals({
+            'error': {
+                'code': 'UNKNOWN_ERROR',
+                'message': 'YouMessedUpException You, sir, have messed up.'}},
+            parsed_response)
```

### Comparing `cdpcli-0.9.9/tests/unit/test_utils.py` & `cdpcli-0.9.90/tests/unit/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,53 @@
 from cdpcli import OBJECT_TYPE
 from cdpcli import xform_name
 from cdpcli.model import DenormalizedStructureBuilder
 from cdpcli.model import ServiceModel
 from cdpcli.utils import ArgumentGenerator
 from cdpcli.utils import CachedProperty
 from cdpcli.utils import datetime2timestamp
+from cdpcli.utils import get_extension_registers
 from cdpcli.utils import get_service_module_name
 from cdpcli.utils import instance_cache
+from cdpcli.utils import is_absolute_url
 from cdpcli.utils import parse_timestamp
 from cdpcli.utils import parse_to_aware_datetime
 from dateutil.tz import tzoffset, tzutc
 from tests import unittest
 
 
+class TestExtension(unittest.TestCase):
+    def test_get_extension_registers(self):
+        reg_ext, reg_cmd = get_extension_registers('iam')
+        self.assertIsNone(reg_ext)
+        self.assertIsNone(reg_cmd)
+
+        reg_ext, reg_cmd = get_extension_registers('redirect')
+        self.assertIsNotNone(reg_ext)
+        self.assertIsNone(reg_cmd)
+
+        reg_ext, reg_cmd = get_extension_registers('workload')
+        self.assertIsNotNone(reg_ext)
+        self.assertIsNone(reg_cmd)
+
+        reg_ext, reg_cmd = get_extension_registers('df')
+        self.assertIsNotNone(reg_ext)
+        self.assertIsNotNone(reg_cmd)
+
+        reg_ext, reg_cmd = get_extension_registers('invalid')
+        self.assertIsNone(reg_ext)
+        self.assertIsNone(reg_cmd)
+
+
+class TestUrl(unittest.TestCase):
+    def test_is_absolute_url(self):
+        self.assertTrue(is_absolute_url('https://host.com/api/v1/test'))
+        self.assertFalse(is_absolute_url('/api/v1/test'))
+
+
 class TestTransformName(unittest.TestCase):
     def test_upper_camel_case(self):
         self.assertEqual(xform_name('UpperCamelCase'), 'upper_camel_case')
         self.assertEqual(xform_name('UpperCamelCase', '-'), 'upper-camel-case')
 
     def test_lower_camel_case(self):
         self.assertEqual(xform_name('lowerCamelCase'), 'lower_camel_case')
@@ -193,23 +224,25 @@
         self.assert_skeleton_from_model_is(
             model={
                 'A': {'type': 'string'},
                 'B': {'type': 'integer'},
                 'C': {'type': 'float'},
                 'D': {'type': 'double'},
                 'E': {'type': 'boolean'},
-                'F': {'type': 'datetime'}
+                'F': {'type': 'datetime'},
+                'G': {'type': 'blob'}
             },
             generated_skeleton={
                 'A': '',
                 'B': 0,
                 'C': 0.0,
                 'D': 0.0,
                 'E': True,
-                'F': '2002-10-02T13:00:00+00:00'
+                'F': '2002-10-02T13:00:00+00:00',
+                'G': ''
             }
         )
 
     def test_generate_nested_objects(self):
         self.assert_skeleton_from_model_is(
             model={
                 'A': {
```

### Comparing `cdpcli-0.9.9/tests/unit/test_model.py` & `cdpcli-0.9.90/tests/unit/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,33 +42,55 @@
         service_model = ServiceModel(self.model, 'myservice')
         self.assertEqual(service_model.service_name, 'myservice')
 
     def test_products(self):
         service_model = ServiceModel(self.model, 'myservice')
         self.assertEqual(service_model.products, ['ALTUS'])
 
+    def test_form_factors(self):
+        service_model = ServiceModel(self.model, 'myservice')
+        self.assertEqual(service_model.form_factors, ['public', 'private'])
+
+    def test_endpoint_prefix(self):
+        service_model = ServiceModel(self.model, 'myservice')
+        self.assertEqual(service_model.endpoint_prefix, 'api')
+
     def test_operations(self):
         self.assertTrue(self.service_model.operation_model(
                 'createDirector') is not None)
         self.assertTrue(self.service_model.operation_model(
                 'deleteDirector') is not None)
         self.assertTrue(self.service_model.operation_model(
                 'describeDirectors') is not None)
+        self.assertTrue(self.service_model.operation_model(
+                'getDirectors') is not None)
         with self.assertRaises(OperationNotFoundError):
             self.service_model.operation_model('NonExistentOperation')
 
+    def test_multiple_operation_ids(self):
+        self.assertFalse(self.service_model.operation_model(
+                'describeDirectors').is_deprecated)
+        self.assertTrue(self.service_model.operation_model(
+                'getDirectors').is_deprecated)
+        self.assertEquals(self.service_model.operation_model(
+                'getDirectors').name, 'getDirectors')
+        self.assertEquals(
+                self.service_model.operation_model('getDirectors').http,
+                self.service_model.operation_model('describeDirectors').http)
+
     def test_documentation(self):
         self.assertTrue(self.service_model.documentation.startswith(
                 'Cloudera CDP Test Service Description'))
 
     def test_operation_names(self):
-        self.assertEquals(len(self.service_model.operation_names), 3)
+        self.assertEquals(len(self.service_model.operation_names), 4)
         self.assertTrue('createDirector' in self.service_model.operation_names)
         self.assertTrue('deleteDirector' in self.service_model.operation_names)
         self.assertTrue('describeDirectors' in self.service_model.operation_names)
+        self.assertTrue('getDirectors' in self.service_model.operation_names)
 
 
 class TestOperationModel(unittest.TestCase):
     def setUp(self):
         self.model = yaml.safe_load(open(os.path.join(MODEL_DIR, 'service.yaml')))
         self.service_model = ServiceModel(self.model, 'servicename')
 
@@ -84,14 +106,20 @@
         self.assertEqual(operation_model.paging_result, 'directors')
         operation_model = self.service_model.operation_model('createDirector')
         self.assertEqual(operation_model.can_paginate, False)
         self.assertEqual(operation_model.paging_input_token, None)
         self.assertEqual(operation_model.paging_output_token, None)
         self.assertEqual(operation_model.paging_result, None)
 
+    def test_form_factors(self):
+        operation_model = self.service_model.operation_model('describeDirectors')
+        self.assertIsNone(operation_model.form_factors)
+        operation_model = self.service_model.operation_model('deleteDirector')
+        self.assertEqual(operation_model.form_factors, ['public'])
+
     def test_operation_input(self):
         operation_model = self.service_model.operation_model('createDirector')
         self.assertEqual(operation_model.http['method'], 'post')
         self.assertEqual(operation_model.http['requestUri'], '/directors/createDirector')
         self.assertEqual(operation_model.input_shape.name, 'input')
         self.assertEqual(list(operation_model.input_shape.members), ['name'])
 
@@ -177,18 +205,18 @@
 
     def test_invalid_shape_type(self):
         with self.assertRaises(InvalidShapeError):
             self.resolver.get_shape_by_name('invalid', 'MissingShapeType')
         with self.assertRaises(InvalidShapeError):
             self.resolver.get_shape_by_name('invalid', 'InvalidShapeType')
 
-    def test_undocumented_param(self):
+    def test_deprecated_param(self):
         shape = self.resolver.get_shape_by_name('shape', 'UndocumentedParmTest')
-        self.assertEqual(shape.members['undocumentedParam'].is_undocumented, True)
-        self.assertEqual(shape.members['documentedParam'].is_undocumented, False)
+        self.assertEqual(shape.members['undocumentedParam'].is_deprecated, True)
+        self.assertEqual(shape.members['documentedParam'].is_deprecated, False)
 
     def test_referenced_map(self):
         shape = self.resolver.get_shape_by_name('shape', 'ReferencedMapTest')
         self.assertEqual(shape.members['endpoints'].type_name, 'map')
         self.assertEqual(shape.members['endpoints'].key.type_name, 'string')
         self.assertEqual(shape.members['endpoints'].value.type_name, 'object')
         self.assertTrue(self._compare_lists(
@@ -212,14 +240,18 @@
             shape.members['endpoints'].value
 
     def test_no_freeform_map_true_shape(self):
         with self.assertRaises(InvalidShapeError):
             shape = self.resolver.get_shape_by_name('invalid', 'NoFreeformMapTrueTest')
             shape.members['endpoints'].value
 
+    def test_blob_shape(self):
+        shape = self.resolver.get_shape_by_name('shape', 'BlobTest')
+        self.assertEqual(shape.members['blobparam'].type_name, 'blob')
+
     def _compare_lists(self, x, y):
         return collections.Counter(x) == collections.Counter(y)
 
 
 class TestBuilders(unittest.TestCase):
 
     def test_structure_shape_builder_with_scalar_types(self):
```

### Comparing `cdpcli-0.9.9/tests/unit/test_paginate.py` & `cdpcli-0.9.90/tests/unit/test_paginate.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,34 @@
         responses = [{'Foo': 'foo', 'NextToken': 'm1'},
                      {'NextToken': 'm2'},
                      {'Foo': 'bar'}]
         self.method.side_effect = responses
         result = self.paginator.paginate().build_full_result()
         self.assertEqual(result, {'Foo': 'foobar'})
 
+    def test_build_full_result_extra_field(self):
+        responses = [{'Extra': 'hello', 'Foo': 0.0, 'NextToken': 'm1'},
+                     {'Extra': 'hello', 'Foo': 0.0}]
+        self.method.side_effect = responses
+        result = self.paginator.paginate().build_full_result()
+        self.assertEqual(result, {'Extra': 'hello', 'Foo': 0.0})
+
+    def test_build_full_result_extra_field_from_first_response(self):
+        responses = [{'Extra': 'hello', 'Foo': 0.0, 'NextToken': 'm1'},
+                     {'Field': 'world', 'Foo': 0.0}]
+        self.method.side_effect = responses
+        result = self.paginator.paginate().build_full_result()
+        self.assertEqual(result, {'Extra': 'hello', 'Foo': 0.0})
+
+    def test_build_full_result_extra_field_only(self):
+        responses = [{'Extra': 'hello'}]
+        self.method.side_effect = responses
+        result = self.paginator.paginate().build_full_result()
+        self.assertEqual(result, {'Extra': 'hello'})
+
     def test_exception_raised_if_same_next_token(self):
         responses = [{'NextToken': 'token1'},
                      {'NextToken': 'token2'},
                      {'NextToken': 'token2'}]
         self.method.side_effect = responses
         with self.assertRaises(PaginationError):
             list(self.paginator.paginate())
```

### Comparing `cdpcli-0.9.9/tests/unit/test_table_formatter.py` & `cdpcli-0.9.90/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.9/tests/unit/test_credentials.py` & `cdpcli-0.9.90/tests/unit/test_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,36 +48,46 @@
     'private_key': raw_metadata['foobar']['PrivateKey'],
     'expiry_time': raw_metadata['foobar']['Expiration'],
 }
 context = Context()
 
 
 class TestCredentials(BaseEnvVar):
-    def _ensure_credential_is_normalized_as_unicode(self, access, secret):
-        c = credentials.Credentials(access, secret, 'test')
+    def _ensure_credential_is_normalized_as_unicode(self, access, secret, token):
+        c = credentials.Credentials(access_key_id=access,
+                                    private_key=secret,
+                                    access_token=token,
+                                    method='test')
         self.assertTrue(isinstance(c.access_key_id, type(u'u')))
         self.assertTrue(isinstance(c.private_key, type(u'u')))
+        self.assertTrue(isinstance(c.access_token, type(u'u')))
 
     def test_detect_nonascii_character(self):
         self._ensure_credential_is_normalized_as_unicode(
-            'foo\xe2\x80\x99', 'bar\xe2\x80\x99')
+            'foo\xe2\x80\x99', 'bar\xe2\x80\x99', 'tea\xe2\x80\x99')
 
     def test_unicode_input(self):
         self._ensure_credential_is_normalized_as_unicode(
-            u'foo', u'bar')
+            u'foo', u'bar', u'tea')
 
     def test_frozen_credentials(self):
-        cred = credentials.Credentials("key", "secret", "test")
+        cred = credentials.Credentials(access_key_id="key",
+                                       private_key="secret",
+                                       access_token='token',
+                                       method="test")
         frozen_creds = cred.get_frozen_credentials()
         self.assertEqual("key", frozen_creds.access_key_id)
         self.assertEqual("secret", frozen_creds.private_key)
+        self.assertEqual("token", frozen_creds.access_token)
         cred.access_key_id = "foobar"
         cred.private_key = "foo"
+        cred.access_token = "bar"
         self.assertEqual("key", frozen_creds.access_key_id)
         self.assertEqual("secret", frozen_creds.private_key)
+        self.assertEqual("token", frozen_creds.access_token)
 
 
 class TestBaseCredentialProvider(BaseEnvVar):
     def test_load(self):
         cred_provider = credentials.CredentialProvider()
         self.assertTrue(cred_provider.load())
 
@@ -102,14 +112,24 @@
         provider = credentials.EnvProvider(environ)
         creds = provider.load()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
         self.assertEqual(creds.method, 'env')
 
+    def test_envvars_are_found_access_token(self):
+        environ = {
+            'CDP_ACCESS_TOKEN': 'tea'
+        }
+        provider = credentials.EnvProvider(environ)
+        creds = provider.load()
+        self.assertIsNotNone(creds)
+        self.assertEqual(creds.access_token, 'tea')
+        self.assertEqual(creds.method, 'env')
+
     def test_envvars_not_found(self):
         provider = credentials.EnvProvider(environ={})
         cred = provider.load()
         self.assertTrue(cred is None)
 
     def test_can_override_env_var_mapping(self):
         # We can change the env var provider to
@@ -125,14 +145,29 @@
         provider = credentials.EnvProvider(
             environ, mapping
         )
         creds = provider.load()
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
 
+    def test_can_override_env_var_mapping_access_token(self):
+        # We can change the env var provider to
+        # use our specified env var names.
+        environ = {
+            'FOO_ACCESS_token': 'foo'
+        }
+        mapping = {
+            'access_token': 'FOO_ACCESS_token'
+        }
+        provider = credentials.EnvProvider(
+            environ, mapping
+        )
+        creds = provider.load()
+        self.assertEqual(creds.access_token, 'foo')
+
     def test_can_override_partial_env_var_mapping(self):
         # Only changing the access key mapping.
         # The other 2 use the default values of
         # CDP_SECRET_ACCESS_KEY and CDP_SESSION_TOKEN
         # use our specified env var names.
         environ = {
             'FOO_ACCESS_KEY_ID': 'foo',
@@ -161,14 +196,21 @@
         # use our specified env var names.
         self.environ['CDP_ACCESS_KEY_ID'] = 'foo'
         self.environ['CDP_PRIVATE_KEY'] = self.pem_file
         creds = credentials.get_credentials(context)
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
 
+    def test_credential_with_envprovider_access_token(self):
+        # We can change the env var provider to
+        # use our specified env var names.
+        self.environ['CDP_ACCESS_TOKEN'] = 'foo'
+        creds = credentials.get_credentials(context)
+        self.assertEqual(creds.access_token, 'foo')
+
     def test_raise_if_not_a_file(self):
         environ = {
             'CDP_ACCESS_KEY_ID': 'foo',
             'CDP_PRIVATE_KEY': self.pem_file + "dose_not_exist",
         }
         provider = credentials.EnvProvider(environ)
         with self.assertRaises(NoCredentialsError):
@@ -190,15 +232,17 @@
 class CredentialResolverTest(BaseEnvVar):
     def setUp(self):
         super(CredentialResolverTest, self).setUp()
         self.provider1 = mock.Mock()
         self.provider1.METHOD = 'provider1'
         self.provider2 = mock.Mock()
         self.provider2.METHOD = 'provider2'
-        self.fake_creds = credentials.Credentials('a', 'b', 'test')
+        self.fake_creds = credentials.Credentials(access_key_id='a',
+                                                  private_key='b',
+                                                  method='test')
 
     def test_load_credentials_single_provider(self):
         self.provider1.load.return_value = self.fake_creds
         resolver = credentials.CredentialResolver(providers=[self.provider1])
         creds = resolver.load_credentials()
         self.assertEqual(creds.access_key_id, 'a')
         self.assertEqual(creds.private_key, 'b')
@@ -245,15 +289,17 @@
         # Now, if we were to call resolver.load() now, provider2 would
         # win because it's returning a non None response.
         # However we can inject a new provider before provider2 to
         # override this process.
         # Providers can be added by the METHOD name of each provider.
         new_provider = mock.Mock()
         new_provider.METHOD = 'new_provider'
-        new_provider.load.return_value = credentials.Credentials('d', 'e', 'test')
+        new_provider.load.return_value = credentials.Credentials(access_key_id='d',
+                                                                 private_key='e',
+                                                                 method='test')
 
         resolver.insert_after('provider1', new_provider)
 
         creds = resolver.load_credentials()
         self.assertIsNotNone(creds)
 
         self.assertEqual(creds.access_key_id, 'd')
@@ -263,28 +309,32 @@
         # a non-None response.
         self.provider1.load.assert_called_with()
         self.assertTrue(not self.provider2.called)
 
     def test_inject_provider_before_existing(self):
         new_provider = mock.Mock()
         new_provider.METHOD = 'override'
-        new_provider.load.return_value = credentials.Credentials('x', 'y', 'test')
+        new_provider.load.return_value = credentials.Credentials(access_key_id='x',
+                                                                 private_key='y',
+                                                                 method='test')
 
         resolver = credentials.CredentialResolver(providers=[self.provider1,
                                                              self.provider2])
         resolver.insert_before(self.provider1.METHOD, new_provider)
         creds = resolver.load_credentials()
         self.assertEqual(creds.access_key_id, 'x')
         self.assertEqual(creds.private_key, 'y')
 
     def test_can_remove_providers(self):
-        self.provider1.load.return_value = credentials.Credentials(
-            'a', 'b', 'test')
-        self.provider2.load.return_value = credentials.Credentials(
-            'd', 'e', 'test')
+        self.provider1.load.return_value = credentials.Credentials(access_key_id='a',
+                                                                   private_key='b',
+                                                                   method='test')
+        self.provider2.load.return_value = credentials.Credentials(access_key_id='d',
+                                                                   private_key='e',
+                                                                   method='test')
         resolver = credentials.CredentialResolver(providers=[self.provider1,
                                                              self.provider2])
         resolver.remove('provider1')
         creds = resolver.load_credentials()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'd')
         self.assertEqual(creds.private_key, 'e')
@@ -356,14 +406,25 @@
         provider = credentials.AuthConfigFile(self.conf_file)
         creds = provider.load()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'key_id')
         self.assertEqual(creds.private_key, 'secret')
         self.assertEqual(creds.method, 'auth_config_file')
 
+    def test_config_is_found_access_token(self):
+        def validate(path):
+            provider = credentials.AuthConfigFile(path)
+            cred = provider.load()
+            self.assertIsNotNone(cred)
+            self.assertEqual(cred.access_token, 'Bearer A.B.C')
+            self.assertEqual(cred.method, 'auth_config_file')
+
+        conf = '{"access_token": "Bearer A.B.C"}'
+        _run_test(conf, validate)
+
     def test_config_not_found(self):
         with self.assertRaises(NoCredentialsError):
             provider = credentials.AuthConfigFile(
                 self.conf_file + "_does_not_exist")
             provider.load()
 
     def test_bad_json(self):
@@ -491,7 +552,52 @@
 
         conf = """
 [default]
 cdp_private_key = secret\\nwith\\na\\nfew\\nnewlines
 cdp_access_key_id = the_key
 """
         _run_test(conf, validate)
+
+    def test_credentials_file_access_token(self):
+        def validate(path):
+            provider = credentials.SharedCredentialProvider(
+                creds_filename=path, profile_name=DEFAULT_PROFILE_NAME)
+            creds = provider.load()
+            self.assertIsNotNone(creds)
+            self.assertEqual(creds.access_token, 'Bearer A.B.C')
+            self.assertEqual(creds.method, 'shared-credentials-file')
+
+        conf = """
+[default]
+cdp_access_token = Bearer A.B.C
+"""
+        _run_test(conf, validate)
+
+
+class TestParamsProvider(unittest.TestCase):
+    def test_no_param(self):
+        provider = credentials.ParamsProvider(None)
+        creds = provider.load()
+        self.assertIsNone(creds)
+
+    def test_no_access_token_param(self):
+        params = {}
+        provider = credentials.ParamsProvider(params)
+        creds = provider.load()
+        self.assertIsNone(creds)
+
+    def test_empty_access_token_param(self):
+        params = mock.Mock()
+        params.access_token = ''
+        provider = credentials.ParamsProvider(params)
+        creds = provider.load()
+        self.assertIsNone(creds)
+
+    def test_access_token_param(self):
+        access_token = 'Bearer A.B'
+        params = mock.Mock()
+        params.access_token = access_token
+        provider = credentials.ParamsProvider(params)
+        creds = provider.load()
+        self.assertIsNotNone(creds)
+        self.assertEqual(creds.access_token, access_token)
+        self.assertEqual(creds.method, 'params')
```

### Comparing `cdpcli-0.9.9/tests/unit/test_signers.py` & `cdpcli-0.9.90/tests/unit/test_signers.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from cdpcli.signers import RequestSigner
 import mock
 from tests import unittest
 
 
 class BaseSignerTest(unittest.TestCase):
     def setUp(self):
-        self.credentials = Credentials('key', 'secret', 'test')
+        self.credentials = Credentials(access_key_id='key',
+                                       private_key='secret',
+                                       method='test')
         self.signer = RequestSigner('rsav1', self.credentials)
         self.fixed_credentials = self.credentials.get_frozen_credentials()
 
 
 class TestSigner(BaseSignerTest):
 
     def test_signature_version(self):
```

### Comparing `cdpcli-0.9.9/tests/unit/test_completer.py` & `cdpcli-0.9.90/tests/unit/test_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,49 @@
             },
             'arguments': []
         }
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
         self.assert_completion(completer, 'cdp bin', [])
 
+    def test_complete_cli_enum_options(self):
+        commands = {
+            'subcommands': {},
+            'arguments': ['version', 'output', 'color']
+        }
+        clidriver = self.clidriver_creator.create_clidriver(commands)
+        clidriver._cli_data = {
+            "options": {
+                "version": {
+                    "action": "version",
+                    "help": "<p>Display the version of this tool.</p>"
+                },
+                "output": {
+                    "choices": [
+                        "json",
+                        "text",
+                        "table"
+                    ],
+                    "help": "<p>The formatting style for command output.</p>"
+                },
+                "color": {
+                    "choices": [
+                        "on",
+                        "off",
+                        "auto"
+                    ],
+                    "default": "auto",
+                    "help": "<p>Turn on/off color output.</p>"
+                }
+            }
+        }
+        completer = Completer(clidriver)
+        self.assert_completion(completer, 'cdp --output ', ['json', 'text', 'table'])
+        self.assert_completion(completer, 'cdp --color ', ['on', 'off', 'auto'])
+
     def test_complete_top_level_args(self):
         commands = {
             'subcommands': {},
             'arguments': ['foo', 'bar']
         }
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
@@ -289,14 +324,15 @@
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
         self.assert_completion(completer, 'cdp ', ['foo'])
 
 
 class MockModel:
     is_hidden = False
+    is_deprecated = False
 
 
 class MockCLIDriverFactory(object):
     def create_clidriver(self, commands=None):
         clidriver = mock.Mock(spec=CLIDriver)
         clidriver._create_help_command.return_value = \
             self._create_top_level_help(clidriver, commands)
@@ -320,15 +356,15 @@
         service_command._service_model = {}
         service_command._command_table = command_table
         return service_command
 
     def _create_operation_command(self, clidriver, name, command):
         argument_table = self.create_argument_table(
             command.get('arguments', []))
-        operation = ServiceOperation(name, 'parent', None, MockModel())
+        operation = ServiceOperation(clidriver, name, 'parent', None, MockModel())
         operation._arg_table = argument_table
         return operation
 
     def create_command_table(self, clidriver, commands, command_creator):
         if not commands:
             return OrderedDict()
         command_table = OrderedDict()
```

### Comparing `cdpcli-0.9.9/tests/unit/test_argparser.py` & `cdpcli-0.9.90/tests/unit/test_argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) 2016 Cloudera, Inc. All rights reserved.
 
 import os
 
 from cdpcli.argparser import ArgTableArgParser
 from cdpcli.argparser import ServiceArgParser
-from cdpcli.clidriver import ServiceOperation
+from cdpcli.clidriver import CLIDriver, ServiceOperation
 from cdpcli.model import ServiceModel
+from mock import Mock
 from tests import unittest
 import yaml
 
 MODEL_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                          'argparser')
 TEST_ARGS = ['submit-spark-job',
              '--jars',
@@ -42,14 +43,15 @@
 class TestArgTableArgParser(unittest.TestCase):
 
     def setUp(self):
         self.args = TEST_ARGS[1:]
         model = yaml.safe_load(open(os.path.join(MODEL_DIR, 'service.yaml')))
         service_model = ServiceModel(model, 'servicename')
         service_operation = ServiceOperation(
+            Mock(spec=CLIDriver),
             'submit-spark-job',
             'dataeng',
             '',
             service_model.operation_model('submitSparkJob'))
         self.parser = ArgTableArgParser(service_operation.arg_table)
 
     def testArsParsedCorrectly(self):
```

### Comparing `cdpcli-0.9.9/tests/unit/test_shorthand.py` & `cdpcli-0.9.90/tests/unit/test_shorthand.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,24 +221,27 @@
     def test_can_convert_scalar_types_from_string(self):
         m = model.DenormalizedStructureBuilder().with_members({
             'A': {'type': 'integer'},
             'B': {'type': 'string'},
             'C': {'type': 'float'},
             'D': {'type': 'boolean'},
             'E': {'type': 'boolean'},
+            'F': {'type': 'blob'},
         }).build_model()
         b = shorthand.BackCompatVisitor()
 
         params = {'A': '24', 'B': '24', 'C': '24.12345',
-                  'D': 'true', 'E': 'false'}
+                  'D': 'true', 'E': 'false',
+                  'F': 'SGVsbG8gV29ybGQ='}
         b.visit(params, m)
         self.assertEqual(
             params,
             {'A': 24, 'B': '24', 'C': float('24.12345'),
-             'D': True, 'E': False})
+             'D': True, 'E': False,
+             'F': 'SGVsbG8gV29ybGQ='})
 
     def test_empty_values_not_added(self):
         m = model.DenormalizedStructureBuilder().with_members({
             'A': {'type': 'boolean'},
         }).build_model()
         b = shorthand.BackCompatVisitor()
```

### Comparing `cdpcli-0.9.9/tests/unit/test_validate.py` & `cdpcli-0.9.90/tests/unit/test_validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from datetime import datetime
 import decimal
 import os
+import sys
 
 from cdpcli.model import ServiceModel
 from cdpcli.model import ShapeResolver
 from cdpcli.validate import ParamValidator
 from tests import unittest
 import yaml
 
@@ -79,23 +80,25 @@
             {'stringparam': 24,
              'intparam': 'notint',
              'boolparam': 'notbool',
              'numberparam': 'notnumber',
              'datetimeparam': 'notdatetime',
              'arrayparam': 'notarray',
              'objectparam': 'notobject',
-             'mapparam': 'notmap'},
+             'mapparam': 'notmap',
+             'blobparam': 123},
             ['Invalid type for parameter stringparam',
              'Invalid type for parameter intparam',
              'Invalid type for parameter boolparam',
              'Invalid type for parameter numberparam',
              'Invalid type for parameter datetimeparam',
              'Invalid type for parameter arrayparam',
              'Invalid type for parameter objectparam',
-             'Invalid type for parameter mapparam'])
+             'Invalid type for parameter mapparam',
+             'Invalid type for parameter blobparam'])
 
     def test_datetime_type_accepts_datetime_object(self):
         errors = self.get_validation_error_message(
             self.resolver.get_shape_by_name('typestest', 'TypesTest'),
             {'datetimeparam': datetime.now()})
         self.assertEqual(errors.generate_report(), '')
 
@@ -131,14 +134,58 @@
 
     def test_invalid_value_map(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('typestest', 'TypesTest'),
             {'mapparam': {'key1': 'value1', 'key2': 2}},
             ["Invalid type for parameter mapparam.key2, value: 2"])
 
+    def test_valid_blob_base64(self):
+        errors = self.get_validation_error_message(
+            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+            {'blobparam': 'SGVsbG8gV29ybGQ='})
+        self.assertEqual(errors.generate_report(), '')
+
+    def test_valid_blob_empty_base64(self):
+        errors = self.get_validation_error_message(
+            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+            {'blobparam': ''})
+        self.assertEqual(errors.generate_report(), '')
+
+    def test_invalid_value_blob_base64(self):
+        self.assert_has_validation_errors(
+            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+            {'blobparam': 'ABC'},
+            ["Invalid base64 value for parameter blobparam, error: Incorrect padding"])
+
+    if sys.version_info.major >= 3:  # bytes is introduced in python3
+        def test_valid_blob_bytes(self):
+            errors = self.get_validation_error_message(
+                self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+                {'blobparam': b'BlobTest'})
+            self.assertEqual(errors.generate_report(), '')
+
+    if sys.version_info.major >= 3:  # bytes is introduced in python3
+        def test_valid_blob_empty_bytes(self):
+            errors = self.get_validation_error_message(
+                self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+                {'blobparam': b''})
+            self.assertEqual(errors.generate_report(), '')
+
+    def test_valid_blob_bytearray(self):
+        errors = self.get_validation_error_message(
+            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+            {'blobparam': bytearray(b'BlobTest')})
+        self.assertEqual(errors.generate_report(), '')
+
+    def test_valid_blob_empty_bytearray(self):
+        errors = self.get_validation_error_message(
+            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
+            {'blobparam': bytearray(b'')})
+        self.assertEqual(errors.generate_report(), '')
+
 
 class TestValidateRanges(BaseTestValidate):
 
     def test_less_than_range(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
             {'intparam': -10,
@@ -193,14 +240,52 @@
 
     def test_only_max_value_specified(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
             {'maxonlystringparam': 'thisistoolong'},
             ['Invalid length for parameter maxonlystringparam'])
 
+    if sys.version_info.major >= 3:  # bytes is introduced in python3
+        def test_blob_min_length_contraint_bytes(self):
+            self.assert_has_validation_errors(
+                self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+                {'blobparam': b''},
+                ['Invalid length for parameter blobparam'])
+
+    if sys.version_info.major >= 3:  # bytes is introduced in python3
+        def test_blob_max_length_contraint_bytes(self):
+            self.assert_has_validation_errors(
+                self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+                {'blobparam': b'thisistoolong'},
+                ['Invalid length for parameter blobparam'])
+
+    def test_blob_min_length_contraint_bytearray(self):
+        self.assert_has_validation_errors(
+            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+            {'blobparam': bytearray(b'')},
+            ['Invalid length for parameter blobparam'])
+
+    def test_blob_max_length_contraint_bytearray(self):
+        self.assert_has_validation_errors(
+            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+            {'blobparam': bytearray(b'thisistoolong')},
+            ['Invalid length for parameter blobparam'])
+
+    def test_blob_min_length_contraint_base64(self):
+        self.assert_has_validation_errors(
+            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+            {'blobparam': ''},
+            ['Invalid length for parameter blobparam'])
+
+    def test_blob_max_length_contraint_base64(self):
+        self.assert_has_validation_errors(
+            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
+            {'blobparam': 'dGhpc2lzdG9vbG9uZw=='},
+            ['Invalid length for parameter blobparam'])
+
 
 class TestValidationNumberType(BaseTestValidate):
 
     def test_range_number(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('numbertest', 'NumberTest'),
             {'numberparam': 1},
```

### Comparing `cdpcli-0.9.9/tests/unit/test_retryhandler.py` & `cdpcli-0.9.90/tests/unit/test_retryhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 
 from cdpcli import retryhandler
-from cdpcli.thirdparty.requests import ConnectionError, Timeout
-from cdpcli.thirdparty.requests.packages.urllib3.exceptions \
-    import ClosedPoolError
 import mock
+from requests import ConnectionError, Timeout
 from tests import unittest
-
+from urllib3.exceptions import ClosedPoolError
 
 HTTP_500_RESPONSE = mock.Mock()
 HTTP_500_RESPONSE.status_code = 500
 
 HTTP_400_RESPONSE = mock.Mock()
 HTTP_400_RESPONSE.status_code = 400
```

### Comparing `cdpcli-0.9.9/tests/unit/__init__.py` & `cdpcli-0.9.90/tests/unit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,24 @@
 zU0IHNaprGxO+yZuMvdyfxcJVuFQf22mujPI8GluXyfA5i2IZjScNf5Awccu8HS5
 mzJp12+5oAZ+tJE1scpVoaVdZloY8XA1u0aCt2BhZavjIizTyzY4L8clo2iGIO1x
 yj5v7z/1wWTorT4w3/IHcwM=
 -----END PRIVATE KEY-----"""
 
 ED25519_KEY = 'VHswlNpwJnMpuXhIq7LYDfzs+R9pHvVLqgBGbhcnbSE='
 
+ECDSA_KEY = \
+    """-----BEGIN PRIVATE KEY-----
+MIH3AgEAMBAGByqGSM49AgEGBSuBBAAjBIHfMIHcAgEBBEIB/VhgNb6ccDq9hV/s
+TD8f1hSZo2Y7A7zZbCK0418vU0HYOi4Ic8TKjKIYw8cMQN7+2fGLQTkGezgu9NBw
+gzR/LGKgBwYFK4EEACOhgYkDgYYABAGxMOPpk3m7wgXPRHBCSpW9as4tuCv38UJQ
+37xSJqmim6LlF6s/eFRpRktNO98fLuAvAFt+97iYwOfhix4h/uVCSgFR0xloJtMe
+MEQft1ColfYUlGSiNuMsGyugK/ilkmulX52Y7z3RY6hxlFAegHI8d9uzeVqUL+KO
+1xtgNBDXVMnQCA==
+-----END PRIVATE KEY-----"""
+
 
 class FakeContext(object):
 
     def __init__(self,
                  all_variables,
                  profile_does_not_exist=False,
                  config_file_vars={},
@@ -65,15 +75,15 @@
         self.environment_vars = environment_vars
         self._credentials = credentials
         self.profile = None
         self.effective_profile = None
         # This lets us use the FakeContext as both context and "client_creator"
         self.context = self
 
-    def get_credentials(self):
+    def get_credentials(self, parsed_globals=None):
         return self._credentials
 
     def get_scoped_config(self):
         if self.profile_does_not_exist:
             raise ProfileNotFound(profile='foo')
         return self.config
```

