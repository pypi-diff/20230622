# Comparing `tmp/aa-simplewiki-1.0.2.tar.gz` & `tmp/aa-simplewiki-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-1.0.2.tar", last modified: Mon Jun 12 04:03:55 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.3.tar", last modified: Thu Jun 22 13:24:11 2023, max compression
```

## Comparing `aa-simplewiki-1.0.2.tar` & `aa-simplewiki-1.0.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-12 03:50:34.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-06-12 04:03:55.413730 aa-simplewiki-1.0.2/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1205 2023-06-12 03:50:11.000000 aa-simplewiki-1.0.2/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-12 03:51:40.000000 aa-simplewiki-1.0.2/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-12 03:28:56.000000 aa-simplewiki-1.0.2/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-12 03:43:22.000000 aa-simplewiki-1.0.2/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12859 2023-06-12 03:44:46.000000 aa-simplewiki-1.0.2/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.868511 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1206 2023-06-22 13:22:42.000000 aa-simplewiki-1.0.3/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.868511 aa-simplewiki-1.0.3/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-22 13:23:52.000000 aa-simplewiki-1.0.3/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.876514 aa-simplewiki-1.0.3/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.864510 aa-simplewiki-1.0.3/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.876514 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.864510 aa-simplewiki-1.0.3/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_sections.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12930 2023-06-22 11:57:18.000000 aa-simplewiki-1.0.3/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/wsgi.py
```

### Comparing `aa-simplewiki-1.0.2/LICENSE` & `aa-simplewiki-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/PKG-INFO` & `aa-simplewiki-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.2/README.md` & `aa-simplewiki-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.3/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.2/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.3/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/setup.cfg` & `aa-simplewiki-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/setup.py` & `aa-simplewiki-1.0.3/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
-)
+)
```

### Comparing `aa-simplewiki-1.0.2/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.3/simplewiki/admin_helper_menus.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.3/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.3/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.3/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/models.py` & `aa-simplewiki-1.0.3/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.3/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/simplewiki/views.py` & `aa-simplewiki-1.0.3/simplewiki/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,23 +157,24 @@
         group_names = requested_menu.groups.split(',')
     except Exception as e:
         group_names = ""
 
     context.update({'group_names': group_names})
 
     #if not requested_menu.groups or requested_menu.groups in list(request.user.groups.values_list('name', flat=True)):
-    if any(group_name in request.user.groups.values_list('name', flat=True) for group_name in group_names) or any(element == "none" for element in group_names):
+    if any(group_name in request.user.groups.values_list('name', flat=True) for group_name in group_names) or any(element == "none" or not element for element in group_names):
         return render(request, 'simplewiki/dynamic_page.html', context)
     else:
         # If more then two groups are required
         if len(requested_menu.groups.split(',')) > 1:
             group_plural = "groups"
         else:
             group_plural = "group"
         context.update({'error_code': '#1001'})
+        print(requested_menu.groups.replace(',', ', '))
         error_message = "You don\'t have the permissions to access this page. You need to be in the <b>" + requested_menu.groups.replace(',', ', ') + "</b> " + group_plural + " on auth."
         context.update({'error_msg': error_message})
         return render(request, 'simplewiki/error.html', context)
 
 @login_required
 @permission_required("simplewiki.basic_access") 
 def search(request: WSGIRequest) -> HttpResponse:
```

### Comparing `aa-simplewiki-1.0.2/testauth/celery.py` & `aa-simplewiki-1.0.3/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.2/testauth/settings.py` & `aa-simplewiki-1.0.3/testauth/settings.py`

 * *Files identical despite different names*

