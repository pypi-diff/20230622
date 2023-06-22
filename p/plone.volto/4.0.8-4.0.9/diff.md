# Comparing `tmp/plone.volto-4.0.8.tar.gz` & `tmp/plone.volto-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.volto-4.0.8.tar", last modified: Thu Mar 23 11:58:19 2023, max compression
+gzip compressed data, was "plone.volto-4.0.9.tar", last modified: Thu Jun 22 19:24:03 2023, max compression
```

## Comparing `plone.volto-4.0.8.tar` & `plone.volto-4.0.9.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.868768 plone.volto-4.0.8/
--rw-r--r--   0 maurits    (501) staff       (20)    13707 2023-03-23 11:58:18.000000 plone.volto-4.0.8/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-03-23 11:58:18.000000 plone.volto-4.0.8/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)    25931 2023-03-23 11:58:19.868470 plone.volto-4.0.8/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    10929 2023-03-23 11:58:18.000000 plone.volto-4.0.8/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.833430 plone.volto-4.0.8/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-03-23 11:58:18.000000 plone.volto-4.0.8/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      657 2023-03-23 11:58:18.000000 plone.volto-4.0.8/docs/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       74 2023-03-23 11:58:18.000000 plone.volto-4.0.8/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      881 2023-03-23 11:58:18.000000 plone.volto-4.0.8/pyproject.toml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.834661 plone.volto-4.0.8/requirements/
--rw-r--r--   0 maurits    (501) staff       (20)       12 2023-03-23 11:58:18.000000 plone.volto-4.0.8/requirements/dev.txt
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-03-23 11:58:18.000000 plone.volto-4.0.8/requirements/plone-5.2.txt
--rw-r--r--   0 maurits    (501) staff       (20)       69 2023-03-23 11:58:18.000000 plone.volto-4.0.8/requirements/plone-6.0.txt
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-23 11:58:18.000000 plone.volto-4.0.8/requirements/prod.txt
--rw-r--r--   0 maurits    (501) staff       (20)      402 2023-03-23 11:58:18.000000 plone.volto-4.0.8/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-03-23 11:58:19.868839 plone.volto-4.0.8/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2227 2023-03-23 11:58:18.000000 plone.volto-4.0.8/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.825103 plone.volto-4.0.8/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.834950 plone.volto-4.0.8/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.843243 plone.volto-4.0.8/src/plone/volto/
--rw-r--r--   0 maurits    (501) staff       (20)      222 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.844931 plone.volto-4.0.8/src/plone/volto/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      534 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/headtitle.py
--rw-r--r--   0 maurits    (501) staff       (20)      345 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/navtitle.py
--rw-r--r--   0 maurits    (501) staff       (20)      727 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/preview.py
--rw-r--r--   0 maurits    (501) staff       (20)     2475 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/behaviors/preview_link.py
--rw-r--r--   0 maurits    (501) staff       (20)     1614 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/blocksuuidfixer.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.847499 plone.volto-4.0.8/src/plone/volto/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2046 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/breadcrumbs.py
--rw-r--r--   0 maurits    (501) staff       (20)     1743 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3673 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/migrate_richtext.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5548 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/migrate_richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     6692 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/migrate_to_volto.pt
--rw-r--r--   0 maurits    (501) staff       (20)    13972 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/migrate_to_volto.py
--rw-r--r--   0 maurits    (501) staff       (20)     4499 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/navigation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.847782 plone.volto-4.0.8/src/plone/volto/browser/static/
--rw-r--r--   0 maurits    (501) staff       (20)      754 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/static/volto.svg
--rw-r--r--   0 maurits    (501) staff       (20)     1368 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/browser/voltobackendwarning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3273 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      697 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/content.py
--rw-r--r--   0 maurits    (501) staff       (20)      974 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/controlpanel.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.848912 plone.volto-4.0.8/src/plone/volto/coresandbox/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/coresandbox/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      540 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/coresandbox/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    28820 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/coresandbox/example.py
--rw-r--r--   0 maurits    (501) staff       (20)      745 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/coresandbox/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.849444 plone.volto-4.0.8/src/plone/volto/cors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/cors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      462 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/cors/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.850896 plone.volto-4.0.8/src/plone/volto/default_homepage/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/default_homepage/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    34756 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/default_homepage/default.py
--rw-r--r--   0 maurits    (501) staff       (20)    28345 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/default_homepage/demo.py
--rw-r--r--   0 maurits    (501) staff       (20)     3019 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/default_homepage/lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      516 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/dependencies.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1062 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1006 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1576 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/linkintegrity.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.851482 plone.volto-4.0.8/src/plone/volto/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.826884 plone.volto-4.0.8/src/plone/volto/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.852096 plone.volto-4.0.8/src/plone/volto/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2258 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4528 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.827181 plone.volto-4.0.8/src/plone/volto/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.852703 plone.volto-4.0.8/src/plone/volto/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      622 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.827464 plone.volto-4.0.8/src/plone/volto/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.853302 plone.volto-4.0.8/src/plone/volto/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2559 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4693 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.827750 plone.volto-4.0.8/src/plone/volto/locales/eu/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.853907 plone.volto-4.0.8/src/plone/volto/locales/eu/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     2478 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4611 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.828041 plone.volto-4.0.8/src/plone/volto/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.854534 plone.volto-4.0.8/src/plone/volto/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1145 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
--rw-r--r--   0 maurits    (501) staff       (20)     4086 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
--rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/plone.volto.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)      502 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/locales/update.sh
--rw-r--r--   0 maurits    (501) staff       (20)      256 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/patches.py
--rw-r--r--   0 maurits    (501) staff       (20)      858 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/patches.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.829747 plone.volto-4.0.8/src/plone/volto/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.855740 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/
--rw-r--r--   0 maurits    (501) staff       (20)      206 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/diff_tool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/repositorytool.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.856035 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2466 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/types/example.xml
--rw-r--r--   0 maurits    (501) staff       (20)      165 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.857822 plone.volto-4.0.8/src/plone/volto/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      156 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      196 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      612 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      181 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1791 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.859531 plone.volto-4.0.8/src/plone/volto/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      286 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      814 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      501 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      604 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/LRF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      464 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles/default/types/News_Item.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.860101 plone.volto-4.0.8/src/plone/volto/profiles/demo/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/demo/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      291 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/demo/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.860374 plone.volto-4.0.8/src/plone/volto/profiles/homepage/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/homepage/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.860929 plone.volto-4.0.8/src/plone/volto/profiles/multilingual/
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/multilingual/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      546 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/multilingual/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.861487 plone.volto-4.0.8/src/plone/volto/profiles/richtext/
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/richtext/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.861742 plone.volto-4.0.8/src/plone/volto/profiles/richtext/types/
--rw-r--r--   0 maurits    (501) staff       (20)      320 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/richtext/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/richtext/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.861997 plone.volto-4.0.8/src/plone/volto/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3591 2023-03-23 11:58:18.000000 plone.volto-4.0.8/src/plone/volto/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3436 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scaling.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.864051 plone.volto-4.0.8/src/plone/volto/scripts/
--rw-r--r--   0 maurits    (501) staff       (20)      752 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/add_image_field_metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     1206 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/auditblocks.py
--rw-r--r--   0 maurits    (501) staff       (20)      202 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/clear-rebuild-catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      773 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/listingaddsummary.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/migrate_richtext.py
--rwxr-xr-x   0 maurits    (501) staff       (20)      123 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/packdb.py
--rw-r--r--   0 maurits    (501) staff       (20)     1594 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/searchscalesinimageblocks.py
--rw-r--r--   0 maurits    (501) staff       (20)      932 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/scripts/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     9939 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      312 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     4513 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.867355 plone.volto-4.0.8/src/plone/volto/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_coresandbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     2442 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_linkintegrity.py
--rw-r--r--   0 maurits    (501) staff       (20)    11813 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_migrate_to_volto.py
--rw-r--r--   0 maurits    (501) staff       (20)     1823 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_preview_link_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2126 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_scripts.py
--rw-r--r--   0 maurits    (501) staff       (20)     3102 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1709 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_summary_serialization.py
--rw-r--r--   0 maurits    (501) staff       (20)    11245 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     6498 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/tests/test_upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     4805 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)     5327 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     2222 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.868088 plone.volto-4.0.8/src/plone/volto/vocabularies/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/vocabularies/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      105 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/vocabularies/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4305 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone/volto/vocabularies/subject.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:58:19.837380 plone.volto-4.0.8/src/plone.volto.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25931 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5012 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-23 11:58:19.000000 plone.volto-4.0.8/src/plone.volto.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.142418 plone.volto-4.0.9/
+-rw-r--r--   0 maurits    (501) staff       (20)    13945 2023-06-22 19:24:02.000000 plone.volto-4.0.9/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2023-06-22 19:24:02.000000 plone.volto-4.0.9/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    26169 2023-06-22 19:24:03.142043 plone.volto-4.0.9/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    10929 2023-06-22 19:24:02.000000 plone.volto-4.0.9/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.109167 plone.volto-4.0.9/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      657 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       74 2023-06-22 19:24:02.000000 plone.volto-4.0.9/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      881 2023-06-22 19:24:02.000000 plone.volto-4.0.9/pyproject.toml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.110174 plone.volto-4.0.9/requirements/
+-rw-r--r--   0 maurits    (501) staff       (20)       12 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/dev.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/plone-5.2.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       69 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/plone-6.0.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements/prod.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      402 2023-06-22 19:24:02.000000 plone.volto-4.0.9/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-22 19:24:03.142554 plone.volto-4.0.9/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2227 2023-06-22 19:24:02.000000 plone.volto-4.0.9/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.102243 plone.volto-4.0.9/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.110418 plone.volto-4.0.9/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.117643 plone.volto-4.0.9/src/plone/volto/
+-rw-r--r--   0 maurits    (501) staff       (20)      222 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.119151 plone.volto-4.0.9/src/plone/volto/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      534 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/headtitle.py
+-rw-r--r--   0 maurits    (501) staff       (20)      345 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/navtitle.py
+-rw-r--r--   0 maurits    (501) staff       (20)      727 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/preview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2475 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/behaviors/preview_link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1614 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/blocksuuidfixer.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.121590 plone.volto-4.0.9/src/plone/volto/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2046 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/breadcrumbs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1743 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3673 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5548 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6949 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14011 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4499 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/navigation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.121965 plone.volto-4.0.9/src/plone/volto/browser/static/
+-rw-r--r--   0 maurits    (501) staff       (20)      754 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/static/volto.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     1368 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/browser/voltobackendwarning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3273 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      697 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      974 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/controlpanel.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.123098 plone.volto-4.0.9/src/plone/volto/coresandbox/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    28820 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)      745 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/coresandbox/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.123761 plone.volto-4.0.9/src/plone/volto/cors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/cors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      462 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/cors/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.124975 plone.volto-4.0.9/src/plone/volto/default_homepage/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34756 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/default.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28345 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/demo.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3019 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/default_homepage/lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      516 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/dependencies.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1062 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1006 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1576 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/linkintegrity.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.125501 plone.volto-4.0.9/src/plone/volto/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.103599 plone.volto-4.0.9/src/plone/volto/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.126108 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2258 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4528 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.103885 plone.volto-4.0.9/src/plone/volto/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.126623 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      622 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104121 plone.volto-4.0.9/src/plone/volto/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.127215 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2559 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4693 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104357 plone.volto-4.0.9/src/plone/volto/locales/eu/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.127694 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2478 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4611 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.104593 plone.volto-4.0.9/src/plone/volto/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.128242 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1145 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4086 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
+-rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/plone.volto.pot
+-rwxr-xr-x   0 maurits    (501) staff       (20)      502 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/locales/update.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      256 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/patches.py
+-rw-r--r--   0 maurits    (501) staff       (20)      858 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/patches.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.106045 plone.volto-4.0.9/src/plone/volto/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.129223 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/
+-rw-r--r--   0 maurits    (501) staff       (20)      206 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/diff_tool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      210 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/repositorytool.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.129553 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2466 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/example.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.131171 plone.volto-4.0.9/src/plone/volto/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      156 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      196 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      612 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1791 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.132856 plone.volto-4.0.9/src/plone/volto/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      286 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      814 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      604 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/LRF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      464 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/default/types/News_Item.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.133520 plone.volto-4.0.9/src/plone/volto/profiles/demo/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/demo/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/demo/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.133765 plone.volto-4.0.9/src/plone/volto/profiles/homepage/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/homepage/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.134251 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      546 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/multilingual/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.134927 plone.volto-4.0.9/src/plone/volto/profiles/richtext/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.135169 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      320 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/richtext/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.135416 plone.volto-4.0.9/src/plone/volto/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3591 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3436 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scaling.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.137688 plone.volto-4.0.9/src/plone/volto/scripts/
+-rw-r--r--   0 maurits    (501) staff       (20)      752 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/add_image_field_metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1206 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/auditblocks.py
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/clear-rebuild-catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      773 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/listingaddsummary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/migrate_richtext.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)      123 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/packdb.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1594 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/searchscalesinimageblocks.py
+-rw-r--r--   0 maurits    (501) staff       (20)      932 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/scripts/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9939 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      312 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4513 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.140586 plone.volto-4.0.9/src/plone/volto/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_coresandbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2442 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_linkintegrity.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11771 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_migrate_to_volto.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1823 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_preview_link_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2126 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_scripts.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3102 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1709 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_summary_serialization.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11245 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6498 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/tests/test_upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4805 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5327 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2222 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/upgrades.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.141649 plone.volto-4.0.9/src/plone/volto/vocabularies/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4305 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone/volto/vocabularies/subject.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:24:03.112559 plone.volto-4.0.9/src/plone.volto.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    26169 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5012 2023-06-22 19:24:03.000000 plone.volto-4.0.9/src/plone.volto.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:24:02.000000 plone.volto-4.0.9/src/plone.volto.egg-info/top_level.txt
```

### Comparing `plone.volto-4.0.8/CHANGES.rst` & `plone.volto-4.0.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.9 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
+  [pbauer] (#122)
+- Fix value of unchecked checkboxes in migrate_to_volto.
+  [pbauer] (#124)
+
+
 4.0.8 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Use correct service_url when calling make_document. Fix #95
```

### Comparing `plone.volto-4.0.8/PKG-INFO` & `plone.volto-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.0.8
+Version: 4.0.9
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -322,14 +322,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.9 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
+  [pbauer] (#122)
+- Fix value of unchecked checkboxes in migrate_to_volto.
+  [pbauer] (#124)
+
+
 4.0.8 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Use correct service_url when calling make_document. Fix #95
```

### Comparing `plone.volto-4.0.8/README.rst` & `plone.volto-4.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/docs/LICENSE.GPL` & `plone.volto-4.0.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/docs/LICENSE.rst` & `plone.volto-4.0.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/pyproject.toml` & `plone.volto-4.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/setup.py` & `plone.volto-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         readfile("CONTRIBUTORS.rst"),
         readfile("CHANGES.rst"),
     ]
 )
 
 setup(
     name="plone.volto",
-    version="4.0.8",
+    version="4.0.9",
     description="Volto integration add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.volto-4.0.8/src/plone/volto/behaviors/configure.zcml` & `plone.volto-4.0.9/src/plone/volto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/behaviors/headtitle.py` & `plone.volto-4.0.9/src/plone/volto/behaviors/headtitle.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/behaviors/preview.py` & `plone.volto-4.0.9/src/plone/volto/behaviors/preview.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/behaviors/preview_link.py` & `plone.volto-4.0.9/src/plone/volto/behaviors/preview_link.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/blocksuuidfixer.py` & `plone.volto-4.0.9/src/plone/volto/blocksuuidfixer.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/breadcrumbs.py` & `plone.volto-4.0.9/src/plone/volto/browser/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/configure.zcml` & `plone.volto-4.0.9/src/plone/volto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/migrate_richtext.pt` & `plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/migrate_richtext.py` & `plone.volto-4.0.9/src/plone/volto/browser/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/migrate_to_volto.pt` & `plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.pt`

 * *Files 18% similar despite different names*

```diff
@@ -51,27 +51,29 @@
 
         <h3 i18n:translate="">Advanced settings</h3>
         <p i18n:translate="">
         It is recommendet to use the default settings but here you can disable some of the migration-steps.
         </p>
 
         <div class="form-check mb-3">
+            <input name="migrate_folders:boolean:default" type="hidden" value="" />
             <input
                 class="form-check-input"
                 type="checkbox"
                 name="migrate_folders:boolean"
                 id="migrate_folders"
                 tal:attributes="checked python:view.migrate_folders"
                 />
             <label class="form-check-label" for="migrate_folders">
             Migrate Folders to Folderish Pages
             </label>
         </div>
 
         <div class="form-check mb-3 ms-4">
+            <input name="migrate_default_pages:boolean:default" type="hidden" value="" />
             <input
                 class="form-check-input"
                 type="checkbox"
                 name="migrate_default_pages:boolean"
                 id="migrate_default_pages"
                 tal:attributes="checked python:view.migrate_default_pages"
                 />
@@ -82,14 +84,15 @@
             Collections and Pages that are the default-page of a Folder will be applied on the migrated Folderish Page.
             For Collections that means adding a listing block with the same query.
             This only happens if you also you migrate Folders to Folderish Pages.
             </div>
         </div>
 
         <div class="form-check mb-3">
+            <input name="purge_richtext:boolean:default" type="hidden" value="" />
             <input
                 class="form-check-input"
                 type="checkbox"
                 name="purge_richtext:boolean"
                 id="purge_richtext"
                 tal:attributes="checked python:view.purge_richtext"
                 />
```

#### html2text {}

```diff
@@ -34,20 +34,20 @@
       tool running on an accessible URL. The easiest way to have that running
       on your machine is: docker run -it -p 5000:5000 plone/blocks-conversion-
       tool:latest. More for options read https://github.com/plone/blocks-
       conversion-tool.
 **** Advanced settings ****
 It is recommendet to use the default settings but here you can disable some of
 the migration-steps.
-⁰  Migrate Folders to Folderish Pages
-⁰  Migrate default Pages into the Folderish Pages if possible
+ ⁰  Migrate Folders to Folderish Pages
+ ⁰  Migrate default Pages into the Folderish Pages if possible
 Collections and Pages that are the default-page of a Folder will be applied on
 the migrated Folderish Page. For Collections that means adding a listing block
 with the same query. This only happens if you also you migrate Folders to
 Folderish Pages.
-⁰  Purge old Richtext-fields after migrating to Volto blocks
+ ⁰  Purge old Richtext-fields after migrating to Volto blocks
 The RichtextValue objects will be removed from the migrated objects. The old
 fields (from the behavior plone.volto) are no longer available.
  URL of blocks-conversion-tool.  [service_url         ]
 The migration requires a service to run. See https://github.com/plone/blocks-
 conversion-tool for details.
  Migrate to Volto
```

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/migrate_to_volto.py` & `plone.volto-4.0.9/src/plone/volto/browser/migrate_to_volto.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
     def __call__(self):
         request = self.request
         self.service_url = request.get("service_url", "http://localhost:5000/html")
         self.migrate_folders = request.get("migrate_folders", True)
         self.migrate_default_pages = request.get("migrate_default_pages", True)
         self.purge_richtext = request.get("purge_richtext", True)
-        # We still use draftjs at the moment
-        self.slate = request.get("slate", False)
+        # We can still use outdated draftjs by setting slate to False on the request
+        self.slate = request.get("slate", True)
 
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         # 1. Install plone volto to enable plone.blocks behavior and change klass on fti
         self.install_plone_volto()
```

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/navigation.py` & `plone.volto-4.0.9/src/plone/volto/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/static/volto.svg` & `plone.volto-4.0.9/src/plone/volto/browser/static/volto.svg`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/browser/voltobackendwarning.pt` & `plone.volto-4.0.9/src/plone/volto/browser/voltobackendwarning.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/configure.zcml` & `plone.volto-4.0.9/src/plone/volto/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/content.py` & `plone.volto-4.0.9/src/plone/volto/content.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/controlpanel.py` & `plone.volto-4.0.9/src/plone/volto/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/coresandbox/configure.zcml` & `plone.volto-4.0.9/src/plone/volto/coresandbox/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/coresandbox/example.py` & `plone.volto-4.0.9/src/plone/volto/coresandbox/example.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/coresandbox/vocabularies.py` & `plone.volto-4.0.9/src/plone/volto/coresandbox/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/default_homepage/default.py` & `plone.volto-4.0.9/src/plone/volto/default_homepage/default.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/default_homepage/demo.py` & `plone.volto-4.0.9/src/plone/volto/default_homepage/demo.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/default_homepage/lrf.py` & `plone.volto-4.0.9/src/plone/volto/default_homepage/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/dependencies.zcml` & `plone.volto-4.0.9/src/plone/volto/dependencies.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/indexers.py` & `plone.volto-4.0.9/src/plone/volto/indexers.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/interfaces.py` & `plone.volto-4.0.9/src/plone/volto/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/linkintegrity.py` & `plone.volto-4.0.9/src/plone/volto/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo` & `plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po` & `plone.volto-4.0.9/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo` & `plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po` & `plone.volto-4.0.9/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo` & `plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po` & `plone.volto-4.0.9/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo` & `plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po` & `plone.volto-4.0.9/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo` & `plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po` & `plone.volto-4.0.9/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/locales/plone.volto.pot` & `plone.volto-4.0.9/src/plone/volto/locales/plone.volto.pot`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/patches.py` & `plone.volto-4.0.9/src/plone/volto/patches.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/patches.zcml` & `plone.volto-4.0.9/src/plone/volto/patches.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/coresandbox/types/example.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/coresandbox/types/example.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/default/actions.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/default/controlpanel.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/default/registry.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/default/types/Document.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/default/types/LRF.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/default/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles/multilingual/registry.xml` & `plone.volto-4.0.9/src/plone/volto/profiles/multilingual/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/profiles.zcml` & `plone.volto-4.0.9/src/plone/volto/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scaling.py` & `plone.volto-4.0.9/src/plone/volto/scaling.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/add_image_field_metadata.py` & `plone.volto-4.0.9/src/plone/volto/scripts/add_image_field_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/auditblocks.py` & `plone.volto-4.0.9/src/plone/volto/scripts/auditblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/listingaddsummary.py` & `plone.volto-4.0.9/src/plone/volto/scripts/listingaddsummary.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/migrate_richtext.py` & `plone.volto-4.0.9/src/plone/volto/scripts/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/searchscalesinimageblocks.py` & `plone.volto-4.0.9/src/plone/volto/scripts/searchscalesinimageblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/scripts/utils.py` & `plone.volto-4.0.9/src/plone/volto/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/setuphandlers.py` & `plone.volto-4.0.9/src/plone/volto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/testing.py` & `plone.volto-4.0.9/src/plone/volto/testing.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_coresandbox.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_coresandbox.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_linkintegrity.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_migrate_to_volto.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_migrate_to_volto.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,14 @@
             title="Document",
             text=RichTextValue(html, "text/plain", "text/html"),
         )
         self.assertTrue(isinstance(doc.text, RichTextValue))
 
         view = self.portal.restrictedTraverse("@@migrate_to_volto")
         self.request.form["form.submitted"] = True
-        self.request.form["slate"] = True
         view()
 
         doc = self.portal["doc"]
         self.assertIsNone(doc.text)
         uuid = doc.blocks_layout["items"][1]
         block = doc.blocks[uuid]
         self.assertEqual(block["plaintext"], "I am html text")
```

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_preview_link_behavior.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_preview_link_behavior.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_scripts.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_setup.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_summary_serialization.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_summary_serialization.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_transforms.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/tests/test_upgrades.py` & `plone.volto-4.0.9/src/plone/volto/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/transforms.py` & `plone.volto-4.0.9/src/plone/volto/transforms.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/upgrades.py` & `plone.volto-4.0.9/src/plone/volto/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/upgrades.zcml` & `plone.volto-4.0.9/src/plone/volto/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone/volto/vocabularies/subject.py` & `plone.volto-4.0.9/src/plone/volto/vocabularies/subject.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.0.8/src/plone.volto.egg-info/PKG-INFO` & `plone.volto-4.0.9/src/plone.volto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.0.8
+Version: 4.0.9
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -322,14 +322,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.9 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Let the migration-form @@migrate_to_volto transform richtext to slate-blocks by default.
+  [pbauer] (#122)
+- Fix value of unchecked checkboxes in migrate_to_volto.
+  [pbauer] (#124)
+
+
 4.0.8 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Use correct service_url when calling make_document. Fix #95
```

### Comparing `plone.volto-4.0.8/src/plone.volto.egg-info/SOURCES.txt` & `plone.volto-4.0.9/src/plone.volto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

