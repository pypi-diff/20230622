# Comparing `tmp/pulumi_linode-4.3.0a1687055232.tar.gz` & `tmp/pulumi_linode-4.3.0a1687424922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_linode-4.3.0a1687055232.tar", last modified: Sun Jun 18 02:36:49 2023, max compression
+gzip compressed data, was "pulumi_linode-4.3.0a1687424922.tar", last modified: Thu Jun 22 09:14:54 2023, max compression
```

## Comparing `pulumi_linode-4.3.0a1687055232.tar` & `pulumi_linode-4.3.0a1687424922.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:36:49.138024 pulumi_linode-4.3.0a1687055232/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-18 02:36:49.134024 pulumi_linode-4.3.0a1687055232/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:36:49.134024 pulumi_linode-4.3.0a1687055232/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130974 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/account_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:36:49.134024 pulumi_linode-4.3.0a1687055232/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain_zonefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_linode_object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_lke_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (123)   253542 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:36:49.134024 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-18 02:36:49.000000 pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:36:49.138024 pulumi_linode-4.3.0a1687055232/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-18 02:36:48.000000 pulumi_linode-4.3.0a1687055232/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.986074 pulumi_linode-4.3.0a1687424922/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134820 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/account_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_zonefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_linode_object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)   257564 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:53.982074 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:14:53.986074 pulumi_linode-4.3.0a1687424922/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 09:14:53.000000 pulumi_linode-4.3.0a1687424922/setup.py
```

### Comparing `pulumi_linode-4.3.0a1687055232/PKG-INFO` & `pulumi_linode-4.3.0a1687424922/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_linode
-Version: 4.3.0a1687055232
+Version: 4.3.0a1687424922
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.3.0a1687055232/README.md` & `pulumi_linode-4.3.0a1687424922/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/__init__.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/_inputs.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     'GetDatabaseEnginesFilterArgs',
     'GetDatabaseMysqlBackupsFilterArgs',
     'GetDatabasesFilterArgs',
     'GetImagesFilterArgs',
     'GetInstanceTypesFilterArgs',
     'GetInstancesFilterArgs',
     'GetRegionsFilterArgs',
+    'GetRegionsRegionArgs',
+    'GetRegionsRegionResolverArgs',
     'GetStackScriptsFilterArgs',
     'GetUserDomainGrantArgs',
     'GetUserFirewallGrantArgs',
     'GetUserImageGrantArgs',
     'GetUserLinodeGrantArgs',
     'GetUserLongviewGrantArgs',
     'GetUserNodebalancerGrantArgs',
