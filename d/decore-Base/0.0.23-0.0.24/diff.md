# Comparing `tmp/decore_Base-0.0.23.tar.gz` & `tmp/decore_Base-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.23.tar", last modified: Mon Jun 19 13:19:09 2023, max compression
+gzip compressed data, was "decore_Base-0.0.24.tar", last modified: Thu Jun 22 12:19:02 2023, max compression
```

## Comparing `decore_Base-0.0.23.tar` & `decore_Base-0.0.24.tar`

### file list

```diff
@@ -1,236 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-19 13:18:55.000000 decore_Base-0.0.23/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 13:18:55.000000 decore_Base-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-19 13:19:09.549661 decore_Base-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-19 13:18:55.000000 decore_Base-0.0.23/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-06-19 13:18:55.000000 decore_Base-0.0.23/README_DE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/decore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.517661 decore_Base-0.0.23/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/person_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1363968 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/querybase.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/uniform/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/uniform/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/reform_server_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/decore.rst.out
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/language.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/model.rst.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)    79165 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    46074 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    42879 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/docs/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/state/querybase.db
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 13:18:55.000000 decore_Base-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 13:18:55.000000 decore_Base-0.0.23/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-19 13:19:09.549661 decore_Base-0.0.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 12:18:54.000000 decore_Base-0.0.24/KOFI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-22 12:18:54.000000 decore_Base-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 12:19:02.731172 decore_Base-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-06-22 12:18:54.000000 decore_Base-0.0.24/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-06-22 12:18:54.000000 decore_Base-0.0.24/README_DE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/decore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    33933 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/586.6cfbf2b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/app.aff5db90.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376913 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/vendor.6fe961ae.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/person_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/586.aa14c175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/app.af6cbe84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/vendor.0902ddb5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)    57344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/reform_server_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/decore.rst.out
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/language.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/model.rst.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)    79165 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    46074 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/pygments.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42879 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/docs/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/state/querybase.db
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 12:18:54.000000 decore_Base-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 12:18:54.000000 decore_Base-0.0.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-22 12:19:02.731172 decore_Base-0.0.24/setup.cfg
```

### Comparing `decore_Base-0.0.23/.github/FUNDING.yml` & `decore_Base-0.0.24/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/.gitignore` & `decore_Base-0.0.24/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/.vscode/launch.json` & `decore_Base-0.0.24/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/KOFI.md` & `decore_Base-0.0.24/KOFI.md`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/LICENSE` & `decore_Base-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/PKG-INFO` & `decore_Base-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.23
+Version: 0.0.24
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -226,15 +226,15 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model(data['item'])
+                     item = First_model(**data['item'])
                      item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
                         return False, 'Error while saving ' + item.title
 
 .. note::
```

### Comparing `decore_Base-0.0.23/README.rst` & `decore_Base-0.0.24/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model(data['item'])
+                     item = First_model(**data['item'])
                      item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
                         return False, 'Error while saving ' + item.title
 
 .. note::
```

### Comparing `decore_Base-0.0.23/README_DE.rst` & `decore_Base-0.0.24/README_DE.rst`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model(data['item'])
+                     item = First_model(**data['item'])
                      item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
                         return False, 'Error while saving ' + item.title
 
 .. note::
```

### Comparing `decore_Base-0.0.23/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.24/decore_Base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.23
+Version: 0.0.24
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -226,15 +226,15 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model(data['item'])
+                     item = First_model(**data['item'])
                      item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
                         return False, 'Error while saving ' + item.title
 
 .. note::
```

### Comparing `decore_Base-0.0.23/decore_Base.egg-info/SOURCES.txt` & `decore_Base-0.0.24/decore_Base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 decore_base/decore.py
 decore_base/globals.py
 decore_base/classes/decore_action.py
 decore_base/classes/decore_app.py
 decore_base/classes/decore_base.py
 decore_base/classes/decore_dialog.py
 decore_base/classes/decore_element.py
+decore_base/classes/decore_fields.py
 decore_base/classes/decore_function.py
 decore_base/classes/decore_list.py
 decore_base/classes/decore_model.py
 decore_base/classes/decore_object.py
 decore_base/classes/decore_pool.py
 decore_base/classes/decore_prompt.py
 decore_base/classes/decore_query.py
@@ -60,18 +61,18 @@
 decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
 decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
 decore_base/prepare/spa/static/icons/favicon-128x128.png
 decore_base/prepare/spa/static/icons/favicon-16x16.png
 decore_base/prepare/spa/static/icons/favicon-32x32.png
 decore_base/prepare/spa/static/icons/favicon-96x96.png
-decore_base/prepare/spa/static/js/586.aa14c175.js
+decore_base/prepare/spa/static/js/586.6cfbf2b5.js
 decore_base/prepare/spa/static/js/65.940d9b80.js
-decore_base/prepare/spa/static/js/app.af6cbe84.js
-decore_base/prepare/spa/static/js/vendor.0902ddb5.js
+decore_base/prepare/spa/static/js/app.aff5db90.js
+decore_base/prepare/spa/static/js/vendor.6fe961ae.js
 decore_base/prepare/spa/templates/index.html
 decore_base/sample/.gitignore
 decore_base/sample/app.py
 decore_base/sample/config.json
 decore_base/sample/language.json
 decore_base/sample/.vscode/launch.json
 decore_base/sample/.vscode/settings.json
```

### Comparing `decore_Base-0.0.23/decore_Base.egg-info/requires.txt` & `decore_Base-0.0.24/decore_Base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_list.py` & `decore_Base-0.0.24/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_model.py` & `decore_Base-0.0.24/decore_base/decore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,375 +1,384 @@
-import inspect
-import logging
-import operator
-from functools import reduce
-from pathlib import Path, PosixPath, WindowsPath
-from shutil import move
-from uuid import uuid1
-
-from cerberus import Validator
-from peewee import *
-from peewee import FieldAccessor, MetaField
-from playhouse.migrate import *
-from playhouse.reflection import Introspector
-from playhouse.shortcuts import model_to_dict
-from pykeepass.entry import Entry
+from .classes.decore_action import Decore_action
+from .classes.decore_app import Decore_app
+from .classes.decore_base import Decore_base
+from .classes.decore_dialog import Decore_dialog
+from .classes.decore_element import Decore_element
+from .classes.decore_function import Decore_function
+from .classes.decore_model import Decore_model
+from .classes.decore_pool import Decore_pool
+from .classes.decore_query import Decore_query
+from .classes.decore_view import Decore_view
+from .classes.decore_widget import Decore_widget
+from .classes.decore_prompt import Decore_prompt
 
-from ..globals import globals
-from .decore_translate import Decore_translate as t
+from . import globals
 
+from playhouse.shortcuts import model_to_dict
+from uuid import uuid1
+from typing import Literal
+from time import perf_counter
 
-class PasswordFieldAccessor(object):
-    def __init__(self, model, field, name):
-        self.model = model
-        self.field = field
-        self.name = name
-    #TODO - alles nochmal durch debuggen SET und GET
-    def __get__(self, instance, instance_type=None):
-        if instance is not None:
-            t_entry = None
-            # MEMO - Suche nach einem Eintrag der dem Identifiziern entspricht und gebe das Password des Eintrages zurück
-            for entry in instance.kdb_group.entries:
-                if entry.title == self.name and entry.username == instance.id:
-                    return entry.password
-            # MEMO - Wenn kein Eintrag vorhanden ist, gebe None als Passwort aus
-            if not t_entry: #TODO - diese Zeile kann wahrscheinlich weg, einfach nur return None wenn bei Schleifenabarbeitung nichts zurückgegeben wird
-                return None
-        return self.field
-
-    def __set__(self, instance, value):
-        instance.kdb_group = instance.__class__().kdb_group
-        if instance.id:
-            t_entry = None
-            # MEMO - Suche nach einem Eintrag der dem Identifiziern entspricht 
-            for entry in instance.kdb_group.entries:
-                if entry.title == self.name and entry.username == instance.id:
-                    t_entry = entry
-            # MEMO - Wenn kein Eintrag vorhanden ist, lege einen neuen an und füge diesen der Gruppe hinzu
-            if not t_entry:
-                t_entry = Entry(title=self.name, username=instance.id, password=value, kp=globals.kdb)
-                instance.kdb_group.append(t_entry)
-                globals.kdb.save()
-            # MEMO - Wenn der neue Wert nicht mit dem Password im Entry übereinstimmt und auch nicht mit der UUID dann ändere und speichere
-            if not value == t_entry.password and not value == str(t_entry.uuid):
-                t_entry.password = value
-                globals.kdb.save()
-            # MEMO - schreibe die UUID des Entries in das __data__ Dict um das Kennwort zu verschleiern
-            instance.__data__[self.name] = str(t_entry.uuid)
+from flask import Flask, render_template, request, jsonify, send_file
+from flask_wtf.csrf import generate_csrf
+from flask_cors import CORS
+
+import json, logging
+from str2type import str2type
+from pathlib import Path
+from collections import OrderedDict
+
+
+class Decore(object):
+    def __init__(self):
+        if not globals.flags.production_mode:
+            self.prompt = Decore_prompt()
+        self.pool = Decore_pool()
+        self.api = self.get_api()
+        Decore_query.create_table(safe=True)
+        
+    def get_api(self):
+        t_static_folder = Path('spa/static')
+        t_template_folder = Path('spa/templates')
+        api = Flask(__name__, static_folder=t_static_folder.absolute(), template_folder=t_template_folder.absolute())
+        
+        if globals.flags.dev_mode:
+            CORS(api, expose_headers=["Content-Disposition"])
+            
+        elif not globals.flags.dev_mode: 
+            api.config['SECRET_KEY'] = '325245hkhf486axcv5719bf9397cbn69xv'
+            api.config['WTF_CSRF_ENABLED'] = False  # TODO - csrf enable when not cors
+        
+        # print('APP_ROOT_FOLDER >> ' + str(api.root_path))
+        # print('STATIC_FOLDER >> ' + str(api.static_folder))
+        # print('TEMPLATE_FOLDER >> ' + str(api.template_folder))
+        api.add_url_rule('/', 'index', self.index, defaults={'p_path': ''})
+        api.add_url_rule('/<path:p_path>', 'index', self.index)
+        api.add_url_rule('/get_meta', 'get_meta', self.get_meta)
+        api.add_url_rule('/get_default/<p_source_id>', 'get_default', self.get_default)
+        api.add_url_rule('/get_last/<p_source_id>', 'get_last', self.get_last)
+        api.add_url_rule('/post_item_s/<p_source_id>', 'post_item_s', self.post_item_s, methods=['POST'])
+        api.add_url_rule('/post_option_s/<p_source_id>', 'post_option_s', self.post_option_s, methods=['POST'])
+        api.add_url_rule('/post_action/<p_action_id>', 'post_action', self.post_action, methods=['POST'])
+        api.add_url_rule('/get_query_s', 'get_query_s', self.get_query_s)
+        api.add_url_rule('/post_save_query/<p_base_id>/<p_view_id>', 'post_save_query', self.post_save_query, methods=['POST'])
+        api.add_url_rule('/get_remove_query/<p_id>', 'get_remove_query', self.get_remove_query)
+        return api
+
+    def start_api(self):
+        import os, sys
+        from waitress import serve
+        HOST = os.environ.get('SERVER_HOST', 'localhost')
+        try:
+            PORT = int(os.environ.get('SERVER_PORT', str(globals.config.app_port)))
+        except ValueError:
+            PORT = globals.config.app_port
+        
+        if not globals.flags.dev_mode:
+            logger = logging.getLogger('waitress')
+            logger.info(self.pool.app.title + ' now running on: http://' + str(HOST) + ':' + str(PORT))
+            logger.info('Press CTRL+C to quit.')
+            logger.setLevel(logging.WARNING)
+            serve(self.api, host=HOST, port=PORT)
+            
         else:
-            logging.error('%s > %s' % (self.name, 'u get no password while ur item id was not setted'))
-            instance.__data__[self.name] = None
-        instance._dirty.add(self.name)
-
-class FileFieldAccessor(object):
-    def __init__(self, model, field, name):
-        self.model = model
-        self.field = field
-        self.name = name
-
-    def __get__(self, instance, instance_type=None):
-        if instance is not None:
-            t_path = Path(globals.config['default']['state_path']).joinpath('filebase').joinpath(self.model.__name__).joinpath(instance.id).joinpath(self.name).joinpath(instance.__data__.get(self.name))
-            if t_path.exists():
-                return t_path.absolute()
-            else:
-                return None
-        return self.field
+            self.api.run(HOST, PORT)
 
-    def __set__(self, instance, value):
-        if instance.id:
-            if type(value) == WindowsPath or type(value) == PosixPath:
-                t_path = Path(globals.config['default']['state_path']).joinpath('filebase').joinpath(self.model.__name__).joinpath(instance.id).joinpath(self.name).joinpath(value.name)
-                t_path.parent.mkdir(parents=True, exist_ok=True)
-                move(value, t_path)
-                instance.__data__[self.name] = value.name
+    def app(self, title):
+        '''Decorator for app registration'''
+        def wrapper(func):
+            self.pool.register(Decore_app('app', None, None, None, title, None, func.__doc__))
+            self.pool.extend()
+            i_base: Decore_base
+            for i_base in self.pool.base_s:
+                i_base.start_shot()
+                i_base.start_work()
+            self.start_api()
+        return wrapper
+
+    def base(self, icon=None, title=None, desc=None, model=Decore_model):
+        def wrapper(cls):
+            t_base = Decore_base(cls.__name__, icon, title, desc, model)
+            t_base.__class__ = type(cls.__name__, (Decore_base, cls), {
+                '__init__': cls.__init__(t_base),
+            })
+            self.pool.register(t_base)
+        return wrapper
+
+    l_view_type = Literal['table']
+    l_view_pag_type = Literal['client']
+
+    def view(self, parent_id=None, icon=None, title=None, desc=None, type: l_view_type = 'table', fields=[], filters=[], query={}, pag_type: l_view_pag_type = 'client', pag_recs=16):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            if not parent_id:
+                t_parent_id = t_parent_s[-2]
             else:
-                instance.__data__[self.name] = value
-        else:
-            logging.error('%s > %s' % (self.name, 'u can not store files while ur item id was not setted'))
-            instance.__data__[self.name] = None
-        instance._dirty.add(self.name)
-
-class PasswordField(Field):
-    accessor_class = PasswordFieldAccessor
-    field_type = 'VARCHAR'
+                t_parent_id = parent_id
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_view(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, fields, filters, query, pag_type, pag_recs))
+            func()
+        return wrapper
+
+    l_dialog_type = Literal['standard', 'tabs', 'stepper']
+    l_dialog_display = Literal['modal', 'drawer']
+    l_dialog_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
+
+    # TODO - Überprüfen ob element mit gleicher ID schon vorhanden ist und Execption
+    def dialog(self, parent_id=None, icon=None, title=None, desc=None, type: l_dialog_type = 'standard', display: l_dialog_display = 'drawer', activator: l_dialog_activator = 'none'):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            if not parent_id:
+                t_parent_id = t_parent_s[-2]
+            else:
+                t_parent_id = parent_id
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_dialog(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, display, activator))
+            func()
+        return wrapper
+
+    l_widget_type = Literal['default', 'info', 'form', 'table']
+
+    def widget(self, parent_id=None, icon=None, title=None, desc=None, type: l_widget_type = 'default', layout='cera', fields=[]):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            if not parent_id:
+                t_parent_id = t_parent_s[-2]
+            else:
+                t_parent_id = parent_id
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_widget(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, layout, fields))
+            func()
+        return wrapper
+
+    l_element_type = Literal['p', 'checkbox']
+
+    def element(self, parent_id=None, icon=None, title=None, desc=None, type: l_element_type = 'text', default=None, disable=False, schema=None):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            if not parent_id:
+                t_parent_id = t_parent_s[-2]
+            else:
+                t_parent_id = parent_id
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_element(func.__name__, t_parent_id, t_source_id, icon, title, desc, type, default, disable, schema, func))
+        return wrapper
+
+    l_action_type = Literal['standard', 'submit', 'check', 'response', 'file', 'download']
+    l_action_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
+
+    def action(self, parent_id=None, icon=None, title=None, desc=None, type: l_action_type = 'standard', activator: l_action_activator = 'none'):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            if not parent_id:
+                t_parent_id = t_parent_s[-2]
+            else:
+                t_parent_id = parent_id
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_action(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, activator, func))
+        return wrapper
+
+    l_function_type = Literal['shot', 'work']
+  
+    def function(self, type:l_function_type = 'shot'):
+        def wrapper(func):
+            t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
+            t_parent_id = t_parent_s[-2]
+            t_source_id = t_parent_s[0]
+            self.pool.register(Decore_function(func.__name__, t_parent_id, t_source_id, None, None, None, func.__doc__, type, func))
+        return wrapper
+
+    def get_base_by_id(self, p_id):
+        i_base: Decore_base
+        for i_base in self.pool.base_s:
+            if i_base.id == p_id:
+                return i_base
+
+    def get_base_by_model(self, p_model) -> Decore_base:
+        i_base: Decore_base
+        for i_base in self.pool.base_s:
+            if i_base.model == p_model:
+                return i_base
+
+    def get_base_by_module(self, p_module):
+        i_base: Decore_base
+        for i_base in self.pool.base_s:
+            if i_base.__module__ == p_module:
+                return i_base
     
-class FileField(Field):
-    accessor_class = FileFieldAccessor
-    field_type = 'VARCHAR'
-
-class ManyToManyField(ManyToManyField):
-    def __init__(self, model, backref=None, on_delete=None, on_update=None, _is_backref=False, verbose_name=None, help_text=None, filter_fields=None):
-        super().__init__(model, backref, on_delete, on_update, _is_backref)
-        self.verbose_name = verbose_name
-        self.help_text = help_text
-        self.filter_fields = filter_fields
+    #### Api methods ####
+
+    def index(self, p_path):
+        return render_template('index.html', port=globals.config.app_port)
     
-class BackRefMetaField(MetaField):
-    def __init__(self,verbose_name=None, help_text=None, filter_fields=None):
-        super().__init__(False, False, False, None, None, False, None, None, None, False, None, help_text, verbose_name, None, None, False)
-        self.filter_fields = filter_fields
+    def get_meta(self):
+        return jsonify(self.pool.export())
     
-    def bind(self, model, name, set_attribute):
-        super().bind(model, name, set_attribute)
-        setattr(model,'br_'+name, getattr(model, name)) 
-        delattr(model, name)
-
-class Decore_model(Model):
-    id = CharField(primary_key=True, unique=True, verbose_name="ID")
-    title = CharField(verbose_name=t('Title'))
-    desc = CharField(verbose_name=t('Description'), null=True)
-    item_type = CharField(verbose_name=t('Item type'), default='object')
-    parent_path = CharField(verbose_name=t('Parent path'), null=True)
+    def get_default(self, p_source_id):
+        t_source = self.pool.__data__[p_source_id]
+        t_item = t_source.model().__data__
+        return jsonify(t_item), 200
     
-    class Meta:
-        # tbase = SqliteDatabase('state/database.db', pragmas=(('cache_size', -1024 * 64),('journal_mode', 'wal')))
-        tbase = SqliteDatabase('state/database.db')
-
-    def __init__(self, *args, **kwargs):
-        Model.__init__(self, *args, **kwargs)
-        self.kdb_group = self.get_kdb_group()
-        if not self.id:
-            self.id = self.create_uuid()
-
-    @classmethod
-    def register(cls):
-        if cls._meta.database:
-            cls.create_table(safe=True)
-        for field in cls._meta.manytomany.values():
-            through_model = field.get_through_model()
-            cls._meta.tbase.create_tables([through_model])
-        return cls
-
-    @classmethod
-    def migrate_database(cls):
-        t_introspector = Introspector.from_database(cls._meta.database)
-        t_database_model = t_introspector.generate_models(table_names=cls._meta.table_name)[cls._meta.table_name]
-        
-        for cls_field in cls._meta.fields.values():
-            b_cls_field_found = False
-            for db_field in t_database_model._meta.fields.values():
-                if cls_field.column_name == db_field.column_name:
-                    b_cls_field_found = True
-                    break
-            if not b_cls_field_found:
-                migrate(cls._meta.migrator.add_column(cls._meta.table_name, cls_field.column_name, cls_field))
-        
-        if globals.flags.purge_unused_database_cols:
-            for db_field in t_database_model._meta.fields.values():
-                b_db_field_found = False
-                for cls_field in cls._meta.fields.values():
-                    if db_field.column_name == cls_field.column_name:
-                        b_db_field_found = True
-                        break
-                if not b_db_field_found:
-                    migrate(cls._meta.migrator.drop_column(cls._meta.table_name, db_field.column_name, cascade=False))
-
-    @classmethod
-    @property
-    def field_s(cls):
-        return list(cls._meta.fields.values())
-
-    @classmethod
-    @property
-    def rel_field_s(cls):
-        r_value = []
-        for field in cls._meta.backrefs:
-            if not 'Through' in field.model.__name__:
-                r_value.append(field)
-        for field in cls._meta.manytomany.values():
-            r_value.append(field)
-        return r_value
+    def get_last(self, p_source_id):
+        t_source = self.pool.__data__[p_source_id]
+        if not len(t_source.model.select()) == 0:
+            t_item = t_source.model.select()[-1].__data__
+            return jsonify(t_item), 200
+        else:
+            return self.get_default(p_source_id)
+
+    def post_item_s(self, p_source_id):
+        t_start = perf_counter()
+        t_query = json.loads(request.data)
+        t_source = self.pool.__data__[p_source_id]
+        t_item_s = t_source.model.get_dict_s(t_query)
+        t_end = perf_counter()
+        logging.info('%s > %s %s' % ('dict_s created in', t_end - t_start, 'seconds'))
+        return jsonify(t_item_s), 200
     
-    @classmethod
-    @property
-    def full_field_s(cls):
-        r_value = []
-        for value in cls.__dict__.values():
-            if FieldAccessor in inspect.getmro(value.__class__):
-                r_value.append(value.field)
-        return r_value
+    def post_option_s(self, p_source_id):
+        t_start = perf_counter()
+        t_data = json.loads(request.data)
+        t_query = t_data['query']
+        t_attr = t_data['attr']
+        t_rel_attr = t_data['rel_attr']
+        t_source = self.pool.__data__[p_source_id]
+        t_option_s = t_source.model.get_option_s(t_query, t_attr, t_rel_attr)
+        t_end = perf_counter()
+        logging.info('%s > %s %s' % ('option_s created in', t_end - t_start, 'seconds'))
+        return jsonify(t_option_s), 200
     
-    @classmethod
-    @property
-    def verbose_names(cls):
-        r_value = {}
-        for field in cls.full_field_s:
-            if not hasattr(field, 'ref_name') and hasattr(field, 'verbose_name'):
-                r_value[field.name] = str(field.verbose_name)
-            elif hasattr(field, 'ref_name'):
-                r_value[field.ref_name] = str(field.verbose_name)
-        return r_value
-
-    @classmethod
-    def build_schema(cls):
-        t_schema = {}
-        for i_field in cls.field_s:
-         
-            if i_field.field_type == 'VARCHAR' and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'string'}
-
-            if i_field.field_type == 'TEXT'and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'string'}
-
-            if i_field.field_type == 'BOOL'and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'boolean'}
-
-            if i_field.field_type == 'INT'and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'integer'}
-
-            if i_field.field_type == 'DATETIME'and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'datetime'}
-
-            if i_field.field_type == 'FLOAT'and i_field.null == False:
-                t_schema[i_field.name] = {'type': 'float'}
-
-        return t_schema
-
-    @classmethod
-    def query(cls, p_query={}):
-        r_item_s = cls.select()
-        t_mm_query = {}
-        for key, value in p_query.items():         
-            t_query_attr_s = key.split('__')
-            t_field = t_query_attr_s[0]
-            if t_field in cls._meta.manytomany.keys():
-                t_rel_field = t_query_attr_s[1]
-                t_operator =  t_query_attr_s[2]                
-                t_mm_query.setdefault(t_field, []).append({'operator': t_operator, 'field': t_rel_field,  'value': value})
-            else:
-                if type(value) is list:
-                    t_exp = None
-                    for item in value:
-                        t_exp |= DQ(**{key: item})
-                    r_item_s = r_item_s.filter(t_exp)
+    def post_action(self, p_action_id):
+        t_action = self.pool.__data__[p_action_id]
+        t_data = dict()
+        if request.data:
+            t_data.update(json.loads(request.data))
+        #OUT request.form wird nicht benötigt
+        if request.form:
+            t_data.update(json.loads(request.form['value']))
+        if request.files:
+            for key, value in request.files.items():
+                # TODO - temporyry aus config.json verwenden
+                t_path = Path('temporary').joinpath(value.filename)
+                t_path.parent.mkdir(parents=True, exist_ok=True)
+                value.save(t_path)
+                t_data['item'][key] = t_path
 
-                elif type(value) is str:
-                    r_item_s = r_item_s.filter(**{key: value})
-                else:
-                    raise Exception('Type error in query value')
-        
-        for key, value in t_mm_query.items():   
-            t_rel_model = cls._meta.manytomany[key].rel_model
-            t_through_model = cls._meta.manytomany[key]._through_model
-            r_item_s = r_item_s.join(t_through_model).join(t_rel_model)
-            for i_attrs in value:
-                t_operator = i_attrs['operator']
-                t_field = i_attrs['field']
-                t_value = i_attrs['value']
-                if t_operator == 'eq':
-                    if type(t_value) is list:
-                        t_clause_s = []
-                        for item in t_value:
-                            t_clause_s.append((getattr(t_rel_model, t_field) == item))
-                        t_exp = reduce(operator.or_, t_clause_s)
-                        r_item_s = r_item_s.where(t_exp)
-                    elif type(t_value) is str:
-                        r_item_s = r_item_s.where(getattr(t_rel_model, t_field) == t_value)
-                    else:
-                        raise Exception('Type error in query value')
-        
-        return r_item_s
+        t_return = t_action.func(self.pool.__data__[t_action.source_id], t_data)
 
-    @classmethod
-    def get_dict_s(cls, p_query=None, p_pag=None):
-        t_dict_s = []
-        t_item_s = None
+        if t_action.type == 'standard':
+            return {'success': t_return[0], 'result': str(t_return[1])}, 200
         
-        #MEMO - Relationale Daten abrufen
-        t_rel = {}
-        for i_field in cls.field_s:
-            if type(i_field) == ForeignKeyField:
-                t_rel[i_field.name] = {}
-                for i_value in i_field.rel_model.select().dicts():
-                    t_rel[i_field.name][i_value['id']] = i_value
-        
-        #MEMO - Query anwenden
-            t_item_s = cls.query(p_query)
+        if t_action.type == 'submit':
+            return {'success': t_return[0], 'result': str(t_return[1])}, 200
 
-        #MEMO - Items mit relationalen Daten erweitern
-        for i_item in t_item_s.dicts():
-            for i_field in cls.field_s:
-                if type(i_field) == ForeignKeyField:
-                    i_item[i_field.name]=t_rel[i_field.name][i_item[i_field.name]]
-            
-            if not i_item in t_dict_s:
-                t_dict_s.append(i_item)
+        elif t_action.type == 'check':
+            return {'success': t_return}, 200
+
+        elif t_action.type == 'file':
+            t_path = Path(t_return)
+            return send_file(t_path, download_name=t_path.name)
         
-        return {'item_s': t_dict_s, 'count': t_item_s.count()}
+    def get_query_s(self):
+        def expand():
+            for i_query in t_query_s:
+                i_query['children'] = []
+                for i2_query in t_query_s:
+                    if i2_query['parent'] and i_query['id'] == i2_query['parent']['id']:
+                        i_query['children'].append(i2_query)
+
+        t_query_s = []
+        for i_query in Decore_query.select():
+            t_query_s.append(model_to_dict(i_query))
+
+        expand()
+
+        return jsonify(t_query_s)
+    
+    def post_save_query(self, p_base_id, p_view_id):
+
+        # TODO - sorted DICT wieder einsetzen - p_query = OrderedDict(sorted((json.loads(request.data)).items()))
+        p_query = json.loads(request.data)
+
+        def get_url_query():
+            if t_parent.id:
+                r_parent_to:dict = json.loads(t_parent.to)
+                r_parent_to['query'][i_query_key] = i_query_value
+                return r_parent_to
+            elif not t_parent.id:
+                return {'path': '/' + p_base_id + '/' + p_view_id, 'query': {i_query_key: i_query_value}}
+
+        # def get_title():
+        #     t_title_key = ''
+        #     t_title_value = i_query_value
+
+        #     i_view: Decore_view
+        #     for i_view in self.view_s:
+        #         if p_view_id == i_view.id:
+        #             t_model = self.get_base_by_id(i_view.source_id).model
+        #             for i_field_key, i_field_value in t_model._meta.fields.items():
+        #                 if i_query_key == i_field_key:
+        #                     t_title_key = i_field_value.verbose_name
+        #                     if 'ForeignKeyField' in str(i_field_value.__class__):
+        #                         t_title_value = i_field_value.rel_model.get(
+        #                             i_field_value.rel_model.id == i_query_value).title
+
+        #     return t_title_key+"="+t_title_value
+
+        t_parent = Decore_query()
+
+        for i_query_key, i_query_value in p_query.items():
+            # TODO - t_item = Decore_query.get_or_none(Decore_query.parent_id == t_parent.id and Decore_query.base_id == p_base_id and Decore_query.view_id == p_view_id and Decore_query.key == key and Decore_query.value == value)
+            t_item = None
+            i_item: Decore_query
+            for i_item in Decore_query.select():
+                if i_item.base_id == p_base_id:
+                    if i_item.view_id == p_view_id:
+                        if i_item.key == i_query_key:
+                            if json.loads(i_item.value) == i_query_value:
+                                if i_item.parent_id == t_parent.id:
+                                    t_item = i_item
 
-    @classmethod
-    def get_option_s(cls, p_query, p_attr, p_rel_attr):
-        r_value = []
-        t_item_s = cls.query(p_query)
-        for item in t_item_s:
-            if p_rel_attr:
-                t_attr = getattr(item, p_attr) 
-                try:
-                    for rel_item in t_attr:
-                        t_value = rel_item.__data__[p_rel_attr]
-                        if not t_value in r_value:
-                            r_value.append(t_value)
-                except TypeError as error:
-                    t_value = t_attr.__data__[p_rel_attr]
-                    if not t_value in r_value:
-                        r_value.append(t_value)
-            else:
-                t_value = item.__data__[p_attr]
-                if not t_value in r_value:
-                    r_value.append(t_value)
-        return r_value
-
-    def get_kdb_group(self):
-        t_group = globals.kdb.find_groups_by_name(self.__class__.__name__, group=globals.kdb.root_group, first=True)
-        if not t_group:
-            t_group = globals.kdb.add_group(globals.kdb.root_group, self.__class__.__name__)
-            globals.kdb.save()
-        return t_group
-
-    def validate(self):
-        t_schema = self.build_schema()
-        #TODO - Schema as property and Validator as attribute in model
-        t_val = Validator(t_schema, require_all=True, allow_unknown = True)
-        r_value =  t_val.validate(self.__data__)
-        if r_value == False:
-            logging.error('%s > %s' % ('validate_model', str(t_val.errors)))
-        return r_value
-
-    # TODO - Wer ruft das auf? was ist damit?
-    def to_dict(self):
-        return model_to_dict(self, recurse=True, max_depth=1)
-
-    #TODO - return values prüfen; werden die eigentlich benötigt? > save_item
-    def save(self):
-        if self.validate():
-            t_item = self.__class__.get_or_none(self.__class__.id == self.id)
             if not t_item:
-                if super(Decore_model,self).save(force_insert=True):
-                    return True
+                t_item = Decore_query()
+                t_item.id = str(uuid1())
+                t_item.parent = t_parent
+                t_item.base_id = p_base_id
+                t_item.view_id = p_view_id
+                t_item.title = str(i_query_key +':'+ str(i_query_value))
+                t_item.key = i_query_key
+                t_item.value = json.dumps(i_query_value)
+                t_item.to = json.dumps(get_url_query())
+                t_item.depth = t_parent.depth + 1 if t_parent.id else 0
+                if t_item.save(force_insert=True):
+                    t_parent = t_item
                 else:
-                    logging.error('%s > %s' % ('save_item', 'Insert error'))
-                    return False
+                    return 'error', 200
             elif t_item:
-                # t_data = {k: v for k, v in t_item.__data__.items() if v is not None}
-                if not self.__data__ == t_item.__data__:
-                    if self.save():
-                        return True
-                    else:
-                        logging.error('%s > %s' % ('save_item', 'Update error'))
-                        return False
-                else:
-                    return True
-        else:
-            logging.error('%s > %s' % ('save_item', 'Validation error'))
-            return False
+                t_parent = t_item
 
-    #TODO - return values prüfen; werden die eigentlich benötigt? > delete_instance
-    def delete_instance(self):
-        if self(Decore_model, self).delete_instance():
-            return True
+        return 'success', 200
+
+
+    def get_remove_query(self, p_id):
+        t_query_item = Decore_query.get_or_none(Decore_query.id == p_id)
+        if t_query_item:
+            t_query_item.delete_instance(recursive=True, delete_nullable=True)
+            return 'success', 200
         else:
-            logging.error('%s > %s' % ('remove_item', 'Remove error'))
-            return False
-    
-    def create_uuid(self):
-        return str(uuid1())
+            return 'error', 200
+        
+decore = Decore()
+
+# @api.route('/get_uniform')
+# def get_uniform():
+#     t_uniform = uniform.export()
+#     t_uniform['csrf_token'] = generate_csrf()
+#     return jsonify(t_uniform), 200
+
+# @api.route('/element/<p_widget_id>/<p_element_id>', methods=['POST'])
+# def element(p_widget_id, p_element_id):
+#     t_widget = uniform.widget_s.get_by_id(p_widget_id)
+#     t_element = t_widget.element_s.get_by_id(p_element_id)
+#     t_data = json.loads(request.data)
+#     t_return = t_element.func(uniform.get_base_by_module(t_element.func.__module__), t_data)
+#     return json.dumps(t_return)
```

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_pool.py` & `decore_Base-0.0.24/decore_base/classes/decore_pool.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.24/decore_base/classes/decore_prompt.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_query.py` & `decore_Base-0.0.24/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_return.py` & `decore_Base-0.0.24/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_translate.py` & `decore_Base-0.0.24/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/classes/decore_view.py` & `decore_Base-0.0.24/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/globals.py` & `decore_Base-0.0.24/decore_base/globals.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.24/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/powershell.py` & `decore_Base-0.0.24/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/powershell2.py` & `decore_Base-0.0.24/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/return_value.py` & `decore_Base-0.0.24/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.24/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.24/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.24/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/.gitignore` & `decore_Base-0.0.24/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/.vscode/launch.json` & `decore_Base-0.0.24/decore_base/prepare/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.24/decore_base/prepare/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.24/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.24/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.24/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.24/decore_base/sample/spa/static/js/586.aa14c175.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.24/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.24/decore_base/sample/spa/static/js/app.af6cbe84.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.24/decore_base/sample/spa/static/js/vendor.0902ddb5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.24/decore_base/sample/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/.gitignore` & `decore_Base-0.0.24/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/.vscode/launch.json` & `decore_Base-0.0.24/decore_base/sample/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/bases/account_base.py` & `decore_Base-0.0.24/decore_base/sample/bases/account_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from decore_base import decore
 from models.account_model import Account_model as Model
 
 @decore.base(title='Accounts', model=Model)
-class Account_base(object):
+class Account_base:
     @decore.widget(parent_id='per_vi1_di1_wi1', title='Accounts' , type='table', fields=[Model.title, Model.email])
     def per_vi1_di1_wi1_wi1():
         pass
 
     @decore.view(parent_id='Information_system_base', title='Accounts',icon='mdi-account-circle-outline', type='table', fields=Model.field_s, filters=[Model.password ,Model.person])
     def acc_vi1():
         pass
```

### Comparing `decore_Base-0.0.23/decore_base/sample/bases/company_base.py` & `decore_Base-0.0.24/decore_base/sample/bases/company_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from decore_base import decore
 from models.company_model import Company_model as Model
 
 @decore.base(title='Companies', model=Model)
-class Company_base(object):
+class Company_base:
     
     @decore.widget(parent_id='per_vi1_di1_wi1', title='Companies', type='table', fields=Model.field_s)
     def per_vi1_di1_wi1_wi2():
         pass
 
     @decore.view(parent_id='Global_management_base', title='Companies', icon='mdi-domain', fields=Model.field_s)
     def com_vi1():
```

### Comparing `decore_Base-0.0.23/decore_base/sample/bases/global_management_base.py` & `decore_Base-0.0.24/decore_base/sample/bases/global_management_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,43 +6,51 @@
 
 from mimesis import Person, Finance
 from random import randrange
 
 @decore.base(title='Global Management', icon='mdi-account-supervisor-circle-outline')
 class Global_management_base:
     def __init__(self):
+        self.test_attr = 'test_attr'
+        pass
+
+    @decore.function(type='shot')
+    def create_data(self):
         self.test_item()
-        # self.query_tester()
+        self.query_tester()
         self.create_company_s()
         self.create_person_s()
-        self.set_company_person()
+        # self.set_company_person()
     
     def test_item(self):
-        t_person_s = Person_model.select()[0]
-        t_person = Person_model()
+        t_account = Account_model()
+        t_account.title = 'test'
+        t_account.email = 'test@mail.com'
+        t_account.password = 'test'
+        t_account.save()
+        t_account_s = list(Account_model.select())
         pass
 
     # Query tester
     def query_tester(self):
         t_item_s = Person_model.query({'companies__title__eq':'NetApp'})
         pass
 
     # Create 32 companies with capacity 16-128 of persons
     def create_company_s(self):
         while len(Company_model.select()) < 32:
             t_finance = Finance()
             t_item = Company_model()
-            t_item.id = t_item.create_uuid()
             t_item.title = t_finance.company()
             t_item.capacity = randrange(16, 128)
             t_item.save()
 
     # Create 4096 persons with capacity 1-2 of companies
     def create_person_s(self):        
-        while len(Person_model.select()) < 4500:
+        while len(Person_model.select()) < 32:
             t_item = Person_model()
             t_item.title = t_item.first_name + ' ' + t_item.last_name
             t_item.save()
 
     # Set persons to companies
     def set_company_person(self):
         for company in Company_model.select():
```

### Comparing `decore_Base-0.0.23/decore_base/sample/bases/person_base.py` & `decore_Base-0.0.24/decore_base/sample/bases/person_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from decore_base import decore
-from decore_base.classes.decore_base import Decore_base as Base
 from models.person_model import Person_model as Model
 
 @decore.base(title='Person', model=Model)
