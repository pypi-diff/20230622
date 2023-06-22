# Comparing `tmp/python-upwork-oauth2-3.0.4.tar.gz` & `tmp/python-upwork-oauth2-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-upwork-oauth2-3.0.4.tar", last modified: Thu Dec 23 11:23:48 2021, max compression
+gzip compressed data, was "python-upwork-oauth2-3.1.0.tar", last modified: Thu Jun 22 08:45:41 2023, max compression
```

## Comparing `python-upwork-oauth2-3.0.4.tar` & `python-upwork-oauth2-3.1.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/
--rw-rw-r--   0 m         (1000) m         (1000)      170 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/CHANGELOG.md
--rw-rw-r--   0 m         (1000) m         (1000)      231 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/CONTRIBUTING.md
--rw-rw-r--   0 m         (1000) m         (1000)    10173 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/LICENSE
--rw-rw-r--   0 m         (1000) m         (1000)      179 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/MANIFEST.in
--rw-rw-r--   0 m         (1000) m         (1000)     3593 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/PKG-INFO
--rw-rw-r--   0 m         (1000) m         (1000)     2183 2021-10-11 12:20:12.000000 python-upwork-oauth2-3.0.4/README.md
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/
--rw-rw-r--   0 m         (1000) m         (1000)     3593 2021-12-23 11:23:48.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/PKG-INFO
--rw-rw-r--   0 m         (1000) m         (1000)     1839 2021-12-23 11:23:48.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/SOURCES.txt
--rw-rw-r--   0 m         (1000) m         (1000)        1 2021-12-23 11:23:48.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/dependency_links.txt
--rw-rw-r--   0 m         (1000) m         (1000)        1 2020-09-18 15:04:15.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/not-zip-safe
--rw-rw-r--   0 m         (1000) m         (1000)       25 2021-12-23 11:23:48.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/requires.txt
--rw-rw-r--   0 m         (1000) m         (1000)       13 2021-12-23 11:23:48.000000 python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/top_level.txt
--rw-rw-r--   0 m         (1000) m         (1000)       38 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/setup.cfg
--rw-rw-r--   0 m         (1000) m         (1000)     1216 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/setup.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/
--rw-rw-r--   0 m         (1000) m         (1000)      272 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/upwork/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     5590 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/upwork/client.py
--rw-rw-r--   0 m         (1000) m         (1000)     1048 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/config.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/
--rw-rw-r--   0 m         (1000) m         (1000)      397 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/__init__.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/activities/
--rw-rw-r--   0 m         (1000) m         (1000)       14 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/activities/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1137 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/activities/engagement.py
--rw-rw-r--   0 m         (1000) m         (1000)     3449 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/activities/team.py
--rw-rw-r--   0 m         (1000) m         (1000)      845 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/auth.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/freelancers/
--rw-rw-r--   0 m         (1000) m         (1000)       77 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/freelancers/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1108 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/freelancers/profile.py
--rw-rw-r--   0 m         (1000) m         (1000)      917 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/freelancers/search.py
--rw-rw-r--   0 m         (1000) m         (1000)      910 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/graphql.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/hr/
--rw-rw-r--   0 m         (1000) m         (1000)      300 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/__init__.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/
--rw-rw-r--   0 m         (1000) m         (1000)       14 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1220 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/applications.py
--rw-rw-r--   0 m         (1000) m         (1000)     1400 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/offers.py
--rw-rw-r--   0 m         (1000) m         (1000)     1498 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/contracts.py
--rw-rw-r--   0 m         (1000) m         (1000)     1115 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/engagements.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/
--rw-rw-r--   0 m         (1000) m         (1000)       87 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1167 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/applications.py
--rw-rw-r--   0 m         (1000) m         (1000)     1431 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/offers.py
--rw-rw-r--   0 m         (1000) m         (1000)      971 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/interviews.py
--rw-rw-r--   0 m         (1000) m         (1000)     1700 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/jobs.py
--rw-rw-r--   0 m         (1000) m         (1000)     2545 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/milestones.py
--rw-rw-r--   0 m         (1000) m         (1000)     1068 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/roles.py
--rw-rw-r--   0 m         (1000) m         (1000)     1567 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/hr/submissions.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/jobs/
--rw-rw-r--   0 m         (1000) m         (1000)       77 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/jobs/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)      897 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/jobs/profile.py
--rw-rw-r--   0 m         (1000) m         (1000)      912 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/jobs/search.py
--rw-rw-r--   0 m         (1000) m         (1000)     4627 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/messages.py
--rw-rw-r--   0 m         (1000) m         (1000)     1675 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/metadata.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/organization/
--rw-rw-r--   0 m         (1000) m         (1000)       95 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/organization/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1485 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/organization/companies.py
--rw-rw-r--   0 m         (1000) m         (1000)     1029 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/organization/teams.py
--rw-rw-r--   0 m         (1000) m         (1000)     1038 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/organization/users.py
--rw-rw-r--   0 m         (1000) m         (1000)      992 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/payments.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/reports/
--rw-rw-r--   0 m         (1000) m         (1000)       73 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/__init__.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2021-12-23 11:23:48.372139 python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/
--rw-rw-r--   0 m         (1000) m         (1000)      105 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/__init__.py
--rw-rw-r--   0 m         (1000) m         (1000)     1529 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/accounts.py
--rw-rw-r--   0 m         (1000) m         (1000)     2858 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/billings.py
--rw-rw-r--   0 m         (1000) m         (1000)     2858 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/earnings.py
--rw-rw-r--   0 m         (1000) m         (1000)     3109 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/reports/time.py
--rw-rw-r--   0 m         (1000) m         (1000)     1641 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/snapshots.py
--rw-rw-r--   0 m         (1000) m         (1000)     1645 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/workdays.py
--rw-rw-r--   0 m         (1000) m         (1000)     1429 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.0.4/upwork/routers/workdiary.py
--rw-rw-r--   0 m         (1000) m         (1000)      126 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.0.4/upwork/upwork.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.364972 python-upwork-oauth2-3.1.0/
+-rw-rw-r--   0 m         (1000) m         (1000)      223 2023-06-22 08:37:05.000000 python-upwork-oauth2-3.1.0/CHANGELOG.md
+-rw-rw-r--   0 m         (1000) m         (1000)      231 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/CONTRIBUTING.md
+-rw-rw-r--   0 m         (1000) m         (1000)    10173 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/LICENSE
+-rw-rw-r--   0 m         (1000) m         (1000)      179 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.1.0/MANIFEST.in
+-rw-rw-r--   0 m         (1000) m         (1000)     3016 2023-06-22 08:45:41.364972 python-upwork-oauth2-3.1.0/PKG-INFO
+-rw-rw-r--   0 m         (1000) m         (1000)     2183 2021-10-11 12:20:12.000000 python-upwork-oauth2-3.1.0/README.md
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/
+-rw-rw-r--   0 m         (1000) m         (1000)     3016 2023-06-22 08:45:41.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/PKG-INFO
+-rw-rw-r--   0 m         (1000) m         (1000)     1839 2023-06-22 08:45:41.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/SOURCES.txt
+-rw-rw-r--   0 m         (1000) m         (1000)        1 2023-06-22 08:45:41.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/dependency_links.txt
+-rw-rw-r--   0 m         (1000) m         (1000)        1 2020-09-18 15:04:15.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/not-zip-safe
+-rw-rw-r--   0 m         (1000) m         (1000)       25 2023-06-22 08:45:41.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/requires.txt
+-rw-rw-r--   0 m         (1000) m         (1000)       13 2023-06-22 08:45:41.000000 python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/top_level.txt
+-rw-rw-r--   0 m         (1000) m         (1000)       38 2023-06-22 08:45:41.364972 python-upwork-oauth2-3.1.0/setup.cfg
+-rw-rw-r--   0 m         (1000) m         (1000)     1216 2023-06-22 08:37:05.000000 python-upwork-oauth2-3.1.0/setup.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/
+-rw-rw-r--   0 m         (1000) m         (1000)      272 2023-06-22 08:37:05.000000 python-upwork-oauth2-3.1.0/upwork/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     5926 2023-06-22 08:37:05.000000 python-upwork-oauth2-3.1.0/upwork/client.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1235 2023-06-22 08:37:05.000000 python-upwork-oauth2-3.1.0/upwork/config.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/
+-rw-rw-r--   0 m         (1000) m         (1000)      397 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/__init__.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/activities/
+-rw-rw-r--   0 m         (1000) m         (1000)       14 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/activities/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1137 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/activities/engagement.py
+-rw-rw-r--   0 m         (1000) m         (1000)     3449 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/activities/team.py
+-rw-rw-r--   0 m         (1000) m         (1000)      845 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/auth.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/freelancers/
+-rw-rw-r--   0 m         (1000) m         (1000)       77 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/freelancers/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1108 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/freelancers/profile.py
+-rw-rw-r--   0 m         (1000) m         (1000)      917 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/freelancers/search.py
+-rw-rw-r--   0 m         (1000) m         (1000)      910 2021-12-23 11:22:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/graphql.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/hr/
+-rw-rw-r--   0 m         (1000) m         (1000)      300 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/__init__.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/
+-rw-rw-r--   0 m         (1000) m         (1000)       87 2023-02-07 16:42:39.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1220 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/applications.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1400 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/offers.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1498 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/contracts.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1115 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/engagements.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/
+-rw-rw-r--   0 m         (1000) m         (1000)       87 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1167 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/applications.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1431 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/offers.py
+-rw-rw-r--   0 m         (1000) m         (1000)      971 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/interviews.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1700 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/jobs.py
+-rw-rw-r--   0 m         (1000) m         (1000)     2545 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/milestones.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1068 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/roles.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1567 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/hr/submissions.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/jobs/
+-rw-rw-r--   0 m         (1000) m         (1000)       77 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/jobs/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)      897 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/jobs/profile.py
+-rw-rw-r--   0 m         (1000) m         (1000)      912 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/jobs/search.py
+-rw-rw-r--   0 m         (1000) m         (1000)     4627 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/messages.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1675 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/metadata.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/organization/
+-rw-rw-r--   0 m         (1000) m         (1000)       95 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/organization/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1485 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/organization/companies.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1029 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/organization/teams.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1038 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/organization/users.py
+-rw-rw-r--   0 m         (1000) m         (1000)      992 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/payments.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/reports/
+-rw-rw-r--   0 m         (1000) m         (1000)       73 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/__init__.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-06-22 08:45:41.360972 python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/
+-rw-rw-r--   0 m         (1000) m         (1000)      105 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/__init__.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1529 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/accounts.py
+-rw-rw-r--   0 m         (1000) m         (1000)     2858 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/billings.py
+-rw-rw-r--   0 m         (1000) m         (1000)     2858 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/earnings.py
+-rw-rw-r--   0 m         (1000) m         (1000)     3109 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/reports/time.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1641 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/snapshots.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1645 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/workdays.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1429 2020-09-18 15:03:59.000000 python-upwork-oauth2-3.1.0/upwork/routers/workdiary.py
+-rw-rw-r--   0 m         (1000) m         (1000)      126 2023-06-20 18:14:08.000000 python-upwork-oauth2-3.1.0/upwork/upwork.py
```

### Comparing `python-upwork-oauth2-3.0.4/LICENSE` & `python-upwork-oauth2-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/PKG-INFO` & `python-upwork-oauth2-3.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: python-upwork-oauth2
-Version: 3.0.4
+Version: 3.1.0
 Summary: Python bindings for Upwork API (OAuth2)
 Home-page: https://github.com/upwork/python-upwork-oauth2
 Author: Maksym Novozhylov
 Author-email: mnovozhilov@upwork.com
 License: Apache Software License 2.0
