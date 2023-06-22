# Comparing `tmp/glance_store-4.5.0.tar.gz` & `tmp/glance_store-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glance_store-4.5.0.tar", last modified: Tue May 30 07:25:24 2023, max compression
+gzip compressed data, was "glance_store-4.6.0.tar", last modified: Thu Jun 22 12:31:18 2023, max compression
```

## Comparing `glance_store-4.5.0.tar` & `glance_store-4.6.0.tar`

### file list

```diff
@@ -1,232 +1,234 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-30 07:24:56.000000 glance_store-4.5.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6002 2023-05-30 07:24:56.000000 glance_store-4.5.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6334 2023-05-30 07:25:24.000000 glance_store-4.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29309 2023-05-30 07:25:24.000000 glance_store-4.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-30 07:24:56.000000 glance_store-4.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-05-30 07:25:24.890111 glance_store-4.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-05-30 07:24:56.000000 glance_store-4.5.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-30 07:24:56.000000 glance_store-4.5.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.842106 glance_store-4.5.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/etc/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-05-30 07:24:56.000000 glance_store-4.5.0/etc/glance/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.850107 glance_store-4.5.0/etc/glance/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2023-05-30 07:24:56.000000 glance_store-4.5.0/etc/glance/rootwrap.d/glance_cinder_store.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.854107 glance_store-4.5.0/glance_store/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.858108 glance_store-4.5.0/glance_store/_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.858108 glance_store-4.5.0/glance_store/_drivers/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/cinder/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/cinder/nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/cinder/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43313 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/cinder/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28027 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38109 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/s3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.858108 glance_store-4.5.0/glance_store/_drivers/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/swift/buffered.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/swift/connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/swift/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/swift/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32181 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/_drivers/vmware_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.858108 glance_store-4.5.0/glance_store/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/common/attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/common/cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/common/fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10356 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/glance_store/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/glance_store/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.858108 glance_store-4.5.0/glance_store/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8378 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/glance_store/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/multi_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/etc/glance-swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/tests/functional/filesystem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/filesystem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.862108 glance_store-4.5.0/glance_store/tests/functional/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/functional/swift/test_functional_swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.870109 glance_store-4.5.0/glance_store/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.870109 glance_store-4.5.0/glance_store/tests/unit/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4661 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41368 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_cinder_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_cinder_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12926 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/cinder/test_scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.874109 glance_store-4.5.0/glance_store/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/common/test_attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/common/test_cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/common/test_fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_filesystem_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_http_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_multistore_filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17509 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_multistore_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_multistore_s3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_multistore_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26314 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_rbd_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_s3_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_store_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_store_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101249 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_swift_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_swift_store_multibackend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/unit/test_vmware_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-05-30 07:24:56.000000 glance_store-4.5.0/glance_store/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.854107 glance_store-4.5.0/glance_store.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-30 07:25:24.000000 glance_store-4.5.0/glance_store.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.886111 glance_store-4.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fix-rbd-lockup-3aa2bb86f7d29e19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.886111 glance_store-4.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58180 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.846106 glance_store-4.5.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-30 07:24:56.000000 glance_store-4.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-05-30 07:24:56.000000 glance_store-4.5.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7157 2023-05-30 07:24:56.000000 glance_store-4.5.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2345 2023-05-30 07:25:24.890111 glance_store-4.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-30 07:24:56.000000 glance_store-4.5.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-05-30 07:24:56.000000 glance_store-4.5.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 07:25:24.890111 glance_store-4.5.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11648 2023-05-30 07:24:56.000000 glance_store-4.5.0/tools/colorizer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-05-30 07:24:56.000000 glance_store-4.5.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5647 2023-05-30 07:24:56.000000 glance_store-4.5.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-05-30 07:24:56.000000 glance_store-4.5.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2023-05-30 07:24:56.000000 glance_store-4.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.812583 glance_store-4.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-06-22 12:30:54.000000 glance_store-4.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5994 2023-06-22 12:30:54.000000 glance_store-4.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6334 2023-06-22 12:31:18.000000 glance_store-4.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29475 2023-06-22 12:31:18.000000 glance_store-4.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-22 12:30:54.000000 glance_store-4.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-06-22 12:31:18.812583 glance_store-4.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-06-22 12:30:54.000000 glance_store-4.6.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-22 12:30:54.000000 glance_store-4.6.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.764577 glance_store-4.6.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/etc/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-06-22 12:30:54.000000 glance_store-4.6.0/etc/glance/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.772579 glance_store-4.6.0/etc/glance/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2023-06-22 12:30:54.000000 glance_store-4.6.0/etc/glance/rootwrap.d/glance_cinder_store.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.776579 glance_store-4.6.0/glance_store/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.780579 glance_store-4.6.0/glance_store/_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.780579 glance_store-4.6.0/glance_store/_drivers/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/cinder/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/cinder/nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/cinder/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43313 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/cinder/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28343 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38109 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/s3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.780579 glance_store-4.6.0/glance_store/_drivers/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/swift/buffered.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/swift/connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/swift/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/swift/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32181 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/_drivers/vmware_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.780579 glance_store-4.6.0/glance_store/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/common/attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/common/cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/common/fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11014 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/glance_store/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/glance_store/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.780579 glance_store-4.6.0/glance_store/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8378 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/glance_store/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/multi_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/etc/glance-swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/tests/functional/filesystem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/filesystem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.784580 glance_store-4.6.0/glance_store/tests/functional/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/functional/swift/test_functional_swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.788580 glance_store-4.6.0/glance_store/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.792581 glance_store-4.6.0/glance_store/tests/unit/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4661 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41368 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_cinder_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_cinder_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12926 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/cinder/test_scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.792581 glance_store-4.6.0/glance_store/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/common/test_attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/common/test_cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/common/test_fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_filesystem_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_http_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_multistore_filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17478 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_multistore_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_multistore_s3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_multistore_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30137 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_rbd_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_s3_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_store_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_store_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101249 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_swift_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_swift_store_multibackend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/unit/test_vmware_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-06-22 12:30:54.000000 glance_store-4.6.0/glance_store/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.776579 glance_store-4.6.0/glance_store.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8530 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-06-22 12:31:18.000000 glance_store-4.6.0/glance_store.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.804582 glance_store-4.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/add-store-weight-d443fbea8cc8d4c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fix-rbd-lockup-3aa2bb86f7d29e19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/rbd-trash-snapshots-158a39da4248fb0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58180 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.768578 glance_store-4.6.0/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-06-22 12:30:54.000000 glance_store-4.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-06-22 12:30:54.000000 glance_store-4.6.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7157 2023-06-22 12:30:54.000000 glance_store-4.6.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2345 2023-06-22 12:31:18.812583 glance_store-4.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-06-22 12:30:54.000000 glance_store-4.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-06-22 12:30:54.000000 glance_store-4.6.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-22 12:31:18.808583 glance_store-4.6.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11648 2023-06-22 12:30:54.000000 glance_store-4.6.0/tools/colorizer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-06-22 12:30:54.000000 glance_store-4.6.0/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5647 2023-06-22 12:30:54.000000 glance_store-4.6.0/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-06-22 12:30:54.000000 glance_store-4.6.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2023-06-22 12:30:54.000000 glance_store-4.6.0/tox.ini
```

### Comparing `glance_store-4.5.0/.zuul.yaml` & `glance_store-4.6.0/.zuul.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     parent: devstack-plugin-ceph-tempest-py3
     description: |
       Runs tempest tests with the latest glance_store and the Ceph backend
       Former names for this job were:
       * legacy-tempest-dsvm-full-ceph-plugin-src-glance_store
     required-projects:
       - opendev.org/openstack/glance_store