@@ -3269,14 +3271,141 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
+class GetRegionsRegionArgs:
+    def __init__(__self__, *,
+                 capabilities: Sequence[str],
+                 country: str,
+                 id: str,
+                 label: str,
+                 status: str,
+                 resolvers: Optional[Sequence['GetRegionsRegionResolverArgs']] = None):
+        """
+        :param Sequence[str] capabilities: A list of capabilities of this region.
+        :param str country: The country the region resides in.
+        :param str label: Detailed location information for this Region, including city, state or region, and country.
+        :param str status: This region’s current operational status (ok or outage).
+        """
+        pulumi.set(__self__, "capabilities", capabilities)
+        pulumi.set(__self__, "country", country)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "status", status)
+        if resolvers is not None:
+            pulumi.set(__self__, "resolvers", resolvers)
+
+    @property
+    @pulumi.getter
+    def capabilities(self) -> Sequence[str]:
+        """
+        A list of capabilities of this region.
+        """
+        return pulumi.get(self, "capabilities")
+
+    @capabilities.setter
+    def capabilities(self, value: Sequence[str]):
+        pulumi.set(self, "capabilities", value)
+
+    @property
+    @pulumi.getter
+    def country(self) -> str:
+        """
+        The country the region resides in.
+        """
+        return pulumi.get(self, "country")
+
+    @country.setter
+    def country(self, value: str):
+        pulumi.set(self, "country", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: str):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        """
+        Detailed location information for this Region, including city, state or region, and country.
+        """
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: str):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        """
+        This region’s current operational status (ok or outage).
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: str):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
+    def resolvers(self) -> Optional[Sequence['GetRegionsRegionResolverArgs']]:
+        return pulumi.get(self, "resolvers")
+
+    @resolvers.setter
+    def resolvers(self, value: Optional[Sequence['GetRegionsRegionResolverArgs']]):
+        pulumi.set(self, "resolvers", value)
+
+
+@pulumi.input_type
+class GetRegionsRegionResolverArgs:
+    def __init__(__self__, *,
+                 ipv4: str,
+                 ipv6: str):
+        """
+        :param str ipv4: The IPv4 addresses for this region’s DNS resolvers, separated by commas.
+        :param str ipv6: The IPv6 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        pulumi.set(__self__, "ipv4", ipv4)
+        pulumi.set(__self__, "ipv6", ipv6)
+
+    @property
+    @pulumi.getter
+    def ipv4(self) -> str:
+        """
+        The IPv4 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        return pulumi.get(self, "ipv4")
+
+    @ipv4.setter
+    def ipv4(self, value: str):
+        pulumi.set(self, "ipv4", value)
+
+    @property
+    @pulumi.getter
+    def ipv6(self) -> str:
+        """
+        The IPv6 addresses for this region’s DNS resolvers, separated by commas.
+        """
+        return pulumi.get(self, "ipv6")
+
+    @ipv6.setter
+    def ipv6(self, value: str):
+        pulumi.set(self, "ipv6", value)
+
+
+@pulumi.input_type
 class GetStackScriptsFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/_utilities.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/account_settings.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/config/vars.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/database_access_controls.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_access_controls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/database_mysql.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/database_postgresql.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/domain.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/domain_record.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/firewall.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/firewall_device.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/firewall_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_login.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_logins.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_logins.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_account_settings.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_backups.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_engines.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_engines.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_mysql.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         pulumi.set(__self__, "engine_id", engine_id)
         if host_primary and not isinstance(host_primary, str):
             raise TypeError("Expected argument 'host_primary' to be a str")
         pulumi.set(__self__, "host_primary", host_primary)
         if host_secondary and not isinstance(host_secondary, str):
             raise TypeError("Expected argument 'host_secondary' to be a str")
         pulumi.set(__self__, "host_secondary", host_secondary)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
+        if id and not isinstance(id, int):
+            raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if label and not isinstance(label, str):
             raise TypeError("Expected argument 'label' to be a str")
         pulumi.set(__self__, "label", label)
         if region and not isinstance(region, str):
             raise TypeError("Expected argument 'region' to be a str")
         pulumi.set(__self__, "region", region)
@@ -120,15 +120,15 @@
         """
         When this Managed Database was created.
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter(name="databaseId")
-    def database_id(self) -> int:
+    def database_id(self) -> Optional[int]:
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def encrypted(self) -> bool:
         """
         Whether the Managed Databases is encrypted.
@@ -165,18 +165,15 @@
         """
         The secondary/private network host for the Managed Database.
         """
         return pulumi.get(self, "host_secondary")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
+    def id(self) -> Optional[int]:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def label(self) -> str:
         """
         A unique, user-defined string referring to the Managed Database.
