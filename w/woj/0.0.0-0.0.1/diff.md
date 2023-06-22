# Comparing `tmp/woj-0.0.0.tar.gz` & `tmp/woj-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woj-0.0.0.tar", last modified: Wed Jun 21 14:12:47 2023, max compression
+gzip compressed data, was "woj-0.0.1.tar", last modified: Thu Jun 22 20:53:36 2023, max compression
```

## Comparing `woj-0.0.0.tar` & `woj-0.0.1.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.260175 woj-0.0.0/
--rw-r--r--   0 jacoblincool   (501) staff       (20)      376 2023-06-21 14:12:47.260257 woj-0.0.0/PKG-INFO
--rw-r--r--   0 jacoblincool   (501) staff       (20)     4764 2023-06-21 14:12:45.000000 woj-0.0.0/README.md
--rw-r--r--   0 jacoblincool   (501) staff       (20)      720 2023-06-21 14:12:45.000000 woj-0.0.0/pyproject.toml
--rw-r--r--   0 jacoblincool   (501) staff       (20)       69 2023-06-21 14:12:47.260492 woj-0.0.0/setup.cfg
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1252 2023-06-21 14:12:45.000000 woj-0.0.0/setup.py
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.254399 woj-0.0.0/test/
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1606 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_auth_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1814 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_auth_send_post200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1617 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_auth_send_post400_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1618 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_auth_send_post_request.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1608 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_me_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2425 2023-06-21 14:12:44.000000 woj-0.0.0/test/test_api_problem_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2102 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_problem_get200_response_problems_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     4051 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_problem_id_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     3529 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_problem_id_get200_response_problem.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1971 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_problem_id_get200_response_problem_policy_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2060 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_problem_id_get200_response_problem_testcase_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2599 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2278 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_get200_response_submissions_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     5264 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_id_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2500 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_id_get200_response_submission.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1651 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_post200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1709 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_submission_post_request.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2258 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_sys_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1658 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_sys_get200_response_cfg.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1733 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_api_sys_get200_response_stat.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1608 2023-06-21 14:12:45.000000 woj-0.0.0/test/test_default_api.py
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.255709 woj-0.0.0/woj/
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2567 2023-06-21 14:12:45.000000 woj-0.0.0/woj/__init__.py
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.257080 woj-0.0.0/woj/api/
--rw-r--r--   0 jacoblincool   (501) staff       (20)       91 2023-06-21 14:12:45.000000 woj-0.0.0/woj/api/__init__.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)    55722 2023-06-21 14:12:45.000000 woj-0.0.0/woj/api/default_api.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)    29946 2023-06-21 14:12:45.000000 woj-0.0.0/woj/api_client.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)      844 2023-06-21 14:12:45.000000 woj-0.0.0/woj/api_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)    15228 2023-06-21 14:12:45.000000 woj-0.0.0/woj/configuration.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     5311 2023-06-21 14:12:45.000000 woj-0.0.0/woj/exceptions.py
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.260050 woj-0.0.0/woj/models/
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2079 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/__init__.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2047 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_auth_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2149 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_auth_send_post200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     1949 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_auth_send_post400_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2168 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_auth_send_post_request.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2378 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_me_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2555 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_problem_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2455 2023-06-21 14:12:44.000000 woj-0.0.0/woj/models/api_problem_get200_response_problems_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2312 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_problem_id_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     3858 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_problem_id_get200_response_problem.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2354 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_problem_id_get200_response_problem_policy_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2784 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_problem_id_get200_response_problem_testcase_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2598 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     3775 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_get200_response_submissions_inner.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2851 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_id_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     4372 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_id_get200_response_submission.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2018 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_post200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2538 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_submission_post_request.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2587 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_sys_get200_response.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2190 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_sys_get200_response_cfg.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2312 2023-06-21 14:12:45.000000 woj-0.0.0/woj/models/api_sys_get200_response_stat.py
--rw-r--r--   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:45.000000 woj-0.0.0/woj/py.typed
--rw-r--r--   0 jacoblincool   (501) staff       (20)    12870 2023-06-21 14:12:45.000000 woj-0.0.0/woj/rest.py
-drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-21 14:12:47.256647 woj-0.0.0/woj.egg-info/
--rw-r--r--   0 jacoblincool   (501) staff       (20)      376 2023-06-21 14:12:46.000000 woj-0.0.0/woj.egg-info/PKG-INFO
--rw-r--r--   0 jacoblincool   (501) staff       (20)     2294 2023-06-21 14:12:47.000000 woj-0.0.0/woj.egg-info/SOURCES.txt
--rw-r--r--   0 jacoblincool   (501) staff       (20)        1 2023-06-21 14:12:47.000000 woj-0.0.0/woj.egg-info/dependency_links.txt
--rw-r--r--   0 jacoblincool   (501) staff       (20)       65 2023-06-21 14:12:47.000000 woj-0.0.0/woj.egg-info/requires.txt
--rw-r--r--   0 jacoblincool   (501) staff       (20)        4 2023-06-21 14:12:47.000000 woj-0.0.0/woj.egg-info/top_level.txt
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.899950 woj-0.0.1/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      352 2023-06-22 20:53:36.900037 woj-0.0.1/PKG-INFO
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     4776 2023-06-22 20:53:34.000000 woj-0.0.1/README.md
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      696 2023-06-22 20:53:34.000000 woj-0.0.1/pyproject.toml
+-rw-r--r--   0 jacoblincool   (501) staff       (20)       69 2023-06-22 20:53:36.900282 woj-0.0.1/setup.cfg
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1257 2023-06-22 20:53:34.000000 woj-0.0.1/setup.py
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.894283 woj-0.0.1/test/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1635 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_auth_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1843 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_auth_send_post200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1646 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_auth_send_post400_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1647 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_auth_send_post_request.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1637 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_me_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2454 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2131 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_get200_response_problems_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     4080 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_id_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     3558 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_id_get200_response_problem.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2000 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_id_get200_response_problem_policy_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2089 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_problem_id_get200_response_problem_testcase_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2628 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2307 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_get200_response_submissions_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     5293 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_id_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2529 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_id_get200_response_submission.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1680 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_post200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1738 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_submission_post_request.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2287 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_sys_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1687 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_sys_get200_response_cfg.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1762 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_api_sys_get200_response_stat.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      877 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_auth_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      877 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_default_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      901 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_problem_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1043 2023-06-22 20:53:34.000000 woj-0.0.1/test/test_submission_api.py
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.895205 woj-0.0.1/woj/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2725 2023-06-22 20:53:34.000000 woj-0.0.1/woj/__init__.py
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.896765 woj-0.0.1/woj/api/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      220 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api/__init__.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    13479 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api/auth_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    11931 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api/default_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    12379 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api/problem_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    20950 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api/submission_api.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    29975 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api_client.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      844 2023-06-22 20:53:34.000000 woj-0.0.1/woj/api_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    15257 2023-06-22 20:53:34.000000 woj-0.0.1/woj/configuration.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     5340 2023-06-22 20:53:34.000000 woj-0.0.1/woj/exceptions.py
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.899809 woj-0.0.1/woj/models/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2108 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/__init__.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2076 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_auth_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2178 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_auth_send_post200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     1978 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_auth_send_post400_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2197 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_auth_send_post_request.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2407 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_me_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2584 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2484 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_get200_response_problems_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2341 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_id_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     3887 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_id_get200_response_problem.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2383 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_id_get200_response_problem_policy_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2813 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_problem_id_get200_response_problem_testcase_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2627 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     3804 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_get200_response_submissions_inner.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2880 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_id_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     4401 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_id_get200_response_submission.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2047 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_post200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2567 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_submission_post_request.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2616 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_sys_get200_response.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2219 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_sys_get200_response_cfg.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2341 2023-06-22 20:53:34.000000 woj-0.0.1/woj/models/api_sys_get200_response_stat.py
+-rw-r--r--   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:34.000000 woj-0.0.1/woj/py.typed
+-rw-r--r--   0 jacoblincool   (501) staff       (20)    12899 2023-06-22 20:53:34.000000 woj-0.0.1/woj/rest.py
+drwxr-xr-x   0 jacoblincool   (501) staff       (20)        0 2023-06-22 20:53:36.895976 woj-0.0.1/woj.egg-info/
+-rw-r--r--   0 jacoblincool   (501) staff       (20)      352 2023-06-22 20:53:36.000000 woj-0.0.1/woj.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblincool   (501) staff       (20)     2438 2023-06-22 20:53:36.000000 woj-0.0.1/woj.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblincool   (501) staff       (20)        1 2023-06-22 20:53:36.000000 woj-0.0.1/woj.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblincool   (501) staff       (20)       65 2023-06-22 20:53:36.000000 woj-0.0.1/woj.egg-info/requires.txt
+-rw-r--r--   0 jacoblincool   (501) staff       (20)        4 2023-06-22 20:53:36.000000 woj-0.0.1/woj.egg-info/top_level.txt
```

### Comparing `woj-0.0.0/README.md` & `woj-0.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # woj
 You can interact with WASM OJ Wonderland through this API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.0.0
