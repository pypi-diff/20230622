# Comparing `tmp/plone.app.layout-4.0.5.tar.gz` & `tmp/plone.app.layout-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.layout-4.0.5.tar", last modified: Mon May 22 17:51:06 2023, max compression
+gzip compressed data, was "plone.app.layout-4.0.6.tar", last modified: Thu Jun 22 19:14:46 2023, max compression
```

## Comparing `plone.app.layout-4.0.5.tar` & `plone.app.layout-4.0.6.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.809621 plone.app.layout-4.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    62066 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    63734 2023-05-22 17:51:06.809771 plone.app.layout-4.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      740 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.777106 plone.app.layout-4.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.777361 plone.app.layout-4.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.779940 plone.app.layout-4.0.5/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.781209 plone.app.layout-4.0.5/plone/app/layout/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.782260 plone.app.layout-4.0.5/plone/app/layout/analytics/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      322 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.783053 plone.app.layout-4.0.5/plone/app/layout/analytics/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/tests/analytics.txt
--rw-r--r--   0 maurits    (501) staff       (20)      637 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1024 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/analytics/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      550 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.783750 plone.app.layout-4.0.5/plone/app/layout/dashboard/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/dashboard/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      100 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/dashboard/dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/dashboard/user_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      885 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/favicon_handler.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.785784 plone.app.layout-4.0.5/plone/app/layout/globals/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9179 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/context.py
--rw-r--r--   0 maurits    (501) staff       (20)     4098 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     6502 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    12280 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.787267 plone.app.layout-4.0.5/plone/app/layout/globals/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.787515 plone.app.layout-4.0.5/plone/app/layout/globals/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)       30 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10563 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     3885 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     8497 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     6324 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_tools.py
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/globals/tools.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.788454 plone.app.layout-4.0.5/plone/app/layout/icons/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/icons/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1553 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/icons/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5639 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/icons/icons.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/icons/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.790158 plone.app.layout-4.0.5/plone/app/layout/links/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/author.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1166 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      284 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/favicon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/rsslink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      363 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/search.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.791448 plone.app.layout-4.0.5/plone/app/layout/links/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      803 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/tests/test_canonical_url.py
--rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/tests/test_favicon_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1402 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/tests/test_rssviewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     7019 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/links/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.792930 plone.app.layout-4.0.5/plone/app/layout/navigation/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/navigation/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/navigation/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/navigation/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    14357 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/navigation/navtree.py
--rw-r--r--   0 maurits    (501) staff       (20)      445 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/navigation/root.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.794708 plone.app.layout-4.0.5/plone/app/layout/nextprevious/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      989 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      909 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/links.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1673 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/nextprevious.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/nextprevious/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      323 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.796043 plone.app.layout-4.0.5/plone/app/layout/sitemap/
--rw-r--r--   0 maurits    (501) staff       (20)      159 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      301 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4491 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)      820 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/sitemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.796555 plone.app.layout-4.0.5/plone/app/layout/sitemap/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11362 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/sitemap/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.807277 plone.app.layout-4.0.5/plone/app/layout/viewlets/
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      409 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/anontools.pt
--rw-r--r--   0 maurits    (501) staff       (20)      445 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)    20134 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    10329 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18430 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     6137 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)      782 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/contentviews.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1239 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/document_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/document_byline.pt
--rw-r--r--   0 maurits    (501) staff       (20)      980 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/document_contributors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1833 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/document_relateditems.pt
--rw-r--r--   0 maurits    (501) staff       (20)      375 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/document_rights.pt
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/dublin_core.pt
--rw-r--r--   0 maurits    (501) staff       (20)      793 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/globalstatusmessage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1579 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/globalstatusmessage.py
--rw-r--r--   0 maurits    (501) staff       (20)      620 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/history_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      953 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/httpheaders.py
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/keywords.pt
--rw-r--r--   0 maurits    (501) staff       (20)      361 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/membertools.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/menu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      811 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/path_bar.pt
--rw-r--r--   0 maurits    (501) staff       (20)      515 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/popup_content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3320 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/review_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1621 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/searchbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/sections.pt
--rw-r--r--   0 maurits    (501) staff       (20)      552 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/site_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5451 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/social.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/social_tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)      294 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/social_tags_body.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.809404 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      665 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2621 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/history.txt
--rw-r--r--   0 maurits    (501) staff       (20)    27962 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_common.py
--rw-r--r--   0 maurits    (501) staff       (20)    14111 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)      590 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5391 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_social.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/tiny_logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)       66 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)      382 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/toc.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2517 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/toolbar.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1779 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/toolbar.py
--rw-r--r--   0 maurits    (501) staff       (20)       79 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone/app/layout/viewlets/viewport.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:51:06.779660 plone.app.layout-4.0.5/plone.app.layout.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    63734 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4931 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      463 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/plone.app.layout.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 17:51:06.810277 plone.app.layout-4.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2159 2023-05-22 17:51:06.000000 plone.app.layout-4.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:46.011426 plone.app.layout-4.0.6/
+-rw-r--r--   0 maurits    (501) staff       (20)    62177 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    63845 2023-06-22 19:14:46.011799 plone.app.layout-4.0.6/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.977452 plone.app.layout-4.0.6/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.977690 plone.app.layout-4.0.6/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.980486 plone.app.layout-4.0.6/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.981783 plone.app.layout-4.0.6/plone/app/layout/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.982884 plone.app.layout-4.0.6/plone/app/layout/analytics/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      322 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.983715 plone.app.layout-4.0.6/plone/app/layout/analytics/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/tests/analytics.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1024 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/analytics/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.984398 plone.app.layout-4.0.6/plone/app/layout/dashboard/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/dashboard/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      100 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/dashboard/dashboard.py
+-rw-r--r--   0 maurits    (501) staff       (20)      103 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/dashboard/user_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      885 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/favicon_handler.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.986537 plone.app.layout-4.0.6/plone/app/layout/globals/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9179 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4098 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6502 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12280 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.988167 plone.app.layout-4.0.6/plone/app/layout/globals/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.988466 plone.app.layout-4.0.6/plone/app/layout/globals/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10563 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3885 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8497 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6324 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_tools.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/globals/tools.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.989609 plone.app.layout-4.0.6/plone/app/layout/icons/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/icons/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1553 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/icons/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5639 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/icons/icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/icons/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.991387 plone.app.layout-4.0.6/plone/app/layout/links/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/author.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1166 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      284 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/favicon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/rsslink.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/search.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.992523 plone.app.layout-4.0.6/plone/app/layout/links/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      803 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/tests/test_canonical_url.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/tests/test_favicon_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1402 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/tests/test_rssviewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7019 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/links/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.994067 plone.app.layout-4.0.6/plone/app/layout/navigation/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/navigation/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/navigation/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/navigation/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14357 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/navigation/navtree.py
+-rw-r--r--   0 maurits    (501) staff       (20)      445 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/navigation/root.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.995806 plone.app.layout-4.0.6/plone/app/layout/nextprevious/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      989 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/links.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1673 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/nextprevious.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/nextprevious/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      323 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.997161 plone.app.layout-4.0.6/plone/app/layout/sitemap/
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4491 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/sitemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.997655 plone.app.layout-4.0.6/plone/app/layout/sitemap/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11362 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/sitemap/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:46.008948 plone.app.layout-4.0.6/plone/app/layout/viewlets/
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/anontools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      432 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    20134 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10329 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18430 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6137 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      782 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/contentviews.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/default_page_warning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1239 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/document_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/document_byline.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/document_contributors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1833 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/document_relateditems.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      375 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/document_rights.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/dublin_core.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/globalstatusmessage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1579 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/globalstatusmessage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      620 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/history_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      953 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/httpheaders.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/keywords.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      361 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/membertools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/menu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      811 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/path_bar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      515 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/popup_content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3320 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/review_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1621 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/searchbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/sections.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      552 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/site_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5451 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/social.py
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/social_tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/social_tags_body.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:46.011216 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      665 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2621 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/history.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    27962 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14111 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      590 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5391 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_social.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/tiny_logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       66 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      382 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/toc.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2517 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/toolbar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1779 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/toolbar.py
+-rw-r--r--   0 maurits    (501) staff       (20)       79 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone/app/layout/viewlets/viewport.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:14:45.980125 plone.app.layout-4.0.6/plone.app.layout.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    63845 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4931 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      463 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/plone.app.layout.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-06-22 19:14:46.012650 plone.app.layout-4.0.6/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2159 2023-06-22 19:14:45.000000 plone.app.layout-4.0.6/setup.py
```

### Comparing `plone.app.layout-4.0.5/CHANGES.rst` & `plone.app.layout-4.0.6/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Unify default values for translations
+  [erral] (#347)
+
+
 4.0.5 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Deprecate moved `getNavigationRoot` and `getNavigationRootObject` in `plone.app.layout.navigation.root`.
```

### Comparing `plone.app.layout-4.0.5/PKG-INFO` & `plone.app.layout-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.5
+Version: 4.0.6
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Unify default values for translations
+  [erral] (#347)
+
+
 4.0.5 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Deprecate moved `getNavigationRoot` and `getNavigationRootObject` in `plone.app.layout.navigation.root`.
```

### Comparing `plone.app.layout-4.0.5/README.rst` & `plone.app.layout-4.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/docs/LICENSE.GPL` & `plone.app.layout-4.0.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/docs/LICENSE.txt` & `plone.app.layout-4.0.6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/analytics/tests/analytics.txt` & `plone.app.layout-4.0.6/plone/app/layout/analytics/tests/analytics.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/analytics/tests/test_doctests.py` & `plone.app.layout-4.0.6/plone/app/layout/analytics/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/analytics/view.py` & `plone.app.layout-4.0.6/plone/app/layout/analytics/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/favicon_handler.py` & `plone.app.layout-4.0.6/plone/app/layout/favicon_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/globals/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/context.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/interface.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/interfaces.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/layout.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/portal.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_context.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_interface.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_layout.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_portal.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tests/test_tools.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/globals/tools.py` & `plone.app.layout-4.0.6/plone/app/layout/globals/tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/icons/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/icons/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/icons/icons.py` & `plone.app.layout-4.0.6/plone/app/layout/icons/icons.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/icons/interfaces.py` & `plone.app.layout-4.0.6/plone/app/layout/icons/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/author.pt` & `plone.app.layout-4.0.6/plone/app/layout/links/author.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/tests/test_canonical_url.py` & `plone.app.layout-4.0.6/plone/app/layout/links/tests/test_canonical_url.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/tests/test_favicon_viewlet.py` & `plone.app.layout-4.0.6/plone/app/layout/links/tests/test_favicon_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/tests/test_rssviewlet.py` & `plone.app.layout-4.0.6/plone/app/layout/links/tests/test_rssviewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/links/viewlets.py` & `plone.app.layout-4.0.6/plone/app/layout/links/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/navigation/interfaces.py` & `plone.app.layout-4.0.6/plone/app/layout/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/navigation/navtree.py` & `plone.app.layout-4.0.6/plone/app/layout/navigation/navtree.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/nextprevious/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/nextprevious/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/nextprevious/links.pt` & `plone.app.layout-4.0.6/plone/app/layout/nextprevious/links.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/nextprevious/nextprevious.pt` & `plone.app.layout-4.0.6/plone/app/layout/nextprevious/nextprevious.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/nextprevious/view.py` & `plone.app.layout-4.0.6/plone/app/layout/nextprevious/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/sitemap/sitemap.py` & `plone.app.layout-4.0.6/plone/app/layout/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/sitemap/sitemap.xml` & `plone.app.layout-4.0.6/plone/app/layout/sitemap/sitemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/sitemap/tests/test_sitemap.py` & `plone.app.layout-4.0.6/plone/app/layout/sitemap/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/testing.py` & `plone.app.layout-4.0.6/plone/app/layout/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/common.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/configure.zcml` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/content.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/content_history.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/contentviews.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/contentviews.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/default_page_warning.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/document_actions.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/document_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/document_byline.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/document_byline.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/document_contributors.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/document_contributors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/document_relateditems.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/document_relateditems.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/globalstatusmessage.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/globalstatusmessage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/globalstatusmessage.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/globalstatusmessage.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/history_view.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/history_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/httpheaders.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/httpheaders.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/interfaces.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/keywords.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/keywords.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/membertools.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/membertools.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/menu.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/menu.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/path_bar.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/path_bar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/popup_content_history.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/popup_content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/review_history.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/review_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/searchbox.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/searchbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/sections.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/sections.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/site_actions.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/site_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/social.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/base.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/history.txt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/history.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_common.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_content.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_functional.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_history.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/tests/test_social.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/toolbar.pt` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/toolbar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone/app/layout/viewlets/toolbar.py` & `plone.app.layout-4.0.6/plone/app/layout/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/plone.app.layout.egg-info/PKG-INFO` & `plone.app.layout-4.0.6/plone.app.layout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.5
+Version: 4.0.6
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Unify default values for translations
+  [erral] (#347)
+
+
 4.0.5 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Deprecate moved `getNavigationRoot` and `getNavigationRootObject` in `plone.app.layout.navigation.root`.
```

### Comparing `plone.app.layout-4.0.5/plone.app.layout.egg-info/SOURCES.txt` & `plone.app.layout-4.0.6/plone.app.layout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/pyproject.toml` & `plone.app.layout-4.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.5/setup.py` & `plone.app.layout-4.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.5"
+version = "4.0.6"
 
 long_description = open("README.rst").read() + "\n" + open("CHANGES.rst").read()
 
 setup(
     name="plone.app.layout",
     version=version,
     description="Layout mechanisms for Plone",
```

