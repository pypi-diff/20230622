# Comparing `tmp/plone.app.upgrade-3.0.5.tar.gz` & `tmp/plone.app.upgrade-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.upgrade-3.0.5.tar", last modified: Tue May 30 13:45:41 2023, max compression
+gzip compressed data, was "plone.app.upgrade-3.0.6.tar", last modified: Thu Jun 22 19:29:59 2023, max compression
```

## Comparing `plone.app.upgrade-3.0.5.tar` & `plone.app.upgrade-3.0.6.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.349414 plone.app.upgrade-3.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    10501 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    11787 2023-05-30 13:45:41.349558 plone.app.upgrade-3.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      351 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.326525 plone.app.upgrade-3.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.326896 plone.app.upgrade-3.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.329863 plone.app.upgrade-3.0.5/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.330847 plone.app.upgrade-3.0.5/plone/app/upgrade/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.331678 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/
--rw-r--r--   0 maurits    (501) staff       (20)      266 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/InstalledProduct.py
--rw-r--r--   0 maurits    (501) staff       (20)      784 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/QuickInstallerTool.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.332475 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)      158 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/interfaces/installable.py
--rw-r--r--   0 maurits    (501) staff       (20)      133 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/interfaces/portal_quickinstaller.py
--rw-r--r--   0 maurits    (501) staff       (20)      448 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.333536 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5732 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.333814 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/
--rw-r--r--   0 maurits    (501) staff       (20)       15 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.334173 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub1/
--rw-r--r--   0 maurits    (501) staff       (20)       21 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub1/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.334583 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub1/subsub1/
--rw-r--r--   0 maurits    (501) staff       (20)       25 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub1/subsub1/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.334846 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub2/
--rw-r--r--   0 maurits    (501) staff       (20)       21 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/skin_test/sub2/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2845 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/test_upgrade.py
--rw-r--r--   0 maurits    (501) staff       (20)     3624 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    15675 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.336776 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3740 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/alphas.py
--rw-r--r--   0 maurits    (501) staff       (20)     5567 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/betas.py
--rw-r--r--   0 maurits    (501) staff       (20)     6810 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    11549 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/final.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.321895 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.337047 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_521/
--rw-r--r--   0 maurits    (501) staff       (20)      268 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_521/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.321088 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_522/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.337619 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_522/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      348 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_522/registry/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_522/registry/image_captioning.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.338475 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/
--rw-r--r--   0 maurits    (501) staff       (20)     1639 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1337 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      554 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.340225 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      533 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2404 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1054 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      428 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/rolemap.xml
--rw-r--r--   0 maurits    (501) staff       (20)      187 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/toolset.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.321750 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc1/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.340533 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc1/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      329 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc1/registry/resources.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.321997 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc4/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.341055 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc4/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc4/registry/security.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1878 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    11140 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v52/tests.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.343166 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    15741 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/alphas.py
--rw-r--r--   0 maurits    (501) staff       (20)     4269 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/betas.py
--rw-r--r--   0 maurits    (501) staff       (20)     7188 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5643 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/final.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.323655 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.344621 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/
--rw-r--r--   0 maurits    (501) staff       (20)      387 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2067 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      611 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/toolset.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.345547 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6003/
--rw-r--r--   0 maurits    (501) staff       (20)      507 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6003/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6003/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.346951 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/
--rw-r--r--   0 maurits    (501) staff       (20)      435 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2553 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      291 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.347367 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/types/
--rw-r--r--   0 maurits    (501) staff       (20)      267 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.347934 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6005/
--rw-r--r--   0 maurits    (501) staff       (20)      575 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6005/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6005/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.348209 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6007/
--rw-r--r--   0 maurits    (501) staff       (20)     4558 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6007/actions.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.348560 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6012/
--rw-r--r--   0 maurits    (501) staff       (20)      234 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6012/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.348891 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to_dx_site_root/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.349156 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to_dx_site_root/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2782 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to_dx_site_root/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2248 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6695 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/plone/app/upgrade/v60/tests.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-30 13:45:41.329571 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    11787 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3449 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      318 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-30 13:45:41.000000 plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      116 2023-05-30 13:45:41.350027 plone.app.upgrade-3.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1967 2023-05-30 13:45:40.000000 plone.app.upgrade-3.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.047376 plone.app.upgrade-3.0.6/
+-rw-r--r--   0 maurits    (501) staff       (20)    10612 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    11898 2023-06-22 19:29:59.047516 plone.app.upgrade-3.0.6/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      351 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.025117 plone.app.upgrade-3.0.6/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.025458 plone.app.upgrade-3.0.6/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.028068 plone.app.upgrade-3.0.6/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.028842 plone.app.upgrade-3.0.6/plone/app/upgrade/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.029741 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/
+-rw-r--r--   0 maurits    (501) staff       (20)      266 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/InstalledProduct.py
+-rw-r--r--   0 maurits    (501) staff       (20)      784 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/QuickInstallerTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.030760 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      215 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/interfaces/installable.py
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/interfaces/portal_quickinstaller.py
+-rw-r--r--   0 maurits    (501) staff       (20)      448 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.031815 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5732 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.032093 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/
+-rw-r--r--   0 maurits    (501) staff       (20)       15 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.032347 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub1/
+-rw-r--r--   0 maurits    (501) staff       (20)       21 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub1/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.032600 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub1/subsub1/
+-rw-r--r--   0 maurits    (501) staff       (20)       25 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub1/subsub1/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.032914 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub2/
+-rw-r--r--   0 maurits    (501) staff       (20)       21 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/skin_test/sub2/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2845 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/test_upgrade.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3624 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15675 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.034736 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3740 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/alphas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5567 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/betas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6810 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    11549 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/final.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.020928 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.034998 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_521/
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_521/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.020266 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_522/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.035519 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_522/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_522/registry/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_522/registry/image_captioning.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.036346 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1639 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1337 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      554 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.038480 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      533 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2404 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1054 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      428 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/rolemap.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/toolset.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.020790 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc1/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.038984 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc1/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      329 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc1/registry/resources.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.021027 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc4/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.039614 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc4/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc4/registry/security.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1878 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    11140 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v52/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.042078 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15741 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/alphas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4269 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/betas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7486 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5643 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/final.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.022412 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.043336 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/
+-rw-r--r--   0 maurits    (501) staff       (20)      387 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2067 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      611 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/toolset.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.043854 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6003/
+-rw-r--r--   0 maurits    (501) staff       (20)      507 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6003/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6003/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.044964 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/
+-rw-r--r--   0 maurits    (501) staff       (20)      435 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2553 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.045282 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      267 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.045868 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6005/
+-rw-r--r--   0 maurits    (501) staff       (20)      575 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6005/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6005/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.046149 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6007/
+-rw-r--r--   0 maurits    (501) staff       (20)     4558 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6007/actions.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.046431 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6012/
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6012/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.046744 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to_dx_site_root/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.047160 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to_dx_site_root/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2782 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to_dx_site_root/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2248 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6695 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone/app/upgrade/v60/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:29:59.027789 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    11898 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3449 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      318 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2023-06-22 19:29:59.047989 plone.app.upgrade-3.0.6/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1967 2023-06-22 19:29:58.000000 plone.app.upgrade-3.0.6/setup.py
```

### Comparing `plone.app.upgrade-3.0.5/CHANGES.rst` & `plone.app.upgrade-3.0.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Added upgrade to 6017, Plone 6.0.6.  [maurits] (#6017)
+
+
 3.0.5 (2023-05-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix TinyMCE problem: Tools and View do not show up in menubar.
```

### Comparing `plone.app.upgrade-3.0.5/PKG-INFO` & `plone.app.upgrade-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.upgrade
-Version: 3.0.5
+Version: 3.0.6
 Summary: Upgrade machinery for Plone.
 Home-page: https://pypi.org/project/plone.app.upgrade/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone upgrade migration
 Classifier: Development Status :: 6 - Mature
@@ -41,14 +41,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Added upgrade to 6017, Plone 6.0.6.  [maurits] (#6017)
+
+
 3.0.5 (2023-05-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix TinyMCE problem: Tools and View do not show up in menubar.
```

### Comparing `plone.app.upgrade-3.0.5/docs/LICENSE.GPL` & `plone.app.upgrade-3.0.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/docs/LICENSE.txt` & `plone.app.upgrade-3.0.6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/__init__.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/bbb_qi/QuickInstallerTool.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/bbb_qi/QuickInstallerTool.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/tests/base.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/tests/test_upgrade.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/tests/test_utils.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/utils.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/alphas.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/alphas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/betas.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/betas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/configure.zcml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/final.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/final.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/actions.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/registry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/profiles.zcml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v52/tests.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v52/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/alphas.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/alphas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/betas.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/betas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/configure.zcml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -285,8 +285,22 @@
         <gs:upgradeStep
             title="Fix TinyMCE menubar"
             handler=".final.fix_tinymce_menubar"
             />
 
     </gs:upgradeSteps>
 
+    <gs:upgradeSteps
+        profile="Products.CMFPlone:plone"
+        source="6016"
+        destination="6017"
+        >
+        <!-- Plone 6.0.6 -->
+
+        <gs:upgradeStep
+            title="Miscellaneous"
+            handler="..utils.null_upgrade_step"
+            />
+
+    </gs:upgradeSteps>
+
 </configure>
```

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/final.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/final.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6000/registry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6000/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6004/registry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6004/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6005/registry.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6005/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to6007/actions.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to6007/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/profiles.zcml` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone/app/upgrade/v60/tests.py` & `plone.app.upgrade-3.0.6/plone/app/upgrade/v60/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/PKG-INFO` & `plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.upgrade
-Version: 3.0.5
+Version: 3.0.6
 Summary: Upgrade machinery for Plone.
 Home-page: https://pypi.org/project/plone.app.upgrade/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone upgrade migration
 Classifier: Development Status :: 6 - Mature
@@ -41,14 +41,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Added upgrade to 6017, Plone 6.0.6.  [maurits] (#6017)
+
+
 3.0.5 (2023-05-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix TinyMCE problem: Tools and View do not show up in menubar.
```

### Comparing `plone.app.upgrade-3.0.5/plone.app.upgrade.egg-info/SOURCES.txt` & `plone.app.upgrade-3.0.6/plone.app.upgrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.0.5/setup.py` & `plone.app.upgrade-3.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.5"
+version = "3.0.6"
 
 setup(
     name="plone.app.upgrade",
     version=version,
     description="Upgrade machinery for Plone.",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
```

