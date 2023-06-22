# Comparing `tmp/kpops-1.2.2.tar.gz` & `tmp/kpops-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.2.2.tar", max compression
+gzip compressed data, was "kpops-1.2.3.tar", max compression
```

## Comparing `kpops-1.2.2.tar` & `kpops-1.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1064 2023-06-21 14:31:45.886680 kpops-1.2.2/LICENSE
--rw-r--r--   0        0        0     2350 2023-06-21 14:31:45.886680 kpops-1.2.2/README.md
--rw-r--r--   0        0        0       22 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/exception.py
--rw-r--r--   0        0        0    11727 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/main.py
--rw-r--r--   0        0        0     4206 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1969 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       52 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0    10517 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     4341 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8142 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      235 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5832 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1825 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      999 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6272 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      231 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9358 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6917 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     7127 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     6658 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    15917 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     7306 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0       66 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2471 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3340 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     8915 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1110 2023-06-21 14:31:45.890680 kpops-1.2.2/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2831 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9067 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3463 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    13226 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     3878 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2597 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1032 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/environment.py
--rw-r--r--   0        0        0     5620 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      552 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     2563 2023-06-21 14:31:45.894680 kpops-1.2.2/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1900 2023-06-21 14:31:45.894680 kpops-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-22 09:32:13.753019 kpops-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2350 2023-06-22 09:32:13.753019 kpops-1.2.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11727 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/main.py
+-rw-r--r--   0        0        0     4206 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1969 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       52 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0    10517 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4341 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8142 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      235 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5832 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1825 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      999 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6272 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9358 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6917 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     7711 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     6658 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    15917 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6941 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0       66 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2471 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3340 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     8915 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1110 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2831 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9067 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3463 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    13148 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     3878 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2597 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1032 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5620 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      552 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     2563 2023-06-22 09:32:13.761019 kpops-1.2.3/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1900 2023-06-22 09:32:13.761019 kpops-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.2.3/PKG-INFO
```

### Comparing `kpops-1.2.2/LICENSE` & `kpops-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/README.md` & `kpops-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/cli/custom_formatter.py` & `kpops-1.2.3/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/cli/main.py` & `kpops-1.2.3/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/cli/pipeline_config.py` & `kpops-1.2.3/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/cli/registry.py` & `kpops-1.2.3/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/__init__.py` & `kpops-1.2.3/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-1.2.3/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.2.3/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.2.3/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.2.3/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.2.3/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.2.3/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.2.3/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.2.3/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.2.3/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.2.3/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/topic/handler.py` & `kpops-1.2.3/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/topic/model.py` & `kpops-1.2.3/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.2.3/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/topic/utils.py` & `kpops-1.2.3/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/component_handlers/utils/exception.py` & `kpops-1.2.3/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/base_components/base_defaults_component.py` & `kpops-1.2.3/kpops/components/base_components/base_defaults_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     :type type: str
     :param enrich: Whether to enrich component with defaults, defaults to False
     :type enrich: bool, optional
     :param config: Pipeline configuration to be accessed by this component
     :type config: PipelineConfig
     :param handlers: Component handlers to be accessed by this component
     :type handlers: ComponentHandlers
+    :param validate: Whether to run custom validation on the component, defaults to True
+    :type validate: bool, optional
     """
 
     type: str = Field(
         default=..., description=describe_attr("type", __doc__), const=True
     )
 
     enrich: bool = Field(
@@ -54,22 +56,31 @@
     )
     handlers: ComponentHandlers = Field(
         default=...,
         description=describe_attr("handlers", __doc__),
         exclude=True,
         hidden_from_schema=True,
     )
+    validate_: bool = Field(
+        alias="validate",
+        default=True,
+        description=describe_attr("validate", __doc__),
+        exclude=True,
+        hidden_from_schema=True,
+    )
 
     class Config(DescConfig):
         arbitrary_types_allowed = True
 
     def __init__(self, **kwargs) -> None:
         if kwargs.get("enrich", True):
             kwargs = self.extend_with_defaults(**kwargs)
         super().__init__(**kwargs)
+        if kwargs.get("validate", True):
+            self._validate_custom(**kwargs)
 
     @classmethod  # NOTE: property as classmethod deprecated in Python 3.11
     def get_component_type(cls) -> str:
         """Return calling component's type
 
         :returns: Component type
         :rtype: str
@@ -100,14 +111,21 @@
         )
         defaults = load_defaults(
             self.__class__, main_default_file_path, environment_default_file_path
         )
         kwargs = update_nested(kwargs, defaults)
         return kwargs
 