+    timeout: 9000
     vars:
       tempest_test_regex: (^tempest\.(api|scenario)|(^cinder_tempest_plugin))
 
 - job:
     name: cross-glance-tox-functional
     parent: openstack-tox
     description: |
@@ -152,15 +153,14 @@
       - openstack-python3-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - cross-glance-tox-functional
         - glance_store-src-ceph-tempest:
-            voting: false
             irrelevant-files: &tempest-irrelevant-files
               - ^doc/.*$
               - ^releasenotes/.*$
               - ^.*\.rst$
               - ^(test-|)requirements.txt$
               - ^setup.cfg$
               - ^tox.ini$
```

### Comparing `glance_store-4.5.0/AUTHORS` & `glance_store-4.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/ChangeLog` & `glance_store-4.6.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+4.6.0
+-----
+
+* RBD: Trash image when snapshots prevent deletion
+* Add per-store weight config element
+* RBD: Wrap RBD calls in native threads
+* Make ceph job voting
+
 4.5.0
 -----
 
 * Revert "RBD: Wrap RBD calls in native threads"
 * Update 'extras' for cinder driver
 * Imported Translations from Zanata
```

### Comparing `glance_store-4.5.0/LICENSE` & `glance_store-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/PKG-INFO` & `glance_store-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance_store
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.5.0/README.rst` & `glance_store-4.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/doc/source/conf.py` & `glance_store-4.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/doc/source/index.rst` & `glance_store-4.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/doc/source/user/drivers.rst` & `glance_store-4.6.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/etc/glance/rootwrap.conf` & `glance_store-4.6.0/etc/glance/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/etc/glance/rootwrap.d/glance_cinder_store.filters` & `glance_store-4.6.0/etc/glance/rootwrap.d/glance_cinder_store.filters`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/__init__.py` & `glance_store-4.6.0/glance_store/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/cinder/__init__.py` & `glance_store-4.6.0/glance_store/_drivers/cinder/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/cinder/base.py` & `glance_store-4.6.0/glance_store/_drivers/cinder/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/cinder/nfs.py` & `glance_store-4.6.0/glance_store/_drivers/cinder/nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/cinder/scaleio.py` & `glance_store-4.6.0/glance_store/_drivers/cinder/scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/cinder/store.py` & `glance_store-4.6.0/glance_store/_drivers/cinder/store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/filesystem.py` & `glance_store-4.6.0/glance_store/_drivers/filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/http.py` & `glance_store-4.6.0/glance_store/_drivers/http.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/rbd.py` & `glance_store-4.6.0/glance_store/_drivers/rbd.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
    (RADOS (Reliable Autonomic Distributed Object Store) Block Device)"""
 
 import contextlib
 import logging
 import math
 import urllib
 
+from eventlet import tpool
 from oslo_config import cfg
 from oslo_utils import encodeutils
+from oslo_utils import eventletutils
 from oslo_utils import units
 
 from glance_store import capabilities
 from glance_store.common import utils
 from glance_store import driver
 from glance_store import exceptions
 from glance_store.i18n import _, _LE, _LI, _LW
@@ -286,14 +288,20 @@
     OPTIONS = _RBD_OPTS
 
     EXAMPLE_URL = "rbd://<FSID>/<POOL>/<IMAGE>/<SNAP>"
 
     def get_schemes(self):
         return ('rbd',)
 
+    def RBDProxy(self):
+        if eventletutils.is_monkey_patched('thread'):
+            return tpool.Proxy(rbd.RBD())
+        else:
+            return rbd.RBD()
+
     @contextlib.contextmanager
     def get_connection(self, conffile, rados_id):
         client = rados.Rados(conffile=conffile, rados_id=rados_id)
 
         try:
             client.connect()
         except (rados.Error, rados.ObjectNotFound) as e:
@@ -427,20 +435,20 @@
         make it a cloneable snapshot, so that copy-on-write
         volumes can be created from it.
 
         :param image_name: Image's name
 
         :returns: `glance_store.rbd.StoreLocation` object
         """
-        librbd = rbd.RBD()
         features = conn.conf_get('rbd_default_features')
         if ((features is None) or (int(features) == 0)):
             features = rbd.RBD_FEATURE_LAYERING
-        librbd.create(ioctx, image_name, size, order, old_format=False,
-                      features=int(features))
+        self.RBDProxy().create(ioctx, image_name, size, order,
+                               old_format=False,
+                               features=int(features))
         return StoreLocation({
             'fsid': fsid,
             'pool': self.pool,
             'image': image_name,
             'snapshot': DEFAULT_SNAPNAME,
         }, self.conf)
 
@@ -467,22 +475,14 @@
                                  rados_id=self.user) as conn:
             with conn.open_ioctx(target_pool) as ioctx:
                 try:
                     # First remove snapshot.
                     if snapshot_name is not None:
                         with rbd.Image(ioctx, image_name) as image:
                             try:
-                                # NOTE(abhishekk): Check whether snapshot
-                                # has any external references
-                                if self._snapshot_has_external_reference(
-                                        image, snapshot_name):
-                                    raise rbd.ImageBusy(
-                                        "Image snapshot has external "
-                                        "references.")
-
                                 self._unprotect_snapshot(image, snapshot_name)
                                 image.remove_snap(snapshot_name)
                             except rbd.ImageNotFound as exc:
                                 msg = (_("Snap Operating Exception "
                                          "%(snap_exc)s "
                                          "Snapshot does not exist.") %
                                        {'snap_exc': exc})
@@ -492,20 +492,29 @@
                                                "%(snap_exc)s "
                                                "Snapshot is in use.") %
                                            {'snap_exc': exc})
                                 LOG.warning(log_msg)
                                 raise exceptions.InUseByStore()
 
                     # Then delete image.
-                    rbd.RBD().remove(ioctx, image_name)
+                    self.RBDProxy().remove(ioctx, image_name)
                 except rbd.ImageHasSnapshots:
-                    log_msg = (_LW("Remove image %(img_name)s failed. "
-                                   "It has snapshot(s) left.") %
+                    log_msg = (_LW("Unable to remove image %(img_name)s: it "
+                                   "has snapshot(s) left; trashing instead") %
                                {'img_name': image_name})
                     LOG.warning(log_msg)
+                    with rbd.Image(ioctx, image_name) as image:
+                        try:
+                            rbd.RBD().trash_move(ioctx, image_name)
+                            LOG.debug('Moved %s to trash', image_name)
+                        except rbd.ImageBusy:
+                            LOG.warning(_('Unable to move in-use image to '
+                                          'trash'))
+                            raise exceptions.InUseByStore()
+                        return
                     raise exceptions.HasSnapshot()
                 except rbd.ImageBusy:
                     log_msg = (_LW("Remove image %(img_name)s failed. "
                                    "It is in use.") %
                                {'img_name': image_name})
                     LOG.warning(log_msg)
                     raise exceptions.InUseByStore()
```

