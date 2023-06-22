# Comparing `tmp/grpclib-0.4.4.tar.gz` & `tmp/grpclib-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpclib-0.4.4.tar", last modified: Thu May 11 19:29:29 2023, max compression
+gzip compressed data, was "dist/grpclib-0.4.5.tar", last modified: Thu Jun 22 20:52:23 2023, max compression
```

## Comparing `grpclib-0.4.4.tar` & `grpclib-0.4.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 19:29:11.000000 grpclib-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-11 19:29:29.000000 grpclib-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-11 19:29:11.000000 grpclib-0.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/channelz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/channelz/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    54996 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34946 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/health/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26879 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 19:29:11.000000 grpclib-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-11 19:29:29.000000 grpclib-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 19:29:11.000000 grpclib-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-22 20:52:00.000000 grpclib-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-22 20:52:23.000000 grpclib-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-22 20:52:00.000000 grpclib-0.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/channelz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/channelz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/channelz/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/channelz/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/channelz/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/channelz/v1/channelz_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/channelz/v1/channelz_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54996 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34946 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/encoding/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/health/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/health/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/health/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/health/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/health/v1/health_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/health/v1/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/health/v1/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/reflection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/reflection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/reflection/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/reflection/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/reflection/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/reflection/v1/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/reflection/v1/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-22 20:52:20.000000 grpclib-0.4.5/grpclib/reflection/v1/reflection_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib/reflection/v1alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/reflection/v1alpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-06-22 20:52:21.000000 grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26879 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-22 20:52:00.000000 grpclib-0.4.5/grpclib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 20:52:23.000000 grpclib-0.4.5/grpclib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 20:52:00.000000 grpclib-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-22 20:52:23.000000 grpclib-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 20:52:00.000000 grpclib-0.4.5/setup.py
```

### Comparing `grpclib-0.4.4/LICENSE.txt` & `grpclib-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/PKG-INFO` & `grpclib-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
```

### Comparing `grpclib-0.4.4/README.rst` & `grpclib-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/_typing.py` & `grpclib-0.4.5/grpclib/_typing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/channelz/service.py` & `grpclib-0.4.5/grpclib/channelz/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/channelz/v1/channelz_grpc.py` & `grpclib-0.4.5/grpclib/channelz/v1/channelz_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.py` & `grpclib-0.4.5/grpclib/channelz/v1/channelz_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.pyi` & `grpclib-0.4.5/grpclib/channelz/v1/channelz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/client.py` & `grpclib-0.4.5/grpclib/client.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/config.py` & `grpclib-0.4.5/grpclib/config.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/const.py` & `grpclib-0.4.5/grpclib/const.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/encoding/base.py` & `grpclib-0.4.5/grpclib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/encoding/proto.py` & `grpclib-0.4.5/grpclib/encoding/proto.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/events.py` & `grpclib-0.4.5/grpclib/events.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/exceptions.py` & `grpclib-0.4.5/grpclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/health/check.py` & `grpclib-0.4.5/grpclib/health/check.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/health/service.py` & `grpclib-0.4.5/grpclib/health/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/health/v1/health_grpc.py` & `grpclib-0.4.5/grpclib/health/v1/health_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/health/v1/health_pb2.py` & `grpclib-0.4.5/grpclib/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/health/v1/health_pb2.pyi` & `grpclib-0.4.5/grpclib/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/metadata.py` & `grpclib-0.4.5/grpclib/metadata.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/plugin/main.py` & `grpclib-0.4.5/grpclib/plugin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
         buf.add('')
         buf.add('class {}Stub:', service.name)
         with buf.indent():
             buf.add('')
             buf.add('def __init__(self, channel: {}.{}) -> None:'
                     .format(client.__name__, client.Channel.__name__))
             with buf.indent():
+                if len(service.methods) == 0:
+                    buf.add('pass')
                 for method in service.methods:
                     name, cardinality, request_type, reply_type = method
                     full_name = '/{}/{}'.format(service_name, name)
                     method_cls: type
                     if cardinality is const.Cardinality.UNARY_UNARY:
                         method_cls = client.UnaryUnaryMethod
                     elif cardinality is const.Cardinality.UNARY_STREAM:
```

### Comparing `grpclib-0.4.4/grpclib/protocol.py` & `grpclib-0.4.5/grpclib/protocol.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/_deprecated.py` & `grpclib-0.4.5/grpclib/reflection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/service.py` & `grpclib-0.4.5/grpclib/reflection/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1/reflection_grpc.py` & `grpclib-0.4.5/grpclib/reflection/v1/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.py` & `grpclib-0.4.5/grpclib/reflection/v1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.pyi` & `grpclib-0.4.5/grpclib/reflection/v1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_grpc.py` & `grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.py` & `grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.pyi` & `grpclib-0.4.5/grpclib/reflection/v1alpha/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/server.py` & `grpclib-0.4.5/grpclib/server.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/stream.py` & `grpclib-0.4.5/grpclib/stream.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/testing.py` & `grpclib-0.4.5/grpclib/testing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib/utils.py` & `grpclib-0.4.5/grpclib/utils.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/grpclib.egg-info/PKG-INFO` & `grpclib-0.4.5/grpclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
```

### Comparing `grpclib-0.4.4/grpclib.egg-info/SOURCES.txt` & `grpclib-0.4.5/grpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.4/setup.cfg` & `grpclib-0.4.5/setup.cfg`

 * *Files identical despite different names*