-Description: Python bindings for Upwork API (OAuth2)
-        ============
-        
-        [![License](https://img.shields.io/github/license/upwork/python-upwork-oauth2)](http://www.apache.org/licenses/LICENSE-2.0.html)
-        [![PyPI Version](https://badge.fury.io/py/python-upwork.svg)](http://badge.fury.io/py/python-upwork)
-        [![GitHub release](https://img.shields.io/github/release/upwork/python-upwork.svg)](https://github.com/upwork/python-upwork/releases)
-        [![Build Status](https://github.com/upwork/python-upwork-oauth2/workflows/build/badge.svg)](https://github.com/upwork/python-upwork-oauth2/actions)
-        
-        # Upwork API
-        
-        This project provides a set of resources of Upwork API from http://developers.upwork.com
-         based on OAuth 2.0.
-        
-        # Features
-        These are the supported API resources:
-        
-        * My Info
-        * Custom Payments
-        * Hiring
-        * Job and Freelancer Profile
-        * Search Jobs and Freelancers
-        * Organization
-        * Messages
-        * Time and Financial Reporting
-        * Metadata
-        * Snapshot
-        * Team
-        * Workd Diary
-        * Activities
-        
-        # License
-        
-        Copyright 2020 Upwork Corporation. All Rights Reserved.
-        
-        python-upwork is licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        ## SLA
-        The usage of this API is ruled by the Terms of Use at:
-        
-            https://developers.upwork.com/api-tos.html
-        
-        # Requirements
-        To integrate this library you need to have:
-        
-        * Python 3.8+
-        * requests_oauthlib >= 1.3.0
-        
-        ## Installation
-        
-            pip3 install python-upwork-oauth2
-        
-        All the dependencies will be automatically installed as well.
-        
-        ## Usage
-        
-        1.
-        Follow instructions from the `Installation` section.
-        
-        2.
-        Run `myapp.py` and follow the instructions, or open `myapp.py` and type the `client_id` and `client_secret` that you previously got from the API Center.
-        ***That's all. Run your app as `python myapp.py` and have fun.***'
-        
 Keywords: python-upwork-oauth2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python bindings for Upwork API (OAuth2)
+============
+
+[![License](https://img.shields.io/github/license/upwork/python-upwork-oauth2)](http://www.apache.org/licenses/LICENSE-2.0.html)
+[![PyPI Version](https://badge.fury.io/py/python-upwork.svg)](http://badge.fury.io/py/python-upwork)
+[![GitHub release](https://img.shields.io/github/release/upwork/python-upwork.svg)](https://github.com/upwork/python-upwork/releases)
+[![Build Status](https://github.com/upwork/python-upwork-oauth2/workflows/build/badge.svg)](https://github.com/upwork/python-upwork-oauth2/actions)
+
+# Upwork API
+
+This project provides a set of resources of Upwork API from http://developers.upwork.com
+ based on OAuth 2.0.
+
+# Features
+These are the supported API resources:
+
+* My Info
+* Custom Payments
+* Hiring
+* Job and Freelancer Profile
+* Search Jobs and Freelancers
+* Organization
+* Messages
+* Time and Financial Reporting
+* Metadata
+* Snapshot
+* Team
+* Workd Diary
+* Activities
+
+# License
+
+Copyright 2020 Upwork Corporation. All Rights Reserved.
+
+python-upwork is licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+## SLA
+The usage of this API is ruled by the Terms of Use at:
+
+    https://developers.upwork.com/api-tos.html
+
+# Requirements
+To integrate this library you need to have:
+
+* Python 3.8+
+* requests_oauthlib >= 1.3.0
+
+## Installation
+
+    pip3 install python-upwork-oauth2
+
+All the dependencies will be automatically installed as well.
+
+## Usage
+
+1.
+Follow instructions from the `Installation` section.
+
+2.
+Run `myapp.py` and follow the instructions, or open `myapp.py` and type the `client_id` and `client_secret` that you previously got from the API Center.
+***That's all. Run your app as `python myapp.py` and have fun.***'
```

### Comparing `python-upwork-oauth2-3.0.4/README.md` & `python-upwork-oauth2-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/PKG-INFO` & `python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: python-upwork-oauth2
-Version: 3.0.4
+Version: 3.1.0
 Summary: Python bindings for Upwork API (OAuth2)
 Home-page: https://github.com/upwork/python-upwork-oauth2
 Author: Maksym Novozhylov
 Author-email: mnovozhilov@upwork.com
 License: Apache Software License 2.0
-Description: Python bindings for Upwork API (OAuth2)
-        ============
-        
-        [![License](https://img.shields.io/github/license/upwork/python-upwork-oauth2)](http://www.apache.org/licenses/LICENSE-2.0.html)
-        [![PyPI Version](https://badge.fury.io/py/python-upwork.svg)](http://badge.fury.io/py/python-upwork)
-        [![GitHub release](https://img.shields.io/github/release/upwork/python-upwork.svg)](https://github.com/upwork/python-upwork/releases)
-        [![Build Status](https://github.com/upwork/python-upwork-oauth2/workflows/build/badge.svg)](https://github.com/upwork/python-upwork-oauth2/actions)
-        
-        # Upwork API
-        
-        This project provides a set of resources of Upwork API from http://developers.upwork.com
-         based on OAuth 2.0.
-        
-        # Features
-        These are the supported API resources:
-        
-        * My Info
-        * Custom Payments
-        * Hiring
-        * Job and Freelancer Profile
-        * Search Jobs and Freelancers
-        * Organization
-        * Messages
-        * Time and Financial Reporting
-        * Metadata
-        * Snapshot
-        * Team
-        * Workd Diary
-        * Activities
-        
-        # License
-        
-        Copyright 2020 Upwork Corporation. All Rights Reserved.
-        
-        python-upwork is licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        ## SLA
-        The usage of this API is ruled by the Terms of Use at:
-        
-            https://developers.upwork.com/api-tos.html
-        
-        # Requirements
-        To integrate this library you need to have:
-        
-        * Python 3.8+
-        * requests_oauthlib >= 1.3.0
-        
-        ## Installation
-        
-            pip3 install python-upwork-oauth2
-        
-        All the dependencies will be automatically installed as well.
-        
-        ## Usage
-        
-        1.
-        Follow instructions from the `Installation` section.
-        
-        2.
-        Run `myapp.py` and follow the instructions, or open `myapp.py` and type the `client_id` and `client_secret` that you previously got from the API Center.
-        ***That's all. Run your app as `python myapp.py` and have fun.***'
-        
 Keywords: python-upwork-oauth2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python bindings for Upwork API (OAuth2)
+============
+
+[![License](https://img.shields.io/github/license/upwork/python-upwork-oauth2)](http://www.apache.org/licenses/LICENSE-2.0.html)
+[![PyPI Version](https://badge.fury.io/py/python-upwork.svg)](http://badge.fury.io/py/python-upwork)
+[![GitHub release](https://img.shields.io/github/release/upwork/python-upwork.svg)](https://github.com/upwork/python-upwork/releases)
+[![Build Status](https://github.com/upwork/python-upwork-oauth2/workflows/build/badge.svg)](https://github.com/upwork/python-upwork-oauth2/actions)
+
+# Upwork API
+
+This project provides a set of resources of Upwork API from http://developers.upwork.com
+ based on OAuth 2.0.
+
+# Features
+These are the supported API resources:
+
+* My Info
+* Custom Payments
+* Hiring
+* Job and Freelancer Profile
+* Search Jobs and Freelancers
+* Organization
+* Messages
+* Time and Financial Reporting
+* Metadata
+* Snapshot
+* Team
+* Workd Diary
+* Activities
+
+# License
+
+Copyright 2020 Upwork Corporation. All Rights Reserved.
+
+python-upwork is licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+## SLA
+The usage of this API is ruled by the Terms of Use at:
+
+    https://developers.upwork.com/api-tos.html
+
+# Requirements
+To integrate this library you need to have:
+
+* Python 3.8+
+* requests_oauthlib >= 1.3.0
+
+## Installation
+
+    pip3 install python-upwork-oauth2
+
+All the dependencies will be automatically installed as well.
+
+## Usage
+
+1.
+Follow instructions from the `Installation` section.
+
+2.
+Run `myapp.py` and follow the instructions, or open `myapp.py` and type the `client_id` and `client_secret` that you previously got from the API Center.
+***That's all. Run your app as `python myapp.py` and have fun.***'
```

### Comparing `python-upwork-oauth2-3.0.4/python_upwork_oauth2.egg-info/SOURCES.txt` & `python-upwork-oauth2-3.1.0/python_upwork_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/setup.py` & `python-upwork-oauth2-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="python-upwork-oauth2",
     name="python-upwork-oauth2",
     packages=find_packages(),
     setup_requires=[],
     url="https://github.com/upwork/python-upwork-oauth2",
-    version="3.0.4",
+    version="3.1.0",
     zip_safe=False,
 )
```

### Comparing `python-upwork-oauth2-3.0.4/upwork/client.py` & `python-upwork-oauth2-3.1.0/upwork/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # limitations under the License.
 #
 # Author::    Maksym Novozhylov (mnovozhilov@upwork.com)
 # Copyright:: Copyright 2020(c) Upwork.com
 # License::   See LICENSE.txt and TOS - https://developers.upwork.com/api-tos.html
 
 from . import upwork
+from oauthlib.oauth2 import BackendApplicationClient
 from requests_oauthlib import OAuth2Session  # type: ignore
 from urllib.parse import parse_qsl, urlencode
 
 
 class Client(object):
     """API client for OAuth2 authorization
     
@@ -44,30 +45,36 @@
                 auto_refresh_kwargs={
                     "client_id": self.config.client_id,
                     "client_secret": self.config.client_secret,
                 },
                 token_updater=self.refresh_config_from_access_token,
             )
         except AttributeError as e:
-            # start from authorization step
-            self.__oauth = OAuth2Session(
-                self.config.client_id, redirect_uri=self.config.redirect_uri
-            )
+            if self.config.grant_type == "client_credentials":
+                client = BackendApplicationClient(client_id=self.config.client_id)
+                self.__oauth = OAuth2Session(
+                    client=client
+                )
+            else:
+                # start from authorization step
+                self.__oauth = OAuth2Session(
+                    self.config.client_id, redirect_uri=self.config.redirect_uri
+                )
 
     def get_authorization_url(self):
         """Get authorization URL
 
         :param redirect_uri:  (Default value = None)
 
         """
         return self.__oauth.authorization_url(
             "{0}{1}".format(upwork.BASE_HOST, self.__uri_auth)
         )
 
-    def get_access_token(self, authorization_response):
+    def get_access_token(self, authorization_response=None):
         """Finish auth process and get access token
 
         :param authorization_response: 
 
         """
         self.config.token = self.__oauth.fetch_token(
             full_url(self.__uri_atoken, upwork.DEFAULT_EPOINT),
```

### Comparing `python-upwork-oauth2-3.0.4/upwork/config.py` & `python-upwork-oauth2-3.1.0/upwork/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,13 +17,18 @@
 
     def __init__(self, config):
         self.client_id, self.client_secret = (
             config["client_id"],
             config["client_secret"],
         )
 
+        if "grant_type" in config:
+            self.grant_type = config["grant_type"]
+        else:
+            self.grant_type = None # Authorization Code Grant flow is used by default
+
         if "redirect_uri" in config:
             self.redirect_uri = config["redirect_uri"]
 
         # access-, refresh token, and expires_in/at data
         if "token" in config:
             self.token = config["token"]
```

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/activities/engagement.py` & `python-upwork-oauth2-3.1.0/upwork/routers/activities/engagement.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/activities/team.py` & `python-upwork-oauth2-3.1.0/upwork/routers/activities/team.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/auth.py` & `python-upwork-oauth2-3.1.0/upwork/routers/auth.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/freelancers/profile.py` & `python-upwork-oauth2-3.1.0/upwork/routers/freelancers/profile.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/freelancers/search.py` & `python-upwork-oauth2-3.1.0/upwork/routers/freelancers/search.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/graphql.py` & `python-upwork-oauth2-3.1.0/upwork/routers/graphql.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/applications.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/applications.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/clients/offers.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/clients/offers.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/contracts.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/contracts.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/engagements.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/engagements.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/applications.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/applications.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/freelancers/offers.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/freelancers/offers.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/interviews.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/interviews.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/jobs.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/jobs.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/milestones.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/milestones.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/roles.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/roles.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/hr/submissions.py` & `python-upwork-oauth2-3.1.0/upwork/routers/hr/submissions.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/jobs/profile.py` & `python-upwork-oauth2-3.1.0/upwork/routers/jobs/profile.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/jobs/search.py` & `python-upwork-oauth2-3.1.0/upwork/routers/jobs/search.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/messages.py` & `python-upwork-oauth2-3.1.0/upwork/routers/messages.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/metadata.py` & `python-upwork-oauth2-3.1.0/upwork/routers/metadata.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/organization/companies.py` & `python-upwork-oauth2-3.1.0/upwork/routers/organization/companies.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/organization/teams.py` & `python-upwork-oauth2-3.1.0/upwork/routers/organization/teams.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/organization/users.py` & `python-upwork-oauth2-3.1.0/upwork/routers/organization/users.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/payments.py` & `python-upwork-oauth2-3.1.0/upwork/routers/payments.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/accounts.py` & `python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/accounts.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/billings.py` & `python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/billings.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/reports/finance/earnings.py` & `python-upwork-oauth2-3.1.0/upwork/routers/reports/finance/earnings.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/reports/time.py` & `python-upwork-oauth2-3.1.0/upwork/routers/reports/time.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/snapshots.py` & `python-upwork-oauth2-3.1.0/upwork/routers/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/workdays.py` & `python-upwork-oauth2-3.1.0/upwork/routers/workdays.py`

 * *Files identical despite different names*

### Comparing `python-upwork-oauth2-3.0.4/upwork/routers/workdiary.py` & `python-upwork-oauth2-3.1.0/upwork/routers/workdiary.py`

 * *Files identical despite different names*

