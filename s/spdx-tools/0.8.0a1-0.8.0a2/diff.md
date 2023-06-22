# Comparing `tmp/spdx-tools-0.8.0a1.tar.gz` & `tmp/spdx-tools-0.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdx-tools-0.8.0a1.tar", last modified: Thu Apr 20 14:22:18 2023, max compression
+gzip compressed data, was "spdx-tools-0.8.0a2.tar", last modified: Wed May 17 08:09:19 2023, max compression
```

## Comparing `spdx-tools-0.8.0a1.tar` & `spdx-tools-0.8.0a2.tar`

### file list

```diff
@@ -1,354 +1,359 @@
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.circleci/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      316 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.circleci/config.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      147 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/.editorconfig
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      123 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/.flake8
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.github/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      502 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a1/.github/dependabot.yml
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.github/workflows/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      772 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.github/workflows/check_codestyle.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1167 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.github/workflows/install_and_test.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      442 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/.gitignore
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3709 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a1/CHANGELOG.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4048 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/CONTRIBUTING.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11356 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/LICENSE
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      360 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/MANIFEST.in
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11784 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/PKG-INFO
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10830 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/README.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      549 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/appveyor.yml
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/assets/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)   147064 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/assets/SPDXJSONExample-v2.3.spdx.png
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/examples/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6181 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/examples/spdx2_document_from_scratch.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2181 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/pyproject.toml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       38 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/setup.cfg
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)       88 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/setup.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.445628 spdx-tools-0.8.0a1/src/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.445628 spdx-tools-0.8.0a1/src/spdx_tools/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/src/spdx_tools/common/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      421 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/constructor_type_errors.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2259 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/dataclass_with_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1186 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/type_checks.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.449628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      507 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/casing_tools.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.449628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4870 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/pyspdxtools.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      127 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/constants.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      599 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/datetime_conversions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/document_utils.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      890 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/formats.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3367 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/graph_generation.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.450628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/annotation_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      322 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/annotation_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1223 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/checksum_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      269 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/checksum_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3263 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1505 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/creation_info_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      320 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/creation_info_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5260 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      583 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1559 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      312 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_document_ref_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1363 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_package_ref_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1775 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      346 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3341 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      619 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      429 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/json_property.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      449 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/optional_utils.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      950 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1254 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_verification_code_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/relationship_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      337 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/relationship_properties.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3713 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/snippet_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/snippet_properties.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      941 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1068 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/actor.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      849 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/annotation.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/checksum.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2845 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/document.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/external_document_ref.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1082 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/extracted_licensing_info.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2711 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/file.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5547 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/package.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2145 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1880 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship_filters.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1896 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/snippet.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      424 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/spdx_no_assertion.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      372 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/spdx_none.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/version.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2352 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/actor_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      317 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/error.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      451 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/json_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.452628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4930 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1252 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5606 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2830 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1576 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3934 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1005 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9546 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8696 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6292 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/logger.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1477 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parse_anything.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parsing_functions.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/annotation_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1517 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/checksum_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5514 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2122 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3751 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/file_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5556 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2814 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8924 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/package_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4422 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/rdf_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2482 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/relationship_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6398 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/snippet_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5259 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6949 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/lexer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    29288 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      388 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/tagvalue_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2082 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/xml_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      457 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/yaml_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/py.typed
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      368 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/namespace.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1019 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/actor_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/annotation_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/checksum_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1692 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/creation_info_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4741 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/document_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1926 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_document_ref_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_package_ref_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1936 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3385 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/file_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2893 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/license_expression_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6514 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_verification_code_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1948 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/relationship_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3988 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/snippet_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3916 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/spdx_id_validators.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1427 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/uri_validators.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1038 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/validation_message.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1474 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/json_writer.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.455628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1520 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/annotation_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1009 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/checksum_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2006 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      991 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/file_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3979 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/package_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3026 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/rdf_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2001 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/relationship_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3246 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/snippet_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2257 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/writer_utils.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1319 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1485 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1382 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2004 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/file_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4391 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/package_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1205 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1809 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4792 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4351 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1184 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/write_anything.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/xml_writer.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1480 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/yaml_writer.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/src/spdx_tools.egg-info/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    14412 2023-04-20 14:22:18.000000 spdx-tools-0.8.0a1/src/spdx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       93 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/stdeb.cfg
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/tests/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/tests/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.457628 spdx-tools-0.8.0a1/tests/spdx/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.462628 spdx-tools-0.8.0a1/tests/spdx/data/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20805 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    21342 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1141 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXLite.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)   338588 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)   342594 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18104 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.2.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18538 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24020 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24884 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    19895 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20504 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/fixtures.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.463628 spdx-tools-0.8.0a1/tests/spdx/jsonschema/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1965 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_annotation_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_checksum_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2674 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_creation_info_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10012 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_document_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2361 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_document_ref_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2020 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_package_ref_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3621 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_file_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    15912 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_verification_code_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2722 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_relationship_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_snippet_converter.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/mock_utils.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/model/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/model/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1764 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_actor.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1762 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_annotation.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      592 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_checksum.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4008 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_creation_info.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_document.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1028 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_external_document_ref.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1210 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_external_package_reference.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1230 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_extracted_licensing_info.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_file.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7323 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_package.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      666 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_package_verification_code.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1105 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_relationship.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3087 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_snippet.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      827 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_version.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/parser/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2146 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/test_parse_from_file.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6439 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_annotation_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1587 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_checksum_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4968 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1582 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3004 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7138 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_file_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1560 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13446 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_package_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8057 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_relationship_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5605 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_snippet_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/data/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13653 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_annotation_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2960 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_checksum_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3506 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_creation_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1575 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_file_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1314 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_graph_parsing_function.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1987 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_license_expression_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4256 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_package_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2492 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_relationship_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6750 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_snippet_parser.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.466629 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3016 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_annotation_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_creation_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3720 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2805 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_file_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5014 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_helper_methods.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6118 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_package_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_relationship_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3489 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_snippet_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    16856 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_lexer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2945 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_actor_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      788 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_casing_tools.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_cli.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      986 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_datetime_conversions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4798 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_document_utils.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_graph_generation.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/validation/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/validation/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_actor_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1415 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_annotation_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    12050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_checksum_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1663 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_creation_info_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5938 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_document_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      639 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_external_document_ref_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13202 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_external_package_ref_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1675 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_extracted_licensing_info_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2443 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_file_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5644 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_license_expression_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_package_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1924 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_package_verification_code_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2937 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_relationship_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2596 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_snippet_validator.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6481 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_spdx_id_validators.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_uri_validators.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/json/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5745 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/expected.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1400 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/test_json_writer.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.468629 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1133 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_annotation_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_checksum_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1573 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_creation_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1036 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_external_document_ref_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1307 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1612 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_file_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2719 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_license_expression_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5264 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_package_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      632 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_rdf_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      942 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_relationship_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_snippet_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      874 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_writer_utils.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/expected_results/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1306 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1018 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_annotation_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1227 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_checksum_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_creation_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1165 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1617 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_file_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2905 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_package_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_relationship_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1552 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_snippet_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4996 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.296769 spdx-tools-0.8.0a2/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.244768 spdx-tools-0.8.0a2/.circleci/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      316 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/.circleci/config.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      147 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/.editorconfig
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      123 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/.flake8
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.244768 spdx-tools-0.8.0a2/.github/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      502 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a2/.github/dependabot.yml
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.245768 spdx-tools-0.8.0a2/.github/workflows/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      772 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/.github/workflows/check_codestyle.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1167 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/.github/workflows/install_and_test.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      442 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/.gitignore
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3709 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a2/CHANGELOG.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4048 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/CONTRIBUTING.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11356 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/LICENSE
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      360 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/MANIFEST.in
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11784 2023-05-17 08:09:19.295769 spdx-tools-0.8.0a2/PKG-INFO
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10830 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/README.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      549 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/appveyor.yml
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.245768 spdx-tools-0.8.0a2/assets/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   147064 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/assets/SPDXJSONExample-v2.3.spdx.png
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.245768 spdx-tools-0.8.0a2/examples/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6181 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/examples/spdx2_document_from_scratch.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2307 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/pyproject.toml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)       38 2023-05-17 08:09:19.296769 spdx-tools-0.8.0a2/setup.cfg
+-rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)       88 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/setup.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.242768 spdx-tools-0.8.0a2/src/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.242768 spdx-tools-0.8.0a2/src/spdx_tools/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.246768 spdx-tools-0.8.0a2/src/spdx_tools/common/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/common/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.246768 spdx-tools-0.8.0a2/src/spdx_tools/common/typing/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/common/typing/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      421 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/common/typing/constructor_type_errors.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3126 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/common/typing/dataclass_with_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1186 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/common/typing/type_checks.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.248768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      507 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/casing_tools.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.248768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/clitools/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/clitools/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4870 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/clitools/pyspdxtools.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      127 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/constants.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      599 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/datetime_conversions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/document_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      890 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/formats.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3367 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/graph_generation.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.252768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/annotation_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      322 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/annotation_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1223 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/checksum_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      269 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/checksum_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3263 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1505 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/creation_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      320 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/creation_info_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5260 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/document_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      583 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/document_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1559 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      312 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_document_ref_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1363 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_package_ref_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1775 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      346 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3341 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/file_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      619 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/file_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      429 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/json_property.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      449 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/optional_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      950 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1254 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_verification_code_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/relationship_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      337 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/relationship_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3713 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/snippet_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/snippet_properties.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.254768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1030 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1068 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/actor.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      849 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/annotation.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/checksum.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2845 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/document.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/external_document_ref.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1082 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/extracted_licensing_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2711 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/file.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5547 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/package.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2145 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/relationship.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1880 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/relationship_filters.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1896 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/snippet.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      424 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/spdx_no_assertion.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      372 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/spdx_none.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/version.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.255768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2352 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/actor_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      317 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/error.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.255768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/json/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      451 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/json/json_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.257768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4930 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1252 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5100 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2830 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1576 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3934 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1005 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9546 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8696 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6292 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/logger.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1477 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/parse_anything.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/parsing_functions.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.258768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1517 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5582 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2122 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3798 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5634 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2814 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8985 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4302 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/rdf_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2482 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6419 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.259768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5259 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6949 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/lexer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    29555 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      388 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/tagvalue_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.259768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/xml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/xml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2099 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/xml/xml_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.259768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/yaml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/yaml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      457 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/yaml/yaml_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/py.typed
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.259768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/rdfschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/rdfschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      368 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/rdfschema/namespace.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.263769 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1019 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/actor_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/annotation_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/checksum_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1692 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/creation_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4741 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/document_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1926 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/external_document_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/external_package_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1936 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3385 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/file_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2893 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/license_expression_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6514 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/package_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/package_verification_code_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1948 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/relationship_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3988 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/snippet_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3916 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/spdx_id_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1427 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/uri_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1038 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/validation_message.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.264768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.264768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/json/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1474 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/json/json_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.267768 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1520 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1009 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2006 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      991 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3979 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3026 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/rdf_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2001 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3246 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2257 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/writer_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.269769 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1319 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1485 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1382 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2004 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4391 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1205 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1809 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4792 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4351 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1184 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/write_anything.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.269769 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/xml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/xml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/xml/xml_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.269769 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/yaml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/yaml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1480 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/yaml/yaml_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.295769 spdx-tools-0.8.0a2/src/spdx_tools.egg-info/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    14699 2023-05-17 08:09:19.000000 spdx-tools-0.8.0a2/src/spdx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)       93 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/stdeb.cfg
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.269769 spdx-tools-0.8.0a2/tests/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a2/tests/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.271769 spdx-tools-0.8.0a2/tests/spdx/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.276769 spdx-tools-0.8.0a2/tests/spdx/data/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20805 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    21342 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1141 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXLite.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   338588 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   342594 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18104 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXTagExample-v2.2.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18538 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24020 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24809 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    19895 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20429 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/fixtures.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.278769 spdx-tools-0.8.0a2/tests/spdx/jsonschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1965 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_annotation_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_checksum_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2674 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_creation_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10012 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_document_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2361 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_external_document_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2020 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_external_package_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3621 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_file_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    15912 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_package_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_package_verification_code_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2722 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_relationship_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_snippet_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/mock_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.283769 spdx-tools-0.8.0a2/tests/spdx/model/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/model/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1764 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_actor.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1762 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_annotation.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      592 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_checksum.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4008 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_creation_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_document.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1028 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_external_document_ref.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1210 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_external_package_reference.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1230 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_extracted_licensing_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_file.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7323 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_package.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      666 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_package_verification_code.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1105 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_relationship.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3087 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_snippet.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      827 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/model/test_version.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.283769 spdx-tools-0.8.0a2/tests/spdx/parser/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.283769 spdx-tools-0.8.0a2/tests/spdx/parser/all_formats/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/all_formats/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2146 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/all_formats/test_parse_from_file.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.285769 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4896 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1329 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3429 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1582 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1544 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_error_message.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2659 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6206 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1560 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11438 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7717 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4815 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.287769 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.287769 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13653 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.287769 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/invalid_documents/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2491 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      781 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4516 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2960 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4223 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2062 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1314 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_graph_parsing_function.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1987 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4740 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2492 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7173 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.290769 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3016 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3720 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2805 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5014 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_helper_methods.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6118 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3489 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_snippet_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    16856 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_tag_value_lexer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3946 2023-05-17 07:53:32.000000 spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_tag_value_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_actor_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      788 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_casing_tools.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_cli.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      986 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_datetime_conversions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4798 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_document_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/test_graph_generation.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.292769 spdx-tools-0.8.0a2/tests/spdx/validation/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/validation/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_actor_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1415 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_annotation_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    12050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_checksum_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1663 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_creation_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5938 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_document_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      639 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_external_document_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13202 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_external_package_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1675 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_extracted_licensing_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2443 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_file_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5644 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_license_expression_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_package_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1924 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_package_verification_code_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2937 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_relationship_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2596 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_snippet_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6481 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_spdx_id_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/validation/test_uri_validators.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.292769 spdx-tools-0.8.0a2/tests/spdx/writer/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.292769 spdx-tools-0.8.0a2/tests/spdx/writer/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/json/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.292769 spdx-tools-0.8.0a2/tests/spdx/writer/json/expected_results/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/json/expected_results/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5745 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/json/expected_results/expected.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1400 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/json/test_json_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.294769 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1133 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1573 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1036 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_external_document_ref_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1307 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1612 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2719 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_license_expression_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5264 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      632 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_rdf_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      942 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      874 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_writer_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.295769 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-05-17 08:09:19.295769 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/expected_results/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1306 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1018 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1227 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1165 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1617 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2905 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1552 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4996 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_tagvalue_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py
```

### Comparing `spdx-tools-0.8.0a1/.github/workflows/check_codestyle.yml` & `spdx-tools-0.8.0a2/.github/workflows/check_codestyle.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/.github/workflows/install_and_test.yml` & `spdx-tools-0.8.0a2/.github/workflows/install_and_test.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/CHANGELOG.md` & `spdx-tools-0.8.0a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/CONTRIBUTING.md` & `spdx-tools-0.8.0a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/LICENSE` & `spdx-tools-0.8.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/PKG-INFO` & `spdx-tools-0.8.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdx-tools
-Version: 0.8.0a1
+Version: 0.8.0a2
 Summary: SPDX parser and tools.
 Author-email: "Ahmed H. Ismail" <ahm3d.hisham@gmail.com>
 Maintainer: SPDX group at the Linux Foundation and others
 Maintainer-email: Philippe Ombredanne <pombredanne@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/tools-python
 Classifier: Intended Audience :: Developers
