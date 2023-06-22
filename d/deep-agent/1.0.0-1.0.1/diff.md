# Comparing `tmp/deep_agent-1.0.0.tar.gz` & `tmp/deep_agent-1.0.1.tar.gz`

## Comparing `deep_agent-1.0.0.tar` & `deep_agent-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/__init__.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/version.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/__init__.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/deep.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/types.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/attributes/__init__.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/auth/__init__.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/__init__.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/otel.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/python.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/resource/__init__.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/__init__.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/eventsnapshot.py
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/tracepoint_config.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/__init__.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/config_service.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/tracepoint_config.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/grpc/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/grpc/grpc_service.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/logging/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/logging/logging.conf
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/poll/__init__.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/poll/poll.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/__init__.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_collector.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_config.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_processor.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/trigger_handler.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/variable_processor.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/bfs/__init__.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/push/__init__.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/push/push_service.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/task/__init__.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 deep_agent-1.0.0/.gitignore
--rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 deep_agent-1.0.0/LICENSE
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 deep_agent-1.0.0/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 deep_agent-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 deep_agent-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/__init__.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/version.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/deep.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/types.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/attributes/__init__.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/auth/__init__.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/plugin/__init__.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/plugin/otel.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/plugin/python.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/resource/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/tracepoint/__init__.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/tracepoint/eventsnapshot.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/api/tracepoint/tracepoint_config.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/config/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/config/config_service.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/config/tracepoint_config.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/grpc/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/grpc/grpc_service.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/logging/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/logging/logging.conf
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/poll/__init__.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/poll/poll.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/__init__.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/frame_collector.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/frame_config.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/frame_processor.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/trigger_handler.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/variable_processor.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/processor/bfs/__init__.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/push/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/push/push_service.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 deep_agent-1.0.1/src/deep/task/__init__.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 deep_agent-1.0.1/.gitignore
+-rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 deep_agent-1.0.1/LICENSE
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 deep_agent-1.0.1/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 deep_agent-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 deep_agent-1.0.1/PKG-INFO
```

### Comparing `deep_agent-1.0.0/src/deep/__init__.py` & `deep_agent-1.0.1/src/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/utils.py` & `deep_agent-1.0.1/src/deep/utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/version.py` & `deep_agent-1.0.1/src/deep/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #      (at your option) any later version.
 #
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 
-__version__ = "1.0.0"  # this version is set by the build, but not updated in the code.
+__version__ = "1.0.1"  # this version is set by the build, but not updated in the code.
 """The version of the agent that is running."""
```

### Comparing `deep_agent-1.0.0/src/deep/api/__init__.py` & `deep_agent-1.0.1/src/deep/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/deep.py` & `deep_agent-1.0.1/src/deep/api/deep.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/types.py` & `deep_agent-1.0.1/src/deep/api/types.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/attributes/__init__.py` & `deep_agent-1.0.1/src/deep/api/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/auth/__init__.py` & `deep_agent-1.0.1/src/deep/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/plugin/__init__.py` & `deep_agent-1.0.1/src/deep/api/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/plugin/otel.py` & `deep_agent-1.0.1/src/deep/api/plugin/otel.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/plugin/python.py` & `deep_agent-1.0.1/src/deep/api/plugin/python.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/resource/__init__.py` & `deep_agent-1.0.1/src/deep/api/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/tracepoint/__init__.py` & `deep_agent-1.0.1/src/deep/api/tracepoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/tracepoint/eventsnapshot.py` & `deep_agent-1.0.1/src/deep/api/tracepoint/eventsnapshot.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/api/tracepoint/tracepoint_config.py` & `deep_agent-1.0.1/src/deep/api/tracepoint/tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/config/__init__.py` & `deep_agent-1.0.1/src/deep/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/config/config_service.py` & `deep_agent-1.0.1/src/deep/config/config_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             # if not in custom then load from 'deep.config'
             if attr is None:
                 from deep import config
                 has_attr = hasattr(config, name)
                 if not has_attr:
                     # attribute is no in 'deep.config', so look in env
-                    from_env = os.getenv(name, None)
+                    from_env = os.getenv("DEEP_%s" % name, None)
                     if from_env is None:
                         # not found in env - log and return none
                         logging.warning("Unrecognised config key: %s", name)
                         return None
                     else:
                         # if loaded from env, then cannot be function
                         return from_env
```

### Comparing `deep_agent-1.0.0/src/deep/config/tracepoint_config.py` & `deep_agent-1.0.1/src/deep/config/tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/grpc/__init__.py` & `deep_agent-1.0.1/src/deep/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/grpc/grpc_service.py` & `deep_agent-1.0.1/src/deep/grpc/grpc_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/logging/__init__.py` & `deep_agent-1.0.1/src/deep/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/poll/__init__.py` & `deep_agent-1.0.1/src/deep/poll/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/poll/poll.py` & `deep_agent-1.0.1/src/deep/poll/poll.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/__init__.py` & `deep_agent-1.0.1/src/deep/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/frame_collector.py` & `deep_agent-1.0.1/src/deep/processor/frame_collector.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/frame_config.py` & `deep_agent-1.0.1/src/deep/processor/frame_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/frame_processor.py` & `deep_agent-1.0.1/src/deep/processor/frame_processor.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/trigger_handler.py` & `deep_agent-1.0.1/src/deep/processor/trigger_handler.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/variable_processor.py` & `deep_agent-1.0.1/src/deep/processor/variable_processor.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/processor/bfs/__init__.py` & `deep_agent-1.0.1/src/deep/processor/bfs/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/push/__init__.py` & `deep_agent-1.0.1/src/deep/push/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/push/push_service.py` & `deep_agent-1.0.1/src/deep/push/push_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/src/deep/task/__init__.py` & `deep_agent-1.0.1/src/deep/task/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/.gitignore` & `deep_agent-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/LICENSE` & `deep_agent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/README.md` & `deep_agent-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/pyproject.toml` & `deep_agent-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deep_agent-1.0.0/PKG-INFO` & `deep_agent-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: DEEP Python Agent
 Author-email: Intergral GmbH <support@intergral.com>, Ben Donnelly <b.w.donnelly1@gmail.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

