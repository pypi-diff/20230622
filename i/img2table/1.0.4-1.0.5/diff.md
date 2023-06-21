# Comparing `tmp/img2table-1.0.4.tar.gz` & `tmp/img2table-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-1.0.4.tar", last modified: Mon Jun 12 20:53:24 2023, max compression
+gzip compressed data, was "dist/img2table-1.0.5.tar", last modified: Wed Jun 21 22:15:37 2023, max compression
```

## Comparing `img2table-1.0.4.tar` & `img2table-1.0.5.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 20:51:11.000000 img2table-1.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-12 20:51:11.000000 img2table-1.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 20:51:11.000000 img2table-1.0.4/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 20:51:11.000000 img2table-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-12 20:51:11.000000 img2table-1.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-12 20:53:24.000000 img2table-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-12 20:51:11.000000 img2table-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 20:51:11.000000 img2table-1.0.4/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/examples/data/borderless/
--rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/borderless/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/borderless/2.png
--rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/borderless/3.png
--rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/borderless/4.png
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/borderless.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 20:51:11.000000 img2table-1.0.4/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 20:51:11.000000 img2table-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 20:51:11.000000 img2table-1.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 20:51:11.000000 img2table-1.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 20:51:11.000000 img2table-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 20:53:24.000000 img2table-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 20:51:11.000000 img2table-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/easyocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/coherency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-12 20:51:11.000000 img2table-1.0.4/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 20:53:24.000000 img2table-1.0.4/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/easyocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/easyocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/easyocr/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/easyocr/test_data/ocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/easyocr/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/easyocr/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/easyocr/test_easyocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_coherency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_rows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:24.000000 img2table-1.0.4/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 20:51:11.000000 img2table-1.0.4/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 22:13:27.000000 img2table-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-21 22:13:27.000000 img2table-1.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-21 22:15:37.000000 img2table-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-21 22:13:27.000000 img2table-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-21 22:13:27.000000 img2table-1.0.5/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/data/borderless/
+-rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 22:13:27.000000 img2table-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-21 22:13:27.000000 img2table-1.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-21 22:13:27.000000 img2table-1.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 22:13:27.000000 img2table-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 22:15:37.000000 img2table-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 22:13:27.000000 img2table-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/easyocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/ocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_easyocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_coherency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-1.0.4/LICENSE.txt` & `img2table-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/Makefile` & `img2table-1.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/PKG-INFO` & `img2table-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.4
+Version: 1.0.5
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.4 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.5 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-1.0.4/README.md` & `img2table-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/Basic_usage.ipynb` & `img2table-1.0.5/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/Implicit_rows.ipynb` & `img2table-1.0.5/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/borderless.ipynb` & `img2table-1.0.5/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/borderless/1.png` & `img2table-1.0.5/examples/data/borderless/1.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/borderless/2.png` & `img2table-1.0.5/examples/data/borderless/2.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/borderless/3.png` & `img2table-1.0.5/examples/data/borderless/3.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/borderless/4.png` & `img2table-1.0.5/examples/data/borderless/4.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/borderless.jpg` & `img2table-1.0.5/examples/data/borderless.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/implicit.png` & `img2table-1.0.5/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/tables.pdf` & `img2table-1.0.5/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/tables.png` & `img2table-1.0.5/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/data/tables.xlsx` & `img2table-1.0.5/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/examples/utils.py` & `img2table-1.0.5/examples/utils.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/setup.cfg` & `img2table-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/__init__.py` & `img2table-1.0.5/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/document/base/__init__.py` & `img2table-1.0.5/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/document/base/rotation.py` & `img2table-1.0.5/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/document/image.py` & `img2table-1.0.5/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/document/pdf.py` & `img2table-1.0.5/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/aws_textract.py` & `img2table-1.0.5/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/azure.py` & `img2table-1.0.5/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/base.py` & `img2table-1.0.5/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/data.py` & `img2table-1.0.5/src/img2table/ocr/data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/easyocr.py` & `img2table-1.0.5/src/img2table/ocr/easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/google_vision.py` & `img2table-1.0.5/src/img2table/ocr/google_vision.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 import base64
 import binascii
 import os
 from concurrent.futures import ThreadPoolExecutor
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Tuple
 
 import cv2
 import numpy as np
 import polars as pl
 import requests
 from google.cloud import vision, vision_v1
 
@@ -38,37 +38,45 @@
         :param api_key: Google Vision API key
         :param timeout: requests timeout in seconds
         """
         super(VisionEndpointContent, self).__init__(timeout=timeout)
         self.api_key = api_key
 
     @staticmethod
-    def map_response(response: Dict, page: int) -> List[Dict]:
+    def map_response(response: Dict, page: int, width: int, height: int) -> List[Dict]:
         """
         Extract test_data from API endpoint response
         :param response: json response from Google API endpoint
         :param page: page number