-class Person_base(Base):
-    
+class Person_base:
     @decore.widget(parent_id='com_vi1_di1', title='Persons', type='table', fields=Model.field_s)
     def com_vi1_di1_wi1():
         pass
-
     @decore.view(parent_id='Global_management_base', title='Persons', icon='mdi-account-group-outline', type='table', fields=Model.field_s, filters=[Model.academic_degree, Model.companies, Model.accounts])
     def per_vi1():
-        
         @decore.dialog(title='Add person...', icon='mdi-plus' , type='standard', activator='default-menu')
         def per_vi1_di3():
             @decore.widget(type='form', fields=[Model.first_name, Model.last_name, Model.academic_degree, Model.age, Model.capacity])
             def per_vi1_di3_wi1():
                 @decore.action(type='submit')
                 def per_vi1_di3_wi1_ac1(self, p_data):
                     t_item = Model(p_data['item'])
                     t_item.title = t_item.first_name + ' ' + t_item.last_name
-                    return True, 'Success!'
-        
+                    if t_item.save():
+                        return True, 'Success!'
+                    else:
+                        return False, 'Error!'
         @decore.action(title='Test action', icon='mdi-test-tube', type='standard', activator='default-menu')
         def per_vi1_ac1(self, p_data):
             return True, 'Success!'
-
         @decore.dialog(title='Person', type='standard', display='drawer', activator='item-click')
         def per_vi1_di1():
             @decore.widget(title='Informations', type='info', fields=Model.field_s)
             def per_vi1_di1_wi1():
                 @decore.dialog(title='Edit Person', icon='mdi-pencil', type='standard', display='drawer', activator='item-menu')
                 def per_vi1_wi1_di1():
                     @decore.widget(type='form', fields=[Model.first_name, Model.last_name])
                     def per_vi1_di1_wi1_di1_wi1():
                         @decore.action(type='submit')
                         def per_vi1_di1_wi1_di1_wi1_ac1(self, p_data):
                             return True, 'Success!'
-        
         @decore.dialog(title='Edit Person', icon='mdi-pencil', type='standard', display='drawer', activator='item-menu')
         def per_vi1_di2():
             @decore.widget(type='form', fields=[Model.first_name, Model.last_name])
             def per_vi1_di2_wi1():
                 @decore.action(type='submit')
-                def per_vi1_di2_wi1_ac1(self, p_data):
-                    return True, 'Success!'
+                def per_vi1_di2_wi1_ac1(self, data):
+                    t_item = Model(**data['item'])
+                    if t_item.save():
+                        return True, 'Success!'
+                    else:
+                        return False, 'Error!'
```

### Comparing `decore_Base-0.0.23/decore_base/sample/bases/test_base.py` & `decore_Base-0.0.24/decore_base/sample/bases/test_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/models/person_model.py` & `decore_Base-0.0.24/decore_base/sample/models/person_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/models/test_model.py` & `decore_Base-0.0.24/decore_base/sample/models/test_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.24/decore_base/sample/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.24/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.24/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/favicon.ico` & `decore_Base-0.0.24/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.24/decore_base/prepare/spa/static/js/586.6cfbf2b5.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniform_front"] = globalThis["webpackChunkuniform_front"] || []).push([
     [586], {
         1586: (e, t, l) => {
             l.r(t), l.d(t, {
-                default: () => tl
+                default: () => ul
             });
             var a = l(9835),
                 s = l(499),
                 i = (l(9665), l(5360)),
                 o = l(8339);
             class n extends i.y {
                 constructor(e) {
@@ -24,15 +24,15 @@
                         this.route_dialog_s.push(e), e.widget_s.forEach((e => {
                             this.setRouteDialogs(e)
                         }))
                     }))
                 }
             }
             var u = l(4629);