@@ -42,15 +42,15 @@
 
 We encourage you to use the new, refactored version (on the main branch) if you
 - want to use the soon-to-be released SPDX v3.0 in the future
 - want to perform full validation of your SPDX documents against the v2.2 and v2.3 specification
 - want to use the RDF format of SPDX with all v2.3 features.
 
 If you are planning to migrate from v0.7.x of these tools,
-please have a look at the [migration guide](https://github.com/spdx/tools-python/wiki/How-to-migrate-from-0.7-to-1.0).
+please have a look at the [migration guide](https://github.com/spdx/tools-python/wiki/How-to-migrate-from-0.7-to-0.8).
 
 # Information
 
 This library implements SPDX parsers, convertors, validators and handlers in Python.
 
 - Home: https://github.com/spdx/tools-python
 - Issues: https://github.com/spdx/tools-python/issues
```

### Comparing `spdx-tools-0.8.0a1/README.md` & `spdx-tools-0.8.0a2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 We encourage you to use the new, refactored version (on the main branch) if you
 - want to use the soon-to-be released SPDX v3.0 in the future
 - want to perform full validation of your SPDX documents against the v2.2 and v2.3 specification
 - want to use the RDF format of SPDX with all v2.3 features.
 
 If you are planning to migrate from v0.7.x of these tools,
-please have a look at the [migration guide](https://github.com/spdx/tools-python/wiki/How-to-migrate-from-0.7-to-1.0).
+please have a look at the [migration guide](https://github.com/spdx/tools-python/wiki/How-to-migrate-from-0.7-to-0.8).
 
 # Information
 
 This library implements SPDX parsers, convertors, validators and handlers in Python.
 
 - Home: https://github.com/spdx/tools-python
 - Issues: https://github.com/spdx/tools-python/issues
```

### Comparing `spdx-tools-0.8.0a1/appveyor.yml` & `spdx-tools-0.8.0a2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/assets/SPDXJSONExample-v2.3.spdx.png` & `spdx-tools-0.8.0a2/assets/SPDXJSONExample-v2.3.spdx.png`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/examples/spdx2_document_from_scratch.py` & `spdx-tools-0.8.0a2/examples/spdx2_document_from_scratch.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/pyproject.toml` & `spdx-tools-0.8.0a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { Homepage = "https://github.com/spdx/tools-python" }
 requires-python = ">=3.7"
-dependencies = ["click", "pyyaml", "xmltodict", "rdflib", "typeguard==2.13.3", "uritools", "license_expression", "ply"]
+dependencies = ["click", "pyyaml", "xmltodict", "rdflib", "typeguard==4.0.0", "uritools", "license_expression", "ply"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 code_style = ["isort", "black", "flake8"]
 graph_generation = ["pygraphviz", "networkx"]
 development = ["black", "flake8", "isort", "networkx", "pytest"]
@@ -58,7 +58,10 @@
 line-length = 119
 include = "(^/src/.*.py|^/tests/.*.py)"
 
 [tool.isort]
 profile = "black"
 line_length = 119
 skip = ["__init__.py"]
+
+[tool.pytest.ini_options]
+norecursedirs = []  # overwrite the default to not skip tests/build folder which is needed in spdx3
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/common/typing/type_checks.py` & `spdx-tools-0.8.0a2/src/spdx_tools/common/typing/type_checks.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/pyspdxtools.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/clitools/pyspdxtools.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/datetime_conversions.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/datetime_conversions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/document_utils.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/document_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/formats.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/formats.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/graph_generation.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/graph_generation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/annotation_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/annotation_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/checksum_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/checksum_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/creation_info_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/creation_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/document_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_properties.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/document_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/file_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_properties.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/file_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_properties.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/relationship_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/relationship_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/snippet_converter.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/jsonschema/snippet_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/actor.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/actor.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/annotation.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/checksum.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/checksum.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/document.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/external_document_ref.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/external_document_ref.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/extracted_licensing_info.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/extracted_licensing_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/file.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/package.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship_filters.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/relationship_filters.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/snippet.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/version.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/model/version.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/actor_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/actor_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 from typing import Dict, List, Optional
 
 from spdx_tools.spdx.datetime_conversions import datetime_from_str
 from spdx_tools.spdx.model import Actor, Checksum, CreationInfo, ExternalDocumentRef, Version
 from spdx_tools.spdx.parser.actor_parser import ActorParser
 from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.jsonlikedict.checksum_parser import ChecksumParser
-from spdx_tools.spdx.parser.jsonlikedict.dict_parsing_functions import (
-    append_parsed_field_or_log_error,
-    parse_field_or_log_error,
-    parse_field_or_no_assertion,
-)
+from spdx_tools.spdx.parser.jsonlikedict.dict_parsing_functions import parse_field_or_log_error
 from spdx_tools.spdx.parser.logger import Logger
 from spdx_tools.spdx.parser.parsing_functions import (
     construct_or_raise_parsing_error,
     raise_parsing_error_if_logger_has_messages,
 )
 
 
@@ -41,15 +37,15 @@
 
         # There are nested required properties. If creationInfo is not set, we cannot continue parsing.
         if creation_info_dict is None:
             logger.append("CreationInfo does not exist.")
             raise SPDXParsingError([f"Error while parsing document {name}: {logger.get_messages()}"])
 
         creators: List[Actor] = parse_field_or_log_error(
-            logger, creation_info_dict.get("creators"), self.parse_creators
+            logger, creation_info_dict.get("creators"), self.actor_parser.parse_actor, field_is_list=True
         )
 
         created: Optional[datetime] = parse_field_or_log_error(
             logger, creation_info_dict.get("created"), datetime_from_str
         )
 
         creator_comment: Optional[str] = creation_info_dict.get("comment")
@@ -79,25 +75,14 @@
                 data_license=data_license,
                 external_document_refs=external_document_refs,
             ),
         )
 
         return creation_info
 
-    def parse_creators(self, creators_list_from_dict: List[str]) -> List[Actor]:
-        logger = Logger()
-        creators = []
-        for creator_str in creators_list_from_dict:
-            creators = append_parsed_field_or_log_error(
-                logger, creators, creator_str, lambda x: parse_field_or_no_assertion(x, self.actor_parser.parse_actor)
-            )
-
-        raise_parsing_error_if_logger_has_messages(logger)
-        return creators
-
     @staticmethod
     def parse_version(version_str: str) -> Version:
         try:
             return Version.from_string(version_str)
         except ValueError as err:
             raise SPDXParsingError([f"Error while parsing version {version_str}: {err.args[0]}"])
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ) -> List[Any]:
     try:
         parsed_element = method_to_parse(field)
         list_to_append_to.append(parsed_element)
     except SPDXParsingError as err:
         logger.extend(err.get_messages())
     except (TypeError, ValueError) as err:
-        logger.extend(err.args[0])
+        logger.append(err.args[0])
     return list_to_append_to
 
 
 def parse_field_or_no_assertion_or_none(field: Optional[str], method_for_field: Callable = lambda x: x) -> Any:
     if field == SpdxNoAssertion().__str__():
         return SpdxNoAssertion()
     elif field == SpdxNone().__str__():
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parse_anything.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/parse_anything.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parsing_functions.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/annotation_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/checksum_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     )
     creator_comment = parse_literal(logger, graph, creation_info_node, RDFS.comment)
     creators = []
     for _, _, creator_literal in get_correctly_typed_triples(
         logger, graph, creation_info_node, SPDX_NAMESPACE.creator
     ):
         creators.append(ActorParser.parse_actor(creator_literal.toPython()))
+    if not creators:
+        logger.append("No creators provided.")
     external_document_refs = []
     for _, _, external_document_node in get_correctly_typed_triples(
         logger, graph, doc_node, SPDX_NAMESPACE.externalDocumentRef
     ):
         external_document_refs.append(parse_external_document_refs(external_document_node, graph, namespace))
 
     raise_parsing_error_if_logger_has_messages(logger, "CreationInfo")
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/file_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/file_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
-from rdflib import RDFS, Graph, URIRef
+from typing import Union
+
+from rdflib import RDFS, BNode, Graph, URIRef
 
 from spdx_tools.spdx.model import File, FileType
 from spdx_tools.spdx.parser.logger import Logger
 from spdx_tools.spdx.parser.parsing_functions import (
     construct_or_raise_parsing_error,
     raise_parsing_error_if_logger_has_messages,
 )
@@ -19,15 +21,15 @@
     parse_literal_or_no_assertion_or_none,
     parse_spdx_id,
 )
 from spdx_tools.spdx.parser.rdf.license_expression_parser import parse_license_expression
 from spdx_tools.spdx.rdfschema.namespace import SPDX_NAMESPACE
 
 
-def parse_file(file_node: URIRef, graph: Graph, doc_namespace: str) -> File:
+def parse_file(file_node: Union[URIRef, BNode], graph: Graph, doc_namespace: str) -> File:
     logger = Logger()
     spdx_id = parse_spdx_id(file_node, doc_namespace, graph)
     name = parse_literal(logger, graph, file_node, SPDX_NAMESPACE.fileName)
     checksums = []
     for _, _, checksum_node in get_correctly_typed_triples(logger, graph, file_node, SPDX_NAMESPACE.checksum):
         checksums.append(parse_checksum(checksum_node, graph))
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         enum_without_rdf_prefix = remove_prefix(enum_str, prefix)
         value = camel_case_to_snake_case(enum_without_rdf_prefix).upper()
         return enum_class[value]
     except KeyError:
         raise SPDXParsingError([f"Invalid value for {enum_class}: {enum_str}"])
 
 
-def parse_spdx_id(resource: URIRef, doc_namespace: str, graph: Graph) -> Optional[str]:
-    if not resource:
+def parse_spdx_id(resource: Union[URIRef, BNode], doc_namespace: str, graph: Graph) -> Optional[str]:
+    if not resource or isinstance(resource, BNode):
         return None
     if resource.startswith(f"{doc_namespace}#"):
         return resource.fragment
     if "#" in resource:
         namespace_manager = NamespaceManager(graph)
         return namespace_manager.normalizeUri(resource)
     return resource.toPython() or None
@@ -136,13 +136,13 @@
     _object: Optional[Node] = None,
     default: Optional[Any] = None,
     _any: Optional[bool] = True,
 ) -> Optional[Union[URIRef, Literal, BNode]]:
     # this is a helper method to cast some rdf types from graph.value() to be compatible with the
     # code that follows
     value = graph.value(subject=subject, predicate=predicate, object=_object, default=default, any=_any)
-    if value and not isinstance(value, (URIRef, Literal, BNode)):
+    if value != default and value is not None and not isinstance(value, (URIRef, Literal, BNode)):
         logger.append(
             f"Warning: Node {value} should be of type BNode, Literal or URIRef, but is {type(value).__name__}. "
             f"This might lead to a failure."
         )
     return value
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/package_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/package_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import Optional
+from typing import Optional, Union
 
 from rdflib import DOAP, RDFS, Graph, URIRef
 from rdflib.term import BNode
 
 from spdx_tools.spdx.datetime_conversions import datetime_from_str
 from spdx_tools.spdx.model import (
     ExternalPackageRef,
@@ -30,15 +30,15 @@
     parse_literal_or_no_assertion_or_none,
     parse_spdx_id,
 )
 from spdx_tools.spdx.parser.rdf.license_expression_parser import parse_license_expression
 from spdx_tools.spdx.rdfschema.namespace import REFERENCE_NAMESPACE, SPDX_NAMESPACE
 
 
-def parse_package(package_node: URIRef, graph: Graph, doc_namespace: str) -> Package:
+def parse_package(package_node: Union[URIRef, BNode], graph: Graph, doc_namespace: str) -> Package:
     logger = Logger()
     spdx_id = parse_spdx_id(package_node, doc_namespace, graph)
     name = parse_literal(logger, graph, package_node, SPDX_NAMESPACE.name)
     download_location = parse_literal_or_no_assertion_or_none(
         logger, graph, package_node, SPDX_NAMESPACE.downloadLocation
     )
     checksums = []
@@ -104,25 +104,26 @@
         graph,
         package_node,
         SPDX_NAMESPACE.primaryPackagePurpose,
         parsing_method=lambda x: parse_enum_value(x, PackagePurpose, SPDX_NAMESPACE.purpose_),
     )
     homepage = parse_literal(logger, graph, package_node, DOAP.homepage)
     attribution_texts = []
-    for _, _, attribution_text_literal in graph.triples((package_node, SPDX_NAMESPACE.attributionText, None)):
+    for _, _, attribution_text_literal in get_correctly_typed_triples(
+        logger, graph, package_node, SPDX_NAMESPACE.attributionText, None
+    ):
         attribution_texts.append(attribution_text_literal.toPython())
 
     release_date = parse_literal(
         logger, graph, package_node, SPDX_NAMESPACE.releaseDate, parsing_method=datetime_from_str
     )
     built_date = parse_literal(logger, graph, package_node, SPDX_NAMESPACE.builtDate, parsing_method=datetime_from_str)
     valid_until_date = parse_literal(
         logger, graph, package_node, SPDX_NAMESPACE.validUntilDate, parsing_method=datetime_from_str
     )
-
     raise_parsing_error_if_logger_has_messages(logger, "Package")
     package = construct_or_raise_parsing_error(
         Package,
         dict(
             name=name,
             spdx_id=spdx_id,
             download_location=download_location,
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/rdf_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/rdf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,15 @@
     document: Document = translate_graph_to_document(graph)
     return document
 
 
 def translate_graph_to_document(graph: Graph) -> Document:
     parsed_fields: Dict[str, Any] = dict()
     logger = Logger()
-    try:
-        creation_info, doc_node = parse_creation_info(graph)
-    except SPDXParsingError as err:
-        logger.extend(err.get_messages())
-        creation_info = None
+    creation_info, doc_node = parse_creation_info(graph)
 
     parsed_fields["creation_info"] = creation_info
 
     for element, triple, parsing_method in [
         ("packages", (None, RDF.type, SPDX_NAMESPACE.Package), parse_package),
         ("files", (None, RDF.type, SPDX_NAMESPACE.File), parse_file),
         ("snippets", (None, RDF.type, SPDX_NAMESPACE.Snippet), parse_snippet),
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/relationship_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/snippet_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/rdf/snippet_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 from rdflib import RDF, RDFS, Graph
 from rdflib.exceptions import UniquenessError
 from rdflib.term import BNode, Node, URIRef
 
 from spdx_tools.spdx.model import Snippet
 from spdx_tools.spdx.parser.error import SPDXParsingError
@@ -23,15 +23,15 @@
     parse_literal_or_no_assertion_or_none,
     parse_spdx_id,
 )
 from spdx_tools.spdx.parser.rdf.license_expression_parser import parse_license_expression
 from spdx_tools.spdx.rdfschema.namespace import POINTER_NAMESPACE, SPDX_NAMESPACE
 
 
-def parse_snippet(snippet_node: URIRef, graph: Graph, doc_namespace: str) -> Snippet:
+def parse_snippet(snippet_node: Union[URIRef, BNode], graph: Graph, doc_namespace: str) -> Snippet:
     logger = Logger()
     spdx_id = parse_spdx_id(snippet_node, doc_namespace, graph)
     file_spdx_id_uri = get_value_from_graph(
         logger, graph, subject=snippet_node, predicate=SPDX_NAMESPACE.snippetFromFile
     )
     file_spdx_id = parse_spdx_id(file_spdx_id_uri, doc_namespace, graph)
     byte_range = None
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/lexer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/lexer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/tagvalue/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,11 +576,17 @@
         file_spdx_id = self.current_element["spdx_id"]
         if "packages" not in self.elements_built:
             return
         # We assume that all files that are not contained in a package precede any package information. Any file
         # information that follows any package information is assigned to the last parsed package by creating a
         # corresponding contains relationship.
         # (see https://spdx.github.io/spdx-spec/v2.3/composition-of-an-SPDX-document/#5.2.2)
+        if not self.elements_built["packages"]:
+            self.logger.append(
+                f"Error while building contains relationship for file {file_spdx_id}, "
+                f"preceding package was not parsed successfully."
+            )
+            return
         package_spdx_id = self.elements_built["packages"][-1].spdx_id
         relationship = Relationship(package_spdx_id, RelationshipType.CONTAINS, file_spdx_id)
         if relationship not in self.elements_built.setdefault("relationships", []):
             self.elements_built["relationships"].append(relationship)
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/xml_parser.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/parser/xml/xml_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     XML files do not contain lists. Thus, single fields that should be a list in SPDX have to be manually cast.
     This method takes a parsed dictionary and converts all values with key from LIST_LIKE_FIELDS to lists.
     """
     if isinstance(data, dict):
         new_data = {}
         for key, value in data.items():
             if key in LIST_LIKE_FIELDS and not isinstance(value, list):
-                new_data[key] = [_fix_list_like_fields(value)]
+                new_data[key] = [_fix_list_like_fields(value)] if value else []
             else:
                 new_data[key] = _fix_list_like_fields(value)
         return new_data
 
     if isinstance(data, list):
         new_data = []
         for element in data:
```

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/actor_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/actor_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/annotation_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/annotation_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/checksum_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/checksum_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/creation_info_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/creation_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/document_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/document_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_document_ref_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/external_document_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_package_ref_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/external_package_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/file_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/file_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/license_expression_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/license_expression_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/package_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_verification_code_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/package_verification_code_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/relationship_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/relationship_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/snippet_validator.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/snippet_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/spdx_id_validators.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/spdx_id_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/uri_validators.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/uri_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/validation_message.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/validation/validation_message.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/json_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/json/json_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/annotation_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/checksum_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/file_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/package_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/rdf_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/rdf_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/relationship_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/snippet_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/writer_utils.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/rdf/writer_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/file_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/package_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/write_anything.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/write_anything.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/xml_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/xml/xml_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/yaml_writer.py` & `spdx-tools-0.8.0a2/src/spdx_tools/spdx/writer/yaml/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/src/spdx_tools.egg-info/SOURCES.txt` & `spdx-tools-0.8.0a2/src/spdx_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
 tests/spdx/parser/all_formats/__init__.py
 tests/spdx/parser/all_formats/test_parse_from_file.py
 tests/spdx/parser/jsonlikedict/__init__.py
 tests/spdx/parser/jsonlikedict/test_annotation_parser.py
 tests/spdx/parser/jsonlikedict/test_checksum_parser.py
 tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
 tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
+tests/spdx/parser/jsonlikedict/test_error_message.py
 tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
 tests/spdx/parser/jsonlikedict/test_file_parser.py
 tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
 tests/spdx/parser/jsonlikedict/test_package_parser.py
 tests/spdx/parser/jsonlikedict/test_relationship_parser.py
 tests/spdx/parser/jsonlikedict/test_snippet_parser.py
 tests/spdx/parser/rdf/__init__.py
@@ -239,14 +240,17 @@
 tests/spdx/parser/rdf/test_file_parser.py
 tests/spdx/parser/rdf/test_graph_parsing_function.py
 tests/spdx/parser/rdf/test_license_expression_parser.py
 tests/spdx/parser/rdf/test_package_parser.py
 tests/spdx/parser/rdf/test_relationship_parser.py
 tests/spdx/parser/rdf/test_snippet_parser.py
 tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
+tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml
+tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml
+tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml
 tests/spdx/parser/tagvalue/__init__.py
 tests/spdx/parser/tagvalue/test_annotation_parser.py
 tests/spdx/parser/tagvalue/test_creation_info_parser.py
 tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
 tests/spdx/parser/tagvalue/test_file_parser.py
 tests/spdx/parser/tagvalue/test_helper_methods.py
 tests/spdx/parser/tagvalue/test_package_parser.py
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXLite.spdx` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXLite.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.2.spdx` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXTagExample-v2.2.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.3.spdx` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 1% similar despite different names*

#### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -263,15 +263,15 @@
   </packages>
   <packages>
     <SPDXID>SPDXRef-fromDoap-0</SPDXID>
     <downloadLocation>https://search.maven.org/remotecontent?filepath=org/apache/jena/apache-jena/3.12.0/apache-jena-3.12.0.tar.gz</downloadLocation>
     <externalRefs>
       <referenceCategory>PACKAGE-MANAGER</referenceCategory>
       <referenceLocator>pkg:maven/org.apache.jena/apache-jena@3.12.0</referenceLocator>
-      <referenceType>http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#purl</referenceType>
+      <referenceType>purl</referenceType>
     </externalRefs>
     <filesAnalyzed>false</filesAnalyzed>
     <homepage>http://www.openjena.org/</homepage>
     <name>Jena</name>
     <versionInfo>3.12.0</versionInfo>
   </packages>
   <packages>
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml` & `spdx-tools-0.8.0a2/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
   licenseDeclared: "NOASSERTION"
   name: "Apache Commons Lang"
 - SPDXID: "SPDXRef-fromDoap-0"
   downloadLocation: "https://search.maven.org/remotecontent?filepath=org/apache/jena/apache-jena/3.12.0/apache-jena-3.12.0.tar.gz"
   externalRefs:
   - referenceCategory: "PACKAGE-MANAGER"
     referenceLocator: "pkg:maven/org.apache.jena/apache-jena@3.12.0"
-    referenceType: "http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#purl"
+    referenceType: "purl"
   filesAnalyzed: false
   homepage: "http://www.openjena.org/"
   name: "Jena"
   versionInfo: "3.12.0"
 - SPDXID: "SPDXRef-Saxon"
   checksums:
   - algorithm: "SHA1"
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/fixtures.py` & `spdx-tools-0.8.0a2/tests/spdx/fixtures.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_annotation_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_annotation_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_checksum_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_checksum_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_creation_info_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_creation_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_document_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_document_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_document_ref_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_external_document_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_package_ref_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_external_package_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_file_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_file_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_package_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_verification_code_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_package_verification_code_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_relationship_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_relationship_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_snippet_converter.py` & `spdx-tools-0.8.0a2/tests/spdx/jsonschema/test_snippet_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/mock_utils.py` & `spdx-tools-0.8.0a2/tests/spdx/mock_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_actor.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_actor.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_annotation.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_checksum.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_checksum.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_creation_info.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_creation_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_document.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_external_document_ref.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_external_document_ref.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_external_package_reference.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_external_package_reference.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_extracted_licensing_info.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_extracted_licensing_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_file.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_package.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_package_verification_code.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_package_verification_code.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_relationship.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_snippet.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/model/test_version.py` & `spdx-tools-0.8.0a2/tests/spdx/model/test_version.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/test_parse_from_file.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/all_formats/test_parse_from_file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_checksum_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_checksum_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,17 +32,9 @@
     )
 
 
 def test_parse_incomplete_checksum():
     checksum_parser = ChecksumParser()
     checksum_dict = {"algorithm": "SHA1"}
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         checksum_parser.parse_checksum(checksum_dict)
-
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            'Error while constructing Checksum: [\'SetterError Checksum: type of argument "value" must be str; '
-            "got NoneType instead: None']"
-        ],
-    )
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_creation_info_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,124 @@
-# SPDX-FileCopyrightText: 2022 spdx contributors
+# SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
 from datetime import datetime
 from unittest import TestCase
 
 import pytest
 
 from spdx_tools.spdx.constants import DOCUMENT_SPDX_ID
 from spdx_tools.spdx.model import Actor, ActorType, Checksum, ChecksumAlgorithm, ExternalDocumentRef, Version
 from spdx_tools.spdx.parser.error import SPDXParsingError
-from spdx_tools.spdx.parser.jsonlikedict.creation_info_parser import CreationInfoParser
+from spdx_tools.spdx.parser.tagvalue.parser import Parser
 
+DOCUMENT_STR = "\n".join(
+    [
+        "SPDXVersion: SPDX-2.3",
+        "DataLicense: CC0-1.0",
+        "DocumentName: Sample_Document-V2.3",
+        f"SPDXID: {DOCUMENT_SPDX_ID}",
+        "DocumentComment: <text>Sample Comment</text>",
+        "DocumentNamespace: https://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301",
+        "ExternalDocumentRef: DocumentRef-spdx-tool-1.2 "
+        "http://spdx.org/spdxdocs/spdx-tools-v1.2-3F2504E0-4F89-41D3-9A0C-0305E82C3301 "
+        "SHA1: d6a770ba38583ed4bb4525bd96e50461655d2759",
+        "Creator: Person: Bob (bob@example.com)",
+        "Creator: Organization: Acme.",
+        "Created: 2010-02-03T00:00:00Z",
+        "CreatorComment: <text>Sample Comment \nwith multiple \nlines.</text>",
+        "LicenseListVersion: 3.17",
+    ]
+)
 
-def test_parse_creation_info():
-    creation_info_parser = CreationInfoParser()
-    doc_dict = {
-        "spdxVersion": "2.3",
-        "SPDXID": DOCUMENT_SPDX_ID,
-        "name": "Example Document",
-        "dataLicense": "CC0-1.0",
-        "documentNamespace": "namespace",
-        "externalDocumentRefs": [
-            {
-                "externalDocumentId": "DocumentRef-spdx-tool-1.2",
-                "checksum": {"algorithm": "SHA1", "checksumValue": "d6a770ba38583ed4bb4525bd96e50461655d2759"},
-                "spdxDocument": "http://spdx.org/spdxdocs/spdx-tools-v1.2-3F2504E0-4F89-41D3-9A0C-0305E82C3301",
-            }
-        ],
-        "creationInfo": {
-            "created": "2010-01-29T18:30:22Z",
-            "creators": ["Tool: LicenseFind-1.0", "Organization: ExampleCodeInspect ()", "Person: Jane Doe ()"],
-            "licenseListVersion": "3.7",
-            "comment": "Some comment.",
-        },
-    }
-    creation_info = creation_info_parser.parse_creation_info(doc_dict)
 
-    assert creation_info.spdx_version == "2.3"
+def test_parse_creation_info():
+    parser = Parser()
+    document = parser.parse(DOCUMENT_STR)
+    assert document is not None
+    creation_info = document.creation_info
+    assert creation_info is not None
+    assert creation_info.spdx_version == "SPDX-2.3"
+    assert creation_info.data_license == "CC0-1.0"
+    assert creation_info.name == "Sample_Document-V2.3"
     assert creation_info.spdx_id == DOCUMENT_SPDX_ID
-    assert creation_info.name == "Example Document"
-    assert creation_info.document_namespace == "namespace"
-    assert creation_info.created == datetime(2010, 1, 29, 18, 30, 22)
+    assert creation_info.document_comment == "Sample Comment"
+    assert (
+        creation_info.document_namespace
+        == "https://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301"
+    )
     TestCase().assertCountEqual(
         creation_info.creators,
-        [
-            Actor(ActorType.TOOL, "LicenseFind-1.0"),
-            Actor(ActorType.ORGANIZATION, "ExampleCodeInspect"),
-            Actor(ActorType.PERSON, "Jane Doe"),
-        ],
+        [Actor(ActorType.PERSON, "Bob", "bob@example.com"), Actor(ActorType.ORGANIZATION, "Acme.")],
     )
-    assert creation_info.license_list_version == Version(3, 7)
+    assert creation_info.creator_comment == "Sample Comment \nwith multiple \nlines."
+    assert creation_info.created == datetime(2010, 2, 3)
+    assert creation_info.license_list_version == Version(3, 17)
     assert creation_info.external_document_refs == [
         ExternalDocumentRef(
-            document_ref_id="DocumentRef-spdx-tool-1.2",
-            checksum=Checksum(algorithm=ChecksumAlgorithm.SHA1, value="d6a770ba38583ed4bb4525bd96e50461655d2759"),
-            document_uri="http://spdx.org/spdxdocs/spdx-tools-v1.2-3F2504E0-4F89-41D3-9A0C-0305E82C3301",
+            "DocumentRef-spdx-tool-1.2",
+            "http://spdx.org/spdxdocs/spdx-tools-v1.2-3F2504E0-4F89-41D3-9A0C-0305E82C3301",
+            Checksum(ChecksumAlgorithm.SHA1, "d6a770ba38583ed4bb4525bd96e50461655d2759"),
         )
     ]
 
 
 @pytest.mark.parametrize(
-    "incomplete_dict,expected_message",
-    [
-        (
-            {"spdxVersion": "2.3", "SPDXID": DOCUMENT_SPDX_ID, "name": "Example Document"},
-            ["Error while parsing document Example Document: ['CreationInfo does not exist.']"],
-        ),
-        (
-            {"creationInfo": {"created": "2019-02-01T11:30:40Z"}},
-            [
-                "Error while constructing CreationInfo: ['SetterError CreationInfo: type of "
-                'argument "spdx_version" must be str; got NoneType instead: None\', '
-                '\'SetterError CreationInfo: type of argument "spdx_id" must be str; got '
-                "NoneType instead: None', 'SetterError CreationInfo: type of argument "
-                "\"name\" must be str; got NoneType instead: None', 'SetterError "
-                'CreationInfo: type of argument "document_namespace" must be str; got '
-                "NoneType instead: None', 'SetterError CreationInfo: type of argument "
-                "\"creators\" must be a list; got NoneType instead: None', 'SetterError "
-                'CreationInfo: type of argument "data_license" must be str; got NoneType '
-                "instead: None']"
-            ],
-        ),
-    ],
+    "document_str, expected_message",
+    (
+        [
+            (
+                "\n".join(
+                    [
+                        "SPDXVersion: SPDX-2.3",
+                        "DataLicense: CC0-1.0",
+                        "DocumentName: Sample_Document-V2.3",
+                        f"SPDXID: {DOCUMENT_SPDX_ID}",
+                        "DocumentComment: <text>Sample Comment</text>",
+                        "DocumentNamespace: <text>Sample Comment</text>",
+                        "ExternalDocumentRef: DocumentRef-spdx-tool-1.2:htp://spdx.org:SHA1: "
+                        "d6a770ba38583ed4bb4525bd96e50461655d2759",
+                        "Creator: Person Bob (bob@example.com)",
+                        "Creator: Organization: Acme [email]",
+                        "Created: 2010-02-03T00:00:0Z",
+                        "CreatorComment: <text>Sample Comment</text>",
+                        "LicenseListVersion: 7",
+                    ]
+                ),
+                (
+                    "Error while parsing CreationInfo: ['Error while parsing DocumentNamespace: "
+                    "Token did not match specified grammar rule. Line: 6', \"Error while parsing "
+                    "ExternalDocumentRef: Couldn't split the first part of the value into "
+                    "document_ref_id and document_uri. Line: 7\", 'Error while parsing Creator: "
+                    "Token did not match specified grammar rule. Line: 8', 'Error while parsing "
+                    "Created: Token did not match specified grammar rule. Line: 10', '7 is not a "
+                    "valid version string']"
+                ),
+            ),
+            (
+                "\n".join(
+                    [
+                        "SPDXVersion: SPDX-2.3",
+                        "DataLicense: CC0-1.0",
+                        "DocumentName: Sample_Document-V2.3",
+                        f"SPDXID: {DOCUMENT_SPDX_ID}",
+                    ]
+                ),
+                r"__init__() missing 3 required positional arguments: 'document_namespace', 'creators', and 'created'",
+            ),
+            (
+                "LicenseListVersion: 3.5\nLicenseListVersion: 3.7",
+                "Error while parsing CreationInfo: ['Multiple values for LicenseListVersion found. Line: 2']",
+            ),
+            (
+                "ExternalDocumentRef: Document_ref document_uri SHA1: afded",
+                "Error while parsing CreationInfo: [\"Error while parsing ExternalDocumentRef: Couldn't match "
+                'Checksum. Line: 1"]',
+            ),
+        ]
+    ),
 )
-def test_parse_incomplete_document_info(incomplete_dict, expected_message):
-    creation_info_parser = CreationInfoParser()
-
+def test_parse_invalid_creation_info(document_str, expected_message):
+    parser = Parser()
     with pytest.raises(SPDXParsingError) as err:
-        creation_info_parser.parse_creation_info(incomplete_dict)
-
-    TestCase().assertCountEqual(err.value.get_messages(), expected_message)
-
-
-def test_parse_invalid_creation_info():
-    creation_info_parser = CreationInfoParser()
-    doc_dict = {
-        "spdxVersion": "2.3",
-        "SPDXID": DOCUMENT_SPDX_ID,
-        "name": "Example Document",
-        "creationInfo": {
-            "created": "2010-01-29T18:30:22Z",
-            "creators": ["Tool: LicenseFind-1.0", "Organization: ExampleCodeInspect ()", "Person: Jane Doe ()"],
-        },
-        "dataLicense": None,
-    }
-
-    with pytest.raises(SPDXParsingError) as err:
-        creation_info_parser.parse_creation_info(doc_dict)
-
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing CreationInfo: ['SetterError CreationInfo: type of "
-            'argument "document_namespace" must be str; got NoneType instead: None\', '
-            '\'SetterError CreationInfo: type of argument "data_license" must be str; got '
-            "NoneType instead: None']"
-        ],
-    )
+        parser.parse(document_str)
+    assert expected_message in err.value.get_messages()[0]
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # SPDX-FileCopyrightText: 2022 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
-from unittest import TestCase
-
 import pytest
 
 from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.jsonlikedict.extracted_licensing_info_parser import ExtractedLicensingInfoParser
 
 
 def test_parse_extracted_licensing_info():
@@ -47,18 +45,9 @@
         "extractedText": '"THE BEER-WARE LICENSE" (Revision 42):\nphk@FreeBSD.ORG wrote this file. As long as you '
         "retain this notice you\ncan do whatever you want with this stuff. If we meet some day, and "
         "you think this stuff is worth it, you can buy me a beer in return Poul-Henning Kamp",
         "name": "Beer-Ware License (Version 42)",
         "seeAlsos": ["http://people.freebsd.org/~phk/"],
     }
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         extracted_licensing_info_parser.parse_extracted_licensing_info(extracted_licensing_infos_dict)
-
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing ExtractedLicensingInfo: ['SetterError "
-            'ExtractedLicensingInfo: type of argument "comment" must be one of (str, '
-            "NoneType); got int instead: 56']"
-        ],
-    )
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_file_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_file_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -89,30 +89,14 @@
     )
     assert (
         file.license_comment == "The concluded license was taken from the package level that the file was included in."
     )
     assert file.attribution_texts == ["Some attribution text."]
 
 
-def test_parse_incomplete_file():
-    file_parser = FileParser()
-    file_dict = {"SPDXID": "SPDXRef-File", "fileName": "Incomplete File"}
-
-    with pytest.raises(SPDXParsingError) as err:
-        file_parser.parse_file(file_dict)
-
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing File: ['SetterError File: type of argument "
-            '"checksums" must be a list; got NoneType instead: None\']'
-        ],
-    )
-
-
 def test_parse_invalid_files():
     file_parser = FileParser()
     files = [
         {"SPDXID": "SPDXRef-File", "fileName": "Incomplete File"},
         {
             "SPDXID": "SPDXRef-File",
             "attributionTexts": ["Some attribution text."],
@@ -125,28 +109,19 @@
             "SPDXID": "SPDXRef-File",
             "attributionTexts": ["Some attribution text."],
             "checksums": [
                 {"algorithm": "SHA1", "checksumValue": "d6a770ba38583ed4bb4525bd96e50461655d2758"},
                 {"algorithm": "MD", "checksumValue": "624c1abb3664f4b35547e7c73864ad24"},
             ],
         },
+        {"SPDXID": "SPDXRef-File", "fileName": "Incomplete File"},
     ]
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         parse_list_of_elements(files, file_parser.parse_file)
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing File: ['SetterError File: type of argument "
-            '"checksums" must be a list; got NoneType instead: None\']',
-            'Error while constructing File: [\'SetterError File: type of argument "name" '
-            "must be str; got NoneType instead: None']",
-            "Error while parsing File: [\"Error while parsing Checksum: ['Invalid ChecksumAlgorithm: MD']\"]",
-        ],
-    )
 
 
 def test_parse_file_types():
     file_parser = FileParser()
     file_types_list = ["OTHER", "APPLICATION"]
 
     file_types = file_parser.parse_file_types(file_types_list)
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_package_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_package_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -224,106 +224,57 @@
     assert package.primary_package_purpose == PackagePurpose.SOURCE
     assert package.release_date == datetime(2012, 1, 29, 18, 30, 22)
     assert package.built_date == datetime(2011, 1, 29, 18, 30, 22)
     assert package.valid_until_date == datetime(2014, 1, 29, 18, 30, 22)
 
 
 @pytest.mark.parametrize(
-    "incomplete_package_dict,expected_message",
+    "incomplete_package_dict",
     [
-        (
-            {"SPDXID": "SPDXRef-Package"},
-            [
-                "Error while constructing Package: ['SetterError Package: type of "
-                "argument \"name\" must be str; got NoneType instead: None', 'SetterError Package: type of argument "
-                '"download_location" must be one of (str, spdx_tools.spdx.model.spdx_no_assertion.SpdxNoAssertion, '
-                "spdx_tools.spdx.model.spdx_none.SpdxNone); "
-                "got NoneType instead: None']"
-            ],
-        ),
-        (
-            {"SPDXID": "SPDXRef-Package", "name": 5, "downloadLocation": "NONE"},
-            [
-                "Error while constructing Package: ['SetterError Package: type of argument "
-                '"name" must be str; got int instead: 5\']'
-            ],
-        ),
+        {"SPDXID": "SPDXRef-Package"},
+        {"SPDXID": "SPDXRef-Package", "name": 5, "downloadLocation": "NONE"},
+        {
+            "SPDXID": "SPDXRef-Package",
+            "name": "Example Package",
+            "downloadLocation": "NONE",
+            "checksums": [{"algorithm": "SHA", "value": "1234"}],
+        },
     ],
 )
-def test_parse_incomplete_package(incomplete_package_dict, expected_message):
+def test_parse_invalid_package(incomplete_package_dict):
     package_parser = PackageParser()
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         package_parser.parse_package(incomplete_package_dict)
 
-    TestCase().assertCountEqual(err.value.get_messages(), expected_message)
-
-
-def test_parse_invalid_package():
-    package_parser = PackageParser()
-    package_dict = {
-        "SPDXID": "SPDXRef-Package",
-        "name": "Example Package",
-        "downloadLocation": "NONE",
-        "checksums": [{"algorithm": "SHA", "value": "1234"}],
-    }
-
-    with pytest.raises(SPDXParsingError) as err:
-        package_parser.parse_package(package_dict)
-
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        ["Error while parsing Package: [\"Error while parsing Checksum: ['Invalid ChecksumAlgorithm: SHA']\"]"],
-    )
-
 
 def test_parse_packages():
     package_parser = PackageParser()
     packages_list = [
         {
             "SPDXID": "SPDXRef-Package",
             "name": "Example Package",
             "downloadLocation": "NONE",
             "checksums": [{"algorithm": "SHA", "value": "1234"}],
         },
         {"SPDXID": "SPDXRef-Package", "name": 5, "downloadLocation": "NONE"},
         {"SPDXID": "SPDXRef-Package", "name": "Example Package", "downloadLocation": "NONE"},
     ]
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         parse_list_of_elements(packages_list, package_parser.parse_package)
 
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            'Error while parsing Package: ["Error while parsing Checksum: ' "['Invalid ChecksumAlgorithm: SHA']\"]",
-            "Error while constructing Package: ['SetterError Package: type of argument "
-            '"name" must be str; got int instead: 5\']',
-        ],
-    )
-
 
 def test_parse_external_ref():
     package_parser = PackageParser()
     external_ref = {"referenceType": "fix"}
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         package_parser.parse_external_ref(external_ref)
 
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing ExternalPackageRef: ['SetterError "
-            'ExternalPackageRef: type of argument "category" must be '
-            "spdx_tools.spdx.model.package.ExternalPackageRefCategory; got NoneType instead: None', "
-            '\'SetterError ExternalPackageRef: type of argument "locator" must be str; '
-            "got NoneType instead: None']"
-        ],
-    )
-
 
 def test_parse_invalid_external_package_ref_category():
     package_parser = PackageParser()
     external_package_ref_category = "TEST"
 
     with pytest.raises(SPDXParsingError) as err:
         package_parser.parse_external_ref_category(external_package_ref_category)
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_relationship_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_relationship_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,17 @@
     relationship_parser = RelationshipParser()
     relationship_dict = {
         "spdxElementId": DOCUMENT_SPDX_ID,
         "relatedSpdxElement": "SPDXRef-Package",
         "comment": "Comment.",
     }
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         relationship_parser.parse_relationship(relationship_dict)
 
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing Relationship: ['SetterError Relationship: type of "
-            'argument "relationship_type" must be '
-            "spdx_tools.spdx.model.relationship.RelationshipType; got NoneType instead: None']"
-        ],
-    )
-
 
 def test_parse_relationship_type():
     relationship_parser = RelationshipParser()
     relationship_type_str = "DEPENDENCY_OF"
 
     relationship_type = relationship_parser.parse_relationship_type(relationship_type_str)
     assert relationship_type == RelationshipType.DEPENDENCY_OF
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_snippet_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/jsonlikedict/test_snippet_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,54 +70,34 @@
     assert snippet.attribution_texts == ["Some example attibution text."]
 
 
 def test_parse_incomplete_snippet():
     snippet_parser = SnippetParser()
     incomplete_snippet_dict = {"SPDXID": "SPDXRef-Snippet", "file_spdx_id": "SPDXRef-File"}
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         snippet_parser.parse_snippet(incomplete_snippet_dict)
 
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing Snippet: ['SetterError Snippet: type of argument "
-            "\"file_spdx_id\" must be str; got NoneType instead: None', 'SetterError Snippet: type of argument "
-            '"byte_range" must be a tuple; got NoneType '
-            "instead: None']"
-        ],
-    )
-
 
 def test_parse_snippet_with_invalid_snippet_range():
     snippet_parser = SnippetParser()
     snippet_with_invalid_ranges_list = {
         "SPDXID": "SPDXRef-Snippet",
         "file_spdx_id": "SPDXRef-File",
         "ranges": [
             {
                 "endPointer": {"offset": 23, "reference": "SPDXRef-DoapSource"},
                 "startPointer": {"offset": "310s", "reference": "SPDXRef-DoapSource"},
             }
         ],
     }
 
-    with pytest.raises(SPDXParsingError) as err:
+    with pytest.raises(SPDXParsingError):
         snippet_parser.parse_snippet(snippet_with_invalid_ranges_list)
 
-    TestCase().assertCountEqual(
-        err.value.get_messages(),
-        [
-            "Error while constructing Snippet: ['SetterError Snippet: type of argument "
-            "\"file_spdx_id\" must be str; got NoneType instead: None', 'SetterError "
-            'Snippet: type of argument "byte_range"[0] must be int; got str instead: '
-            "(\\'310s\\', 23)']"
-        ],
-    )
-
 
 def test_parse_invalid_snippet_range():
     snippet_parser = SnippetParser()
 
     ranges = [
         {
             "endPointer": {"lineNumber": 23, "reference": "SPDXRef-DoapSource"},
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_annotation_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_checksum_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_creation_info_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_creation_info_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 import pytest
 from rdflib import RDF, Graph, URIRef
 from rdflib.term import Node
 
 from spdx_tools.spdx.constants import DOCUMENT_SPDX_ID
 from spdx_tools.spdx.model import Actor, ActorType, Checksum, ChecksumAlgorithm, Version
+from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.rdf.creation_info_parser import (
     parse_creation_info,
     parse_external_document_refs,
     parse_namespace_and_spdx_id,
 )
+from spdx_tools.spdx.parser.rdf.rdf_parser import parse_from_file
 from spdx_tools.spdx.rdfschema.namespace import SPDX_NAMESPACE
 
 
 def test_parse_creation_info():
     graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/file_to_test_rdf_parser.rdf.xml"))
 
     creation_info, _ = parse_creation_info(graph)
@@ -86,7 +88,24 @@
     external_document_ref = parse_external_document_refs(external_doc_ref_node, graph, doc_namespace)
 
     assert external_document_ref.document_ref_id == "DocumentRef-external"
     assert external_document_ref.checksum == Checksum(
         ChecksumAlgorithm.SHA1, "71c4025dd9897b364f3ebbb42c484ff43d00791c"
     )
     assert external_document_ref.document_uri == "https://namespace.com"
+
+
+@pytest.mark.parametrize(
+    "file, error_message",
+    [
+        (
+            "invalid_creation_info.rdf.xml",
+            "Error while parsing CreationInfo: ['No creators provided.']",
+        ),
+        ("invalid_creation_info_with_snippet.rdf.xml", "Error while parsing CreationInfo: ['No creators provided.']"),
+    ],
+)
+def test_parse_invalid_creation_info(file, error_message):
+    with pytest.raises(SPDXParsingError) as err:
+        parse_from_file(os.path.join(os.path.dirname(__file__), f"data/invalid_documents/{file}"))
+
+    assert err.value.get_messages() == [error_message]
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_file_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_file_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 from unittest import TestCase
 
+import pytest
 from license_expression import get_spdx_licensing
-from rdflib import RDF, Graph, URIRef
+from rdflib import RDF, BNode, Graph, URIRef
 
 from spdx_tools.spdx.model import Checksum, ChecksumAlgorithm, FileType, SpdxNoAssertion
+from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.rdf.file_parser import parse_file
 from spdx_tools.spdx.rdfschema.namespace import SPDX_NAMESPACE
 
 
 def test_parse_file():
     graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/file_to_test_rdf_parser.rdf.xml"))
     file_node = graph.value(predicate=RDF.type, object=SPDX_NAMESPACE.File)
@@ -31,7 +33,17 @@
     TestCase().assertCountEqual(
         file.license_info_in_file,
         [get_spdx_licensing().parse("MIT"), get_spdx_licensing().parse("GPL-2.0"), SpdxNoAssertion()],
     )
     assert file.license_comment == "licenseComment"
     assert file.notice == "fileNotice"
     assert file.attribution_texts == ["fileAttributionText"]
+
+
+def test_parse_invalid_file():
+    graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/invalid_documents/file_without_spdx_ids.xml"))
+    file_node = graph.value(predicate=RDF.type, object=SPDX_NAMESPACE.File)
+    doc_namespace = "https://some.namespace"
+
+    assert isinstance(file_node, BNode)
+    with pytest.raises(SPDXParsingError):
+        parse_file(file_node, graph, doc_namespace)
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_graph_parsing_function.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_graph_parsing_function.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_license_expression_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_package_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_package_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Checksum,
     ChecksumAlgorithm,
     ExternalPackageRefCategory,
     PackagePurpose,
     PackageVerificationCode,
     SpdxNoAssertion,
 )
+from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.rdf.package_parser import parse_external_package_ref, parse_package
 from spdx_tools.spdx.rdfschema.namespace import SPDX_NAMESPACE
 
 
 def test_package_parser():
     graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/file_to_test_rdf_parser.rdf.xml"))
     # we have two packages in the test file, graph.value() will return the first package
@@ -91,7 +92,17 @@
 
     external_package_ref = parse_external_package_ref(external_package_ref_node, graph, doc_namespace)
 
     assert external_package_ref.category == category
     assert external_package_ref.locator == locator
     assert external_package_ref.reference_type == type
     assert external_package_ref.comment == comment
+
+
+def test_parse_invalid_package():
+    graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/invalid_documents/file_without_spdx_ids.xml"))
+    package_node = graph.value(predicate=RDF.type, object=SPDX_NAMESPACE.Package)
+    doc_namespace = "https://some.namespace"
+
+    assert isinstance(package_node, BNode)
+    with pytest.raises(SPDXParsingError):
+        parse_package(package_node, graph, doc_namespace)
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_relationship_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_snippet_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/rdf/test_snippet_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,17 @@
     start_end_pointer = BNode()
     graph.add((start_end_pointer, RDF.type, POINTER_NAMESPACE.StartEndPointer))
     for predicate, value, pointer_class, pointer_member in predicate_value_class_member:
         pointer_node = BNode()
         graph.add((pointer_node, RDF.type, pointer_class))
         graph.add((start_end_pointer, predicate, pointer_node))
         graph.add((pointer_node, pointer_member, Literal(value)))
+
+
+def test_parse_invalid_file():
+    graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/invalid_documents/file_without_spdx_ids.xml"))
+    snippet_node = graph.value(predicate=RDF.type, object=SPDX_NAMESPACE.Snippet)
+    doc_namespace = "https://some.namespace"
+
+    assert isinstance(snippet_node, BNode)
+    with pytest.raises(SPDXParsingError):
+        parse_snippet(snippet_node, graph, doc_namespace)
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_annotation_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_file_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_helper_methods.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_helper_methods.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_package_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_relationship_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_snippet_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_lexer.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_tag_value_lexer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/parser/tagvalue/test_tag_value_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,14 +50,39 @@
     assert document.relationships == [
         Relationship("SPDXRef-Package-with-two-files", RelationshipType.CONTAINS, "SPDXRef-File-in-Package"),
         Relationship("SPDXRef-Package-with-two-files", RelationshipType.CONTAINS, "SPDXRef-Second-File-in-Package"),
         Relationship("SPDXRef-Package-with-one-file", RelationshipType.CONTAINS, "SPDXRef-File-in-different-Package"),
     ]
 
 
+def test_build_contains_relationship_with_error():
+    parser = Parser()
+    file_spdx_ids = ["SPDXRef-File-in-Package", "SPDXRef-Second-File-in-Package"]
+    document_str = "\n".join(
+        [
+            DOCUMENT_STR,
+            "PackageName: Package with two files",
+            "PackageDownloadLocation: https://download.com",
+            "FileName: File in package",
+            f"SPDXID: {file_spdx_ids[0]}",
+            "FileChecksum: SHA1: d6a770ba38583ed4bb4525bd96e50461655d2759",
+            "FileName: Second file in package",
+            f"SPDXID: {file_spdx_ids[1]}",
+            "FileChecksum: SHA1: d6a770ba38583ed4bb4525bd96e50461655d2759",
+        ]
+    )
+    with pytest.raises(SPDXParsingError) as err:
+        parser.parse(document_str)
+    for file_spdx_id in file_spdx_ids:
+        assert (
+            f"Error while building contains relationship for file {file_spdx_id}, preceding package was not "
+            "parsed successfully." in err.value.get_messages()
+        )
+
+
 def test_document_with_mixed_values():
     parser = Parser()
     document_str = "\n".join(
         [
             f"SPDXID:{DOCUMENT_SPDX_ID}",
             "FileName: File without package",
             "SPDXID: SPDXRef-File",
```

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_actor_parser.py` & `spdx-tools-0.8.0a2/tests/spdx/test_actor_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_casing_tools.py` & `spdx-tools-0.8.0a2/tests/spdx/test_casing_tools.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_cli.py` & `spdx-tools-0.8.0a2/tests/spdx/test_cli.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_datetime_conversions.py` & `spdx-tools-0.8.0a2/tests/spdx/test_datetime_conversions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_document_utils.py` & `spdx-tools-0.8.0a2/tests/spdx/test_document_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/test_graph_generation.py` & `spdx-tools-0.8.0a2/tests/spdx/test_graph_generation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_actor_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_actor_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_annotation_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_annotation_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_checksum_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_checksum_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_creation_info_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_creation_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_document_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_document_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_external_document_ref_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_external_document_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_external_package_ref_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_external_package_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_extracted_licensing_info_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_extracted_licensing_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_file_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_file_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_license_expression_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_license_expression_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_package_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_package_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_package_verification_code_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_package_verification_code_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_relationship_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_relationship_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_snippet_validator.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_snippet_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_spdx_id_validators.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_spdx_id_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/validation/test_uri_validators.py` & `spdx-tools-0.8.0a2/tests/spdx/validation/test_uri_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/expected.json` & `spdx-tools-0.8.0a2/tests/spdx/writer/json/expected_results/expected.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/json/test_json_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/json/test_json_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_annotation_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_checksum_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_creation_info_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_external_document_ref_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_external_document_ref_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_file_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_license_expression_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_license_expression_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_package_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_rdf_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_relationship_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_snippet_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_writer_utils.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/rdf/test_writer_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_annotation_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_checksum_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_creation_info_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_file_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_package_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_relationship_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_snippet_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_tagvalue_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py` & `spdx-tools-0.8.0a2/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py`

 * *Files identical despite different names*