+        :param width: image width
+        :param height: image height
         :return: list of OCR elements
         """
         elements = list()
         for id_block, block in enumerate(response['responses'][0]['fullTextAnnotation']['pages'][0]['blocks']):
             for id_par, par in enumerate(block.get('paragraphs')):
                 id_line = 0
                 for id_word, word in enumerate(par.get('words')):
+                    # Compute x and y replacement values
+                    x_avg = np.mean([el.get('x') for el in word.get('boundingBox').get('vertices') if el.get('x')])
+                    x_repl = sorted([0, width], key=lambda val: abs(val - x_avg)).pop(0)
+                    y_avg = np.mean([el.get('y') for el in word.get('boundingBox').get('vertices') if el.get('y')])
+                    y_repl = sorted([0, height], key=lambda val: abs(val - y_avg)).pop(0)
+
                     d_el = {
                         "page": page,
                         "class": "ocrx_word",
                         "id": f"word_{id_block}_{id_par}_{id_line}_{id_word}",
                         "parent": f"line_{id_block}_{id_par}_{id_line}",
                         "value": ''.join([sym.get('text') for sym in word.get('symbols')]),
                         "confidence": round(100 * word.get('confidence')),
-                        "x1": min(map(lambda el: el.get('x'), word.get('boundingBox').get('vertices'))),
-                        "x2": max(map(lambda el: el.get('x'), word.get('boundingBox').get('vertices'))),
-                        "y1": min(map(lambda el: el.get('y'), word.get('boundingBox').get('vertices'))),
-                        "y2": max(map(lambda el: el.get('y'), word.get('boundingBox').get('vertices')))
+                        "x1": min(map(lambda el: el.get('x', x_repl), word.get('boundingBox').get('vertices'))),
+                        "x2": max(map(lambda el: el.get('x', x_repl), word.get('boundingBox').get('vertices'))),
+                        "y1": min(map(lambda el: el.get('y', y_repl), word.get('boundingBox').get('vertices'))),
+                        "y2": max(map(lambda el: el.get('y', y_repl), word.get('boundingBox').get('vertices')))
                     }
 
                     # Check for break
                     _break = word.get('symbols')[-1].get('property', {}).get('detectedBreak', {}).get('type')
 
                     # Apply breaks
                     if _break in ['EOL_SURE_SPACE', 'LINE_BREAK']:
@@ -104,15 +112,15 @@
         # Post to API
         req = requests.post(url="https://vision.googleapis.com/v1/images:annotate",
                             json=payload,
                             params={"key": self.api_key},
                             timeout=self.timeout)
         response = req.json()
 
-        return self.map_response(response=response, page=page)
+        return self.map_response(response=response, page=page, width=img.shape[1], height=img.shape[0])
 
     def get_content(self, document: Document) -> List[List[Dict]]:
         """
         Get OCR content corresponding to document
         :param document: Document object
         :return: list of OCR elements by page
         """
@@ -132,38 +140,64 @@
         Document content class from Google Vision using direct requests to endpoint
         :param timeout: requests timeout in seconds
         """
         super(VisionAPIContent, self).__init__(timeout=timeout)
         self.client = vision.ImageAnnotatorClient()
 
     @staticmethod
-    def map_response(response: vision_v1.types.BatchAnnotateImagesResponse) -> List[List[Dict]]:
+    def map_response(response: vision_v1.types.BatchAnnotateImagesResponse,
+                     shapes: List[Tuple[int, int]]) -> List[List[Dict]]:
         """
         Extract data from API endpoint response object
         :param response: API endpoint response object
+        :param shapes: list of images shapes
         :return: list of OCR elements by pages
         """
         elements = list()
         for id_page, page in enumerate(response.responses):
+            # Get image shape
+            height, width = shapes[id_page]
+
             page_elements = list()
             for id_block, block in enumerate(page.full_text_annotation.pages[0].blocks):
                 for id_par, par in enumerate(block.paragraphs):
                     id_line = 0
                     for id_word, word in enumerate(par.words):