@@ -288,27 +285,28 @@
             type=self.type,
             updated=self.updated,
             updates=self.updates,
             version=self.version)
 
 
 def get_database_mysql(database_id: Optional[int] = None,
+                       id: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseMysqlResult:
     """
     Provides information about a Linode MySQL Database.
 
     ## Example Usage
 
     Get information about a MySQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_mysql(database_id=12345)
+    my_db = linode.get_database_mysql(id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -317,18 +315,20 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the MySQL database.
+    :param int database_id: The ID of the MySQL database. Deprecated: Use id instead.
+    :param int id: The ID of the MySQL database. Mutually exclusive with `database_id`.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
+    __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMysql:getDatabaseMysql', __args__, opts=opts, typ=GetDatabaseMysqlResult).value
 
     return AwaitableGetDatabaseMysqlResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
@@ -350,28 +350,29 @@
         type=__ret__.type,
         updated=__ret__.updated,
         updates=__ret__.updates,
         version=__ret__.version)
 
 
 @_utilities.lift_output_func(get_database_mysql)
-def get_database_mysql_output(database_id: Optional[pulumi.Input[int]] = None,
+def get_database_mysql_output(database_id: Optional[pulumi.Input[Optional[int]]] = None,
+                              id: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseMysqlResult]:
     """
     Provides information about a Linode MySQL Database.
 
     ## Example Usage
 
     Get information about a MySQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_mysql(database_id=12345)
+    my_db = linode.get_database_mysql(id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -380,10 +381,11 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the MySQL database.
+    :param int database_id: The ID of the MySQL database. Deprecated: Use id instead.
+    :param int id: The ID of the MySQL database. Mutually exclusive with `database_id`.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_mysql_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_database_postgresql.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_database_postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         pulumi.set(__self__, "engine_id", engine_id)
         if host_primary and not isinstance(host_primary, str):
             raise TypeError("Expected argument 'host_primary' to be a str")
         pulumi.set(__self__, "host_primary", host_primary)
         if host_secondary and not isinstance(host_secondary, str):
             raise TypeError("Expected argument 'host_secondary' to be a str")
         pulumi.set(__self__, "host_secondary", host_secondary)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
+        if id and not isinstance(id, int):
+            raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if label and not isinstance(label, str):
             raise TypeError("Expected argument 'label' to be a str")
         pulumi.set(__self__, "label", label)
         if port and not isinstance(port, int):
             raise TypeError("Expected argument 'port' to be a int")
         pulumi.set(__self__, "port", port)
@@ -126,15 +126,15 @@
         """
         When this Managed Database was created.
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter(name="databaseId")
-    def database_id(self) -> int:
+    def database_id(self) -> Optional[int]:
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def encrypted(self) -> bool:
         """
         Whether the Managed Databases is encrypted.
@@ -171,18 +171,15 @@
         """
         The secondary/private network host for the Managed Database.
         """
         return pulumi.get(self, "host_secondary")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
+    def id(self) -> Optional[int]:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def label(self) -> str:
         """
         A unique, user-defined string referring to the Managed Database.
@@ -309,27 +306,28 @@
             type=self.type,
             updated=self.updated,
             updates=self.updates,
             version=self.version)
 
 
 def get_database_postgresql(database_id: Optional[int] = None,
+                            id: Optional[int] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabasePostgresqlResult:
     """
     Provides information about a Linode PostgreSQL Database.
 
     ## Example Usage
 
     Get information about a PostgreSQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_postgresql(database_id=12345)
+    my_db = linode.get_database_postgresql(id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -338,18 +336,20 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the PostgreSQL database.
+    :param int database_id: The ID of the PostgreSQL database. Deprecated: Use id instead.
+    :param int id: The ID of the PostgreSQL database. Mutually exclusive with `database_id`.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
+    __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabasePostgresql:getDatabasePostgresql', __args__, opts=opts, typ=GetDatabasePostgresqlResult).value
 
     return AwaitableGetDatabasePostgresqlResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
@@ -373,28 +373,29 @@
         type=__ret__.type,
         updated=__ret__.updated,
         updates=__ret__.updates,
         version=__ret__.version)
 
 
 @_utilities.lift_output_func(get_database_postgresql)
-def get_database_postgresql_output(database_id: Optional[pulumi.Input[int]] = None,
+def get_database_postgresql_output(database_id: Optional[pulumi.Input[Optional[int]]] = None,
+                                   id: Optional[pulumi.Input[Optional[int]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabasePostgresqlResult]:
     """
     Provides information about a Linode PostgreSQL Database.
 
     ## Example Usage
 
     Get information about a PostgreSQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_postgresql(database_id=12345)
+    my_db = linode.get_database_postgresql(id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -403,10 +404,11 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the PostgreSQL database.
+    :param int database_id: The ID of the PostgreSQL database. Deprecated: Use id instead.
+    :param int id: The ID of the PostgreSQL database. Mutually exclusive with `database_id`.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_databases.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         pulumi.set(__self__, "domain", domain)
         if expire_sec and not isinstance(expire_sec, int):
             raise TypeError("Expected argument 'expire_sec' to be a int")
         pulumi.set(__self__, "expire_sec", expire_sec)
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
         pulumi.set(__self__, "group", group)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
+        if id and not isinstance(id, int):
+            raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if master_ips and not isinstance(master_ips, list):
             raise TypeError("Expected argument 'master_ips' to be a list")
         pulumi.set(__self__, "master_ips", master_ips)
         if refresh_sec and not isinstance(refresh_sec, int):
             raise TypeError("Expected argument 'refresh_sec' to be a int")
         pulumi.set(__self__, "refresh_sec", refresh_sec)
@@ -103,15 +103,15 @@
         """
         The group this Domain belongs to.
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
+    def id(self) -> Optional[int]:
         """
         The unique ID of this Domain.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="masterIps")
@@ -197,34 +197,34 @@
             status=self.status,
             tags=self.tags,
             ttl_sec=self.ttl_sec,
             type=self.type)
 
 
 def get_domain(domain: Optional[str] = None,
-               id: Optional[str] = None,
+               id: Optional[int] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainResult:
     """
     Provides information about a Linode domain.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode domain.
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    foo = linode.get_domain(id="1234567")
+    foo = linode.get_domain(id=1234567)
     bar = linode.get_domain(domain="bar.example.com")
     ```
 
 
     :param str domain: The unique domain name of the Domain record to query.
-    :param str id: The unique numeric ID of the Domain record to query.
+    :param int id: The unique numeric ID of the Domain record to query.
     """
     __args__ = dict()
     __args__['domain'] = domain
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
@@ -243,29 +243,29 @@
         tags=__ret__.tags,
         ttl_sec=__ret__.ttl_sec,
         type=__ret__.type)
 
 
 @_utilities.lift_output_func(get_domain)
 def get_domain_output(domain: Optional[pulumi.Input[Optional[str]]] = None,
-                      id: Optional[pulumi.Input[Optional[str]]] = None,
+                      id: Optional[pulumi.Input[Optional[int]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
     Provides information about a Linode domain.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode domain.
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    foo = linode.get_domain(id="1234567")
+    foo = linode.get_domain(id=1234567)
     bar = linode.get_domain(domain="bar.example.com")
     ```
 
 
     :param str domain: The unique domain name of the Domain record to query.
-    :param str id: The unique numeric ID of the Domain record to query.
+    :param int id: The unique numeric ID of the Domain record to query.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain_record.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_domain_zonefile.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_domain_zonefile.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,22 +39,19 @@
         The associated domain's unique ID.
         """
         return pulumi.get(self, "domain_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="zoneFiles")
-    def zone_files(self) -> Optional[Sequence[str]]:
+    def zone_files(self) -> Sequence[str]:
         """
         Array of strings representing the Domain Zonefile.
         """
         return pulumi.get(self, "zone_files")
 
 
 class AwaitableGetDomainZonefileResult(GetDomainZonefileResult):
@@ -65,15 +62,14 @@
         return GetDomainZonefileResult(
             domain_id=self.domain_id,
             id=self.id,
             zone_files=self.zone_files)
 
 
 def get_domain_zonefile(domain_id: Optional[int] = None,
-                        zone_files: Optional[Sequence[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainZonefileResult:
     """
     Provides information about a Linode Domain Zonefile.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode Domain Zonefile.
@@ -83,31 +79,28 @@
     import pulumi_linode as linode
 
     my_zonefile = linode.get_domain_zonefile(domain_id=3150401)
     ```
 
 
     :param int domain_id: The associated domain's unique ID.
-    :param Sequence[str] zone_files: Array of strings representing the Domain Zonefile.
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
-    __args__['zoneFiles'] = zone_files
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomainZonefile:getDomainZonefile', __args__, opts=opts, typ=GetDomainZonefileResult).value
 
     return AwaitableGetDomainZonefileResult(
         domain_id=__ret__.domain_id,
         id=__ret__.id,
         zone_files=__ret__.zone_files)
 
 
 @_utilities.lift_output_func(get_domain_zonefile)
 def get_domain_zonefile_output(domain_id: Optional[pulumi.Input[int]] = None,
-                               zone_files: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainZonefileResult]:
     """
     Provides information about a Linode Domain Zonefile.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode Domain Zonefile.
@@ -117,10 +110,9 @@
     import pulumi_linode as linode
 
     my_zonefile = linode.get_domain_zonefile(domain_id=3150401)
     ```
 
 
     :param int domain_id: The associated domain's unique ID.
-    :param Sequence[str] zone_files: Array of strings representing the Domain Zonefile.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_firewall.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_image.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_images.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_images.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_backups.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_networking.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_networking.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,14 @@
         if linode_id and not isinstance(linode_id, int):
             raise TypeError("Expected argument 'linode_id' to be a int")
         pulumi.set(__self__, "linode_id", linode_id)
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def ipv4s(self) -> Sequence['outputs.GetInstanceNetworkingIpv4Result']:
         return pulumi.get(self, "ipv4s")
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_type.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instance_types.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instance_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_instances.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ipv6_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,14 @@
         if region and not isinstance(region, str):
             raise TypeError("Expected argument 'region' to be a str")
         pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="isBgp")
     def is_bgp(self) -> bool:
         return pulumi.get(self, "is_bgp")
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_kernel.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_kernel.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_linode_object_storage_bucket.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_linode_object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_lke_versions.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_lke_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_networking_ip.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_networking_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_object_storage_cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -85,19 +85,15 @@
             domain=self.domain,
             id=self.id,
             region=self.region,
             static_site_domain=self.static_site_domain,
             status=self.status)
 
 
-def get_object_storage_cluster(domain: Optional[str] = None,
-                               id: Optional[str] = None,
-                               region: Optional[str] = None,
-                               static_site_domain: Optional[str] = None,
-                               status: Optional[str] = None,
+def get_object_storage_cluster(id: Optional[str] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetObjectStorageClusterResult:
     """
     Provides information about a Linode Object Storage Cluster
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode Object Storage Cluster.
@@ -106,43 +102,31 @@
     import pulumi
     import pulumi_linode as linode
 
     primary = linode.get_object_storage_cluster(id="us-east-1")
     ```
 
 
-    :param str domain: The base URL for this cluster.
     :param str id: The unique ID of this cluster.
-    :param str region: The region this cluster is located in. See all regions [here](https://api.linode.com/v4/regions).
-    :param str static_site_domain: The base URL for this cluster used when hosting static sites.
-    :param str status: This cluster's status. (`available`, `unavailable`)
     """
     __args__ = dict()
-    __args__['domain'] = domain
     __args__['id'] = id
-    __args__['region'] = region
-    __args__['staticSiteDomain'] = static_site_domain
-    __args__['status'] = status
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getObjectStorageCluster:getObjectStorageCluster', __args__, opts=opts, typ=GetObjectStorageClusterResult).value
 
     return AwaitableGetObjectStorageClusterResult(
         domain=__ret__.domain,
         id=__ret__.id,
         region=__ret__.region,
         static_site_domain=__ret__.static_site_domain,
         status=__ret__.status)
 
 
 @_utilities.lift_output_func(get_object_storage_cluster)
-def get_object_storage_cluster_output(domain: Optional[pulumi.Input[Optional[str]]] = None,
-                                      id: Optional[pulumi.Input[str]] = None,
-                                      region: Optional[pulumi.Input[Optional[str]]] = None,
-                                      static_site_domain: Optional[pulumi.Input[Optional[str]]] = None,
-                                      status: Optional[pulumi.Input[Optional[str]]] = None,
+def get_object_storage_cluster_output(id: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetObjectStorageClusterResult]:
     """
     Provides information about a Linode Object Storage Cluster
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode Object Storage Cluster.
@@ -151,14 +135,10 @@
     import pulumi
     import pulumi_linode as linode
 
     primary = linode.get_object_storage_cluster(id="us-east-1")
     ```
 
 
-    :param str domain: The base URL for this cluster.
     :param str id: The unique ID of this cluster.
-    :param str region: The region this cluster is located in. See all regions [here](https://api.linode.com/v4/regions).
-    :param str static_site_domain: The base URL for this cluster used when hosting static sites.
-    :param str status: This cluster's status. (`available`, `unavailable`)
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_profile.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_region.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_regions.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_regions.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,22 +38,19 @@
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.GetRegionsFilterResult']]:
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def regions(self) -> Sequence['outputs.GetRegionsRegionResult']:
+    def regions(self) -> Optional[Sequence['outputs.GetRegionsRegionResult']]:
         return pulumi.get(self, "regions")
 
 
 class AwaitableGetRegionsResult(GetRegionsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -61,14 +58,15 @@
         return GetRegionsResult(
             filters=self.filters,
             id=self.id,
             regions=self.regions)
 
 
 def get_regions(filters: Optional[Sequence[pulumi.InputType['GetRegionsFilterArgs']]] = None,
+                regions: Optional[Sequence[pulumi.InputType['GetRegionsRegionArgs']]] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegionsResult:
     """
     Provides information about Linode regions that match a set of filters.
 
     ```python
     import pulumi
     import pulumi_linode as linode
@@ -92,25 +90,27 @@
 
     * `country`
 
     * `capabilities`
     """
     __args__ = dict()
     __args__['filters'] = filters
+    __args__['regions'] = regions
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getRegions:getRegions', __args__, opts=opts, typ=GetRegionsResult).value
 
     return AwaitableGetRegionsResult(
         filters=__ret__.filters,
         id=__ret__.id,
         regions=__ret__.regions)
 
 
 @_utilities.lift_output_func(get_regions)
 def get_regions_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionsFilterArgs']]]]] = None,
+                       regions: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionsRegionArgs']]]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionsResult]:
     """
     Provides information about Linode regions that match a set of filters.
 
     ```python
     import pulumi
     import pulumi_linode as linode
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_ssh_key.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_ssh_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         """
         The date this key was added.
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def id(self) -> Optional[str]:
         """
-        The provider-assigned unique ID for this managed resource.
+        The ID of the SSH Key
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def label(self) -> str:
         return pulumi.get(self, "label")
@@ -73,15 +73,16 @@
         return GetSshKeyResult(
             created=self.created,
             id=self.id,
             label=self.label,
             ssh_key=self.ssh_key)
 
 
-def get_ssh_key(label: Optional[str] = None,
+def get_ssh_key(id: Optional[str] = None,
+                label: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSshKeyResult:
     """
     `SshKey` provides access to a specifically labeled SSH Key in the Profile of the User identified by the access token.
 
     ## Example Usage
 
     The following example shows how the resource might be used to obtain the name of the SSH Key configured on the Linode user profile.
@@ -90,30 +91,33 @@
     import pulumi
     import pulumi_linode as linode
 
     foo = linode.get_ssh_key(label="foo")
     ```
 
 
+    :param str id: The ID of the SSH Key
     :param str label: The label of the SSH Key to select.
     """
     __args__ = dict()
+    __args__['id'] = id
     __args__['label'] = label
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getSshKey:getSshKey', __args__, opts=opts, typ=GetSshKeyResult).value
 
     return AwaitableGetSshKeyResult(
         created=__ret__.created,
         id=__ret__.id,
         label=__ret__.label,
         ssh_key=__ret__.ssh_key)
 
 
 @_utilities.lift_output_func(get_ssh_key)
-def get_ssh_key_output(label: Optional[pulumi.Input[str]] = None,
+def get_ssh_key_output(id: Optional[pulumi.Input[Optional[str]]] = None,
+                       label: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshKeyResult]:
     """
     `SshKey` provides access to a specifically labeled SSH Key in the Profile of the User identified by the access token.
 
     ## Example Usage
 
     The following example shows how the resource might be used to obtain the name of the SSH Key configured on the Linode user profile.
@@ -122,10 +126,11 @@
     import pulumi
     import pulumi_linode as linode
 
     foo = linode.get_ssh_key(label="foo")
     ```
 
 
+    :param str id: The ID of the SSH Key
     :param str label: The label of the SSH Key to select.
     """
     ...
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_stack_script.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_stack_scripts.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_user.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_vlans.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_vlans.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/get_volume.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/image.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/instance.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_disk.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_ip.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/instance_shared_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/ipv6_range.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/lke_cluster.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer_config.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/node_balancer_node.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/node_balancer_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,56 +251,14 @@
                  nodebalancer_id: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Provides a Linode NodeBalancer Node resource.  This can be used to create, modify, and delete Linodes NodeBalancer Nodes.
         For more information, see [Getting Started with NodeBalancers](https://www.linode.com/docs/platform/nodebalancer/getting-started-with-nodebalancers/) and the [Linode APIv4 docs](https://developers.linode.com/api/v4#operation/createNodeBalancerNode).
 
-        ## Example Usage
-
-        The following example shows how one might use this resource to configure NodeBalancer Nodes attached to Linode instances.
-
-        ```python
-        import pulumi
-        import pulumi_linode as linode
-
-        web = []
-        for range in [{"value": i} for i in range(0, 3)]:
-            web.append(linode.Instance(f"web-{range['value']}",
-                label=f"web-{range['value'] + 1}",
-                image="linode/ubuntu18.04",
-                region="us-east",
-                type="g6-standard-1",
-                authorized_keys=["ssh-rsa AAAA...Gw== user@example.local"],
-                root_pass="test",
-                private_ip=True))
-        foobar = linode.NodeBalancer("foobar",
-            label="mynodebalancer",
-            region="us-east",
-            client_conn_throttle=20)
-        foofig = linode.NodeBalancerConfig("foofig",
-            nodebalancer_id=foobar.id,
-            port=80,
-            protocol="http",
-            check="http",
-            check_path="/foo",
-            check_attempts=3,
-            check_timeout=30,
-            stickiness="http_cookie",
-            algorithm="source")
-        foonode = []
-        for range in [{"value": i} for i in range(0, 3)]:
-            foonode.append(linode.NodeBalancerNode(f"foonode-{range['value']}",
-                nodebalancer_id=foobar.id,
-                config_id=foofig.id,
-                address=[__item.private_ip_address for __item in web][range["value"]].apply(lambda private_ip_addresses: f"{private_ip_addresses}:80"),
-                label="mynodebalancernode",
-                weight=50))
-        ```
-
         ## Import
 
         NodeBalancer Nodes can be imported using the NodeBalancer `nodebalancer_id` followed by the NodeBalancer Config `config_id` followed by the NodeBalancer Node `id`, separated by a comma, e.g.
 
         ```sh
          $ pulumi import linode:index/nodeBalancerNode:NodeBalancerNode https-foobar-1 1234567,7654321,9999999
         ```
@@ -324,56 +282,14 @@
                  resource_name: str,
                  args: NodeBalancerNodeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Linode NodeBalancer Node resource.  This can be used to create, modify, and delete Linodes NodeBalancer Nodes.
         For more information, see [Getting Started with NodeBalancers](https://www.linode.com/docs/platform/nodebalancer/getting-started-with-nodebalancers/) and the [Linode APIv4 docs](https://developers.linode.com/api/v4#operation/createNodeBalancerNode).
 
-        ## Example Usage
-
-        The following example shows how one might use this resource to configure NodeBalancer Nodes attached to Linode instances.
-
-        ```python
-        import pulumi
-        import pulumi_linode as linode
-
-        web = []
-        for range in [{"value": i} for i in range(0, 3)]:
-            web.append(linode.Instance(f"web-{range['value']}",
-                label=f"web-{range['value'] + 1}",
-                image="linode/ubuntu18.04",
-                region="us-east",
-                type="g6-standard-1",
-                authorized_keys=["ssh-rsa AAAA...Gw== user@example.local"],
-                root_pass="test",
-                private_ip=True))
-        foobar = linode.NodeBalancer("foobar",
-            label="mynodebalancer",
-            region="us-east",
-            client_conn_throttle=20)
-        foofig = linode.NodeBalancerConfig("foofig",
-            nodebalancer_id=foobar.id,
-            port=80,
-            protocol="http",
-            check="http",
-            check_path="/foo",
-            check_attempts=3,
-            check_timeout=30,
-            stickiness="http_cookie",
-            algorithm="source")
-        foonode = []
-        for range in [{"value": i} for i in range(0, 3)]:
-            foonode.append(linode.NodeBalancerNode(f"foonode-{range['value']}",
-                nodebalancer_id=foobar.id,
-                config_id=foofig.id,
-                address=[__item.private_ip_address for __item in web][range["value"]].apply(lambda private_ip_addresses: f"{private_ip_addresses}:80"),
-                label="mynodebalancernode",
-                weight=50))
-        ```
-
         ## Import
 
         NodeBalancer Nodes can be imported using the NodeBalancer `nodebalancer_id` followed by the NodeBalancer Config `config_id` followed by the NodeBalancer Node `id`, separated by a comma, e.g.
 
         ```sh
          $ pulumi import linode:index/nodeBalancerNode:NodeBalancerNode https-foobar-1 1234567,7654321,9999999
         ```
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_key.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/object_storage_object.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/object_storage_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/outputs.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4274,31 +4274,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv4PrivateResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4313,23 +4319,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -4358,31 +4380,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv4PublicResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4397,23 +4425,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -4442,31 +4486,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv4ReservedResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4481,23 +4531,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -4526,31 +4592,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv4SharedResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4565,23 +4637,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -4609,34 +4697,34 @@
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv6Result(dict):
     def __init__(__self__, *,
                  globals: Sequence['outputs.GetInstanceNetworkingIpv6GlobalResult'],
-                 link_locals: Sequence['outputs.GetInstanceNetworkingIpv6LinkLocalResult'],
-                 slaacs: Sequence['outputs.GetInstanceNetworkingIpv6SlaacResult']):
+                 link_local: 'outputs.GetInstanceNetworkingIpv6LinkLocalResult',
+                 slaac: 'outputs.GetInstanceNetworkingIpv6SlaacResult'):
         pulumi.set(__self__, "globals", globals)
-        pulumi.set(__self__, "link_locals", link_locals)
-        pulumi.set(__self__, "slaacs", slaacs)
+        pulumi.set(__self__, "link_local", link_local)
+        pulumi.set(__self__, "slaac", slaac)
 
     @property
     @pulumi.getter
     def globals(self) -> Sequence['outputs.GetInstanceNetworkingIpv6GlobalResult']:
         return pulumi.get(self, "globals")
 
     @property
-    @pulumi.getter(name="linkLocals")
-    def link_locals(self) -> Sequence['outputs.GetInstanceNetworkingIpv6LinkLocalResult']:
-        return pulumi.get(self, "link_locals")
+    @pulumi.getter(name="linkLocal")
+    def link_local(self) -> 'outputs.GetInstanceNetworkingIpv6LinkLocalResult':
+        return pulumi.get(self, "link_local")
 
     @property
     @pulumi.getter
-    def slaacs(self) -> Sequence['outputs.GetInstanceNetworkingIpv6SlaacResult']:
-        return pulumi.get(self, "slaacs")
+    def slaac(self) -> 'outputs.GetInstanceNetworkingIpv6SlaacResult':
+        return pulumi.get(self, "slaac")
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv6GlobalResult(dict):
     def __init__(__self__, *,
                  prefix: int,
                  range: str,
@@ -4687,31 +4775,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv6LinkLocalResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4726,23 +4820,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -4771,31 +4881,37 @@
 
 
 @pulumi.output_type
 class GetInstanceNetworkingIpv6SlaacResult(dict):
     def __init__(__self__, *,
                  address: str,
                  gateway: str,
+                 linode_id: int,
                  prefix: int,
+                 public: bool,
                  rdns: str,
                  region: str,
                  subnet_mask: str,
                  type: str):
         """
         :param str address: The address.
         :param str gateway: The default gateway for this address.
+        :param int linode_id: The Linode instance's ID.
         :param int prefix: The network prefix.
+        :param bool public: Whether this is a public or private IP address.
         :param str rdns: The reverse DNS assigned to this address.
         :param str region: (Filterable) The Region this address resides in.
         :param str subnet_mask: The subnet mask.
         :param str type: The type of address this is.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "gateway", gateway)
+        pulumi.set(__self__, "linode_id", linode_id)
         pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "rdns", rdns)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subnet_mask", subnet_mask)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
@@ -4810,23 +4926,39 @@
     def gateway(self) -> str:
         """
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
+    @pulumi.getter(name="linodeId")
+    def linode_id(self) -> int:
+        """
+        The Linode instance's ID.
+        """
+        return pulumi.get(self, "linode_id")
+
+    @property
     @pulumi.getter
     def prefix(self) -> int:
         """
         The network prefix.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
+    def public(self) -> bool:
+        """
+        Whether this is a public or private IP address.
+        """
+        return pulumi.get(self, "public")
+
+    @property
+    @pulumi.getter
     def rdns(self) -> str:
         """
         The reverse DNS assigned to this address.
         """
         return pulumi.get(self, "rdns")
 
     @property
@@ -6527,28 +6659,29 @@
 @pulumi.output_type
 class GetRegionsRegionResult(dict):
     def __init__(__self__, *,
                  capabilities: Sequence[str],
                  country: str,
                  id: str,
                  label: str,
-                 resolvers: Sequence['outputs.GetRegionsRegionResolverResult'],
-                 status: str):
+                 status: str,
+                 resolvers: Optional[Sequence['outputs.GetRegionsRegionResolverResult']] = None):
         """
         :param Sequence[str] capabilities: A list of capabilities of this region.
         :param str country: The country the region resides in.
         :param str label: Detailed location information for this Region, including city, state or region, and country.
         :param str status: This region’s current operational status (ok or outage).
         """
         pulumi.set(__self__, "capabilities", capabilities)
         pulumi.set(__self__, "country", country)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "resolvers", resolvers)
         pulumi.set(__self__, "status", status)
+        if resolvers is not None:
+            pulumi.set(__self__, "resolvers", resolvers)
 
     @property
     @pulumi.getter
     def capabilities(self) -> Sequence[str]:
         """
         A list of capabilities of this region.
         """
@@ -6573,25 +6706,25 @@
         """
         Detailed location information for this Region, including city, state or region, and country.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
-    def resolvers(self) -> Sequence['outputs.GetRegionsRegionResolverResult']:
-        return pulumi.get(self, "resolvers")
-
-    @property
-    @pulumi.getter
     def status(self) -> str:
         """
         This region’s current operational status (ok or outage).
         """
         return pulumi.get(self, "status")
 
+    @property
+    @pulumi.getter
+    def resolvers(self) -> Optional[Sequence['outputs.GetRegionsRegionResolverResult']]:
+        return pulumi.get(self, "resolvers")
+
 
 @pulumi.output_type
 class GetRegionsRegionResolverResult(dict):
     def __init__(__self__, *,
                  ipv4: str,
                  ipv6: str):
         """
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/provider.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/rdns.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/ssh_key.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/stack_script.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/token.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/user.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode/volume.py` & `pulumi_linode-4.3.0a1687424922/pulumi_linode/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-linode
-Version: 4.3.0a1687055232
+Version: 4.3.0a1687424922
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.3.0a1687055232/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-4.3.0a1687424922/pulumi_linode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.3.0a1687055232/setup.py` & `pulumi_linode-4.3.0a1687424922/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.3.0a1687055232"
-PLUGIN_VERSION = "4.3.0-alpha.1687055232+65412787"
+VERSION = "4.3.0a1687424922"
+PLUGIN_VERSION = "4.3.0-alpha.1687424922+8a494834"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'linode', PLUGIN_VERSION])
         except OSError as error:
```