-            class c extends i.y {
+            class d extends i.y {
                 constructor(e) {
                     super(e), this.ql = {}, this.action_store = (0, u.j)(), this.context = "none", this.show = !1, this.has_submit_btn = !1, this.has_close_btn = !1
                 }
                 setSubmitBtn() {
                     let e = !1;
                     this.widget_s.forEach((t => {
                         t.action_s.forEach((t => {
@@ -73,23 +73,23 @@
                     this.show = !1, this.widget_s.forEach((e => {
                         this.ref[e.id].reset(), e.widget_s.forEach((e => {
                             this.ref[e.id].reset()
                         }))
                     }))
                 }
             }
-            var d = l(6970),
+            var c = l(6970),
                 r = l(5288);
             const m = {
                     class: "dialog-content"
                 },
-                h = {
+                p = {
                     inheritAttrs: !1
                 },
-                p = Object.assign(h, {
+                h = Object.assign(p, {
                     __name: "uf-dialog-layout",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, a.Fl)((() => {
                                 let e = "none";
                                 return t.show && (e = "block"), e
                             }));
@@ -97,57 +97,57 @@
                             let e = "sub-dialog";
                             return t.ref[t.parent_id].class.includes("view") && (e = "main-dialog"), e
                         }));
                         return (e, i) => {
                             const o = (0, a.up)("q-toolbar-title"),
                                 n = (0, a.up)("q-space"),
                                 u = (0, a.up)("q-btn"),
-                                c = (0, a.up)("q-toolbar"),
-                                h = (0, a.up)("q-header"),
-                                p = (0, a.up)("q-footer"),
+                                d = (0, a.up)("q-toolbar"),
+                                p = (0, a.up)("q-header"),
+                                h = (0, a.up)("q-footer"),
                                 _ = (0, a.up)("q-layout");
                             return (0, a.wg)(), (0, a.iD)("div", {
-                                style: (0, d.j5)({
+                                style: (0, c.j5)({
                                     display: (0, s.SU)(l)
                                 })
                             }, [(0, a.Wm)(_, {
                                 container: "",
                                 style: {
                                     height: "calc(100vh - 102px)"
                                 }
                             }, {
                                 default: (0, a.w5)((() => [(0, a.Wm)(r.Z, {
                                     use: (0, s.SU)(t)
-                                }, null, 8, ["use"]), (0, a.Wm)(h, {
+                                }, null, 8, ["use"]), (0, a.Wm)(p, {
                                     reveal: ""
                                 }, {
-                                    default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                    default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                         class: "bg-grey-2"
                                     }, {
                                         default: (0, a.w5)((() => [(0, a.Wm)(o, {
                                             class: "text-black"
                                         }, {
-                                            default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)((0, s.SU)(t).title), 1)])),
+                                            default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)((0, s.SU)(t).title), 1)])),
                                             _: 1
                                         }), (0, a.Wm)(n), (0, s.SU)(t).has_close_btn ? ((0, a.wg)(), (0, a.j4)(u, {
                                             key: 0,
                                             class: "text-black",
                                             round: "",
                                             flat: "",
                                             dense: "",
                                             onClick: i[0] || (i[0] = e => (0, s.SU)(t).closeDialog()),
                                             icon: "close"
                                         })) : (0, a.kq)("", !0)])),
                                         _: 1
                                     })])),
                                     _: 1
-                                }), (0, a._)("div", m, [(0, a.WI)(e.$slots, "dialog-content")]), (0, a.Wm)(p, {
+                                }), (0, a._)("div", m, [(0, a.WI)(e.$slots, "dialog-content")]), (0, a.Wm)(h, {
                                     reveal: ""
                                 }, {
-                                    default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                    default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                         class: "bg-grey-2"
                                     }, {
                                         default: (0, a.w5)((() => [(0, s.SU)(t).has_submit_btn ? ((0, a.wg)(), (0, a.j4)(u, {
                                             key: 0,
                                             class: "text-black",
                                             label: "Submit",
                                             flat: "",
@@ -173,17 +173,17 @@
                 g = l(1663),
                 f = l(1973),
                 v = l(136),
                 b = l(8879),
                 k = l(1378),
                 y = l(9984),
                 U = l.n(y);
-            const q = p,
-                S = q;
-            U()(p, "components", {
+            const S = h,
+                q = S;
+            U()(h, "components", {
                 QLayout: _.Z,
                 QHeader: w.Z,
                 QToolbar: g.Z,
                 QToolbarTitle: f.Z,
                 QSpace: v.Z,
                 QBtn: b.Z,
                 QFooter: k.Z
@@ -207,47 +207,47 @@
                                 "onUpdate:modelValue": i[0] || (i[0] = e => (0, s.SU)(t).show = e),
                                 elevated: "",
                                 overlay: "",
                                 side: "right",
                                 breakpoint: 0,
                                 width: .5 * (0, s.SU)(l)
                             }, {
-                                default: (0, a.w5)((() => [(0, a.Wm)(S, {
+                                default: (0, a.w5)((() => [(0, a.Wm)(q, {
                                     use: (0, s.SU)(t)
                                 }, {
                                     "dialog-content": (0, a.w5)((() => [(0, a.WI)(e.$slots, "dialog-content")])),
                                     _: 3
                                 }, 8, ["use"])])),
                                 _: 3
                             }, 8, ["modelValue", "width"])) : (0, a.kq)("", !0)
                         }
                     }
                 });
             var j = l(3655);
-            const Z = D,
-                Q = Z;
+            const V = D,
+                Z = V;
             U()(D, "components", {
                 QDrawer: j.Z
             });
-            class V {
+            class Q {
                 constructor(e, t) {
                     this.source = e, this.query = t, this.search = "", this.item = {}, this.item_s = [], this.select_s = [], this.count = 0
                 }
                 setItems() {
                     this.source.getItems(this.query).then((e => {
                         this.item_s = e.data.item_s, this.count = e.data.count
                     })).catch((e => {
                         console.log(e)
                     }))
                 }
             }
-            var C = l(1809);
+            var F = l(1809);
 
-            function F(e) {
-                const t = (0, C.Q_)(e, {
+            function C(e) {
+                const t = (0, F.Q_)(e, {
                         state: () => ({
                             el: {}
                         }),
                         getters: {},
                         actions: {
                             sendElement(e, t, l, a) {
                                 let s = {
@@ -264,15 +264,15 @@
                         }
                     }),
                     l = t();
                 return l
             }
             class x extends i.y {
                 constructor(e) {
-                    super(e), this.data = (0, s.qj)(new V(this.uniform.source[this.source_id], {})), this.compose_store = F(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
+                    super(e), this.data = (0, s.qj)(new Q(this.uniform.source[this.source_id], {})), this.compose_store = C(this.id), this.action_store = (0, u.j)(), this.form_ref = void 0, this.composer_ref = void 0, this.valid = !0, this.item_s_mode = !1
                 }
                 regComposerElement(e) {
                     e.id in this.item || (this.item[e.id] = e.default), e.schema && (this.source.schema[e.id] = e.schema), this.compose_store.el[e.id] = e
                 }
                 refForm(e) {
                     this.form_ref = e
                 }
@@ -284,21 +284,21 @@
                         s = l;
                     this.data.item_s = [], "default" == a && this.data.source.getDefault().then((e => {
                         this.data.item = e.data, this.item_s_mode && this.data.setItems()
                     })), "item" == a && (this.data.source.model == s.model ? (this.data.item = {
                         ...e
                     }, this.item_s_mode && this.data.setItems()) : this.data.source.getDefault().then((t => {
                         this.data.item = t.data, s.rel_field_s.forEach((t => {
-                            if ("ForeignKeyField" == t.class && this.data.source.model == t.model) {
+                            if (t.class.includes("ForeignKeyField") && this.data.source.model == t.model) {
                                 let l = t.name + "__eq";
                                 this.data.query[l] = e.id, this.data.item[t.name] = {
                                     ...e
                                 }
                             }
-                            if ("ManyToManyField" == t.class && this.data.source.model == t.rel_model) {
+                            if (t.class.includes("ManyToManyField") && this.data.source.model == t.rel_model) {
                                 let l = t.backref + "__id__eq";
                                 this.data.query[l] = e.id
                             }
                         })), this.item_s_mode && this.data.setItems()
                     }))), "last" == a && this.data.source.getLast().then((e => {
                         this.data.item = e.data, this.item_s_mode && this.data.setItems()
                     })), this.element_s.forEach((e => {
@@ -333,21 +333,21 @@
             }
             const E = {
                     key: 0
                 },
                 H = {
                     key: 1
                 },
-                I = {
+                z = {
                     key: 2
                 },
-                K = {
+                I = {
                     key: 3
                 },
-                z = {
+                K = {
                     key: 4
                 },
                 O = {
                     key: 5
                 },
                 A = {
                     inheritAttrs: !1
@@ -364,15 +364,15 @@
                                 greedy: "",
                                 ref: e => {
                                     (0, s.SU)(t).refComposer(e)
                                 }
                             }, {
                                 default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).compose_store.el, (e => ((0, a.wg)(), (0, a.iD)("span", {
                                     key: e.id
-                                }, ["p" == e.type ? ((0, a.wg)(), (0, a.iD)("p", E, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h1" == e.type ? ((0, a.wg)(), (0, a.iD)("h1", H, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h2" == e.type ? ((0, a.wg)(), (0, a.iD)("h2", I, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h3" == e.type ? ((0, a.wg)(), (0, a.iD)("h3", K, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h4" == e.type ? ((0, a.wg)(), (0, a.iD)("h4", z, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h5" == e.type ? ((0, a.wg)(), (0, a.iD)("h5", O, (0, d.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "checkbox" == e.type ? ((0, a.wg)(), (0, a.j4)(o, {
+                                }, ["p" == e.type ? ((0, a.wg)(), (0, a.iD)("p", E, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h1" == e.type ? ((0, a.wg)(), (0, a.iD)("h1", H, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h2" == e.type ? ((0, a.wg)(), (0, a.iD)("h2", z, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h3" == e.type ? ((0, a.wg)(), (0, a.iD)("h3", I, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h4" == e.type ? ((0, a.wg)(), (0, a.iD)("h4", K, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "h5" == e.type ? ((0, a.wg)(), (0, a.iD)("h5", O, (0, c.zw)((0, s.SU)(t).item[e.id]), 1)) : (0, a.kq)("", !0), "checkbox" == e.type ? ((0, a.wg)(), (0, a.j4)(o, {
                                     key: 6,
                                     "hide-bottom-space": "",
                                     dense: "",
                                     borderless: "",
                                     modelValue: (0, s.SU)(t).item[e.id],
                                     "onUpdate:modelValue": l => (0, s.SU)(t).item[e.id] = l,
                                     rules: (0, s.SU)(t).getRules(e.id),
@@ -389,21 +389,21 @@
                                 _: 1
                             }, 512)
                         }
                     }
                 });
             var P = l(8326),
                 T = l(8149),
-                M = l(1006);
-            const B = Y,
-                R = B;
+                B = l(1221);
+            const M = Y,
+                R = M;
             U()(Y, "components", {
                 QForm: P.Z,
                 QField: T.Z,
-                QCheckbox: M.Z
+                QCheckbox: B.Z
             });
             const L = {
                     key: 0
                 },
                 N = {
                     key: 1
                 },
@@ -418,26 +418,26 @@
                     setup(e) {
                         const t = (0, a.l1)().use;
                         return (e, l) => {
                             const i = (0, a.up)("q-space"),
                                 o = (0, a.up)("q-icon"),
                                 n = (0, a.up)("q-toolbar"),
                                 u = (0, a.up)("q-card-section"),
-                                c = (0, a.up)("q-btn"),
+                                d = (0, a.up)("q-btn"),
                                 r = (0, a.up)("q-card-actions"),
                                 m = (0, a.up)("q-separator"),
-                                h = (0, a.up)("q-card");
-                            return (0, a.wg)(), (0, a.j4)(h, {
+                                p = (0, a.up)("q-card");
+                            return (0, a.wg)(), (0, a.j4)(p, {
                                 class: "widget-card",
                                 flat: ""
                             }, {
                                 default: (0, a.w5)((() => [(0, a.Wm)(n, {
                                     class: "widget-card-toolbar"
                                 }, {
-                                    default: (0, a.w5)((() => [(0, a._)("h5", null, (0, d.zw)((0, s.SU)(t).title), 1), (0, a.Wm)(i), (0, a.Wm)(o, {
+                                    default: (0, a.w5)((() => [(0, a._)("h5", null, (0, c.zw)((0, s.SU)(t).title), 1), (0, a.Wm)(i), (0, a.Wm)(o, {
                                         name: (0, s.SU)(t).icon
                                     }, null, 8, ["name"])])),
                                     _: 1
                                 }), ((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).layout, (l => ((0, a.wg)(), (0, a.iD)("span", {
                                     key: l
                                 }, ["c" == l ? ((0, a.wg)(), (0, a.iD)("span", L, [(0, a.Wm)(u, {
                                     class: "widget-card-section"
@@ -450,32 +450,32 @@
                                     default: (0, a.w5)((() => [(0, a.Wm)(R, {
                                         use: (0, s.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
                                 })])) : (0, a.kq)("", !0), "a" == l ? ((0, a.wg)(), (0, a.iD)("span", $, [(0, a.Wm)(r, null, {
                                     default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).dialog_s, (l => ((0, a.wg)(), (0, a.iD)("span", {
                                         key: l.id
-                                    }, ["default-menu" == l.activator ? ((0, a.wg)(), (0, a.j4)(c, {
+                                    }, ["default-menu" == l.activator ? ((0, a.wg)(), (0, a.j4)(d, {
                                         key: 0,
                                         onClick: a => e.uniform.dialog[l.id].showDialog(void 0, "default", (0, s.SU)(t).source),
                                         icon: l.icon,
                                         dense: "",
                                         flat: ""
                                     }, {
-                                        default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)(l.title) + "...", 1)])),
+                                        default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)(l.title) + "...", 1)])),
                                         _: 2
                                     }, 1032, ["onClick", "icon"])) : (0, a.kq)("", !0)])))), 128)), ((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).action_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                                         key: e.id
-                                    }, ["default-menu" == e.activator ? ((0, a.wg)(), (0, a.j4)(c, {
+                                    }, ["default-menu" == e.activator ? ((0, a.wg)(), (0, a.j4)(d, {
                                         key: 0,
                                         icon: e.icon,
                                         dense: "",
                                         flat: ""
                                     }, {
-                                        default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)(e.title) + "...", 1)])),
+                                        default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)(e.title) + "...", 1)])),
                                         _: 2
                                     }, 1032, ["icon"])) : (0, a.kq)("", !0)])))), 128))])),
                                     _: 1
                                 })])) : (0, a.kq)("", !0)])))), 128)), (0, a.Wm)(m)])),
                                 _: 3
                             })
                         }
@@ -505,108 +505,144 @@
                     __name: "uf-widget-default",
                     setup(e) {
                         (0, a.l1)().use;
                         return (e, t) => ((0, a.wg)(), (0, a.iD)("span"))
                     }
                 }),
                 ue = ne,
-                ce = ue,
-                de = {
+                de = ue,
+                ce = {
+                    key: 0,
+                    class: "q-pb-sm"
+                },
+                re = {
+                    key: 1,
+                    class: "q-pb-sm"
+                },
+                me = {
+                    key: 2,
+                    class: "q-pb-sm"
+                },
+                pe = {
+                    key: 3,
+                    class: "q-pb-sm"
+                },
+                he = {
+                    key: 4,
+                    class: "q-pb-sm"
+                },
+                _e = {
+                    key: 5
+                },
+                we = {
                     inheritAttrs: !1
                 },
-                re = Object.assign(de, {
+                ge = Object.assign(we, {
                     __name: "uf-widget-form",
                     setup(e) {
                         const t = (0, a.l1)().use;
                         return (e, l) => {
                             const i = (0, a.up)("q-input"),
-                                o = (0, a.up)("q-form");
-                            return (0, a.wg)(), (0, a.j4)(o, {
+                                o = (0, a.up)("q-toggle"),
+                                n = (0, a.up)("q-form");
+                            return (0, a.wg)(), (0, a.j4)(n, {
                                 greedy: "",
                                 ref: e => {
                                     (0, s.SU)(t).refForm(e)
                                 }
                             }, {
                                 default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).active_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                                     key: e.id
-                                }, [e.class.includes("CharField") ? ((0, a.wg)(), (0, a.j4)(i, {
-                                    key: 0,
-                                    class: "q-pb-sm",
+                                }, [e.class.includes("CharField") ? ((0, a.wg)(), (0, a.iD)("div", ce, [(0, a.Wm)(i, {
                                     dense: "",
                                     outlined: "",
+                                    "hide-bottom-space": "",
                                     modelValue: (0, s.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, s.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, s.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
-                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, a.kq)("", !0), e.class.includes("TextField") ? ((0, a.wg)(), (0, a.j4)(i, {
-                                    key: 1,
-                                    class: "q-pb-sm",
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])])) : e.class.includes("TextField") ? ((0, a.wg)(), (0, a.iD)("div", re, [(0, a.Wm)(i, {
                                     dense: "",
                                     outlined: "",
+                                    "hide-bottom-space": "",
                                     modelValue: (0, s.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, s.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, s.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand",
                                     autogrow: ""
-                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, a.kq)("", !0), e.class.includes("IntegerField") ? ((0, a.wg)(), (0, a.j4)(i, {
-                                    key: 2,
-                                    class: "q-pb-sm",
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])])) : e.class.includes("IntegerField") ? ((0, a.wg)(), (0, a.iD)("div", me, [(0, a.Wm)(i, {
+                                    type: "number",
                                     dense: "",
                                     outlined: "",
-                                    type: "number",
+                                    "hide-bottom-space": "",
                                     modelValue: (0, s.SU)(t).data.item[e.name],
                                     "onUpdate:modelValue": l => (0, s.SU)(t).data.item[e.name] = l,
                                     label: e.verbose_name,
                                     rules: (0, s.SU)(t).getRules(e.name),
                                     "lazy-rules": "ondemand"
-                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])) : (0, a.kq)("", !0)])))), 128))])),
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])])) : e.class.includes("PasswordField") ? ((0, a.wg)(), (0, a.iD)("div", pe, [(0, a.Wm)(i, {
+                                    type: "password",
+                                    dense: "",
+                                    outlined: "",
+                                    "hide-bottom-space": "",
+                                    modelValue: (0, s.SU)(t).data.item[e.name],
+                                    "onUpdate:modelValue": l => (0, s.SU)(t).data.item[e.name] = l,
+                                    label: e.verbose_name,
+                                    rules: (0, s.SU)(t).getRules(e.name),
+                                    "lazy-rules": "ondemand"
+                                }, null, 8, ["modelValue", "onUpdate:modelValue", "label", "rules"])])) : e.class.includes("BooleanField") ? ((0, a.wg)(), (0, a.iD)("div", he, [(0, a.Wm)(o, {
+                                    modelValue: (0, s.SU)(t).data.item[e.name],
+                                    "onUpdate:modelValue": l => (0, s.SU)(t).data.item[e.name] = l
+                                }, null, 8, ["modelValue", "onUpdate:modelValue"])])) : ((0, a.wg)(), (0, a.iD)("div", _e, (0, c.zw)(e.class) + " is momentarily not implemented. When you think this is wrong pleas open an issue on github.", 1))])))), 128))])),
                                 _: 1
                             }, 512)
                         }
                     }
                 });
-            var me = l(6611);
-            const he = re,
-                pe = he;
-            U()(re, "components", {
+            var fe = l(6611),
+                ve = l(3175);
+            const be = ge,
+                ke = be;
+            U()(ge, "components", {
                 QForm: P.Z,
-                QInput: me.Z
+                QInput: fe.Z,
+                QToggle: ve.Z
             });
-            const _e = {
+            const ye = {
                     class: "row"
                 },
-                we = {
+                Ue = {
                     class: "row"
                 },
-                ge = {
+                Se = {
                     key: 0,
                     class: "col-auto text-body"
                 },
-                fe = {
+                qe = {
                     key: 1,
                     class: "col-auto text-body"
                 },
-                ve = {
+                We = {
                     class: "col-auto"
                 },
-                be = {
+                De = {
                     inheritAttrs: !1
                 },
-                ke = Object.assign(be, {
+                je = Object.assign(De, {
                     __name: "uf-widget-info",
                     setup(e) {
                         const t = (0, a.l1)().use;
                         return (e, l) => {
                             const i = (0, a.up)("q-btn");
-                            return (0, a.wg)(), (0, a.iD)("div", _e, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).active_s, (e => ((0, a.wg)(), (0, a.iD)("div", {
+                            return (0, a.wg)(), (0, a.iD)("div", ye, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).active_s, (e => ((0, a.wg)(), (0, a.iD)("div", {
                                 class: "widget-info-col col-lg-3 col-md-6 col-sm-12",
                                 key: e.id
-                            }, [(0, a._)("h6", null, (0, d.zw)(e.verbose_name), 1), (0, a._)("div", we, [(0, s.SU)(t).data.item[e.column_name] ? ((0, a.wg)(), (0, a.iD)("div", ge, (0, d.zw)((0, s.SU)(t).data.item[e.column_name]), 1)) : ((0, a.wg)(), (0, a.iD)("div", fe, "null " + (0, d.zw)(e.verbose_name), 1)), (0, a._)("div", ve, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).dialog_s, (l => ((0, a.wg)(), (0, a.iD)("span", {
+                            }, [(0, a._)("h6", null, (0, c.zw)(e.verbose_name), 1), (0, a._)("div", Ue, [(0, s.SU)(t).data.item[e.column_name] ? ((0, a.wg)(), (0, a.iD)("div", Se, (0, c.zw)((0, s.SU)(t).data.item[e.column_name]), 1)) : ((0, a.wg)(), (0, a.iD)("div", qe, "null " + (0, c.zw)(e.verbose_name), 1)), (0, a._)("div", We, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).dialog_s, (l => ((0, a.wg)(), (0, a.iD)("span", {
                                 key: l.id
                             }, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)(l.widget_s, (o => ((0, a.wg)(), (0, a.iD)("span", {
                                 key: o.key
                             }, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)(o.active_s, (o => ((0, a.wg)(), (0, a.iD)("span", {
                                 key: o.name
                             }, ["item-menu" == l.activator && e.column_name == o.column_name ? ((0, a.wg)(), (0, a.j4)(i, {
                                 key: 0,
@@ -617,23 +653,23 @@
                                 size: "xs",
                                 icon: l.icon,
                                 onClick: e => (0, s.SU)(t).ref[l.id].showDialog((0, s.SU)(t).data.item, "item", (0, s.SU)(t).data.source)
                             }, null, 8, ["icon", "onClick"])) : (0, a.kq)("", !0)])))), 128))])))), 128))])))), 128))])])])))), 128))])
                         }
                     }
                 }),
-                ye = ke,
-                Ue = ye;
-            U()(ke, "components", {
+                Ve = je,
+                Ze = Ve;
+            U()(je, "components", {
                 QBtn: b.Z
             });
-            const qe = {
+            const Qe = {
                     inheritAttrs: !1
                 },
-                Se = Object.assign(qe, {
+                Fe = Object.assign(Qe, {
                     __name: "uf-widget-table",
                     setup(e) {
                         const t = (0, a.l1)().use;
 
                         function l() {
                             let e = [];
                             return e.push({
@@ -667,102 +703,102 @@
                                 columns: l(),
                                 rows: (0, s.SU)(t).data.item_s,
                                 flat: ""
                             }, null, 8, ["columns", "rows"])
                         }
                     }
                 });
-            var We = l(7580);
-            const De = Se,
-                je = De;
-            U()(Se, "components", {
-                QTable: We.Z
+            var Ce = l(7580);
+            const xe = Fe,
+                Ee = xe;
+            U()(Fe, "components", {
+                QTable: Ce.Z
             });
-            const Ze = {
+            const He = {
                     __name: "uf-widget",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
                             l = (0, s.qj)(new x(t.id));
                         return (e, t) => ((0, a.wg)(), (0, a.j4)(ie, {
                             use: l
                         }, {
-                            "widget-content": (0, a.w5)((() => ["default" == l.type ? ((0, a.wg)(), (0, a.j4)(ce, {
+                            "widget-content": (0, a.w5)((() => ["default" == l.type ? ((0, a.wg)(), (0, a.j4)(de, {
                                 key: 0,
                                 use: l
-                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "form" == l.type ? ((0, a.wg)(), (0, a.j4)(pe, {
+                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "form" == l.type ? ((0, a.wg)(), (0, a.j4)(ke, {
                                 key: 1,
                                 use: l
-                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "info" == l.type ? ((0, a.wg)(), (0, a.j4)(Ue, {
+                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "info" == l.type ? ((0, a.wg)(), (0, a.j4)(Ze, {
                                 key: 2,
                                 use: l
-                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "table" == l.type ? ((0, a.wg)(), (0, a.j4)(je, {
+                            }, null, 8, ["use"])) : (0, a.kq)("", !0), "table" == l.type ? ((0, a.wg)(), (0, a.j4)(Ee, {
                                 key: 3,
                                 use: l
                             }, null, 8, ["use"])) : (0, a.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
-                Qe = Ze,
-                Ve = Qe,
-                Ce = {
+                ze = He,
+                Ie = ze,
+                Ke = {
                     inheritAttrs: !1
                 },
-                Fe = Object.assign(Ce, {
+                Oe = Object.assign(Ke, {
                     __name: "uf-dialog-standard",
                     setup(e) {
                         const t = (0, a.l1)().use;
                         return (e, l) => ((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).widget_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                             key: e.id
-                        }, [(0, a.Wm)(Ve, {
+                        }, [(0, a.Wm)(Ie, {
                             id: e.id
                         }, null, 8, ["id"]), ((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)(e.widget_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                             key: e.id
-                        }, [(0, a.Wm)(Ve, {
+                        }, [(0, a.Wm)(Ie, {
                             id: e.id
                         }, null, 8, ["id"])])))), 128))])))), 128))
                     }
                 }),
-                xe = Fe,
-                Ee = xe,
-                He = {
+                Ae = Oe,
+                Ye = Ae,
+                Pe = {
                     __name: "uf-dialog",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
-                            l = (0, s.qj)(new c(t.id));
-                        return (e, t) => ((0, a.wg)(), (0, a.j4)(Q, {
+                            l = (0, s.qj)(new d(t.id));
+                        return (e, t) => ((0, a.wg)(), (0, a.j4)(Z, {
                             use: l
                         }, {
-                            "dialog-content": (0, a.w5)((() => ["standard" == l.type ? ((0, a.wg)(), (0, a.j4)(Ee, {
+                            "dialog-content": (0, a.w5)((() => ["standard" == l.type ? ((0, a.wg)(), (0, a.j4)(Ye, {
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, a.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
-                Ie = He,
-                Ke = Ie;
-            class ze {
+                Te = Pe,
+                Be = Te;
+            class Me {
                 constructor(e) {
                     this.rowsPerPageOptions = [4, 8, 16, 32, 64, 128, 265, 512, 1024], this.rowsPerPage = e, this.page = 1
                 }
             }
-            class Oe extends i.y {
+            class Re extends i.y {
                 constructor(e) {
-                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, s.qj)(new V(this.uniform.source[this.source_id], {
+                    super(e), this.ql = {}, this.route = (0, o.yj)(), this.data = (0, s.qj)(new Q(this.uniform.source[this.source_id], {
                         ...this.query,
                         ...this.route.query
-                    })), this.pagination = (0, s.qj)(new ze(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
+                    })), this.pagination = (0, s.qj)(new Me(this.pag_recs)), this.item_menu_target = !1, this.item_menu_model = !1, this.item_menu_row = {}
                 }
                 get column_s() {
                     let e = [];
                     return e.push({
                         name: "gotos",
                         label: "",
                         field: "gotos"
@@ -811,35 +847,35 @@
                                 break
                             }
                 }
                 onItemMenuClick(e, t) {
                     this.item_menu_target = e.target, this.item_menu_model = !0, this.item_menu_row = t
                 }
             }
-            const Ae = {
+            const Le = {
                     inheritAttrs: !1
                 },
-                Ye = Object.assign(Ae, {
+                Ne = Object.assign(Le, {
                     __name: "uf-view-item-menu",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, u.j)();
                         return (e, i) => {
                             const o = (0, a.up)("q-icon"),
                                 n = (0, a.up)("q-item-section"),
                                 u = (0, a.up)("q-item"),
-                                c = (0, a.up)("q-list"),
+                                d = (0, a.up)("q-list"),
                                 r = (0, a.up)("q-menu");
                             return (0, a.wg)(), (0, a.j4)(r, {
                                 "auto-close": "",
                                 target: (0, s.SU)(t).item_menu_target,
                                 modelValue: (0, s.SU)(t).item_menu_model,
                                 "onUpdate:modelValue": i[0] || (i[0] = e => (0, s.SU)(t).item_menu_model = e)
                             }, {
-                                default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                     style: {
                                         "min-width": "100px"
                                     }
                                 }, {
                                     default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).dialog_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                                         key: e.id
                                     }, ["item-menu" == e.activator ? ((0, a.wg)(), (0, a.j4)(u, {
@@ -852,15 +888,15 @@
                                             avatar: ""
                                         }, {
                                             default: (0, a.w5)((() => [(0, a.Wm)(o, {
                                                 name: e.icon
                                             }, null, 8, ["name"])])),
                                             _: 2
                                         }, 1024), (0, a.Wm)(n, null, {
-                                            default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)(e.title), 1)])),
+                                            default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)(e.title), 1)])),
                                             _: 2
                                         }, 1024)])),
                                         _: 2
                                     }, 1032, ["onClick"])) : (0, a.kq)("", !0)])))), 128)), ((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).action_s, (e => ((0, a.wg)(), (0, a.iD)("span", {
                                         key: e.id
                                     }, ["item-menu" == e.activator ? ((0, a.wg)(), (0, a.j4)(u, {
                                         key: 0,
@@ -872,52 +908,52 @@
                                             avatar: ""
                                         }, {
                                             default: (0, a.w5)((() => [(0, a.Wm)(o, {
                                                 name: e.icon
                                             }, null, 8, ["name"])])),
                                             _: 2
                                         }, 1024), (0, a.Wm)(n, null, {
-                                            default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)(e.title), 1)])),
+                                            default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)(e.title), 1)])),
                                             _: 2
                                         }, 1024)])),
                                         _: 2
                                     }, 1032, ["onClick"])) : (0, a.kq)("", !0)])))), 128))])),
                                     _: 1
                                 })])),
                                 _: 1
                             }, 8, ["target", "modelValue"])
                         }
                     }
                 });
-            var Pe = l(6362),
-                Te = l(3246),
-                Me = l(490),
-                Be = l(1233);
-            const Re = Ye,
-                Le = Re;
-            U()(Ye, "components", {
-                QMenu: Pe.Z,
-                QList: Te.Z,
-                QItem: Me.Z,
-                QItemSection: Be.Z,
+            var $e = l(6362),
+                Ge = l(3246),
+                Je = l(490),
+                Xe = l(1233);
+            const et = Ne,
+                tt = et;
+            U()(Ne, "components", {
+                QMenu: $e.Z,
+                QList: Ge.Z,
+                QItem: Je.Z,
+                QItemSection: Xe.Z,
                 QIcon: ee.Z
             });
-            const Ne = {
+            const lt = {
                     class: "row full-width items-center"
                 },
-                $e = {
+                at = {
                     class: "col-auto float-left"
                 },
-                Ge = {
+                st = {
                     class: "col"
                 },
-                Je = {
+                it = {
                     inheritAttrs: !1
                 },
-                Xe = Object.assign(Je, {
+                ot = Object.assign(it, {
                     __name: "uf-view-header-menu",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, s.iH)(null),
                             i = (0, s.iH)(null),
                             o = (0, a.Fl)((() => {
                                 let e = [];
@@ -934,52 +970,52 @@
                                 })), e
                             }));
                         return (0, a.YP)(n, (() => {
                             i.value && i.value.forEach(((e, t) => {
                                 n.value.includes(t) ? e.classList.add("overflowed") : e.classList.remove("overflowed")
                             }))
                         })), (e, u) => {
-                            const c = (0, a.up)("q-btn"),
-                                d = (0, a.up)("q-item-section"),
+                            const d = (0, a.up)("q-btn"),
+                                c = (0, a.up)("q-item-section"),
                                 r = (0, a.up)("q-item"),
                                 m = (0, a.up)("q-list"),
-                                h = (0, a.up)("q-menu");
-                            return (0, a.wg)(), (0, a.iD)("div", Ne, [(0, a._)("div", $e, [(0, s.SU)(n).length > 0 ? ((0, a.wg)(), (0, a.j4)(c, {
+                                p = (0, a.up)("q-menu");
+                            return (0, a.wg)(), (0, a.iD)("div", lt, [(0, a._)("div", at, [(0, s.SU)(n).length > 0 ? ((0, a.wg)(), (0, a.j4)(d, {
                                 key: 0,
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-dots-vertical"
                             }, {
-                                default: (0, a.w5)((() => [(0, a.Wm)(h, null, {
+                                default: (0, a.w5)((() => [(0, a.Wm)(p, null, {
                                     default: (0, a.w5)((() => [(0, a.Wm)(m, null, {
                                         default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(o), ((l, i) => ((0, a.wg)(), (0, a.iD)("div", {
                                             key: l.id
                                         }, ["Decore_dialog" == l.class && (0, s.SU)(n).includes(i) ? ((0, a.wg)(), (0, a.j4)(r, {
                                             key: 0,
                                             clickable: ""
                                         }, {
-                                            default: (0, a.w5)((() => [(0, a.Wm)(d, null, {
-                                                default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                            default: (0, a.w5)((() => [(0, a.Wm)(c, null, {
+                                                default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                                     class: "text-black no-wrap",
                                                     flat: "",
                                                     icon: l.icon,
                                                     label: l.title,
                                                     onClick: e => (0, s.SU)(t).ref[l.id].showDialog({}, "default", (0, s.SU)(t).data.source)
                                                 }, null, 8, ["icon", "label", "onClick"])])),
                                                 _: 2
                                             }, 1024)])),
                                             _: 2
                                         }, 1024)) : (0, a.kq)("", !0), "Decore_action" == l.class && (0, s.SU)(n).includes(i) ? ((0, a.wg)(), (0, a.j4)(r, {
                                             key: 1,
                                             clickable: ""
                                         }, {
-                                            default: (0, a.w5)((() => [(0, a.Wm)(d, null, {
-                                                default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                            default: (0, a.w5)((() => [(0, a.Wm)(c, null, {
+                                                default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                                     class: "text-black no-wrap",
                                                     flat: "",
                                                     icon: l.icon,
                                                     label: l.title,
                                                     onClick: t => e.action_store.sendAction(l, {}, [])
                                                 }, null, 8, ["icon", "label", "onClick"])])),
                                                 _: 2
@@ -987,120 +1023,120 @@
                                             _: 2
                                         }, 1024)) : (0, a.kq)("", !0)])))), 128))])),
                                         _: 1
                                     })])),
                                     _: 1
                                 })])),
                                 _: 1
-                            })) : (0, a.kq)("", !0)]), (0, a._)("div", Ge, [(0, a._)("div", {
+                            })) : (0, a.kq)("", !0)]), (0, a._)("div", st, [(0, a._)("div", {
                                 ref_key: "menu",
                                 ref: l,
                                 class: "row no-wrap items-center"
                             }, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(o), (l => ((0, a.wg)(), (0, a.iD)("div", {
                                 class: "col-auto",
                                 key: l.id
                             }, [(0, a._)("div", {
                                 ref_for: !0,
                                 ref_key: "component",
                                 ref: i,
                                 class: "menu-item row no-wrap"
-                            }, ["Decore_dialog" == l.class ? ((0, a.wg)(), (0, a.j4)(c, {
+                            }, ["Decore_dialog" == l.class ? ((0, a.wg)(), (0, a.j4)(d, {
                                 key: 0,
                                 class: "text-black",
                                 flat: "",
                                 icon: l.icon,
                                 label: l.title,
                                 onClick: e => (0, s.SU)(t).ref[l.id].showDialog({}, "default", (0, s.SU)(t).data.source)
-                            }, null, 8, ["icon", "label", "onClick"])) : (0, a.kq)("", !0), "Decore_action" == l.class ? ((0, a.wg)(), (0, a.j4)(c, {
+                            }, null, 8, ["icon", "label", "onClick"])) : (0, a.kq)("", !0), "Decore_action" == l.class ? ((0, a.wg)(), (0, a.j4)(d, {
                                 key: 1,
                                 class: "text-black",
                                 flat: "",
                                 icon: l.icon,
                                 label: l.title,
                                 onClick: t => e.action_store.sendAction(l, {}, [])
                             }, null, 8, ["icon", "label", "onClick"])) : (0, a.kq)("", !0)], 512)])))), 128))], 512)])])
                         }
                     }
                 });
-            var et = l(1639);
-            const tt = (0, et.Z)(Xe, [
+            var nt = l(1639);
+            const ut = (0, nt.Z)(ot, [
                     ["__scopeId", "data-v-1026096e"]
                 ]),
-                lt = tt;
-            U()(Xe, "components", {
+                dt = ut;
+            U()(ot, "components", {
                 QBtn: b.Z,
-                QMenu: Pe.Z,
-                QList: Te.Z,
-                QItem: Me.Z,
-                QItemSection: Be.Z
+                QMenu: $e.Z,
+                QList: Ge.Z,
+                QItem: Je.Z,
+                QItemSection: Xe.Z
             });
-            const at = {
+            const ct = {
                     class: "row full-width items-center"
                 },
-                st = {
+                rt = {
                     class: "col-auto"
                 },
-                it = {
+                mt = {
                     class: "col-auto"
                 },
-                ot = {
+                pt = {
                     key: 0,
                     class: "col"
                 },
-                nt = {
+                ht = {
                     key: 1,
                     class: "col"
                 },
-                ut = {
+                _t = {
                     key: 2,
                     class: "col full-width"
                 },
-                ct = {
+                wt = {
                     class: "row full-width items-center"
                 },
-                dt = {
+                gt = {
                     class: "col-auto"
                 },
-                rt = {
+                ft = {
                     class: "col"
                 },
-                mt = {
+                vt = {
                     class: "col-auto"
                 },
-                ht = {
+                bt = {
                     inheritAttrs: !1
                 },
-                pt = Object.assign(ht, {
+                kt = Object.assign(bt, {
                     __name: "uf-view-filter",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, o.tv)(),
                             i = (0, o.yj)(),
                             n = (0, s.iH)(null),
                             u = (0, s.iH)(null),
-                            c = (0, s.iH)("eq"),
-                            d = (0, s.iH)(null);
+                            d = (0, s.iH)("eq"),
+                            c = (0, s.iH)(null);
 
                         function r() {
-                            n.value && !u.value ? (n.value = null, w.value = null, d.value = null) : n.value && u.value && (u.value = null, w.value = null, d.value = null)
+                            n.value && !u.value ? (n.value = null, w.value = null, c.value = null) : n.value && u.value && (u.value = null, w.value = null, c.value = null)
                         }
                         const m = (0, a.Fl)((() => {
                                 let e = !1;
                                 return !n.value || "ForeignKeyField" != n.value.class && "BackRefMetaField" != n.value.class && "ManyToManyField" != n.value.class || (e = !0), e
                             })),
-                            h = (0, a.Fl)((() => {
+                            p = (0, a.Fl)((() => {
                                 let e = [];
                                 return t.filter_s.forEach((l => {
                                     let a = !1;
                                     Object.entries(t.data.query).forEach((([e]) => {
                                         e.includes(l.name) && "ForeignKeyField" != l.class && (a = !0)
                                     })), a || e.push(l)
                                 })), e
                             })),
-                            p = (0, a.Fl)((() => {
+                            h = (0, a.Fl)((() => {
                                 let e, l = [];
                                 if ("ForeignKeyField" == n.value.class) e = n.value.rel_model;
                                 else {
                                     let l = t.data.source.rel_field_s.filter((e => "ForeignKeyField" == e.class && e.backref == n.value.name || "ManyToManyField" == e.class && e.name == n.value.name))[0];
                                     e = "ForeignKeyField" == l.class ? l.model : l.rel_model
                                 }
                                 let a = t.uniform.getSourceByModel(e);
@@ -1134,327 +1170,327 @@
                         }
 
                         function f() {
                             let e = {
                                     ...i.query
                                 },
                                 t = "";
-                            m.value ? m.value && (t = (n.value.class, t + n.value.name + "__" + u.value.name)) : t = n.value.name, t = t + "__" + c.value, e[t] = d.value, l.push({
+                            m.value ? m.value && (t = (n.value.class, t + n.value.name + "__" + u.value.name)) : t = n.value.name, t = t + "__" + d.value, e[t] = c.value, l.push({
                                 path: i.path,
                                 query: e
                             })
                         }
                         return (e, l) => {
                             const o = (0, a.up)("q-btn"),
                                 v = (0, a.up)("q-select");
-                            return (0, a.wg)(), (0, a.iD)("div", at, [(0, a._)("div", st, [(0, a.Wm)(o, {
+                            return (0, a.wg)(), (0, a.iD)("div", ct, [(0, a._)("div", rt, [(0, a.Wm)(o, {
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-content-save",
                                 onClick: l[0] || (l[0] = e => (0, s.SU)(t).uniform.queries.saveQuery((0, s.SU)(i)))
-                            })]), (0, a._)("div", it, [(0, a.Wm)(o, {
+                            })]), (0, a._)("div", mt, [(0, a.Wm)(o, {
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-undo",
                                 onClick: l[1] || (l[1] = e => r()),
                                 disable: !n.value
-                            }, null, 8, ["disable"])]), n.value ? (0, a.kq)("", !0) : ((0, a.wg)(), (0, a.iD)("div", ot, [(0, a.Wm)(v, {
+                            }, null, 8, ["disable"])]), n.value ? (0, a.kq)("", !0) : ((0, a.wg)(), (0, a.iD)("div", pt, [(0, a.Wm)(v, {
                                 dense: "",
                                 outlined: "",
                                 modelValue: n.value,
                                 "onUpdate:modelValue": [l[2] || (l[2] = e => n.value = e), l[3] || (l[3] = e => g())],
-                                options: (0, s.SU)(h),
+                                options: (0, s.SU)(p),
                                 "option-value": "name",
                                 "option-label": "verbose_name",
                                 "options-dense": "",
                                 label: "Select field for filtering",
                                 style: {
                                     width: "100%"
                                 }
-                            }, null, 8, ["modelValue", "options"])])), (0, s.SU)(m) && n.value && !u.value ? ((0, a.wg)(), (0, a.iD)("div", nt, [(0, a.Wm)(v, {
+                            }, null, 8, ["modelValue", "options"])])), (0, s.SU)(m) && n.value && !u.value ? ((0, a.wg)(), (0, a.iD)("div", ht, [(0, a.Wm)(v, {
                                 dense: "",
                                 outlined: "",
                                 modelValue: u.value,
                                 "onUpdate:modelValue": [l[4] || (l[4] = e => u.value = e), l[5] || (l[5] = e => g())],
-                                options: (0, s.SU)(p),
+                                options: (0, s.SU)(h),
                                 "option-value": "name",
                                 "option-label": "verbose_name",
                                 "options-dense": "",
                                 label: "Select related field for filtering",
                                 style: {
                                     width: "100%"
                                 }
-                            }, null, 8, ["modelValue", "options"])])) : (0, a.kq)("", !0), (0, s.SU)(m) && n.value && u.value || !(0, s.SU)(m) && n.value ? ((0, a.wg)(), (0, a.iD)("div", ut, [(0, a._)("div", ct, [(0, a._)("div", dt, [(0, a.Wm)(v, {
+                            }, null, 8, ["modelValue", "options"])])) : (0, a.kq)("", !0), (0, s.SU)(m) && n.value && u.value || !(0, s.SU)(m) && n.value ? ((0, a.wg)(), (0, a.iD)("div", _t, [(0, a._)("div", wt, [(0, a._)("div", gt, [(0, a.Wm)(v, {
                                 dense: "",
                                 outlined: "",
-                                modelValue: c.value,
-                                "onUpdate:modelValue": l[6] || (l[6] = e => c.value = e),
+                                modelValue: d.value,
+                                "onUpdate:modelValue": l[6] || (l[6] = e => d.value = e),
                                 options: (0, s.SU)(_),
                                 "option-value": "name",
                                 "option-label": "verbose_name",
                                 "options-dense": "",
                                 "map-options": "",
                                 "emit-value": ""
-                            }, null, 8, ["modelValue", "options"])]), (0, a._)("div", rt, ["eq" == c.value ? ((0, a.wg)(), (0, a.j4)(v, {
+                            }, null, 8, ["modelValue", "options"])]), (0, a._)("div", ft, ["eq" == d.value ? ((0, a.wg)(), (0, a.j4)(v, {
                                 key: 0,
                                 dense: "",
                                 outlined: "",
-                                modelValue: d.value,
-                                "onUpdate:modelValue": l[7] || (l[7] = e => d.value = e),
+                                modelValue: c.value,
+                                "onUpdate:modelValue": l[7] || (l[7] = e => c.value = e),
                                 multiple: "",
                                 options: w.value,
                                 "options-dense": "",
                                 label: "Select value for filtering",
                                 style: {
                                     width: "100%"
                                 },
                                 disable: !w.value,
                                 loading: !w.value
-                            }, null, 8, ["modelValue", "options", "disable", "loading"])) : (0, a.kq)("", !0)])])])) : (0, a.kq)("", !0), (0, a._)("div", mt, [(0, a.Wm)(o, {
+                            }, null, 8, ["modelValue", "options", "disable", "loading"])) : (0, a.kq)("", !0)])])])) : (0, a.kq)("", !0), (0, a._)("div", vt, [(0, a.Wm)(o, {
                                 class: "float-right text-black",
                                 dense: "",
                                 round: "",
                                 flat: "",
                                 icon: "mdi-database-search",
                                 onClick: l[8] || (l[8] = e => f()),
-                                disable: !d.value
+                                disable: !c.value
                             }, null, 8, ["disable"])])])
                         }
                     }
                 });
-            var _t = l(2762);
-            const wt = pt,
-                gt = wt;
-            U()(pt, "components", {
+            var yt = l(2762);
+            const Ut = kt,
+                St = Ut;
+            U()(kt, "components", {
                 QBtn: b.Z,
-                QSelect: _t.Z
+                QSelect: yt.Z
             });
-            const ft = {
+            const qt = {
                     class: "row full-width row items-center"
                 },
-                vt = {
+                Wt = {
                     class: "col-4"
                 },
-                bt = {
+                Dt = {
                     class: "col-4"
                 },
-                kt = {
+                jt = {
                     class: "col-4"
                 },
-                yt = {
+                Vt = {
                     class: "row items-center"
                 },
-                Ut = {
+                Zt = {
                     class: "col-2"
                 },
-                qt = {
+                Qt = {
                     class: "col"
                 },
-                St = {
+                Ft = {
                     class: "row full-width items-center"
                 },
-                Wt = {
+                Ct = {
                     inheritAttrs: !1
                 },
-                Dt = Object.assign(Wt, {
+                xt = Object.assign(Ct, {
                     __name: "uf-view-header",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, o.yj)();
                         return (e, i) => {
                             const o = (0, a.up)("q-btn"),
                                 n = (0, a.up)("q-input"),
                                 u = (0, a.up)("q-toolbar"),
-                                c = (0, a.up)("q-chip");
+                                d = (0, a.up)("q-chip");
                             return (0, a.wg)(), (0, a.iD)(a.HY, null, [(0, a.Wm)(u, {
                                 class: "bg-grey-2"
                             }, {
-                                default: (0, a.w5)((() => [(0, a._)("div", ft, [(0, a._)("div", vt, [(0, a.Wm)(lt, {
+                                default: (0, a.w5)((() => [(0, a._)("div", qt, [(0, a._)("div", Wt, [(0, a.Wm)(dt, {
                                     use: (0, s.SU)(t)
-                                }, null, 8, ["use"])]), (0, a._)("div", bt, [(0, a.Wm)(gt, {
+                                }, null, 8, ["use"])]), (0, a._)("div", Dt, [(0, a.Wm)(St, {
                                     use: (0, s.SU)(t)
-                                }, null, 8, ["use"])]), (0, a._)("div", kt, [(0, a._)("div", yt, [(0, a._)("div", Ut, [(0, a.Wm)(o, {
+                                }, null, 8, ["use"])]), (0, a._)("div", jt, [(0, a._)("div", Vt, [(0, a._)("div", Zt, [(0, a.Wm)(o, {
                                     class: "float-right text-black",
                                     dense: "",
                                     round: "",
                                     flat: "",
                                     icon: "clear",
                                     disable: !(0, s.SU)(t).data.search,
                                     onClick: i[0] || (i[0] = e => (0, s.SU)(t).data.search = null)
-                                }, null, 8, ["disable"])]), (0, a._)("div", qt, [(0, a.Wm)(n, {
+                                }, null, 8, ["disable"])]), (0, a._)("div", Qt, [(0, a.Wm)(n, {
                                     class: "text-black",
                                     dense: "",
                                     outlined: "",
                                     modelValue: (0, s.SU)(t).data.search,
                                     "onUpdate:modelValue": i[1] || (i[1] = e => (0, s.SU)(t).data.search = e),
                                     label: "Fast search in " + (0, s.SU)(t).title
                                 }, null, 8, ["modelValue", "label"])])])])])])),
                                 _: 1
-                            }), (0, a._)("div", St, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(l).query, ((e, t) => ((0, a.wg)(), (0, a.j4)(c, {
+                            }), (0, a._)("div", Ft, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(l).query, ((e, t) => ((0, a.wg)(), (0, a.j4)(d, {
                                 label: t + "=" + e,
                                 key: t
                             }, null, 8, ["label"])))), 128))])], 64)
                         }
                     }
                 });
-            var jt = l(7691);
-            const Zt = Dt,
-                Qt = Zt;
-            U()(Dt, "components", {
+            var Et = l(7691);
+            const Ht = xt,
+                zt = Ht;
+            U()(xt, "components", {
                 QToolbar: g.Z,
                 QBtn: b.Z,
-                QInput: me.Z,
-                QChip: jt.Z
+                QInput: fe.Z,
+                QChip: Et.Z
             });
-            const Vt = {
+            const It = {
                     class: "row items-center"
                 },
-                Ct = {
+                Kt = {
                     class: "view-footer-pagination col-auto"
                 },
-                Ft = {
+                Ot = {
                     class: "col-auto"
                 },
-                xt = {
+                At = {
                     inheritAttrs: !1
                 },
-                Et = Object.assign(xt, {
+                Yt = Object.assign(At, {
                     __name: "uf-view-footer",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, a.Fl)((() => {
                                 let e = Math.ceil(t.data.count / t.pagination.rowsPerPage);
                                 return e
                             }));
                         return (e, i) => {
                             const o = (0, a.up)("q-space"),
                                 n = (0, a.up)("q-pagination"),
                                 u = (0, a.up)("q-select"),
-                                c = (0, a.up)("q-toolbar");
-                            return (0, a.wg)(), (0, a.j4)(c, {
+                                d = (0, a.up)("q-toolbar");
+                            return (0, a.wg)(), (0, a.j4)(d, {
                                 class: "bg-grey-2"
                             }, {
-                                default: (0, a.w5)((() => [(0, a.Wm)(o), (0, a._)("div", Vt, [(0, a._)("div", Ct, [(0, a.Wm)(n, {
+                                default: (0, a.w5)((() => [(0, a.Wm)(o), (0, a._)("div", It, [(0, a._)("div", Kt, [(0, a.Wm)(n, {
                                     modelValue: (0, s.SU)(t).pagination.page,
                                     "onUpdate:modelValue": i[0] || (i[0] = e => (0, s.SU)(t).pagination.page = e),
                                     max: (0, s.SU)(l),
                                     "max-pages": 5,
                                     "direction-links": "",
                                     "boundary-links": "",
                                     "boundary-numbers": "",
                                     color: "black"
-                                }, null, 8, ["modelValue", "max"])]), (0, a._)("div", Ft, [(0, a.Wm)(u, {
+                                }, null, 8, ["modelValue", "max"])]), (0, a._)("div", Ot, [(0, a.Wm)(u, {
                                     modelValue: (0, s.SU)(t).pagination.rowsPerPage,
                                     "onUpdate:modelValue": i[1] || (i[1] = e => (0, s.SU)(t).pagination.rowsPerPage = e),
                                     options: (0, s.SU)(t).pagination.rowsPerPageOptions,
                                     dense: "",
                                     outlined: ""
                                 }, null, 8, ["modelValue", "options"])])])])),
                                 _: 1
                             })
                         }
                     }
                 });
-            var Ht = l(996);
-            const It = Et,
-                Kt = It;
-            U()(Et, "components", {
+            var Pt = l(996);
+            const Tt = Yt,
+                Bt = Tt;
+            U()(Yt, "components", {
                 QToolbar: g.Z,
                 QSpace: v.Z,
-                QPagination: Ht.Z,
-                QSelect: _t.Z
+                QPagination: Pt.Z,
+                QSelect: yt.Z
             });
-            const zt = {
+            const Mt = {
                     inheritAttrs: !1
                 },
-                Ot = Object.assign(zt, {
+                Rt = Object.assign(Mt, {
                     __name: "uf-view-layout",
                     setup(e) {
                         const t = (0, a.l1)().use,
                             l = (0, a.Fl)((() => {
                                 let e = "0 px";
                                 return t.ql.hasOwnProperty("header") && (e = t.ql.header.size + "px"), e
                             }));
                         return (e, i) => {
                             const o = (0, a.up)("q-header"),
                                 n = (0, a.up)("q-footer"),
                                 u = (0, a.up)("q-layout");
-                            return (0, a.wg)(), (0, a.iD)(a.HY, null, [(0, a.Wm)(Le, {
+                            return (0, a.wg)(), (0, a.iD)(a.HY, null, [(0, a.Wm)(tt, {
                                 use: (0, s.SU)(t)
                             }, null, 8, ["use"]), (0, a.Wm)(u, {
                                 container: "",
                                 style: {
                                     height: "calc(100vh - 102px)"
                                 }
                             }, {
                                 default: (0, a.w5)((() => [(0, a.Wm)(r.Z, {
                                     use: (0, s.SU)(t)
                                 }, null, 8, ["use"]), (0, a.Wm)(o, {
                                     reveal: "",
                                     class: "bg-white"
                                 }, {
-                                    default: (0, a.w5)((() => [(0, a.Wm)(Qt, {
+                                    default: (0, a.w5)((() => [(0, a.Wm)(zt, {
                                         use: (0, s.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
                                 }), (0, a._)("div", {
                                     class: "view-content",
-                                    style: (0, d.j5)({
+                                    style: (0, c.j5)({
                                         "padding-top": (0, s.SU)(l)
                                     })
                                 }, [(0, a.WI)(e.$slots, "view-content")], 4), (0, a.Wm)(n, {
                                     reveal: ""
                                 }, {
-                                    default: (0, a.w5)((() => [(0, a.Wm)(Kt, {
+                                    default: (0, a.w5)((() => [(0, a.Wm)(Bt, {
                                         use: (0, s.SU)(t)
                                     }, null, 8, ["use"])])),
                                     _: 1
                                 })])),
                                 _: 3
                             })], 64)
                         }
                     }
                 }),
-                At = Ot,
-                Yt = At;
-            U()(Ot, "components", {
+                Lt = Rt,
+                Nt = Lt;
+            U()(Rt, "components", {
                 QLayout: _.Z,
                 QHeader: w.Z,
                 QFooter: k.Z
             });
-            const Pt = {
+            const $t = {
                     inheritAttrs: !1
                 },
-                Tt = Object.assign(Pt, {
+                Gt = Object.assign($t, {
                     __name: "uf-view-table",
                     setup(e) {
                         const t = (0, a.l1)().use;
                         t.data.setItems();
                         const l = (0, a.Fl)((() => {
                             let e = 16,
                                 l = "0 px";
                             return e += t.ref.app.ql.header.size, e += t.ref.app.ql.footer.size, e += t.ql.header.size, e += t.ql.footer.size, l = "calc(100vh - " + e + "px)", l
                         }));
                         return (e, i) => {
                             const o = (0, a.up)("q-item-section"),
                                 n = (0, a.up)("q-item"),
                                 u = (0, a.up)("q-list"),
-                                c = (0, a.up)("q-menu"),
+                                d = (0, a.up)("q-menu"),
                                 r = (0, a.up)("q-btn"),
                                 m = (0, a.up)("q-td"),
-                                h = (0, a.up)("q-table");
-                            return (0, a.wg)(), (0, a.j4)(h, {
+                                p = (0, a.up)("q-table");
+                            return (0, a.wg)(), (0, a.j4)(p, {
                                 columns: (0, s.SU)(t).column_s,
                                 filter: (0, s.SU)(t).data.search,
                                 rows: (0, s.SU)(t).data.item_s,
-                                style: (0, d.j5)({
+                                style: (0, c.j5)({
                                     height: (0, s.SU)(l)
                                 }),
                                 class: "sticky-header-table",
                                 dense: "",
                                 flat: "",
                                 "hide-bottom": "",
                                 "row-key": "id",
@@ -1472,29 +1508,29 @@
                                 }, {
                                     default: (0, a.w5)((() => [(0, a.Wm)(r, {
                                         dense: "",
                                         round: "",
                                         flat: "",
                                         icon: "mdi-link"
                                     }, {
-                                        default: (0, a.w5)((() => [(0, a.Wm)(c, {
+                                        default: (0, a.w5)((() => [(0, a.Wm)(d, {
                                             "auto-close": ""
                                         }, {
                                             default: (0, a.w5)((() => [(0, a.Wm)(u, {
                                                 style: {
                                                     "min-width": "100px"
                                                 }
                                             }, {
                                                 default: (0, a.w5)((() => [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)((0, s.SU)(t).rel_view_s, (t => ((0, a.wg)(), (0, a.j4)(n, {
                                                     dense: "",
                                                     key: t.id,
                                                     to: "/" + t.parent_id + "/" + t.id + "?" + t.rel_field_name + "__eq=" + e.row.id
                                                 }, {
                                                     default: (0, a.w5)((() => [(0, a.Wm)(o, null, {
-                                                        default: (0, a.w5)((() => [(0, a.Uk)((0, d.zw)("view " + t.title + " from " + e.row.title), 1)])),
+                                                        default: (0, a.w5)((() => [(0, a.Uk)((0, c.zw)("view " + t.title + " from " + e.row.title), 1)])),
                                                         _: 2
                                                     }, 1024)])),
                                                     _: 2
                                                 }, 1032, ["to"])))), 128))])),
                                                 _: 2
                                             }, 1024)])),
                                             _: 2
@@ -1518,77 +1554,77 @@
                                     _: 2
                                 }, 1032, ["props"])])),
                                 _: 1
                             }, 8, ["columns", "filter", "rows", "style", "pagination", "selected"])
                         }
                     }
                 });
-            var Mt = l(7220);
-            const Bt = Tt,
-                Rt = Bt;
-            U()(Tt, "components", {
-                QTable: We.Z,
-                QTd: Mt.Z,
+            var Jt = l(7220);
+            const Xt = Gt,
+                el = Xt;
+            U()(Gt, "components", {
+                QTable: Ce.Z,
+                QTd: Jt.Z,
                 QBtn: b.Z,
-                QMenu: Pe.Z,
-                QList: Te.Z,
-                QItem: Me.Z,
-                QItemSection: Be.Z
+                QMenu: $e.Z,
+                QList: Ge.Z,
+                QItem: Je.Z,
+                QItemSection: Xe.Z
             });
-            const Lt = {
+            const tl = {
                     __name: "uf-view",
                     props: {
                         id: {}
                     },
                     setup(e) {
                         const t = e,
-                            l = (0, s.qj)(new Oe(t.id));
+                            l = (0, s.qj)(new Re(t.id));
                         return (0, a.bv)((() => {
                             for (const e of l.dialog_s)
                                 if ("none" == e.activator) {
                                     l.ref[e.id].showDialog({}, "last", l.data.source);
                                     break
                                 }
-                        })), (e, t) => ((0, a.wg)(), (0, a.j4)(Yt, {
+                        })), (e, t) => ((0, a.wg)(), (0, a.j4)(Nt, {
                             use: l
                         }, {
-                            "view-content": (0, a.w5)((() => ["table" == l.type ? ((0, a.wg)(), (0, a.j4)(Rt, {
+                            "view-content": (0, a.w5)((() => ["table" == l.type ? ((0, a.wg)(), (0, a.j4)(el, {
                                 key: 0,
                                 use: l
                             }, null, 8, ["use"])) : (0, a.kq)("", !0)])),
                             _: 1
                         }, 8, ["use"]))
                     }
                 },
-                Nt = Lt,
-                $t = Nt,
-                Gt = {
+                ll = tl,
+                al = ll,
+                sl = {
                     key: 0
                 },
-                Jt = {
+                il = {
                     __name: "uf-base",
                     setup(e) {
                         const t = (0, o.yj)(),
                             l = (0, s.qj)(new n(t.params.base_id));
                         return (e, t) => {
                             const s = (0, a.up)("q-page");
-                            return (0, a.wg)(), (0, a.iD)(a.HY, null, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)(l.route_dialog_s, (e => ((0, a.wg)(), (0, a.j4)(Ke, {
+                            return (0, a.wg)(), (0, a.iD)(a.HY, null, [((0, a.wg)(!0), (0, a.iD)(a.HY, null, (0, a.Ko)(l.route_dialog_s, (e => ((0, a.wg)(), (0, a.j4)(Be, {
                                 key: e.id,
                                 id: e.id
                             }, null, 8, ["id"])))), 128)), (0, a.Wm)(s, null, {
-                                default: (0, a.w5)((() => [l.getView().id ? ((0, a.wg)(), (0, a.iD)("span", Gt, [(0, a.Wm)($t, {
+                                default: (0, a.w5)((() => [l.getView().id ? ((0, a.wg)(), (0, a.iD)("span", sl, [(0, a.Wm)(al, {
                                     id: l.getView().id
                                 }, null, 8, ["id"])])) : (0, a.kq)("", !0)])),
                                 _: 1
                             })], 64)
                         }
                     }
                 };
-            var Xt = l(9885);
-            const el = Jt,
-                tl = el;
-            U()(Jt, "components", {
-                QPage: Xt.Z
+            var ol = l(9885);
+            const nl = il,
+                ul = nl;
+            U()(il, "components", {
+                QPage: ol.Z
             })
         }
     }
 ]);
```

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.24/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.24/decore_base/prepare/spa/static/js/app.aff5db90.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -813,15 +813,15 @@
             })
         }
     })(), (() => {
         n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, o) => (n.f[o](e, t), t)), []))
     })(), (() => {
         n.u = e => "js/" + e + "." + {
             65: "940d9b80",
-            586: "aa14c175"
+            586: "6cfbf2b5"
         } [e] + ".js"
     })(), (() => {
         n.miniCssF = e => "css/" + e + ".ed179a62.css"
     })(), (() => {
         n.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
```

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.24/decore_base/prepare/spa/static/js/vendor.6fe961ae.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -12,29 +12,29 @@
         499: (e, t, n) => {
             "use strict";
             n.d(t, {
                 B: () => i,
                 BK: () => Ke,
                 Bj: () => l,
                 EB: () => u,
-                Fl: () => Qe,
+                Fl: () => Xe,
                 IU: () => Re,
-                Jd: () => q,
+                Jd: () => F,
                 PG: () => Oe,
                 SU: () => Ue,
-                Um: () => qe,
+                Um: () => Fe,
                 WL: () => Ze,
                 X$: () => P,
                 X3: () => Ae,
                 XI: () => Ne,
                 Xl: () => Le,
                 dq: () => Me,
                 iH: () => Ie,
                 j: () => E,
-                lk: () => F,
+                lk: () => q,
                 nZ: () => s,
                 qj: () => Ce,
                 qq: () => S,
                 yT: () => Te
             });
             var o = n(6970);
             let r;
@@ -155,19 +155,19 @@
                     for (let n = 0; n < t.length; n++) t[n].delete(e);
                     t.length = 0
                 }
             }
             let k = !0;
             const C = [];
 
-            function q() {
+            function F() {
                 C.push(k), k = !1
             }
 
-            function F() {
+            function q() {
                 const e = C.pop();
                 k = void 0 === e || e
             }
 
             function E(e, t, n) {
                 if (k && b) {
                     let t = h.get(e);
@@ -241,17 +241,17 @@
                         const n = Re(this);
                         for (let t = 0, r = this.length; t < r; t++) E(n, "get", t + "");
                         const o = n[t](...e);
                         return -1 === o || !1 === o ? n[t](...e.map(Re)) : o
                     }
                 })), ["push", "pop", "shift", "unshift", "splice"].forEach((t => {
                     e[t] = function(...e) {
-                        q();
+                        F();
                         const n = Re(this)[t].apply(this, e);
-                        return F(), n
+                        return q(), n
                     }
                 })), e
             }
 
             function N(e) {
                 const t = Re(this);
                 return E(t, "has", e), t.hasOwnProperty(e)
@@ -265,15 +265,15 @@
                     if ("__v_raw" === r && l === (e ? t ? Se : _e : t ? we : be).get(n)) return n;
                     const i = (0, o.kJ)(n);
                     if (!e) {
                         if (i && (0, o.RI)(M, r)) return Reflect.get(M, r, l);
                         if ("hasOwnProperty" === r) return N
                     }
                     const a = Reflect.get(n, r, l);
-                    return ((0, o.yk)(r) ? $.has(r) : L(r)) ? a : (e || E(n, "get", r), t ? a : Me(a) ? i && (0, o.S0)(r) ? a : a.value : (0, o.Kn)(a) ? e ? Fe(a) : Ce(a) : a)
+                    return ((0, o.yk)(r) ? $.has(r) : L(r)) ? a : (e || E(n, "get", r), t ? a : Me(a) ? i && (0, o.S0)(r) ? a : a.value : (0, o.Kn)(a) ? e ? qe(a) : Ce(a) : a)
                 }
             }
             const z = D(),
                 U = D(!0);
 
             function D(e = !1) {
                 return function(t, n, r, l) {
@@ -313,29 +313,29 @@
                     set(e, t) {
                         return !0
                     },
                     deleteProperty(e, t) {
                         return !0
                     }
                 },
-                X = (0, o.l7)({}, J, {
+                Q = (0, o.l7)({}, J, {
                     get: B,
                     set: U
                 }),
-                Q = e => e,
+                X = e => e,
                 G = e => Reflect.getPrototypeOf(e);
 
             function ee(e, t, n = !1, o = !1) {
                 e = e["__v_raw"];
                 const r = Re(e),
                     l = Re(t);
                 n || (t !== l && E(r, "get", t), E(r, "get", l));
                 const {
                     has: i
-                } = G(r), a = o ? Q : n ? je : $e;
+                } = G(r), a = o ? X : n ? je : $e;
                 return i.call(r, t) ? a(e.get(t)) : i.call(r, l) ? a(e.get(l)) : void(e !== r && e.get(t))
             }
 
             function te(e, t = !1) {
                 const n = this["__v_raw"],
                     o = Re(n),
                     r = Re(e);
@@ -389,28 +389,28 @@
             }
 
             function ae(e, t) {
                 return function(n, o) {
                     const r = this,
                         l = r["__v_raw"],
                         i = Re(l),
-                        a = t ? Q : e ? je : $e;
+                        a = t ? X : e ? je : $e;
                     return !e && E(i, "iterate", w), l.forEach(((e, t) => n.call(o, a(e), a(t), r)))
                 }
             }
 
             function se(e, t, n) {
                 return function(...r) {
                     const l = this["__v_raw"],
                         i = Re(l),
                         a = (0, o._N)(i),
                         s = "entries" === e || e === Symbol.iterator && a,
                         u = "keys" === e && a,
                         c = l[e](...r),
-                        d = n ? Q : t ? je : $e;
+                        d = n ? X : t ? je : $e;
                     return !t && E(i, "iterate", u ? _ : w), {
                         next() {
                             const {
                                 value: e,
                                 done: t
                             } = c.next();
                             return t ? {
@@ -539,19 +539,19 @@
                 return e["__v_skip"] || !Object.isExtensible(e) ? 0 : xe((0, o.W7)(e))
             }
 
             function Ce(e) {
                 return Pe(e) ? e : Ee(e, !1, J, me, be)
             }
 
-            function qe(e) {
-                return Ee(e, !1, X, ge, we)
+            function Fe(e) {
+                return Ee(e, !1, Q, ge, we)
             }
 
-            function Fe(e) {
+            function qe(e) {
                 return Ee(e, !0, W, ye, _e)
             }
 
             function Ee(e, t, n, r, l) {
                 if (!(0, o.Kn)(e)) return e;
                 if (e["__v_raw"] && (!t || !e["__v_isReactive"])) return e;
                 const i = l.get(e);
@@ -583,15 +583,15 @@
                 return t ? Re(t) : e
             }
 
             function Le(e) {
                 return (0, o.Nj)(e, "__v_skip", !0), e
             }
             const $e = e => (0, o.Kn)(e) ? Ce(e) : e,
-                je = e => (0, o.Kn)(e) ? Fe(e) : e;
+                je = e => (0, o.Kn)(e) ? qe(e) : e;
 
             function Be(e) {
                 k && b && (e = Re(e), O(e.dep || (e.dep = c())))
             }
 
             function Ve(e, t) {
                 e = Re(e);
@@ -664,34 +664,34 @@
             }
 
             function Je(e, t, n) {
                 const o = e[t];
                 return Me(o) ? o : new Ye(e, t, n)
             }
             var We;
-            class Xe {
+            class Qe {
                 constructor(e, t, n, o) {
                     this._setter = t, this.dep = void 0, this.__v_isRef = !0, this[We] = !1, this._dirty = !0, this.effect = new S(e, (() => {
                         this._dirty || (this._dirty = !0, Ve(this))
                     })), this.effect.computed = this, this.effect.active = this._cacheable = !o, this["__v_isReadonly"] = n
                 }
                 get value() {
                     const e = Re(this);
                     return Be(e), !e._dirty && e._cacheable || (e._dirty = !1, e._value = e.effect.run()), e._value
                 }
                 set value(e) {
                     this._setter(e)
                 }
             }
 
-            function Qe(e, t, n = !1) {
+            function Xe(e, t, n = !1) {
                 let r, l;
                 const i = (0, o.mf)(e);
                 i ? (r = e, l = o.dG) : (r = e.get, l = e.set);
-                const a = new Xe(r, l, i || !l, n);
+                const a = new Qe(r, l, i || !l, n);
                 return a
             }
             We = "__v_isReadonly"
         },
         9835: (e, t, n) => {
             "use strict";
             n.d(t, {
@@ -703,30 +703,30 @@
                 JJ: () => U,
                 Jd: () => ke,
                 Ko: () => Be,
                 P$: () => te,
                 Q6: () => ae,
                 U2: () => oe,
                 Uk: () => cn,
-                Us: () => qt,
+                Us: () => Ft,
                 WI: () => Ve,
                 Wm: () => ln,
                 Xn: () => Se,
                 Y3: () => y,
-                Y8: () => Q,
+                Y8: () => X,
                 YP: () => K,
                 _: () => rn,
                 aZ: () => se,
                 bv: () => _e,
                 dl: () => fe,
                 f3: () => D,
                 h: () => In,
-                iD: () => Xt,
+                iD: () => Qt,
                 ic: () => xe,
-                j4: () => Qt,
+                j4: () => Xt,
                 kq: () => dn,
                 l1: () => Vn,
                 lR: () => Vt,
                 nK: () => ie,
                 se: () => pe,
                 up: () => Re,
                 w5: () => $,
@@ -797,15 +797,15 @@
             }
 
             function b(e) {
                 let t = f + 1,
                     n = d.length;
                 while (t < n) {
                     const o = t + n >>> 1,
-                        r = q(d[o]);
+                        r = F(d[o]);
                     r < e ? t = o + 1 : n = o
                 }
                 return t
             }
 
             function w(e) {
                 d.length && d.includes(e, u && e.allowRecurse ? f + 1 : f) || (null == e.id ? d.push(e) : d.splice(b(e.id), 0, e), _())
@@ -831,30 +831,30 @@
                 }
             }
 
             function C(e) {
                 if (p.length) {
                     const e = [...new Set(p)];
                     if (p.length = 0, v) return void v.push(...e);
-                    for (v = e, v.sort(((e, t) => q(e) - q(t))), h = 0; h < v.length; h++) v[h]();
+                    for (v = e, v.sort(((e, t) => F(e) - F(t))), h = 0; h < v.length; h++) v[h]();
                     v = null, h = 0
                 }
             }
-            const q = e => null == e.id ? 1 / 0 : e.id,
-                F = (e, t) => {
-                    const n = q(e) - q(t);
+            const F = e => null == e.id ? 1 / 0 : e.id,
+                q = (e, t) => {
+                    const n = F(e) - F(t);
                     if (0 === n) {
                         if (e.pre && !t.pre) return -1;
                         if (t.pre && !e.pre) return 1
                     }
                     return n
                 };
 
             function E(e) {
-                c = !1, u = !0, d.sort(F);
+                c = !1, u = !0, d.sort(q);
                 r.dG;
                 try {
                     for (f = 0; f < d.length; f++) {
                         const e = d[f];
                         e && !1 !== e.active && l(e, null, 14)
                     }
                 } finally {
@@ -1065,26 +1065,26 @@
                 flush: s,
                 onTrack: u,
                 onTrigger: c
             } = r.kT) {
                 const d = (0, o.nZ)() === (null === wn || void 0 === wn ? void 0 : wn.scope) ? wn : null;
                 let f, p, v = !1,
                     h = !1;
-                if ((0, o.dq)(e) ? (f = () => e.value, v = (0, o.yT)(e)) : (0, o.PG)(e) ? (f = () => e, a = !0) : (0, r.kJ)(e) ? (h = !0, v = e.some((e => (0, o.PG)(e) || (0, o.yT)(e))), f = () => e.map((e => (0, o.dq)(e) ? e.value : (0, o.PG)(e) ? X(e) : (0, r.mf)(e) ? l(e, d, 2) : void 0))) : f = (0, r.mf)(e) ? t ? () => l(e, d, 2) : () => {
+                if ((0, o.dq)(e) ? (f = () => e.value, v = (0, o.yT)(e)) : (0, o.PG)(e) ? (f = () => e, a = !0) : (0, r.kJ)(e) ? (h = !0, v = e.some((e => (0, o.PG)(e) || (0, o.yT)(e))), f = () => e.map((e => (0, o.dq)(e) ? e.value : (0, o.PG)(e) ? Q(e) : (0, r.mf)(e) ? l(e, d, 2) : void 0))) : f = (0, r.mf)(e) ? t ? () => l(e, d, 2) : () => {
                         if (!d || !d.isUnmounted) return p && p(), i(e, d, 3, [g])
                     } : r.dG, t && a) {
                     const e = f;
-                    f = () => X(e())
+                    f = () => Q(e())
                 }
                 let m, g = e => {
                     p = S.onStop = () => {
                         l(e, d, 4)
                     }
                 };
-                if (Fn) {
+                if (qn) {
                     if (g = r.dG, t ? n && i(t, d, 3, [f(), h ? [] : void 0, g]) : f(), "sync" !== s) return r.dG; {
                         const e = Hn();
                         m = e.__watcherHandles || (e.__watcherHandles = [])
                     }
                 }
                 let y = h ? new Array(e.length).fill(Z) : Z;
                 const b = () => {
@@ -1120,29 +1120,29 @@
                 return () => {
                     let t = e;
                     for (let e = 0; e < n.length && t; e++) t = t[n[e]];
                     return t
                 }
             }
 
-            function X(e, t) {
+            function Q(e, t) {
                 if (!(0, r.Kn)(e) || e["__v_skip"]) return e;
                 if (t = t || new Set, t.has(e)) return e;
-                if (t.add(e), (0, o.dq)(e)) X(e.value, t);
+                if (t.add(e), (0, o.dq)(e)) Q(e.value, t);
                 else if ((0, r.kJ)(e))
-                    for (let n = 0; n < e.length; n++) X(e[n], t);
+                    for (let n = 0; n < e.length; n++) Q(e[n], t);
                 else if ((0, r.DM)(e) || (0, r._N)(e)) e.forEach((e => {
-                    X(e, t)
+                    Q(e, t)
                 }));
                 else if ((0, r.PO)(e))
-                    for (const n in e) X(e[n], t);
+                    for (const n in e) Q(e[n], t);
                 return e
             }
 
-            function Q() {
+            function X() {
                 const e = {
                     isMounted: !1,
                     isLeaving: !1,
                     isUnmounting: !1,
                     leavingVNodes: new Map
                 };
                 return _e((() => {
@@ -1171,15 +1171,15 @@
                         onAfterAppear: G,
                         onAppearCancelled: G
                     },
                     setup(e, {
                         slots: t
                     }) {
                         const n = _n(),
-                            r = Q();
+                            r = X();
                         let l;
                         return () => {
                             const i = t.default && ae(t.default(), !0);
                             if (!i || !i.length) return;
                             let a = i[0];
                             if (i.length > 1) {
                                 let e = !1;
@@ -1389,23 +1389,23 @@
                             (0, o.Jd)(), Sn(n);
                             const l = i(t, n, e, r);
                             return xn(), (0, o.lk)(), l
                         });
                     return r ? l.unshift(a) : l.push(a), a
                 }
             }
-            const be = e => (t, n = wn) => (!Fn || "sp" === e) && ye(e, ((...e) => t(...e)), n),
+            const be = e => (t, n = wn) => (!qn || "sp" === e) && ye(e, ((...e) => t(...e)), n),
                 we = be("bm"),
                 _e = be("m"),
                 Se = be("bu"),
                 xe = be("u"),
                 ke = be("bum"),
                 Ce = be("um"),
-                qe = be("sp"),
-                Fe = be("rtg"),
+                Fe = be("sp"),
+                qe = be("rtg"),
                 Ee = be("rtc");
 
             function Oe(e, t = wn) {
                 ye("ec", e, t)
             }
 
             function Pe(e, t) {
@@ -1414,15 +1414,15 @@
                 const o = Ln(n) || n.proxy,
                     l = e.dirs || (e.dirs = []);
                 for (let i = 0; i < t.length; i++) {
                     let [e, n, a, s = r.kT] = t[i];
                     e && ((0, r.mf)(e) && (e = {
                         mounted: e,
                         updated: e
-                    }), e.deep && X(n), l.push({
+                    }), e.deep && Q(n), l.push({
                         dir: e,
                         instance: o,
                         value: n,
                         oldValue: void 0,
                         arg: a,
                         modifiers: s
                     }))
@@ -1490,15 +1490,15 @@
             }
 
             function Ve(e, t, n = {}, o, r) {
                 if (A.isCE || A.parent && ue(A.parent) && A.parent.isCE) return "default" !== t && (n.name = t), ln("slot", n, o && o());
                 let l = e[t];
                 l && l._c && (l._d = !1), Zt();
                 const i = l && Me(l(n)),
-                    a = Qt(It, {
+                    a = Xt(It, {
                         key: n.key || i && i.key || `_${t}`
                     }, i || (o ? o() : []), i && 1 === e._ ? 64 : -2);
                 return !r && a.scopeId && (a.slotScopeIds = [a.scopeId + "-s"]), l && l._c && (l._d = !0), a
             }
 
             function Me(e) {
                 return e.some((e => !Gt(e) || e.type !== Ht && !(e.type === It && !Me(e.children)))) ? e : null
@@ -1609,16 +1609,16 @@
                     beforeDestroy: b,
                     beforeUnmount: w,
                     destroyed: _,
                     unmounted: S,
                     render: x,
                     renderTracked: k,
                     renderTriggered: C,
-                    errorCaptured: q,
-                    serverPrefetch: F,
+                    errorCaptured: F,
+                    serverPrefetch: q,
                     expose: E,
                     inheritAttrs: O,
                     components: P,
                     directives: T,
                     filters: A
                 } = t, R = null;
                 if (d && Ze(d, l, R, e.appContext.config.unwrapInjectedRef), s)
@@ -1656,15 +1656,15 @@
                         U(t, e[t])
                     }))
                 }
 
                 function L(e, t) {
                     (0, r.kJ)(t) ? t.forEach((t => e(t.bind(n)))): t && e(t.bind(n))
                 }
-                if (f && Ke(f, e, "c"), L(we, p), L(_e, v), L(Se, h), L(xe, m), L(fe, g), L(pe, y), L(Oe, q), L(Ee, k), L(Fe, C), L(ke, w), L(Ce, S), L(qe, F), (0, r.kJ)(E))
+                if (f && Ke(f, e, "c"), L(we, p), L(_e, v), L(Se, h), L(xe, m), L(fe, g), L(pe, y), L(Oe, F), L(Ee, k), L(qe, C), L(ke, w), L(Ce, S), L(Fe, q), (0, r.kJ)(E))
                     if (E.length) {
                         const t = e.exposed || (e.exposed = {});
                         E.forEach((e => {
                             Object.defineProperty(t, e, {
                                 get: () => n[e],
                                 set: t => n[e] = t
                             })
@@ -1729,20 +1729,20 @@
                     mixins: r,
                     extends: l
                 } = t;
                 l && We(e, l, n, !0), r && r.forEach((t => We(e, t, n, !0)));
                 for (const i in t)
                     if (o && "expose" === i);
                     else {
-                        const o = Xe[i] || n && n[i];
+                        const o = Qe[i] || n && n[i];
                         e[i] = o ? o(e[i], t[i]) : t[i]
                     } return e
             }
-            const Xe = {
-                data: Qe,
+            const Qe = {
+                data: Xe,
                 props: nt,
                 emits: nt,
                 methods: nt,
                 computed: nt,
                 beforeCreate: tt,
                 created: tt,
                 beforeMount: tt,
@@ -1756,19 +1756,19 @@
                 activated: tt,
                 deactivated: tt,
                 errorCaptured: tt,
                 serverPrefetch: tt,
                 components: nt,
                 directives: nt,
                 watch: ot,
-                provide: Qe,
+                provide: Xe,
                 inject: Ge
             };
 
-            function Qe(e, t) {
+            function Xe(e, t) {
                 return t ? e ? function() {
                     return (0, r.l7)((0, r.mf)(e) ? e.call(this, this) : e, (0, r.mf)(t) ? t.call(this, this) : t)
                 } : t : e
             }
 
             function Ge(e, t) {
                 return nt(et(e), et(t))
@@ -2085,19 +2085,19 @@
                     } else 0
                 }
             }
 
             function kt() {}
             const Ct = z;
 
-            function qt(e) {
-                return Ft(e)
+            function Ft(e) {
+                return qt(e)
             }
 
-            function Ft(e, t) {
+            function qt(e, t) {
                 kt();
                 const n = (0, r.E9)();
                 n.__VUE__ = !0;
                 const {
                     insert: l,
                     remove: i,
                     patchProp: a,
@@ -2108,15 +2108,15 @@
                     setElementText: f,
                     parentNode: p,
                     nextSibling: v,
                     setScopeId: h = r.dG,
                     insertStaticContent: m
                 } = e, g = (e, t, n, o = null, r = null, l = null, i = !1, a = null, s = !!t.dynamicChildren) => {
                     if (e === t) return;
-                    e && !en(e, t) && (o = Q(e), K(e, r, l, !0), e = null), -2 === t.patchFlag && (s = !1, t.dynamicChildren = null);
+                    e && !en(e, t) && (o = X(e), K(e, r, l, !0), e = null), -2 === t.patchFlag && (s = !1, t.dynamicChildren = null);
                     const {
                         type: u,
                         ref: c,
                         shapeFlag: d
                     } = t;
                     switch (u) {
                         case Nt:
@@ -2128,15 +2128,15 @@
                         case zt:
                             null == e && _(t, n, o, i);
                             break;
                         case It:
                             L(e, t, n, o, r, l, i, a, s);
                             break;
                         default:
-                            1 & d ? F(e, t, n, o, r, l, i, a, s) : 6 & d ? $(e, t, n, o, r, l, i, a, s) : (64 & d || 128 & d) && u.process(e, t, n, o, r, l, i, a, s, ee)
+                            1 & d ? q(e, t, n, o, r, l, i, a, s) : 6 & d ? $(e, t, n, o, r, l, i, a, s) : (64 & d || 128 & d) && u.process(e, t, n, o, r, l, i, a, s, ee)
                     }
                     null != c && r && xt(c, e && e.ref, l, t || e, !t)
                 }, y = (e, t, n, o) => {
                     if (null == e) l(t.el = u(t.children), n, o);
                     else {
                         const n = t.el = e.el;
                         t.children !== e.children && d(n, t.children)
@@ -2148,34 +2148,34 @@
                 }, x = ({
                     el: e,
                     anchor: t
                 }, n, o) => {
                     let r;
                     while (e && e !== t) r = v(e), l(e, n, o), e = r;
                     l(t, n, o)
-                }, q = ({
+                }, F = ({
                     el: e,
                     anchor: t
                 }) => {
                     let n;
                     while (e && e !== t) n = v(e), i(e), e = n;
                     i(t)
-                }, F = (e, t, n, o, r, l, i, a, s) => {
+                }, q = (e, t, n, o, r, l, i, a, s) => {
                     i = i || "svg" === t.type, null == e ? E(t, n, o, r, l, i, a, s) : T(e, t, r, l, i, a, s)
                 }, E = (e, t, n, o, i, u, c, d) => {
                     let p, v;
                     const {
                         type: h,
                         props: m,
                         shapeFlag: g,
                         transition: y,
                         dirs: b
                     } = e;
                     if (p = e.el = s(e.type, u, m && m.is, m), 8 & g ? f(p, e.children) : 16 & g && P(e.children, p, null, o, i, u && "foreignObject" !== h, c, d), b && Te(e, null, o, "created"), O(p, e, e.scopeId, c, o), m) {
-                        for (const t in m) "value" === t || (0, r.Gg)(t) || a(p, t, null, m[t], u, e.children, o, i, X);
+                        for (const t in m) "value" === t || (0, r.Gg)(t) || a(p, t, null, m[t], u, e.children, o, i, Q);
                         "value" in m && a(p, "value", null, m.value), (v = m.onVnodeBeforeMount) && mn(v, o, e)
                     }
                     b && Te(e, null, o, "beforeMount");
                     const w = (!i || i && !i.pendingBranch) && y && !y.persisted;
                     w && y.beforeEnter(p), l(p, t, n), ((v = m && m.onVnodeMounted) || w || b) && Ct((() => {
                         v && mn(v, o, e), w && y.enter(p), b && Te(e, null, o, "mounted")
                     }), i)
@@ -2211,15 +2211,15 @@
                         if (16 & c) R(u, t, v, h, n, o, l);
                         else if (2 & c && v.class !== h.class && a(u, "class", null, h.class, l), 4 & c && a(u, "style", v.style, h.style, l), 8 & c) {
                             const r = t.dynamicProps;
                             for (let t = 0; t < r.length; t++) {
                                 const i = r[t],
                                     s = v[i],
                                     c = h[i];
-                                c === s && "value" !== i || a(u, i, s, c, l, e.children, n, o, X)
+                                c === s && "value" !== i || a(u, i, s, c, l, e.children, n, o, Q)
                             }
                         }
                         1 & c && e.children !== t.children && f(u, t.children)
                     } else s || null != d || R(u, t, v, h, n, o, l);
                     ((m = h.onVnodeUpdated) || p) && Ct((() => {
                         m && mn(m, n, t, e), p && Te(t, e, n, "updated")
                     }), o)
@@ -2229,20 +2229,20 @@
                             u = t[a],
                             c = s.el && (s.type === It || !en(s, u) || 70 & s.shapeFlag) ? p(s.el) : n;
                         g(s, u, c, null, o, r, l, i, !0)
                     }
                 }, R = (e, t, n, o, l, i, s) => {
                     if (n !== o) {
                         if (n !== r.kT)
-                            for (const u in n)(0, r.Gg)(u) || u in o || a(e, u, n[u], null, s, t.children, l, i, X);
+                            for (const u in n)(0, r.Gg)(u) || u in o || a(e, u, n[u], null, s, t.children, l, i, Q);
                         for (const u in o) {
                             if ((0, r.Gg)(u)) continue;
                             const c = o[u],
                                 d = n[u];
-                            c !== d && "value" !== u && a(e, u, d, c, s, t.children, l, i, X)
+                            c !== d && "value" !== u && a(e, u, d, c, s, t.children, l, i, Q)
                         }
                         "value" in o && a(e, "value", n.value, o.value)
                     }
                 }, L = (e, t, n, o, r, i, a, s, c) => {
                     const d = t.el = e ? e.el : u(""),
                         f = t.anchor = e ? e.anchor : u("");
                     let {
@@ -2278,15 +2278,15 @@
                                         vnode: c
                                     } = e,
                                     d = n;
                                 0, Et(e, !1), n ? (n.el = c.el, H(e, n, s)) : n = c, o && (0, r.ir)(o), (t = n.props && n.props.onVnodeBeforeUpdate) && mn(t, u, n, c), Et(e, !0);
                                 const f = j(e);
                                 0;
                                 const v = e.subTree;
-                                e.subTree = f, g(v, f, p(v.el), Q(v), e, i, a), n.el = f.el, null === d && N(e, f.el), l && Ct(l, i), (t = n.props && n.props.onVnodeUpdated) && Ct((() => mn(t, u, n, c)), i)
+                                e.subTree = f, g(v, f, p(v.el), X(v), e, i, a), n.el = f.el, null === d && N(e, f.el), l && Ct(l, i), (t = n.props && n.props.onVnodeUpdated) && Ct((() => mn(t, u, n, c)), i)
                             } else {
                                 let o;
                                 const {
                                     el: s,
                                     props: u
                                 } = t, {
                                     bm: c,
@@ -2324,26 +2324,26 @@
                             patchFlag: p,
                             shapeFlag: v
                         } = t;
                     if (p > 0) {
                         if (128 & p) return void D(u, d, n, o, r, l, i, a, s);
                         if (256 & p) return void U(u, d, n, o, r, l, i, a, s)
                     }
-                    8 & v ? (16 & c && X(u, r, l), d !== u && f(n, d)) : 16 & c ? 16 & v ? D(u, d, n, o, r, l, i, a, s) : X(u, r, l, !0) : (8 & c && f(n, ""), 16 & v && P(d, n, o, r, l, i, a, s))
+                    8 & v ? (16 & c && Q(u, r, l), d !== u && f(n, d)) : 16 & c ? 16 & v ? D(u, d, n, o, r, l, i, a, s) : Q(u, r, l, !0) : (8 & c && f(n, ""), 16 & v && P(d, n, o, r, l, i, a, s))
                 }, U = (e, t, n, o, l, i, a, s, u) => {
                     e = e || r.Z6, t = t || r.Z6;
                     const c = e.length,
                         d = t.length,
                         f = Math.min(c, d);
                     let p;
                     for (p = 0; p < f; p++) {
                         const o = t[p] = u ? pn(t[p]) : fn(t[p]);
                         g(e[p], o, n, null, l, i, a, s, u)
                     }
-                    c > d ? X(e, l, i, !0, !1, f) : P(t, n, o, l, i, a, s, u, f)
+                    c > d ? Q(e, l, i, !0, !1, f) : P(t, n, o, l, i, a, s, u, f)
                 }, D = (e, t, n, o, l, i, a, s, u) => {
                     let c = 0;
                     const d = t.length;
                     let f = e.length - 1,
                         p = d - 1;
                     while (c <= f && c <= p) {
                         const o = e[c],
@@ -2449,27 +2449,27 @@
                     if (null != a && xt(a, null, n, e, !0), 256 & c) return void t.ctx.deactivate(e);
                     const p = 1 & c && f,
                         v = !ue(e);
                     let h;
                     if (v && (h = i && i.onVnodeBeforeUnmount) && mn(h, t, e), 6 & c) W(e.component, n, o);
                     else {
                         if (128 & c) return void e.suspense.unmount(n, o);
-                        p && Te(e, null, t, "beforeUnmount"), 64 & c ? e.type.remove(e, t, n, r, ee, o) : u && (l !== It || d > 0 && 64 & d) ? X(u, t, n, !1, !0) : (l === It && 384 & d || !r && 16 & c) && X(s, t, n), o && Y(e)
+                        p && Te(e, null, t, "beforeUnmount"), 64 & c ? e.type.remove(e, t, n, r, ee, o) : u && (l !== It || d > 0 && 64 & d) ? Q(u, t, n, !1, !0) : (l === It && 384 & d || !r && 16 & c) && Q(s, t, n), o && Y(e)
                     }(v && (h = i && i.onVnodeUnmounted) || p) && Ct((() => {
                         h && mn(h, t, e), p && Te(e, null, t, "unmounted")
                     }), n)
                 }, Y = e => {
                     const {
                         type: t,
                         el: n,
                         anchor: o,
                         transition: r
                     } = e;
                     if (t === It) return void J(n, o);
-                    if (t === zt) return void q(e);
+                    if (t === zt) return void F(e);
                     const l = () => {
                         i(n), r && !r.persisted && r.afterLeave && r.afterLeave()
                     };
                     if (1 & e.shapeFlag && r && !r.persisted) {
                         const {
                             leave: t,
                             delayLeave: o
@@ -2487,28 +2487,28 @@
                         update: i,
                         subTree: a,
                         um: s
                     } = e;
                     o && (0, r.ir)(o), l.stop(), i && (i.active = !1, K(a, e, t, n)), s && Ct(s, t), Ct((() => {
                         e.isUnmounted = !0
                     }), t), t && t.pendingBranch && !t.isUnmounted && e.asyncDep && !e.asyncResolved && e.suspenseId === t.pendingId && (t.deps--, 0 === t.deps && t.resolve())
-                }, X = (e, t, n, o = !1, r = !1, l = 0) => {
+                }, Q = (e, t, n, o = !1, r = !1, l = 0) => {
                     for (let i = l; i < e.length; i++) K(e[i], t, n, o, r)
-                }, Q = e => 6 & e.shapeFlag ? Q(e.component.subTree) : 128 & e.shapeFlag ? e.suspense.next() : v(e.anchor || e.el), G = (e, t, n) => {
+                }, X = e => 6 & e.shapeFlag ? X(e.component.subTree) : 128 & e.shapeFlag ? e.suspense.next() : v(e.anchor || e.el), G = (e, t, n) => {
                     null == e ? t._vnode && K(t._vnode, null, null, !0) : g(t._vnode || null, e, t, null, null, null, n), k(), C(), t._vnode = e
                 }, ee = {
                     p: g,
                     um: K,
                     m: Z,
                     r: Y,
                     mt: B,
                     mc: P,
                     pc: z,
                     pbc: A,
-                    n: Q,
+                    n: X,
                     o: e
                 };
                 let te, ne;
                 return t && ([te, ne] = t(ee)), {
                     render: G,
                     hydrate: te,
                     createApp: St(G, te)
@@ -2711,19 +2711,19 @@
                 Yt += e
             }
 
             function Wt(e) {
                 return e.dynamicChildren = Yt > 0 ? Dt || r.Z6 : null, Kt(), Yt > 0 && Dt && Dt.push(e), e
             }
 
-            function Xt(e, t, n, o, r, l) {
+            function Qt(e, t, n, o, r, l) {
                 return Wt(rn(e, t, n, o, r, l, !0))
             }
 
-            function Qt(e, t, n, o, r) {
+            function Xt(e, t, n, o, r) {
                 return Wt(ln(e, t, n, o, r, !0))
             }
 
             function Gt(e) {
                 return !!e && !0 === e.__v_isVNode
             }
 
@@ -2838,15 +2838,15 @@
             }
 
             function cn(e = " ", t = 0) {
                 return ln(Nt, null, e, t)
             }
 
             function dn(e = "", t = !1) {
-                return t ? (Zt(), Qt(Ht, null, e)) : ln(Ht, null, e)
+                return t ? (Zt(), Xt(Ht, null, e)) : ln(Ht, null, e)
             }
 
             function fn(e) {
                 return null == e || "boolean" === typeof e ? ln(Ht) : (0, r.kJ)(e) ? ln(It, null, e.slice()) : "object" === typeof e ? pn(e) : ln(Nt, null, String(e))
             }
 
             function pn(e) {
@@ -2971,25 +2971,25 @@
                 xn = () => {
                     wn && wn.scope.off(), wn = null
                 };
 
             function kn(e) {
                 return 4 & e.vnode.shapeFlag
             }
-            let Cn, qn, Fn = !1;
+            let Cn, Fn, qn = !1;
 
             function En(e, t = !1) {
-                Fn = t;
+                qn = t;
                 const {
                     props: n,
                     children: o
                 } = e.vnode, r = kn(e);
                 rt(e, n, r, t), yt(e, o);
                 const l = r ? On(e, t) : void 0;
-                return Fn = !1, l
+                return qn = !1, l
             }
 
             function On(e, t) {
                 const n = e.type;
                 e.accessCache = Object.create(null), e.proxy = (0, o.Xl)(new Proxy(e.ctx, ze));
                 const {
                     setup: i
@@ -3029,15 +3029,15 @@
                             } = l, s = (0, r.l7)((0, r.l7)({
                                 isCustomElement: n,
                                 delimiters: i
                             }, o), a);
                             l.render = Cn(t, s)
                         }
                     }
-                    e.render = l.render || r.dG, qn && qn(e)
+                    e.render = l.render || r.dG, Fn && Fn(e)
                 }
                 Sn(e), (0, o.Jd)(), De(e), (0, o.lk)(), xn()
             }
 
             function An(e) {
                 return new Proxy(e.attrs, {
                     get(t, n) {
@@ -3075,15 +3075,15 @@
             function $n(e, t = !0) {
                 return (0, r.mf)(e) ? e.displayName || e.name : e.name || t && e.__name
             }
 
             function jn(e) {
                 return (0, r.mf)(e) && "__vccOpts" in e
             }
-            const Bn = (e, t) => (0, o.Fl)(e, t, Fn);
+            const Bn = (e, t) => (0, o.Fl)(e, t, qn);
 
             function Vn() {
                 return Mn().attrs
             }
 
             function Mn() {
                 const e = _n();
@@ -3265,25 +3265,25 @@
                     t = {};
                     while (n = e.match(x)) e = e.slice(0, e.length - n[0].length), t[n[0].toLowerCase()] = !0
                 }
                 const n = ":" === e[2] ? e.slice(3) : (0, o.rs)(e.slice(2));
                 return [n, t]
             }
             let C = 0;
-            const q = Promise.resolve(),
-                F = () => C || (q.then((() => C = 0)), C = Date.now());
+            const F = Promise.resolve(),
+                q = () => C || (F.then((() => C = 0)), C = Date.now());
 
             function E(e, t) {
                 const n = e => {
                     if (e._vts) {
                         if (e._vts <= n.attached) return
                     } else e._vts = Date.now();
                     (0, r.$d)(O(e, n.value), t, 5, [e])
                 };
-                return n.value = e, n.attached = F(), n
+                return n.value = e, n.attached = q(), n
             }
 
             function O(e, t) {
                 if ((0, o.kJ)(t)) {
                     const n = e.stopImmediatePropagation;
                     return e.stopImmediatePropagation = () => {
                         n.call(e), e._stopped = !0
@@ -3352,21 +3352,21 @@
                     onEnter: b,
                     onEnterCancelled: w,
                     onLeave: _,
                     onLeaveCancelled: S,
                     onBeforeAppear: x = y,
                     onAppear: k = b,
                     onAppearCancelled: C = w
-                } = t, q = (e, t, n) => {
+                } = t, F = (e, t, n) => {
                     U(e, t ? d : s), U(e, t ? c : a), n && n()
-                }, F = (e, t) => {
+                }, q = (e, t) => {
                     e._isLeaving = !1, U(e, f), U(e, v), U(e, p), t && t()
                 }, E = e => (t, n) => {
                     const o = e ? k : b,
-                        l = () => q(t, e, n);
+                        l = () => F(t, e, n);
                     V(o, [t, l]), D((() => {
                         U(t, e ? u : i), z(t, e ? d : s), M(o) || K(t, r, m, l)
                     }))
                 };
                 return (0, o.l7)(t, {
                     onBeforeEnter(e) {
                         V(y, [e]), z(e, i), z(e, a)
@@ -3374,27 +3374,27 @@
                     onBeforeAppear(e) {
                         V(x, [e]), z(e, u), z(e, c)
                     },
                     onEnter: E(!1),
                     onAppear: E(!0),
                     onLeave(e, t) {
                         e._isLeaving = !0;
-                        const n = () => F(e, t);
-                        z(e, f), X(), z(e, p), D((() => {
+                        const n = () => q(e, t);
+                        z(e, f), Q(), z(e, p), D((() => {
                             e._isLeaving && (U(e, f), z(e, v), M(_) || K(e, r, g, n))
                         })), V(_, [e, n])
                     },
                     onEnterCancelled(e) {
-                        q(e, !1), V(w, [e])
+                        F(e, !1), V(w, [e])
                     },
                     onAppearCancelled(e) {
-                        q(e, !0), V(C, [e])
+                        F(e, !0), V(C, [e])
                     },
                     onLeaveCancelled(e) {
-                        F(e), V(S, [e])
+                        q(e), V(S, [e])
                     }
                 })
             }
 
             function N(e) {
                 if (null == e) return null;
                 if ((0, o.Kn)(e)) return [H(e.enter), H(e.leave)]; {
@@ -3479,18 +3479,18 @@
                 return Math.max(...t.map(((t, n) => W(t) + W(e[n]))))
             }
 
             function W(e) {
                 return 1e3 * Number(e.slice(0, -1).replace(",", "."))
             }
 
-            function X() {
+            function Q() {
                 return document.body.offsetHeight
             }
-            const Q = new WeakMap,
+            const X = new WeakMap,
                 G = new WeakMap,
                 ee = {
                     name: "TransitionGroup",
                     props: (0, o.l7)({}, B, {
                         tag: String,
                         moveClass: String
                     }),
@@ -3502,15 +3502,15 @@
                         let i, a;
                         return (0, r.ic)((() => {
                             if (!i.length) return;
                             const t = e.moveClass || `${e.name||"v"}-move`;
                             if (!re(i[0].el, n.vnode.el, t)) return;
                             i.forEach(te), i.forEach(ne);
                             const o = i.filter(oe);
-                            X(), o.forEach((e => {
+                            Q(), o.forEach((e => {
                                 const n = e.el,
                                     o = n.style;
                                 z(n, t), o.transform = o.webkitTransform = o.transitionDuration = "";
                                 const r = n._moveCb = e => {
                                     e && e.target !== n || e && !/transform$/.test(e.propertyName) || (n.removeEventListener("transitionend", r), n._moveCb = null, U(n, t))
                                 };
                                 n.addEventListener("transitionend", r)
@@ -3523,15 +3523,15 @@
                             for (let e = 0; e < a.length; e++) {
                                 const t = a[e];
                                 null != t.key && (0, r.nK)(t, (0, r.U2)(t, u, o, n))
                             }
                             if (i)
                                 for (let e = 0; e < i.length; e++) {
                                     const t = i[e];
-                                    (0, r.nK)(t, (0, r.U2)(t, u, o, n)), Q.set(t, t.el.getBoundingClientRect())
+                                    (0, r.nK)(t, (0, r.U2)(t, u, o, n)), X.set(t, t.el.getBoundingClientRect())
                                 }
                             return (0, r.Wm)(c, null, a)
                         }
                     }
                 };
             ee.props;
 
@@ -3541,15 +3541,15 @@
             }
 
             function ne(e) {
                 G.set(e, e.el.getBoundingClientRect())
             }
 
             function oe(e) {
-                const t = Q.get(e),
+                const t = X.get(e),
                     n = G.get(e),
                     o = t.left - n.left,
                     r = t.top - n.top;
                 if (o || r) {
                     const t = e.el.style;
                     return t.transform = t.webkitTransform = `translate(${o}px,${r}px)`, t.transitionDuration = "0s", e
                 }
@@ -3690,22 +3690,22 @@
                 e1: () => l,
                 fY: () => o,
                 h5: () => oe,
                 hR: () => G,
                 hq: () => g,
                 ir: () => te,
                 j5: () => i,
-                kC: () => Q,
+                kC: () => X,
                 kJ: () => T,
                 kT: () => w,
-                l7: () => F,
+                l7: () => q,
                 mf: () => j,
-                rs: () => X,
+                rs: () => Q,
                 tI: () => I,
-                tR: () => q,
+                tR: () => F,
                 yA: () => v,
                 yk: () => V,
                 zw: () => y
             });
             const r = "Infinity,undefined,NaN,isFinite,isNaN,parseFloat,parseInt,decodeURI,decodeURIComponent,encodeURI,encodeURIComponent,Math,Number,Date,Array,Object,Boolean,String,RegExp,Map,Set,JSON,Intl,BigInt",
                 l = o(r);
 
@@ -3793,16 +3793,16 @@
                 } : !M(t) || T(t) || U(t) ? t : String(t),
                 w = {},
                 _ = [],
                 S = () => {},
                 x = () => !1,
                 k = /^on[^a-z]/,
                 C = e => k.test(e),
-                q = e => e.startsWith("onUpdate:"),
-                F = Object.assign,
+                F = e => e.startsWith("onUpdate:"),
+                q = Object.assign,
                 E = (e, t) => {
                     const n = e.indexOf(t);
                     n > -1 && e.splice(n, 1)
                 },
                 O = Object.prototype.hasOwnProperty,
                 P = (e, t) => O.call(e, t),
                 T = Array.isArray,
@@ -3827,17 +3827,17 @@
                         const o = t[n];
                         return o || (t[n] = e(n))
                     }
                 },
                 Y = /-(\w)/g,
                 J = K((e => e.replace(Y, ((e, t) => t ? t.toUpperCase() : "")))),
                 W = /\B([A-Z])/g,
-                X = K((e => e.replace(W, "-$1").toLowerCase())),
-                Q = K((e => e.charAt(0).toUpperCase() + e.slice(1))),
-                G = K((e => e ? `on${Q(e)}` : "")),
+                Q = K((e => e.replace(W, "-$1").toLowerCase())),
+                X = K((e => e.charAt(0).toUpperCase() + e.slice(1))),
+                G = K((e => e ? `on${X(e)}` : "")),
                 ee = (e, t) => !Object.is(e, t),
                 te = (e, t) => {
                     for (let n = 0; n < e.length; n++) e[n](t)
                 },
                 ne = (e, t, n) => {
                     Object.defineProperty(e, t, {
                         configurable: !0,
@@ -4671,34 +4671,34 @@
                 return e.trim ? e.trim() : e.replace(/^\s+|\s+$/g, "")
             }
 
             function C() {
                 return ("undefined" === typeof navigator || "ReactNative" !== navigator.product && "NativeScript" !== navigator.product && "NS" !== navigator.product) && ("undefined" !== typeof window && "undefined" !== typeof document)
             }
 
-            function q(e, t) {
+            function F(e, t) {
                 if (null !== e && "undefined" !== typeof e)
                     if ("object" !== typeof e && (e = [e]), a(e))
                         for (var n = 0, o = e.length; n < o; n++) t.call(null, e[n], n, e);
                     else
                         for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.call(null, e[r], r, e)
             }
 
-            function F() {
+            function q() {
                 var e = {};
 
                 function t(t, n) {
-                    h(e[n]) && h(t) ? e[n] = F(e[n], t) : h(t) ? e[n] = F({}, t) : a(t) ? e[n] = t.slice() : e[n] = t
+                    h(e[n]) && h(t) ? e[n] = q(e[n], t) : h(t) ? e[n] = q({}, t) : a(t) ? e[n] = t.slice() : e[n] = t
                 }
-                for (var n = 0, o = arguments.length; n < o; n++) q(arguments[n], t);
+                for (var n = 0, o = arguments.length; n < o; n++) F(arguments[n], t);
                 return e
             }
 
             function E(e, t, n) {
-                return q(t, (function(t, r) {
+                return F(t, (function(t, r) {
                     e[r] = n && "function" === typeof t ? o(t, n) : t
                 })), e
             }
 
             function O(e) {
                 return 65279 === e.charCodeAt(0) && (e = e.slice(1)), e
             }
@@ -4751,16 +4751,16 @@
                 isDate: m,
                 isFile: g,
                 isBlob: y,
                 isFunction: w,
                 isStream: _,
                 isURLSearchParams: x,
                 isStandardBrowserEnv: C,
-                forEach: q,
-                merge: F,
+                forEach: F,
+                merge: q,
                 extend: E,
                 trim: k,
                 stripBOM: O,
                 inherits: P,
                 toFlatObject: T,
                 kindOf: l,
                 kindOfTest: i,
@@ -4813,15 +4813,15 @@
                         style: b,
                         innerClasses: w,
                         attributes: _,
                         hasLink: S,
                         linkTag: x,
                         navigateOnClick: k,
                         isActionable: C
-                    } = (0, u.ZP)(e), q = (0, r.iH)(null), F = (0, r.iH)(null);
+                    } = (0, u.ZP)(e), F = (0, r.iH)(null), q = (0, r.iH)(null);
                     let E, O = null,
                         P = null;
                     const T = (0, o.Fl)((() => void 0 !== e.label && null !== e.label && "" !== e.label)),
                         A = (0, o.Fl)((() => !0 !== e.disable && !1 !== e.ripple && {
                             keyCodes: !0 === S.value ? [13, 32] : [13],
                             ...!0 === e.ripple ? {} : e.ripple
                         })),
@@ -4856,68 +4856,68 @@
                                 return t
                             }
                             return {
                                 onClick: f.NS
                             }
                         })),
                         j = (0, o.Fl)((() => ({
-                            ref: q,
+                            ref: F,
                             class: "q-btn q-btn-item non-selectable no-outline " + y.value,
                             style: b.value,
                             ..._.value,
                             ...$.value
                         })));
 
                     function B(t) {
-                        if (null !== q.value) {
+                        if (null !== F.value) {
                             if (void 0 !== t) {
                                 if (!0 === t.defaultPrevented) return;
                                 const n = document.activeElement;
-                                if ("submit" === e.type && n !== document.body && !1 === q.value.contains(n) && !1 === n.contains(q.value)) {
-                                    q.value.focus();
+                                if ("submit" === e.type && n !== document.body && !1 === F.value.contains(n) && !1 === n.contains(F.value)) {
+                                    F.value.focus();
                                     const e = () => {
-                                        document.removeEventListener("keydown", f.NS, !0), document.removeEventListener("keyup", e, v), null !== q.value && q.value.removeEventListener("blur", e, v)
+                                        document.removeEventListener("keydown", f.NS, !0), document.removeEventListener("keyup", e, v), null !== F.value && F.value.removeEventListener("blur", e, v)
                                     };
-                                    document.addEventListener("keydown", f.NS, !0), document.addEventListener("keyup", e, v), q.value.addEventListener("blur", e, v)
+                                    document.addEventListener("keydown", f.NS, !0), document.addEventListener("keyup", e, v), F.value.addEventListener("blur", e, v)
                                 }
                             }
                             k(t)
                         }
                     }
 
                     function V(e) {
-                        null !== q.value && (n("keydown", e), !0 === (0, p.So)(e, [13, 32]) && m !== q.value && (null !== m && H(), !0 !== e.defaultPrevented && (q.value.focus(), m = q.value, q.value.classList.add("q-btn--active"), document.addEventListener("keyup", N, !0), q.value.addEventListener("blur", N, v)), (0, f.NS)(e)))
+                        null !== F.value && (n("keydown", e), !0 === (0, p.So)(e, [13, 32]) && m !== F.value && (null !== m && H(), !0 !== e.defaultPrevented && (F.value.focus(), m = F.value, F.value.classList.add("q-btn--active"), document.addEventListener("keyup", N, !0), F.value.addEventListener("blur", N, v)), (0, f.NS)(e)))
                     }
 
                     function M(e) {
-                        null !== q.value && (n("touchstart", e), !0 !== e.defaultPrevented && (h !== q.value && (null !== h && H(), h = q.value, O = e.target, O.addEventListener("touchcancel", N, v), O.addEventListener("touchend", N, v)), E = !0, null !== P && clearTimeout(P), P = setTimeout((() => {
+                        null !== F.value && (n("touchstart", e), !0 !== e.defaultPrevented && (h !== F.value && (null !== h && H(), h = F.value, O = e.target, O.addEventListener("touchcancel", N, v), O.addEventListener("touchend", N, v)), E = !0, null !== P && clearTimeout(P), P = setTimeout((() => {
                             P = null, E = !1
                         }), 200)))
                     }
 
                     function I(e) {
-                        null !== q.value && (e.qSkipRipple = !0 === E, n("mousedown", e), !0 !== e.defaultPrevented && g !== q.value && (null !== g && H(), g = q.value, q.value.classList.add("q-btn--active"), document.addEventListener("mouseup", N, v)))
+                        null !== F.value && (e.qSkipRipple = !0 === E, n("mousedown", e), !0 !== e.defaultPrevented && g !== F.value && (null !== g && H(), g = F.value, F.value.classList.add("q-btn--active"), document.addEventListener("mouseup", N, v)))
                     }
 
                     function N(e) {
-                        if (null !== q.value && (void 0 === e || "blur" !== e.type || document.activeElement !== q.value)) {
+                        if (null !== F.value && (void 0 === e || "blur" !== e.type || document.activeElement !== F.value)) {
                             if (void 0 !== e && "keyup" === e.type) {
-                                if (m === q.value && !0 === (0, p.So)(e, [13, 32])) {
+                                if (m === F.value && !0 === (0, p.So)(e, [13, 32])) {
                                     const t = new MouseEvent("click", e);
-                                    t.qKeyEvent = !0, !0 === e.defaultPrevented && (0, f.X$)(t), !0 === e.cancelBubble && (0, f.sT)(t), q.value.dispatchEvent(t), (0, f.NS)(e), e.qKeyEvent = !0
+                                    t.qKeyEvent = !0, !0 === e.defaultPrevented && (0, f.X$)(t), !0 === e.cancelBubble && (0, f.sT)(t), F.value.dispatchEvent(t), (0, f.NS)(e), e.qKeyEvent = !0
                                 }
                                 n("keyup", e)
                             }
                             H()
                         }
                     }
 
                     function H(e) {
-                        const t = F.value;
-                        !0 === e || h !== q.value && g !== q.value || null === t || t === document.activeElement || (t.setAttribute("tabindex", -1), t.focus()), h === q.value && (null !== O && (O.removeEventListener("touchcancel", N, v), O.removeEventListener("touchend", N, v)), h = O = null), g === q.value && (document.removeEventListener("mouseup", N, v), g = null), m === q.value && (document.removeEventListener("keyup", N, !0), null !== q.value && q.value.removeEventListener("blur", N, v), m = null), null !== q.value && q.value.classList.remove("q-btn--active")
+                        const t = q.value;
+                        !0 === e || h !== F.value && g !== F.value || null === t || t === document.activeElement || (t.setAttribute("tabindex", -1), t.focus()), h === F.value && (null !== O && (O.removeEventListener("touchcancel", N, v), O.removeEventListener("touchend", N, v)), h = O = null), g === F.value && (document.removeEventListener("mouseup", N, v), g = null), m === F.value && (document.removeEventListener("keyup", N, !0), null !== F.value && F.value.removeEventListener("blur", N, v), m = null), null !== F.value && F.value.classList.remove("q-btn--active")
                     }
 
                     function z(e) {
                         (0, f.NS)(e), e.qSkipRipple = !0
                     }
                     return (0, o.Jd)((() => {
                         H(!0)
@@ -4936,15 +4936,15 @@
                             name: e.iconRight,
                             right: !1 === e.stack && !0 === T.value,
                             role: "img",
                             "aria-hidden": "true"
                         }));
                         const r = [(0, o.h)("span", {
                             class: "q-focus-helper",
-                            ref: F
+                            ref: q
                         })];
                         return !0 === e.loading && void 0 !== e.percentage && r.push((0, o.h)("span", {
                             class: "q-btn__progress absolute-full overflow-hidden" + (!0 === e.darkPercentage ? " q-btn__progress--dark" : "")
                         }, [(0, o.h)("span", {
                             class: "q-btn__progress-indicator fit block",
                             style: L.value
                         })])), r.push((0, o.h)("span", {
@@ -5174,57 +5174,100 @@
                     const n = (0, o.Fl)((() => "q-card__section q-card__section--" + (!0 === e.horizontal ? "horiz row no-wrap" : "vert")));
                     return () => (0, o.h)(e.tag, {
                         class: n.value
                     }, (0, l.KR)(t.default))
                 }
             })
         },
-        1006: (e, t, n) => {
+        1221: (e, t, n) => {
             "use strict";
             n.d(t, {
-                Z: () => y
+                Z: () => s
             });
             var o = n(9835),
                 r = n(2857),
                 l = n(5987),
-                i = (n(9665), n(499)),
-                a = n(8234),
-                s = n(244);
+                i = n(5413);
+            const a = (0, o.h)("div", {
+                    key: "svg",
+                    class: "q-checkbox__bg absolute"
+                }, [(0, o.h)("svg", {
+                    class: "q-checkbox__svg fit absolute-full",
+                    viewBox: "0 0 24 24"
+                }, [(0, o.h)("path", {
+                    class: "q-checkbox__truthy",
+                    fill: "none",
+                    d: "M1.73,12.91 8.1,19.28 22.79,4.59"
+                }), (0, o.h)("path", {
+                    class: "q-checkbox__indet",
+                    d: "M4,14H20V10H4"
+                })])]),
+                s = (0, l.L)({
+                    name: "QCheckbox",
+                    props: i.Fz,
+                    emits: i.ZB,
+                    setup(e) {
+                        function t(t, n) {
+                            const l = (0, o.Fl)((() => (!0 === t.value ? e.checkedIcon : !0 === n.value ? e.indeterminateIcon : e.uncheckedIcon) || null));
+                            return () => null !== l.value ? [(0, o.h)("div", {
+                                key: "icon",
+                                class: "q-checkbox__icon-container absolute-full flex flex-center no-wrap"
+                            }, [(0, o.h)(r.Z, {
+                                class: "q-checkbox__icon",
+                                name: l.value
+                            })])] : [a]
+                        }
+                        return (0, i.ZP)("checkbox", t)
+                    }
+                })
+        },
+        5413: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                ZP: () => v,
+                ZB: () => p,
+                Fz: () => f
+            });
+            n(9665);
+            var o = n(9835),
+                r = n(499),
+                l = n(8234),
+                i = n(244);
 
-            function u(e, t) {
-                const n = (0, i.iH)(null),
-                    r = (0, o.Fl)((() => !0 === e.disable ? null : (0, o.h)("span", {
+            function a(e, t) {
+                const n = (0, r.iH)(null),
+                    l = (0, o.Fl)((() => !0 === e.disable ? null : (0, o.h)("span", {
                         ref: n,
                         class: "no-outline",
                         tabindex: -1
                     })));
 
-                function l(e) {
+                function i(e) {
                     const o = t.value;
                     void 0 !== e && 0 === e.type.indexOf("key") ? null !== o && document.activeElement !== o && !0 === o.contains(document.activeElement) && o.focus() : null !== n.value && (void 0 === e || null !== o && !0 === o.contains(e.target)) && n.value.focus()
                 }
                 return {
-                    refocusTargetEl: r,
-                    refocusTarget: l
+                    refocusTargetEl: l,
+                    refocusTarget: i
                 }
             }
-            var c = n(9256);
-            const d = {
+            var s = n(9256);
+            const u = {
                 xs: 30,
                 sm: 35,
                 md: 40,
                 lg: 50,
                 xl: 60
             };
-            var f = n(1384),
-                p = n(2026);
-            const v = {
-                    ...a.S,
-                    ...s.LU,
-                    ...c.Fz,
+            var c = n(1384),
+                d = n(2026);
+            const f = {
+                    ...l.S,
+                    ...i.LU,
+                    ...s.Fz,
                     modelValue: {
                         required: !0,
                         default: null
                     },
                     val: {},
                     trueValue: {
                         default: !0
@@ -5247,56 +5290,56 @@
                     leftLabel: Boolean,
                     color: String,
                     keepColor: Boolean,
                     dense: Boolean,
                     disable: Boolean,
                     tabindex: [String, Number]
                 },
-                h = ["update:modelValue"];
+                p = ["update:modelValue"];
 
-            function m(e, t) {
+            function v(e, t) {
                 const {
                     props: n,
-                    slots: r,
-                    emit: l,
+                    slots: f,
+                    emit: p,
                     proxy: v
                 } = (0, o.FN)(), {
                     $q: h
-                } = v, m = (0, a.Z)(n, h), g = (0, i.iH)(null), {
+                } = v, m = (0, l.Z)(n, h), g = (0, r.iH)(null), {
                     refocusTargetEl: y,
                     refocusTarget: b
-                } = u(n, g), w = (0, s.ZP)(n, d), _ = (0, o.Fl)((() => void 0 !== n.val && Array.isArray(n.modelValue))), S = (0, o.Fl)((() => {
-                    const e = (0, i.IU)(n.val);
-                    return !0 === _.value ? n.modelValue.findIndex((t => (0, i.IU)(t) === e)) : -1
-                })), x = (0, o.Fl)((() => !0 === _.value ? S.value > -1 : (0, i.IU)(n.modelValue) === (0, i.IU)(n.trueValue))), k = (0, o.Fl)((() => !0 === _.value ? -1 === S.value : (0, i.IU)(n.modelValue) === (0, i.IU)(n.falseValue))), C = (0, o.Fl)((() => !1 === x.value && !1 === k.value)), q = (0, o.Fl)((() => !0 === n.disable ? -1 : n.tabindex || 0)), F = (0, o.Fl)((() => `q-${e} cursor-pointer no-outline row inline no-wrap items-center` + (!0 === n.disable ? " disabled" : "") + (!0 === m.value ? ` q-${e}--dark` : "") + (!0 === n.dense ? ` q-${e}--dense` : "") + (!0 === n.leftLabel ? " reverse" : ""))), E = (0, o.Fl)((() => {
+                } = a(n, g), w = (0, i.ZP)(n, u), _ = (0, o.Fl)((() => void 0 !== n.val && Array.isArray(n.modelValue))), S = (0, o.Fl)((() => {
+                    const e = (0, r.IU)(n.val);
+                    return !0 === _.value ? n.modelValue.findIndex((t => (0, r.IU)(t) === e)) : -1
+                })), x = (0, o.Fl)((() => !0 === _.value ? S.value > -1 : (0, r.IU)(n.modelValue) === (0, r.IU)(n.trueValue))), k = (0, o.Fl)((() => !0 === _.value ? -1 === S.value : (0, r.IU)(n.modelValue) === (0, r.IU)(n.falseValue))), C = (0, o.Fl)((() => !1 === x.value && !1 === k.value)), F = (0, o.Fl)((() => !0 === n.disable ? -1 : n.tabindex || 0)), q = (0, o.Fl)((() => `q-${e} cursor-pointer no-outline row inline no-wrap items-center` + (!0 === n.disable ? " disabled" : "") + (!0 === m.value ? ` q-${e}--dark` : "") + (!0 === n.dense ? ` q-${e}--dense` : "") + (!0 === n.leftLabel ? " reverse" : ""))), E = (0, o.Fl)((() => {
                     const t = !0 === x.value ? "truthy" : !0 === k.value ? "falsy" : "indet",
                         o = void 0 === n.color || !0 !== n.keepColor && ("toggle" === e ? !0 !== x.value : !0 === k.value) ? "" : ` text-${n.color}`;
                     return `q-${e}__inner relative-position non-selectable q-${e}__inner--${t}${o}`
                 })), O = (0, o.Fl)((() => {
                     const e = {
                         type: "checkbox"
                     };
                     return void 0 !== n.name && Object.assign(e, {
                         ".checked": x.value,
                         "^checked": !0 === x.value ? "checked" : void 0,
                         name: n.name,
                         value: !0 === _.value ? n.val : n.trueValue
                     }), e
-                })), P = (0, c.eX)(O), T = (0, o.Fl)((() => {
+                })), P = (0, s.eX)(O), T = (0, o.Fl)((() => {
                     const t = {
-                        tabindex: q.value,
+                        tabindex: F.value,
                         role: "toggle" === e ? "switch" : "checkbox",
                         "aria-label": n.label,
                         "aria-checked": !0 === C.value ? "mixed" : !0 === x.value ? "true" : "false"
                     };
                     return !0 === n.disable && (t["aria-disabled"] = "true"), t
                 }));
 
                 function A(e) {
-                    void 0 !== e && ((0, f.NS)(e), b(e)), !0 !== n.disable && l("update:modelValue", R(), e)
+                    void 0 !== e && ((0, c.NS)(e), b(e)), !0 !== n.disable && p("update:modelValue", R(), e)
                 }
 
                 function R() {
                     if (!0 === _.value) {
                         if (!0 === x.value) {
                             const e = n.modelValue.slice();
                             return e.splice(S.value, 1), e
@@ -5309,77 +5352,45 @@
                         if (!0 !== k.value) return "ft" !== n.toggleOrder ? n.trueValue : n.falseValue;
                         if ("ft" === n.toggleOrder || !1 === n.toggleIndeterminate) return n.trueValue
                     }
                     return n.indeterminateValue
                 }
 
                 function L(e) {
-                    13 !== e.keyCode && 32 !== e.keyCode || (0, f.NS)(e)
+                    13 !== e.keyCode && 32 !== e.keyCode || (0, c.NS)(e)
                 }
 
                 function $(e) {
                     13 !== e.keyCode && 32 !== e.keyCode || A(e)
                 }
                 const j = t(x, C);
                 return Object.assign(v, {
                     toggle: A
                 }), () => {
                     const t = j();
                     !0 !== n.disable && P(t, "unshift", ` q-${e}__native absolute q-ma-none q-pa-none`);
-                    const l = [(0, o.h)("div", {
+                    const r = [(0, o.h)("div", {
                         class: E.value,
                         style: w.value,
                         "aria-hidden": "true"
                     }, t)];
-                    null !== y.value && l.push(y.value);
-                    const i = void 0 !== n.label ? (0, p.vs)(r.default, [n.label]) : (0, p.KR)(r.default);
-                    return void 0 !== i && l.push((0, o.h)("div", {
+                    null !== y.value && r.push(y.value);
+                    const l = void 0 !== n.label ? (0, d.vs)(f.default, [n.label]) : (0, d.KR)(f.default);
+                    return void 0 !== l && r.push((0, o.h)("div", {
                         class: `q-${e}__label q-anchor--skip`
-                    }, i)), (0, o.h)("div", {
+                    }, l)), (0, o.h)("div", {
                         ref: g,
-                        class: F.value,
+                        class: q.value,
                         ...T.value,
                         onClick: A,
                         onKeydown: L,
                         onKeyup: $
-                    }, l)
+                    }, r)
                 }
             }
-            const g = (0, o.h)("div", {
-                    key: "svg",
-                    class: "q-checkbox__bg absolute"
-                }, [(0, o.h)("svg", {
-                    class: "q-checkbox__svg fit absolute-full",
-                    viewBox: "0 0 24 24"
-                }, [(0, o.h)("path", {
-                    class: "q-checkbox__truthy",
-                    fill: "none",
-                    d: "M1.73,12.91 8.1,19.28 22.79,4.59"
-                }), (0, o.h)("path", {
-                    class: "q-checkbox__indet",
-                    d: "M4,14H20V10H4"
-                })])]),
-                y = (0, l.L)({
-                    name: "QCheckbox",
-                    props: v,
-                    emits: h,
-                    setup(e) {
-                        function t(t, n) {
-                            const l = (0, o.Fl)((() => (!0 === t.value ? e.checkedIcon : !0 === n.value ? e.indeterminateIcon : e.uncheckedIcon) || null));
-                            return () => null !== l.value ? [(0, o.h)("div", {
-                                key: "icon",
-                                class: "q-checkbox__icon-container absolute-full flex flex-center no-wrap"
-                            }, [(0, o.h)(r.Z, {
-                                class: "q-checkbox__icon",
-                                name: l.value
-                            })])] : [g]
-                        }
-                        return m("checkbox", t)
-                    }
-                })
         },
         7691: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => f
             });
             n(9665);
@@ -5584,15 +5595,15 @@
                         emit: n,
                         attrs: p
                     }) {
                         const S = (0, o.FN)(),
                             x = (0, r.iH)(null),
                             k = (0, r.iH)(!1),
                             C = (0, r.iH)(!1);
-                        let q, F, E = null,
+                        let F, q, E = null,
                             O = null;
                         const P = (0, o.Fl)((() => !0 !== e.persistent && !0 !== e.noRouteDismiss && !0 !== e.seamless)),
                             {
                                 preventBodyScroll: T
                             } = (0, f.Z)(),
                             {
                                 registerTimeout: A
@@ -5639,15 +5650,15 @@
                                             top: e,
                                             bottom: t
                                         } = document.activeElement.getBoundingClientRect(), {
                                             innerHeight: n
                                         } = window, o = void 0 !== window.visualViewport ? window.visualViewport.height : n;
                                         e > 0 && t > o / 2 && (document.scrollingElement.scrollTop = Math.min(document.scrollingElement.scrollHeight - o, t >= n ? 1 / 0 : Math.ceil(document.scrollingElement.scrollTop + t - o / 2))), document.activeElement.scrollIntoView()
                                     }
-                                    F = !0, x.value.click(), F = !1
+                                    q = !0, x.value.click(), q = !1
                                 }
                                 B(!0), C.value = !1, n("show", t)
                             }), e.transitionDuration)
                         }
 
                         function J(t) {
                             L(), z(), G(!0), C.value = !0, V(), null !== O && (((t && 0 === t.type.indexOf("key") ? O.closest('[tabindex]:not([tabindex^="-"])') : void 0) || O).focus(), O = null), A((() => {
@@ -5660,42 +5671,42 @@
                                 let t = x.value;
                                 null !== t && !0 !== t.contains(document.activeElement) && (t = ("" !== e ? t.querySelector(e) : null) || t.querySelector("[autofocus][tabindex], [data-autofocus][tabindex]") || t.querySelector("[autofocus] [tabindex], [data-autofocus] [tabindex]") || t.querySelector("[autofocus], [data-autofocus]") || t, t.focus({
                                     preventScroll: !0
                                 }))
                             }))
                         }
 
-                        function X(e) {
+                        function Q(e) {
                             e && "function" === typeof e.focus ? e.focus({
                                 preventScroll: !0
                             }) : W(), n("shake");
                             const t = x.value;
                             null !== t && (t.classList.remove("q-animate--scale"), t.classList.add("q-animate--scale"), null !== E && clearTimeout(E), E = setTimeout((() => {
                                 E = null, null !== x.value && (t.classList.remove("q-animate--scale"), W())
                             }), 170))
                         }
 
-                        function Q() {
-                            !0 !== e.seamless && (!0 === e.persistent || !0 === e.noEscDismiss ? !0 !== e.maximized && !0 !== e.noShake && X() : (n("escapeKey"), N()))
+                        function X() {
+                            !0 !== e.seamless && (!0 === e.persistent || !0 === e.noEscDismiss ? !0 !== e.maximized && !0 !== e.noShake && Q() : (n("escapeKey"), N()))
                         }
 
                         function G(t) {
-                            null !== E && (clearTimeout(E), E = null), !0 !== t && !0 !== k.value || (ee(!1), !0 !== e.seamless && (T(!1), (0, g.H)(oe), (0, m.k)(Q))), !0 !== t && (O = null)
+                            null !== E && (clearTimeout(E), E = null), !0 !== t && !0 !== k.value || (ee(!1), !0 !== e.seamless && (T(!1), (0, g.H)(oe), (0, m.k)(X))), !0 !== t && (O = null)
                         }
 
                         function ee(e) {
-                            !0 === e ? !0 !== q && (b < 1 && document.body.classList.add("q-body--dialog"), b++, q = !0) : !0 === q && (b < 2 && document.body.classList.remove("q-body--dialog"), b--, q = !1)
+                            !0 === e ? !0 !== F && (b < 1 && document.body.classList.add("q-body--dialog"), b++, F = !0) : !0 === F && (b < 2 && document.body.classList.remove("q-body--dialog"), b--, F = !1)
                         }
 
                         function te(e) {
-                            !0 !== F && (N(e), n("click", e))
+                            !0 !== q && (N(e), n("click", e))
                         }
 
                         function ne(t) {
-                            !0 !== e.persistent && !0 !== e.noBackdropDismiss ? N(t) : !0 !== e.noShake && X()
+                            !0 !== e.persistent && !0 !== e.noBackdropDismiss ? N(t) : !0 !== e.noShake && Q()
                         }
 
                         function oe(t) {
                             !0 !== e.allowFocusOutside && !0 === M.value && !0 !== (0, v.mY)(x.value, t.target) && W('[tabindex]:not([tabindex="-1"])')
                         }
 
                         function re() {
@@ -5720,18 +5731,18 @@
                                 tabindex: -1,
                                 ...Z.value
                             }, (0, h.KR)(t.default)) : null))])
                         }
                         return (0, o.YP)((() => e.maximized), (e => {
                             !0 === k.value && ee(e)
                         })), (0, o.YP)(D, (e => {
-                            T(e), !0 === e ? ((0, g.i)(oe), (0, m.c)(Q)) : ((0, g.H)(oe), (0, m.k)(Q))
+                            T(e), !0 === e ? ((0, g.i)(oe), (0, m.c)(X)) : ((0, g.H)(oe), (0, m.k)(X))
                         })), Object.assign(S.proxy, {
                             focus: W,
-                            shake: X,
+                            shake: Q,
                             __updateRefocusTarget(e) {
                                 O = e || null
                             }
                         }), (0, o.Jd)(G), I
                     }
                 })
         },
@@ -6008,22 +6019,22 @@
                             {
                                 registerTimeout: h,
                                 removeTimeout: m
                             } = (0, s.Z)(),
                             g = (0, o.f3)(x.YE, x.qO);
                         if (g === x.qO) return console.error("QDrawer needs to be child of QLayout"), x.qO;
                         let y, b, C = null;
-                        const q = (0, r.iH)("mobile" === e.behavior || "desktop" !== e.behavior && g.totalWidth.value <= e.breakpoint),
-                            F = (0, o.Fl)((() => !0 === e.mini && !0 !== q.value)),
-                            E = (0, o.Fl)((() => !0 === F.value ? e.miniWidth : e.width)),
-                            O = (0, r.iH)(!0 === e.showIfAbove && !1 === q.value || !0 === e.modelValue),
-                            P = (0, o.Fl)((() => !0 !== e.persistent && (!0 === q.value || !0 === Y.value)));
+                        const F = (0, r.iH)("mobile" === e.behavior || "desktop" !== e.behavior && g.totalWidth.value <= e.breakpoint),
+                            q = (0, o.Fl)((() => !0 === e.mini && !0 !== F.value)),
+                            E = (0, o.Fl)((() => !0 === q.value ? e.miniWidth : e.width)),
+                            O = (0, r.iH)(!0 === e.showIfAbove && !1 === F.value || !0 === e.modelValue),
+                            P = (0, o.Fl)((() => !0 !== e.persistent && (!0 === F.value || !0 === Y.value)));
 
                         function T(e, t) {
-                            if ($(), !1 !== e && g.animate(), ae(0), !0 === q.value) {
+                            if ($(), !1 !== e && g.animate(), ae(0), !0 === F.value) {
                                 const e = g.instances[U.value];
                                 void 0 !== e && !0 === e.belowBreakpoint && e.hide(!1), se(1), !0 !== g.isContainer.value && v(!0)
                             } else se(0), !1 !== e && ue(!1);
                             h((() => {
                                 !1 !== e && ue(!0), !0 !== t && n("show", e)
                             }), k)
                         }
@@ -6041,28 +6052,28 @@
                             hideOnRouteChange: P,
                             handleShow: T,
                             handleHide: A
                         }), {
                             addToHistory: $,
                             removeFromHistory: j
                         } = (0, l.Z)(O, L, P), B = {
-                            belowBreakpoint: q,
+                            belowBreakpoint: F,
                             hide: L
-                        }, V = (0, o.Fl)((() => "right" === e.side)), M = (0, o.Fl)((() => (!0 === f.lang.rtl ? -1 : 1) * (!0 === V.value ? 1 : -1))), I = (0, r.iH)(0), N = (0, r.iH)(!1), H = (0, r.iH)(!1), z = (0, r.iH)(E.value * M.value), U = (0, o.Fl)((() => !0 === V.value ? "left" : "right")), D = (0, o.Fl)((() => !0 === O.value && !1 === q.value && !1 === e.overlay ? !0 === e.miniToOverlay ? e.miniWidth : E.value : 0)), Z = (0, o.Fl)((() => !0 === e.overlay || !0 === e.miniToOverlay || g.view.value.indexOf(V.value ? "R" : "L") > -1 || !0 === f.platform.is.ios && !0 === g.isContainer.value)), K = (0, o.Fl)((() => !1 === e.overlay && !0 === O.value && !1 === q.value)), Y = (0, o.Fl)((() => !0 === e.overlay && !0 === O.value && !1 === q.value)), J = (0, o.Fl)((() => "fullscreen q-drawer__backdrop" + (!1 === O.value && !1 === N.value ? " hidden" : ""))), W = (0, o.Fl)((() => ({
+                        }, V = (0, o.Fl)((() => "right" === e.side)), M = (0, o.Fl)((() => (!0 === f.lang.rtl ? -1 : 1) * (!0 === V.value ? 1 : -1))), I = (0, r.iH)(0), N = (0, r.iH)(!1), H = (0, r.iH)(!1), z = (0, r.iH)(E.value * M.value), U = (0, o.Fl)((() => !0 === V.value ? "left" : "right")), D = (0, o.Fl)((() => !0 === O.value && !1 === F.value && !1 === e.overlay ? !0 === e.miniToOverlay ? e.miniWidth : E.value : 0)), Z = (0, o.Fl)((() => !0 === e.overlay || !0 === e.miniToOverlay || g.view.value.indexOf(V.value ? "R" : "L") > -1 || !0 === f.platform.is.ios && !0 === g.isContainer.value)), K = (0, o.Fl)((() => !1 === e.overlay && !0 === O.value && !1 === F.value)), Y = (0, o.Fl)((() => !0 === e.overlay && !0 === O.value && !1 === F.value)), J = (0, o.Fl)((() => "fullscreen q-drawer__backdrop" + (!1 === O.value && !1 === N.value ? " hidden" : ""))), W = (0, o.Fl)((() => ({
                             backgroundColor: `rgba(0,0,0,${.4*I.value})`
-                        }))), X = (0, o.Fl)((() => !0 === V.value ? "r" === g.rows.value.top[2] : "l" === g.rows.value.top[0])), Q = (0, o.Fl)((() => !0 === V.value ? "r" === g.rows.value.bottom[2] : "l" === g.rows.value.bottom[0])), G = (0, o.Fl)((() => {
+                        }))), Q = (0, o.Fl)((() => !0 === V.value ? "r" === g.rows.value.top[2] : "l" === g.rows.value.top[0])), X = (0, o.Fl)((() => !0 === V.value ? "r" === g.rows.value.bottom[2] : "l" === g.rows.value.bottom[0])), G = (0, o.Fl)((() => {
                             const e = {};
-                            return !0 === g.header.space && !1 === X.value && (!0 === Z.value ? e.top = `${g.header.offset}px` : !0 === g.header.space && (e.top = `${g.header.size}px`)), !0 === g.footer.space && !1 === Q.value && (!0 === Z.value ? e.bottom = `${g.footer.offset}px` : !0 === g.footer.space && (e.bottom = `${g.footer.size}px`)), e
+                            return !0 === g.header.space && !1 === Q.value && (!0 === Z.value ? e.top = `${g.header.offset}px` : !0 === g.header.space && (e.top = `${g.header.size}px`)), !0 === g.footer.space && !1 === X.value && (!0 === Z.value ? e.bottom = `${g.footer.offset}px` : !0 === g.footer.space && (e.bottom = `${g.footer.size}px`)), e
                         })), ee = (0, o.Fl)((() => {
                             const e = {
                                 width: `${E.value}px`,
                                 transform: `translateX(${z.value}px)`
                             };
-                            return !0 === q.value ? e : Object.assign(e, G.value)
-                        })), te = (0, o.Fl)((() => "q-drawer__content fit " + (!0 !== g.isContainer.value ? "scroll" : "overflow-auto"))), ne = (0, o.Fl)((() => `q-drawer q-drawer--${e.side}` + (!0 === H.value ? " q-drawer--mini-animate" : "") + (!0 === e.bordered ? " q-drawer--bordered" : "") + (!0 === p.value ? " q-drawer--dark q-dark" : "") + (!0 === N.value ? " no-transition" : !0 === O.value ? "" : " q-layout--prevent-focus") + (!0 === q.value ? " fixed q-drawer--on-top q-drawer--mobile q-drawer--top-padding" : " q-drawer--" + (!0 === F.value ? "mini" : "standard") + (!0 === Z.value || !0 !== K.value ? " fixed" : "") + (!0 === e.overlay || !0 === e.miniToOverlay ? " q-drawer--on-top" : "") + (!0 === X.value ? " q-drawer--top-padding" : "")))), oe = (0, o.Fl)((() => {
+                            return !0 === F.value ? e : Object.assign(e, G.value)
+                        })), te = (0, o.Fl)((() => "q-drawer__content fit " + (!0 !== g.isContainer.value ? "scroll" : "overflow-auto"))), ne = (0, o.Fl)((() => `q-drawer q-drawer--${e.side}` + (!0 === H.value ? " q-drawer--mini-animate" : "") + (!0 === e.bordered ? " q-drawer--bordered" : "") + (!0 === p.value ? " q-drawer--dark q-dark" : "") + (!0 === N.value ? " no-transition" : !0 === O.value ? "" : " q-layout--prevent-focus") + (!0 === F.value ? " fixed q-drawer--on-top q-drawer--mobile q-drawer--top-padding" : " q-drawer--" + (!0 === q.value ? "mini" : "standard") + (!0 === Z.value || !0 !== K.value ? " fixed" : "") + (!0 === e.overlay || !0 === e.miniToOverlay ? " q-drawer--on-top" : "") + (!0 === Q.value ? " q-drawer--top-padding" : "")))), oe = (0, o.Fl)((() => {
                             const t = !0 === f.lang.rtl ? e.side : U.value;
                             return [
                                 [w, de, void 0, {
                                     [t]: !0,
                                     mouse: !0
                                 }]
                             ]
@@ -6082,21 +6093,21 @@
                                     mouse: !0,
                                     mouseAllDir: !0
                                 }]
                             ]
                         }));
 
                         function ie() {
-                            he(q, "mobile" === e.behavior || "desktop" !== e.behavior && g.totalWidth.value <= e.breakpoint)
+                            he(F, "mobile" === e.behavior || "desktop" !== e.behavior && g.totalWidth.value <= e.breakpoint)
                         }
 
                         function ae(e) {
                             void 0 === e ? (0, o.Y3)((() => {
                                 e = !0 === O.value ? 0 : E.value, ae(M.value * e)
-                            })) : (!0 !== g.isContainer.value || !0 !== V.value || !0 !== q.value && Math.abs(e) !== E.value || (e += M.value * g.scrollbarWidth.value), z.value = e)
+                            })) : (!0 !== g.isContainer.value || !0 !== V.value || !0 !== F.value && Math.abs(e) !== E.value || (e += M.value * g.scrollbarWidth.value), z.value = e)
                         }
 
                         function se(e) {
                             I.value = e
                         }
 
                         function ue(e) {
@@ -6144,15 +6155,15 @@
                         function he(e, t) {
                             e.value !== t && (e.value = t)
                         }
 
                         function me(t, n) {
                             ve("size", !0 === t ? e.miniWidth : n)
                         }
-                        return (0, o.YP)(q, (t => {
+                        return (0, o.YP)(F, (t => {
                             !0 === t ? (y = O.value, !0 === O.value && L(!1)) : !1 === e.overlay && "mobile" !== e.behavior && !1 !== y && (!0 === O.value ? (ae(0), se(0), pe()) : R(!1))
                         })), (0, o.YP)((() => e.side), ((e, t) => {
                             g.instances[t] === B && (g.instances[t] = void 0, g[t].space = !1, g[t].offset = 0), g.instances[e] = B, g[e].size = E.value, g[e].space = K.value, g[e].offset = D.value
                         })), (0, o.YP)(g.totalWidth, (() => {
                             !0 !== g.isContainer.value && !0 === document.qScrollPrevented || ie()
                         })), (0, o.YP)((() => e.behavior + e.breakpoint), ie), (0, o.YP)(g.isContainer, (e => {
                             !0 === O.value && v(!0 !== e), !0 === e && ie()
@@ -6168,53 +6179,53 @@
                             ae(), me(e.miniToOverlay, t)
                         })), (0, o.YP)((() => e.miniToOverlay), (e => {
                             me(e, E.value)
                         })), (0, o.YP)((() => f.lang.rtl), (() => {
                             ae()
                         })), (0, o.YP)((() => e.mini), (() => {
                             !0 === e.modelValue && (ce(), g.animate())
-                        })), (0, o.YP)(F, (e => {
+                        })), (0, o.YP)(q, (e => {
                             n("miniState", e)
                         })), g.instances[e.side] = B, me(e.miniToOverlay, E.value), ve("space", K.value), ve("offset", D.value), !0 === e.showIfAbove && !0 !== e.modelValue && !0 === O.value && void 0 !== e["onUpdate:modelValue"] && n("update:modelValue", !0), (0, o.bv)((() => {
-                            n("onLayout", K.value), n("miniState", F.value), y = !0 === e.showIfAbove;
+                            n("onLayout", K.value), n("miniState", q.value), y = !0 === e.showIfAbove;
                             const t = () => {
                                 const e = !0 === O.value ? T : A;
                                 e(!1, !0)
                             };
                             0 === g.totalWidth.value ? b = (0, o.YP)(g.totalWidth, (() => {
-                                b(), b = void 0, !1 === O.value && !0 === e.showIfAbove && !1 === q.value ? R(!1) : t()
+                                b(), b = void 0, !1 === O.value && !0 === e.showIfAbove && !1 === F.value ? R(!1) : t()
                             })) : (0, o.Y3)(t)
                         })), (0, o.Jd)((() => {
                             void 0 !== b && b(), null !== C && (clearTimeout(C), C = null), !0 === O.value && pe(), g.instances[e.side] === B && (g.instances[e.side] = void 0, ve("size", 0), ve("offset", 0), ve("space", !1))
                         })), () => {
                             const n = [];
-                            !0 === q.value && (!1 === e.noSwipeOpen && n.push((0, o.wy)((0, o.h)("div", {
+                            !0 === F.value && (!1 === e.noSwipeOpen && n.push((0, o.wy)((0, o.h)("div", {
                                 key: "open",
                                 class: `q-drawer__opener fixed-${e.side}`,
                                 "aria-hidden": "true"
                             }), oe.value)), n.push((0, S.Jl)("div", {
                                 ref: "backdrop",
                                 class: J.value,
                                 style: W.value,
                                 "aria-hidden": "true",
                                 onClick: L
                             }, void 0, "backdrop", !0 !== e.noSwipeBackdrop && !0 === O.value, (() => le.value))));
-                            const r = !0 === F.value && void 0 !== t.mini,
+                            const r = !0 === q.value && void 0 !== t.mini,
                                 l = [(0, o.h)("div", {
                                     ...c,
                                     key: "" + r,
                                     class: [te.value, c.class]
                                 }, !0 === r ? t.mini() : (0, S.KR)(t.default))];
                             return !0 === e.elevated && !0 === O.value && l.push((0, o.h)("div", {
                                 class: "q-layout__shadow absolute-full overflow-hidden no-pointer-events"
                             })), n.push((0, S.Jl)("aside", {
                                 ref: "content",
                                 class: ne.value,
                                 style: ee.value
-                            }, l, "contentclose", !0 !== e.noSwipeClose && !0 === q.value, (() => re.value))), (0, o.h)("div", {
+                            }, l, "contentclose", !0 !== e.noSwipeClose && !0 === F.value, (() => re.value))), (0, o.h)("div", {
                                 class: "q-drawer-container"
                             }, n)
                         }
                     }
                 })
         },
         8149: (e, t, n) => {
@@ -6326,17 +6337,17 @@
                     })), (0, o.YP)((() => e.reveal), (t => {
                         !1 === t && S(f, e.modelValue)
                     })), (0, o.YP)(f, (e => {
                         c.animate(), n("reveal", e)
                     })), (0, o.YP)([d, c.scroll, c.height], k), (0, o.YP)((() => a.screen.height), (e => {
                         !0 !== c.isContainer.value && S(p, e)
                     }));
-                    const q = {};
-                    return c.instances.footer = q, !0 === e.modelValue && _("size", d.value), _("space", e.modelValue), _("offset", m.value), (0, o.Jd)((() => {
-                        c.instances.footer === q && (c.instances.footer = void 0, _("size", 0), _("offset", 0), _("space", !1))
+                    const F = {};
+                    return c.instances.footer = F, !0 === e.modelValue && _("size", d.value), _("space", e.modelValue), _("offset", m.value), (0, o.Jd)((() => {
+                        c.instances.footer === F && (c.instances.footer = void 0, _("size", 0), _("offset", 0), _("space", !1))
                     })), () => {
                         const n = (0, s.vs)(t.default, [(0, o.h)(i.Z, {
                             debounce: 0,
                             onResize: x
                         })]);
                         return !0 === e.elevated && n.push((0, o.h)("div", {
                             class: "q-layout__shadow absolute-full overflow-hidden no-pointer-events"
@@ -6880,30 +6891,30 @@
                             if ("insertFromPaste" !== i || !0 === e.reverseFillMask)
                                 if (["deleteContentBackward", "deleteContentForward"].indexOf(i) > -1) {
                                     const t = !0 === e.reverseFillMask ? 0 === s ? h.length > v.length ? 1 : 0 : Math.max(0, h.length - (h === p ? 0 : Math.min(v.length, c) + 1)) + 1 : s;
                                     a.setSelectionRange(t, t, "forward")
                                 } else if (!0 === e.reverseFillMask)
                             if (!0 === g) {
                                 const e = Math.max(0, h.length - (h === p ? 0 : Math.min(v.length, c + 1)));
-                                1 === e && 1 === s ? a.setSelectionRange(e, e, "forward") : q.rightReverse(a, e)
+                                1 === e && 1 === s ? a.setSelectionRange(e, e, "forward") : F.rightReverse(a, e)
                             } else {
                                 const e = h.length - c;
                                 a.setSelectionRange(e, e, "backward")
                             }
                         else if (!0 === g) {
                             const e = Math.max(0, u.indexOf(f), Math.min(v.length, s) - 1);
-                            q.right(a, e)
+                            F.right(a, e)
                         } else {
                             const e = s - 1;
-                            q.right(a, e)
+                            F.right(a, e)
                         } else {
                             const e = a.selectionEnd;
                             let t = s - 1;
                             for (let n = m; n <= t && n < e; n++) u[n] !== f && t++;
-                            q.right(a, t)
+                            F.right(a, t)
                         } else {
                             const t = !0 === e.reverseFillMask ? p.length : 0;
                             a.setSelectionRange(t, t, "forward")
                         }
                     }));
                     const y = !0 === e.unmaskedValue ? T(h) : h;
                     String(e.modelValue) !== y && n(y, !0)
@@ -6919,82 +6930,82 @@
                         x(), e.modelValue !== n && t("update:modelValue", n)
                     }
                 })), (0, o.YP)((() => e.fillMask + e.reverseFillMask), (() => {
                     !0 === y.value && k(b.value, !0)
                 })), (0, o.YP)((() => e.unmaskedValue), (() => {
                     !0 === y.value && k(b.value)
                 }));
-                const q = {
+                const F = {
                     left(e, t) {
                         const n = -1 === u.slice(t - 1).indexOf(f);
                         let o = Math.max(0, t - 1);
                         for (; o >= 0; o--)
                             if (u[o] === f) {
                                 t = o, !0 === n && t++;
                                 break
-                            } if (o < 0 && void 0 !== u[t] && u[t] !== f) return q.right(e, 0);
+                            } if (o < 0 && void 0 !== u[t] && u[t] !== f) return F.right(e, 0);
                         t >= 0 && e.setSelectionRange(t, t, "backward")
                     },
                     right(e, t) {
                         const n = e.value.length;
                         let o = Math.min(n, t + 1);
                         for (; o <= n; o++) {
                             if (u[o] === f) {
                                 t = o;
                                 break
                             }
                             u[o - 1] === f && (t = o)
                         }
-                        if (o > n && void 0 !== u[t - 1] && u[t - 1] !== f) return q.left(e, n);
+                        if (o > n && void 0 !== u[t - 1] && u[t - 1] !== f) return F.left(e, n);
                         e.setSelectionRange(t, t, "forward")
                     },
                     leftReverse(e, t) {
                         const n = S(e.value.length);
                         let o = Math.max(0, t - 1);
                         for (; o >= 0; o--) {
                             if (n[o - 1] === f) {
                                 t = o;
                                 break
                             }
                             if (n[o] === f && (t = o, 0 === o)) break
                         }
-                        if (o < 0 && void 0 !== n[t] && n[t] !== f) return q.rightReverse(e, 0);
+                        if (o < 0 && void 0 !== n[t] && n[t] !== f) return F.rightReverse(e, 0);
                         t >= 0 && e.setSelectionRange(t, t, "backward")
                     },
                     rightReverse(e, t) {
                         const n = e.value.length,
                             o = S(n),
                             r = -1 === o.slice(0, t + 1).indexOf(f);
                         let l = Math.min(n, t + 1);
                         for (; l <= n; l++)
                             if (o[l - 1] === f) {
                                 t = l, t > 0 && !0 === r && t--;
                                 break
-                            } if (l > n && void 0 !== o[t - 1] && o[t - 1] !== f) return q.leftReverse(e, n);
+                            } if (l > n && void 0 !== o[t - 1] && o[t - 1] !== f) return F.leftReverse(e, n);
                         e.setSelectionRange(t, t, "forward")
                     }
                 };
 
-                function F(e) {
+                function q(e) {
                     t("click", e), g = void 0
                 }
 
                 function E(n) {
                     if (t("keydown", n), !0 === (0, i.Wm)(n)) return;
                     const o = l.value,
                         r = o.selectionStart,
                         a = o.selectionEnd;
                     if (n.shiftKey || (g = void 0), 37 === n.keyCode || 39 === n.keyCode) {
                         n.shiftKey && void 0 === g && (g = "forward" === o.selectionDirection ? r : a);
-                        const t = q[(39 === n.keyCode ? "right" : "left") + (!0 === e.reverseFillMask ? "Reverse" : "")];
+                        const t = F[(39 === n.keyCode ? "right" : "left") + (!0 === e.reverseFillMask ? "Reverse" : "")];
                         if (n.preventDefault(), t(o, g === r ? a : r), n.shiftKey) {
                             const e = o.selectionStart;
                             o.setSelectionRange(Math.min(g, e), Math.max(g, e), "forward")
                         }
-                    } else 8 === n.keyCode && !0 !== e.reverseFillMask && r === a ? q.left(o, r) : 46 === n.keyCode && !0 === e.reverseFillMask && r === a && q.rightReverse(o, a)
+                    } else 8 === n.keyCode && !0 !== e.reverseFillMask && r === a ? F.left(o, r) : 46 === n.keyCode && !0 === e.reverseFillMask && r === a && F.rightReverse(o, a)
                 }
 
                 function O(t) {
                     if (void 0 === t || null === t || "" === t) return "";
                     if (!0 === e.reverseFillMask) return P(t);
                     const n = v;
                     let o = 0,
@@ -7039,15 +7050,15 @@
                 }
                 return {
                     innerValue: b,
                     hasMask: y,
                     moveCursorForPaste: C,
                     updateMaskValue: k,
                     onMaskedKeydown: E,
-                    onMaskedClick: F
+                    onMaskedClick: q
                 }
             }
             var h = n(9256);
 
             function m(e, t) {
                 function n() {
                     const t = e.modelValue;
@@ -7107,16 +7118,16 @@
                         p = null;
                     const y = (0, r.iH)(null),
                         S = (0, h.Do)(e),
                         {
                             innerValue: x,
                             hasMask: k,
                             moveCursorForPaste: C,
-                            updateMaskValue: q,
-                            onMaskedKeydown: F,
+                            updateMaskValue: F,
+                            onMaskedKeydown: q,
                             onMaskedClick: E
                         } = v(e, t, H, y),
                         O = m(e, !0),
                         P = (0, o.Fl)((() => (0, l.yV)(x.value))),
                         T = (0, g.Z)(I),
                         A = (0, l.tL)(),
                         R = (0, o.Fl)((() => "textarea" === e.type || !0 === e.autogrow)),
@@ -7126,15 +7137,15 @@
                                 ...A.splitAttrs.listeners.value,
                                 onInput: I,
                                 onPaste: M,
                                 onChange: U,
                                 onBlur: D,
                                 onFocus: b.sT
                             };
-                            return t.onCompositionstart = t.onCompositionupdate = t.onCompositionend = T, !0 === k.value && (t.onKeydown = F, t.onClick = E), !0 === e.autogrow && (t.onAnimationend = N), t
+                            return t.onCompositionstart = t.onCompositionupdate = t.onCompositionend = T, !0 === k.value && (t.onKeydown = q, t.onClick = E), !0 === e.autogrow && (t.onAnimationend = N), t
                         })),
                         j = (0, o.Fl)((() => {
                             const t = {
                                 tabindex: 0,
                                 "data-autofocus": !0 === e.autofocus || void 0,
                                 rows: "textarea" === e.type ? 6 : void 0,
                                 "aria-label": e.label,
@@ -7170,15 +7181,15 @@
                     }
 
                     function I(n) {
                         if (!n || !n.target) return;
                         if ("file" === e.type) return void t("update:modelValue", n.target.files);
                         const r = n.target.value;
                         if (!0 !== n.target.qComposing) {
-                            if (!0 === k.value) q(r, !1, n.inputType);
+                            if (!0 === k.value) F(r, !1, n.inputType);
                             else if (H(r), !0 === L.value && n.target === document.activeElement) {
                                 const {
                                     selectionStart: e,
                                     selectionEnd: t
                                 } = n.target;
                                 void 0 !== e && void 0 !== t && (0, o.Y3)((() => {
                                     n.target === document.activeElement && 0 === r.indexOf(n.target.value) && n.target.setSelectionRange(e, t)
@@ -7230,15 +7241,15 @@
                     function Z() {
                         return !0 === s.hasOwnProperty("value") ? s.value : void 0 !== x.value ? x.value : ""
                     }(0, o.YP)((() => e.type), (() => {
                         y.value && (y.value.value = e.modelValue)
                     })), (0, o.YP)((() => e.modelValue), (t => {
                         if (!0 === k.value) {
                             if (!0 === c && (c = !1, String(t) === f)) return;
-                            q(t)
+                            F(t)
                         } else x.value !== t && (x.value = t, "number" === e.type && !0 === s.hasOwnProperty("value") && (!0 === u ? u = !1 : delete s.value));
                         !0 === e.autogrow && (0, o.Y3)(z)
                     })), (0, o.YP)((() => e.autogrow), (e => {
                         !0 === e ? (0, o.Y3)(z) : null !== y.value && n.rows > 0 && (y.value.style.height = "auto")
                     })), (0, o.YP)((() => e.dense), (() => {
                         !0 === e.autogrow && (0, o.Y3)(z)
                     })), (0, o.Jd)((() => {
@@ -7597,16 +7608,16 @@
 
                     function C() {
                         if (!0 === e.container) {
                             const e = u.value > m.value ? (0, a.np)() : 0;
                             g.value !== e && (g.value = e)
                         }
                     }
-                    let q = null;
-                    const F = {
+                    let F = null;
+                    const q = {
                         instances: {},
                         view: (0, o.Fl)((() => e.view)),
                         isContainer: (0, o.Fl)((() => e.container)),
                         rootRef: s,
                         height: u,
                         containerHeight: m,
                         scrollbarWidth: g,
@@ -7637,23 +7648,23 @@
                         left: (0, r.qj)({
                             size: 300,
                             offset: 0,
                             space: !1
                         }),
                         scroll: h,
                         animate() {
-                            null !== q ? clearTimeout(q) : document.body.classList.add("q-body--layout-animate"), q = setTimeout((() => {
-                                q = null, document.body.classList.remove("q-body--layout-animate")
+                            null !== F ? clearTimeout(F) : document.body.classList.add("q-body--layout-animate"), F = setTimeout((() => {
+                                F = null, document.body.classList.remove("q-body--layout-animate")
                             }), 155)
                         },
                         update(e, t, n) {
-                            F[e][t] = n
+                            q[e][t] = n
                         }
                     };
-                    if ((0, o.JJ)(v.YE, F), (0, a.np)() > 0) {
+                    if ((0, o.JJ)(v.YE, q), (0, a.np)() > 0) {
                         let E = null;
                         const O = document.body;
 
                         function P() {
                             E = null, O.classList.remove("hide-scrollbar")
                         }
 
@@ -7770,15 +7781,15 @@
                 },
                 emits: [...s.gH, "click", "escapeKey"],
                 setup(e, {
                     slots: t,
                     emit: n,
                     attrs: v
                 }) {
-                    let C, q, F, E = null;
+                    let C, F, q, E = null;
                     const O = (0, o.FN)(),
                         {
                             proxy: P
                         } = O,
                         {
                             $q: T
                         } = P,
@@ -7826,16 +7837,16 @@
                         W = {
                             anchorEl: U,
                             innerRef: A,
                             onClickOutside(t) {
                                 if (!0 !== e.persistent && !0 === R.value) return Z(t), ("touchstart" === t.type || t.target.classList.contains("q-dialog__backdrop")) && (0, g.NS)(t), !0
                             }
                         },
-                        X = (0, o.Fl)((() => (0, k.li)(e.anchor || (!0 === e.cover ? "center middle" : "bottom start"), T.lang.rtl))),
-                        Q = (0, o.Fl)((() => !0 === e.cover ? X.value : (0, k.li)(e.self || "top start", T.lang.rtl))),
+                        Q = (0, o.Fl)((() => (0, k.li)(e.anchor || (!0 === e.cover ? "center middle" : "bottom start"), T.lang.rtl))),
+                        X = (0, o.Fl)((() => !0 === e.cover ? Q.value : (0, k.li)(e.self || "top start", T.lang.rtl))),
                         G = (0, o.Fl)((() => (!0 === e.square ? " q-menu--square" : "") + (!0 === $.value ? " q-menu--dark q-dark" : ""))),
                         ee = (0, o.Fl)((() => !0 === e.autoClose ? {
                             onClick: ae
                         } : {})),
                         te = (0, o.Fl)((() => !0 === R.value && !0 !== e.persistent));
 
                     function ne() {
@@ -7857,37 +7868,37 @@
                                 } = U.value.getBoundingClientRect();
                                 C = {
                                     left: e.left - n,
                                     top: e.top - t
                                 }
                             }
                         }
-                        void 0 === q && (q = (0, o.YP)((() => T.screen.width + "|" + T.screen.height + "|" + e.self + "|" + e.anchor + "|" + T.lang.rtl), ce)), !0 !== e.noFocus && document.activeElement.blur(), j((() => {
+                        void 0 === F && (F = (0, o.YP)((() => T.screen.width + "|" + T.screen.height + "|" + e.self + "|" + e.anchor + "|" + T.lang.rtl), ce)), !0 !== e.noFocus && document.activeElement.blur(), j((() => {
                             ce(), !0 !== e.noFocus && ne()
                         })), V((() => {
-                            !0 === T.platform.is.ios && (F = e.autoClose, A.value.click()), ce(), K(!0), n("show", t)
+                            !0 === T.platform.is.ios && (q = e.autoClose, A.value.click()), ce(), K(!0), n("show", t)
                         }), e.transitionDuration)
                     }
 
                     function re(t) {
                         B(), Y(), le(!0), null === E || void 0 !== t && !0 === t.qClickOutside || (((t && 0 === t.type.indexOf("key") ? E.closest('[tabindex]:not([tabindex^="-"])') : void 0) || E).focus(), E = null), V((() => {
                             Y(!0), n("hide", t)
                         }), e.transitionDuration)
                     }
 
                     function le(e) {
-                        C = void 0, void 0 !== q && (q(), q = void 0), !0 !== e && !0 !== R.value || ((0, w.H)(se), z(), (0, S.D)(W), (0, b.k)(ue)), !0 !== e && (E = null)
+                        C = void 0, void 0 !== F && (F(), F = void 0), !0 !== e && !0 !== R.value || ((0, w.H)(se), z(), (0, S.D)(W), (0, b.k)(ue)), !0 !== e && (E = null)
                     }
 
                     function ie() {
                         null === U.value && void 0 === e.scrollTarget || (N.value = (0, m.b0)(U.value, e.scrollTarget), H(N.value, ce))
                     }
 
                     function ae(e) {
-                        !0 !== F ? ((0, h.AH)(P, e), n("click", e)) : F = !1
+                        !0 !== q ? ((0, h.AH)(P, e), n("click", e)) : q = !1
                     }
 
                     function se(t) {
                         !0 === te.value && !0 !== e.noFocus && !0 !== (0, _.mY)(A.value, t.target) && ne()
                     }
 
                     function ue(e) {
@@ -7896,16 +7907,16 @@
 
                     function ce() {
                         const t = A.value;
                         null !== t && null !== U.value && (0, k.wq)({
                             el: t,
                             offset: e.offset,
                             anchorEl: U.value,
-                            anchorOrigin: X.value,
-                            selfOrigin: Q.value,
+                            anchorOrigin: Q.value,
+                            selfOrigin: X.value,
                             absoluteOffset: C,
                             fit: e.fit,
                             cover: e.cover,
                             maxHeight: e.maxHeight,
                             maxWidth: e.maxWidth
                         })
                     }
@@ -8118,16 +8129,16 @@
                         }
                     });
                     (0, o.YP)((() => `${v.value}|${h.value}`), (() => {
                         x.value = e.modelValue
                     }));
                     const k = (0, o.Fl)((() => "q-pagination row no-wrap items-center" + (!0 === e.disable ? " disabled" : ""))),
                         C = (0, o.Fl)((() => e.gutter in s.jA ? `${s.jA[e.gutter]}px` : e.gutter || null)),
-                        q = (0, o.Fl)((() => null !== C.value ? `--q-pagination-gutter-parent:-${C.value};--q-pagination-gutter-child:${C.value}` : null)),
-                        F = (0, o.Fl)((() => {
+                        F = (0, o.Fl)((() => null !== C.value ? `--q-pagination-gutter-parent:-${C.value};--q-pagination-gutter-child:${C.value}` : null)),
+                        q = (0, o.Fl)((() => {
                             const t = [e.iconFirst || u.iconSet.pagination.first, e.iconPrev || u.iconSet.pagination.prev, e.iconNext || u.iconSet.pagination.next, e.iconLast || u.iconSet.pagination.last];
                             return !0 === u.lang.rtl ? t.reverse() : t
                         })),
                         E = (0, o.Fl)((() => ({
                             "aria-disabled": !0 === e.disable ? "true" : "false",
                             role: "navigation"
                         }))),
@@ -8211,27 +8222,27 @@
                     }), () => {
                         const t = [],
                             n = [];
                         let r;
                         if (!0 === y.value && (t.push(B({
                                 key: "bls",
                                 disable: e.disable || e.modelValue <= v.value,
-                                icon: F.value[0]
+                                icon: q.value[0]
                             }, v.value)), n.unshift(B({
                                 key: "ble",
                                 disable: e.disable || e.modelValue >= h.value,
-                                icon: F.value[3]
+                                icon: q.value[3]
                             }, h.value))), !0 === w.value && (t.push(B({
                                 key: "bdp",
                                 disable: e.disable || e.modelValue <= v.value,
-                                icon: F.value[1]
+                                icon: q.value[1]
                             }, e.modelValue - 1)), n.unshift(B({
                                 key: "bdn",
                                 disable: e.disable || e.modelValue >= h.value,
-                                icon: F.value[2]
+                                icon: q.value[2]
                             }, e.modelValue + 1))), !0 !== e.input) {
                             r = [];
                             const {
                                 pgFrom: o,
                                 pgTo: l,
                                 marginalStyle: i
                             } = R.value;
@@ -8273,15 +8284,15 @@
                             }, t, t === e.modelValue))
                         }
                         return (0, o.h)("div", {
                             class: k.value,
                             ...E.value
                         }, [(0, o.h)("div", {
                             class: "q-pagination__content row no-wrap items-center",
-                            style: q.value
+                            style: F.value
                         }, [...t, !0 === e.input ? (0, o.h)(i.Z, {
                             class: "inline",
                             style: {
                                 width: g.value.length / 1.5 + "em"
                             },
                             type: "number",
                             dense: !0,
@@ -8401,15 +8412,15 @@
                         }
                     }
                 })
         },
         2762: (e, t, n) => {
             "use strict";
             n.d(t, {
-                Z: () => q
+                Z: () => F
             });
             n(9665);
             var o = n(9835),
                 r = n(499),
                 l = n(8149),
                 i = n(2857),
                 a = n(7691),
@@ -8451,15 +8462,15 @@
                 b = n(4680),
                 w = n(1384),
                 _ = n(321),
                 S = n(1705);
             const x = e => ["add", "add-unique", "toggle"].includes(e),
                 k = ".*+?^${}()|[]\\",
                 C = Object.keys(h.Cl),
-                q = (0, c.L)({
+                F = (0, c.L)({
                     name: "QSelect",
                     inheritAttrs: !1,
                     props: {
                         ...m.t9,
                         ...g.Fz,
                         ...h.Cl,
                         modelValue: {
@@ -8532,30 +8543,30 @@
                     setup(e, {
                         slots: t,
                         emit: n
                     }) {
                         const {
                             proxy: c
                         } = (0, o.FN)(), {
-                            $q: q
-                        } = c, F = (0, r.iH)(!1), E = (0, r.iH)(!1), O = (0, r.iH)(-1), P = (0, r.iH)(""), T = (0, r.iH)(!1), A = (0, r.iH)(!1);
+                            $q: F
+                        } = c, q = (0, r.iH)(!1), E = (0, r.iH)(!1), O = (0, r.iH)(-1), P = (0, r.iH)(""), T = (0, r.iH)(!1), A = (0, r.iH)(!1);
                         let R, L, $, j, B, V, M, I = null,
                             N = null;
                         const H = (0, r.iH)(null),
                             z = (0, r.iH)(null),
                             U = (0, r.iH)(null),
                             D = (0, r.iH)(null),
                             Z = (0, r.iH)(null),
                             K = (0, g.Do)(e),
                             Y = (0, y.Z)(Je),
                             J = (0, o.Fl)((() => Array.isArray(e.options) ? e.options.length : 0)),
                             W = (0, o.Fl)((() => void 0 === e.virtualScrollItemSize ? !0 === e.optionsDense ? 24 : 48 : e.virtualScrollItemSize)),
                             {
-                                virtualScrollSliceRange: X,
-                                virtualScrollSliceSizeComputed: Q,
+                                virtualScrollSliceRange: Q,
+                                virtualScrollSliceSizeComputed: X,
                                 localResetVirtualScroll: G,
                                 padVirtualScroll: ee,
                                 onVirtualScrollEvt: te,
                                 scrollTo: ne,
                                 setVirtualScrollSize: oe
                             } = (0, m.vp)({
                                 virtualScrollLength: J,
@@ -8597,15 +8608,15 @@
                             ge = (0, o.Fl)((() => {
                                 const t = {
                                     tabindex: e.tabindex,
                                     role: "combobox",
                                     "aria-label": e.label,
                                     "aria-readonly": !0 === e.readonly ? "true" : "false",
                                     "aria-autocomplete": !0 === e.useInput ? "list" : "none",
-                                    "aria-expanded": !0 === F.value ? "true" : "false",
+                                    "aria-expanded": !0 === q.value ? "true" : "false",
                                     "aria-controls": `${re.targetUid.value}_lb`
                                 };
                                 return O.value >= 0 && (t["aria-activedescendant"] = `${re.targetUid.value}_${O.value}`), t
                             })),
                             ye = (0, o.Fl)((() => ({
                                 id: `${re.targetUid.value}_lb`,
                                 role: "listbox",
@@ -8621,17 +8632,17 @@
                                 tabindex: me.value
                             }))))),
                             we = (0, o.Fl)((() => {
                                 if (0 === J.value) return [];
                                 const {
                                     from: t,
                                     to: n
-                                } = X.value;
+                                } = Q.value;
                                 return e.options.slice(t, n).map(((n, o) => {
-                                    const r = !0 === qe.value(n),
+                                    const r = !0 === Fe.value(n),
                                         l = t + o,
                                         i = {
                                             clickable: !0,
                                             active: !1,
                                             activeClass: xe.value,
                                             manualFocus: !0,
                                             focused: !1,
@@ -8641,36 +8652,36 @@
                                             dark: ae.value,
                                             role: "option",
                                             id: `${re.targetUid.value}_${l}`,
                                             onClick: () => {
                                                 Re(n)
                                             }
                                         };
-                                    return !0 !== r && (!0 === Ve(n) && (i.active = !0), O.value === l && (i.focused = !0), i["aria-selected"] = !0 === i.active ? "true" : "false", !0 === q.platform.is.desktop && (i.onMousemove = () => {
-                                        !0 === F.value && Le(l)
+                                    return !0 !== r && (!0 === Ve(n) && (i.active = !0), O.value === l && (i.focused = !0), i["aria-selected"] = !0 === i.active ? "true" : "false", !0 === F.platform.is.desktop && (i.onMousemove = () => {
+                                        !0 === q.value && Le(l)
                                     })), {
                                         index: l,
                                         opt: n,
                                         html: ve.value(n),
                                         label: Ce.value(n),
                                         selected: i.active,
                                         focused: i.focused,
                                         toggleOption: Re,
                                         setOptionIndex: Le,
                                         itemProps: i
                                     }
                                 }))
                             })),
-                            _e = (0, o.Fl)((() => void 0 !== e.dropdownIcon ? e.dropdownIcon : q.iconSet.arrow.dropdown)),
+                            _e = (0, o.Fl)((() => void 0 !== e.dropdownIcon ? e.dropdownIcon : F.iconSet.arrow.dropdown)),
                             Se = (0, o.Fl)((() => !1 === e.optionsCover && !0 !== e.outlined && !0 !== e.standout && !0 !== e.borderless && !0 !== e.rounded)),
                             xe = (0, o.Fl)((() => void 0 !== e.optionsSelectedClass ? e.optionsSelectedClass : void 0 !== e.color ? `text-${e.color}` : "")),
                             ke = (0, o.Fl)((() => Be(e.optionValue, "value"))),
                             Ce = (0, o.Fl)((() => Be(e.optionLabel, "label"))),
-                            qe = (0, o.Fl)((() => Be(e.optionDisable, "disable"))),
-                            Fe = (0, o.Fl)((() => le.value.map((e => ke.value(e))))),
+                            Fe = (0, o.Fl)((() => Be(e.optionDisable, "disable"))),
+                            qe = (0, o.Fl)((() => le.value.map((e => ke.value(e))))),
                             Ee = (0, o.Fl)((() => {
                                 const e = {
                                     onInput: Je,
                                     onChange: Y,
                                     onKeydown: ze,
                                     onKeyup: Ne,
                                     onKeypress: He,
@@ -8699,41 +8710,41 @@
 
                         function Te(e) {
                             Pe(e), re.focus()
                         }
 
                         function Ae(t, o) {
                             const r = Oe(t);
-                            if (!0 !== e.multiple) return !0 === e.fillInput && Xe(Ce.value(t), !0, !0), void n("update:modelValue", r);
+                            if (!0 !== e.multiple) return !0 === e.fillInput && Qe(Ce.value(t), !0, !0), void n("update:modelValue", r);
                             if (0 === le.value.length) return n("add", {
                                 index: 0,
                                 value: r
                             }), void n("update:modelValue", !0 === e.multiple ? [r] : r);
                             if (!0 === o && !0 === Ve(t)) return;
                             if (void 0 !== e.maxValues && e.modelValue.length >= e.maxValues) return;
                             const l = e.modelValue.slice();
                             n("add", {
                                 index: l.length,
                                 value: r
                             }), l.push(r), n("update:modelValue", l)
                         }
 
                         function Re(t, o) {
-                            if (!0 !== re.editable.value || void 0 === t || !0 === qe.value(t)) return;
+                            if (!0 !== re.editable.value || void 0 === t || !0 === Fe.value(t)) return;
                             const r = ke.value(t);
-                            if (!0 !== e.multiple) return !0 !== o && (Xe(!0 === e.fillInput ? Ce.value(t) : "", !0, !0), ct()), null !== z.value && z.value.focus(), void(0 !== le.value.length && !0 === (0, b.xb)(ke.value(le.value[0]), r) || n("update:modelValue", !0 === e.emitValue ? r : t));
+                            if (!0 !== e.multiple) return !0 !== o && (Qe(!0 === e.fillInput ? Ce.value(t) : "", !0, !0), ct()), null !== z.value && z.value.focus(), void(0 !== le.value.length && !0 === (0, b.xb)(ke.value(le.value[0]), r) || n("update:modelValue", !0 === e.emitValue ? r : t));
                             if ((!0 !== L || !0 === T.value) && re.focus(), Me(), 0 === le.value.length) {
                                 const o = !0 === e.emitValue ? r : t;
                                 return n("add", {
                                     index: 0,
                                     value: o
                                 }), void n("update:modelValue", !0 === e.multiple ? [o] : o)
                             }
                             const l = e.modelValue.slice(),
-                                i = Fe.value.findIndex((e => (0, b.xb)(e, r)));
+                                i = qe.value.findIndex((e => (0, b.xb)(e, r)));
                             if (i > -1) n("remove", {
                                 index: i,
                                 value: l.splice(i, 1)[0]
                             });
                             else {
                                 if (void 0 !== e.maxValues && l.length >= e.maxValues) return;
                                 const o = !0 === e.emitValue ? r : t;
@@ -8742,25 +8753,25 @@
                                     value: o
                                 }), l.push(o)
                             }
                             n("update:modelValue", l)
                         }
 
                         function Le(e) {
-                            if (!0 !== q.platform.is.desktop) return;
+                            if (!0 !== F.platform.is.desktop) return;
                             const t = e > -1 && e < J.value ? e : -1;
                             O.value !== t && (O.value = t)
                         }
 
                         function $e(t = 1, n) {
-                            if (!0 === F.value) {
+                            if (!0 === q.value) {
                                 let o = O.value;
                                 do {
                                     o = (0, _.Uz)(o + t, -1, J.value - 1)
-                                } while (-1 !== o && o !== O.value && !0 === qe.value(e.options[o]));
+                                } while (-1 !== o && o !== O.value && !0 === Fe.value(e.options[o]));
                                 O.value !== o && (Le(o), ne(o), !0 !== n && !0 === e.useInput && !0 === e.fillInput && We(o >= 0 ? Ce.value(e.options[o]) : j))
                             }
                         }
 
                         function je(t, n) {
                             const o = e => (0, b.xb)(ke.value(e), t);
                             return e.options.find(o) || n.find(o) || t
@@ -8769,38 +8780,38 @@
                         function Be(e, t) {
                             const n = void 0 !== e ? e : t;
                             return "function" === typeof n ? n : e => null !== e && "object" === typeof e && n in e ? e[n] : e
                         }
 
                         function Ve(e) {
                             const t = ke.value(e);
-                            return void 0 !== Fe.value.find((e => (0, b.xb)(e, t)))
+                            return void 0 !== qe.value.find((e => (0, b.xb)(e, t)))
                         }
 
                         function Me(t) {
                             !0 === e.useInput && null !== z.value && (void 0 === t || z.value === t.target && t.target.value === fe.value) && z.value.select()
                         }
 
                         function Ie(e) {
-                            !0 === (0, S.So)(e, 27) && !0 === F.value && ((0, w.sT)(e), ct(), dt()), n("keyup", e)
+                            !0 === (0, S.So)(e, 27) && !0 === q.value && ((0, w.sT)(e), ct(), dt()), n("keyup", e)
                         }
 
                         function Ne(t) {
                             const {
                                 value: n
                             } = t.target;
                             if (void 0 === t.keyCode)
                                 if (t.target.value = "", null !== I && (clearTimeout(I), I = null), dt(), "string" === typeof n && n.length > 0) {
                                     const t = n.toLocaleLowerCase(),
                                         o = n => {
                                             const o = e.options.find((e => n.value(e).toLocaleLowerCase() === t));
                                             return void 0 !== o && (-1 === le.value.indexOf(o) ? Re(o) : ct(), !0)
                                         },
                                         r = e => {
-                                            !0 !== o(ke) && !0 !== o(Ce) && !0 !== e && Qe(n, !0, (() => r(!0)))
+                                            !0 !== o(ke) && !0 !== o(Ce) && !0 !== e && Xe(n, !0, (() => r(!0)))
                                         };
                                     r()
                                 } else re.clearValue(t);
                             else Ie(t)
                         }
 
                         function He(e) {
@@ -8810,62 +8821,62 @@
                         function ze(t) {
                             if (n("keydown", t), !0 === (0, S.Wm)(t)) return;
                             const r = P.value.length > 0 && (void 0 !== e.newValueMode || void 0 !== e.onNewValue),
                                 l = !0 !== t.shiftKey && !0 !== e.multiple && (O.value > -1 || !0 === r);
                             if (27 === t.keyCode) return void(0, w.X$)(t);
                             if (9 === t.keyCode && !1 === l) return void st();
                             if (void 0 === t.target || t.target.id !== re.targetUid.value) return;
-                            if (40 === t.keyCode && !0 !== re.innerLoading.value && !1 === F.value) return (0, w.NS)(t), void ut();
+                            if (40 === t.keyCode && !0 !== re.innerLoading.value && !1 === q.value) return (0, w.NS)(t), void ut();
                             if (8 === t.keyCode && !0 !== e.hideSelected && 0 === P.value.length) return void(!0 === e.multiple && !0 === Array.isArray(e.modelValue) ? Pe(e.modelValue.length - 1) : !0 !== e.multiple && null !== e.modelValue && n("update:modelValue", null));
-                            35 !== t.keyCode && 36 !== t.keyCode || "string" === typeof P.value && 0 !== P.value.length || ((0, w.NS)(t), O.value = -1, $e(36 === t.keyCode ? 1 : -1, e.multiple)), 33 !== t.keyCode && 34 !== t.keyCode || void 0 === Q.value || ((0, w.NS)(t), O.value = Math.max(-1, Math.min(J.value, O.value + (33 === t.keyCode ? -1 : 1) * Q.value.view)), $e(33 === t.keyCode ? 1 : -1, e.multiple)), 38 !== t.keyCode && 40 !== t.keyCode || ((0, w.NS)(t), $e(38 === t.keyCode ? -1 : 1, e.multiple));
+                            35 !== t.keyCode && 36 !== t.keyCode || "string" === typeof P.value && 0 !== P.value.length || ((0, w.NS)(t), O.value = -1, $e(36 === t.keyCode ? 1 : -1, e.multiple)), 33 !== t.keyCode && 34 !== t.keyCode || void 0 === X.value || ((0, w.NS)(t), O.value = Math.max(-1, Math.min(J.value, O.value + (33 === t.keyCode ? -1 : 1) * X.value.view)), $e(33 === t.keyCode ? 1 : -1, e.multiple)), 38 !== t.keyCode && 40 !== t.keyCode || ((0, w.NS)(t), $e(38 === t.keyCode ? -1 : 1, e.multiple));
                             const i = J.value;
                             if ((void 0 === V || M < Date.now()) && (V = ""), i > 0 && !0 !== e.useInput && void 0 !== t.key && 1 === t.key.length && !1 === t.altKey && !1 === t.ctrlKey && !1 === t.metaKey && (32 !== t.keyCode || V.length > 0)) {
-                                !0 !== F.value && ut(t);
+                                !0 !== q.value && ut(t);
                                 const n = t.key.toLocaleLowerCase(),
                                     r = 1 === V.length && V[0] === n;
                                 M = Date.now() + 1500, !1 === r && ((0, w.NS)(t), V += n);
                                 const l = new RegExp("^" + V.split("").map((e => k.indexOf(e) > -1 ? "\\" + e : e)).join(".*"), "i");
                                 let a = O.value;
                                 if (!0 === r || a < 0 || !0 !== l.test(Ce.value(e.options[a])))
                                     do {
                                         a = (0, _.Uz)(a + 1, -1, i - 1)
-                                    } while (a !== O.value && (!0 === qe.value(e.options[a]) || !0 !== l.test(Ce.value(e.options[a]))));
+                                    } while (a !== O.value && (!0 === Fe.value(e.options[a]) || !0 !== l.test(Ce.value(e.options[a]))));
                                 O.value !== a && (0, o.Y3)((() => {
                                     Le(a), ne(a), a >= 0 && !0 === e.useInput && !0 === e.fillInput && We(Ce.value(e.options[a]))
                                 }))
                             } else if (13 === t.keyCode || 32 === t.keyCode && !0 !== e.useInput && "" === V || 9 === t.keyCode && !1 !== l)
                                 if (9 !== t.keyCode && (0, w.NS)(t), O.value > -1 && O.value < i) Re(e.options[O.value]);
                                 else {
                                     if (!0 === r) {
                                         const t = (t, n) => {
                                             if (n) {
                                                 if (!0 !== x(n)) return
                                             } else n = e.newValueMode;
                                             if (void 0 === t || null === t) return;
-                                            Xe("", !0 !== e.multiple, !0);
+                                            Qe("", !0 !== e.multiple, !0);
                                             const o = "toggle" === n ? Re : Ae;
                                             o(t, "add-unique" === n), !0 !== e.multiple && (null !== z.value && z.value.focus(), ct())
                                         };
                                         if (void 0 !== e.onNewValue ? n("newValue", P.value, t) : t(P.value), !0 !== e.multiple) return
-                                    }!0 === F.value ? st() : !0 !== re.innerLoading.value && ut()
+                                    }!0 === q.value ? st() : !0 !== re.innerLoading.value && ut()
                                 }
                         }
 
                         function Ue() {
                             return !0 === L ? Z.value : null !== U.value && null !== U.value.contentEl ? U.value.contentEl : void 0
                         }
 
                         function De() {
                             return Ue()
                         }
 
                         function Ze() {
                             return !0 === e.hideSelected ? [] : void 0 !== t["selected-item"] ? be.value.map((e => t["selected-item"](e))).slice() : void 0 !== t.selected ? [].concat(t.selected()) : !0 === e.useChips ? be.value.map(((t, n) => (0, o.h)(a.Z, {
                                 key: "option-" + n,
-                                removable: !0 === re.editable.value && !0 !== qe.value(t.opt),
+                                removable: !0 === re.editable.value && !0 !== Fe.value(t.opt),
                                 dense: !0,
                                 textColor: e.color,
                                 tabindex: me.value,
                                 onRemove() {
                                     t.removeAtIndex(n)
                                 }
                             }, (() => (0, o.h)("span", {
@@ -8912,51 +8923,51 @@
                                     ...Ee.value
                                 };
                             return !0 !== t && !0 === L && (!0 === Array.isArray(l.class) ? l.class = [...l.class, "no-pointer-events"] : l.class += " no-pointer-events"), (0, o.h)("input", l)
                         }
 
                         function Je(t) {
                             null !== I && (clearTimeout(I), I = null), t && t.target && !0 === t.target.qComposing || (We(t.target.value || ""), $ = !0, j = P.value, !0 === re.focused.value || !0 === L && !0 !== T.value || re.focus(), void 0 !== e.onFilter && (I = setTimeout((() => {
-                                I = null, Qe(P.value)
+                                I = null, Xe(P.value)
                             }), e.inputDebounce)))
                         }
 
                         function We(e) {
                             P.value !== e && (P.value = e, n("inputValue", e))
                         }
 
-                        function Xe(t, n, o) {
-                            $ = !0 !== o, !0 === e.useInput && (We(t), !0 !== n && !0 === o || (j = t), !0 !== n && Qe(t))
+                        function Qe(t, n, o) {
+                            $ = !0 !== o, !0 === e.useInput && (We(t), !0 !== n && !0 === o || (j = t), !0 !== n && Xe(t))
                         }
 
-                        function Qe(t, r, l) {
+                        function Xe(t, r, l) {
                             if (void 0 === e.onFilter || !0 !== r && !0 !== re.focused.value) return;
                             !0 === re.innerLoading.value ? n("filterAbort") : (re.innerLoading.value = !0, A.value = !0), "" !== t && !0 !== e.multiple && le.value.length > 0 && !0 !== $ && t === Ce.value(le.value[0]) && (t = "");
                             const i = setTimeout((() => {
-                                !0 === F.value && (F.value = !1)
+                                !0 === q.value && (q.value = !1)
                             }), 10);
                             null !== N && clearTimeout(N), N = i, n("filter", t, ((e, t) => {
                                 !0 !== r && !0 !== re.focused.value || N !== i || (clearTimeout(N), "function" === typeof e && e(), A.value = !1, (0, o.Y3)((() => {
-                                    re.innerLoading.value = !1, !0 === re.editable.value && (!0 === r ? !0 === F.value && ct() : !0 === F.value ? ft(!0) : F.value = !0), "function" === typeof t && (0, o.Y3)((() => {
+                                    re.innerLoading.value = !1, !0 === re.editable.value && (!0 === r ? !0 === q.value && ct() : !0 === q.value ? ft(!0) : q.value = !0), "function" === typeof t && (0, o.Y3)((() => {
                                         t(c)
                                     })), "function" === typeof l && (0, o.Y3)((() => {
                                         l(c)
                                     }))
                                 })))
                             }), (() => {
-                                !0 === re.focused.value && N === i && (clearTimeout(N), re.innerLoading.value = !1, A.value = !1), !0 === F.value && (F.value = !1)
+                                !0 === re.focused.value && N === i && (clearTimeout(N), re.innerLoading.value = !1, A.value = !1), !0 === q.value && (q.value = !1)
                             }))
                         }
 
                         function Ge() {
                             return (0, o.h)(p.Z, {
                                 ref: U,
                                 class: ce.value,
                                 style: e.popupContentStyle,
-                                modelValue: F.value,
+                                modelValue: q.value,
                                 fit: !0 !== e.menuShrink,
                                 cover: !0 === e.optionsCover && !0 !== de.value && !0 !== e.useInput,
                                 anchor: e.menuAnchor,
                                 self: e.menuSelf,
                                 offset: e.menuOffset,
                                 dark: ae.value,
                                 noParentEvent: !0,
@@ -9009,15 +9020,15 @@
                                 onBlur: ot
                             }, {
                                 ...t,
                                 rawControl: () => re.getControl(!0),
                                 before: void 0,
                                 after: void 0
                             })];
-                            return !0 === F.value && n.push((0, o.h)("div", {
+                            return !0 === q.value && n.push((0, o.h)("div", {
                                 ref: Z,
                                 class: ce.value + " scroll",
                                 style: e.popupContentStyle,
                                 ...ye.value,
                                 onClick: w.X$,
                                 onScrollPassive: te
                             }, Ke())), (0, o.h)(v.Z, {
@@ -9046,29 +9057,29 @@
 
                         function at() {
                             const e = document.activeElement;
                             null !== e && e.id === re.targetUid.value || null === z.value || z.value === e || z.value.focus(), oe()
                         }
 
                         function st() {
-                            !0 !== E.value && (O.value = -1, !0 === F.value && (F.value = !1), !1 === re.focused.value && (null !== N && (clearTimeout(N), N = null), !0 === re.innerLoading.value && (n("filterAbort"), re.innerLoading.value = !1, A.value = !1)))
+                            !0 !== E.value && (O.value = -1, !0 === q.value && (q.value = !1), !1 === re.focused.value && (null !== N && (clearTimeout(N), N = null), !0 === re.innerLoading.value && (n("filterAbort"), re.innerLoading.value = !1, A.value = !1)))
                         }
 
                         function ut(n) {
                             !0 === re.editable.value && (!0 === L ? (re.onControlFocusin(n), E.value = !0, (0, o.Y3)((() => {
                                 re.focus()
-                            }))) : re.focus(), void 0 !== e.onFilter ? Qe(P.value) : !0 === de.value && void 0 === t["no-option"] || (F.value = !0))
+                            }))) : re.focus(), void 0 !== e.onFilter ? Xe(P.value) : !0 === de.value && void 0 === t["no-option"] || (q.value = !0))
                         }
 
                         function ct() {
                             E.value = !1, st()
                         }
 
                         function dt() {
-                            !0 === e.useInput && Xe(!0 !== e.multiple && !0 === e.fillInput && le.value.length > 0 && Ce.value(le.value[0]) || "", !0, !0)
+                            !0 === e.useInput && Qe(!0 !== e.multiple && !0 === e.fillInput && le.value.length > 0 && Ce.value(le.value[0]) || "", !0, !0)
                         }
 
                         function ft(t) {
                             let n = -1;
                             if (!0 === t) {
                                 if (le.value.length > 0) {
                                     const t = ke.value(le.value[0]);
@@ -9076,16 +9087,16 @@
                                 }
                                 G(n)
                             }
                             Le(n)
                         }
 
                         function pt(e, t) {
-                            !0 === F.value && !1 === re.innerLoading.value && (G(-1, !0), (0, o.Y3)((() => {
-                                !0 === F.value && !1 === re.innerLoading.value && (e > t ? G() : ft(!0))
+                            !0 === q.value && !1 === re.innerLoading.value && (G(-1, !0), (0, o.Y3)((() => {
+                                !0 === q.value && !1 === re.innerLoading.value && (e > t ? G() : ft(!0))
                             })))
                         }
 
                         function vt() {
                             !1 === E.value && null !== U.value && U.value.updatePosition()
                         }
 
@@ -9094,37 +9105,37 @@
                         }
 
                         function mt(e) {
                             void 0 !== e && (0, w.sT)(e), n("popupHide", e), re.hasPopupOpen = !1, re.onControlFocusout(e)
                         }
 
                         function gt() {
-                            L = (!0 === q.platform.is.mobile || "dialog" === e.behavior) && ("menu" !== e.behavior && (!0 !== e.useInput || (void 0 !== t["no-option"] || void 0 !== e.onFilter || !1 === de.value))), B = !0 === q.platform.is.ios && !0 === L && !0 === e.useInput ? "fade" : e.transitionShow
+                            L = (!0 === F.platform.is.mobile || "dialog" === e.behavior) && ("menu" !== e.behavior && (!0 !== e.useInput || (void 0 !== t["no-option"] || void 0 !== e.onFilter || !1 === de.value))), B = !0 === F.platform.is.ios && !0 === L && !0 === e.useInput ? "fade" : e.transitionShow
                         }
                         return (0, o.YP)(le, (t => {
-                            R = t, !0 === e.useInput && !0 === e.fillInput && !0 !== e.multiple && !0 !== re.innerLoading.value && (!0 !== E.value && !0 !== F.value || !0 !== se.value) && (!0 !== $ && dt(), !0 !== E.value && !0 !== F.value || Qe(""))
+                            R = t, !0 === e.useInput && !0 === e.fillInput && !0 !== e.multiple && !0 !== re.innerLoading.value && (!0 !== E.value && !0 !== q.value || !0 !== se.value) && (!0 !== $ && dt(), !0 !== E.value && !0 !== q.value || Xe(""))
                         }), {
                             immediate: !0
-                        }), (0, o.YP)((() => e.fillInput), dt), (0, o.YP)(F, ft), (0, o.YP)(J, pt), (0, o.Xn)(gt), (0, o.ic)(vt), gt(), (0, o.Jd)((() => {
+                        }), (0, o.YP)((() => e.fillInput), dt), (0, o.YP)(q, ft), (0, o.YP)(J, pt), (0, o.Xn)(gt), (0, o.ic)(vt), gt(), (0, o.Jd)((() => {
                             null !== I && clearTimeout(I)
                         })), Object.assign(c, {
                             showPopup: ut,
                             hidePopup: ct,
                             removeAtIndex: Pe,
                             add: Ae,
                             toggleOption: Re,
                             getOptionIndex: () => O.value,
                             setOptionIndex: Le,
                             moveOptionSelection: $e,
-                            filter: Qe,
+                            filter: Xe,
                             updateMenuPosition: vt,
-                            updateInputValue: Xe,
+                            updateInputValue: Qe,
                             isOptionSelected: Ve,
                             getEmittingOptionValue: Oe,
-                            isOptionDisabled: (...e) => !0 === qe.value.apply(null, e),
+                            isOptionDisabled: (...e) => !0 === Fe.value.apply(null, e),
                             getOptionValue: (...e) => ke.value.apply(null, e),
                             getOptionLabel: (...e) => Ce.value.apply(null, e)
                         }), Object.assign(re, {
                             innerValue: le,
                             fieldClass: (0, o.Fl)((() => `q-select q-field--auto-height q-select--with${!0!==e.useInput?"out":""}-input q-select--with${!0!==e.useChips?"out":""}-chips q-select--` + (!0 === e.multiple ? "multiple" : "single"))),
                             inputRef: H,
                             targetRef: z,
@@ -9141,15 +9152,15 @@
                                 },
                                 onFocusout(e) {
                                     re.onControlFocusout(e, (() => {
                                         dt(), st()
                                     }))
                                 },
                                 onClick(e) {
-                                    if ((0, w.X$)(e), !0 !== L && !0 === F.value) return st(), void(null !== z.value && z.value.focus());
+                                    if ((0, w.X$)(e), !0 !== L && !0 === q.value) return st(), void(null !== z.value && z.value.focus());
                                     ut(e)
                                 }
                             },
                             getControl: t => {
                                 const n = Ze(),
                                     r = !0 === t || !0 !== E.value || !0 !== L;
                                 if (!0 === e.useInput) n.push(Ye(t, r));
@@ -9170,16 +9181,16 @@
                                     })), !0 === r && "string" === typeof e.autocomplete && e.autocomplete.length > 0 && n.push((0, o.h)("input", {
                                         class: "q-select__autocomplete-input",
                                         autocomplete: e.autocomplete,
                                         tabindex: -1,
                                         onKeyup: Ne
                                     }))
                                 }
-                                if (void 0 !== K.value && !0 !== e.disable && Fe.value.length > 0) {
-                                    const t = Fe.value.map((e => (0, o.h)("option", {
+                                if (void 0 !== K.value && !0 !== e.disable && qe.value.length > 0) {
+                                    const t = qe.value.map((e => (0, o.h)("option", {
                                         value: e,
                                         selected: !0
                                     })));
                                     n.push((0, o.h)("select", {
                                         class: "hidden",
                                         name: K.value,
                                         multiple: e.multiple
@@ -9189,15 +9200,15 @@
                                 return (0, o.h)("div", {
                                     class: "q-field__native row items-center",
                                     ...l,
                                     ...re.splitAttrs.listeners.value
                                 }, n)
                             },
                             getInnerAppend: () => !0 !== e.loading && !0 !== A.value && !0 !== e.hideDropdownIcon ? [(0, o.h)(i.Z, {
-                                class: "q-select__dropdown-icon" + (!0 === F.value ? " rotate-180" : ""),
+                                class: "q-select__dropdown-icon" + (!0 === q.value ? " rotate-180" : ""),
                                 name: _e.value
                             })] : null
                         }), (0, h.ZP)(re)
                     }
                 })
         },
         926: (e, t, n) => {
@@ -9594,16 +9605,16 @@
                             "aria-valuemin": 0,
                             "aria-valuemax": 1,
                             "aria-valuenow": !0 === e.indeterminate ? void 0 : e.value
                         }, (0, a.vs)(t.default, n))
                     }
                 }
             });
-            var q = n(1006),
-                F = n(8879),
+            var F = n(1221),
+                q = n(8879),
                 E = n(5310),
                 O = n(2046);
             let P = 0;
             const T = {
                     fullscreen: Boolean,
                     noRouteFullscreenExit: Boolean
                 },
@@ -9948,15 +9959,15 @@
                 return Array.isArray(e) ? e.slice() : []
             }
             const J = {
                     expanded: Array
                 },
                 W = ["update:expanded"];
 
-            function X(e, t) {
+            function Q(e, t) {
                 const n = (0, r.iH)(Y(e.expanded));
 
                 function l(e) {
                     return n.value.includes(e)
                 }
 
                 function i(o) {
@@ -9972,15 +9983,15 @@
                     n.value = Y(e)
                 })), {
                     isRowExpanded: l,
                     setExpanded: i,
                     updateExpanded: a
                 }
             }
-            const Q = {
+            const X = {
                 visibleColumns: Array
             };
 
             function G(e, t, n) {
                 const r = (0, o.Fl)((() => {
                         if (void 0 !== e.columns) return e.columns;
                         const t = e.rows[0];
@@ -10090,15 +10101,15 @@
                     hideNoData: Boolean,
                     hidePagination: Boolean,
                     onRowClick: Function,
                     onRowDblclick: Function,
                     onRowContextmenu: Function,
                     ...d.S,
                     ...T,
-                    ...Q,
+                    ...X,
                     ...V,
                     ...H,
                     ...J,
                     ...D,
                     ...j
                 },
                 emits: ["request", "virtualScroll", ...A, ...W, ...Z],
@@ -10135,15 +10146,15 @@
                         setPagination: A
                     } = z(i, je), {
                         computedFilterMethod: L
                     } = M(e, A), {
                         isRowExpanded: $,
                         setExpanded: j,
                         updateExpanded: V
-                    } = X(e, n), I = (0, o.Fl)((() => {
+                    } = Q(e, n), I = (0, o.Fl)((() => {
                         let t = e.rows;
                         if (!0 === P.value || 0 === t.length) return t;
                         const {
                             sortBy: n,
                             descending: o
                         } = O.value;
                         return e.filter && (t = L.value(t, e.filter, ie.value, je)), null !== ue.value && (t = ce.value(e.rows === t ? t.slice() : t, n, o)), t
@@ -10156,15 +10167,15 @@
                         return 0 !== n && (0 === fe.value && e.rows !== t ? t.length > pe.value && (t = t.slice(0, pe.value)) : t = t.slice(fe.value, pe.value)), t
                     })), {
                         hasSelectionMode: D,
                         singleSelection: Z,
                         multipleSelection: Y,
                         allRowsSelected: J,
                         someRowsSelected: W,
-                        rowsSelectedNumber: Q,
+                        rowsSelectedNumber: X,
                         isRowSelected: ne,
                         clearSelection: oe,
                         updateSelection: re
                     } = K(e, n, H, m), {
                         colList: le,
                         computedCols: ie,
                         computedColsMap: ae,
@@ -10192,15 +10203,15 @@
                         })), void 0 === t.virtualScrollItemSize && (t.virtualScrollItemSize = !0 === e.dense ? 28 : 48), t
                     }));
 
                     function Ce() {
                         !0 === b.value && y.value.reset()
                     }
 
-                    function qe() {
+                    function Fe() {
                         if (!0 === e.grid) return Je();
                         const n = !0 !== e.hideHeader ? Ie : null;
                         if (!0 === b.value) {
                             const r = t["top-row"],
                                 l = t["bottom-row"],
                                 i = {
                                     default: e => Pe(e.item, t.body, e.index)
@@ -10228,15 +10239,15 @@
                         const r = [Te()];
                         return null !== n && r.unshift(n()), v({
                             class: ["q-table__middle scroll", e.tableClass],
                             style: e.tableStyle
                         }, r)
                     }
 
-                    function Fe(t, o) {
+                    function qe(t, o) {
                         if (null !== y.value) return void y.value.scrollTo(t, o);
                         t = parseInt(t, 10);
                         const r = g.value.querySelector(`tbody tr:nth-of-type(${t+1})`);
                         if (null !== r) {
                             const o = g.value.querySelector(".q-table__middle.scroll"),
                                 l = r.offsetTop - e.virtualScrollStickySizeStart,
                                 i = l < o.scrollTop ? "decrease" : "increase";
@@ -10288,15 +10299,15 @@
                             }));
                         if (!0 === D.value) {
                             const n = t["body-selection"],
                                 l = void 0 !== n ? n(Le({
                                     key: a,
                                     row: r,
                                     pageIndex: i
-                                })) : [(0, o.h)(q.Z, {
+                                })) : [(0, o.h)(F.Z, {
                                     modelValue: s,
                                     color: e.color,
                                     dark: c.value,
                                     dense: e.dense,
                                     "onUpdate:modelValue": (e, t) => {
                                         re([a], [r], e, t)
                                     }
@@ -10380,15 +10391,15 @@
                     })));
 
                     function Ve() {
                         const n = t.top,
                             r = t["top-left"],
                             l = t["top-right"],
                             i = t["top-selection"],
-                            a = !0 === D.value && void 0 !== i && Q.value > 0,
+                            a = !0 === D.value && void 0 !== i && X.value > 0,
                             s = "q-table__top relative-position row items-center";
                         if (void 0 !== n) return (0, o.h)("div", {
                             class: s
                         }, [n(Be.value)]);
                         let u;
                         return !0 === a ? u = i(Be.value).slice() : (u = [], void 0 !== r ? u.push((0, o.h)("div", {
                             class: "q-table__control"
@@ -10434,15 +10445,15 @@
                             }, (() => e.label))
                         }));
                         if (!0 === Z.value && !0 !== e.grid) l.unshift((0, o.h)("th", {
                             class: "q-table--col-auto-width"
                         }, " "));
                         else if (!0 === Y.value) {
                             const n = t["header-selection"],
-                                r = void 0 !== n ? n(He({})) : [(0, o.h)(q.Z, {
+                                r = void 0 !== n ? n(He({})) : [(0, o.h)(F.Z, {
                                     color: e.color,
                                     modelValue: Me.value,
                                     dark: c.value,
                                     dense: e.dense,
                                     "onUpdate:modelValue": ze
                                 })];
                             l.unshift((0, o.h)("th", {
@@ -10492,17 +10503,17 @@
                                 class: te + " q-table__bottom--nodata"
                             }, i)
                         }
                         const n = t.bottom;
                         if (void 0 !== n) return (0, o.h)("div", {
                             class: te
                         }, [n(Be.value)]);
-                        const r = !0 !== e.hideSelectedBanner && !0 === D.value && Q.value > 0 ? [(0, o.h)("div", {
+                        const r = !0 !== e.hideSelectedBanner && !0 === D.value && X.value > 0 ? [(0, o.h)("div", {
                             class: "q-table__control"
-                        }, [(0, o.h)("div", [(e.selectedRowsLabel || a.lang.table.selectedRecords)(Q.value)])])] : [];
+                        }, [(0, o.h)("div", [(e.selectedRowsLabel || a.lang.table.selectedRecords)(X.value)])])] : [];
                         return !0 !== e.hidePagination ? (0, o.h)("div", {
                             class: te + " justify-end"
                         }, Ke(r)) : r.length > 0 ? (0, o.h)("div", {
                             class: te
                         }, r) : void 0
                     }
 
@@ -10542,33 +10553,33 @@
                             } : {}, [l ? i(fe.value + 1, Math.min(pe.value, ye.value), ye.value) : i(1, N.value, ye.value)])], 0 !== l && me.value > 1) {
                             const t = {
                                 color: e.color,
                                 round: !0,
                                 dense: !0,
                                 flat: !0
                             };
-                            !0 === e.dense && (t.size = "sm"), me.value > 2 && r.push((0, o.h)(F.Z, {
+                            !0 === e.dense && (t.size = "sm"), me.value > 2 && r.push((0, o.h)(q.Z, {
                                 key: "pgFirst",
                                 ...t,
                                 icon: Ue.value[0],
                                 disable: ve.value,
                                 onClick: be
-                            })), r.push((0, o.h)(F.Z, {
+                            })), r.push((0, o.h)(q.Z, {
                                 key: "pgPrev",
                                 ...t,
                                 icon: Ue.value[1],
                                 disable: ve.value,
                                 onClick: we
-                            }), (0, o.h)(F.Z, {
+                            }), (0, o.h)(q.Z, {
                                 key: "pgNext",
                                 ...t,
                                 icon: Ue.value[2],
                                 disable: he.value,
                                 onClick: _e
-                            })), me.value > 2 && r.push((0, o.h)(F.Z, {
+                            })), me.value > 2 && r.push((0, o.h)(q.Z, {
                                 key: "pgLast",
                                 ...t,
                                 icon: Ue.value[3],
                                 disable: he.value,
                                 onClick: Se
                             }))
                         }
@@ -10593,15 +10604,15 @@
                             }, [(0, o.h)("div", {
                                 class: "q-table__grid-item-title"
                             }, [e.label]), (0, o.h)("div", {
                                 class: "q-table__grid-item-value"
                             }, [e.value])])));
                             if (!0 === D.value) {
                                 const n = t["body-selection"],
-                                    i = void 0 !== n ? n(r) : [(0, o.h)(q.Z, {
+                                    i = void 0 !== n ? n(r) : [(0, o.h)(F.Z, {
                                         modelValue: r.selected,
                                         color: e.color,
                                         dark: c.value,
                                         dense: e.dense,
                                         "onUpdate:modelValue": (e, t) => {
                                             re([r.key], [r.row], e, t)
                                         }
@@ -10642,30 +10653,30 @@
                         lastPage: Se,
                         isRowSelected: ne,
                         clearSelection: oe,
                         isRowExpanded: $,
                         setExpanded: j,
                         sort: de,
                         resetVirtualScroll: Ce,
-                        scrollTo: Fe,
+                        scrollTo: qe,
                         getCellValue: je
                     }), (0, ee.K)(i.proxy, {
                         filteredSortedRows: () => I.value,
                         computedRows: () => H.value,
                         computedRowsNumber: () => ye.value
                     }), () => {
                         const n = [Ve()],
                             r = {
                                 ref: g,
                                 class: k.value
                             };
                         return !0 === e.grid ? n.push(Ye()) : Object.assign(r, {
                             class: [r.class, e.cardClass],
                             style: e.cardStyle
-                        }), n.push(qe(), De()), !0 === e.loading && void 0 !== t.loading && n.push(t.loading()), (0, o.h)("div", r, n)
+                        }), n.push(Fe(), De()), !0 === e.loading && void 0 !== t.loading && n.push(t.loading()), (0, o.h)("div", r, n)
                     }
                 }
             })
         },
         7220: (e, t, n) => {
             "use strict";
             n.d(t, {
@@ -10700,14 +10711,48 @@
                             class: r.value + a.__tdClass(s),
                             style: a.__tdStyle(s)
                         }, (0, l.KR)(t.default))
                     }
                 }
             })
         },
+        3175: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                Z: () => a
+            });
+            var o = n(9835),
+                r = n(2857),
+                l = n(5413),
+                i = n(5987);
+            const a = (0, i.L)({
+                name: "QToggle",
+                props: {
+                    ...l.Fz,
+                    icon: String,
+                    iconColor: String
+                },
+                emits: l.ZB,
+                setup(e) {
+                    function t(t, n) {
+                        const l = (0, o.Fl)((() => (!0 === t.value ? e.checkedIcon : !0 === n.value ? e.indeterminateIcon : e.uncheckedIcon) || e.icon)),
+                            i = (0, o.Fl)((() => !0 === t.value ? e.iconColor : null));
+                        return () => [(0, o.h)("div", {
+                            class: "q-toggle__track"
+                        }), (0, o.h)("div", {
+                            class: "q-toggle__thumb absolute flex flex-center no-wrap"
+                        }, void 0 !== l.value ? [(0, o.h)(r.Z, {
+                            name: l.value,
+                            color: i.value
+                        })] : void 0)]
+                    }
+                    return (0, l.ZP)("toggle", t)
+                }
+            })
+        },
         1663: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => i
             });
             var o = n(9835),
                 r = n(5987),
@@ -10832,16 +10877,16 @@
                         {
                             proxy: {
                                 $q: x
                             }
                         } = S,
                         k = (0, r.iH)(null),
                         C = (0, r.iH)(!1),
-                        q = (0, o.Fl)((() => (0, b.li)(e.anchor, x.lang.rtl))),
-                        F = (0, o.Fl)((() => (0, b.li)(e.self, x.lang.rtl))),
+                        F = (0, o.Fl)((() => (0, b.li)(e.anchor, x.lang.rtl))),
+                        q = (0, o.Fl)((() => (0, b.li)(e.self, x.lang.rtl))),
                         E = (0, o.Fl)((() => !0 !== e.persistent)),
                         {
                             registerTick: O,
                             removeTick: P
                         } = (0, d.Z)(),
                         {
                             registerTimeout: T
@@ -10850,22 +10895,22 @@
                             transitionProps: A,
                             transitionStyle: R
                         } = (0, c.Z)(e),
                         {
                             localScrollTarget: L,
                             changeScrollEvent: $,
                             unconfigureScrollTarget: j
-                        } = (0, a.Z)(e, Q),
+                        } = (0, a.Z)(e, X),
                         {
                             anchorEl: B,
                             canShow: V,
                             anchorEvents: M
                         } = (0, i.Z)({
                             showing: C,
-                            configureAnchorEl: X
+                            configureAnchorEl: Q
                         }),
                         {
                             show: I,
                             hide: N
                         } = (0, s.ZP)({
                             showing: C,
                             canShow: V,
@@ -10903,15 +10948,15 @@
                     function D(t) {
                         H(), O((() => {
                             _ = new MutationObserver((() => Y())), _.observe(k.value, {
                                 attributes: !1,
                                 childList: !0,
                                 characterData: !0,
                                 subtree: !0
-                            }), Y(), Q()
+                            }), Y(), X()
                         })), void 0 === w && (w = (0, o.YP)((() => x.screen.width + "|" + x.screen.height + "|" + e.self + "|" + e.anchor + "|" + x.lang.rtl), Y)), T((() => {
                             H(!0), n("show", t)
                         }), e.transitionDuration)
                     }
 
                     function Z(t) {
                         P(), z(), K(), T((() => {
@@ -10925,16 +10970,16 @@
 
                     function Y() {
                         const t = k.value;
                         null !== B.value && t && (0, b.wq)({
                             el: t,
                             offset: e.offset,
                             anchorEl: B.value,
-                            anchorOrigin: q.value,
-                            selfOrigin: F.value,
+                            anchorOrigin: F.value,
+                            selfOrigin: q.value,
                             maxHeight: e.maxHeight,
                             maxWidth: e.maxWidth
                         })
                     }
 
                     function J(t) {
                         if (!0 === x.platform.is.mobile) {
@@ -10952,26 +10997,26 @@
                         !0 === x.platform.is.mobile && ((0, h.ul)(M, "tooltipTemp"), (0, m.M)(), setTimeout((() => {
                             document.body.classList.remove("non-selectable")
                         }), 10)), T((() => {
                             N(t)
                         }), e.hideDelay)
                     }
 
-                    function X() {
+                    function Q() {
                         if (!0 === e.noParentEvent || null === B.value) return;
                         const t = !0 === x.platform.is.mobile ? [
                             [B.value, "touchstart", "delayShow", "passive"]
                         ] : [
                             [B.value, "mouseenter", "delayShow", "passive"],
                             [B.value, "mouseleave", "delayHide", "passive"]
                         ];
                         (0, h.M0)(M, "anchor", t)
                     }
 
-                    function Q() {
+                    function X() {
                         if (null !== B.value || void 0 !== e.scrollTarget) {
                             L.value = (0, v.b0)(B.value, e.scrollTarget);
                             const t = !0 === e.noParentEvent ? Y : N;
                             $(L.value, t)
                         }
                     }
 
@@ -11000,15 +11045,15 @@
                 Z: () => m
             });
             n(9665);
             var o = n(9835),
                 r = n(499),
                 l = n(1957),
                 i = n(2857),
-                a = n(1006),
+                a = n(1221),
                 s = n(5987);
             const u = (0, s.L)({
                 name: "QSlideTransition",
                 props: {
                     appear: Boolean,
                     duration: {
                         type: Number,
@@ -11129,19 +11174,19 @@
                             w = {}
                         }));
                         const _ = (0, o.Fl)((() => "q-tree q-tree--" + (!0 === e.dense ? "dense" : "standard") + (!0 === e.noConnectors ? " q-tree--no-connectors" : "") + (!0 === m.value ? " q-tree--dark" : "") + (void 0 !== e.color ? ` text-${e.color}` : ""))),
                             S = (0, o.Fl)((() => void 0 !== e.selected)),
                             x = (0, o.Fl)((() => e.icon || h.iconSet.tree.icon)),
                             k = (0, o.Fl)((() => e.controlColor || e.color)),
                             C = (0, o.Fl)((() => void 0 !== e.textColor ? ` text-${e.textColor}` : "")),
-                            q = (0, o.Fl)((() => {
+                            F = (0, o.Fl)((() => {
                                 const t = e.selectedColor || e.color;
                                 return t ? ` text-${t}` : ""
                             })),
-                            F = (0, o.Fl)((() => void 0 !== e.filterMethod ? e.filterMethod : (t, n) => {
+                            q = (0, o.Fl)((() => void 0 !== e.filterMethod ? e.filterMethod : (t, n) => {
                                 const o = n.toLowerCase();
                                 return t[e.labelKey] && t[e.labelKey].toLowerCase().indexOf(o) > -1
                             })),
                             E = (0, o.Fl)((() => {
                                 const t = {},
                                     n = (o, r) => {
                                         const l = o.tickStrategy || (r ? r.tickStrategy : e.tickStrategy),
@@ -11161,15 +11206,15 @@
                                             key: i,
                                             parent: r,
                                             isParent: a,
                                             lazy: h,
                                             disabled: o.disabled,
                                             link: !0 !== o.disabled && (!0 === s || !0 === u && (!0 === a || !0 === h)),
                                             children: [],
-                                            matchesFilter: !e.filter || F.value(o, e.filter),
+                                            matchesFilter: !e.filter || q.value(o, e.filter),
                                             selected: i === e.selected && !0 === s,
                                             selectable: s,
                                             expanded: !0 === a && b.value.includes(i),
                                             expandable: u,
                                             noTick: !0 === o.noTick || !0 !== d && h && "loaded" !== h,
                                             tickable: v,
                                             tickStrategy: l,
@@ -11355,15 +11400,15 @@
                                 keepColor: !0,
                                 disable: !0 !== s.tickable,
                                 onKeydown: f.NS,
                                 "onUpdate:modelValue": e => {
                                     Y(s, e)
                                 }
                             }) : null, (0, o.h)("div", {
-                                class: "q-tree__node-header-content col row no-wrap items-center" + (!0 === s.selected ? q.value : C.value)
+                                class: "q-tree__node-header-content col row no-wrap items-center" + (!0 === s.selected ? F.value : C.value)
                             }, [d ? d(y) : [N(n), (0, o.h)("div", n[e.labelKey])]])]), !0 === h ? !0 === e.noTransition ? (0, o.h)("div", {
                                 class: "q-tree__node-collapsible" + C.value,
                                 key: `${r}__q`
                             }, [g, (0, o.h)("div", {
                                 class: "q-tree__children" + (!0 === s.disabled ? " q-tree__node--disabled" : "")
                             }, s.expanded ? v : null)]) : (0, o.h)(u, {
                                 duration: e.duration,
@@ -11551,16 +11596,16 @@
                         proxy: y
                     } = a,
                     {
                         $q: b
                     } = y;
                 let w, _, S, x, k = [];
                 const C = (0, r.iH)(0),
-                    q = (0, r.iH)(0),
-                    F = (0, r.iH)({}),
+                    F = (0, r.iH)(0),
+                    q = (0, r.iH)({}),
                     E = (0, r.iH)(null),
                     O = (0, r.iH)(null),
                     P = (0, r.iH)(null),
                     T = (0, r.iH)({
                         from: 0,
                         to: 0
                     }),
@@ -11585,15 +11630,15 @@
                 }
 
                 function V() {
                     const o = t();
                     if (void 0 === o || null === o || 8 === o.nodeType) return;
                     const r = p(o, n(), E.value, O.value, m.virtualScrollHorizontal, b.lang.rtl, m.virtualScrollStickySizeStart, m.virtualScrollStickySizeEnd),
                         l = e.value - 1,
-                        i = r.scrollMaxSize - r.offsetStart - r.offsetEnd - q.value;
+                        i = r.scrollMaxSize - r.offsetStart - r.offsetEnd - F.value;
                     if (w === r.scrollStart) return;
                     if (r.scrollMaxSize <= 0) return void M(o, r, 0, 0);
                     S !== r.scrollViewSize && z(r.scrollViewSize), I(T.value.from);
                     const a = Math.floor(r.scrollMaxSize - Math.max(r.scrollViewSize, r.offsetEnd) - Math.min(x[l], r.scrollViewSize / 2));
                     if (a > 0 && Math.ceil(r.scrollStart) >= a) return void M(o, r, l, r.scrollMaxSize - r.offsetEnd - k.reduce(f, 0));
                     let u = 0,
                         c = r.scrollStart - r.offsetStart,
@@ -11605,36 +11650,36 @@
                     M(o, r, u, d)
                 }
 
                 function M(t, n, o, r, l) {
                     const i = "string" === typeof l && l.indexOf("-force") > -1,
                         a = !0 === i ? l.replace("-force", "") : l,
                         s = void 0 !== a ? a : "start";
-                    let u = Math.max(0, o - F.value[s]),
-                        c = u + F.value.total;
-                    c > e.value && (c = e.value, u = Math.max(0, c - F.value.total)), w = n.scrollStart;
+                    let u = Math.max(0, o - q.value[s]),
+                        c = u + q.value.total;
+                    c > e.value && (c = e.value, u = Math.max(0, c - q.value.total)), w = n.scrollStart;
                     const p = u !== T.value.from || c !== T.value.to;
                     if (!1 === p && void 0 === a) return void D(o);
                     const {
                         activeElement: g
                     } = document, y = P.value;
                     !0 === p && null !== y && y !== g && !0 === y.contains(g) && (y.addEventListener("focusout", N), setTimeout((() => {
                         null !== y && y.removeEventListener("focusout", N)
                     }))), d(y, o - u);
                     const _ = void 0 !== a ? x.slice(u, o).reduce(f, 0) : 0;
                     if (!0 === p) {
                         const t = c >= T.value.from && u <= T.value.to ? T.value.to : c;
                         T.value = {
                             from: u,
                             to: t
-                        }, C.value = h(k, x, 0, u), q.value = h(k, x, c, e.value), requestAnimationFrame((() => {
+                        }, C.value = h(k, x, 0, u), F.value = h(k, x, c, e.value), requestAnimationFrame((() => {
                             T.value.to !== c && w === n.scrollStart && (T.value = {
                                 from: T.value.from,
                                 to: c
-                            }, q.value = h(k, x, c, e.value))
+                            }, F.value = h(k, x, c, e.value))
                         }))
                     }
                     requestAnimationFrame((() => {
                         if (w !== n.scrollStart) return;
                         !0 === p && I(u);
                         const e = x.slice(u, o).reduce(f, 0),
                             l = e + n.offsetStart + C.value,
@@ -11678,15 +11723,15 @@
                     k = [];
                     for (let o = 0; o <= a; o++) {
                         let t = 0;
                         const n = Math.min((o + 1) * s, e.value);
                         for (let e = o * s; e < n; e++) t += x[e];
                         k.push(t)
                     }
-                    _ = -1, w = void 0, C.value = h(k, x, 0, T.value.from), q.value = h(k, x, T.value.to, e.value), t >= 0 ? (I(T.value.from), (0, o.Y3)((() => {
+                    _ = -1, w = void 0, C.value = h(k, x, 0, T.value.from), F.value = h(k, x, T.value.to, e.value), t >= 0 ? (I(T.value.from), (0, o.Y3)((() => {
                         B(t)
                     }))) : Z()
                 }
 
                 function z(e) {
                     if (void 0 === e && "undefined" !== typeof window) {
                         const o = t();
@@ -11694,15 +11739,15 @@
                     }
                     S = e;
                     const o = parseFloat(m.virtualScrollSliceRatioBefore) || 0,
                         r = parseFloat(m.virtualScrollSliceRatioAfter) || 0,
                         l = 1 + o + r,
                         a = void 0 === e || e <= 0 ? 1 : Math.ceil(e / i.value),
                         s = Math.max(1, a, Math.ceil((m.virtualScrollSliceSize > 0 ? m.virtualScrollSliceSize : 10) / l));
-                    F.value = {
+                    q.value = {
                         total: Math.ceil(s * l),
                         start: Math.ceil(s * o),
                         center: Math.ceil(s * (.5 + o)),
                         end: Math.ceil(s * (1 + o)),
                         view: a
                     }
                 }
@@ -11737,24 +11782,24 @@
                         tabindex: -1
                     }, t.flat()), "tbody" === e ? (0, o.h)(e, {
                         class: "q-virtual-scroll__padding",
                         key: "after",
                         ref: O
                     }, [(0, o.h)("tr", [(0, o.h)("td", {
                         style: {
-                            [n]: `${q.value}px`,
+                            [n]: `${F.value}px`,
                             ...r
                         },
                         colspan: A.value
                     })])]) : (0, o.h)(e, {
                         class: "q-virtual-scroll__padding",
                         key: "after",
                         ref: O,
                         style: {
-                            [n]: `${q.value}px`,
+                            [n]: `${F.value}px`,
                             ...r
                         }
                     })]
                 }
 
                 function D(e) {
                     _ !== e && (void 0 !== m.onVirtualScroll && g("virtualScroll", {
@@ -11782,15 +11827,15 @@
                     Z.cancel()
                 })), Object.assign(y, {
                     scrollTo: B,
                     reset: $,
                     refresh: j
                 }), {
                     virtualScrollSliceRange: T,
-                    virtualScrollSliceSizeComputed: F,
+                    virtualScrollSliceSizeComputed: q,
                     setVirtualScrollSize: z,
                     onVirtualScrollEvt: Z,
                     localResetVirtualScroll: H,
                     padVirtualScroll: U,
                     scrollTo: B,
                     reset: $,
                     refresh: j
@@ -12133,15 +12178,15 @@
                     for (const e in t.props) !0 === x.test(e) && (r[e] = t.props[e]);
                     n.attributes.value = o, n.listeners.value = r
                 }
                 return (0, o.Xn)(l), l(), n
             }
             var C = n(2026);
             n(5231), n(3075), n(548), n(2079), n(8218), n(6046);
-            let q, F = 0;
+            let F, q = 0;
             const E = new Array(256);
             for (let I = 0; I < 256; I++) E[I] = (I + 256).toString(16).substring(1);
             const O = (() => {
                     const e = "undefined" !== typeof crypto ? crypto : "undefined" !== typeof window ? window.crypto || window.msCrypto : void 0;
                     if (void 0 !== e) {
                         if (void 0 !== e.randomBytes) return e.randomBytes;
                         if (void 0 !== e.getRandomValues) return t => {
@@ -12154,16 +12199,16 @@
                         for (let n = e; n > 0; n--) t.push(Math.floor(256 * Math.random()));
                         return t
                     }
                 })(),
                 P = 4096;
 
             function T() {
-                (void 0 === q || F + 16 > P) && (F = 0, q = O(P));
-                const e = Array.prototype.slice.call(q, F, F += 16);
+                (void 0 === F || q + 16 > P) && (q = 0, F = O(P));
+                const e = Array.prototype.slice.call(F, q, q += 16);
                 return e[6] = 15 & e[6] | 64, e[8] = 63 & e[8] | 128, E[e[0]] + E[e[1]] + E[e[2]] + E[e[3]] + "-" + E[e[4]] + E[e[5]] + "-" + E[e[6]] + E[e[7]] + "-" + E[e[8]] + E[e[9]] + "-" + E[e[10]] + E[e[11]] + E[e[12]] + E[e[13]] + E[e[14]] + E[e[15]]
             }
             var A = n(1384),
                 R = n(7026);
 
             function L(e) {
                 return void 0 === e ? `f_${T()}` : e
@@ -12258,15 +12303,15 @@
                 })));
                 const {
                     isDirtyModel: p,
                     hasRules: v,
                     hasError: h,
                     errorMessage: m,
                     resetValidation: g
-                } = S(e.focused, e.innerLoading), y = void 0 !== e.floatingLabel ? (0, o.Fl)((() => !0 === t.stackLabel || !0 === e.focused.value || !0 === e.floatingLabel.value)) : (0, o.Fl)((() => !0 === t.stackLabel || !0 === e.focused.value || !0 === e.hasValue.value)), b = (0, o.Fl)((() => !0 === t.bottomSlots || void 0 !== t.hint || !0 === v.value || !0 === t.counter || null !== t.error)), w = (0, o.Fl)((() => !0 === t.filled ? "filled" : !0 === t.outlined ? "outlined" : !0 === t.borderless ? "borderless" : t.standout ? "standout" : "standard")), _ = (0, o.Fl)((() => `q-field row no-wrap items-start q-field--${w.value}` + (void 0 !== e.fieldClass ? ` ${e.fieldClass.value}` : "") + (!0 === t.rounded ? " q-field--rounded" : "") + (!0 === t.square ? " q-field--square" : "") + (!0 === y.value ? " q-field--float" : "") + (!0 === k.value ? " q-field--labeled" : "") + (!0 === t.dense ? " q-field--dense" : "") + (!0 === t.itemAligned ? " q-field--item-aligned q-item-type" : "") + (!0 === e.isDark.value ? " q-field--dark" : "") + (void 0 === e.getControl ? " q-field--auto-height" : "") + (!0 === e.focused.value ? " q-field--focused" : "") + (!0 === h.value ? " q-field--error" : "") + (!0 === h.value || !0 === e.focused.value ? " q-field--highlighted" : "") + (!0 !== t.hideBottomSpace && !0 === b.value ? " q-field--with-bottom" : "") + (!0 === t.disable ? " q-field--disabled" : !0 === t.readonly ? " q-field--readonly" : ""))), x = (0, o.Fl)((() => "q-field__control relative-position row no-wrap" + (void 0 !== t.bgColor ? ` bg-${t.bgColor}` : "") + (!0 === h.value ? " text-negative" : "string" === typeof t.standout && t.standout.length > 0 && !0 === e.focused.value ? ` ${t.standout}` : void 0 !== t.color ? ` text-${t.color}` : ""))), k = (0, o.Fl)((() => !0 === t.labelSlot || void 0 !== t.label)), q = (0, o.Fl)((() => "q-field__label no-pointer-events absolute ellipsis" + (void 0 !== t.labelColor && !0 !== h.value ? ` text-${t.labelColor}` : ""))), F = (0, o.Fl)((() => ({
+                } = S(e.focused, e.innerLoading), y = void 0 !== e.floatingLabel ? (0, o.Fl)((() => !0 === t.stackLabel || !0 === e.focused.value || !0 === e.floatingLabel.value)) : (0, o.Fl)((() => !0 === t.stackLabel || !0 === e.focused.value || !0 === e.hasValue.value)), b = (0, o.Fl)((() => !0 === t.bottomSlots || void 0 !== t.hint || !0 === v.value || !0 === t.counter || null !== t.error)), w = (0, o.Fl)((() => !0 === t.filled ? "filled" : !0 === t.outlined ? "outlined" : !0 === t.borderless ? "borderless" : t.standout ? "standout" : "standard")), _ = (0, o.Fl)((() => `q-field row no-wrap items-start q-field--${w.value}` + (void 0 !== e.fieldClass ? ` ${e.fieldClass.value}` : "") + (!0 === t.rounded ? " q-field--rounded" : "") + (!0 === t.square ? " q-field--square" : "") + (!0 === y.value ? " q-field--float" : "") + (!0 === k.value ? " q-field--labeled" : "") + (!0 === t.dense ? " q-field--dense" : "") + (!0 === t.itemAligned ? " q-field--item-aligned q-item-type" : "") + (!0 === e.isDark.value ? " q-field--dark" : "") + (void 0 === e.getControl ? " q-field--auto-height" : "") + (!0 === e.focused.value ? " q-field--focused" : "") + (!0 === h.value ? " q-field--error" : "") + (!0 === h.value || !0 === e.focused.value ? " q-field--highlighted" : "") + (!0 !== t.hideBottomSpace && !0 === b.value ? " q-field--with-bottom" : "") + (!0 === t.disable ? " q-field--disabled" : !0 === t.readonly ? " q-field--readonly" : ""))), x = (0, o.Fl)((() => "q-field__control relative-position row no-wrap" + (void 0 !== t.bgColor ? ` bg-${t.bgColor}` : "") + (!0 === h.value ? " text-negative" : "string" === typeof t.standout && t.standout.length > 0 && !0 === e.focused.value ? ` ${t.standout}` : void 0 !== t.color ? ` text-${t.color}` : ""))), k = (0, o.Fl)((() => !0 === t.labelSlot || void 0 !== t.label)), F = (0, o.Fl)((() => "q-field__label no-pointer-events absolute ellipsis" + (void 0 !== t.labelColor && !0 !== h.value ? ` text-${t.labelColor}` : ""))), q = (0, o.Fl)((() => ({
                     id: e.targetUid.value,
                     editable: e.editable.value,
                     focused: e.focused.value,
                     floatingLabel: y.value,
                     modelValue: t.modelValue,
                     emitValue: e.emitValue
                 }))), E = (0, o.Fl)((() => {
@@ -12349,16 +12394,16 @@
                         class: "q-field__prefix no-pointer-events row items-center"
                     }, t.prefix)), void 0 !== e.getShadowControl && !0 === e.hasShadow.value && n.push(e.getShadowControl()), void 0 !== e.getControl ? n.push(e.getControl()) : void 0 !== r.rawControl ? n.push(r.rawControl()) : void 0 !== r.control && n.push((0, o.h)("div", {
                         ref: e.targetRef,
                         class: "q-field__native row",
                         tabindex: -1,
                         ...e.splitAttrs.attributes.value,
                         "data-autofocus": !0 === t.autofocus || void 0
-                    }, r.control(F.value))), !0 === k.value && n.push((0, o.h)("div", {
-                        class: q.value
+                    }, r.control(q.value))), !0 === k.value && n.push((0, o.h)("div", {
+                        class: F.value
                     }, (0, C.KR)(r.label, t.label))), void 0 !== t.suffix && null !== t.suffix && n.push((0, o.h)("div", {
                         class: "q-field__suffix no-pointer-events row items-center"
                     }, t.suffix)), n.concat((0, C.KR)(r.default))
                 }
 
                 function N() {
                     let n, i;
@@ -12856,15 +12901,15 @@
                     if (!0 === s.disable) return e.preventDefault(), Promise.resolve(!1);
                     if (e.metaKey || e.altKey || e.ctrlKey || e.shiftKey || void 0 !== e.button && 0 !== e.button || "_blank" === s.target) return Promise.resolve(!1);
                     e.preventDefault();
                     const r = u.$router[!0 === o ? "replace" : "push"](n);
                     return !0 === t ? r : r.then((() => {})).catch((() => {}))
                 }
 
-                function q(e) {
+                function F(e) {
                     if (!0 === m.value) {
                         const t = t => C(e, t);
                         d("click", e, t), !0 !== e.defaultPrevented && t()
                     } else d("click", e)
                 }
                 return {
                     hasRouterLink: m,
@@ -12874,15 +12919,15 @@
                     resolvedLink: h,
                     linkIsActive: _,
                     linkIsExactActive: S,
                     linkClass: x,
                     linkAttrs: b,
                     getLink: k,
                     navigateToRouterLink: C,
-                    navigateOnClick: q
+                    navigateOnClick: F
                 }
             }
         },
         4088: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => i
@@ -14537,15 +14582,15 @@
                                 void 0 !== t.config.brand && k(t.config.brand);
                                 const n = S(o.Lp, t.config);
                                 document.body.classList.add.apply(document.body.classList, n)
                             }!0 === o.Lp.is.ios && document.body.addEventListener("touchstart", a.ZT), window.addEventListener("keydown", w.ZK, !0)
                         }
                     }
                 },
-                q = {
+                F = {
                     name: "material-icons",
                     type: {
                         positive: "check_circle",
                         negative: "warning",
                         info: "info",
                         warning: "priority_high"
                     },
@@ -14665,36 +14710,36 @@
                         clear: "clear",
                         add: "add_box",
                         upload: "cloud_upload",
                         removeQueue: "clear_all",
                         removeUploaded: "done_all"
                     }
                 },
-                F = i({
+                q = i({
                     iconMapFn: null,
                     __icons: {}
                 }, {
                     set(e, t) {
                         const n = {
                             ...e,
                             rtl: !0 === e.rtl
                         };
-                        n.set = F.set, Object.assign(F.__icons, n)
+                        n.set = q.set, Object.assign(q.__icons, n)
                     },
                     install({
                         $q: e,
                         iconSet: t,
                         ssrContext: n
                     }) {
                         void 0 !== e.config.iconMapFn && (this.iconMapFn = e.config.iconMapFn), e.iconSet = this.__icons, (0, l.g)(e, "iconMapFn", (() => this.iconMapFn), (e => {
                             this.iconMapFn = e
-                        })), !0 === this.__installed ? void 0 !== t && this.set(t) : this.set(t || q)
+                        })), !0 === this.__installed ? void 0 !== t && this.set(t) : this.set(t || F)
                     }
                 }),
-                E = F;
+                E = q;
             var O = n(5439),
                 P = n(7495),
                 T = n(4680);
             const A = [o.ZP, C, p, d, v.Z, y, E];
 
             function R(e, t) {
                 t.forEach((t => {
@@ -14782,19 +14827,19 @@
                 b = n(6534),
                 w = n(4103),
                 _ = n(3965),
                 S = n(780),
                 x = S.enforce,
                 k = S.get,
                 C = s.Int8Array,
-                q = C && C.prototype,
-                F = s.Uint8ClampedArray,
-                E = F && F.prototype,
+                F = C && C.prototype,
+                q = s.Uint8ClampedArray,
+                E = q && q.prototype,
                 O = C && y(C),
-                P = q && y(q),
+                P = F && y(F),
                 T = Object.prototype,
                 A = s.TypeError,
                 R = w("toStringTag"),
                 L = _("TYPED_ARRAY_TAG"),
                 $ = "TypedArrayConstructor",
                 j = i && !!b && "Opera" !== f(s.opera),
                 B = !1,
@@ -14847,15 +14892,15 @@
                                     delete l.prototype[e]
                                 } catch (i) {
                                     try {
                                         l.prototype[e] = t
                                     } catch (u) {}
                                 }
                             }
-                        P[e] && !n || h(P, e, n ? t : j && q[e] || t, o)
+                        P[e] && !n || h(P, e, n ? t : j && F[e] || t, o)
                     }
                 },
                 Z = function(e, t, n) {
                     var o, r;
                     if (a) {
                         if (b) {
                             if (n)
@@ -16369,45 +16414,45 @@
 
             function C(e) {
                 if ("string" === typeof e) {
                     var t = unescape(encodeURIComponent(e));
                     e = new Uint8Array(t.length);
                     for (var n = 0; n < t.length; ++n) e[n] = t.charCodeAt(n)
                 }
-                return q(E(O(e), 8 * e.length))
+                return F(E(O(e), 8 * e.length))
             }
 
-            function q(e) {
+            function F(e) {
                 for (var t = [], n = 32 * e.length, o = "0123456789abcdef", r = 0; r < n; r += 8) {
                     var l = e[r >> 5] >>> r % 32 & 255,
                         i = parseInt(o.charAt(l >>> 4 & 15) + o.charAt(15 & l), 16);
                     t.push(i)
                 }
                 return t
             }
 
-            function F(e) {
+            function q(e) {
                 return 14 + (e + 64 >>> 9 << 4) + 1
             }
 
             function E(e, t) {
-                e[t >> 5] |= 128 << t % 32, e[F(t) - 1] = t;
+                e[t >> 5] |= 128 << t % 32, e[q(t) - 1] = t;
                 for (var n = 1732584193, o = -271733879, r = -1732584194, l = 271733878, i = 0; i < e.length; i += 16) {
                     var a = n,
                         s = o,
                         u = r,
                         c = l;
                     n = R(n, o, r, l, e[i], 7, -680876936), l = R(l, n, o, r, e[i + 1], 12, -389564586), r = R(r, l, n, o, e[i + 2], 17, 606105819), o = R(o, r, l, n, e[i + 3], 22, -1044525330), n = R(n, o, r, l, e[i + 4], 7, -176418897), l = R(l, n, o, r, e[i + 5], 12, 1200080426), r = R(r, l, n, o, e[i + 6], 17, -1473231341), o = R(o, r, l, n, e[i + 7], 22, -45705983), n = R(n, o, r, l, e[i + 8], 7, 1770035416), l = R(l, n, o, r, e[i + 9], 12, -1958414417), r = R(r, l, n, o, e[i + 10], 17, -42063), o = R(o, r, l, n, e[i + 11], 22, -1990404162), n = R(n, o, r, l, e[i + 12], 7, 1804603682), l = R(l, n, o, r, e[i + 13], 12, -40341101), r = R(r, l, n, o, e[i + 14], 17, -1502002290), o = R(o, r, l, n, e[i + 15], 22, 1236535329), n = L(n, o, r, l, e[i + 1], 5, -165796510), l = L(l, n, o, r, e[i + 6], 9, -1069501632), r = L(r, l, n, o, e[i + 11], 14, 643717713), o = L(o, r, l, n, e[i], 20, -373897302), n = L(n, o, r, l, e[i + 5], 5, -701558691), l = L(l, n, o, r, e[i + 10], 9, 38016083), r = L(r, l, n, o, e[i + 15], 14, -660478335), o = L(o, r, l, n, e[i + 4], 20, -405537848), n = L(n, o, r, l, e[i + 9], 5, 568446438), l = L(l, n, o, r, e[i + 14], 9, -1019803690), r = L(r, l, n, o, e[i + 3], 14, -187363961), o = L(o, r, l, n, e[i + 8], 20, 1163531501), n = L(n, o, r, l, e[i + 13], 5, -1444681467), l = L(l, n, o, r, e[i + 2], 9, -51403784), r = L(r, l, n, o, e[i + 7], 14, 1735328473), o = L(o, r, l, n, e[i + 12], 20, -1926607734), n = $(n, o, r, l, e[i + 5], 4, -378558), l = $(l, n, o, r, e[i + 8], 11, -2022574463), r = $(r, l, n, o, e[i + 11], 16, 1839030562), o = $(o, r, l, n, e[i + 14], 23, -35309556), n = $(n, o, r, l, e[i + 1], 4, -1530992060), l = $(l, n, o, r, e[i + 4], 11, 1272893353), r = $(r, l, n, o, e[i + 7], 16, -155497632), o = $(o, r, l, n, e[i + 10], 23, -1094730640), n = $(n, o, r, l, e[i + 13], 4, 681279174), l = $(l, n, o, r, e[i], 11, -358537222), r = $(r, l, n, o, e[i + 3], 16, -722521979), o = $(o, r, l, n, e[i + 6], 23, 76029189), n = $(n, o, r, l, e[i + 9], 4, -640364487), l = $(l, n, o, r, e[i + 12], 11, -421815835), r = $(r, l, n, o, e[i + 15], 16, 530742520), o = $(o, r, l, n, e[i + 2], 23, -995338651), n = j(n, o, r, l, e[i], 6, -198630844), l = j(l, n, o, r, e[i + 7], 10, 1126891415), r = j(r, l, n, o, e[i + 14], 15, -1416354905), o = j(o, r, l, n, e[i + 5], 21, -57434055), n = j(n, o, r, l, e[i + 12], 6, 1700485571), l = j(l, n, o, r, e[i + 3], 10, -1894986606), r = j(r, l, n, o, e[i + 10], 15, -1051523), o = j(o, r, l, n, e[i + 1], 21, -2054922799), n = j(n, o, r, l, e[i + 8], 6, 1873313359), l = j(l, n, o, r, e[i + 15], 10, -30611744), r = j(r, l, n, o, e[i + 6], 15, -1560198380), o = j(o, r, l, n, e[i + 13], 21, 1309151649), n = j(n, o, r, l, e[i + 4], 6, -145523070), l = j(l, n, o, r, e[i + 11], 10, -1120210379), r = j(r, l, n, o, e[i + 2], 15, 718787259), o = j(o, r, l, n, e[i + 9], 21, -343485551), n = P(n, a), o = P(o, s), r = P(r, u), l = P(l, c)
                 }
                 return [n, o, r, l]
             }
 
             function O(e) {
                 if (0 === e.length) return [];
-                for (var t = 8 * e.length, n = new Uint32Array(F(t)), o = 0; o < t; o += 8) n[o >> 5] |= (255 & e[o / 8]) << o % 32;
+                for (var t = 8 * e.length, n = new Uint32Array(q(t)), o = 0; o < t; o += 8) n[o >> 5] |= (255 & e[o / 8]) << o % 32;
                 return n
             }
 
             function P(e, t) {
                 var n = (65535 & e) + (65535 & t),
                     o = (e >> 16) + (t >> 16) + (n >> 16);
                 return o << 16 | 65535 & n
@@ -16625,23 +16670,23 @@
             })(S || (S = {}));
             const x = "undefined" !== typeof window,
                 k = !1,
                 C = (() => "object" === typeof window && window.window === window ? window : "object" === typeof self && self.self === self ? self : "object" === typeof n.g && n.g.global === n.g ? n.g : "object" === typeof globalThis ? globalThis : {
                     HTMLElement: null
                 })();
 
-            function q(e, {
+            function F(e, {
                 autoBom: t = !1
             } = {}) {
                 return t && /^\s*(?:text\/\S*|application\/xml|\S*\/\S*\+xml)\s*;.*charset\s*=\s*utf-8/i.test(e.type) ? new Blob([String.fromCharCode(65279), e], {
                     type: e.type
                 }) : e
             }
 
-            function F(e, t, n) {
+            function q(e, t, n) {
                 const o = new XMLHttpRequest;
                 o.open("GET", e), o.responseType = "blob", o.onload = function() {
                     A(o.response, t, n)
                 }, o.onerror = function() {
                     console.error("could not download file")
                 }, o.send()
             }
@@ -16667,35 +16712,35 @@
                     userAgent: ""
                 },
                 T = (() => /Macintosh/.test(P.userAgent) && /AppleWebKit/.test(P.userAgent) && !/Safari/.test(P.userAgent))(),
                 A = x ? "undefined" !== typeof HTMLAnchorElement && "download" in HTMLAnchorElement.prototype && !T ? R : "msSaveOrOpenBlob" in P ? L : $ : () => {};
 
             function R(e, t = "download", n) {
                 const o = document.createElement("a");
-                o.download = t, o.rel = "noopener", "string" === typeof e ? (o.href = e, o.origin !== location.origin ? E(o.href) ? F(e, t, n) : (o.target = "_blank", O(o)) : O(o)) : (o.href = URL.createObjectURL(e), setTimeout((function() {
+                o.download = t, o.rel = "noopener", "string" === typeof e ? (o.href = e, o.origin !== location.origin ? E(o.href) ? q(e, t, n) : (o.target = "_blank", O(o)) : O(o)) : (o.href = URL.createObjectURL(e), setTimeout((function() {
                     URL.revokeObjectURL(o.href)
                 }), 4e4), setTimeout((function() {
                     O(o)
                 }), 0))
             }
 
             function L(e, t = "download", n) {
                 if ("string" === typeof e)
-                    if (E(e)) F(e, t, n);
+                    if (E(e)) q(e, t, n);
                     else {
                         const t = document.createElement("a");
                         t.href = e, t.target = "_blank", setTimeout((function() {
                             O(t)
                         }))
                     }
-                else navigator.msSaveOrOpenBlob(q(e, n), t)
+                else navigator.msSaveOrOpenBlob(F(e, n), t)
             }
 
             function $(e, t, n, o) {
-                if (o = o || open("", "_blank"), o && (o.document.title = o.document.body.innerText = "downloading..."), "string" === typeof e) return F(e, t, n);
+                if (o = o || open("", "_blank"), o && (o.document.title = o.document.body.innerText = "downloading..."), "string" === typeof e) return q(e, t, n);
                 const r = "application/octet-stream" === e.type,
                     l = /constructor/i.test(String(C.HTMLElement)) || "safari" in C,
                     i = /CriOS\/[\d]+/.test(navigator.userAgent);
                 if ((i || r && l || T) && "undefined" !== typeof FileReader) {
                     const t = new FileReader;
                     t.onloadend = function() {
                         let e = t.result;
@@ -16839,29 +16884,29 @@
                 })))), e._customProperties.size && (t.customProperties = Array.from(e._customProperties).map((t => ({
                     editable: !0,
                     key: t,
                     value: e[t]
                 })))), t
             }
 
-            function X(e) {
+            function Q(e) {
                 return e ? Array.isArray(e) ? e.reduce(((e, t) => (e.keys.push(t.key), e.operations.push(t.type), e.oldValue[t.key] = t.oldValue, e.newValue[t.key] = t.newValue, e)), {
                     oldValue: {},
                     keys: [],
                     operations: [],
                     newValue: {}
                 }) : {
                     operation: Z(e.type),
                     key: Z(e.key),
                     oldValue: e.oldValue,
                     newValue: e.newValue
                 } : {}
             }
 
-            function Q(e) {
+            function X(e) {
                 switch (e) {
                     case S.direct:
                         return "mutation";
                     case S.patchFunction:
                         return "$patch";
                     case S.patchObject:
                         return "$patch";
@@ -17092,18 +17137,18 @@
                     })), t.$subscribe((({
                         events: o,
                         type: r
                     }, l) => {
                         if (e.notifyComponentUpdate(), e.sendInspectorState(ne), !G) return;
                         const i = {
                             time: n(),
-                            title: Q(r),
+                            title: X(r),
                             data: oe({
                                 store: Z(t.$id)
-                            }, X(o)),
+                            }, Q(o)),
                             groupId: ae
                         };
                         ae = void 0, r === S.patchFunction ? i.subtitle = "⤵️" : r === S.patchObject ? i.subtitle = "🧩" : o && !Array.isArray(o) && (i.subtitle = o.type), o && (i.data["rawEvent(s)"] = {
                             _custom: {
                                 display: "DebuggerEvent",
                                 type: "object",
                                 tooltip: "raw DebuggerEvent[]",
@@ -17294,19 +17339,19 @@
                         state: e
                     } = n, t = e ? e() : {};
                     this.$patch((e => {
                         be(e, t)
                     }))
                 } : fe;
 
-                function q() {
+                function F() {
                     c.stop(), m = [], g = [], a._s.delete(e)
                 }
 
-                function F(t, n) {
+                function q(t, n) {
                     return function() {
                         b(a);
                         const o = Array.from(arguments),
                             r = [],
                             l = [];
 
                         function i(e) {
@@ -17351,28 +17396,28 @@
                                         storeId: e,
                                         type: S.direct,
                                         events: h
                                     }, o)
                                 }), be({}, f, n))));
                             return o
                         },
-                        $dispose: q
+                        $dispose: F
                     };
                 l && (O._r = !1);
                 const P = (0, o.qj)(k ? be({
                     _hmrPayload: E,
                     _customProperties: (0, o.Xl)(new Set)
                 }, O) : O);
                 a._s.set(e, P);
                 const T = a._e.run((() => (c = (0, o.B)(), c.run((() => t())))));
                 for (const r in T) {
                     const t = T[r];
                     if ((0, o.dq)(t) && !we(t) || (0, o.PG)(t)) u || (y && ye(t) && ((0, o.dq)(t) ? t.value = y[r] : he(t, y[r])), l ? i(a.state.value[e], r, t) : a.state.value[e][r] = t);
                     else if ("function" === typeof t) {
-                        const e = F(r, t);
+                        const e = q(r, t);
                         l ? i(T, r, e) : T[r] = e, d.actions[r] = t
                     } else 0
                 }
                 if (l ? Object.keys(T).forEach((e => {
                         i(P, e, T[e])
                     })) : (be(P, T), be((0, o.IU)(P), T)), Object.defineProperty(P, "$state", {
                         get: () => a.state.value[e],
@@ -17553,19 +17598,19 @@
                         const t = document.querySelector("base");
                         e = t && t.getAttribute("href") || "/", e = e.replace(/^\w+:\/\/[^\/]+/, "")
                     } else e = "/";
                 return "/" !== e[0] && "#" !== e[0] && (e = "/" + e), f(e)
             }
             const C = /^[^#]+#/;
 
-            function q(e, t) {
+            function F(e, t) {
                 return e.replace(C, "#") + t
             }
 
-            function F(e, t) {
+            function q(e, t) {
                 const n = document.documentElement.getBoundingClientRect(),
                     o = e.getBoundingClientRect();
                 return {
                     behavior: t.behavior,
                     left: o.left - n.left - (t.left || 0),
                     top: o.top - n.top - (t.top || 0)
                 }
@@ -17579,15 +17624,15 @@
                 let t;
                 if ("el" in e) {
                     const n = e.el,
                         o = "string" === typeof n && n.startsWith("#");
                     0;
                     const r = "string" === typeof n ? o ? document.getElementById(n.slice(1)) : document.querySelector(n) : n;
                     if (!r) return;
-                    t = F(r, e)
+                    t = q(r, e)
                 } else t = e;
                 "scrollBehavior" in document.documentElement.style ? window.scrollTo(t) : window.scrollTo(null != t.left ? t.left : window.pageXOffset, null != t.top ? t.top : window.pageYOffset)
             }
 
             function P(e, t) {
                 const n = history.state ? history.state.position - t : -1;
                 return n + e
@@ -17748,15 +17793,15 @@
                 function o(e, t = !0) {
                     t || n.pauseListeners(), history.go(e)
                 }
                 const r = a({
                     location: "",
                     base: e,
                     go: o,
-                    createHref: q.bind(null, e)
+                    createHref: F.bind(null, e)
                 }, t, n);
                 return Object.defineProperty(r, "location", {
                     enumerable: !0,
                     get: () => t.location.value
                 }), Object.defineProperty(r, "state", {
                     enumerable: !0,
                     get: () => t.state.value
@@ -17894,30 +17939,30 @@
                     score: o,
                     keys: l,
                     parse: s,
                     stringify: u
                 }
             }
 
-            function X(e, t) {
+            function Q(e, t) {
                 let n = 0;
                 while (n < e.length && n < t.length) {
                     const o = t[n] - e[n];
                     if (o) return o;
                     n++
                 }
                 return e.length < t.length ? 1 === e.length && 80 === e[0] ? -1 : 1 : e.length > t.length ? 1 === t.length && 80 === t[0] ? 1 : -1 : 0
             }
 
-            function Q(e, t) {
+            function X(e, t) {
                 let n = 0;
                 const o = e.score,
                     r = t.score;
                 while (n < o.length && n < r.length) {
-                    const e = X(o[n], r[n]);
+                    const e = Q(o[n], r[n]);
                     if (e) return e;
                     n++
                 }
                 if (1 === Math.abs(r.length - o.length)) {
                     if (G(o)) return 1;
                     if (G(r)) return -1
                 }
@@ -18064,15 +18109,15 @@
 
                 function s() {
                     return n
                 }
 
                 function c(e) {
                     let t = 0;
-                    while (t < n.length && Q(e, n[t]) >= 0 && (e.record.path !== n[t].record.path || !de(e, n[t]))) t++;
+                    while (t < n.length && X(e, n[t]) >= 0 && (e.record.path !== n[t].record.path || !de(e, n[t]))) t++;
                     n.splice(t, 0, e), e.record.name && !se(e) && o.set(e.record.name, e)
                 }
 
                 function d(e, t) {
                     let r, l, i, s = {};
                     if ("name" in e && e.name) {
                         if (r = o.get(e.name), !r) throw D(1, {
@@ -18178,32 +18223,32 @@
                 we = /%5E/g,
                 _e = /%60/g,
                 Se = /%7B/g,
                 xe = /%7C/g,
                 ke = /%7D/g,
                 Ce = /%20/g;
 
-            function qe(e) {
+            function Fe(e) {
                 return encodeURI("" + e).replace(xe, "|").replace(ye, "[").replace(be, "]")
             }
 
-            function Fe(e) {
-                return qe(e).replace(Se, "{").replace(ke, "}").replace(we, "^")
+            function qe(e) {
+                return Fe(e).replace(Se, "{").replace(ke, "}").replace(we, "^")
             }
 
             function Ee(e) {
-                return qe(e).replace(ge, "%2B").replace(Ce, "+").replace(fe, "%23").replace(pe, "%26").replace(_e, "`").replace(Se, "{").replace(ke, "}").replace(we, "^")
+                return Fe(e).replace(ge, "%2B").replace(Ce, "+").replace(fe, "%23").replace(pe, "%26").replace(_e, "`").replace(Se, "{").replace(ke, "}").replace(we, "^")
             }
 
             function Oe(e) {
                 return Ee(e).replace(he, "%3D")
             }
 
             function Pe(e) {
-                return qe(e).replace(fe, "%23").replace(me, "%3F")
+                return Fe(e).replace(fe, "%23").replace(me, "%3F")
             }
 
             function Te(e) {
                 return null == e ? "" : Pe(e).replace(ve, "%2F")
             }
 
             function Ae(e) {
@@ -18384,16 +18429,16 @@
                         slots: t
                     }) {
                         const n = (0, r.qj)(De(e)),
                             {
                                 options: l
                             } = (0, o.f3)(Ve),
                             i = (0, o.Fl)((() => ({
-                                [Xe(e.activeClass, l.linkActiveClass, "router-link-active")]: n.isActive,
-                                [Xe(e.exactActiveClass, l.linkExactActiveClass, "router-link-exact-active")]: n.isExactActive
+                                [Qe(e.activeClass, l.linkActiveClass, "router-link-active")]: n.isActive,
+                                [Qe(e.exactActiveClass, l.linkExactActiveClass, "router-link-exact-active")]: n.isExactActive
                             })));
                         return () => {
                             const r = t.default && t.default(n);
                             return e.custom ? r : (0, o.h)("a", {
                                 "aria-current": n.isExactActive ? e.ariaCurrentValue : null,
                                 href: n.href,
                                 onClick: n.navigate,
@@ -18424,16 +18469,16 @@
                 }
                 return !0
             }
 
             function We(e) {
                 return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
             }
-            const Xe = (e, t, n) => null != e ? e : null != t ? t : n,
-                Qe = (0, o.aZ)({
+            const Qe = (e, t, n) => null != e ? e : null != t ? t : n,
+                Xe = (0, o.aZ)({
                     name: "RouterView",
                     inheritAttrs: !1,
                     props: {
                         name: {
                             type: String,
                             default: "default"
                         },
@@ -18492,15 +18537,15 @@
                 });
 
             function Ge(e, t) {
                 if (!e) return null;
                 const n = e(t);
                 return 1 === n.length ? n[0] : n
             }
-            const et = Qe;
+            const et = Xe;
 
             function tt(e) {
                 const t = re(e.routes, e),
                     n = e.parseQuery || Re,
                     i = e.stringifyQuery || Le,
                     d = e.history;
                 const f = Ne(),
@@ -18519,19 +18564,19 @@
                 }
 
                 function C(e) {
                     const n = t.getRecordMatcher(e);
                     n && t.removeRoute(n)
                 }
 
-                function q() {
+                function F() {
                     return t.getRoutes().map((e => e.record))
                 }
 
-                function F(e) {
+                function q(e) {
                     return !!t.getRecordMatcher(e)
                 }
 
                 function T(e, o) {
                     if (o = a({}, o || y.value), "string" === typeof e) {
                         const r = p(n, e, o.path),
                             l = t.resolve({
@@ -18556,15 +18601,15 @@
                             params: _(e.params)
                         }), o.params = _(o.params)
                     }
                     const l = t.resolve(r, o),
                         s = e.hash || "";
                     l.params = w(x(l.params));
                     const u = v(i, a({}, e, {
-                            hash: Fe(s),
+                            hash: qe(s),
                             path: l.path
                         })),
                         c = d.createHref(u);
                     return a({
                         fullPath: u,
                         hash: s,
                         query: i === Le ? $e(e.query) : e.query || {}
@@ -18708,31 +18753,31 @@
                         l && A(P(i.fullPath, n.delta), E()), z(o, i).catch((e => Z(e, 12) ? e : Z(e, 2) ? (M(e.to, o).then((e => {
                             Z(e, 20) && !n.delta && n.type === S.pop && d.go(-1, !1)
                         })).catch(u), Promise.reject()) : (n.delta && d.go(-n.delta, !1), G(e, o, i)))).then((e => {
                             e = e || K(o, i, !1), e && (n.delta && !Z(e, 8) ? d.go(-n.delta, !1) : n.type === S.pop && Z(e, 20) && d.go(-1, !1)), U(o, i, e)
                         })).catch(u)
                     })))
                 }
-                let W, X = Ne(),
-                    Q = Ne();
+                let W, Q = Ne(),
+                    X = Ne();
 
                 function G(e, t, n) {
                     te(e);
-                    const o = Q.list();
+                    const o = X.list();
                     return o.length ? o.forEach((o => o(e, t, n))) : console.error(e), Promise.reject(e)
                 }
 
                 function ee() {
                     return W && y.value !== H ? Promise.resolve() : new Promise(((e, t) => {
-                        X.add([e, t])
+                        Q.add([e, t])
                     }))
                 }
 
                 function te(e) {
-                    return W || (W = !e, J(), X.list().forEach((([t, n]) => e ? n(e) : t())), X.reset()), e
+                    return W || (W = !e, J(), Q.list().forEach((([t, n]) => e ? n(e) : t())), Q.reset()), e
                 }
 
                 function ne(t, n, r, i) {
                     const {
                         scrollBehavior: a
                     } = e;
                     if (!l || !a) return Promise.resolve();
@@ -18743,27 +18788,27 @@
                 let le;
                 const ie = new Set,
                     ae = {
                         currentRoute: y,
                         listening: !0,
                         addRoute: k,
                         removeRoute: C,
-                        hasRoute: F,
-                        getRoutes: q,
+                        hasRoute: q,
+                        getRoutes: F,
                         resolve: T,
                         options: e,
                         push: j,
                         replace: B,
                         go: oe,
                         back: () => oe(-1),
                         forward: () => oe(1),
                         beforeEach: f.add,
                         beforeResolve: h.add,
                         afterEach: g.add,
-                        onError: Q.add,
+                        onError: X.add,
                         isReady: ee,
                         install(e) {
                             const t = this;
                             e.component("RouterLink", Ke), e.component("RouterView", et), e.config.globalProperties.$router = t, Object.defineProperty(e.config.globalProperties, "$route", {
                                 enumerable: !0,
                                 get: () => (0, r.SU)(y)
                             }), l && !le && y.value === H && (le = !0, j(d.location).catch((e => {
```

### Comparing `decore_Base-0.0.23/decore_base/sample/spa/templates/index.html` & `decore_Base-0.0.24/decore_base/prepare/spa/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.0902ddb5.js></script><script defer src=/static/js/app.af6cbe84.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><base href=/static/ ><title>Uniform Front</title><meta charset=utf-8><meta name=description content="A part of Unform Famework"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><meta name=api_prod_port content={{port}}><meta name=api_dev_port content=5566><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=/static/js/vendor.6fe961ae.js></script><script defer src=/static/js/app.aff5db90.js></script><link href=/static/css/vendor.14c9ac7a.css rel=stylesheet><link href=/static/css/app.d398f07d.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `decore_Base-0.0.23/decore_base/uniform/conform_model.py` & `decore_Base-0.0.24/decore_base/uniform/conform_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,13 @@
     def __init__(self, *args, **kwargs):
         Decore_model.__init__(self, *args, **kwargs)
 
     class Meta:
         # TODO - diese Zeile wieder einsetzen wenn alle Relationen zwischen conform und perform passen
         # database = SqliteDatabase('state/database.db', pragmas=(('cache_size', -1024 * 64),('journal_mode', 'wal')))
         database = SqliteDatabase('state/database.db')
-        migrator = SqliteMigrator(database)
 
     @classmethod
     def register(cls):
         super(Conform_model, cls).register()
         cls.migrate_database()
         return cls
```

### Comparing `decore_Base-0.0.23/decore_base/uniform/depricated/askform_base.py` & `decore_Base-0.0.24/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/depricated/buyform_base.py` & `decore_Base-0.0.24/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/depricated/conform_base.py` & `decore_Base-0.0.24/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/depricated/deform_base.py` & `decore_Base-0.0.24/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/perform_model.py` & `decore_Base-0.0.24/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/reform_client_model.py` & `decore_Base-0.0.24/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/decore_base/uniform/reform_server_model.py` & `decore_Base-0.0.24/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/Makefile` & `decore_Base-0.0.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/_static/favicon.ico` & `decore_Base-0.0.24/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/_static/logo.png` & `decore_Base-0.0.24/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/conf.py` & `decore_Base-0.0.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/make.bat` & `decore_Base-0.0.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/doctrees/environment.pickle` & `decore_Base-0.0.24/docs/page/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/doctrees/index.doctree` & `decore_Base-0.0.24/docs/page/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/basic.css` & `decore_Base-0.0.24/docs/page/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/clipboard.min.js` & `decore_Base-0.0.24/docs/page/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/copybutton.css` & `decore_Base-0.0.24/docs/page/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/copybutton.js` & `decore_Base-0.0.24/docs/page/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/copybutton_funcs.js` & `decore_Base-0.0.24/docs/page/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/doctools.js` & `decore_Base-0.0.24/docs/page/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/favicon.ico` & `decore_Base-0.0.24/docs/page/html/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/language_data.js` & `decore_Base-0.0.24/docs/page/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/logo.png` & `decore_Base-0.0.24/docs/page/html/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/pygments.css` & `decore_Base-0.0.24/docs/page/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js` & `decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.map` & `decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js` & `decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map` & `decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/searchtools.js` & `decore_Base-0.0.24/docs/page/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/sphinx_highlight.js` & `decore_Base-0.0.24/docs/page/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/styles/bootstrap.css` & `decore_Base-0.0.24/docs/page/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/styles/pydata-sphinx-theme.css` & `decore_Base-0.0.24/docs/page/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/_static/webpack-macros.html` & `decore_Base-0.0.24/docs/page/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/genindex.html` & `decore_Base-0.0.24/docs/page/html/genindex.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/index.html` & `decore_Base-0.0.24/docs/page/html/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/search.html` & `decore_Base-0.0.24/docs/page/html/search.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/page/html/searchindex.js` & `decore_Base-0.0.24/docs/page/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/state/keybase.kdbx` & `decore_Base-0.0.24/docs/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/docs/state/querybase.db` & `decore_Base-0.0.24/decore_base/sample/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/requirements.txt` & `decore_Base-0.0.24/requirements.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.23/setup.cfg` & `decore_Base-0.0.24/setup.cfg`

 * *Files identical despite different names*

