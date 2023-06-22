# Comparing `tmp/ovs-cluster-agent-2.2.2.tar.gz` & `tmp/ovs-cluster-agent-2.2.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-cluster-agent-2.2.2.tar", last modified: Tue Feb 28 19:32:14 2023, max compression
+gzip compressed data, was "ovs-cluster-agent-2.2.3rc1.tar", last modified: Thu Jun 22 17:31:14 2023, max compression
```

## Comparing `ovs-cluster-agent-2.2.2.tar` & `ovs-cluster-agent-2.2.3rc1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.329350 ovs-cluster-agent-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-28 19:32:14.329350 ovs-cluster-agent-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/cluster_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/mapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/single_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/identity/slurmrestd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/scripts/agentconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/cluster_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/cluster_agent/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-28 19:32:14.000000 ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 19:32:14.329350 ovs-cluster-agent-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.325350 ovs-cluster-agent-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.329350 ovs-cluster-agent-2.2.2/tests/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/identity/test_cluster_api_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/identity/test_slurmrestd_identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:14.329350 ovs-cluster-agent-2.2.2/tests/jobbergate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/jobbergate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/jobbergate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/jobbergate/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/jobbergate/test_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/jobbergate/test_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-28 19:32:07.000000 ovs-cluster-agent-2.2.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/cluster_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/mapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/single_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurmrestd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/agentconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-22 17:31:14.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/tests/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/test_cluster_api_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/test_slurmrestd_identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_settings.py
```

### Comparing `ovs-cluster-agent-2.2.2/LICENSE` & `ovs-cluster-agent-2.2.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/PKG-INFO` & `ovs-cluster-agent-2.2.3rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ovs-cluster-agent
-Version: 2.2.2
+Version: 2.2.3rc1
 Summary: Cluster API data aggregator
 Home-page: https://github.com/omnivector-solutions/ovs-cluster-agent/
 Author: omnivector-solutions
 Author-email: info@omnivector.solutions
 License: MIT
-Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.2tar.gz
+Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3-rc.1tar.gz
 Description: # cluster-agent
         
         # Table of contents
         
         - [Project setup](#project-setup)
           - [Dependencies](#dependencies)
         - [Install the package](#install-the-package)
```

### Comparing `ovs-cluster-agent-2.2.2/README.md` & `ovs-cluster-agent-2.2.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/agent.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 from cluster_agent.identity.cluster_api import backend_client as cluster_api_client
 from cluster_agent.identity.slurmrestd import backend_client as slurmrestd_client
 
 import hostlist
 
 
 async def upsert_partitions():
-
-    r = await slurmrestd_client.get("/slurm/v0.0.36/partitions")
+    r = await slurmrestd_client.get("/partitions")
     SlurmrestdError.require_condition(
         r.status_code == 200,
         f"Slurmrestd returned {r.status_code} when calling {r.url}: {r.text}",
     )
     partitions = r.json()
 
     tasks = list()
 
     for partition in partitions["partitions"]:
-
         # transform nodes names string into a list
         # e.g. "juju-54c58e-[67,45]" -> ["juju-54c58e-67", "juju-54c58e-45"]
         partition["nodes"] = hostlist.expand_hostlist(partition["nodes"])
 
         payload = {
             "meta": partitions["meta"],
             "errors": partitions["errors"],
@@ -40,26 +38,24 @@
     responses = await asyncio.gather(*tasks)
 
     # return a list containing just the responses' status, e.g. [200, 400]
     return [response.status_code for response in responses]
 
 
 async def upsert_nodes():
-
-    r = await slurmrestd_client.get("/slurm/v0.0.36/nodes")
+    r = await slurmrestd_client.get("/nodes")
     SlurmrestdError.require_condition(
         r.status_code == 200,
         f"Slurmrestd returned {r.status_code} when calling {r.url}: {r.text}",
     )
     nodes = r.json()
 
     tasks = list()
 
     for node in nodes["nodes"]:
-
         payload = {
             "meta": nodes["meta"],
             "errors": nodes["errors"],
             "node": node,
         }
 
         tasks.append(
@@ -72,40 +68,39 @@
     responses = await asyncio.gather(*tasks)
 
     # return a list containing just the responses' status, e.g. [200, 400]
     return [response.status_code for response in responses]
 
 
 async def update_diagnostics():
-
-    r = await slurmrestd_client.get("/slurm/v0.0.36/diag/")
+    r = await slurmrestd_client.get("/diag/")
     SlurmrestdError.require_condition(
         r.status_code == 200,
         f"Slurmrestd returned {r.status_code} when calling {r.url}: {r.text}",
     )
     diagnostics = r.json()
 
-    response = await cluster_api_client.post("/cluster/agent/diagnostics", json=diagnostics)
+    response = await cluster_api_client.post(
+        "/cluster/agent/diagnostics", json=diagnostics
+    )
 
     return response.status_code
 
 
 async def upsert_jobs():
-
-    r = await slurmrestd_client.get("/slurm/v0.0.36/jobs")
+    r = await slurmrestd_client.get("/jobs")
     SlurmrestdError.require_condition(
         r.status_code == 200,
         f"Slurmrestd returned {r.status_code} when calling {r.url}: {r.text}",
     )
     jobs = r.json()
 
     tasks = list()
 
     for job in jobs["jobs"]:
-
         payload = {
             "meta": jobs["meta"],
             "errors": jobs["errors"],
             "job": job,
         }
 
         tasks.append(
```

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/cluster_api.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/cluster_api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/factory.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/factory.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/ldap.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/ldap.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/mapper_base.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/mapper_base.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/slurm_user/mappers/single_user.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/single_user.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/identity/slurmrestd.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurmrestd.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,20 @@
     The token is acquired lazily on the first httpx request issued.
     This client should be used for most agent actions.
     """
 
     _token: typing.Optional[str]
 
     def __init__(self):
+        if SETTINGS.SLURM_RESTD_VERSIONED_URL is None:
+            raise ValueError(
+                "SLURM_RESTD_VERSIONED_URL must be set in order to use the AsyncBackendClient"
+            )
         super().__init__(
-            base_url=SETTINGS.BASE_SLURMRESTD_URL,
+            base_url=SETTINGS.SLURM_RESTD_VERSIONED_URL,
             auth=inject_token,
             event_hooks=dict(
                 request=[self._log_request],
                 response=[self._log_response],
             ),
         )
```

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/api.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/constants.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/constants.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/finish.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/finish.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 from cluster_agent.jobbergate.constants import JobSubmissionStatus
 from cluster_agent.jobbergate.schemas import SlurmSubmittedJobStatus
 from cluster_agent.utils.exception import SlurmrestdError
 from cluster_agent.utils.logging import log_error
 
 
 async def fetch_job_status(slurm_job_id: int) -> SlurmSubmittedJobStatus:
-
     logger.debug(f"Fetching slurm job status for slurm job {slurm_job_id}")
 
     with SlurmrestdError.handle_errors(
         "Failed to fetch job status from slurm",
         do_except=log_error,
     ):
-        response = await slurmrestd_client.get(f"/slurm/v0.0.36/job/{slurm_job_id}")
+        response = await slurmrestd_client.get(f"/job/{slurm_job_id}")
         response.raise_for_status()
         data = response.json()
 
     jobs = data["jobs"]
     SlurmrestdError.require_condition(
         len(jobs) == 1,
         f"Couldn't find a slurm job matching id {slurm_job_id}",
```

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/schemas.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/jobbergate/submit.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     )
 
     async with handle_errors_async(
         "An internal error occurred while processing the job-submission",
         raise_exc_class=JobSubmissionError,
         do_except=notify_submission_rejected.report_error,
     ):
-
         email = pending_job_submission.job_submission_owner_email
         name = pending_job_submission.application_name
         mapper_class_name = user_mapper.__class__.__name__
         logger.debug(
             f"Fetching username for email {email} with mapper {mapper_class_name}"
         )
         username = await user_mapper.find_username(email)
@@ -110,15 +109,14 @@
             logger.debug(f"Copied job script file to {local_script_path}")
 
     async with handle_errors_async(
         "Failed to extract Slurm parameters",
         raise_exc_class=SlurmParameterParserError,
         do_except=notify_submission_rejected.report_error,
     ):
-
         job_parameters = get_job_parameters(
             pending_job_submission.execution_parameters,
             name=pending_job_submission.application_name,
             current_working_directory=submit_dir,
             standard_output=submit_dir / f"{name}.out",
             standard_error=submit_dir / f"{name}.err",
         )
@@ -131,19 +129,19 @@
 
     async with handle_errors_async(
         "Failed to submit job to slurm",
         raise_exc_class=SlurmrestdError,
         do_except=notify_submission_rejected.report_error,
     ):
         response = await slurmrestd_client.post(
-            "/slurm/v0.0.36/job/submit",
+            "/job/submit",
             auth=lambda r: inject_token(r, username=username),
             json=json.loads(payload.json()),
         )
-        logger.debug(f"Slurmrestd response: {response.json()}")
+        logger.debug(f"Slurmrestd response: {response.text}")
         sub_data = SlurmSubmitResponse.parse_raw(response.content)
         with handle_errors(unpack_error_from_slurm_response(sub_data)):
             response.raise_for_status()
 
     # Make static type checkers happy.
     slurm_job_id = cast(int, sub_data.job_id)
 
@@ -177,13 +175,12 @@
             ),
             do_except=log_error,
             do_else=lambda: logger.debug(
                 f"Finished submitting pending job_submission {pending_job_submission.id}"
             ),
             re_raise=False,
         ):
-
             slurm_job_id = await submit_job_script(pending_job_submission, user_mapper)
 
             await mark_as_submitted(pending_job_submission.id, slurm_job_id)
 
     logger.debug("...Finished submitting pending jobs")
```

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/main.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/main.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/scripts/agentconfig.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/agentconfig.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/settings.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 from pathlib import Path
 from typing import Optional
 
 import buzz
 from pydantic import AnyHttpUrl, BaseSettings, Field, root_validator
 from pydantic.error_wrappers import ValidationError
 
-from cluster_agent.identity.slurm_user.constants import (
-    LDAPAuthType,
-    MapperType,
-)
+from cluster_agent.identity.slurm_user.constants import LDAPAuthType, MapperType
 from cluster_agent.utils.logging import logger
 
 
 class Settings(BaseSettings):
     # slurmrestd info
     BASE_SLURMRESTD_URL: AnyHttpUrl = Field("http://127.0.0.1:6820")
+    SLURM_RESTD_VERSION: str = "v0.0.36"
+    SLURM_RESTD_VERSIONED_URL: Optional[AnyHttpUrl] = None
     X_SLURM_USER_NAME: str = "ubuntu"
     X_SLURM_USER_TOKEN: Optional[str]
     DEFAULT_SLURM_WORK_DIR: Path = Path("/tmp")
 
     # Slurmrestd authentication
     SLURMRESTD_JWT_KEY_PATH: Optional[str]
     SLURMRESTD_JWT_KEY_STRING: Optional[str]
@@ -55,14 +54,20 @@
     SINGLE_USER_SUBMITTER: Optional[str]
 
     @root_validator
     def compute_extra_settings(cls, values):
         """
         Compute settings values that are based on other settings values.
         """
+        if values.get("SLURM_RESTD_VERSIONED_URL") is None:
+            values["SLURM_RESTD_VERSIONED_URL"] = "{base}/slurm/{version}".format(
+                base=values["BASE_SLURMRESTD_URL"],
+                version=values["SLURM_RESTD_VERSION"],
+            )
+
         ldap_host = values["LDAP_HOST"]
         ldap_domain = values["LDAP_DOMAIN"]
 
         # Just use the LDAP domain as the host if host is not set but domain is
         if ldap_domain is not None and ldap_host is None:
             values["LDAP_HOST"] = ldap_domain
```

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/utils/exception.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/cluster_agent/utils/logging.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/PKG-INFO` & `ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ovs-cluster-agent
-Version: 2.2.2
+Version: 2.2.3rc1
 Summary: Cluster API data aggregator
 Home-page: https://github.com/omnivector-solutions/ovs-cluster-agent/
 Author: omnivector-solutions
 Author-email: info@omnivector.solutions
 License: MIT
-Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.2tar.gz
+Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3-rc.1tar.gz
 Description: # cluster-agent
         
         # Table of contents
         
         - [Project setup](#project-setup)
           - [Dependencies](#dependencies)
         - [Install the package](#install-the-package)
```

### Comparing `ovs-cluster-agent-2.2.2/ovs_cluster_agent.egg-info/SOURCES.txt` & `ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 ovs_cluster_agent.egg-info/entry_points.txt
 ovs_cluster_agent.egg-info/requires.txt
 ovs_cluster_agent.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_agent.py
 tests/test_main.py
+tests/test_settings.py
 tests/identity/__init__.py
 tests/identity/test_cluster_api_identity.py
 tests/identity/test_slurmrestd_identity.py
 tests/jobbergate/__init__.py
 tests/jobbergate/conftest.py
 tests/jobbergate/test_api.py
 tests/jobbergate/test_finish.py
```

### Comparing `ovs-cluster-agent-2.2.2/setup.py` & `ovs-cluster-agent-2.2.3rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os.path import dirname, join
 
 here = dirname(__file__)
 
-_VERSION = "2.2.2"
+_VERSION = "2.2.3-rc.1"
 
 setup(
     name="ovs-cluster-agent",
     version=_VERSION,
     description="Cluster API data aggregator",
     long_description=open(join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
```

### Comparing `ovs-cluster-agent-2.2.2/tests/conftest.py` & `ovs-cluster-agent-2.2.3rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/tests/identity/test_cluster_api_identity.py` & `ovs-cluster-agent-2.2.3rc1/tests/identity/test_cluster_api_identity.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/tests/identity/test_slurmrestd_identity.py` & `ovs-cluster-agent-2.2.3rc1/tests/identity/test_slurmrestd_identity.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/tests/jobbergate/conftest.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/conftest.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/tests/jobbergate/test_api.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.2/tests/jobbergate/test_finish.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_finish.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         respx.post(
             f"https://{SETTINGS.OIDC_DOMAIN}/protocol/openid-connect/token"
         ).mock(
             return_value=httpx.Response(
                 status_code=200, json=dict(access_token="dummy-token")
             )
         )
-        respx.get(f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/{slurm_id}").mock(
+        respx.get(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/{slurm_id}").mock(
             return_value=httpx.Response(
                 status_code=200,
                 json=dict(
                     jobs=[
                         dict(
                             job_state=slurm_status,
                             job_id=slurm_id,
@@ -70,15 +70,15 @@
         respx.post(
             f"https://{SETTINGS.OIDC_DOMAIN}/protocol/openid-connect/token"
         ).mock(
             return_value=httpx.Response(
                 status_code=200, json=dict(access_token="dummy-token")
             )
         )
-        respx.get(f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/11").mock(
+        respx.get(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/11").mock(
             return_value=httpx.Response(status_code=400)
         )
         with pytest.raises(
             SlurmrestdError, match="Failed to fetch job status from slurm"
         ):
             await fetch_job_status(11)
 
@@ -133,15 +133,15 @@
                     else [
                         dict(job_state=mapper[slurm_job_id]),
                     ],
                 ),
             )
 
         slurm_route = respx.get(
-            url__regex=rf"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/\d+"
+            url__regex=rf"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/\d+"
         )
         slurm_route.mock(side_effect=_map_slurm_request)
 
         def _map_update_request(request: httpx.Request):
             job_submission_id = int(request.url.path.split("/")[-1])
             return httpx.Response(status_code=400 if job_submission_id == 2 else 200)
```

### Comparing `ovs-cluster-agent-2.2.2/tests/jobbergate/test_submit.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,15 @@
     user_mapper = mocker.AsyncMock(SlurmUserMapper)
     user_mapper.find_username.return_value = "dummy-user"
 
     pending_job_submission = PendingJobSubmission(**dummy_pending_job_submission_data)
     name = pending_job_submission.application_name
 
     async with respx.mock:
-        submit_route = respx.post(
-            f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/submit"
-        )
+        submit_route = respx.post(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/submit")
         submit_route.mock(
             return_value=httpx.Response(
                 status_code=200,
                 json=dict(job_id=13),
             )
         )
 
@@ -150,17 +148,15 @@
         name=pending_job_submission.application_name,
         current_working_directory=exe_path,
         standard_output=exe_path / f"{name}.out",
         standard_error=exe_path / f"{name}.err",
     )
 
     async with respx.mock:
-        submit_route = respx.post(
-            f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/submit"
-        )
+        submit_route = respx.post(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/submit")
         submit_route.mock(
             return_value=httpx.Response(
                 status_code=200,
                 json=dict(job_id=13),
             )
         )
 
@@ -235,17 +231,15 @@
             )
         )
         update_route = respx.put(
             f"{SETTINGS.BASE_API_URL}/jobbergate/job-submissions/agent/{pending_job_submission.id}"
         )
         update_route.mock(return_value=httpx.Response(status_code=200))
 
-        submit_route = respx.post(
-            f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/submit"
-        )
+        submit_route = respx.post(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/submit")
         submit_route.mock(
             return_value=httpx.Response(
                 status_code=400,
                 json=dict(
                     errors=[
                         dict(
                             error="BOOM!",
@@ -288,17 +282,15 @@
             )
         )
         update_route = respx.put(
             f"{SETTINGS.BASE_API_URL}/jobbergate/job-submissions/agent/{pending_job_submission.id}"
         )
         update_route.mock(return_value=httpx.Response(status_code=200))
 
-        submit_route = respx.post(
-            f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/submit"
-        )
+        submit_route = respx.post(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/submit")
         submit_route.mock(
             return_value=httpx.Response(
                 status_code=200,
                 content="BAD DATA",
             )
         )
 
@@ -388,17 +380,15 @@
                 )
             else:
                 return httpx.Response(
                     status_code=200,
                     json=dict(job_id=fake_slurm_job_id),
                 )
 
-        submit_route = respx.post(
-            f"{SETTINGS.BASE_SLURMRESTD_URL}/slurm/v0.0.36/job/submit"
-        )
+        submit_route = respx.post(f"{SETTINGS.SLURM_RESTD_VERSIONED_URL}/job/submit")
         submit_route.mock(side_effect=_submit_side_effect)
 
         with tweak_settings(SINGLE_USER_SUBMITTER="dummy-user"):
             await submit_pending_jobs()
 
         assert update_1_route.call_count == 1
         assert update_1_route.calls.last.request.content == json.dumps(
```

### Comparing `ovs-cluster-agent-2.2.2/tests/test_agent.py` & `ovs-cluster-agent-2.2.3rc1/tests/test_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         "partitions": [{"nodes": nodes_names_string, "name": partition_name}],
     }
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.json.return_value = mock_response_body
     mock_slurmrestd_client.get.return_value.status_code = 200
     mock_slurmrestd_client.get.return_value.url = (
-        SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/partitions"
+        SETTINGS.SLURM_RESTD_VERSIONED_URL + "/partitions"
     )
     mock_slurmrestd_client.get.return_value.text = "no error"
 
     mock_response_status = mock.Mock()
     mock_response_status.status_code = 200
 
     mock_asyncio.gather = asynctest.CoroutineMock()
@@ -75,15 +75,15 @@
                 errors=list(),
                 partition=dict(
                     nodes=expand_hostlist(nodes_names_string), name=partition_name
                 ),
             ),
         )
     ]
-    mock_slurmrestd_client.get.assert_awaited_with("/slurm/v0.0.36/partitions")
+    mock_slurmrestd_client.get.assert_awaited_with("/partitions")
     mock_asyncio.gather.assert_awaited_once()
     assert test_response == [200]
 
 
 @mock.patch("cluster_agent.agent.asyncio")
 @mock.patch("cluster_agent.agent.cluster_api_client")
 @mock.patch("cluster_agent.agent.slurmrestd_client")
@@ -93,15 +93,15 @@
     mock_slurmrestd_client, mock_cluster_api_client, mock_asyncio, response_status_code
 ):
     """
     Verify if an error is raised in case the slurmrestd request fails
     """
 
     error_message = "dummy error message"
-    url = SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/partitions"
+    url = SETTINGS.SLURM_RESTD_VERSIONED_URL + "/partitions"
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.status_code = response_status_code
     mock_slurmrestd_client.get.return_value.url = url
     mock_slurmrestd_client.get.return_value.text = error_message
 
     mock_response_status = mock.Mock()
@@ -143,15 +143,15 @@
         "nodes": [{"node": dict(), "name": node_name}],
     }
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.json.return_value = mock_response_body
     mock_slurmrestd_client.get.return_value.status_code = 200
     mock_slurmrestd_client.get.return_value.url = (
-        SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/nodes"
+        SETTINGS.SLURM_RESTD_VERSIONED_URL + "/nodes"
     )
     mock_slurmrestd_client.get.return_value.text = "no error"
 
     mock_response_status = mock.Mock()
     mock_response_status.status_code = 200
 
     mock_asyncio.gather = asynctest.CoroutineMock()
@@ -167,15 +167,15 @@
             json=dict(
                 meta=dict(),
                 errors=list(),
                 node=dict(node=dict(), name=node_name),
             ),
         )
     ]
-    mock_slurmrestd_client.get.assert_awaited_with("/slurm/v0.0.36/nodes")
+    mock_slurmrestd_client.get.assert_awaited_with("/nodes")
     mock_asyncio.gather.assert_awaited_once()
     assert test_response == [200]
 
 
 @mock.patch("cluster_agent.agent.asyncio")
 @mock.patch("cluster_agent.agent.cluster_api_client")
 @mock.patch("cluster_agent.agent.slurmrestd_client")
@@ -185,15 +185,15 @@
     mock_slurmrestd_client, mock_cluster_api_client, mock_asyncio, response_status_code
 ):
     """
     Verify if an error is raised in case the slurmrestd request fails
     """
 
     error_message = "dummy error message"
-    url = SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/nodes"
+    url = SETTINGS.SLURM_RESTD_VERSIONED_URL + "/nodes"
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.status_code = response_status_code
     mock_slurmrestd_client.get.return_value.url = url
     mock_slurmrestd_client.get.return_value.text = error_message
 
     mock_response_status = mock.Mock()
@@ -231,27 +231,27 @@
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.json.return_value = (
         mock_diagnostics_response_body
     )
     mock_slurmrestd_client.get.return_value.status_code = 200
     mock_slurmrestd_client.get.return_value.url = (
-        SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/diag/"
+        SETTINGS.SLURM_RESTD_VERSIONED_URL + "/diag/"
     )
     mock_slurmrestd_client.get.return_value.text = "no error"
 
     mock_cluster_api_client.post = asynctest.CoroutineMock()
     mock_cluster_api_client.post.return_value.status_code = 200
 
     test_response = await update_diagnostics()
 
     mock_cluster_api_client.post.assert_awaited_once_with(
         "/cluster/agent/diagnostics", json=mock_diagnostics_response_body
     )
-    mock_slurmrestd_client.get.assert_awaited_once_with("/slurm/v0.0.36/diag/")
+    mock_slurmrestd_client.get.assert_awaited_once_with("/diag/")
 
     assert test_response == 200
 
 
 @mock.patch("cluster_agent.agent.asyncio")
 @mock.patch("cluster_agent.agent.cluster_api_client")
 @mock.patch("cluster_agent.agent.slurmrestd_client")
@@ -261,15 +261,15 @@
     mock_slurmrestd_client, mock_cluster_api_client, mock_asyncio, response_status_code
 ):
     """
     Verify if an error is raised in case the slurmrestd request fails
     """
 
     error_message = "dummy error message"
-    url = SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/diag/"
+    url = SETTINGS.SLURM_RESTD_VERSIONED_URL + "/diag/"
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.status_code = response_status_code
     mock_slurmrestd_client.get.return_value.url = url
     mock_slurmrestd_client.get.return_value.text = error_message
 
     mock_response_status = mock.Mock()
@@ -308,15 +308,15 @@
         "jobs": [{"job_id": job_id}],
     }
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.json.return_value = mock_response_body
     mock_slurmrestd_client.get.return_value.status_code = 200
     mock_slurmrestd_client.get.return_value.url = (
-        SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/jobs"
+        SETTINGS.SLURM_RESTD_VERSIONED_URL + "/jobs"
     )
     mock_slurmrestd_client.get.return_value.text = "no error"
 
     mock_response_status = mock.Mock()
     mock_response_status.status_code = 200
 
     mock_asyncio.gather = asynctest.CoroutineMock()
@@ -332,15 +332,15 @@
             json=dict(
                 meta=dict(),
                 errors=list(),
                 job=dict(job_id=job_id),
             ),
         )
     ]
-    mock_slurmrestd_client.get.assert_awaited_with("/slurm/v0.0.36/jobs")
+    mock_slurmrestd_client.get.assert_awaited_with("/jobs")
     mock_asyncio.gather.assert_awaited_once()
     assert test_response == [200]
 
 
 @mock.patch("cluster_agent.agent.asyncio")
 @mock.patch("cluster_agent.agent.cluster_api_client")
 @mock.patch("cluster_agent.agent.slurmrestd_client")
@@ -350,15 +350,15 @@
     mock_slurmrestd_client, mock_cluster_api_client, mock_asyncio, response_status_code
 ):
     """
     Verify if an error is raised in case the slurmrestd request fails
     """
 
     error_message = "dummy error message"
-    url = SETTINGS.BASE_SLURMRESTD_URL + "/slurm/v0.0.36/jobs"
+    url = SETTINGS.SLURM_RESTD_VERSIONED_URL + "/jobs"
 
     mock_slurmrestd_client.get = asynctest.CoroutineMock()
     mock_slurmrestd_client.get.return_value.status_code = response_status_code
     mock_slurmrestd_client.get.return_value.url = url
     mock_slurmrestd_client.get.return_value.text = error_message
 
     mock_response_status = mock.Mock()
```

### Comparing `ovs-cluster-agent-2.2.2/tests/test_main.py` & `ovs-cluster-agent-2.2.3rc1/tests/test_main.py`

 * *Files identical despite different names*

