# Comparing `tmp/thipster-0.17.7.tar.gz` & `tmp/thipster-0.17.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.7.tar", last modified: Thu Jun 22 10:15:04 2023, max compression
+gzip compressed data, was "thipster-0.17.8.tar", last modified: Thu Jun 22 12:35:35 2023, max compression
```

## Comparing `thipster-0.17.7.tar` & `thipster-0.17.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 10:15:00.000000 thipster-0.17.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 10:15:00.000000 thipster-0.17.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 10:15:04.925057 thipster-0.17.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 10:15:00.000000 thipster-0.17.7/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-22 10:15:00.000000 thipster-0.17.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 10:15:00.000000 thipster-0.17.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:15:04.925057 thipster-0.17.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-22 10:15:01.000000 thipster-0.17.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3466 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    16811 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.913057 thipster-0.17.7/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.917057 thipster-0.17.7/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5081 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.921057 thipster-0.17.7/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.921057 thipster-0.17.7/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    16910 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    21596 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22481 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.913057 thipster-0.17.7/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.444572 thipster-0.17.8/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 12:35:30.000000 thipster-0.17.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 12:35:30.000000 thipster-0.17.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 12:35:35.444572 thipster-0.17.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 12:35:30.000000 thipster-0.17.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-22 12:35:30.000000 thipster-0.17.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 12:35:30.000000 thipster-0.17.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 12:35:35.444572 thipster-0.17.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-22 12:35:31.000000 thipster-0.17.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    16811 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-22 12:35:30.000000 thipster-0.17.8/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.436571 thipster-0.17.8/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.440572 thipster-0.17.8/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.440572 thipster-0.17.8/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.440572 thipster-0.17.8/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.444572 thipster-0.17.8/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    16910 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21596 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.444572 thipster-0.17.8/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.444572 thipster-0.17.8/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22517 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-22 12:35:30.000000 thipster-0.17.8/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:35:35.440572 thipster-0.17.8/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 12:35:35.000000 thipster-0.17.8/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 12:35:35.000000 thipster-0.17.8/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 12:35:35.000000 thipster-0.17.8/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 12:35:35.000000 thipster-0.17.8/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 12:35:35.000000 thipster-0.17.8/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.7/LICENSE` & `thipster-0.17.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/PKG-INFO` & `thipster-0.17.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.7
+Version: 0.17.8
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: google
 Provides-Extra: doc
 Provides-Extra: test
-Provides-Extra: google
 Provides-Extra: dev
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.8 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
-test Provides-Extra: google Provides-Extra: dev License-File: LICENSE #
-THipster THipster is a tool dedicated to simplifying the difficulty associated
-with writing Terraform files. It allows users to write infrastructure as code
-in a simplified format, using either YAML (with JINJA) or the dedicated
-Thipster DSL. Written entirely in Python, it leverages the Python CDK for
-Terraform to create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
+doc Provides-Extra: test Provides-Extra: dev License-File: LICENSE # THipster
+THipster is a tool dedicated to simplifying the difficulty associated with
+writing Terraform files. It allows users to write infrastructure as code in a
+simplified format, using either YAML (with JINJA) or the dedicated Thipster
+DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
+create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                    versions]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.17.7/README.md` & `thipster-0.17.8/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/pyproject.toml` & `thipster-0.17.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/setup.py` & `thipster-0.17.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.17.7'
+__version__ = '0.17.8'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.7/tests/engine/test_engine.py` & `thipster-0.17.8/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/engine/test_generation.py` & `thipster-0.17.8/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.8/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.17.8/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.8/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.8/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.8/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/test_parsedfile.py` & `thipster-0.17.8/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/test_parserfactory.py` & `thipster-0.17.8/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/parser/test_yamlparser.py` & `thipster-0.17.8/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/repository/test_github_repository.py` & `thipster-0.17.8/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/repository/test_local_repository.py` & `thipster-0.17.8/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/repository/test_resourcemodel.py` & `thipster-0.17.8/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/test_e2e.py` & `thipster-0.17.8/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/tests/test_tools.py` & `thipster-0.17.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/auth/google.py` & `thipster-0.17.8/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/engine.py` & `thipster-0.17.8/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/i_parser.py` & `thipster-0.17.8/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/i_repository.py` & `thipster-0.17.8/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/i_terraform.py` & `thipster-0.17.8/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/parsed_file.py` & `thipster-0.17.8/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/engine/resource_model.py` & `thipster-0.17.8/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/helpers.py` & `thipster-0.17.8/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.8/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.8/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.8/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.8/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.8/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.8/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/token.py` & `thipster-0.17.8/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.8/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/exceptions.py` & `thipster-0.17.8/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/parser_factory.py` & `thipster-0.17.8/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/parser/yaml_parser.py` & `thipster-0.17.8/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/repository/exceptions.py` & `thipster-0.17.8/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/repository/github.py` & `thipster-0.17.8/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/repository/json.py` & `thipster-0.17.8/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/repository/local.py` & `thipster-0.17.8/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster/terraform/cdk.py` & `thipster-0.17.8/thipster/terraform/cdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,9 +728,11 @@
             resource_type=dependency_type,
         )
 
         # Creates explicit dependency
         ctx.resource_args[attribute_name] = _create_dependency(
             dep_ctx, attribute_value,
         )
+        return True
 
     ctx.resource_args[attribute_name] = CDK._created_resources[created_name]
+    return True
```

### Comparing `thipster-0.17.7/thipster/terraform/exceptions.py` & `thipster-0.17.8/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.7/thipster.egg-info/PKG-INFO` & `thipster-0.17.8/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.7
+Version: 0.17.8
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: google
 Provides-Extra: doc
 Provides-Extra: test
-Provides-Extra: google
 Provides-Extra: dev
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.8 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
-test Provides-Extra: google Provides-Extra: dev License-File: LICENSE #
-THipster THipster is a tool dedicated to simplifying the difficulty associated
-with writing Terraform files. It allows users to write infrastructure as code
-in a simplified format, using either YAML (with JINJA) or the dedicated
-Thipster DSL. Written entirely in Python, it leverages the Python CDK for
-Terraform to create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: google Provides-Extra:
+doc Provides-Extra: test Provides-Extra: dev License-File: LICENSE # THipster
+THipster is a tool dedicated to simplifying the difficulty associated with
+writing Terraform files. It allows users to write infrastructure as code in a
+simplified format, using either YAML (with JINJA) or the dedicated Thipster
+DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
+create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                    versions]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.17.7/thipster.egg-info/SOURCES.txt` & `thipster-0.17.8/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