+    def _validate_custom(self, **kwargs) -> None:
+        """Run custom validation on component.
+
+        :param kwargs: The init kwargs for the component
+        """
+        pass
+
 
 def load_defaults(
     component_class: type[BaseDefaultsComponent],
     defaults_file_path: Path,
     environment_defaults_file_path: Path | None = None,
 ) -> dict:
     """Resolve component-specific defaults including environment defaults
```

### Comparing `kpops-1.2.2/kpops/components/base_components/kafka_app.py` & `kpops-1.2.3/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/base_components/kafka_connector.py` & `kpops-1.2.3/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/base_components/kubernetes_app.py` & `kpops-1.2.3/kpops/components/base_components/kubernetes_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     """Base class for all Kubernetes apps.
 
     All built-in components are Kubernetes apps, except for the Kafka connectors.
 
     :param type: Component type, defaults to "kubernetes-app"
     :param schema_type: Used for schema generation, same as :param:`type`,
         defaults to "kubernetes-app"
-    :param validate_name: Whether to check if the name of the component is
-        compatible with Kubernetes, defaults to True
     :param app: Application-specific settings
     :param repo_config: Configuration of the Helm chart repo to be used for
         deploying the component, defaults to None
     :param namespace: Namespace in which the component shall be deployed
     :param version: Helm chart version, defaults to None
     """
 
@@ -58,20 +56,14 @@
     )
     schema_type: Literal["kubernetes-app"] = Field(
         default="kubernetes-app",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
-    validate_name: bool = Field(
-        default=True,
-        description=describe_attr("validate_name", __doc__),
-        exclude=True,
-        hidden_from_schema=True,
-    )
     app: KubernetesAppConfig = Field(
         default=...,
         description=describe_attr("app", __doc__),
     )
     repo_config: HelmRepoConfig | None = Field(
         default=None,
         description=describe_attr("repo_config", __doc__),
@@ -84,19 +76,14 @@
         default=None,
         description=describe_attr("version", __doc__),
     )
 
     class Config(CamelCaseConfig, DescConfig):
         pass
 
-    def __init__(self, **kwargs):
-        if kwargs.get("validate_name", True):
-            self.validate_kubernetes_name(kwargs["name"])
-        super().__init__(**kwargs)
-
     @cached_property
     def helm(self) -> Helm:
         """Helm object that contains component-specific config such as repo"""
         helm = Helm(self.config.helm_config)
         if self.repo_config is not None:
             helm.add_repo(
                 self.repo_config.repository_name,
@@ -117,14 +104,18 @@
 
     @property
     def helm_release_name(self) -> str:
         """The name for the Helm release. Can be overridden."""
         return self.name
 
     @override
+    def _validate_custom(self, **kwargs) -> None:
+        self.validate_kubernetes_name(self.name)
+
+    @override
     def template(
         self, api_version: str | None, ca_file: str | None, cert_file: str | None
     ) -> None:
         flags = HelmTemplateFlags(api_version, ca_file, cert_file, self.version)
         stdout = self.helm.template(
             self.helm_release_name,
             self.get_helm_chart(),
```

### Comparing `kpops-1.2.2/kpops/components/base_components/models/from_section.py` & `kpops-1.2.3/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/base_components/models/to_section.py` & `kpops-1.2.3/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/base_components/pipeline_component.py` & `kpops-1.2.3/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.2.3/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.2.3/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.2.3/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.2.3/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/pipeline_generator/pipeline.py` & `kpops-1.2.3/kpops/pipeline_generator/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         :type component_class: type[PipelineComponent]
         :param component_data: Arguments for instantiation of pipeline component
         :type component_data: dict
         """
         component = component_class(
             config=self.config,
             handlers=self.handlers,
-            validate_name=False,
+            validate=False,
             **component_data,
         )
         component = self.enrich_component(component)
 
         # inflate & enrich components
         for inflated_component in component.inflate():  # TODO: recursively
             enriched_component = self.enrich_component(inflated_component)
@@ -226,21 +226,20 @@
         """Enrich a pipeline component with env-specific config and substitute variables
 
         :param component: Component to be enriched
         :type component: PipelineComponent
         :returns: Enriched component
         :rtype: PipelineComponent
         """
+        component.validate_ = True
         env_component_as_dict = update_nested_pair(
             self.env_components_index.get(component.name, {}),
             # HACK: Pydantic .dict() doesn't create jsonable dict
             json.loads(component.json(by_alias=True)),
         )
-        if "validate_name" in env_component_as_dict:
-            del env_component_as_dict["validate_name"]
 
         component_data = self.substitute_in_component(env_component_as_dict)
 
         component_class = type(component)
         return component_class(
             enrich=False,
             config=self.config,
```

### Comparing `kpops-1.2.2/kpops/utils/dict_differ.py` & `kpops-1.2.3/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/dict_ops.py` & `kpops-1.2.3/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/docstring.py` & `kpops-1.2.3/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/environment.py` & `kpops-1.2.3/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/gen_schema.py` & `kpops-1.2.3/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/pydantic.py` & `kpops-1.2.3/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/kpops/utils/yaml_loading.py` & `kpops-1.2.3/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.2.2/pyproject.toml` & `kpops-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.2.2"
+version = "1.2.3"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-1.2.2/PKG-INFO` & `kpops-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.2.2
+Version: 1.2.3
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
```