-- Package version: 0.0.0
+- Package version: 0.0.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -62,40 +62,40 @@
 )
 
 
 
 # Enter a context with an instance of the API client
 with woj.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = woj.DefaultApi(api_client)
+    api_instance = woj.AuthApi(api_client)
     token = 'token_example' # str | 
 
     try:
         api_response = api_instance.api_auth_get(token)
-        print("The response of DefaultApi->api_auth_get:\n")
+        print("The response of AuthApi->api_auth_get:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling DefaultApi->api_auth_get: %s\n" % e)
+        print("Exception when calling AuthApi->api_auth_get: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://woj.csie.cool*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*DefaultApi* | [**api_auth_get**](docs/DefaultApi.md#api_auth_get) | **GET** /api/auth | 
-*DefaultApi* | [**api_auth_send_post**](docs/DefaultApi.md#api_auth_send_post) | **POST** /api/auth/send | 
+*AuthApi* | [**api_auth_get**](docs/AuthApi.md#api_auth_get) | **GET** /api/auth | 
+*AuthApi* | [**api_auth_send_post**](docs/AuthApi.md#api_auth_send_post) | **POST** /api/auth/send | 
+*ProblemApi* | [**api_problem_get**](docs/ProblemApi.md#api_problem_get) | **GET** /api/problem | 
+*ProblemApi* | [**api_problem_id_get**](docs/ProblemApi.md#api_problem_id_get) | **GET** /api/problem/{id} | 
+*SubmissionApi* | [**api_submission_get**](docs/SubmissionApi.md#api_submission_get) | **GET** /api/submission | 
+*SubmissionApi* | [**api_submission_id_get**](docs/SubmissionApi.md#api_submission_id_get) | **GET** /api/submission/{id} | 
+*SubmissionApi* | [**api_submission_post**](docs/SubmissionApi.md#api_submission_post) | **POST** /api/submission | 
 *DefaultApi* | [**api_me_get**](docs/DefaultApi.md#api_me_get) | **GET** /api/me | 
-*DefaultApi* | [**api_problem_get**](docs/DefaultApi.md#api_problem_get) | **GET** /api/problem | 
-*DefaultApi* | [**api_problem_id_get**](docs/DefaultApi.md#api_problem_id_get) | **GET** /api/problem/{id} | 
-*DefaultApi* | [**api_submission_get**](docs/DefaultApi.md#api_submission_get) | **GET** /api/submission | 
-*DefaultApi* | [**api_submission_id_get**](docs/DefaultApi.md#api_submission_id_get) | **GET** /api/submission/{id} | 
-*DefaultApi* | [**api_submission_post**](docs/DefaultApi.md#api_submission_post) | **POST** /api/submission | 
 *DefaultApi* | [**api_sys_get**](docs/DefaultApi.md#api_sys_get) | **GET** /api/sys | 
 
 
 ## Documentation For Models
 
  - [ApiAuthGet200Response](docs/ApiAuthGet200Response.md)
  - [ApiAuthSendPost200Response](docs/ApiAuthSendPost200Response.md)
@@ -128,10 +128,10 @@
 ### bearerAuth
 
 - **Type**: Bearer authentication (JWT)
 
 
 ## Author
 
-
+jacob@csie.cool
```

### Comparing `woj-0.0.0/setup.py` & `woj-0.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
@@ -17,29 +18,29 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "woj"
-VERSION = "0.0.0"
+VERSION = "0.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="WASM OJ Wonderland API",
-    author="OpenAPI Generator community",
-    author_email="team@openapitools.org",
+    author="Jacob Lin",
+    author_email="jacob@csie.cool",
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "WASM OJ Wonderland API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT",
     long_description_content_type='text/markdown',
```

### Comparing `woj-0.0.0/test/test_api_auth_get200_response.py` & `woj-0.0.1/test/test_api_auth_get200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_auth_send_post200_response.py` & `woj-0.0.1/test/test_api_auth_send_post200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_auth_send_post400_response.py` & `woj-0.0.1/test/test_api_auth_send_post400_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_auth_send_post_request.py` & `woj-0.0.1/test/test_api_auth_send_post_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_me_get200_response.py` & `woj-0.0.1/test/test_api_me_get200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_get200_response.py` & `woj-0.0.1/test/test_api_problem_get200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_get200_response_problems_inner.py` & `woj-0.0.1/test/test_api_problem_get200_response_problems_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_id_get200_response.py` & `woj-0.0.1/test/test_api_problem_id_get200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_id_get200_response_problem.py` & `woj-0.0.1/test/test_api_problem_id_get200_response_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_id_get200_response_problem_policy_inner.py` & `woj-0.0.1/test/test_api_problem_id_get200_response_problem_policy_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_problem_id_get200_response_problem_testcase_inner.py` & `woj-0.0.1/test/test_api_problem_id_get200_response_problem_testcase_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_get200_response.py` & `woj-0.0.1/test/test_api_submission_get200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_get200_response_submissions_inner.py` & `woj-0.0.1/test/test_api_submission_get200_response_submissions_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_id_get200_response.py` & `woj-0.0.1/test/test_api_submission_id_get200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_id_get200_response_submission.py` & `woj-0.0.1/test/test_api_submission_id_get200_response_submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_post200_response.py` & `woj-0.0.1/test/test_api_submission_post200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_submission_post_request.py` & `woj-0.0.1/test/test_api_submission_post_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_sys_get200_response.py` & `woj-0.0.1/test/test_api_sys_get200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_sys_get200_response_cfg.py` & `woj-0.0.1/test/test_api_sys_get200_response_cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_api_sys_get200_response_stat.py` & `woj-0.0.1/test/test_api_sys_get200_response_stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
```

### Comparing `woj-0.0.0/test/test_default_api.py` & `woj-0.0.1/test/test_submission_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,66 +2,37 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 
 import woj
-from woj.api.default_api import DefaultApi  # noqa: E501
+from woj.api.submission_api import SubmissionApi  # noqa: E501
 from woj.rest import ApiException
 
 
-class TestDefaultApi(unittest.TestCase):
-    """DefaultApi unit test stubs"""
+class TestSubmissionApi(unittest.TestCase):
+    """SubmissionApi unit test stubs"""
 
     def setUp(self):
-        self.api = woj.api.default_api.DefaultApi()  # noqa: E501
+        self.api = woj.api.submission_api.SubmissionApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_api_auth_get(self):
-        """Test case for api_auth_get
-
-        """
-        pass
-
-    def test_api_auth_send_post(self):
-        """Test case for api_auth_send_post
-
-        """
-        pass
-
-    def test_api_me_get(self):
-        """Test case for api_me_get
-
-        """
-        pass
-
-    def test_api_problem_get(self):
-        """Test case for api_problem_get
-
-        """
-        pass
-
-    def test_api_problem_id_get(self):
-        """Test case for api_problem_id_get
-
-        """
-        pass
-
     def test_api_submission_get(self):
         """Test case for api_submission_get
 
         """
         pass
 
     def test_api_submission_id_get(self):
@@ -72,16 +43,10 @@
 
     def test_api_submission_post(self):
         """Test case for api_submission_post
 
         """
         pass
 
-    def test_api_sys_get(self):
-        """Test case for api_sys_get
-
-        """
-        pass
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `woj-0.0.0/woj/__init__.py` & `woj-0.0.1/woj/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 
 # import apis into sdk package
+from woj.api.auth_api import AuthApi
+from woj.api.problem_api import ProblemApi
+from woj.api.submission_api import SubmissionApi
 from woj.api.default_api import DefaultApi
 
 # import ApiClient
 from woj.api_response import ApiResponse
 from woj.api_client import ApiClient
 from woj.configuration import Configuration
 from woj.exceptions import OpenApiException
```

### Comparing `woj-0.0.0/woj/api_client.py` & `woj-0.0.1/woj/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import atexit
@@ -72,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `woj-0.0.0/woj/api_response.py` & `woj-0.0.1/woj/api_response.py`

 * *Files identical despite different names*

### Comparing `woj-0.0.0/woj/configuration.py` & `woj-0.0.1/woj/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import copy
@@ -373,15 +374,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.0\n"\
-               "SDK Package Version: 0.0.0".\
+               "SDK Package Version: 0.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `woj-0.0.0/woj/exceptions.py` & `woj-0.0.1/woj/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 class OpenApiException(Exception):
```

### Comparing `woj-0.0.0/woj/models/__init__.py` & `woj-0.0.1/woj/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # flake8: noqa
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
```

### Comparing `woj-0.0.0/woj/models/api_auth_get200_response.py` & `woj-0.0.1/woj/models/api_auth_get200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_auth_send_post200_response.py` & `woj-0.0.1/woj/models/api_auth_send_post200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_auth_send_post400_response.py` & `woj-0.0.1/woj/models/api_auth_send_post400_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_auth_send_post_request.py` & `woj-0.0.1/woj/models/api_auth_send_post_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_me_get200_response.py` & `woj-0.0.1/woj/models/api_me_get200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_get200_response.py` & `woj-0.0.1/woj/models/api_problem_get200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_get200_response_problems_inner.py` & `woj-0.0.1/woj/models/api_problem_get200_response_problems_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_id_get200_response.py` & `woj-0.0.1/woj/models/api_problem_id_get200_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_id_get200_response_problem.py` & `woj-0.0.1/woj/models/api_problem_id_get200_response_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_id_get200_response_problem_policy_inner.py` & `woj-0.0.1/woj/models/api_problem_id_get200_response_problem_policy_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_problem_id_get200_response_problem_testcase_inner.py` & `woj-0.0.1/woj/models/api_problem_id_get200_response_problem_testcase_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_get200_response.py` & `woj-0.0.1/woj/models/api_submission_get200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_get200_response_submissions_inner.py` & `woj-0.0.1/woj/models/api_submission_get200_response_submissions_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_id_get200_response.py` & `woj-0.0.1/woj/models/api_submission_id_get200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_id_get200_response_submission.py` & `woj-0.0.1/woj/models/api_submission_id_get200_response_submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_post200_response.py` & `woj-0.0.1/woj/models/api_submission_post200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_submission_post_request.py` & `woj-0.0.1/woj/models/api_submission_post_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_sys_get200_response.py` & `woj-0.0.1/woj/models/api_sys_get200_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_sys_get200_response_cfg.py` & `woj-0.0.1/woj/models/api_sys_get200_response_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/models/api_sys_get200_response_stat.py` & `woj-0.0.1/woj/models/api_sys_get200_response_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
```

### Comparing `woj-0.0.0/woj/rest.py` & `woj-0.0.1/woj/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
     WASM OJ Wonderland API
 
     You can interact with WASM OJ Wonderland through this API  # noqa: E501
 
     The version of the OpenAPI document: 0.0.0
+    Contact: jacob@csie.cool
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import io
```

### Comparing `woj-0.0.0/woj.egg-info/SOURCES.txt` & `woj-0.0.1/woj.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,35 @@
 test/test_api_submission_id_get200_response.py
 test/test_api_submission_id_get200_response_submission.py
 test/test_api_submission_post200_response.py
 test/test_api_submission_post_request.py
 test/test_api_sys_get200_response.py
 test/test_api_sys_get200_response_cfg.py
 test/test_api_sys_get200_response_stat.py
+test/test_auth_api.py
 test/test_default_api.py
+test/test_problem_api.py
+test/test_submission_api.py
 woj/__init__.py
 woj/api_client.py
 woj/api_response.py
 woj/configuration.py
 woj/exceptions.py
 woj/py.typed
 woj/rest.py
 woj.egg-info/PKG-INFO
 woj.egg-info/SOURCES.txt
 woj.egg-info/dependency_links.txt
 woj.egg-info/requires.txt
 woj.egg-info/top_level.txt
 woj/api/__init__.py
+woj/api/auth_api.py
 woj/api/default_api.py
+woj/api/problem_api.py
+woj/api/submission_api.py
 woj/models/__init__.py
 woj/models/api_auth_get200_response.py
 woj/models/api_auth_send_post200_response.py
 woj/models/api_auth_send_post400_response.py
 woj/models/api_auth_send_post_request.py
 woj/models/api_me_get200_response.py
 woj/models/api_problem_get200_response.py
```

