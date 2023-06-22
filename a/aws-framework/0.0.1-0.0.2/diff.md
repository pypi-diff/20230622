# Comparing `tmp/aws_framework-0.0.1.tar.gz` & `tmp/aws_framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_framework-0.0.1.tar", max compression
+gzip compressed data, was "aws_framework-0.0.2.tar", max compression
```

## Comparing `aws_framework-0.0.1.tar` & `aws_framework-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,249 @@
--rw-r--r--   0        0        0      336 2023-06-21 09:29:22.057036 aws_framework-0.0.1/README.md
--rw-r--r--   0        0        0      426 2023-06-21 06:26:23.541471 aws_framework-0.0.1/aws_framework/__init__.py
--rw-r--r--   0        0        0     3234 2023-06-22 06:00:43.151011 aws_framework-0.0.1/aws_framework/_apprunner.py
--rw-r--r--   0        0        0    10188 2023-06-22 04:56:10.781891 aws_framework-0.0.1/aws_framework/_apprunnerTypes.py
--rw-r--r--   0        0        0     2979 2023-06-22 04:56:21.434729 aws_framework-0.0.1/aws_framework/_bucket.py
--rw-r--r--   0        0        0     6042 2023-06-21 01:52:42.904691 aws_framework-0.0.1/aws_framework/_ci_types.py
--rw-r--r--   0        0        0     1392 2023-06-22 04:56:10.757890 aws_framework-0.0.1/aws_framework/_cloudflare.py
--rw-r--r--   0        0        0     2107 2023-06-18 17:10:12.591255 aws_framework-0.0.1/aws_framework/_cognito.py
--rw-r--r--   0        0        0     2088 2023-06-22 05:03:26.864250 aws_framework-0.0.1/aws_framework/_config.py
--rw-r--r--   0        0        0     1471 2023-06-19 06:58:18.028929 aws_framework-0.0.1/aws_framework/_decorators.py
--rw-r--r--   0        0        0     1129 2023-06-15 22:31:36.265101 aws_framework-0.0.1/aws_framework/_exceptions.py
--rw-r--r--   0        0        0     7369 2023-06-17 03:34:06.090883 aws_framework-0.0.1/aws_framework/_fmt.py
--rw-r--r--   0        0        0     1699 2023-06-22 05:08:51.465829 aws_framework-0.0.1/aws_framework/_github.py
--rw-r--r--   0        0        0    10242 2023-06-22 02:21:22.881235 aws_framework-0.0.1/aws_framework/_swagger.py
--rw-r--r--   0        0        0     4848 2023-06-22 04:56:11.041912 aws_framework-0.0.1/aws_framework/_types.py
--rw-r--r--   0        0        0     8035 2023-06-22 04:56:11.193924 aws_framework-0.0.1/aws_framework/api.py
--rw-r--r--   0        0        0     7242 2023-06-22 04:56:11.257929 aws_framework-0.0.1/aws_framework/client.py
--rw-r--r--   0        0        0     3480 2023-06-22 04:56:11.325934 aws_framework-0.0.1/aws_framework/data.py
--rw-r--r--   0        0        0     2735 2023-06-18 23:42:36.620471 aws_framework-0.0.1/aws_framework/odm.py
--rw-r--r--   0        0        0     2632 2023-06-19 01:45:08.487558 aws_framework-0.0.1/aws_framework/repository.py
--rw-r--r--   0        0        0     6822 2023-06-18 21:56:10.109202 aws_framework-0.0.1/aws_framework/service.py
--rw-r--r--   0        0        0     1469 2023-06-19 22:44:58.912289 aws_framework-0.0.1/aws_framework/utils.py
--rw-r--r--   0        0        0      732 2023-06-22 06:10:31.729392 aws_framework-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 aws_framework-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-06-21 09:29:22.057036 aws_framework-0.0.2/README.md
+-rw-r--r--   0        0        0      426 2023-06-21 06:26:23.541471 aws_framework-0.0.2/aws_framework/__init__.py
+-rw-r--r--   0        0        0     3234 2023-06-22 06:00:43.151011 aws_framework-0.0.2/aws_framework/_apprunner.py
+-rw-r--r--   0        0        0    10188 2023-06-22 04:56:10.781891 aws_framework-0.0.2/aws_framework/_apprunnerTypes.py
+-rw-r--r--   0        0        0     2979 2023-06-22 04:56:21.434729 aws_framework-0.0.2/aws_framework/_bucket.py
+-rw-r--r--   0        0        0     6042 2023-06-21 01:52:42.904691 aws_framework-0.0.2/aws_framework/_ci_types.py
+-rw-r--r--   0        0        0     1392 2023-06-22 04:56:10.757890 aws_framework-0.0.2/aws_framework/_cloudflare.py
+-rw-r--r--   0        0        0     2107 2023-06-18 17:10:12.591255 aws_framework-0.0.2/aws_framework/_cognito.py
+-rw-r--r--   0        0        0     2088 2023-06-22 05:03:26.864250 aws_framework-0.0.2/aws_framework/_config.py
+-rw-r--r--   0        0        0     1471 2023-06-19 06:58:18.028929 aws_framework-0.0.2/aws_framework/_decorators.py
+-rw-r--r--   0        0        0     1129 2023-06-15 22:31:36.265101 aws_framework-0.0.2/aws_framework/_exceptions.py
+-rw-r--r--   0        0        0     7369 2023-06-17 03:34:06.090883 aws_framework-0.0.2/aws_framework/_fmt.py
+-rw-r--r--   0        0        0     1699 2023-06-22 05:08:51.465829 aws_framework-0.0.2/aws_framework/_github.py
+-rw-r--r--   0        0        0    10242 2023-06-22 02:21:22.881235 aws_framework-0.0.2/aws_framework/_swagger.py
+-rw-r--r--   0        0        0     4848 2023-06-22 04:56:11.041912 aws_framework-0.0.2/aws_framework/_types.py
+-rw-r--r--   0        0        0     8035 2023-06-22 04:56:11.193924 aws_framework-0.0.2/aws_framework/api.py
+-rw-r--r--   0        0        0     7242 2023-06-22 04:56:11.257929 aws_framework-0.0.2/aws_framework/client.py
+-rw-r--r--   0        0        0     3480 2023-06-22 04:56:11.325934 aws_framework-0.0.2/aws_framework/data.py
+-rw-r--r--   0        0        0     2735 2023-06-18 23:42:36.620471 aws_framework-0.0.2/aws_framework/odm.py
+-rw-r--r--   0        0        0     2632 2023-06-19 01:45:08.487558 aws_framework-0.0.2/aws_framework/repository.py
+-rw-r--r--   0        0        0      525 2023-06-20 11:23:06.967667 aws_framework-0.0.2/aws_framework/scripts/containers/codeserver/Dockerfile
+-rw-r--r--   0        0        0       13 2023-06-20 19:09:31.616926 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 19:09:34.385195 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/HEAD
+-rw-r--r--   0        0        0      262 2023-06-20 19:09:35.493303 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/hooks/update.sample
+-rw-r--r--   0        0        0      369 2023-06-20 19:09:31.616926 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 19:09:22.756064 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/info/exclude
+-rw-r--r--   0        0        0      623 2023-06-20 19:09:34.385195 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/logs/HEAD
+-rw-r--r--   0        0        0      408 2023-06-20 19:09:34.385195 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 19:09:35.493303 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      156 2023-06-20 19:09:31.616926 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/0f/17892b3335fda311e9a610dafbb1bcf5f29181
+-rw-r--r--   0        0        0      149 2023-06-20 19:09:31.616926 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/38/f3b423c51aa41a92c870f98e32cb6f647556be
+-rw-r--r--   0        0        0      133 2023-06-20 19:09:25.244306 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/44/6ebca1e803ef03429002d86e8c261aa5b84fa9
+-rw-r--r--   0        0        0      173 2023-06-20 19:09:25.240306 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/8f/5c91c2b42f5248af11d2a937d22066cd6c67b3
+-rw-r--r--   0        0        0     8500 2023-06-20 19:09:25.244306 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/ab/37744a72c9fa3bb633cc9b6397d99d48cdebf2
+-rw-r--r--   0        0        0      132 2023-06-20 19:09:25.240306 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/objects/b5/d034c774ab50744f187f398ce0bfe3ad0ea2f2
+-rw-r--r--   0        0        0       41 2023-06-20 19:09:34.385195 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 19:09:35.493303 aws_framework-0.0.2/aws_framework/scripts/containers/express/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      139 2023-06-22 05:59:02.103049 aws_framework-0.0.2/aws_framework/scripts/containers/express/Dockerfile
+-rw-r--r--   0        0        0      229 2023-06-18 18:40:13.854402 aws_framework-0.0.2/aws_framework/scripts/containers/express/index.js
+-rw-r--r--   0        0        0      163 2023-06-19 00:20:59.391825 aws_framework-0.0.2/aws_framework/scripts/containers/express/package.json
+-rw-r--r--   0        0        0    17738 2023-06-18 18:39:08.953570 aws_framework-0.0.2/aws_framework/scripts/containers/express/yarn.lock
+-rw-r--r--   0        0        0       13 2023-06-20 19:15:17.030515 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 19:15:20.126816 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/HEAD
+-rw-r--r--   0        0        0      262 2023-06-20 19:15:21.218922 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/hooks/update.sample
+-rw-r--r--   0        0        0      297 2023-06-20 19:15:17.030515 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 19:15:07.969634 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/info/exclude
+-rw-r--r--   0        0        0      623 2023-06-20 19:15:20.126816 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/logs/HEAD
+-rw-r--r--   0        0        0      408 2023-06-20 19:15:20.126816 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 19:15:21.218922 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      114 2023-06-20 19:15:10.557886 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/objects/0a/a38c512c7964cd21abf351448504498126fb9d
+-rw-r--r--   0        0        0      149 2023-06-20 19:15:17.030515 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/objects/5f/db186486498ca52bc8909c8cae75e5f7cebd59
+-rw-r--r--   0        0        0      165 2023-06-20 19:15:10.557886 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/objects/d9/cd87cf63e4008774a12dd1b3996d742d81d1e2
+-rw-r--r--   0        0        0      127 2023-06-20 19:15:17.030515 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/objects/e2/c399967e4dea7f0fd599bacc22011cea28128d
+-rw-r--r--   0        0        0       31 2023-06-20 19:15:10.557886 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/objects/f0/615cfd0938066d9730af294b004eb78858ada4
+-rw-r--r--   0        0        0       41 2023-06-20 19:15:20.126816 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 19:15:21.218922 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      213 2023-06-22 05:58:44.229641 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/Dockerfile
+-rw-r--r--   0        0        0      108 2023-06-19 22:44:59.564352 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/main.py
+-rw-r--r--   0        0        0       15 2023-06-18 18:34:01.246647 aws_framework-0.0.2/aws_framework/scripts/containers/fastapi/requirements.txt
+-rw-r--r--   0        0        0       13 2023-06-20 19:12:39.887234 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 19:12:41.683409 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/HEAD
+-rw-r--r--   0        0        0      260 2023-06-20 19:12:42.859523 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 19:12:30.214294 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/hooks/update.sample
+-rw-r--r--   0        0        0      297 2023-06-20 19:12:39.887234 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 19:12:30.210293 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/info/exclude
+-rw-r--r--   0        0        0      623 2023-06-20 19:12:41.683409 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/logs/HEAD
+-rw-r--r--   0        0        0      408 2023-06-20 19:12:41.683409 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 19:12:42.863524 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      162 2023-06-20 19:12:33.030567 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/objects/1f/a82304602d169683e26dea230afcc564bfe71f
+-rw-r--r--   0        0        0      136 2023-06-20 19:12:33.030567 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/objects/6d/9d134f4a5b6b019f721cda212f8d429d8770b7
+-rw-r--r--   0        0        0      150 2023-06-20 19:12:39.887234 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/objects/9c/6f3fa387f3c509c53213b902a645d58957a8a6
+-rw-r--r--   0        0        0       30 2023-06-20 19:12:33.030567 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/objects/f1/63f4d225b1dd4613d889863a04cb98b727dc0b
+-rw-r--r--   0        0        0      126 2023-06-20 19:12:39.887234 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/objects/f6/9effba823ae0c447f036e1943f8a810d54da68
+-rw-r--r--   0        0        0       41 2023-06-20 19:12:41.683409 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 19:12:42.863524 aws_framework-0.0.2/aws_framework/scripts/containers/flask/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      204 2023-06-22 05:59:14.964063 aws_framework-0.0.2/aws_framework/scripts/containers/flask/Dockerfile
+-rw-r--r--   0        0        0      142 2023-06-18 23:44:12.927637 aws_framework-0.0.2/aws_framework/scripts/containers/flask/app.py
+-rw-r--r--   0        0        0       14 2023-06-18 23:43:04.222525 aws_framework-0.0.2/aws_framework/scripts/containers/flask/requirements.txt
+-rw-r--r--   0        0        0       13 2023-06-20 19:05:22.576708 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 19:06:06.352965 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/HEAD
+-rw-r--r--   0        0        0      258 2023-06-20 19:06:07.453072 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 19:05:10.915574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/hooks/update.sample
+-rw-r--r--   0        0        0      217 2023-06-20 19:05:22.576708 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 19:05:10.911574 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/info/exclude
+-rw-r--r--   0        0        0      623 2023-06-20 19:06:06.352965 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/logs/HEAD
+-rw-r--r--   0        0        0      408 2023-06-20 19:06:06.348965 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 19:06:07.457073 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      149 2023-06-20 19:05:22.576708 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/objects/55/b6863f3b7bc88867421d765b54adc4dd83d946
+-rw-r--r--   0        0        0      244 2023-06-20 19:05:13.103787 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/objects/a1/b7a4ae30bddefa958eed965b1eaeb94601e9ad
+-rw-r--r--   0        0        0      448 2023-06-20 19:05:13.103787 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/objects/ed/6defd5129bd422ec31b625e26336920372337e
+-rw-r--r--   0        0        0       89 2023-06-20 19:05:22.576708 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/objects/fb/cb9ec780d937119b29f00b1075e248571001ae
+-rw-r--r--   0        0        0       41 2023-06-20 19:06:06.348965 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 19:06:07.457073 aws_framework-0.0.2/aws_framework/scripts/containers/php/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      726 2023-06-20 10:54:41.173794 aws_framework-0.0.2/aws_framework/scripts/containers/php/Dockerfile
+-rw-r--r--   0        0        0      312 2023-06-20 10:58:37.108737 aws_framework-0.0.2/aws_framework/scripts/containers/php/index.php
+-rw-r--r--   0        0        0       12 2023-06-20 12:04:57.903833 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 12:05:01.336167 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/HEAD
+-rw-r--r--   0        0        0      260 2023-06-20 12:05:02.780308 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 12:04:21.316275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 12:04:21.308275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 12:04:21.304274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 12:04:21.308275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 12:04:21.300274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 12:04:21.312275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 12:04:21.312275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 12:04:21.312275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 12:04:21.304274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 12:04:21.300274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 12:04:21.304274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 12:04:21.308275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 12:04:21.300274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 12:04:21.308275 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/hooks/update.sample
+-rw-r--r--   0        0        0      902 2023-06-20 12:04:57.903833 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 12:04:21.296274 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/info/exclude
+-rw-r--r--   0        0        0      622 2023-06-20 12:05:01.336167 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/logs/HEAD
+-rw-r--r--   0        0        0      407 2023-06-20 12:05:01.336167 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 12:05:02.780308 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      176 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/0f/f6b07db55db663cdf9cf744b998371e3d445ff
+-rw-r--r--   0        0        0       54 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/11/f02fe2a0061d6e6e1f271b21da95423b448b32
+-rw-r--r--   0        0        0      277 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/2c/d6dcc8618c11a9c9394d20470dc967da0df903
+-rw-r--r--   0        0        0      151 2023-06-20 12:04:57.903833 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/34/8cd9b0b2e9e3aa6ba7afd03710f2bc993480de
+-rw-r--r--   0        0        0      231 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/3e/93fb25331de3fa34e85165e38624edbb5ef458
+-rw-r--r--   0        0        0      164 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/42/872c59f5b01c9155864572bc2fbd5833a7406c
+-rw-r--r--   0        0        0      223 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/43/1d0c3def989bd64a397b57f82c296086d1538f
+-rw-r--r--   0        0        0      133 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/87/6f45b8a95cafa454833d2860bf39d8c5d291e5
+-rw-r--r--   0        0        0      348 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/a7/fc6fbf23de2a53e36754bc4a2c306d0291d7b2
+-rw-r--r--   0        0        0      272 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/a7/ffee13c03d1d20dc6e657589b1ef60795a169b
+-rw-r--r--   0        0        0      251 2023-06-20 12:04:57.903833 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/ba/5723c9029322e8621950e1f50f6fc0b5e45ae6
+-rw-r--r--   0        0        0      148 2023-06-20 12:04:57.903833 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/d2/7978ada85f87b3ca5e646523c7e3b4b1f19a28
+-rw-r--r--   0        0        0      256 2023-06-20 12:04:40.158108 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/objects/e0/d1c840806ee7f517c3d9774be4bcf9c4e889db
+-rw-r--r--   0        0        0       41 2023-06-20 12:05:01.336167 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 12:05:02.780308 aws_framework-0.0.2/aws_framework/scripts/containers/react/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      136 2023-06-20 10:30:00.693834 aws_framework-0.0.2/aws_framework/scripts/containers/react/Dockerfile
+-rw-r--r--   0        0        0      366 2023-06-20 10:30:00.701835 aws_framework-0.0.2/aws_framework/scripts/containers/react/index.html
+-rw-r--r--   0        0        0      407 2023-06-20 10:30:00.717836 aws_framework-0.0.2/aws_framework/scripts/containers/react/package.json
+-rw-r--r--   0        0        0      411 2023-06-20 10:30:00.913855 aws_framework-0.0.2/aws_framework/scripts/containers/react/src/App.tsx
+-rw-r--r--   0        0        0      250 2023-06-20 10:30:00.929857 aws_framework-0.0.2/aws_framework/scripts/containers/react/src/main.tsx
+-rw-r--r--   0        0        0      397 2023-06-20 10:30:00.929857 aws_framework-0.0.2/aws_framework/scripts/containers/react/src/style.css
+-rw-r--r--   0        0        0       38 2023-06-20 10:30:00.945858 aws_framework-0.0.2/aws_framework/scripts/containers/react/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2023-06-20 10:30:00.721837 aws_framework-0.0.2/aws_framework/scripts/containers/react/tsconfig.json
+-rw-r--r--   0        0        0      213 2023-06-20 10:30:00.733838 aws_framework-0.0.2/aws_framework/scripts/containers/react/tsconfig.node.json
+-rw-r--r--   0        0        0      417 2023-06-20 10:30:00.733838 aws_framework-0.0.2/aws_framework/scripts/containers/react/vite.config.ts
+-rw-r--r--   0        0        0       13 2023-06-20 19:03:48.427553 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2023-06-20 19:03:51.639865 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/HEAD
+-rw-r--r--   0        0        0      258 2023-06-20 19:03:53.564052 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/config
+-rw-r--r--   0        0        0       73 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4655 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/hooks/update.sample
+-rw-r--r--   0        0        0      902 2023-06-20 19:03:48.427553 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/index
+-rw-r--r--   0        0        0      240 2023-06-20 19:03:27.365505 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/info/exclude
+-rw-r--r--   0        0        0      623 2023-06-20 19:03:51.639865 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/logs/HEAD
+-rw-r--r--   0        0        0      408 2023-06-20 19:03:51.639865 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      177 2023-06-20 19:03:53.568053 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      134 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/05/c17402a4a92b87397786592fc5135e13b7a666
+-rw-r--r--   0        0        0       54 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/11/f02fe2a0061d6e6e1f271b21da95423b448b32
+-rw-r--r--   0        0        0      254 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/14/3557b5286bc14791d34c5a964941fb3470af70
+-rw-r--r--   0        0        0      246 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/19/e509c0fe2f11054fdcdd5011cdfa756cfa0180
+-rw-r--r--   0        0        0      249 2023-06-20 19:03:48.427553 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/1c/9387971ecaa46a2ce796ef4e9139530f190eb8
+-rw-r--r--   0        0        0       97 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/24/25c0f745bef4d009cb6661b62fd9dfd62960b0
+-rw-r--r--   0        0        0      149 2023-06-20 19:03:48.427553 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/26/a438a62f8b65571b66a5751aca07ec98a21f04
+-rw-r--r--   0        0        0      202 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/2d/86de6c82042f883bb49833256b677212cb0f5e
+-rw-r--r--   0        0        0      164 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/42/872c59f5b01c9155864572bc2fbd5833a7406c
+-rw-r--r--   0        0        0       15 2023-06-20 19:03:41.514881 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/4b/825dc642cb6eb9a060e54bf8d69288fbee4904
+-rw-r--r--   0        0        0      133 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/87/6f45b8a95cafa454833d2860bf39d8c5d291e5
+-rw-r--r--   0        0        0      152 2023-06-20 19:03:48.427553 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/e5/ecd6a118da305817ff0f6553cf2fdc5bd2239e
+-rw-r--r--   0        0        0      237 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/e8/6aca30daea8954b815d872852fd5a939024551
+-rw-r--r--   0        0        0      365 2023-06-20 19:03:46.475363 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/objects/f8/2888f3d0965ccce705eded475631739c36c887
+-rw-r--r--   0        0        0       41 2023-06-20 19:03:51.639865 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-06-20 19:03:53.564052 aws_framework-0.0.2/aws_framework/scripts/containers/vue/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0      136 2023-06-20 10:30:09.718711 aws_framework-0.0.2/aws_framework/scripts/containers/vue/Dockerfile
+-rw-r--r--   0        0        0      362 2023-06-20 10:30:09.738714 aws_framework-0.0.2/aws_framework/scripts/containers/vue/index.html
+-rw-r--r--   0        0        0      333 2023-06-20 10:30:09.746714 aws_framework-0.0.2/aws_framework/scripts/containers/vue/package.json
+-rw-r--r--   0        0        0      361 2023-06-20 10:30:09.926732 aws_framework-0.0.2/aws_framework/scripts/containers/vue/src/App.vue
+-rw-r--r--   0        0        0      111 2023-06-20 10:30:09.974737 aws_framework-0.0.2/aws_framework/scripts/containers/vue/src/main.ts
+-rw-r--r--   0        0        0      454 2023-06-20 10:30:09.978737 aws_framework-0.0.2/aws_framework/scripts/containers/vue/src/style.css
+-rw-r--r--   0        0        0       38 2023-06-20 10:30:09.978737 aws_framework-0.0.2/aws_framework/scripts/containers/vue/src/vite-env.d.ts
+-rw-r--r--   0        0        0      661 2023-06-20 10:30:09.746714 aws_framework-0.0.2/aws_framework/scripts/containers/vue/tsconfig.json
+-rw-r--r--   0        0        0      213 2023-06-20 10:30:09.770717 aws_framework-0.0.2/aws_framework/scripts/containers/vue/tsconfig.node.json
+-rw-r--r--   0        0        0      157 2023-06-20 10:30:09.770717 aws_framework-0.0.2/aws_framework/scripts/containers/vue/vite.config.ts
+-rw-r--r--   0        0        0      780 2023-06-22 06:15:50.490511 aws_framework-0.0.2/aws_framework/scripts/main.py
+-rw-r--r--   0        0        0     6822 2023-06-18 21:56:10.109202 aws_framework-0.0.2/aws_framework/service.py
+-rw-r--r--   0        0        0     1469 2023-06-19 22:44:58.912289 aws_framework-0.0.2/aws_framework/utils.py
+-rw-r--r--   0        0        0      751 2023-06-22 06:16:06.363762 aws_framework-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 aws_framework-0.0.2/PKG-INFO
```

### Comparing `aws_framework-0.0.1/aws_framework/_apprunner.py` & `aws_framework-0.0.2/aws_framework/_apprunner.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_apprunnerTypes.py` & `aws_framework-0.0.2/aws_framework/_apprunnerTypes.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_bucket.py` & `aws_framework-0.0.2/aws_framework/_bucket.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_ci_types.py` & `aws_framework-0.0.2/aws_framework/_ci_types.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_cloudflare.py` & `aws_framework-0.0.2/aws_framework/_cloudflare.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_cognito.py` & `aws_framework-0.0.2/aws_framework/_cognito.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_config.py` & `aws_framework-0.0.2/aws_framework/_config.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_decorators.py` & `aws_framework-0.0.2/aws_framework/_decorators.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_exceptions.py` & `aws_framework-0.0.2/aws_framework/_exceptions.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_fmt.py` & `aws_framework-0.0.2/aws_framework/_fmt.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_github.py` & `aws_framework-0.0.2/aws_framework/_github.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_swagger.py` & `aws_framework-0.0.2/aws_framework/_swagger.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/_types.py` & `aws_framework-0.0.2/aws_framework/_types.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/api.py` & `aws_framework-0.0.2/aws_framework/api.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/client.py` & `aws_framework-0.0.2/aws_framework/client.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/data.py` & `aws_framework-0.0.2/aws_framework/data.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/odm.py` & `aws_framework-0.0.2/aws_framework/odm.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/repository.py` & `aws_framework-0.0.2/aws_framework/repository.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/service.py` & `aws_framework-0.0.2/aws_framework/service.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/aws_framework/utils.py` & `aws_framework-0.0.2/aws_framework/utils.py`

 * *Files identical despite different names*

### Comparing `aws_framework-0.0.1/pyproject.toml` & `aws_framework-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-framework"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Demo Framework for the AWS Workshop"
 authors = ["Oscar Bahamonde <oscar.bahamonde@pucp.pe>"]
 readme = "README.md"
 packages = [{include = "aws_framework"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
@@ -23,8 +23,8 @@
 botocore-stubs = "^1.29.155"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-boto = "scripts:main"
+boto = "aws_framework.scripts.main:main"
```

### Comparing `aws_framework-0.0.1/PKG-INFO` & `aws_framework-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-framework
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Demo Framework for the AWS Workshop
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde@pucp.pe
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

