# Comparing `tmp/nodestream-0.2.0.tar.gz` & `tmp/nodestream-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream-0.2.0.tar", max compression
+gzip compressed data, was "nodestream-0.3.0.tar", max compression
```

## Comparing `nodestream-0.2.0.tar` & `nodestream-0.3.0.tar`

### file list

```diff
@@ -1,122 +1,124 @@
--rw-r--r--   0        0        0    32335 2023-05-18 13:51:44.150322 nodestream-0.2.0/LICENSE
--rw-r--r--   0        0        0     1629 2023-06-05 20:55:40.249844 nodestream-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-18 13:51:44.151306 nodestream-0.2.0/nodestream/__init__.py
--rw-r--r--   0        0        0      321 2023-06-06 14:48:12.777929 nodestream-0.2.0/nodestream/argument_resolvers/__init__.py
--rw-r--r--   0        0        0      440 2023-06-06 14:48:12.778117 nodestream-0.2.0/nodestream/argument_resolvers/argument_resolver.py
--rw-r--r--   0        0        0      600 2023-06-06 14:48:12.778550 nodestream-0.2.0/nodestream/argument_resolvers/environment_variable_resolver.py
--rw-r--r--   0        0        0      689 2023-06-06 14:48:12.778951 nodestream-0.2.0/nodestream/argument_resolvers/include_file_resolver.py
--rw-r--r--   0        0        0      262 2023-06-08 00:32:08.908151 nodestream-0.2.0/nodestream/audits/__init__.py
--rw-r--r--   0        0        0      695 2023-06-08 00:37:19.628414 nodestream-0.2.0/nodestream/audits/audit.py
--rw-r--r--   0        0        0      375 2023-06-08 00:27:12.187711 nodestream-0.2.0/nodestream/audits/audit_printer.py
--rw-r--r--   0        0        0     1635 2023-06-08 14:38:42.505682 nodestream-0.2.0/nodestream/audits/audit_referencial_integrity.py
--rw-r--r--   0        0        0     1516 2023-06-08 14:22:33.346618 nodestream-0.2.0/nodestream/audits/audit_ttls.py
--rw-r--r--   0        0        0      109 2023-05-29 23:36:36.044355 nodestream-0.2.0/nodestream/cli/__init__.py
--rw-r--r--   0        0        0      924 2023-06-08 00:35:45.179471 nodestream-0.2.0/nodestream/cli/application.py
--rw-r--r--   0        0        0      250 2023-06-05 20:55:40.270364 nodestream-0.2.0/nodestream/cli/commands/__init__.py
--rw-r--r--   0        0        0      482 2023-06-08 00:34:18.198907 nodestream-0.2.0/nodestream/cli/commands/audit_command.py
--rw-r--r--   0        0        0      268 2023-06-08 00:35:30.685238 nodestream-0.2.0/nodestream/cli/commands/audit_refs.py
--rw-r--r--   0        0        0      204 2023-06-08 00:34:41.019749 nodestream-0.2.0/nodestream/cli/commands/audit_ttls.py
--rw-r--r--   0        0        0     1090 2023-06-05 20:55:40.270526 nodestream-0.2.0/nodestream/cli/commands/new.py
--rw-r--r--   0        0        0     1108 2023-06-08 00:13:08.470729 nodestream-0.2.0/nodestream/cli/commands/nodestream_command.py
--rw-r--r--   0        0        0     1213 2023-06-07 19:09:40.099387 nodestream-0.2.0/nodestream/cli/commands/print_schema.py
--rw-r--r--   0        0        0      893 2023-06-05 20:55:40.270803 nodestream-0.2.0/nodestream/cli/commands/remove.py
--rw-r--r--   0        0        0     1087 2023-06-06 14:48:12.780185 nodestream-0.2.0/nodestream/cli/commands/run.py
--rw-r--r--   0        0        0     1342 2023-06-05 20:55:40.271104 nodestream-0.2.0/nodestream/cli/commands/scaffold.py
--rw-r--r--   0        0        0      508 2023-06-06 14:48:12.780577 nodestream-0.2.0/nodestream/cli/commands/shared_options.py
--rw-r--r--   0        0        0      596 2023-06-05 20:55:40.271384 nodestream-0.2.0/nodestream/cli/commands/show.py
--rw-r--r--   0        0        0      986 2023-06-08 00:02:45.190774 nodestream-0.2.0/nodestream/cli/operations/__init__.py
--rw-r--r--   0        0        0      988 2023-06-05 20:55:40.271830 nodestream-0.2.0/nodestream/cli/operations/add_pipeline_to_project.py
--rw-r--r--   0        0        0      438 2023-06-05 20:55:40.271946 nodestream-0.2.0/nodestream/cli/operations/commit_project_to_disk.py
--rw-r--r--   0        0        0     2153 2023-06-05 20:55:40.272099 nodestream-0.2.0/nodestream/cli/operations/generate_pipeline_scaffold.py
--rw-r--r--   0        0        0     1434 2023-06-05 20:55:40.272303 nodestream-0.2.0/nodestream/cli/operations/generate_project.py
--rw-r--r--   0        0        0     2317 2023-06-05 20:55:40.272481 nodestream-0.2.0/nodestream/cli/operations/generate_python_scaffold.py
--rw-r--r--   0        0        0      370 2023-06-05 20:55:40.272873 nodestream-0.2.0/nodestream/cli/operations/initialize_logger.py
--rw-r--r--   0        0        0      339 2023-06-05 20:55:40.273047 nodestream-0.2.0/nodestream/cli/operations/initialize_project.py
--rw-r--r--   0        0        0      384 2023-06-05 20:55:40.273394 nodestream-0.2.0/nodestream/cli/operations/operation.py
--rw-r--r--   0        0        0     1208 2023-06-07 19:09:40.100607 nodestream-0.2.0/nodestream/cli/operations/print_project_schema.py
--rw-r--r--   0        0        0      533 2023-06-05 20:55:40.273559 nodestream-0.2.0/nodestream/cli/operations/remove_pipeline_from_project.py
--rw-r--r--   0        0        0     1137 2023-06-08 00:31:31.712160 nodestream-0.2.0/nodestream/cli/operations/run_audit.py
--rw-r--r--   0        0        0     2337 2023-06-05 20:55:40.273891 nodestream-0.2.0/nodestream/cli/operations/run_pipeline.py
--rw-r--r--   0        0        0     2399 2023-06-05 20:55:40.274048 nodestream-0.2.0/nodestream/cli/operations/show_pipelines.py
--rw-r--r--   0        0        0      329 2023-06-07 19:09:40.100995 nodestream-0.2.0/nodestream/cli/schema_printers/__init__.py
--rw-r--r--   0        0        0     5717 2023-06-07 19:09:40.101284 nodestream-0.2.0/nodestream/cli/schema_printers/graphql_schema_printer.py
--rw-r--r--   0        0        0      272 2023-06-07 19:09:40.101737 nodestream-0.2.0/nodestream/cli/schema_printers/plain_text_schema_printer.py
--rw-r--r--   0        0        0      634 2023-06-07 19:09:40.102022 nodestream-0.2.0/nodestream/cli/schema_printers/schema_printer.py
--rw-r--r--   0        0        0      165 2023-05-19 19:07:54.211393 nodestream-0.2.0/nodestream/databases/__init__.py
--rw-r--r--   0        0        0     2958 2023-06-06 14:48:12.780980 nodestream-0.2.0/nodestream/databases/debounced_ingest_strategy.py
--rw-r--r--   0        0        0      166 2023-05-23 15:05:18.008404 nodestream-0.2.0/nodestream/databases/neo4j/__init__.py
--rw-r--r--   0        0        0     2673 2023-06-06 17:09:46.058615 nodestream-0.2.0/nodestream/databases/neo4j/index_query_builder.py
--rw-r--r--   0        0        0     8831 2023-06-06 14:48:12.781801 nodestream-0.2.0/nodestream/databases/neo4j/ingest_query_builder.py
--rw-r--r--   0        0        0     1034 2023-05-23 15:05:18.009754 nodestream-0.2.0/nodestream/databases/neo4j/query.py
--rw-r--r--   0        0        0     3934 2023-06-06 14:48:12.782196 nodestream-0.2.0/nodestream/databases/neo4j/query_executor.py
--rw-r--r--   0        0        0     2793 2023-05-25 20:54:40.568938 nodestream-0.2.0/nodestream/databases/operation_debouncer.py
--rw-r--r--   0        0        0     2060 2023-06-06 14:48:12.782584 nodestream-0.2.0/nodestream/databases/query_executor.py
--rw-r--r--   0        0        0     1661 2023-06-06 14:48:12.783036 nodestream-0.2.0/nodestream/databases/writer.py
--rw-r--r--   0        0        0     2547 2023-06-06 14:48:12.783447 nodestream-0.2.0/nodestream/exceptions.py
--rw-r--r--   0        0        0       63 2023-05-24 19:45:31.927731 nodestream-0.2.0/nodestream/extractors/__init__.py
--rw-r--r--   0        0        0     2641 2023-06-06 17:09:46.059395 nodestream-0.2.0/nodestream/extractors/files.py
--rw-r--r--   0        0        0        0 2023-05-18 13:51:44.153895 nodestream-0.2.0/nodestream/extractors/stores/__init__.py
--rw-r--r--   0        0        0      130 2023-06-05 20:55:40.275076 nodestream-0.2.0/nodestream/extractors/stores/aws/__init__.py
--rw-r--r--   0        0        0     4568 2023-05-24 18:15:07.882841 nodestream-0.2.0/nodestream/extractors/stores/aws/athena_extractor.py
--rw-r--r--   0        0        0     2498 2023-05-19 21:00:08.060042 nodestream-0.2.0/nodestream/extractors/stores/aws/credential_utils.py
--rw-r--r--   0        0        0     2162 2023-06-05 20:55:40.275409 nodestream-0.2.0/nodestream/extractors/stores/aws/s3_extractor.py
--rw-r--r--   0        0        0      231 2023-05-29 23:36:36.048603 nodestream-0.2.0/nodestream/extractors/streams/__init__.py
--rw-r--r--   0        0        0     2850 2023-06-06 17:09:46.060022 nodestream-0.2.0/nodestream/extractors/streams/extractor.py
--rw-r--r--   0        0        0     1550 2023-06-05 20:55:40.276295 nodestream-0.2.0/nodestream/extractors/streams/kafka.py
--rw-r--r--   0        0        0      617 2023-06-06 14:48:12.783869 nodestream-0.2.0/nodestream/extractors/ttls.py
--rw-r--r--   0        0        0      630 2023-06-06 14:48:12.784290 nodestream-0.2.0/nodestream/interpreting/__init__.py
--rw-r--r--   0        0        0     1367 2023-06-06 14:48:12.784779 nodestream-0.2.0/nodestream/interpreting/extract_variables_interpretation.py
--rw-r--r--   0        0        0      823 2023-06-06 14:48:12.785215 nodestream-0.2.0/nodestream/interpreting/interpretation.py
--rw-r--r--   0        0        0     4603 2023-06-06 14:48:12.785766 nodestream-0.2.0/nodestream/interpreting/interpreter.py
--rw-r--r--   0        0        0     1236 2023-06-06 14:48:12.786283 nodestream-0.2.0/nodestream/interpreting/properties_interpretation.py
--rw-r--r--   0        0        0     1826 2023-06-06 14:48:12.786677 nodestream-0.2.0/nodestream/interpreting/record_decomposers.py
--rw-r--r--   0        0        0     9831 2023-06-08 14:26:36.774221 nodestream-0.2.0/nodestream/interpreting/relationship_interpretation.py
--rw-r--r--   0        0        0     4412 2023-06-06 14:48:12.787449 nodestream-0.2.0/nodestream/interpreting/source_node_interpretation.py
--rw-r--r--   0        0        0     1915 2023-06-06 14:48:12.787601 nodestream-0.2.0/nodestream/interpreting/switch_interpretation.py
--rw-r--r--   0        0        0      486 2023-05-23 15:05:18.012902 nodestream-0.2.0/nodestream/logging.py
--rw-r--r--   0        0        0     1541 2023-06-07 19:09:40.102805 nodestream-0.2.0/nodestream/model/__init__.py
--rw-r--r--   0        0        0     3300 2023-06-06 14:48:12.788476 nodestream-0.2.0/nodestream/model/desired_ingest.py
--rw-r--r--   0        0        0     6242 2023-06-06 14:48:12.788918 nodestream-0.2.0/nodestream/model/graph_objects.py
--rw-r--r--   0        0        0     1337 2023-06-08 14:35:15.964089 nodestream-0.2.0/nodestream/model/indexes.py
--rw-r--r--   0        0        0     2668 2023-06-06 14:48:12.789751 nodestream-0.2.0/nodestream/model/ingest_strategy.py
--rw-r--r--   0        0        0      873 2023-05-18 13:51:44.156142 nodestream-0.2.0/nodestream/model/ingestion_hooks.py
--rw-r--r--   0        0        0     1226 2023-06-06 14:48:12.790109 nodestream-0.2.0/nodestream/model/interpreter_context.py
--rw-r--r--   0        0        0      282 2023-05-19 19:07:54.215627 nodestream-0.2.0/nodestream/model/match_strategy.py
--rw-r--r--   0        0        0    13791 2023-06-07 19:09:40.103762 nodestream-0.2.0/nodestream/model/schema.py
--rw-r--r--   0        0        0      794 2023-06-08 00:32:09.016719 nodestream-0.2.0/nodestream/model/ttl.py
--rw-r--r--   0        0        0      327 2023-05-29 23:36:36.050183 nodestream-0.2.0/nodestream/normalizers/__init__.py
--rw-r--r--   0        0        0      240 2023-05-30 15:58:51.571325 nodestream-0.2.0/nodestream/normalizers/lowercase_strings.py
--rw-r--r--   0        0        0     1482 2023-06-07 22:45:15.385531 nodestream-0.2.0/nodestream/normalizers/normalizer.py
--rw-r--r--   0        0        0      249 2023-05-30 15:58:51.571776 nodestream-0.2.0/nodestream/normalizers/remove_trailing_dots.py
--rw-r--r--   0        0        0      236 2023-05-30 15:58:51.572307 nodestream-0.2.0/nodestream/normalizers/trim_whitespace.py
--rw-r--r--   0        0        0      866 2023-06-06 14:48:12.791862 nodestream-0.2.0/nodestream/pipeline/__init__.py
--rw-r--r--   0        0        0     1641 2023-06-06 14:48:12.792250 nodestream-0.2.0/nodestream/pipeline/class_loader.py
--rw-r--r--   0        0        0     1150 2023-05-24 23:18:33.740527 nodestream-0.2.0/nodestream/pipeline/extractors.py
--rw-r--r--   0        0        0     2774 2023-06-06 14:48:12.792635 nodestream-0.2.0/nodestream/pipeline/filters.py
--rw-r--r--   0        0        0       22 2023-05-19 19:07:54.216776 nodestream-0.2.0/nodestream/pipeline/flush.py
--rw-r--r--   0        0        0      415 2023-05-31 17:06:52.911049 nodestream-0.2.0/nodestream/pipeline/meta.py
--rw-r--r--   0        0        0      985 2023-06-07 19:09:40.104346 nodestream-0.2.0/nodestream/pipeline/pipeline.py
--rw-r--r--   0        0        0     2908 2023-06-07 19:09:40.105095 nodestream-0.2.0/nodestream/pipeline/pipeline_file_loader.py
--rw-r--r--   0        0        0      706 2023-05-25 15:29:43.396280 nodestream-0.2.0/nodestream/pipeline/step.py
--rw-r--r--   0        0        0     1036 2023-06-06 17:12:22.610218 nodestream-0.2.0/nodestream/pipeline/transformers.py
--rw-r--r--   0        0        0     1797 2023-05-24 22:50:05.012870 nodestream-0.2.0/nodestream/pipeline/writers.py
--rw-r--r--   0        0        0      351 2023-05-18 13:51:44.158173 nodestream-0.2.0/nodestream/project/__init__.py
--rw-r--r--   0        0        0     2219 2023-06-07 19:09:40.105974 nodestream-0.2.0/nodestream/project/pipeline_definition.py
--rw-r--r--   0        0        0     1170 2023-05-29 23:36:36.051060 nodestream-0.2.0/nodestream/project/pipeline_progress_reporter.py
--rw-r--r--   0        0        0     2554 2023-06-07 19:09:40.106585 nodestream-0.2.0/nodestream/project/pipeline_scope.py
--rw-r--r--   0        0        0     3754 2023-06-08 14:14:09.012485 nodestream-0.2.0/nodestream/project/project.py
--rw-r--r--   0        0        0      736 2023-05-31 17:06:52.911695 nodestream-0.2.0/nodestream/project/run_request.py
--rw-r--r--   0        0        0     1460 2023-05-30 15:58:51.572815 nodestream-0.2.0/nodestream/subclass_registry.py
--rw-r--r--   0        0        0       78 2023-06-06 17:15:51.421169 nodestream-0.2.0/nodestream/transformers/__init__.py
--rw-r--r--   0        0        0      464 2023-06-06 17:15:30.987309 nodestream-0.2.0/nodestream/transformers/value_projection.py
--rw-r--r--   0        0        0      566 2023-05-29 23:36:36.052195 nodestream-0.2.0/nodestream/utilities.py
--rw-r--r--   0        0        0      734 2023-05-25 02:48:03.113484 nodestream-0.2.0/nodestream/value_providers/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-06 17:09:46.061093 nodestream-0.2.0/nodestream/value_providers/jmespath_value_provider.py
--rw-r--r--   0        0        0     1099 2023-06-06 17:09:46.061833 nodestream-0.2.0/nodestream/value_providers/jq_value_provder.py
--rw-r--r--   0        0        0     1250 2023-06-06 14:48:12.795058 nodestream-0.2.0/nodestream/value_providers/mapping_value_provider.py
--rw-r--r--   0        0        0      591 2023-05-18 13:51:44.159528 nodestream-0.2.0/nodestream/value_providers/static_value_provider.py
--rw-r--r--   0        0        0     1262 2023-06-06 14:48:12.795541 nodestream-0.2.0/nodestream/value_providers/string_format_value_provider.py
--rw-r--r--   0        0        0     2205 2023-06-06 14:48:12.797030 nodestream-0.2.0/nodestream/value_providers/value_provider.py
--rw-r--r--   0        0        0      957 2023-05-18 13:51:44.159795 nodestream-0.2.0/nodestream/value_providers/variable_value_provider.py
--rw-r--r--   0        0        0     1696 2023-06-07 21:56:49.102433 nodestream-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 nodestream-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    32335 2023-05-22 04:06:32.540876 nodestream-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1672 2023-06-17 16:58:48.979346 nodestream-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 04:06:32.541980 nodestream-0.3.0/nodestream/__init__.py
+-rw-r--r--   0        0        0      321 2023-06-05 04:07:36.329575 nodestream-0.3.0/nodestream/argument_resolvers/__init__.py
+-rw-r--r--   0        0        0      440 2023-05-22 04:06:32.542297 nodestream-0.3.0/nodestream/argument_resolvers/argument_resolver.py
+-rw-r--r--   0        0        0      600 2023-06-05 04:07:30.110785 nodestream-0.3.0/nodestream/argument_resolvers/environment_variable_resolver.py
+-rw-r--r--   0        0        0      689 2023-06-05 04:07:34.461207 nodestream-0.3.0/nodestream/argument_resolvers/include_file_resolver.py
+-rw-r--r--   0        0        0      262 2023-06-11 15:56:57.107255 nodestream-0.3.0/nodestream/audits/__init__.py
+-rw-r--r--   0        0        0      695 2023-06-10 15:10:55.577065 nodestream-0.3.0/nodestream/audits/audit.py
+-rw-r--r--   0        0        0      375 2023-06-10 15:10:55.577136 nodestream-0.3.0/nodestream/audits/audit_printer.py
+-rw-r--r--   0        0        0     1636 2023-06-11 15:56:53.190820 nodestream-0.3.0/nodestream/audits/audit_referencial_integrity.py
+-rw-r--r--   0        0        0     1516 2023-06-10 15:10:55.577300 nodestream-0.3.0/nodestream/audits/audit_ttls.py
+-rw-r--r--   0        0        0      109 2023-05-28 20:20:03.239872 nodestream-0.3.0/nodestream/cli/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-11 15:54:17.098818 nodestream-0.3.0/nodestream/cli/application.py
+-rw-r--r--   0        0        0      250 2023-06-02 16:12:56.856126 nodestream-0.3.0/nodestream/cli/commands/__init__.py
+-rw-r--r--   0        0        0      482 2023-06-19 21:38:19.553805 nodestream-0.3.0/nodestream/cli/commands/audit_command.py
+-rw-r--r--   0        0        0      268 2023-06-11 15:56:56.149889 nodestream-0.3.0/nodestream/cli/commands/audit_refs.py
+-rw-r--r--   0        0        0      204 2023-06-10 15:10:55.577842 nodestream-0.3.0/nodestream/cli/commands/audit_ttls.py
+-rw-r--r--   0        0        0     1165 2023-06-13 03:41:18.563183 nodestream-0.3.0/nodestream/cli/commands/new.py
+-rw-r--r--   0        0        0     1113 2023-06-19 18:14:07.674722 nodestream-0.3.0/nodestream/cli/commands/nodestream_command.py
+-rw-r--r--   0        0        0     1213 2023-06-10 15:10:55.578317 nodestream-0.3.0/nodestream/cli/commands/print_schema.py
+-rw-r--r--   0        0        0      893 2023-06-02 16:12:56.856258 nodestream-0.3.0/nodestream/cli/commands/remove.py
+-rw-r--r--   0        0        0     1087 2023-06-05 04:08:16.054031 nodestream-0.3.0/nodestream/cli/commands/run.py
+-rw-r--r--   0        0        0     1426 2023-06-13 03:41:18.563615 nodestream-0.3.0/nodestream/cli/commands/scaffold.py
+-rw-r--r--   0        0        0      508 2023-06-05 04:08:28.791988 nodestream-0.3.0/nodestream/cli/commands/shared_options.py
+-rw-r--r--   0        0        0      596 2023-06-01 19:59:52.365390 nodestream-0.3.0/nodestream/cli/commands/show.py
+-rw-r--r--   0        0        0      986 2023-06-10 15:10:55.578960 nodestream-0.3.0/nodestream/cli/operations/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-01 19:59:52.365897 nodestream-0.3.0/nodestream/cli/operations/add_pipeline_to_project.py
+-rw-r--r--   0        0        0      438 2023-06-01 19:59:52.366064 nodestream-0.3.0/nodestream/cli/operations/commit_project_to_disk.py
+-rw-r--r--   0        0        0     2153 2023-06-17 17:14:36.039704 nodestream-0.3.0/nodestream/cli/operations/generate_pipeline_scaffold.py
+-rw-r--r--   0        0        0     1434 2023-06-01 19:59:52.381733 nodestream-0.3.0/nodestream/cli/operations/generate_project.py
+-rw-r--r--   0        0        0     2317 2023-06-02 16:12:56.856800 nodestream-0.3.0/nodestream/cli/operations/generate_python_scaffold.py
+-rw-r--r--   0        0        0      370 2023-06-01 19:59:52.366792 nodestream-0.3.0/nodestream/cli/operations/initialize_logger.py
+-rw-r--r--   0        0        0      339 2023-06-01 19:59:52.366956 nodestream-0.3.0/nodestream/cli/operations/initialize_project.py
+-rw-r--r--   0        0        0      384 2023-06-01 19:59:52.367202 nodestream-0.3.0/nodestream/cli/operations/operation.py
+-rw-r--r--   0        0        0     1208 2023-06-10 15:10:55.579042 nodestream-0.3.0/nodestream/cli/operations/print_project_schema.py
+-rw-r--r--   0        0        0      533 2023-06-02 16:12:56.856946 nodestream-0.3.0/nodestream/cli/operations/remove_pipeline_from_project.py
+-rw-r--r--   0        0        0     1137 2023-06-10 15:10:55.579120 nodestream-0.3.0/nodestream/cli/operations/run_audit.py
+-rw-r--r--   0        0        0     2625 2023-06-13 03:41:18.564086 nodestream-0.3.0/nodestream/cli/operations/run_pipeline.py
+-rw-r--r--   0        0        0     2371 2023-06-22 03:09:31.663197 nodestream-0.3.0/nodestream/cli/operations/show_pipelines.py
+-rw-r--r--   0        0        0      329 2023-06-10 15:10:55.579239 nodestream-0.3.0/nodestream/cli/schema_printers/__init__.py
+-rw-r--r--   0        0        0     5717 2023-06-10 15:10:55.579350 nodestream-0.3.0/nodestream/cli/schema_printers/graphql_schema_printer.py
+-rw-r--r--   0        0        0      272 2023-06-10 15:10:55.579431 nodestream-0.3.0/nodestream/cli/schema_printers/plain_text_schema_printer.py
+-rw-r--r--   0        0        0      634 2023-06-10 15:10:55.579508 nodestream-0.3.0/nodestream/cli/schema_printers/schema_printer.py
+-rw-r--r--   0        0        0      165 2023-05-22 04:06:32.543356 nodestream-0.3.0/nodestream/databases/__init__.py
+-rw-r--r--   0        0        0     3339 2023-06-11 15:51:19.905898 nodestream-0.3.0/nodestream/databases/debounced_ingest_strategy.py
+-rw-r--r--   0        0        0      166 2023-05-23 04:23:50.766140 nodestream-0.3.0/nodestream/databases/neo4j/__init__.py
+-rw-r--r--   0        0        0     2673 2023-06-10 15:10:55.579922 nodestream-0.3.0/nodestream/databases/neo4j/index_query_builder.py
+-rw-r--r--   0        0        0     8831 2023-06-10 21:41:52.186175 nodestream-0.3.0/nodestream/databases/neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0     1060 2023-06-17 16:58:48.979473 nodestream-0.3.0/nodestream/databases/neo4j/query.py
+-rw-r--r--   0        0        0     3984 2023-06-17 16:58:36.163854 nodestream-0.3.0/nodestream/databases/neo4j/query_executor.py
+-rw-r--r--   0        0        0     3344 2023-06-10 17:16:27.625768 nodestream-0.3.0/nodestream/databases/operation_debouncer.py
+-rw-r--r--   0        0        0     2025 2023-06-17 16:58:36.164083 nodestream-0.3.0/nodestream/databases/query_executor.py
+-rw-r--r--   0        0        0     2045 2023-06-13 03:41:18.564442 nodestream-0.3.0/nodestream/databases/query_executor_with_statistics.py
+-rw-r--r--   0        0        0     1897 2023-06-17 16:58:36.164195 nodestream-0.3.0/nodestream/databases/writer.py
+-rw-r--r--   0        0        0     2306 2023-06-19 18:14:07.675098 nodestream-0.3.0/nodestream/exceptions.py
+-rw-r--r--   0        0        0       63 2023-05-28 00:24:04.287321 nodestream-0.3.0/nodestream/extractors/__init__.py
+-rw-r--r--   0        0        0     2634 2023-06-19 18:14:07.675283 nodestream-0.3.0/nodestream/extractors/files.py
+-rw-r--r--   0        0        0        0 2023-05-22 04:06:32.545035 nodestream-0.3.0/nodestream/extractors/stores/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-04 04:53:47.025779 nodestream-0.3.0/nodestream/extractors/stores/aws/__init__.py
+-rw-r--r--   0        0        0     4562 2023-06-17 16:58:36.164918 nodestream-0.3.0/nodestream/extractors/stores/aws/athena_extractor.py
+-rw-r--r--   0        0        0     2498 2023-05-22 04:06:32.545334 nodestream-0.3.0/nodestream/extractors/stores/aws/credential_utils.py
+-rw-r--r--   0        0        0     2156 2023-06-17 16:58:36.165044 nodestream-0.3.0/nodestream/extractors/stores/aws/s3_extractor.py
+-rw-r--r--   0        0        0      231 2023-05-29 05:03:16.758913 nodestream-0.3.0/nodestream/extractors/streams/__init__.py
+-rw-r--r--   0        0        0     2844 2023-06-17 16:58:36.165170 nodestream-0.3.0/nodestream/extractors/streams/extractor.py
+-rw-r--r--   0        0        0     1550 2023-06-04 04:53:47.026562 nodestream-0.3.0/nodestream/extractors/streams/kafka.py
+-rw-r--r--   0        0        0      617 2023-06-05 04:26:56.099448 nodestream-0.3.0/nodestream/extractors/ttls.py
+-rw-r--r--   0        0        0     3566 2023-06-19 18:14:07.675391 nodestream-0.3.0/nodestream/file_io.py
+-rw-r--r--   0        0        0      630 2023-06-05 04:15:51.478247 nodestream-0.3.0/nodestream/interpreting/__init__.py
+-rw-r--r--   0        0        0     1367 2023-06-05 04:12:39.289126 nodestream-0.3.0/nodestream/interpreting/extract_variables_interpretation.py
+-rw-r--r--   0        0        0      818 2023-06-17 16:58:36.165290 nodestream-0.3.0/nodestream/interpreting/interpretation.py
+-rw-r--r--   0        0        0     4637 2023-06-17 16:58:36.165600 nodestream-0.3.0/nodestream/interpreting/interpreter.py
+-rw-r--r--   0        0        0     1236 2023-06-05 04:12:46.763210 nodestream-0.3.0/nodestream/interpreting/properties_interpretation.py
+-rw-r--r--   0        0        0     1826 2023-06-05 04:13:52.143015 nodestream-0.3.0/nodestream/interpreting/record_decomposers.py
+-rw-r--r--   0        0        0     9831 2023-06-10 15:10:55.580731 nodestream-0.3.0/nodestream/interpreting/relationship_interpretation.py
+-rw-r--r--   0        0        0     4412 2023-06-05 04:14:35.045060 nodestream-0.3.0/nodestream/interpreting/source_node_interpretation.py
+-rw-r--r--   0        0        0     1907 2023-06-17 16:58:36.165814 nodestream-0.3.0/nodestream/interpreting/switch_interpretation.py
+-rw-r--r--   0        0        0      486 2023-06-02 21:26:12.184888 nodestream-0.3.0/nodestream/logging.py
+-rw-r--r--   0        0        0     1567 2023-06-17 16:58:36.165926 nodestream-0.3.0/nodestream/model/__init__.py
+-rw-r--r--   0        0        0     3300 2023-06-05 04:16:08.070242 nodestream-0.3.0/nodestream/model/desired_ingest.py
+-rw-r--r--   0        0        0     6930 2023-06-19 21:22:18.492834 nodestream-0.3.0/nodestream/model/graph_objects.py
+-rw-r--r--   0        0        0     1337 2023-06-05 04:16:34.826137 nodestream-0.3.0/nodestream/model/indexes.py
+-rw-r--r--   0        0        0     2668 2023-06-05 04:16:51.308128 nodestream-0.3.0/nodestream/model/ingest_strategy.py
+-rw-r--r--   0        0        0      873 2023-05-22 04:06:32.547741 nodestream-0.3.0/nodestream/model/ingestion_hooks.py
+-rw-r--r--   0        0        0     1226 2023-06-05 04:17:02.553214 nodestream-0.3.0/nodestream/model/interpreter_context.py
+-rw-r--r--   0        0        0      282 2023-05-22 04:06:32.547953 nodestream-0.3.0/nodestream/model/match_strategy.py
+-rw-r--r--   0        0        0    13845 2023-06-17 16:58:36.166062 nodestream-0.3.0/nodestream/model/schema.py
+-rw-r--r--   0        0        0      794 2023-06-10 15:10:55.581297 nodestream-0.3.0/nodestream/model/ttl.py
+-rw-r--r--   0        0        0      327 2023-05-28 20:20:37.526089 nodestream-0.3.0/nodestream/normalizers/__init__.py
+-rw-r--r--   0        0        0      240 2023-05-30 04:13:30.470006 nodestream-0.3.0/nodestream/normalizers/lowercase_strings.py
+-rw-r--r--   0        0        0     1482 2023-06-10 15:10:55.581449 nodestream-0.3.0/nodestream/normalizers/normalizer.py
+-rw-r--r--   0        0        0      249 2023-05-30 04:13:30.470152 nodestream-0.3.0/nodestream/normalizers/remove_trailing_dots.py
+-rw-r--r--   0        0        0      236 2023-05-30 04:13:30.470669 nodestream-0.3.0/nodestream/normalizers/trim_whitespace.py
+-rw-r--r--   0        0        0      875 2023-06-13 04:18:29.734448 nodestream-0.3.0/nodestream/pipeline/__init__.py
+-rw-r--r--   0        0        0     1635 2023-06-17 16:58:36.166185 nodestream-0.3.0/nodestream/pipeline/class_loader.py
+-rw-r--r--   0        0        0     1150 2023-06-13 01:00:29.179849 nodestream-0.3.0/nodestream/pipeline/extractors.py
+-rw-r--r--   0        0        0     3179 2023-06-17 16:58:36.166417 nodestream-0.3.0/nodestream/pipeline/filters.py
+-rw-r--r--   0        0        0       22 2023-05-22 04:06:32.549273 nodestream-0.3.0/nodestream/pipeline/flush.py
+-rw-r--r--   0        0        0      869 2023-06-13 03:41:18.565249 nodestream-0.3.0/nodestream/pipeline/meta.py
+-rw-r--r--   0        0        0     1179 2023-06-17 16:58:36.166723 nodestream-0.3.0/nodestream/pipeline/pipeline.py
+-rw-r--r--   0        0        0     2908 2023-06-10 15:10:55.581708 nodestream-0.3.0/nodestream/pipeline/pipeline_file_loader.py
+-rw-r--r--   0        0        0      742 2023-06-17 16:58:36.167245 nodestream-0.3.0/nodestream/pipeline/step.py
+-rw-r--r--   0        0        0     1036 2023-06-10 23:52:40.650838 nodestream-0.3.0/nodestream/pipeline/transformers.py
+-rw-r--r--   0        0        0     1726 2023-06-11 15:51:19.906645 nodestream-0.3.0/nodestream/pipeline/writers.py
+-rw-r--r--   0        0        0      351 2023-05-22 04:06:32.550015 nodestream-0.3.0/nodestream/project/__init__.py
+-rw-r--r--   0        0        0     2698 2023-06-19 18:14:07.675772 nodestream-0.3.0/nodestream/project/pipeline_definition.py
+-rw-r--r--   0        0        0     1255 2023-06-13 03:41:18.565458 nodestream-0.3.0/nodestream/project/pipeline_progress_reporter.py
+-rw-r--r--   0        0        0     3012 2023-06-19 18:14:07.675899 nodestream-0.3.0/nodestream/project/pipeline_scope.py
+-rw-r--r--   0        0        0     3782 2023-06-19 18:14:07.676081 nodestream-0.3.0/nodestream/project/project.py
+-rw-r--r--   0        0        0      755 2023-06-13 03:41:18.565650 nodestream-0.3.0/nodestream/project/run_request.py
+-rw-r--r--   0        0        0     1460 2023-05-30 04:13:30.470870 nodestream-0.3.0/nodestream/subclass_registry.py
+-rw-r--r--   0        0        0       78 2023-06-10 15:10:55.582898 nodestream-0.3.0/nodestream/transformers/__init__.py
+-rw-r--r--   0        0        0      464 2023-06-10 15:10:55.582964 nodestream-0.3.0/nodestream/transformers/value_projection.py
+-rw-r--r--   0        0        0      566 2023-06-17 17:14:32.469493 nodestream-0.3.0/nodestream/utilities.py
+-rw-r--r--   0        0        0      734 2023-05-22 04:06:32.550995 nodestream-0.3.0/nodestream/value_providers/__init__.py
+-rw-r--r--   0        0        0     1766 2023-06-10 17:16:27.626270 nodestream-0.3.0/nodestream/value_providers/jmespath_value_provider.py
+-rw-r--r--   0        0        0     1132 2023-06-22 03:04:33.322336 nodestream-0.3.0/nodestream/value_providers/jq_value_provder.py
+-rw-r--r--   0        0        0     1291 2023-06-10 17:16:27.626552 nodestream-0.3.0/nodestream/value_providers/mapping_value_provider.py
+-rw-r--r--   0        0        0      619 2023-06-10 17:16:27.626689 nodestream-0.3.0/nodestream/value_providers/static_value_provider.py
+-rw-r--r--   0        0        0     1295 2023-06-22 03:09:31.663589 nodestream-0.3.0/nodestream/value_providers/string_format_value_provider.py
+-rw-r--r--   0        0        0     2205 2023-06-22 03:09:31.663749 nodestream-0.3.0/nodestream/value_providers/value_provider.py
+-rw-r--r--   0        0        0      971 2023-06-10 17:16:27.626936 nodestream-0.3.0/nodestream/value_providers/variable_value_provider.py
+-rw-r--r--   0        0        0     1976 2023-06-22 04:08:48.417569 nodestream-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 nodestream-0.3.0/PKG-INFO
```

### Comparing `nodestream-0.2.0/LICENSE` & `nodestream-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/README.md` & `nodestream-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
 [![PyPI version](https://badge.fury.io/py/nodestream.svg)](https://badge.fury.io/py/nodestream)
 
 ## Features
 
 - Flexible and extensible YAML based DSL for ETL jobs
 - Connect to data sources like Kafka, AWS Athena, flat files, and more.
-- Developer friendly features such as snapshot testing
+- Developer friendly
 - Highly optimized with async and tuned query generation
 
 
 ## Getting Started
 
 Install nodestream with `pip`
 
@@ -47,8 +47,9 @@
 
 ## Authors
 
 - Zach Probst ([@zprobst](https://www.github.com/zprobst))
 - Chad Cloes ([@ccloes](https://www.github.com/ccloes))
 - Oshri Rozenberg([@orozen](https://www.github.com/orozen))
 - Kevin Neal ([@khneal](https://www.github.com/khneal))
+- Grant Hoffman ([@grantleehoffman](https://www.github.com/grantleehoffman))
```

### Comparing `nodestream-0.2.0/nodestream/argument_resolvers/environment_variable_resolver.py` & `nodestream-0.3.0/nodestream/argument_resolvers/environment_variable_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/argument_resolvers/include_file_resolver.py` & `nodestream-0.3.0/nodestream/argument_resolvers/include_file_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/audits/audit.py` & `nodestream-0.3.0/nodestream/audits/audit.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/audits/audit_referencial_integrity.py` & `nodestream-0.3.0/nodestream/audits/audit_referencial_integrity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..interpreting import Interpreter
-from ..project import Project
 from ..model import KeyIndex
+from ..project import Project
 from .audit import Audit
 
 
-class AuditReferencialIntegrity(Audit):
+class AuditReferentialIntegrity(Audit):
     async def run(self, project: Project):
         all_interpreters = project.dig_for_step_of_type(Interpreter)
         node_types_so_far = {}
 
         for definition, step_index, interpreter in all_interpreters:
             for index in interpreter.gather_used_indexes():
                 if not isinstance(index, KeyIndex):
@@ -19,14 +19,14 @@
                     existing_index, existing_definition, existing_step_index = existing
                     if index != existing_index:
                         current_index_fields = ", ".join(index.identity_keys)
                         existing_index_fields = ", ".join(existing_index.identity_keys)
                         self.failure(
                             f"Regarding the type '{index.type}':\n"
                             f"\tthe Interpreter in '{definition.file_path}' step '{step_index}' wants to use an index on the fields '{current_index_fields}' WHILE\n"
-                            f"\tthe interpreter in '{existing_definition.file_path}' step '{existing_step_index}' wants to use an index on the fields '{existing_index_fields}'"
+                            f"\tthe Interpreter in '{existing_definition.file_path}' step '{existing_step_index}' wants to use an index on the fields '{existing_index_fields}'"
                         )
                 else:
                     node_types_so_far[index.type] = (index, definition, step_index)
 
         if self.failure_count == 0:
-            self.success("All Object Types Have Consistent Referencial Integrty")
+            self.success("All Object Types Have Consistent Referential Integrity")
```

### Comparing `nodestream-0.2.0/nodestream/audits/audit_ttls.py` & `nodestream-0.3.0/nodestream/audits/audit_ttls.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/application.py` & `nodestream-0.3.0/nodestream/cli/application.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import importlib.metadata
 import os
 import sys
 
 from cleo.application import Application
 
-from .commands.audit_ttls import AuditTTLs
 from .commands.audit_refs import AuditRefs
+from .commands.audit_ttls import AuditTTLs
 from .commands.new import New
 from .commands.print_schema import PrintSchema
 from .commands.remove import Remove
 from .commands.run import Run
 from .commands.scaffold import Scaffold
 from .commands.show import Show
 
-APPLICATION = Application(name="nodestream")
+APPLICATION = Application(
+    name="nodestream", version=importlib.metadata.version("nodestream")
+)
 APPLICATION.add(Run())
 APPLICATION.add(New())
 APPLICATION.add(Show())
 APPLICATION.add(Scaffold())
 APPLICATION.add(Remove())
 APPLICATION.add(PrintSchema())
 APPLICATION.add(AuditTTLs())
```

### Comparing `nodestream-0.2.0/nodestream/cli/commands/new.py` & `nodestream-0.3.0/nodestream/cli/commands/new.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,8 @@
         db = self.option("database")
         python_files = await self.run_operation(GeneratePythonScaffold(project_root))
         pipelines = await self.run_operation(GeneratePipelineScaffold(project_root, db))
         gen_project = GenerateProject(project_root, pipelines, python_files, db)
         project = await self.run_operation(gen_project)
         commit_to_disk = CommitProjectToDisk(project, project_root / "nodestream.yaml")
         await self.run_operation(commit_to_disk)
+        self.line(f"<info>Created new project at '{project_root}'</info>")
```

### Comparing `nodestream-0.2.0/nodestream/cli/commands/nodestream_command.py` & `nodestream-0.3.0/nodestream/cli/commands/nodestream_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return await operation.perform(self)
 
     def get_project_path(self) -> Path:
         path = self.option("project")
         return DEFAULT_PROJECT_FILE if path is None else Path(path)
 
     def get_project(self) -> Project:
-        return Project.from_file(self.get_project_path())
+        return Project.read_from_file(self.get_project_path())
 
     @property
     def has_json_logging_set(self) -> bool:
         return self.option("json")
 
     @property
     def scope(self) -> str:
```

### Comparing `nodestream-0.2.0/nodestream/cli/commands/print_schema.py` & `nodestream-0.3.0/nodestream/cli/commands/print_schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/commands/remove.py` & `nodestream-0.3.0/nodestream/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/commands/run.py` & `nodestream-0.3.0/nodestream/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/commands/scaffold.py` & `nodestream-0.3.0/nodestream/cli/commands/scaffold.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,12 +28,13 @@
             GeneratePipelineScaffold(
                 project_root=self.get_project_path().parent,
                 database_name=database_name,
                 pipeline_file_name=pipeline_name + ".yaml",
             )
         )
         for generated_pipeline in generated_pipelines:
+            self.line(f"<info>Generated pipeline at '{generated_pipeline}'</info>")
             await self.run_operation(
                 AddPipelineToProject(project, generated_pipeline, desired_scope)
             )
 
         await self.run_operation(CommitProjectToDisk(project, self.get_project_path()))
```

### Comparing `nodestream-0.2.0/nodestream/cli/commands/show.py` & `nodestream-0.3.0/nodestream/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/__init__.py` & `nodestream-0.3.0/nodestream/cli/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/add_pipeline_to_project.py` & `nodestream-0.3.0/nodestream/cli/operations/add_pipeline_to_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/generate_pipeline_scaffold.py` & `nodestream-0.3.0/nodestream/cli/operations/generate_pipeline_scaffold.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/generate_project.py` & `nodestream-0.3.0/nodestream/cli/operations/generate_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/generate_python_scaffold.py` & `nodestream-0.3.0/nodestream/cli/operations/generate_python_scaffold.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/print_project_schema.py` & `nodestream-0.3.0/nodestream/cli/operations/print_project_schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/remove_pipeline_from_project.py` & `nodestream-0.3.0/nodestream/cli/operations/remove_pipeline_from_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/run_audit.py` & `nodestream-0.3.0/nodestream/cli/operations/run_audit.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/operations/run_pipeline.py` & `nodestream-0.3.0/nodestream/cli/operations/run_pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from ...pipeline import PipelineInitializationArguments
+from ...pipeline.meta import PipelineContext
 from ...project import PipelineProgressReporter, Project, RunRequest
 from ..commands.nodestream_command import NodestreamCommand
 from .operation import Operation
 
+STATS_TABLE_COLS = ["Statistic", "Value"]
+
 
 class RunPipeline(Operation):
     def __init__(self, project: Project) -> None:
         self.project = project
 
     async def perform(self, command: NodestreamCommand):
         await self.project.run(self.make_run_request(command))
@@ -44,15 +47,15 @@
 
     def on_start(self):
         pass
 
     def progress_callback(self, _, __):
         pass
 
-    def on_finish(self):
+    def on_finish(self, context: PipelineContext):
         pass
 
     @property
     def pipeline_name(self) -> str:
         return self.command.argument("pipeline")
 
 
@@ -62,9 +65,13 @@
         self.progress.start(f"Running pipeline: '{self.pipeline_name}'")
 
     def progress_callback(self, index, _):
         self.progress.set_message(
             f"Currently processing record at index: <info>{index}</info>"
         )
 
-    def on_finish(self):
+    def on_finish(self, context: PipelineContext):
         self.progress.finish(f"Finished running pipeline: '{self.pipeline_name}'")
+
+        stats = ((k, str(v)) for k, v in context.stats.items())
+        table = self.command.table(STATS_TABLE_COLS, stats)
+        table.render()
```

### Comparing `nodestream-0.2.0/nodestream/cli/operations/show_pipelines.py` & `nodestream-0.3.0/nodestream/cli/operations/show_pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     def output(self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]):
         table = self.command.table(self.HEADERS, self.get_data_rows(matching_pipelines))
         table.render()
 
 
 class JsonOutputFormat(OutputFormat):
     def output(self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]):
-        json_data = [
-            pipeline.as_file_definition() for _, pipeline in matching_pipelines
-        ]
+        json_data = [pipeline.to_file_data() for _, pipeline in matching_pipelines]
         self.command.write(json.dumps(json_data))
 
 
 class ShowPipelines(Operation):
     def __init__(
         self, project: Project, scope_name: Optional[str], use_json: bool = False
     ) -> None:
```

### Comparing `nodestream-0.2.0/nodestream/cli/schema_printers/graphql_schema_printer.py` & `nodestream-0.3.0/nodestream/cli/schema_printers/graphql_schema_printer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/cli/schema_printers/schema_printer.py` & `nodestream-0.3.0/nodestream/cli/schema_printers/schema_printer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/databases/debounced_ingest_strategy.py` & `nodestream-0.3.0/nodestream/databases/debounced_ingest_strategy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from dataclasses import asdict
 from logging import getLogger
 
 from ..model import (
     FieldIndex,
     IngestionHookRunRequest,
     IngestionStrategy,
@@ -53,22 +54,34 @@
         self.logger.info("Ensured Index Created", extra=asdict(index))
 
     async def perform_ttl_operation(self, config: TimeToLiveConfiguration):
         self.logger.debug("Executing TTL", extra=asdict(config))
         await self.executor.perform_ttl_op(config)
         self.logger.info("Executed TTL", extra=asdict(config))
 
-    async def flush(self):
-        for operation, node_group in self.debouncer.drain_node_groups():
-            self.logger.debug("Debounced Nodes", extra=asdict(operation.node_identity))
-            await self.executor.upsert_nodes_in_bulk_with_same_operation(
+    def flush_nodes_updates(self):
+        update_coroutines = (
+            self.executor.upsert_nodes_in_bulk_with_same_operation(
                 operation, node_group
             )
+            for operation, node_group in self.debouncer.drain_node_groups()
+        )
+        return asyncio.gather(*update_coroutines)
 
-        for rel_shape, rel_group in self.debouncer.drain_relationship_groups():
-            self.logger.debug("Draining Debounced Nodes", extra=asdict(rel_shape))
-            await self.executor.upsert_relationships_in_bulk_of_same_operation(
+    def flush_relationship_updates(self):
+        update_coroutines = (
+            self.executor.upsert_relationships_in_bulk_of_same_operation(
                 rel_shape, rel_group
             )
+            for rel_shape, rel_group in self.debouncer.drain_relationship_groups()
+        )
+        return asyncio.gather(*update_coroutines)
+
+    async def flush(self):
+        await self.flush_nodes_updates()
+        await self.flush_relationship_updates()
 
+        # Because we don't know what exactly the hooks do, we can't reliably parallelize
+        # them because we could overwhelm the database so we are going to do them one at
+        # a time.
         for hook in self.hooks_saved_for_after_ingest:
             await self.executor.execute_hook(hook)
```

### Comparing `nodestream-0.2.0/nodestream/databases/neo4j/index_query_builder.py` & `nodestream-0.3.0/nodestream/databases/neo4j/index_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/databases/neo4j/ingest_query_builder.py` & `nodestream-0.3.0/nodestream/databases/neo4j/ingest_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/databases/neo4j/query.py` & `nodestream-0.3.0/nodestream/databases/neo4j/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 COMMIT_QUERY = """
 CALL apoc.periodic.iterate(
     "UNWIND $batched_parameter_sets as params RETURN params",
     $batched_query,
-    {batchsize: 1000, paralell: false, retries: 3, params: {batched_parameter_sets: $batched_parameter_sets}}
+    {batchsize: 1000, parallel: false, retries: 3, params: {batched_parameter_sets: $batched_parameter_sets}}
 )
 YIELD batches, committedOperations, failedOperations, errorMessages
 RETURN batches, committedOperations, failedOperations, errorMessages
 """
 
 
-@dataclass(slots=True)
+@dataclass(slots=True, frozen=True)
 class Query:
     query_statement: str
     parameters: Dict[str, Any]
 
     @classmethod
     def from_statement(cls, statement: str):
         return cls(query_statement=statement, parameters={})
 
 
-@dataclass(slots=True)
+@dataclass(slots=True, frozen=True)
 class QueryBatch:
     query_statement: str
     batched_parameter_sets: List[Dict[str, Any]]
 
     def as_query(self) -> Query:
         return Query(
             COMMIT_QUERY,
```

### Comparing `nodestream-0.2.0/nodestream/databases/neo4j/query_executor.py` & `nodestream-0.3.0/nodestream/databases/neo4j/query_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 )
 from .ingest_query_builder import Neo4jIngestQueryBuilder
 from .query import Query
 
 
 class Neo4jQueryExecutor(QueryExecutor, alias="neo4j"):
     @classmethod
-    def from_file_arguments(
+    def from_file_data(
         cls,
         uri: str,
         username: str,
         password: str,
         database_name: str = "neo4j",
         use_enterprise_features: bool = False,
     ):
@@ -103,15 +103,17 @@
             extra={
                 "query": query.query_statement,
                 "uri": self.driver._pool.address.host,
             },
         )
         await self.driver.verify_connectivity()
         result = await self.driver.execute_query(
-            query.query_statement, query.parameters
+            query.query_statement,
+            query.parameters,
+            database_=self.database_name,
         )
         if log_result:
             for record in result.records:
                 self.logger.info(
                     "Gathered Query Results",
                     extra=dict(**record, query=query.query_statement),
                 )
```

### Comparing `nodestream-0.2.0/nodestream/databases/query_executor.py` & `nodestream-0.3.0/nodestream/databases/query_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,22 +31,21 @@
     relationship_identity: RelationshipIdentityShape
 
 
 @QUERY_EXECUTOR_SUBCLASS_REGISTRY.connect_baseclass
 class QueryExecutor(ABC):
     @classmethod
     def from_database_args(cls, database: str = "neo4j", **database_args):
-        return QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database).from_file_arguments(
+        return QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database).from_file_data(
             **database_args
         )
 
     @classmethod
-    @abstractmethod
-    def from_file_arguments(cls, **kwargs):
-        raise NotImplementedError
+    def from_file_data(cls, **kwargs):
+        return cls(**kwargs)
 
     @abstractmethod
     async def upsert_nodes_in_bulk_with_same_operation(
         self, operation: OperationOnNodeIdentity, nodes: Iterable[Node]
     ):
         raise NotImplementedError
```

### Comparing `nodestream-0.2.0/nodestream/databases/writer.py` & `nodestream-0.3.0/nodestream/databases/writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from typing import Optional
 
 from ..model.ingest_strategy import INGESTION_STRATEGY_REGISTRY, IngestionStrategy
 from ..pipeline import Flush, Writer
 from .debounced_ingest_strategy import DebouncedIngestStrategy
 from .query_executor import QUERY_EXECUTOR_SUBCLASS_REGISTRY
+from .query_executor_with_statistics import QueryExecutorWithStatistics
 
 
 class GraphDatabaseWriter(Writer):
     @classmethod
-    def __declarative_init__(
+    def from_file_data(
         cls,
         batch_size: int,
         database: str,
         ingest_strategy_name: Optional[str] = None,
+        collect_stats: bool = True,
         **database_args
     ):
+        executor_class = QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database)
+        executor = executor_class.from_file_data(**database_args)
+        if collect_stats:
+            executor = QueryExecutorWithStatistics(executor)
+
         ingest_strategy_name = (
             ingest_strategy_name
             or INGESTION_STRATEGY_REGISTRY.name_for(DebouncedIngestStrategy)
         )
-        ingest_strategy = INGESTION_STRATEGY_REGISTRY.get(ingest_strategy_name)
-        executor_class = QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database)
-        executor = executor_class.from_file_arguments(**database_args)
+        ingest_strategy_cls = INGESTION_STRATEGY_REGISTRY.get(ingest_strategy_name)
+        ingest_strategy = ingest_strategy_cls(executor)
+
         return cls(
             batch_size=batch_size,
-            ingest_strategy=ingest_strategy(executor),
+            ingest_strategy=ingest_strategy,
         )
 
     def __init__(self, batch_size: int, ingest_strategy: IngestionStrategy) -> None:
         self.batch_size = batch_size
         self.ingest_strategy = ingest_strategy
         self.pending_records = 0
```

### Comparing `nodestream-0.2.0/nodestream/exceptions.py` & `nodestream-0.3.0/nodestream/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from pathlib import Path
-
-
 class InvalidClassPathError(ValueError):
     """Raised when a class path is invalid."""
 
     pass
 
 
 class InvalidPipelineDefinitionError(ValueError):
@@ -68,16 +65,9 @@
 
     def __init__(self, missing_branch_value, *args: object) -> None:
         super().__init__(
             f"'{missing_branch_value}' was not matched in switch case", *args
         )
 
 
-class MissingProjectFileError(ValueError):
-    """Raised when a project file is missing."""
-
-    def __init__(self, file: Path, *args: object) -> None:
-        super().__init__(f"'{file}' does not exist", *args)
-
-
 class MissingExpectedPipelineError(ValueError):
     pass
```

### Comparing `nodestream-0.2.0/nodestream/extractors/files.py` & `nodestream-0.3.0/nodestream/extractors/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class SupportedFileFormat(ABC):
     def __init__(self, file: Union[Path, StringIO]) -> None:
         self.file = file
 
     @contextmanager
     def read_handle(self) -> StringIO:
         if isinstance(self.file, Path):
-            with open(self.file, "r+") as fp:
+            with open(self.file, "r") as fp:
                 yield fp
         else:
             yield self.file
 
     def read_file(self) -> Iterable[JsonLikeDocument]:
         with self.read_handle() as fp:
             return self.read_file_from_handle(fp)
@@ -60,15 +60,15 @@
 class CommaSeperatedValuesFileFormat(SupportedFileFormat, alias=".csv"):
     def read_file_from_handle(self, fp: StringIO) -> Iterable[JsonLikeDocument]:
         return tuple(DictReader(fp))
 
 
 class FileExtractor(Extractor):
     @classmethod
-    def __declarative_init__(cls, globs: Iterable[str]):
+    def from_file_data(cls, globs: Iterable[str]):
         all_matching_paths = (
             Path(file)
             for glob_string in globs
             for file in glob(glob_string, recursive=True)
         )
         final_paths = {p for p in all_matching_paths if p.is_file()}
         return cls(final_paths)
```

### Comparing `nodestream-0.2.0/nodestream/extractors/stores/aws/athena_extractor.py` & `nodestream-0.3.0/nodestream/extractors/stores/aws/athena_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         if raw_value is None:
             return None
         return CONVERTERS[column_metadata["Type"]](raw_value)
 
 
 class AthenaExtractor(Extractor):
     @classmethod
-    def __declarative_init__(
+    def from_file_data(
         cls,
         query: str,
         database: str,
         workgroup: str,
         output_location: str,
         poll_interval_seconds: int = 1,
         page_size: int = 500,
```

### Comparing `nodestream-0.2.0/nodestream/extractors/stores/aws/credential_utils.py` & `nodestream-0.3.0/nodestream/extractors/stores/aws/credential_utils.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/extractors/stores/aws/s3_extractor.py` & `nodestream-0.3.0/nodestream/extractors/stores/aws/s3_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ....pipeline import Extractor
 from ...files import SupportedFileFormat
 from .credential_utils import AwsClientFactory
 
 
 class S3Extractor(Extractor):
     @classmethod
-    def __declarative_init__(
+    def from_file_data(
         cls,
         bucket: str,
         prefix: Optional[str] = None,
         object_format: Optional[str] = None,
         **aws_client_args,
     ):
         return cls(
```

### Comparing `nodestream-0.2.0/nodestream/extractors/streams/extractor.py` & `nodestream-0.3.0/nodestream/extractors/streams/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """A StreamExtractor implements the standard behavior of polling data from a stream.
 
     The StreamExtractor requires both a StreamConnector and a StreamRecordFormat to delegate
     to for the actual polling implementation and parsing of the data, respectively.
     """
 
     @classmethod
-    def __declarative_init__(
+    def from_file_data(
         cls,
         connector: str,
         record_format: str,
         timeout: int = DEFAULT_TIMEOUT,
         max_records: int = DEFAULT_MAX_RECORDS,
         **connector_args
     ):
```

### Comparing `nodestream-0.2.0/nodestream/extractors/streams/kafka.py` & `nodestream-0.3.0/nodestream/extractors/streams/kafka.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/extractors/ttls.py` & `nodestream-0.3.0/nodestream/extractors/ttls.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/__init__.py` & `nodestream-0.3.0/nodestream/interpreting/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/extract_variables_interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/extract_variables_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/interpretation.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @INTERPRETATION_REGISTRY.connect_baseclass
 class Interpretation(IntrospectiveIngestionComponent, ABC):
     @abstractmethod
     def interpret(self, context: InterpreterContext):
         raise NotImplementedError
 
     @classmethod
-    def from_file_arguments(cls, **arguments) -> "Interpretation":
+    def from_file_data(cls, **arguments) -> "Interpretation":
         name = arguments.pop("type")
         class_to_load = INTERPRETATION_REGISTRY.get(name)
         return class_to_load(**arguments)
 
     def gather_used_indexes(self):
         yield from []
```

### Comparing `nodestream-0.2.0/nodestream/interpreting/interpreter.py` & `nodestream-0.3.0/nodestream/interpreting/interpreter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Iterable
 
 from ..model import (
-    AggregatedIntrospectionMixin,
+    AggregatedIntrospectiveIngestionComponent,
     InterpreterContext,
     IntrospectiveIngestionComponent,
 )
 from ..pipeline import Flush, Step
 from .interpretation import Interpretation
 from .record_decomposers import RecordDecomposer
 
 
 class InterpretationPass(IntrospectiveIngestionComponent, ABC):
     @classmethod
-    def from_file_arguments(self, args):
+    def from_file_data(self, args):
         if args is None:
             return NullInterpretationPass()
 
         if len(args) > 0 and isinstance(args[0], list):
-            return MultiSequenceInterpretationPass.from_file_arguments(args)
+            return MultiSequenceInterpretationPass.from_file_data(args)
 
-        return SingleSequenceInterpretationPass.from_file_arguments(args)
+        return SingleSequenceInterpretationPass.from_file_data(args)
 
     @abstractmethod
     def apply_interpretations(self, context: InterpreterContext):
         pass
 
 
-class NullInterpretationPass(AggregatedIntrospectionMixin, InterpretationPass):
+class NullInterpretationPass(
+    AggregatedIntrospectiveIngestionComponent, InterpretationPass
+):
     def apply_interpretations(self, context: InterpreterContext):
         yield context
 
     def all_subordinate_components(
         self,
     ) -> Iterable[IntrospectiveIngestionComponent]:
         return []
 
 
-class MultiSequenceInterpretationPass(AggregatedIntrospectionMixin, InterpretationPass):
+class MultiSequenceInterpretationPass(
+    AggregatedIntrospectiveIngestionComponent, InterpretationPass
+):
+    __slots__ = ("passes",)
+
     @classmethod
-    def from_file_arguments(cls, args):
-        return cls(*(InterpretationPass.from_file_arguments(arg) for arg in args))
+    def from_file_data(cls, args):
+        return cls(*(InterpretationPass.from_file_data(arg) for arg in args))
 
     def __init__(self, *passes: InterpretationPass) -> None:
         self.passes = passes
 
     def apply_interpretations(self, context: InterpreterContext):
         for interpretation_pass in self.passes:
             provided_subcontext = deepcopy(context)
@@ -53,21 +59,22 @@
                 yield res
 
     def all_subordinate_components(self) -> Iterable[IntrospectiveIngestionComponent]:
         yield from self.passes
 
 
 class SingleSequenceInterpretationPass(
-    AggregatedIntrospectionMixin, InterpretationPass
+    AggregatedIntrospectiveIngestionComponent, InterpretationPass
 ):
+    __slots__ = ("interpretations",)
+
     @classmethod
-    def from_file_arguments(cls, interpretation_arg_list):
+    def from_file_data(cls, interpretation_arg_list):
         interpretations = (
-            Interpretation.from_file_arguments(**args)
-            for args in interpretation_arg_list
+            Interpretation.from_file_data(**args) for args in interpretation_arg_list
         )
         return cls(*interpretations)
 
     def __init__(self, *interpretations: Interpretation):
         self.interpretations = interpretations
 
     def apply_interpretations(self, context: InterpreterContext):
@@ -75,28 +82,26 @@
             interpretation.interpret(context)
         yield context
 
     def all_subordinate_components(self) -> Iterable[IntrospectiveIngestionComponent]:
         yield from self.interpretations
 
 
-class Interpreter(Step, AggregatedIntrospectionMixin, IntrospectiveIngestionComponent):
+class Interpreter(Step, AggregatedIntrospectiveIngestionComponent):
     __slots__ = (
         "before_iteration",
         "interpretations",
         "decomposer",
     )
 
     @classmethod
-    def __declarative_init__(
-        cls, interpretations, before_iteration=None, iterate_on=None
-    ):
+    def from_file_data(cls, interpretations, before_iteration=None, iterate_on=None):
         return cls(
-            before_iteration=InterpretationPass.from_file_arguments(before_iteration),
-            interpretations=InterpretationPass.from_file_arguments(interpretations),
+            before_iteration=InterpretationPass.from_file_data(before_iteration),
+            interpretations=InterpretationPass.from_file_data(interpretations),
             decomposer=RecordDecomposer.from_iteration_arguments(iterate_on),
         )
 
     def __init__(
         self,
         before_iteration: InterpretationPass,
         interpretations: InterpretationPass,
```

### Comparing `nodestream-0.2.0/nodestream/interpreting/properties_interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/properties_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/record_decomposers.py` & `nodestream-0.3.0/nodestream/interpreting/record_decomposers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/relationship_interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/relationship_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/source_node_interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/source_node_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/interpreting/switch_interpretation.py` & `nodestream-0.3.0/nodestream/interpreting/switch_interpretation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any, Dict
 
 from ..exceptions import UnhandledBranchError
-from ..model import AggregatedIntrospectionMixin, InterpreterContext
+from ..model import AggregatedIntrospectiveIngestionComponent, InterpreterContext
 from ..value_providers import StaticValueOrValueProvider, ValueProvider
 from .interpretation import Interpretation
 
 
 class SwitchInterpretation(
-    AggregatedIntrospectionMixin, Interpretation, alias="switch"
+    AggregatedIntrospectiveIngestionComponent, Interpretation, alias="switch"
 ):
     __slots__ = (
         "switch_on",
         "interpretations",
         "default",
         "normalization",
         "fail_on_unhandled",
@@ -23,20 +23,18 @@
         cases: Dict[str, dict],
         default: Dict[str, Any] = None,
         normalization: Dict[str, Any] = None,
         fail_on_unhandled: bool = True,
     ):
         self.switch_on = ValueProvider.guarantee_value_provider(switch_on)
         self.interpretations = {
-            field_value: Interpretation.from_file_arguments(**interpretation)
+            field_value: Interpretation.from_file_data(**interpretation)
             for field_value, interpretation in cases.items()
         }
-        self.default = (
-            Interpretation.from_file_arguments(**default) if default else None
-        )
+        self.default = Interpretation.from_file_data(**default) if default else None
         self.normalization = normalization or {}
         self.fail_on_unhandled = fail_on_unhandled
 
     def all_subordinate_components(self):
         yield from self.interpretations.values()
         if self.default:
             yield self.default
```

### Comparing `nodestream-0.2.0/nodestream/model/__init__.py` & `nodestream-0.3.0/nodestream/model/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     RelationshipIdentityShape,
 )
 from .indexes import FieldIndex, KeyIndex
 from .ingest_strategy import IngestionStrategy
 from .ingestion_hooks import IngestionHook, IngestionHookRunRequest
 from .interpreter_context import InterpreterContext, JsonLikeDocument
 from .schema import (
-    AggregatedIntrospectionMixin,
+    AggregatedIntrospectiveIngestionComponent,
     Cardinality,
     GraphObjectShape,
     GraphObjectType,
     GraphSchema,
     IntrospectiveIngestionComponent,
     KnownTypeMarker,
     PresentRelationship,
@@ -48,14 +48,14 @@
     "TypeMarker",
     "KnownTypeMarker",
     "UnknownTypeMarker",
     "PropertyMetadataSet",
     "PropertyMetadata",
     "PropertyType",
     "IntrospectiveIngestionComponent",
-    "AggregatedIntrospectionMixin",
+    "AggregatedIntrospectiveIngestionComponent",
     "Cardinality",
     "PresentRelationship",
     "RelationshipIdentityShape",
     "NodeIdentityShape",
     "GraphSchema",
 )
```

### Comparing `nodestream-0.2.0/nodestream/model/desired_ingest.py` & `nodestream-0.3.0/nodestream/model/desired_ingest.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/model/graph_objects.py` & `nodestream-0.3.0/nodestream/model/graph_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+from abc import ABC
 from dataclasses import dataclass, field
-from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
 from .match_strategy import MatchStrategy
 
 if TYPE_CHECKING:
     from ..value_providers.value_provider import ValueProvider
     from .interpreter_context import InterpreterContext
 
 
+class DeduplicatableObject(ABC):
+    def get_dedup_key(self) -> tuple:
+        raise NotImplementedError
+
+    def update(self, other: "DeduplicatableObject"):
+        raise NotImplementedError
+
+
 class PropertySet(dict):
     def set_property(self, property_key: str, property_value: Any):
         self[property_key] = property_value
 
     @classmethod
     def default_properties(cls) -> "PropertySet":
-        from ..pipeline import get_pipeline_name
+        from pandas import Timestamp
+
+        from ..pipeline.meta import get_context
 
         """Returns a default set of properties which set values.
 
         These default values indicate when the current pipeline touched the object the properties are for.
         """
-        pipeline_name = get_pipeline_name()
-        now = datetime.utcnow()
+        pipeline_name = get_context().name
+        now = Timestamp.utcnow()
         return cls(
             {
                 "last_ingested_at": now,
                 f"last_ingested_by_{pipeline_name}_at": now,
                 f"was_ingested_by_{pipeline_name}": True,
             }
         )
@@ -49,15 +59,15 @@
         """
         for key, provider in provider_map.items():
             v = provider.normalize_single_value(context, **norm_args)
             self.set_property(key, v)
 
 
 @dataclass(slots=True)
-class Node:
+class Node(DeduplicatableObject):
     """A `Node` is a entity that has a distinct identity.
 
     Each `Node` represents an entity (a person, place, thing, category or other piece of data) that has a distinct
     identity. Nodestream assumes the underlying graph database layer is a Labeled Property Graph. The identity
     of a node is defined by a root `type` (sometimes referred to as a label) as well as set of property name, value pairs
     representing the primary key of that node. In a relational database, this would be the combination of the table name
     as well as the primary key columns.
@@ -93,17 +103,20 @@
 
     def has_same_key(self, other: "Node") -> bool:
         return self.key_values == other.key_values
 
     def update(self, other: "Relationship"):
         self.properties.update(other.properties)
 
+    def get_dedup_key(self) -> tuple:
+        return tuple(sorted(self.key_values.values()))
 
-@dataclass(slots=True)
-class Relationship:
+
+@dataclass(slots=True, frozen=True)
+class Relationship(DeduplicatableObject):
     """A `Relationship` represents an inherent connection between two `Node`s.
 
     Each `Relationship` follows a relatively similar model to a `Node`. There is a _single_ type for the relationship.
     Relationships can store properties on the relationship itself (This would be similar to a jump table in a relational database).
 
     A key for a `Relationship` can also be provided. By default, `nodestream` will assume that there should be one
     relationship of the same type between two nodes. By providing keys, `nodestream` will create multiple relationships between
@@ -124,17 +137,20 @@
 
     def has_same_key(self, other: "Node") -> bool:
         return self.key_values == other.key_values
 
     def update(self, other: "Relationship"):
         self.properties.update(other.properties)
 
+    def get_dedup_key(self) -> tuple:
+        return tuple(sorted(self.key_values.values()))
+
 
 @dataclass(slots=True)
-class RelationshipWithNodes:
+class RelationshipWithNodes(DeduplicatableObject):
     """Stores information about the related node and the relationship itself."""
 
     from_node: Node
     to_node: Node
     relationship: Relationship
 
     to_side_match_strategy: MatchStrategy = MatchStrategy.EAGER
@@ -148,14 +164,21 @@
         )
 
     def update(self, other: "RelationshipWithNodes"):
         self.to_node.properties.update(other.to_node.properties)
         self.from_node.properties.update(other.from_node.properties)
         self.relationship.properties.update(other.relationship.properties)
 
+    def get_dedup_key(self) -> tuple:
+        return (
+            self.to_node.get_dedup_key(),
+            self.from_node.get_dedup_key(),
+            self.relationship.get_dedup_key(),
+        )
+
 
 @dataclass(slots=True, frozen=True)
 class NodeIdentityShape:
     type: str
     keys: Tuple[str]
     additional_types: Tuple[str] = field(default_factory=tuple)
```

### Comparing `nodestream-0.2.0/nodestream/model/indexes.py` & `nodestream-0.3.0/nodestream/model/indexes.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/model/ingest_strategy.py` & `nodestream-0.3.0/nodestream/model/ingest_strategy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/model/ingestion_hooks.py` & `nodestream-0.3.0/nodestream/model/ingestion_hooks.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/model/interpreter_context.py` & `nodestream-0.3.0/nodestream/model/interpreter_context.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/model/schema.py` & `nodestream-0.3.0/nodestream/model/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
 
 class IntrospectiveIngestionComponent(ABC):
     """An IntrospectableIngestionComponent is a componet that can be interrogated what it contributes the Graph Database Schema.
 
     Nearly all components in the transformation part of the ingestion stack (Interpreters, Interpretations, and Pipelines) are
     `IntrospectableIngestionComponent`s. Leaf components like Interpretations provide a relatively local scope as to what it knows
     about the schema. As is the hierarchy grows, more and more data is is combined and aggregated together until an entire schema
-    is produced. For more information on aggregation, see `AggregatedIntrospectionMixin`.
+    is produced. For more information on aggregation, see `AggregatedIntrospectiveIngestionComponent`.
     """
 
     @abstractmethod
     def gather_used_indexes(self):
         raise NotImplementedError
 
     @abstractmethod
@@ -363,15 +363,15 @@
         relationships = self.gather_present_relationships()
         return GraphSchema(
             object_shapes=_merge_overlapping_items(shapes, shapes),
             relationships=_merge_overlapping_items(relationships, shapes),
         )
 
 
-class AggregatedIntrospectionMixin(ABC):
+class AggregatedIntrospectiveIngestionComponent(IntrospectiveIngestionComponent):
     """A mixin to provide utilities for `IntrospectableIngestionComponent`s that are aggregations of others.
 
     For many types in our ingestion hierarchy, they are aggregations of subordinate components that each
     on their own provide part of the make up for a graph schema. When we look at higher order components such
     as a Interpreter, they need to merge and resolve ambiguity amongst its child ingestion components (Interpretations).
 
     This mixin provides that higher order aggregation logic to merge and resolve ambiguity amongst such a hierarchy.
```

### Comparing `nodestream-0.2.0/nodestream/model/ttl.py` & `nodestream-0.3.0/nodestream/model/ttl.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/normalizers/normalizer.py` & `nodestream-0.3.0/nodestream/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/pipeline/__init__.py` & `nodestream-0.3.0/nodestream/pipeline/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from .class_loader import ClassLoader
 from .extractors import Extractor, IterableExtractor
-from .filters import Filter, ValuesMatchPossibilitiesFilter
+from .filters import (
+    ExcludeWhenValuesMatchPossibilities,
+    Filter,
+    ValuesMatchPossibilitiesFilter,
+)
 from .flush import Flush
-from .meta import UNKNOWN_PIPELINE_NAME, get_pipeline_name, set_pipeline_name
+from .meta import UNKNOWN_PIPELINE_NAME
 from .pipeline import Pipeline
 from .pipeline_file_loader import PipelineFileLoader, PipelineInitializationArguments
 from .step import PassStep, Step
 from .transformers import Transformer
 from .writers import LoggerWriter, Writer
 
 __all__ = (
     "ClassLoader",
     "Extractor",
     "IterableExtractor",
     "Filter",
     "ValuesMatchPossibilitiesFilter",
+    "ExcludeWhenValuesMatchPossibilities",
     "PipelineFileLoader",
     "Pipeline",
     "Step",
     "Transformer",
     "Writer",
     "LoggerWriter",
     "PipelineInitializationArguments",
     "PassStep",
     "Flush",
-    "get_pipeline_name",
-    "set_pipeline_name",
     "UNKNOWN_PIPELINE_NAME",
 )
```

### Comparing `nodestream-0.2.0/nodestream/pipeline/class_loader.py` & `nodestream-0.3.0/nodestream/pipeline/class_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from importlib import import_module
 
 from ..exceptions import InvalidClassPathError, PipelineComponentInitializationError
 
-DECLARATIVE_INIT_METHOD_NAME = "__declarative_init__"
+DECLARATIVE_INIT_METHOD_NAME = "from_file_data"
 
 
 def find_class(class_path):
     try:
         module_name, class_name = class_path.split(":")
         module = import_module(module_name)
         return getattr(module, class_name)
```

### Comparing `nodestream-0.2.0/nodestream/pipeline/extractors.py` & `nodestream-0.3.0/nodestream/pipeline/extractors.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/pipeline/filters.py` & `nodestream-0.3.0/nodestream/pipeline/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @abstractmethod
     async def filter_record(self, record: Any) -> bool:
         raise NotImplementedError
 
 
 class ValueMatcher:
     @classmethod
-    def from_file_arguments(
+    def from_file_data(
         cls,
         value: StaticValueOrValueProvider,
         possibilities: Iterable[StaticValueOrValueProvider],
         normalization: Optional[Dict[str, Any]] = None,
     ):
         return cls(
             value_provider=ValueProvider.guarantee_value_provider(value),
@@ -62,19 +62,32 @@
         )
 
 
 class ValuesMatchPossibilitiesFilter(Filter):
     """A filter that checks if a given value matches any of a set of possibilities."""
 
     @classmethod
-    def __declarative_init__(cls, *, fields: Iterable[Dict[str, Any]]):
-        value_matchers = [ValueMatcher.from_file_arguments(**field) for field in fields]
+    def from_file_data(cls, *, fields: Iterable[Dict[str, Any]]):
+        value_matchers = [ValueMatcher.from_file_data(**field) for field in fields]
         return cls(value_matchers=value_matchers)
 
     def __init__(self, value_matchers: Iterable[ValueMatcher]):
         self.value_matchers = value_matchers
 
     async def filter_record(self, item):
         context_from_record = InterpreterContext(item, None)
         return not all(
             matcher.does_match(context_from_record) for matcher in self.value_matchers
         )
+
+
+class ExcludeWhenValuesMatchPossibilities(Filter):
+    @classmethod
+    def from_file_data(cls, **kwargs):
+        inner = ValuesMatchPossibilitiesFilter.from_file_data(**kwargs)
+        return cls(inner)
+
+    def __init__(self, inner: ValuesMatchPossibilitiesFilter) -> None:
+        self.inner = inner
+
+    async def filter_record(self, record: Any) -> bool:
+        return not await self.inner.filter_record(record)
```

### Comparing `nodestream-0.2.0/nodestream/pipeline/pipeline.py` & `nodestream-0.3.0/nodestream/pipeline/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+import asyncio
 from functools import reduce
 from typing import Any, AsyncGenerator, Iterable, List
 
-from ..model import AggregatedIntrospectionMixin, IntrospectiveIngestionComponent
+from ..model import (
+    AggregatedIntrospectiveIngestionComponent,
+    IntrospectiveIngestionComponent,
+)
 from .step import Step
 
 
 async def empty_async_generator():
     for item in []:
         yield item
 
 
-class Pipeline(AggregatedIntrospectionMixin, IntrospectiveIngestionComponent):
+class Pipeline(AggregatedIntrospectiveIngestionComponent):
     """A pipeline is a series of steps that are executed in order."""
 
     __slots__ = ("steps",)
 
     def __init__(self, steps: List[Step]) -> None:
         self.steps = steps
 
-    def run(self) -> AsyncGenerator[Any, Any]:
+    async def run(self) -> AsyncGenerator[Any, Any]:
         record_stream_over_all_steps = reduce(
             lambda stream, step: step.handle_async_record_stream(stream),
             self.steps,
             empty_async_generator(),
         )
-        return record_stream_over_all_steps
+        async for record in record_stream_over_all_steps:
+            yield record
+
+        await self.finish()
+
+    async def finish(self):
+        await asyncio.gather(*(step.finish() for step in self.steps))
 
     def all_subordinate_components(self) -> Iterable[IntrospectiveIngestionComponent]:
         return (s for s in self.steps if isinstance(s, IntrospectiveIngestionComponent))
```

### Comparing `nodestream-0.2.0/nodestream/pipeline/pipeline_file_loader.py` & `nodestream-0.3.0/nodestream/pipeline/pipeline_file_loader.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/pipeline/step.py` & `nodestream-0.3.0/nodestream/pipeline/step.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 from typing import Any, AsyncGenerator
 
 
 class Step(ABC):
     """A `Step` represents a phase of an ETl pipeline."""
 
     @classmethod
-    def __declarative_init__(cls, **kwargs):
+    def from_file_data(cls, **kwargs):
         return cls(**kwargs)
 
     @abstractmethod
     async def handle_async_record_stream(
         self, record_stream: AsyncGenerator[Any, Any]
     ) -> AsyncGenerator[Any, Any]:
         raise NotImplementedError
 
+    async def finish(self):
+        pass
+
 
 class PassStep(Step):
     """A `PassStep` is a step that does nothing."""
 
     async def handle_async_record_stream(
         self, record_stream: AsyncGenerator[Any, Any]
     ) -> AsyncGenerator[Any, Any]:
```

### Comparing `nodestream-0.2.0/nodestream/pipeline/transformers.py` & `nodestream-0.3.0/nodestream/pipeline/transformers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/pipeline/writers.py` & `nodestream-0.3.0/nodestream/pipeline/writers.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,18 @@
     async def handle_async_record_stream(
         self, record_stream: AsyncGenerator[Any, Any]
     ) -> AsyncGenerator[Any, Any]:
         async for record in record_stream:
             await self.write_record(record)
             yield record
 
-        await self.finish()
-
     @abstractmethod
     async def write_record(self, record: Any):
         raise NotImplementedError
 
-    async def finish(self):
-        pass
-
 
 class LoggerWriter(Writer):
     """A `Writer` that logs the record to a logger."""
 
     def __init__(self, logger_name=None, level=INFO) -> None:
         logger_name = logger_name or self.__class__.__name__
         self.logger = getLogger(logger_name)
```

### Comparing `nodestream-0.2.0/nodestream/project/pipeline_definition.py` & `nodestream-0.3.0/nodestream/project/pipeline_definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,81 @@
+import os.path
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict
 
+from ..file_io import LoadsFromYaml, SavesToYaml
 from ..model import IntrospectiveIngestionComponent
 from ..pipeline import Pipeline, PipelineFileLoader, PipelineInitializationArguments
 
 
 def get_default_name(file_path: Path) -> str:
     return file_path.stem
 
 
 @dataclass
-class PipelineDefinition(IntrospectiveIngestionComponent):
+class PipelineDefinition(IntrospectiveIngestionComponent, SavesToYaml, LoadsFromYaml):
     """A `PipelineDefinition` represents a pipeline that can be loaded from a file."""
 
     name: str
     file_path: Path
     annotations: Dict[str, Any] = field(default_factory=dict)
 
     @classmethod
+    def from_path(cls, file_path: Path):
+        return cls(get_default_name(file_path), file_path)
+
+    @classmethod
+    def describe_yaml_schema(cls):
+        from schema import Optional, Or, Schema
+
+        return Schema(
+            Or(
+                str,
+                {
+                    Optional("name"): str,
+                    "path": os.path.exists,
+                    Optional("annotations"): {str: Or(str, int, float, bool)},
+                },
+            )
+        )
+
+    @classmethod
     def from_file_data(cls, data, parent_annotations):
         if isinstance(data, str):
             data = {"path": data}
 
         file_path = Path(data.pop("path"))
         name = data.pop("name", get_default_name(file_path))
         annotations = data.pop("annotations", {})
         return cls(name, file_path, {**parent_annotations, **annotations})
 
-    def initialize(self, init_args: PipelineInitializationArguments) -> Pipeline:
-        return PipelineFileLoader(self.file_path).load_pipeline(init_args)
-
-    @classmethod
-    def from_path(cls, path: Path):
-        return cls(name=get_default_name(path), file_path=path)
-
-    def as_file_definition(self):
+    def to_file_data(self):
         using_default_name = self.name == self.file_path.stem
         if using_default_name and not self.annotations:
             return str(self.file_path)
 
         result = {"path": str(self.file_path)}
         if not using_default_name:
             result["name"] = self.name
         if self.annotations:
             result["annotations"] = self.annotations
 
         return result
 
+    def initialize(self, init_args: PipelineInitializationArguments) -> Pipeline:
+        return PipelineFileLoader(self.file_path).load_pipeline(init_args)
+
     def remove_file(self, missing_ok: bool = True):
         self.file_path.unlink(missing_ok=missing_ok)
 
-    def intialize_for_introspection(self) -> Pipeline:
+    def initialize_for_introspection(self) -> Pipeline:
         return self.initialize(PipelineInitializationArguments.for_introspection())
 
     def gather_object_shapes(self):
-        return self.intialize_for_introspection().gather_object_shapes()
+        return self.initialize_for_introspection().gather_object_shapes()
 
     def gather_present_relationships(self):
-        return self.intialize_for_introspection().gather_present_relationships()
+        return self.initialize_for_introspection().gather_present_relationships()
 
     def gather_used_indexes(self):
-        return self.intialize_for_introspection().gather_used_indexes()
+        return self.initialize_for_introspection().gather_used_indexes()
```

### Comparing `nodestream-0.2.0/nodestream/project/pipeline_progress_reporter.py` & `nodestream-0.3.0/nodestream/project/pipeline_progress_reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from logging import Logger, getLogger
 from typing import Any, Callable
 
 from ..pipeline import Pipeline
+from ..pipeline.meta import PipelineContext, get_context
 from ..utilities import enumerate_async, get_max_mem_mb
 
 
 def no_op(*_, **__):
     pass
 
 
@@ -14,21 +15,21 @@
 class PipelineProgressReporter:
     """A `PipelineProgressReporter` is a utility that can be used to report on the progress of a pipeline."""
 
     reporting_frequency: int = 1000
     logger: Logger = field(default_factory=getLogger)
     callback: Callable[[int, Any], None] = field(default=no_op)
     on_start_callback: Callable[[], None] = field(default=no_op)
-    on_finish_callback: Callable[[], None] = field(default=no_op)
+    on_finish_callback: Callable[[PipelineContext], None] = field(default=no_op)
 
     async def execute_with_reporting(self, pipeline: Pipeline):
         self.on_start_callback()
         async for index, record in enumerate_async(pipeline.run()):
             if index % self.reporting_frequency == 0:
                 self.report(index, record)
-        self.on_finish_callback()
+        self.on_finish_callback(get_context())
 
     def report(self, index, record):
         self.logger.info(
             "Records Processed", extra={"index": index, "max_memory": get_max_mem_mb()}
         )
         self.callback(index, record)
```

### Comparing `nodestream-0.2.0/nodestream/project/pipeline_scope.py` & `nodestream-0.3.0/nodestream/project/pipeline_scope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from typing import Dict, Iterable, List
 
 from ..exceptions import MissingExpectedPipelineError
-from ..model import AggregatedIntrospectionMixin, IntrospectiveIngestionComponent
+from ..file_io import LoadsFromYaml, SavesToYaml
+from ..model import (
+    AggregatedIntrospectiveIngestionComponent,
+    IntrospectiveIngestionComponent,
+)
 from .pipeline_definition import PipelineDefinition
 from .run_request import RunRequest
 
 
-class PipelineScope(AggregatedIntrospectionMixin, IntrospectiveIngestionComponent):
+class PipelineScope(
+    AggregatedIntrospectiveIngestionComponent, LoadsFromYaml, SavesToYaml
+):
     """A `PipelineScope` represents a collection of pipelines subordinate to a project."""
 
     def __init__(self, name: str, pipelines: List[PipelineDefinition]) -> None:
         self.name = name
         self.pipelines_by_name: Dict[str, PipelineDefinition] = {}
         for pipeline in pipelines:
             self.add_pipeline_definition(pipeline)
@@ -21,14 +27,34 @@
         annotations = file_data.pop("annotations", {})
         pipelines = [
             PipelineDefinition.from_file_data(pipeline_data, annotations)
             for pipeline_data in pipelines_data
         ]
         return cls(scope_name, pipelines)
 
+    @classmethod
+    def describe_yaml_schema(cls):
+        from schema import Optional, Or, Schema
+
+        return Schema(
+            {
+                Optional("pipelines"): [
+                    PipelineDefinition.describe_yaml_schema(),
+                ],
+                Optional("annotations"): {
+                    str: Or(str, int, float, bool),
+                },
+            }
+        )
+
+    def to_file_data(self):
+        return {
+            "pipelines": [ppl.to_file_data() for ppl in self.pipelines_by_name.values()]
+        }
+
     async def run_request(self, run_request: "RunRequest"):
         if (name := run_request.pipeline_name) not in self:
             return
 
         await run_request.execute_with_definition(self[name])
 
     def __getitem__(self, pipeline_name):
@@ -57,16 +83,9 @@
 
         del self.pipelines_by_name[pipeline_name]
         if remove_pipeline_file:
             definition.remove_file(missing_ok=missing_ok)
 
         return True
 
-    def as_dict(self):
-        return {
-            "pipelines": [
-                ppl.as_file_definition() for ppl in self.pipelines_by_name.values()
-            ]
-        }
-
     def all_subordinate_components(self) -> Iterable[IntrospectiveIngestionComponent]:
         return self.pipelines_by_name.values()
```

### Comparing `nodestream-0.2.0/nodestream/project/project.py` & `nodestream-0.3.0/nodestream/project/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 import importlib
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, TypeVar, Type, Tuple
+from typing import Dict, Iterable, List, Optional, Tuple, Type, TypeVar
 
-from yaml import safe_load
-
-from ..pipeline import Step
-from ..exceptions import MissingProjectFileError
+from ..file_io import LoadsFromYamlFile, SavesToYamlFile
 from ..model import (
-    AggregatedIntrospectionMixin,
+    AggregatedIntrospectiveIngestionComponent,
     GraphSchema,
     IntrospectiveIngestionComponent,
 )
-from ..utilities import pretty_print_yaml_to_file
-from .pipeline_scope import PipelineScope
+from ..pipeline import Step
 from .pipeline_definition import PipelineDefinition
+from .pipeline_scope import PipelineScope
 from .run_request import RunRequest
 
-
 T = TypeVar("T", bound=Step)
 
 
-class Project(AggregatedIntrospectionMixin, IntrospectiveIngestionComponent):
+class Project(
+    AggregatedIntrospectiveIngestionComponent, LoadsFromYamlFile, SavesToYamlFile
+):
     """A `Project` represents a collection of pipelines."""
 
     @classmethod
-    def from_file(cls, path: Path) -> "Project":
-        if not path.exists:
-            raise MissingProjectFileError(path)
+    def describe_yaml_schema(cls):
+        from schema import Optional, Schema
 
-        with open(path) as fp:
-            return cls.from_file_data(safe_load(fp))
+        return Schema(
+            {
+                Optional("scopes"): {
+                    str: PipelineScope.describe_yaml_schema(),
+                },
+                Optional("imports"): [str],
+            }
+        )
 
     @classmethod
     def from_file_data(cls, data) -> "Project":
         scopes_data = data.pop("scopes", {})
         scopes = [
             PipelineScope.from_file_data(*scope_data)
             for scope_data in scopes_data.items()
         ]
         imports = data.pop("imports", [])
         return cls(scopes, imports)
 
+    def to_file_data(self):
+        return {
+            "scopes": {
+                scope.name: scope.to_file_data()
+                for scope in self.scopes_by_name.values()
+            },
+            "imports": self.imports,
+        }
+
     def __init__(self, scopes: List[PipelineScope], imports: List[str]):
         self.scopes_by_name: Dict[str, PipelineScope] = {}
         for scope in scopes:
             self.add_scope(scope)
         self.imports = imports
 
     def ensure_modules_are_imported(self):
@@ -54,17 +66,14 @@
     async def run(self, request: RunRequest):
         for scope in self.scopes_by_name.values():
             await scope.run_request(request)
 
     def add_scope(self, scope: PipelineScope):
         self.scopes_by_name[scope.name] = scope
 
-    def write_to_path(self, path: Path):
-        pretty_print_yaml_to_file(path, self.as_dict())
-
     def get_scopes_by_name(self, scope_name: Optional[str]) -> Iterable[PipelineScope]:
         if scope_name is None:
             return self.scopes_by_name.values()
 
         if scope_name not in self.scopes_by_name:
             return []
 
@@ -80,33 +89,27 @@
         for scopes in self.get_scopes_by_name(scope_name):
             scopes.delete_pipeline(
                 pipeline_name,
                 remove_pipeline_file=remove_pipeline_file,
                 missing_ok=missing_ok,
             )
 
-    def as_dict(self):
-        return {
-            "scopes": {
-                scope.name: scope.as_dict() for scope in self.scopes_by_name.values()
-            },
-            "imports": self.imports,
-        }
-
     def get_schema(self, type_overrides_file: Optional[Path] = None) -> GraphSchema:
         schema = self.generate_graph_schema()
         if type_overrides_file is not None:
             schema.apply_type_overrides_from_file(type_overrides_file)
         return schema
 
     def all_subordinate_components(self) -> Iterable[IntrospectiveIngestionComponent]:
         return self.scopes_by_name.values()
 
     def dig_for_step_of_type(
         self, step_type: Type[T]
     ) -> Iterable[Tuple[PipelineDefinition, int, T]]:
         for scope in self.scopes_by_name.values():
             for pipeline_definition in scope.pipelines_by_name.values():
-                pipeline_steps = pipeline_definition.intialize_for_introspection().steps
+                pipeline_steps = (
+                    pipeline_definition.initialize_for_introspection().steps
+                )
                 for idx, step in enumerate(pipeline_steps):
                     if isinstance(step, step_type):
                         yield pipeline_definition, idx, step
```

### Comparing `nodestream-0.2.0/nodestream/project/run_request.py` & `nodestream-0.3.0/nodestream/project/run_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from dataclasses import dataclass
 
-from ..pipeline import PipelineInitializationArguments, set_pipeline_name
+from ..pipeline import PipelineInitializationArguments
+from ..pipeline.meta import start_context
 from .pipeline_definition import PipelineDefinition
 from .pipeline_progress_reporter import PipelineProgressReporter
 
 
 @dataclass
 class RunRequest:
     """A `RunRequest` represents a request to run a pipeline."""
 
     pipeline_name: str
     initialization_arguments: PipelineInitializationArguments
     progress_reporter: PipelineProgressReporter
 
     async def execute_with_definition(self, definition: PipelineDefinition):
-        with set_pipeline_name(self.pipeline_name):
+        with start_context(self.pipeline_name):
             pipeline = definition.initialize(self.initialization_arguments)
             await self.progress_reporter.execute_with_reporting(pipeline)
```

### Comparing `nodestream-0.2.0/nodestream/subclass_registry.py` & `nodestream-0.3.0/nodestream/subclass_registry.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/utilities.py` & `nodestream-0.3.0/nodestream/utilities.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/value_providers/__init__.py` & `nodestream-0.3.0/nodestream/value_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/value_providers/jmespath_value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/jmespath_value_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from ..model import InterpreterContext
 from .value_provider import ValueProvider
 
 
 class JmespathValueProvider(ValueProvider):
     """A `ValueProvider` that uses JMESPath to extract values from a document."""
 
+    __slots__ = ("compiled_query",)
+
     @classmethod
     def install_yaml_tag(cls, loader: Type[SafeLoader]):
         loader.add_constructor(
             "!jmespath",
             lambda loader, node: cls.from_string_expression(
                 loader.construct_scalar(node)
             ),
```

### Comparing `nodestream-0.2.0/nodestream/value_providers/jq_value_provder.py` & `nodestream-0.3.0/nodestream/value_providers/jq_value_provder.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from ..model import InterpreterContext
 from .value_provider import ValueProvider
 
 
 class JqValueProvider(ValueProvider):
     """A `ValueProvider` that uses Jq to extract values from a document."""
 
+    __slots__ = ("jq_program",)
+
     @classmethod
     def install_yaml_tag(cls, loader: Type[SafeLoader]):
         loader.add_constructor(
             "!jq", lambda loader, node: cls(jq.compile(loader.construct_scalar(node)))
         )
 
     def __init__(self, jq_program) -> None:
```

### Comparing `nodestream-0.2.0/nodestream/value_providers/mapping_value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/mapping_value_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from ..model import InterpreterContext
 from .value_provider import StaticValueOrValueProvider, ValueProvider
 
 
 class MappingValueProvider(ValueProvider):
     """A `ValueProvider` that uses a mapping to extract values from a document."""
 
+    __slots__ = ("mapping_name", "key")
+
     @classmethod
     def install_yaml_tag(cls, loader: Type[SafeLoader]):
         loader.add_constructor(
             "!mapping",
             lambda loader, node: MappingValueProvider(**loader.construct_mapping(node)),
         )
```

### Comparing `nodestream-0.2.0/nodestream/value_providers/static_value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/static_value_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from ..model import InterpreterContext
 from .value_provider import ValueProvider
 
 
 class StaticValueProvider(ValueProvider):
     """A `ValueProvider` that always returns the same value."""
 
+    __slots__ = ("value",)
+
     def __init__(self, value) -> None:
         self.value = value
 
     def single_value(self, _: InterpreterContext) -> Any:
         return self.value
 
     def many_values(self, _: InterpreterContext) -> Iterable[Any]:
```

### Comparing `nodestream-0.2.0/nodestream/value_providers/string_format_value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/string_format_value_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from ..model import InterpreterContext
 from .value_provider import StaticValueOrValueProvider, ValueProvider
 
 
 class StringFormattingValueProvider(ValueProvider):
     """A `ValueProvider` that uses string formatting to produce a value."""
 
+    __slots__ = ("fmt", "subs")
+
     @classmethod
     def install_yaml_tag(cls, loader: Type[SafeLoader]):
         loader.add_constructor(
             "!format", lambda loader, node: cls(**loader.construct_mapping(node))
         )
 
     def __init__(
```

### Comparing `nodestream-0.2.0/nodestream/value_providers/value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.2.0/nodestream/value_providers/variable_value_provider.py` & `nodestream-0.3.0/nodestream/value_providers/variable_value_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any, Iterable, Type
 
-import jq
 from yaml import SafeLoader
 
 from ..model import InterpreterContext
 from .value_provider import ValueProvider
 
 
 class VariableValueProvider(ValueProvider):
     """A `ValueProvider` that uses a variable to extract values from a document."""
 
+    __slots__ = ("variable_name",)
+
     @classmethod
     def install_yaml_tag(cls, loader: Type[SafeLoader]):
         loader.add_constructor(
             "!variable",
-            lambda loader, node: cls(jq.compile(loader.construct_scalar(node))),
+            lambda loader, node: cls(loader.construct_scalar(node)),
         )
 
     def __init__(self, variable_name: str) -> None:
         self.variable_name = variable_name
 
     def single_value(self, context: InterpreterContext) -> Any:
         return context.variables.get(self.variable_name)
```

### Comparing `nodestream-0.2.0/PKG-INFO` & `nodestream-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodestream
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Fast, Declarative ETL for Graph Databases.
 Home-page: https://github.com/nodestream-proj/nodestream
 License: GPL-3.0-only
 Keywords: etl,neo4j,declarative,data,kafka,ingest
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
@@ -23,16 +23,18 @@
 Requires-Dist: aiokafka (>=0.8.0,<0.9.0)
 Requires-Dist: boto3 (>=1.26.137,<2.0.0)
 Requires-Dist: cleo (>=2.0.1,<3.0.0)
 Requires-Dist: cymple (==0.8.1)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jq (>=1.4.1,<2.0.0)
 Requires-Dist: neo4j (>=5.8.0,<6.0.0)
+Requires-Dist: pandas (>=2,<3)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: schema (>=0.7.5,<0.8.0)
 Project-URL: Documentation, https://nodestream-proj.github.io/nodestream
 Project-URL: Repository, https://github.com/nodestream-proj/nodestream
 Description-Content-Type: text/markdown
 
 
 # Nodestream
 
@@ -47,15 +49,15 @@
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
 [![PyPI version](https://badge.fury.io/py/nodestream.svg)](https://badge.fury.io/py/nodestream)
 
 ## Features
 
 - Flexible and extensible YAML based DSL for ETL jobs
 - Connect to data sources like Kafka, AWS Athena, flat files, and more.
-- Developer friendly features such as snapshot testing
+- Developer friendly
 - Highly optimized with async and tuned query generation
 
 
 ## Getting Started
 
 Install nodestream with `pip`
 
@@ -82,9 +84,10 @@
 
 ## Authors
 
 - Zach Probst ([@zprobst](https://www.github.com/zprobst))
 - Chad Cloes ([@ccloes](https://www.github.com/ccloes))
 - Oshri Rozenberg([@orozen](https://www.github.com/orozen))
 - Kevin Neal ([@khneal](https://www.github.com/khneal))
+- Grant Hoffman ([@grantleehoffman](https://www.github.com/grantleehoffman))
```