+                        # Compute x and y replacement values
+                        x_avg = np.mean([el.x for el in word.bounding_box.vertices if hasattr(el, 'x')])
+                        x_repl = sorted([0, width], key=lambda val: abs(val - x_avg)).pop(0)
+                        y_avg = np.mean([el.y for el in word.bounding_box.vertices if hasattr(el, 'y')])
+                        y_repl = sorted([0, height], key=lambda val: abs(val - y_avg)).pop(0)
+
+                        # Compute x and y values in bounding box
+                        x_vals = list()
+                        for vertex in word.bounding_box.vertices:
+                            try:
+                                x_vals.append(vertex.x or x_repl)
+                            except AttributeError:
+                                x_vals.append(x_repl)
+
+                        y_vals = list()
+                        for vertex in word.bounding_box.vertices:
+                            try:
+                                y_vals.append(vertex.y or y_repl)
+                            except AttributeError:
+                                y_vals.append(y_repl)
+
                         d_el = {
                             "page": id_page,
                             "class": "ocrx_word",
                             "id": f"word_{id_block}_{id_par}_{id_line}_{id_word}",
                             "parent": f"line_{id_block}_{id_par}_{id_line}",
                             "value": ''.join([sym.text for sym in word.symbols]),
                             "confidence": round(100 * word.confidence),
-                            "x1": min(map(lambda el: el.x, word.bounding_box.vertices)),
-                            "x2": max(map(lambda el: el.x, word.bounding_box.vertices)),
-                            "y1": min(map(lambda el: el.y, word.bounding_box.vertices)),
-                            "y2": max(map(lambda el: el.y, word.bounding_box.vertices))
+                            "x1": min(x_vals),
+                            "x2": max(x_vals),
+                            "y1": min(y_vals),
+                            "y2": max(y_vals)
                         }
 
                         # Check for break
                         _break = word.symbols[-1].property.detected_break.type
 
                         # Apply breaks
                         if _break in [vision_v1.TextAnnotation.DetectedBreak.BreakType.EOL_SURE_SPACE,
@@ -181,32 +215,34 @@
 
     def get_content(self, document: Document) -> List[List[Dict]]:
         """
         Get OCR content corresponding to document
         :param document: Document object
         :return: list of OCR elements by page
         """
-        reqs = list()
+        reqs, shapes = list(), list()
         for img in document.images:
             # Create image object
             image = vision_v1.Image()
             image.content = binascii.a2b_base64(self.img_to_b64(img=img))
 
+            shapes.append(img.shape[:2])
+
             # Create request
             request = vision_v1.AnnotateImageRequest()
             request.image = image
             request.features = [{"type_": vision_v1.Feature.Type.DOCUMENT_TEXT_DETECTION}]
 
             reqs.append(request)
 
         # Call API
         result = self.client.batch_annotate_images(requests=reqs,
                                                    timeout=self.timeout)
 
-        return self.map_response(response=result)
+        return self.map_response(response=result, shapes=shapes)
 
 
 class VisionOCR(OCRInstance):
     """
     Google Vision OCR instance
     """
```

### Comparing `img2table-1.0.4/src/img2table/ocr/paddle.py` & `img2table-1.0.5/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/pdf.py` & `img2table-1.0.5/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/ocr/tesseract.py` & `img2table-1.0.5/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/__init__.py` & `img2table-1.0.5/src/img2table/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/image.py` & `img2table-1.0.5/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/metrics.py` & `img2table-1.0.5/src/img2table/tables/metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/objects/__init__.py` & `img2table-1.0.5/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/objects/extraction.py` & `img2table-1.0.5/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/objects/line.py` & `img2table-1.0.5/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/objects/row.py` & `img2table-1.0.5/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/objects/table.py` & `img2table-1.0.5/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     # Get threshold on image and binary image
     blur = cv2.GaussianBlur(img, (3, 3), 0)
     thresh = cv2.adaptiveThreshold(blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
     binary_thresh = cv2.adaptiveThreshold(255 - blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
 
     # Mask on areas with dark background
-    blur_size = max(int(2 * char_length) + 1 - int(2 * char_length) % 2, 1) if char_length else 11
+    blur_size = min(255, max(int(2 * char_length) + 1 - int(2 * char_length) % 2, 1) if char_length else 11)
     blur = cv2.medianBlur(img, blur_size)
     mask = cv2.inRange(blur, 0, 100)
 
     # Get contours of dark areas
     contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # For each dark area, use binary threshold instead of regular threshold
```

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/coherency.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/common.py` & `img2table-1.0.5/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/prepare_image.py` & `img2table-1.0.5/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table/tables/processing/text/titles.py` & `img2table-1.0.5/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/src/img2table.egg-info/PKG-INFO` & `img2table-1.0.5/src/img2table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.4
+Version: 1.0.5
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.4 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.5 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-1.0.4/src/img2table.egg-info/SOURCES.txt` & `img2table-1.0.5/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/_mock_data/azure.pkl` & `img2table-1.0.5/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/_mock_data/tesseract_hocr.html` & `img2table-1.0.5/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/_mock_data/textract.json` & `img2table-1.0.5/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/_mock_data/vision.json` & `img2table-1.0.5/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/_mock_data/vision.pkl` & `img2table-1.0.5/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/conftest.py` & `img2table-1.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/base/test_data/test.png` & `img2table-1.0.5/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/base/test_rotation.py` & `img2table-1.0.5/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/image/test_data/blank.png` & `img2table-1.0.5/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/image/test_data/dark.png` & `img2table-1.0.5/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/image/test_data/expected.xlsx` & `img2table-1.0.5/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/image/test_data/test.png` & `img2table-1.0.5/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/image/test_image.py` & `img2table-1.0.5/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/pdf/test_data/test.pdf` & `img2table-1.0.5/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/document/pdf/test_pdf.py` & `img2table-1.0.5/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-1.0.5/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/aws_textract/test_data/content.json` & `img2table-1.0.5/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/aws_textract/test_data/test.png` & `img2table-1.0.5/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/azure/test_azure.py` & `img2table-1.0.5/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/azure/test_data/test.png` & `img2table-1.0.5/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/data/test_data/expected_table.json` & `img2table-1.0.5/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/data/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/data/test_ocr_data.py` & `img2table-1.0.5/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/easyocr/test_data/ocr.json` & `img2table-1.0.5/tests/ocr/easyocr/test_data/ocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/easyocr/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/easyocr/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/easyocr/test_data/test.png` & `img2table-1.0.5/tests/ocr/easyocr/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/easyocr/test_easyocr.py` & `img2table-1.0.5/tests/ocr/easyocr/test_easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-1.0.5/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/google_vision/test_data/test.png` & `img2table-1.0.5/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/google_vision/test_google_vision.py` & `img2table-1.0.5/tests/ocr/google_vision/test_google_vision.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with open("test_data/expected_content.json", "r") as f:
         expected = json.load(f)
 
     # Test for map_response method
     with open(os.path.join(MOCK_DIR, "vision.json"), "r") as f:
         response = json.load(f)
 
-    result_map_response = content.map_response(response=response, page=0)
+    result_map_response = content.map_response(response=response, page=0, height=417, width=1365)
     assert result_map_response == expected[0]
 
     # Test for get_content method
     result_get_content = content.get_content(document=image)
     assert result_get_content == expected
 
 
@@ -38,15 +38,15 @@
     with open("test_data/expected_content.json", "r") as f:
         expected = json.load(f)
 
     # Test for map_response method
     with open(os.path.join(MOCK_DIR, "vision.pkl"), "rb") as f:
         response = pickle.load(f)
 
-    result_map_response = content.map_response(response=response)
+    result_map_response = content.map_response(response=response, shapes=[(417, 1365)])
     assert result_map_response == expected
 
     # Test for get_content method
     result_get_content = content.get_content(document=image)
     assert result_get_content == expected
```

### Comparing `img2table-1.0.4/tests/ocr/paddle/test_data/hocr.json` & `img2table-1.0.5/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/paddle/test_data/test.png` & `img2table-1.0.5/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/paddle/test_paddle.py` & `img2table-1.0.5/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/pdf/test_data/content.json` & `img2table-1.0.5/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/pdf/test_data/test.pdf` & `img2table-1.0.5/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-1.0.5/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-1.0.5/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/tesseract/test_data/test.png` & `img2table-1.0.5/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/ocr/tesseract/test_tesseract.py` & `img2table-1.0.5/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/image/test_data/blank.png` & `img2table-1.0.5/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/image/test_data/ocr.csv` & `img2table-1.0.5/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/image/test_data/test.png` & `img2table-1.0.5/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/image/test_image.py` & `img2table-1.0.5/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/image/test_metrics.py` & `img2table-1.0.5/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_data/expected_tables.json` & `img2table-1.0.5/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_data/ocr.csv` & `img2table-1.0.5/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_data/tables.json` & `img2table-1.0.5/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_extraction.py` & `img2table-1.0.5/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_line.py` & `img2table-1.0.5/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_row.py` & `img2table-1.0.5/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/objects/test_table.py` & `img2table-1.0.5/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png` & `img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json` & `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_coherency.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json` & `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_data/rows.json` & `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/rows/test_rows.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json` & `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_data/rows.json` & `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/common/test_common.py` & `img2table-1.0.5/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/common/test_data/test.jpg` & `img2table-1.0.5/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-1.0.5/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/text/test_data/ocr.csv` & `img2table-1.0.5/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/text/test_data/table.json` & `img2table-1.0.5/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/text/test_data/test.jpg` & `img2table-1.0.5/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.4/tests/tables/processing/text/test_titles.py` & `img2table-1.0.5/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