### Comparing `glance_store-4.5.0/glance_store/_drivers/s3.py` & `glance_store-4.6.0/glance_store/_drivers/s3.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/swift/__init__.py` & `glance_store-4.6.0/glance_store/_drivers/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/swift/buffered.py` & `glance_store-4.6.0/glance_store/_drivers/swift/buffered.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/swift/connection_manager.py` & `glance_store-4.6.0/glance_store/_drivers/swift/connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/swift/store.py` & `glance_store-4.6.0/glance_store/_drivers/swift/store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/swift/utils.py` & `glance_store-4.6.0/glance_store/_drivers/swift/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/_drivers/vmware_datastore.py` & `glance_store-4.6.0/glance_store/_drivers/vmware_datastore.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/backend.py` & `glance_store-4.6.0/glance_store/backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/capabilities.py` & `glance_store-4.6.0/glance_store/capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/common/attachment_state_manager.py` & `glance_store-4.6.0/glance_store/common/attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/common/cinder_utils.py` & `glance_store-4.6.0/glance_store/common/cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/common/fs_mount.py` & `glance_store-4.6.0/glance_store/common/fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/common/utils.py` & `glance_store-4.6.0/glance_store/common/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/driver.py` & `glance_store-4.6.0/glance_store/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,23 @@
 _MULTI_BACKEND_OPTS = [
     cfg.StrOpt('store_description',
                help=_("""
 This option will be used to provide a constructive information about
 the store backend to end users. Using /v2/stores-info call user can
 seek more information on all available backends.
 
-"""))
+""")),
+    cfg.IntOpt('weight',
+               help=_("""
+This option is used to define a relative weight for this store over
+any others that are configured. The actual value of the weight is meaningless
+and only serves to provide a "sort order" compared to others. Any stores
+with the same weight will be treated as equivalent.
+"""),
+               default=0),
 ]
 
 
 class Store(capabilities.StoreCapability):
 
     OPTIONS = None
     MULTI_BACKEND_OPTIONS = _MULTI_BACKEND_OPTS
@@ -75,14 +83,23 @@
         except cfg.DuplicateOptError:
             pass
 
     @property
     def url_prefix(self):
         return self._url_prefix
 
+    @property
+    def weight(self):
+        if self.backend_group is None:
+            # NOTE(danms): A backend with no config group can not have a
+            # weight set, so just return the default
+            return 0
+        else:
+            return getattr(self.conf, self.backend_group).weight
+
     def configure(self, re_raise_bsc=False):
         """
         Configure the store to use the stored configuration options
         and initialize capabilities based on current configuration.
 
         Any store that needs special configuration should implement
         this method.
```

### Comparing `glance_store-4.5.0/glance_store/exceptions.py` & `glance_store-4.6.0/glance_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/i18n.py` & `glance_store-4.6.0/glance_store/i18n.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po` & `glance_store-4.6.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po` & `glance_store-4.6.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/location.py` & `glance_store-4.6.0/glance_store/location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/multi_backend.py` & `glance_store-4.6.0/glance_store/multi_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/base.py` & `glance_store-4.6.0/glance_store/tests/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/etc/glance-swift.conf` & `glance_store-4.6.0/glance_store/tests/etc/glance-swift.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/fakes.py` & `glance_store-4.6.0/glance_store/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/functional/README.rst` & `glance_store-4.6.0/glance_store/tests/functional/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/functional/base.py` & `glance_store-4.6.0/glance_store/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py` & `glance_store-4.6.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/functional/swift/test_functional_swift.py` & `glance_store-4.6.0/glance_store/tests/functional/swift/test_functional_swift.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_base.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_cinder_base.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_cinder_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_cinder_store.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_cinder_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_multistore_cinder.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_multistore_cinder.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_nfs.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/cinder/test_scaleio.py` & `glance_store-4.6.0/glance_store/tests/unit/cinder/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/common/test_attachment_state_manager.py` & `glance_store-4.6.0/glance_store/tests/unit/common/test_attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/common/test_cinder_utils.py` & `glance_store-4.6.0/glance_store/tests/unit/common/test_cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/common/test_fs_mount.py` & `glance_store-4.6.0/glance_store/tests/unit/common/test_fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/common/test_utils.py` & `glance_store-4.6.0/glance_store/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_backend.py` & `glance_store-4.6.0/glance_store/tests/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_connection_manager.py` & `glance_store-4.6.0/glance_store/tests/unit/test_connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_driver.py` & `glance_store-4.6.0/glance_store/tests/unit/test_driver.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_exceptions.py` & `glance_store-4.6.0/glance_store/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_filesystem_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_filesystem_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_http_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_http_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_location.py` & `glance_store-4.6.0/glance_store/tests/unit/test_location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_multistore_filesystem.py` & `glance_store-4.6.0/glance_store/tests/unit/test_multistore_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_multistore_rbd.py` & `glance_store-4.6.0/glance_store/tests/unit/test_multistore_rbd.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,17 @@
 
         def list(self, *args, **kwargs):
             raise NotImplementedError()
 
         def clone(self, *args, **kwargs):
             raise NotImplementedError()
 
+        def trash_move(self, *args, **kwargs):
+            pass
+
     RBD_FEATURE_LAYERING = 1
 
 
 class TestMultiStore(base.MultiStoreBaseTest,
                      test_store_capabilities.TestStoreCapabilitiesChecking):
 
     # NOTE(flaper87): temporary until we
@@ -423,28 +426,27 @@
 
             self.called_commands_expected = ['unprotect_snap']
 
     def test_delete_image_snap_has_external_references(self):
         with mock.patch.object(MockRBD.Image, 'list_children') as mocked:
             mocked.return_value = True
 
-            self.assertRaises(exceptions.InUseByStore,
-                              self.store._delete_image,
-                              'fake_pool', self.location.image,
-                              snapshot_name='snap')
+            self.store._delete_image('fake_pool',
+                                     self.location.image,
+                                     snapshot_name='snap')
 
     def test_delete_image_w_snap_exc_image_has_snap(self):
         def _fake_remove(*args, **kwargs):
             self.called_commands_actual.append('remove')
             raise MockRBD.ImageHasSnapshots()
 
         with mock.patch.object(MockRBD.RBD, 'remove') as remove:
             remove.side_effect = _fake_remove
-            self.assertRaises(exceptions.HasSnapshot, self.store._delete_image,
-                              'fake_pool', self.location.image)
+            self.store._delete_image('fake_pool',
+                                     self.location.image)
 
             self.called_commands_expected = ['remove']
 
     def test_get_partial_image(self):
         loc = g_location.Location('test_rbd_store', rbd_store.StoreLocation,
                                   self.conf, store_specs=self.store_specs)
         self.assertRaises(exceptions.StoreRandomGetNotSupported,
```

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_multistore_s3.py` & `glance_store-4.6.0/glance_store/tests/unit/test_multistore_s3.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_multistore_vmware.py` & `glance_store-4.6.0/glance_store/tests/unit/test_multistore_vmware.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_opts.py` & `glance_store-4.6.0/glance_store/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_rbd_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_rbd_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -169,14 +169,17 @@
 
         def list(self, *args, **kwargs):
             raise NotImplementedError()
 
         def clone(self, *args, **kwargs):
             raise NotImplementedError()
 
+        def trash_move(self, *args, **kwargs):
+            pass
+
     RBD_FEATURE_LAYERING = 1
 
 
 class TestReSize(base.StoreBaseTest,
                  test_store_capabilities.TestStoreCapabilitiesChecking):
 
     def setUp(self):
@@ -629,31 +632,53 @@
 
             self.called_commands_expected = ['unprotect_snap']
 
     def test_delete_image_snap_has_external_references(self):
         with mock.patch.object(MockRBD.Image, 'list_children') as mocked:
             mocked.return_value = True
 
-            self.assertRaises(exceptions.InUseByStore,
-                              self.store._delete_image,
-                              'fake_pool', self.location.image,
-                              snapshot_name='snap')
+            self.store._delete_image('fake_pool',
+                                     self.location.image,
+                                     snapshot_name='snap')
 
     def test_delete_image_w_snap_exc_image_has_snap(self):
         def _fake_remove(*args, **kwargs):
             self.called_commands_actual.append('remove')
             raise MockRBD.ImageHasSnapshots()
 
+        mock.patch.object(MockRBD.RBD, 'trash_move').start()
+
         with mock.patch.object(MockRBD.RBD, 'remove') as remove:
             remove.side_effect = _fake_remove
-            self.assertRaises(exceptions.HasSnapshot, self.store._delete_image,
-                              'fake_pool', self.location.image)
+            self.store._delete_image('fake_pool',
+                                     self.location.image)
+
+            self.called_commands_expected = ['remove']
+
+        MockRBD.RBD.trash_move.assert_called_once_with(mock.ANY, 'fake_image')
+
+    def test_delete_image_w_snap_exc_image_has_snap_2(self):
+        def _fake_remove(*args, **kwargs):
+            self.called_commands_actual.append('remove')
+            raise MockRBD.ImageHasSnapshots()
+
+        mock.patch.object(MockRBD.RBD, 'trash_move',
+                          side_effect=MockRBD.ImageBusy).start()
+
+        with mock.patch.object(MockRBD.RBD, 'remove') as remove:
+            remove.side_effect = _fake_remove
+            self.assertRaises(exceptions.InUseByStore,
+                              self.store._delete_image,
+                              'fake_pool',
+                              self.location.image)
 
             self.called_commands_expected = ['remove']
 
+        MockRBD.RBD.trash_move.assert_called_once_with(mock.ANY, 'fake_image')
+
     def test_get_partial_image(self):
         loc = g_location.Location('test_rbd_store', rbd_store.StoreLocation,
                                   self.conf, store_specs=self.store_specs)
         self.assertRaises(exceptions.StoreRandomGetNotSupported,
                           self.store.get, loc, chunk_size=1)
 
     @mock.patch.object(MockRados.Rados, 'connect', side_effect=MockRados.Error)
@@ -688,7 +713,71 @@
         create_mock.assert_called_once_with(ioctxt, name, size, order,
                                             old_format=False, features=3)
 
     def tearDown(self):
         self.assertEqual(self.called_commands_expected,
                          self.called_commands_actual)
         super(TestStore, self).tearDown()
+
+    @mock.patch('oslo_utils.eventletutils.is_monkey_patched')
+    def test_create_image_in_native_thread(self, mock_patched):
+        mock_patched.return_value = True
+        # Tests that we use non-0 features from ceph.conf and cast to int.
+        fsid = 'fake'
+        features = '3'
+        conf_get_mock = mock.Mock(return_value=features)
+        conn = mock.Mock(conf_get=conf_get_mock)
+        ioctxt = mock.sentinel.ioctxt
+        name = '1'
+        size = 1024
+        order = 3
+        fake_proxy = mock.MagicMock()
+        fake_rbd = mock.MagicMock()
+
+        with mock.patch.object(rbd_store.tpool, 'Proxy') as tpool_mock, \
+                mock.patch.object(rbd_store.rbd, 'RBD') as rbd_mock:
+            tpool_mock.return_value = fake_proxy
+            rbd_mock.return_value = fake_rbd
+            location = self.store._create_image(
+                fsid, conn, ioctxt, name, size, order)
+            self.assertEqual(fsid, location.specs['fsid'])
+            self.assertEqual(rbd_store.DEFAULT_POOL, location.specs['pool'])
+            self.assertEqual(name, location.specs['image'])
+            self.assertEqual(rbd_store.DEFAULT_SNAPNAME,
+                             location.specs['snapshot'])
+
+        tpool_mock.assert_called_once_with(fake_rbd)
+        fake_proxy.create.assert_called_once_with(ioctxt, name, size, order,
+                                                  old_format=False, features=3)
+
+    @mock.patch('oslo_utils.eventletutils.is_monkey_patched')
+    def test_delete_image_in_native_thread(self, mock_patched):
+        mock_patched.return_value = True
+        fake_proxy = mock.MagicMock()
+        fake_rbd = mock.MagicMock()
+        fake_ioctx = mock.MagicMock()
+
+        with mock.patch.object(rbd_store.tpool, 'Proxy') as tpool_mock, \
+                mock.patch.object(rbd_store.rbd, 'RBD') as rbd_mock, \
+                mock.patch.object(self.store, 'get_connection') as mock_conn:
+
+            mock_get_conn = mock_conn.return_value.__enter__.return_value
+            mock_ioctx = mock_get_conn.open_ioctx.return_value.__enter__
+            mock_ioctx.return_value = fake_ioctx
+            tpool_mock.return_value = fake_proxy
+            rbd_mock.return_value = fake_rbd
+
+            self.store._delete_image('fake_pool', self.location.image)
+
+            tpool_mock.assert_called_once_with(fake_rbd)
+            fake_proxy.remove.assert_called_once_with(fake_ioctx,
+                                                      self.location.image)
+
+    @mock.patch.object(rbd_store, 'rbd')
+    @mock.patch.object(rbd_store, 'tpool')
+    @mock.patch('oslo_utils.eventletutils.is_monkey_patched')
+    def test_rbd_proxy(self, mock_patched, mock_tpool, mock_rbd):
+        mock_patched.return_value = False
+        self.assertEqual(mock_rbd.RBD(), self.store.RBDProxy())
+
+        mock_patched.return_value = True
+        self.assertEqual(mock_tpool.Proxy.return_value, self.store.RBDProxy())
```

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_s3_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_s3_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_store_base.py` & `glance_store-4.6.0/glance_store/tests/unit/test_store_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_store_capabilities.py` & `glance_store-4.6.0/glance_store/tests/unit/test_store_capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_swift_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_swift_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_swift_store_multibackend.py` & `glance_store-4.6.0/glance_store/tests/unit/test_swift_store_multibackend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_swift_store_utils.py` & `glance_store-4.6.0/glance_store/tests/unit/test_swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_test_utils.py` & `glance_store-4.6.0/glance_store/tests/unit/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/unit/test_vmware_store.py` & `glance_store-4.6.0/glance_store/tests/unit/test_vmware_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store/tests/utils.py` & `glance_store-4.6.0/glance_store/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store.egg-info/PKG-INFO` & `glance_store-4.6.0/glance_store.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance-store
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.5.0/glance_store.egg-info/SOURCES.txt` & `glance_store-4.6.0/glance_store.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 glance_store/tests/unit/common/test_attachment_state_manager.py
 glance_store/tests/unit/common/test_cinder_utils.py
 glance_store/tests/unit/common/test_fs_mount.py
 glance_store/tests/unit/common/test_utils.py
 releasenotes/notes/.placeholder
 releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
 releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
+releasenotes/notes/add-store-weight-d443fbea8cc8d4c9.yaml
 releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
 releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
 releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
 releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
 releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
 releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
 releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
@@ -134,14 +135,15 @@
 releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
 releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
 releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
 releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
 releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
 releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
 releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
+releasenotes/notes/rbd-trash-snapshots-158a39da4248fb0c.yaml
 releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
 releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
 releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
 releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
 releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
 releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
 releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
```

### Comparing `glance_store-4.5.0/glance_store.egg-info/entry_points.txt` & `glance_store-4.6.0/glance_store.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/glance_store.egg-info/requires.txt` & `glance_store-4.6.0/glance_store.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml` & `glance_store-4.6.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml` & `glance_store-4.6.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml` & `glance_store-4.6.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml` & `glance_store-4.6.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml` & `glance_store-4.6.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml` & `glance_store-4.6.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml` & `glance_store-4.6.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml` & `glance_store-4.6.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml` & `glance_store-4.6.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml` & `glance_store-4.6.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml` & `glance_store-4.6.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml` & `glance_store-4.6.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml` & `glance_store-4.6.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml` & `glance_store-4.6.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml` & `glance_store-4.6.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml` & `glance_store-4.6.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml` & `glance_store-4.6.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml` & `glance_store-4.6.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml` & `glance_store-4.6.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml` & `glance_store-4.6.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/source/conf.py` & `glance_store-4.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `glance_store-4.6.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `glance_store-4.6.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `glance_store-4.6.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/requirements.txt` & `glance_store-4.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/run_tests.sh` & `glance_store-4.6.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/setup.cfg` & `glance_store-4.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/setup.py` & `glance_store-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/test-requirements.txt` & `glance_store-4.6.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/tools/colorizer.py` & `glance_store-4.6.0/tools/colorizer.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/tools/install_venv.py` & `glance_store-4.6.0/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/tools/install_venv_common.py` & `glance_store-4.6.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.5.0/tox.ini` & `glance_store-4.6.0/tox.ini`

 * *Files identical despite different names*

