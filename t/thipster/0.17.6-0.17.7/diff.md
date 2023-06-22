# Comparing `tmp/thipster-0.17.6.tar.gz` & `tmp/thipster-0.17.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.6.tar", last modified: Thu Jun 22 08:45:33 2023, max compression
+gzip compressed data, was "thipster-0.17.7.tar", last modified: Thu Jun 22 10:15:04 2023, max compression
```

## Comparing `thipster-0.17.6.tar` & `thipster-0.17.7.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 08:45:29.000000 thipster-0.17.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 08:45:29.000000 thipster-0.17.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 08:45:33.252659 thipster-0.17.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 08:45:29.000000 thipster-0.17.6/README.md
--rw-r--r--   0 root         (0) root         (0)      995 2023-06-22 08:45:29.000000 thipster-0.17.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 08:45:29.000000 thipster-0.17.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 08:45:33.252659 thipster-0.17.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-22 08:45:29.000000 thipster-0.17.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    15280 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    13619 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_yamlparser.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3105 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9180 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13507 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17026 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20074 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21404 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 10:15:00.000000 thipster-0.17.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 10:15:00.000000 thipster-0.17.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 10:15:04.925057 thipster-0.17.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 10:15:00.000000 thipster-0.17.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-22 10:15:00.000000 thipster-0.17.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 10:15:00.000000 thipster-0.17.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:15:04.925057 thipster-0.17.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-22 10:15:01.000000 thipster-0.17.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.905057 thipster-0.17.7/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    16811 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-22 10:15:00.000000 thipster-0.17.7/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.909057 thipster-0.17.7/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.913057 thipster-0.17.7/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.917057 thipster-0.17.7/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.921057 thipster-0.17.7/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.921057 thipster-0.17.7/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    16910 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21596 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.925057 thipster-0.17.7/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22481 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-22 10:15:00.000000 thipster-0.17.7/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:15:04.913057 thipster-0.17.7/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 10:15:04.000000 thipster-0.17.7/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.6/LICENSE` & `thipster-0.17.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.6/PKG-INFO` & `thipster-0.17.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.6
+Version: 0.17.7
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: test
 Provides-Extra: google
+Provides-Extra: dev
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.7 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-dev Provides-Extra: doc Provides-Extra: google License-File: LICENSE # THipster
-THipster is a tool dedicated to simplifying the difficulty associated with
-writing Terraform files. It allows users to write infrastructure as code in a
-simplified format, using either YAML (with JINJA) or the dedicated Thipster
-DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
-create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
+test Provides-Extra: google Provides-Extra: dev License-File: LICENSE #
+THipster THipster is a tool dedicated to simplifying the difficulty associated
+with writing Terraform files. It allows users to write infrastructure as code
+in a simplified format, using either YAML (with JINJA) or the dedicated
+Thipster DSL. Written entirely in Python, it leverages the Python CDK for
+Terraform to create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                    versions]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.17.6/README.md` & `thipster-0.17.7/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.6/pyproject.toml` & `thipster-0.17.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -34,8 +34,34 @@
     "F",
     "E",
     "W",
     "I",
     "UP",
     "C90",
     "N",
+    "D",
+    "A",
+    "C4",
+    "EM",
+    "EXE",
+    "ISC",
+    "ICN",
+    "INP",
+    "PYI",
+    "PTH",
+    "Q",
+    "RSE",
+    "RET",
+    "SIM",
+    "TID",
+    "ARG",
+    "RUF",
 ]
+
+[tool.ruff.pydocstyle]
+# Use Google-style docstrings.
+convention = "numpy"
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
+inline-quotes = "single"
+multiline-quotes = "double"
```

### Comparing `thipster-0.17.6/tests/engine/test_generation.py` & `thipster-0.17.7/tests/engine/test_generation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+"""Test the generation of Terraform files."""
 import uuid
 
 import pytest
 
-from thipster.terraform.exceptions import (
-    CDKCyclicDependenciesError,
-    CDKDependencyNotDeclaredError,
-    CDKMissingAttributeInDependencyError,
-)
-
-from ..test_tools import (
+from tests.test_tools import (
     assert_number_of_resource_type_is,
     assert_resource_created,
     get_function_name,
     get_resource_parameter,
     process_file,
 )
+from thipster.terraform.exceptions import (
+    CDKCyclicDependenciesError,
+    CDKDependencyNotDeclaredError,
+    CDKMissingAttributeInDependencyError,
+)
 
 
 def test_empty_bucket():
+    """Test the generation of an empty bucket."""
     function_name = get_function_name()
 
     bucket_name = f'empty-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
 bucket {bucket_name}:
@@ -34,14 +35,15 @@
     assert_number_of_resource_type_is('google_storage_bucket', 1)
     assert_resource_created('google_storage_bucket', bucket_name)
 
     clean_up()
 
 
 def test_empty_bucket_two():
+    """Test the generation of two buckets (one is empty)."""
     function_name = get_function_name()
 
     empty_bucket_name = f'empty-bucket-{uuid.uuid4().int}'
     bucket_name = f'empty-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
@@ -58,14 +60,15 @@
     assert_resource_created('google_storage_bucket', empty_bucket_name)
     assert_resource_created('google_storage_bucket', bucket_name)
 
     clean_up()
 
 
 def test_dep_with_no_options():
+    """Test the generation of a bucket with a missing attribute in its dependency."""
     function_name = get_function_name()
 
     with pytest.raises(CDKMissingAttributeInDependencyError):
         clean_up = process_file(
             directory=function_name,
             file="""
 bucket_bad_dep_parent my-bucket:
@@ -74,14 +77,15 @@
             mock_auth=True,
         )
 
         clean_up()
 
 
 def test_cyclic_deps():
+    """Test the generation of a bucket with a cyclic dependency."""
     function_name = get_function_name()
 
     with pytest.raises(CDKCyclicDependenciesError):
         clean_up = process_file(
             directory=function_name,
             file="""
 bucket_bad_dep_cyclic my-bucket:
@@ -90,14 +94,15 @@
             mock_auth=True,
         )
 
         clean_up()
 
 
 def test_default_internal_object():
+    """Test the generation of a firewall with default internal objects."""
     function_name = get_function_name()
 
     clean_up = process_file(
         directory=function_name,
         file="""
 firewall testparent:
 \tdirection: EGRESS
@@ -105,14 +110,15 @@
         mock_auth=True,
     )
 
     clean_up()
 
 
 def test_explicit_internal_object():
+    """Test the generation of a firewall with explicit internal objects."""
     function_name = get_function_name()
     clean_up = process_file(
         directory=function_name,
         file="""
 firewall testparent:
 \tdirection: EGRESS
 
@@ -122,14 +128,15 @@
         mock_auth=True,
     )
 
     clean_up()
 
 
 def test_missing_explicit_dependency():
+    """Test the generation of a subnetwork with a missing explicit dependency."""
     function_name = get_function_name()
 
     with pytest.raises(CDKDependencyNotDeclaredError):
         clean_up = process_file(
             directory=function_name,
             file="""
 subnetwork lb-subnet:
@@ -140,14 +147,15 @@
             mock_auth=True,
         )
 
         clean_up()
 
 
 def test_explicit_dependency():
+    """Test the generation of a subnetwork with an explicit dependency."""
     function_name = get_function_name()
 
     clean_up = process_file(
         directory=function_name,
         file="""
 network lb-net:
 
@@ -159,14 +167,15 @@
         mock_auth=True,
     )
 
     clean_up()
 
 
 def test_bucket_cors():
+    """Test the generation of a bucket with cors."""
     function_name = get_function_name()
 
     bucket_name = f'cors-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
 bucket {bucket_name}:
@@ -186,14 +195,15 @@
     assert_number_of_resource_type_is('google_storage_bucket', 1)
     assert_resource_created('google_storage_bucket', bucket_name)
 
     clean_up()
 
 
 def test_bucket_two_cors():
+    """Test the generation of a bucket with two cors."""
     function_name = get_function_name()
 
     bucket_name = f'cors-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
 bucket:
@@ -225,14 +235,15 @@
 
     assert len(cors_block) == 2
 
     clean_up()
 
 
 def test_subnetwork_in_network():
+    """Test the generation of multiple subnetworks in a network."""
     function_name = get_function_name()
 
     network_name = f'network-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
 network:
```

### Comparing `thipster-0.17.6/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.7/tests/parser/dsl_parser/test_ast.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+"""Test the AST of the DSL parser."""
 import thipster.parser.dsl_parser.ast as ast
 from thipster.engine.parsed_file import Position
 from thipster.parser.dsl_parser.token import Token
 
 
 def test_create_ast():
+    """Test the creation of an AST."""
     # bucket nom-#test \n\t toto: tata
     tree = ast.FileNode()
 
     tree.add(
         ast.ResourceNode(
             resource_type=ast.StringNode(
                 Token(Position('file', 1, 1), 'STRING', 'bucket'),
```

### Comparing `thipster-0.17.6/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.17.7/tests/parser/dsl_parser/test_dslparser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import os
+"""Tests for the DSLParser class."""
+from pathlib import Path
 
 import pytest
 
 import thipster.engine.parsed_file as pf
+from tests.test_tools import create_dir
 from thipster.parser import DSLParser
 from thipster.parser.dsl_parser.exceptions import (
     DSLArithmeticError,
     DSLConditionError,
     DSLParserPathNotFoundError,
     DSLSyntaxError,
     DSLUnexpectedEOFError,
 )
 from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 
-from ...test_tools import create_dir
-
 
 def test_get_files():
+    """Test the getfiles method."""
     path_input = 'test'
     _destroy_dir = create_dir(
         path_input,
         {f'test_file{i}.thips': 'content' for i in range(1, 4)},
     )
 
     parser = DSLParser
@@ -34,14 +35,15 @@
         assert 'test_file' in k
         assert v == 'content'
 
     _destroy_dir()
 
 
 def test_get_absent_files():
+    """Test the getfiles method with an inexistant path."""
     with pytest.raises(DSLParserPathNotFoundError):
 
         parser = DSLParser
         parser._DSLParser__getfiles('inexistant_path')
 
 
 def __test_file(file: str):
@@ -64,14 +66,15 @@
     finally:
         _destroy_dir()
 
     return output
 
 
 def test_parse_simple_file():
+    """Test the parsing of a simple file."""
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: euw
 """,
     )
 
     assert len(out.resources) == 1
@@ -84,22 +87,24 @@
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'euw'
 
 
 def test_parse_empty_file():
+    """Test the parsing of an empty file."""
     out = __test_file(
         file="""""",
     )
 
     assert len(out.resources) == 0
 
 
 def test_parse_simple_file_with_newlines():
+    """Test the parsing of a simple file with newlines."""
     out = __test_file(
         file="""
 
 bucket my-bucket:
 
 
 \tregion: euw
@@ -119,14 +124,15 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == 'euw'
 
 
 def test_parse_simple_file_with_empty_lines():
+    """Test the parsing of a simple file with empty lines."""
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: euw
 \t
 bucket my-bucket2:
 \tregion: euw
 \t\t
@@ -141,14 +147,15 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == 'euw'
 
 
 def test_parse_list():
+    """Test the parsing of a list."""
     out = __test_file(
         file="""bucket my-bucket:
 \tregion:
 \t\t- toto
 \t\t- titi
 \t\t- tata
 """,
@@ -200,14 +207,15 @@
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert isinstance(region._ParsedAttribute__value, pf.ParsedList)
     assert len(region.value) == 0
 
 
 def test_parse_dict_list_in_dict():
+    """Test the parsing of a list and dict in a dict."""
     out = __test_file(
         file="""bucket my-bucket:
 \ttoto:
 \t\t aaa: val1
 \t\t bbb: val2
 \ttata:
 \t\t- ccc
@@ -227,14 +235,15 @@
     assert isinstance(toto._ParsedAttribute__value, pf.ParsedDict)
     tata = bucket.attributes[1]
     assert tata.name == 'tata'
     assert isinstance(tata._ParsedAttribute__value, pf.ParsedList)
 
 
 def test_parse_if_else():
+    """Test the parsing of if else statements."""
     # IN DICT
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: euw if 1 == 1 else us
 """,
     )
 
@@ -288,14 +297,15 @@
 
     assert len(region.value) == 1
     r = region.value[0]
     assert r.value == 'euw'
 
 
 def test_parse_literal_types():
+    """Test the parsing of literal types."""
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: euw
 """,
     )
 
     assert len(out.resources) == 1
@@ -358,14 +368,15 @@
 
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert region.value is True
 
 
 def test_parse_amount():
+    """Test the parsing of an amount."""
     out = __test_file(
         file="""bucket my-bucket: amount: 3
 \tregion: euw
 """,
     )
 
     assert len(out.resources) == 3
@@ -392,14 +403,15 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == i
 
 
 def test_var_in_name():
+    """Test the parsing of a variable in a name."""
     out = __test_file(
         file="""bucket my-bucket#i: amount: 3 #i
 \tregion: #i
 """,
     )
 
     assert len(out.resources) == 3
@@ -410,14 +422,15 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == i
 
 
 def test_comparisons():
+    """Test the parsing of operator comparisons."""
     def test_cmp(cmp_expr: str, result: str):
         out = __test_file(
             file=f"""bucket my-bucket:
 \tregion: truCase if {cmp_expr} else falsCase
 """,
         )
 
@@ -456,14 +469,15 @@
 
     # NE
     test_cmp('3!=2', 'truCase')
     test_cmp('2!=2', 'falsCase')
 
 
 def test_arithmetic():
+    """Test the parsing of arithmetic expressions."""
     # PLUS
     out = __test_file(
         file="""bucket my-bucket:
 \tvalue: -1+1-3
 """,
     )
 
@@ -528,170 +542,195 @@
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'value'
     assert region.value == 16
 
 
-def __test_parser_raises(mocker, input: str, exception: Exception)\
-        -> pytest.ExceptionInfo:
+def __test_parser_raises(
+    mocker,  # noqa: ARG001
+    input_file: str,
+    exception: Exception,
+) -> pytest.ExceptionInfo:
     with pytest.raises(exception) as exc_info:
         __test_file(
-            file=input,
+            file=input_file,
         )
 
     return exc_info
 
 
 def __test_syntax_error(
-    mocker, input: str, ln: int, col: int,
+    mocker, input_file: str, ln: int, col: int,
     expected: str, got: str,
 ):
 
-    exc_info = __test_parser_raises(mocker, input, DSLSyntaxError)
+    exc_info = __test_parser_raises(
+        mocker,
+        input_file,
+        DSLSyntaxError,
+    )
 
     exp = str(' or '.join(list(map(str, expected))))\
         if isinstance(expected, list) else str(expected.value)
 
     assert str(exc_info.value) == f'(File : \
-{os.getcwd()}/test/test_file.thips, Ln {str(ln)}, Col {str(col)}) :\n\t\
-Syntax error : Expected {exp}, got {str(got.value)}'
+{Path.cwd()}/test/test_file.thips, Ln {ln!s}, Col {col!s}) :\n\t\
+Syntax error : Expected {exp}, got {got.value!s}'
 
 
 def test_syntax_error_resource(mocker):
-    # MISSING NAME
-    input = """bucket :
+    """Test the syntax errors in a resource missing its name."""
+    input_file = """bucket :
             """
     __test_syntax_error(
-        mocker, input=input, ln=1, col=8,
+        mocker, input_file=input_file, ln=1, col=8,
         expected=[TT.STRING, TT.VAR], got=TT.COLON,
     )
 
 
 def test_syntax_error_dict(mocker):
+    """Test the syntax errors associated with a dict."""
     # MISSING COLON
-    input = """
+    input_file = """
 bucket my-bucket:
 \tregion euw
             """
     __test_syntax_error(
-        mocker, input=input, ln=3, col=9,
+        mocker, input_file=input_file, ln=3, col=9,
         expected=TT.COLON, got=TT.STRING,
     )
 
     # MISSING TAB
-    input = """
+    input_file = """
 bucket my-bucket:
 region: euw
             """
     __test_syntax_error(
-        mocker, input=input, ln=3, col=1,
+        mocker, input_file=input_file, ln=3, col=1,
         expected=TT.TAB, got=TT.STRING,
     )
 
     # MISSING VALUE
-    input = """
+    input_file = """
 bucket my-bucket:
 \ttest:
 \tregion: euw
 """
     __test_syntax_error(
-        mocker, input=input, ln=3, col=7,
+        mocker, input_file=input_file, ln=3, col=7,
         expected=TT.STRING, got=TT.NEWLINE,
     )
 
     # MISSING VALUE 2
-    input = """
+    input_file = """
 bucket my-bucket:
 \ttest:
 
 
 
 
 
 """
     exc_info = __test_parser_raises(
-        mocker, input=input, exception=DSLUnexpectedEOFError,
+        mocker, input_file=input_file, exception=DSLUnexpectedEOFError,
     )
 
     assert str(exc_info.value) == 'Unexpected EOF'
 
 
 def test_syntax_error_amount(mocker):
+    """Test the syntax errors in an amount declaration."""
     # MISSING COLON
-    input = """
+    input_file = """
 bucket my-bucket: amount 3
 \tregion: euw
 """
     __test_syntax_error(
-        mocker, input=input, ln=2, col=26,
+        mocker, input_file=input_file, ln=2, col=26,
         expected=TT.COLON, got=TT.INT,
     )
 
     # NO INTEGER
-    input = """
+    input_file = """
 bucket my-bucket: amount: str
 \tregion: euw
 """
     __test_syntax_error(
-        mocker, input=input, ln=2, col=27,
+        mocker, input_file=input_file, ln=2, col=27,
         expected=[TT.INT, TT.FLOAT, TT.PARENTHESES_START], got=TT.STRING,
     )
 
 
 def test_syntax_error_if(mocker):
+    """Test the syntax errors in an if statement."""
     # MISSING CONDITION
-    input = """
+    input_file = """
 bucket my-bucket: if
 """
-    __test_parser_raises(mocker, input=input, exception=DSLConditionError)
+    __test_parser_raises(
+        mocker,
+        input_file=input_file,
+        exception=DSLConditionError,
+    )
 
     # UNEXPECTED IF ELSE
-    input = """
+    input_file = """
 bucket my-bucket: if 1 == 1 else bbb
 """
     __test_syntax_error(
-        mocker, input=input, ln=2, col=29,
+        mocker, input_file=input_file, ln=2, col=29,
         expected=TT.NEWLINE, got=TT.ELSE,
     )
 
 
 def test_syntax_error_if_else(mocker):
+    """Test the syntax errors in an if else statement."""
     # MISSING ELSE VALUE
-    input = """
+    input_file = """
 bucket my-bucket:
 \ttoto:
 \t\tfoo : bar if true else
 """
     __test_syntax_error(
-        mocker, input=input, ln=4, col=25,
+        mocker, input_file=input_file, ln=4, col=25,
         expected=[TT.INT, TT.FLOAT, TT.PARENTHESES_START], got=TT.NEWLINE,
     )
 
     # MISSING CONDITION VALUE
-    input = """
+    input_file = """
 bucket my-bucket:
 \ttoto:
 \t\tfoo : bar if  else bbb
 """
-    __test_parser_raises(mocker, input=input, exception=DSLConditionError)
+    __test_parser_raises(
+        mocker,
+        input_file=input_file,
+        exception=DSLConditionError,
+    )
 
 
 def test_syntax_error_unexpected_token(mocker):
+    """Test the syntax error with an unexpected 'if' as token name."""
     # RESERVED TOKEN NAME
-    input = """
+    input_file = """
 bucket if:
 \tregion: euw
 """
     __test_syntax_error(
-        mocker, input=input, ln=2, col=8,
+        mocker, input_file=input_file, ln=2, col=8,
         expected=[TT.STRING, TT.VAR], got=TT.IF,
     )
 
 
 def test_amount_error(mocker):
+    """Test the syntax error with an unexpected 'amount' value : 3/2 isn't an int."""
     # RESERVED TOKEN NAME
-    input = """
+    input_file = """
 bucket my-bucket: amount: 3/2
 \tregion: euw
 """
-    __test_parser_raises(mocker, input=input, exception=DSLArithmeticError)
+    __test_parser_raises(
+        mocker,
+        input_file=input_file,
+        exception=DSLArithmeticError,
+    )
```

### Comparing `thipster-0.17.6/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.7/tests/parser/dsl_parser/test_lexer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Tests for the THipster DSL lexer module."""
 import pytest
 
 from thipster.parser.dsl_parser.exceptions import DSLParserNoEndingQuotesError
 from thipster.parser.dsl_parser.lexer import Lexer
 from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 
 
@@ -17,341 +18,366 @@
     if value:
         token_str += f', Value: {value}'
     token_str += ')'
     return token_str
 
 
 def __single_token_test(
-    input: str,
+    input_string: str,
     token: str,
     token_value: str | None = None,
     is_newline: bool = False,
 ):
-
-    line_value, column_value = 1, len(input)+1
+    test_file_name = 'test_file.thips'
+    line_value, column_value = 1, len(input_string)+1
     if is_newline:
         line_value, column_value = 2, 1
     expected_output = [
-        __get_token_string('test_file.thips', 1, 1, token, token_value),
+        __get_token_string(test_file_name, 1, 1, token, token_value),
         __get_token_string(
-            'test_file.thips', line_value,
+            test_file_name, line_value,
             column_value, TT.NEWLINE,
         ),
-        __get_token_string('test_file.thips', line_value+1, 1, TT.EOF),
+        __get_token_string(test_file_name, line_value+1, 1, TT.EOF),
     ]
-    lexer = Lexer({'test_file.thips': input})
+    lexer = Lexer({test_file_name: input_string})
     lexer.run()
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_create_lexer():
+    """Test the creation of a Lexer object."""
     files = {
         'file_name_1': 'file_content_1',
         'file_name_2': 'file_content_2',
     }
     lexer = Lexer(files)
 
     assert isinstance(lexer, Lexer)
     assert lexer.files == files
     assert len(lexer.tokenList) == 0
 
 
 def test_lex_single_tokens():
-    for input, output in {
+    """Test the lexing of single characters."""
+    for input_char, output in {
         ':': TT.COLON,
         ',': TT.COMMA,
         '+': TT.PLUS,
         '-': TT.MINUS,
         '=': TT.EQ,
         '*': TT.MUL,
         '/': TT.DIV,
         '!': TT.EXCLAMATION,
         '<': TT.LT,
         '>': TT.GT,
         '^': TT.POW,
     }.items():
-        __single_token_test(input, output)
+        __single_token_test(input_char, output)
 
 
 def test_lex_brackets():
+    """Test the lexing of brackets."""
     lexer = Lexer({'': ''})
-    input = '[toto]'
+    input_string = '[toto]'
     expected_output = [
         __get_token_string('file', 1, 1, TT.BRACKETS_START),
         __get_token_string('file', 1, 2, TT.STRING, 'toto'),
         __get_token_string('file', 1, 6, TT.BRACKETS_END),
         __get_token_string('file', 1, 7, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_quoted_string():
+    """Test the lexing of quoted strings."""
     lexer = Lexer({'': ''})
 
-    input = '"bucket number 21""bucket number 22"'
+    input_string = '"bucket number 21""bucket number 22"'
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number 21'),
         __get_token_string('file', 1, 20, TT.STRING, 'bucket number 22'),
         __get_token_string('file', 1, 37, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
-    input = "'bucket number 21'"
+    input_string = "'bucket number 21'"
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number 21'),
         __get_token_string('file', 1, 19, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
-    input = "'bucket number \"21\"'"
+    input_string = "'bucket number \"21\"'"
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, 'bucket number "21"'),
         __get_token_string('file', 1, 21, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
     lexer = Lexer({'': ''})
-    input = '"bucket number \'21\'"'
+    input_string = '"bucket number \'21\'"'
     expected_output = [
         __get_token_string('file', 1, 2, TT.STRING, "bucket number '21'"),
         __get_token_string('file', 1, 21, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_quoted_string_error():
-    input = {
+    """Test lexing of string with no ending quotes."""
+    input_file = {
         'file': 'bucket nom-8: "amount: 5 \n\t',
     }
-    lexer = Lexer(input)
+    lexer = Lexer(input_file)
     with pytest.raises(DSLParserNoEndingQuotesError):
         lexer.run()
 
 
 def test_lex_multiline_input():
-    input = {
+    """Test the lexing of multiline input."""
+    input_file = {
         'file': 'bucket nom\\\ntest:',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nomtest'),
         __get_token_string('file', 2, 5, TT.COLON),
         __get_token_string('file', 2, 6, TT.NEWLINE),
         __get_token_string('file', 3, 1, TT.EOF),
     ]
-    lexer = Lexer(input)
+    lexer = Lexer(input_file)
     lexer.run()
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_var():
-    input = '#variable'
+    """Test the lexing of a variable."""
+    input_string = '#variable'
     expected_output = [
         __get_token_string('file', 1, 2, TT.VAR, 'variable'),
         __get_token_string('file', 1, 10, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
     lexer = Lexer({'': ''})
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_newline():
+    """Test the lexing of a newline."""
     __single_token_test('\n', TT.NEWLINE, is_newline=True)
 
 
 def test_lex_tab():
+    """Test the lexing of a tab."""
     __single_token_test('\t', TT.TAB)
 
 
 def test_lex_4_whitespaces_as_tab():
-    input = {
+    """Test if 4 whitespaces are considered as a tab."""
+    input_file = {
         'file': '    \n\t',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.TAB),
         __get_token_string('file', 1, 5, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
         __get_token_string('file', 2, 2, TT.NEWLINE),
         __get_token_string('file', 3, 1, TT.EOF),
     ]
-    lexer = Lexer(input)
+    lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_2_4_whitespaces_as_tabs():
-    input = {
+    """Test if 2*4 whitespaces are considered as 2 tabs."""
+    input_file = {
         'file': '        \n\t',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.TAB),
         __get_token_string('file', 1, 5, TT.TAB),
         __get_token_string('file', 1, 9, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.TAB),
         __get_token_string('file', 2, 2, TT.NEWLINE),
         __get_token_string('file', 3, 1, TT.EOF),
     ]
-    lexer = Lexer(input)
+    lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_dash():
+    """Test the lexing of a dash."""
     __single_token_test('-', TT.MINUS)
 
 
 def test_lex_amount():
-    input = 'amount '
+    """Test the lexing of an amount."""
+    input_string = 'amount '
     expected_output = [
         __get_token_string('file', 1, 1, TT.AMOUNT),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
     lexer = Lexer({'': ''})
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_and():
+    """Test the lexing of an 'and' string."""
     __single_token_test('and', TT.AND)
 
 
 def test_lex_if():
+    """Test the lexing of an 'if' string."""
     __single_token_test('if', TT.IF)
 
 
 def test_lex_elif():
+    """Test the lexing of an 'elif' string."""
     __single_token_test('elif', TT.ELIF)
 
 
 def test_lex_else():
+    """Test the lexing of an 'else' string."""
     __single_token_test('else', TT.ELSE)
 
 
 def test_lex_if_else():
-    input = 'if condition else something'
+    """Test the lexing of an 'if else' string."""
+    input_string = 'if condition else something'
     expected_output = [
         __get_token_string('file', 1, 1, TT.IF),
         __get_token_string('file', 1, 3, TT.WHITESPACE),
         __get_token_string('file', 1, 4, TT.STRING, 'condition'),
         __get_token_string('file', 1, 13, TT.WHITESPACE),
         __get_token_string('file', 1, 14, TT.ELSE),
         __get_token_string('file', 1, 18, TT.WHITESPACE),
         __get_token_string('file', 1, 19, TT.STRING, 'something'),
         __get_token_string('file', 1, 28, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
     lexer = Lexer({'': ''})
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_lex_or():
+    """Test the lexing of an 'or' string."""
     __single_token_test('or', TT.OR)
 
 
 def test_lex_true():
+    """Test the lexing of a boolean true."""
     __single_token_test('true', TT.BOOLEAN, token_value='true')
 
 
 def test_lex_false():
+    """Test the lexing of a boolean false."""
     __single_token_test('false', TT.BOOLEAN, token_value='false')
 
 
 def test_lex_int():
+    """Test the lexing of an integer."""
     __single_token_test('8', TT.INT, token_value='8')
 
 
 def test_lex_float():
+    """Test the lexing of a float."""
     __single_token_test('4.5', TT.FLOAT, token_value='4.5')
 
 
 def test_lex_string():
-    input = 'bucket nom-8'
+    """Test the lexing of strings."""
+    input_string = 'bucket nom-8'
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nom'),
         __get_token_string('file', 1, 11, TT.MINUS),
         __get_token_string('file', 1, 12, TT.INT, 8),
         __get_token_string('file', 1, 13, TT.NEWLINE),
         __get_token_string('file', 2, 1, TT.EOF),
     ]
     lexer = Lexer({'': ''})
-    lexer.lex('file', input)
+    lexer.lex('file', input_string)
     output = lexer.tokenList
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_run_lexer():
-    input = {
+    """Test the run method of the lexer."""
+    input_files = {
         'file': 'bucket nom-8: amount: 5 \n\t',
         'file2': 'network aaaa-#i: nombre: 2 4.5\n\t- property',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nom'),
@@ -386,24 +412,25 @@
         __get_token_string('file2', 2, 1, TT.TAB),
         __get_token_string('file2', 2, 2, TT.MINUS),
         __get_token_string('file2', 2, 3, TT.WHITESPACE),
         __get_token_string('file2', 2, 4, TT.STRING, 'property'),
         __get_token_string('file2', 2, 12, TT.NEWLINE),
         __get_token_string('file2', 3, 1, TT.EOF),
     ]
-    lexer = Lexer(input)
+    lexer = Lexer(input_files)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
 
 
 def test_run_lexer_var_in_name():
-    input = {
+    """Test the run method of the lexer with a variable in a name."""
+    input_file = {
         'file': 'bucket nom-#test \n\t toto: tata',
     }
     expected_output = [
         __get_token_string('file', 1, 1, TT.STRING, 'bucket'),
         __get_token_string('file', 1, 7, TT.WHITESPACE),
         __get_token_string('file', 1, 8, TT.STRING, 'nom'),
         __get_token_string('file', 1, 11, TT.MINUS),
@@ -415,13 +442,13 @@
         __get_token_string('file', 2, 3, TT.STRING, 'toto'),
         __get_token_string('file', 2, 7, TT.COLON),
         __get_token_string('file', 2, 8, TT.WHITESPACE),
         __get_token_string('file', 2, 9, TT.STRING, 'tata'),
         __get_token_string('file', 2, 13, TT.NEWLINE),
         __get_token_string('file', 3, 1, TT.EOF),
     ]
-    lexer = Lexer(input)
+    lexer = Lexer(input_file)
     output = lexer.run()
 
     assert len(output) == len(expected_output)
     for i in range(len(expected_output)):
         assert repr(output[i]) == expected_output[i]
```

### Comparing `thipster-0.17.6/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.7/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Test the THipster DSL token parser."""
 from thipster.engine.parsed_file import Position
 from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 from thipster.parser.dsl_parser.token import Token
 from thipster.parser.dsl_parser.token_parser import TokenParser
 
 
 def test_simple_file():
-    input = [
+    """Test the correct parsing of a simple tokenized file."""
+    tokenized_input = [
         Token(Position('file', 1, 1), TT.STRING, 'bucket'),
         Token(Position('file', 1, 7), TT.WHITESPACE),
         Token(Position('file', 1, 8), TT.STRING, 'nom'),
         Token(Position('file', 1, 11), TT.MINUS),
         Token(Position('file', 1, 12), TT.INT, 8),
         Token(Position('file', 1, 13), TT.COLON),
         Token(Position('file', 1, 14), TT.NEWLINE),
@@ -17,26 +19,27 @@
         Token(Position('file', 2, 2), TT.STRING, 'region'),
         Token(Position('file', 1, 8), TT.COLON),
         Token(Position('file', 2, 3), TT.STRING, 'euw'),
         Token(Position('file', 1, 14), TT.NEWLINE),
         Token(Position('file', 2, 4), TT.EOF),
     ]
 
-    parser = TokenParser(input)
+    parser = TokenParser(tokenized_input)
     output = parser.run()
 
     assert str(output) == '<RESOURCE \
 type = <STRING-EXPR <STRING (STRING bucket)>>, \
 name = <STRING-EXPR <STRING (STRING nom)> <STRING (STRING -)> <INT (INT 8)>>, \
 parameters = <DICT <PARAMETER name = <STRING (STRING region)>, \
 value = <STRING-EXPR <STRING (STRING euw)>>>>>'
 
 
 def test_newline_remover():
-    input = [
+    """Test the correct parsing of a tokenized file with multiple newlines."""
+    tokenized_input = [
         Token(Position('file', 1, 14), TT.NEWLINE),
         Token(Position('file', 1, 14), TT.NEWLINE),
         Token(Position('file', 1, 1), TT.STRING, 'bucket'),
         Token(Position('file', 1, 1), TT.WHITESPACE),
         Token(Position('file', 1, 8), TT.STRING, 'nom'),
         Token(Position('file', 1, 8), TT.MINUS),
         Token(Position('file', 1, 8), TT.INT, 8),
@@ -60,15 +63,15 @@
         Token(Position('file', 2, 1), TT.TAB),
         Token(Position('file', 2, 2), TT.STRING, 'region'),
         Token(Position('file', 1, 8), TT.COLON),
         Token(Position('file', 2, 3), TT.STRING, 'euw'),
         Token(Position('file', 1, 14), TT.NEWLINE),
         Token(Position('file', 2, 4), TT.EOF),
     ]
-    parser = TokenParser(input)
+    parser = TokenParser(tokenized_input)
     output = parser.run()
 
     assert str(output) == '<RESOURCE \
 type = <STRING-EXPR <STRING (STRING bucket)>>, \
 name = <STRING-EXPR <STRING (STRING nom)> <STRING (STRING -)> <INT (INT 8)>>, \
 parameters = <DICT <PARAMETER name = <STRING (STRING region)>, \
 value = <STRING-EXPR <STRING (STRING euw)>>>>>\n\
```

### Comparing `thipster-0.17.6/tests/parser/test_parsedfile.py` & `thipster-0.17.7/tests/parser/test_parsedfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,68 @@
+"""Tests for the ParsedFile object."""
 import thipster.engine.parsed_file as pf
 
 
 def test_create_parsed_file():
-    file = pf.ParsedFile()
+    """Test creating a ParsedFile object."""
+    parsed_file = pf.ParsedFile()
 
-    assert isinstance(file, pf.ParsedFile)
+    assert isinstance(parsed_file, pf.ParsedFile)
 
 
 def test_create_resource():
+    """Test creating a ParsedResource object."""
     pos = pf.Position('test_file', 3, 7)
     resource = pf.ParsedResource(
         'test_type', 'test_name',
         attributes=None, position=pos,
     )
 
     assert isinstance(resource, pf.ParsedResource)
     assert resource.resource_type == 'test_type'
     assert resource.name == 'test_name'
     assert resource.attributes is None
     assert resource.position is pos
 
 
 def test_create_position():
+    """Test creating a Position object."""
     pos = pf.Position('test_file', ln=3, col=7)
 
     assert isinstance(pos, pf.Position)
     assert pos.ln == 3
     assert pos.col == 7
 
 
 def test_create_num_attr():
+    """Test creating a ParsedAttribute object with a number value."""
     val = pf.ParsedLiteral(3)
     pos = pf.Position('test_file', 3, 7)
 
     attr = pf.ParsedAttribute('test_attr', value=val, position=pos)
 
     assert isinstance(attr, pf.ParsedAttribute)
     assert isinstance(attr._ParsedAttribute__value, pf.ParsedLiteral)
     assert attr.value == 3
 
 
 def test_create_str_attr():
+    """Test creating a ParsedAttribute object with a string value."""
     val = pf.ParsedLiteral('test_value')
     pos = pf.Position('test_file', 3, 7)
 
     attr = pf.ParsedAttribute('test_attr', value=val, position=pos)
 
     assert isinstance(attr, pf.ParsedAttribute)
     assert isinstance(attr._ParsedAttribute__value, pf.ParsedLiteral)
     assert attr.value == 'test_value'
 
 
 def test_create_list_str_attr():
+    """Test creating a ParsedAttribute object with a list value."""
     val = pf.ParsedList(
         [pf.ParsedLiteral('test_value_' + str(i)) for i in range(3)],
     )
     pos = pf.Position('test_file', 3, 7)
 
     attr = pf.ParsedAttribute('test_attr', value=val, position=pos)
 
@@ -64,14 +71,15 @@
 
     assert len(attr.value) == 3
     for val in attr.value:
         assert 'test_value' in val.value
 
 
 def test_create_dict_str_attr():
+    """Test creating a ParsedAttribute object with a dict value."""
     val = pf.ParsedDict(
         {pf.ParsedLiteral('test_value_' + str(i)) for i in range(3)},
     )
     pos = pf.Position('test_file', 3, 7)
 
     attr = pf.ParsedAttribute('test_attr', value=val, position=pos)
 
@@ -80,14 +88,15 @@
 
     assert len(attr.value) == 3
     for val in attr.value:
         assert 'test_value' in val.value
 
 
 def test_create_composite_attr():
+    """Test creating a ParsedAttribute object with a composite value."""
     attr = [
         pf.ParsedAttribute(
             'attr_num',
             value=pf.ParsedLiteral(3),
             position=pf.Position('test_file', 3, 7),
         ),
         pf.ParsedAttribute(
@@ -144,18 +153,19 @@
 
         elif isinstance(attribute._ParsedAttribute__value, pf.ParsedList):
             for val in attribute.value:
                 assert isinstance(val, pf.ParsedValue)
 
 
 def test_add_resource():
-    file = pf.ParsedFile()
+    """Test adding a resource to a ParsedFile object."""
+    parsed_file = pf.ParsedFile()
 
     pos = pf.Position('test_file', 3, 7)
     resource = pf.ParsedResource(
         'test_type', 'test_name',
         attributes=None, position=pos,
     )
 
-    file.resources.append(resource)
+    parsed_file.resources.append(resource)
 
-    assert resource in file.resources
+    assert resource in parsed_file.resources
```

### Comparing `thipster-0.17.6/tests/parser/test_parserfactory.py` & `thipster-0.17.7/tests/parser/test_parserfactory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+"""Tests for the parser factory."""
 import pytest
 
+from tests.test_tools import create_dir
 from thipster.engine.parsed_file import ParsedFile
 from thipster.parser import ParserFactory
 from thipster.parser.exceptions import NoFileFoundError
 
-from ..test_tools import create_dir
-
 
 def __test_file(files: str):
     path_input = 'test'
     _destroy_dir = create_dir(
         path_input,
         files,
     )
@@ -24,14 +24,15 @@
     finally:
         _destroy_dir()
 
     return output
 
 
 def test_yaml_file():
+    """Test the parser with .YAML and .YML files."""
     # .YAML
     out = __test_file(
         {
             'test_file.yaml':
             """bucket:
   name: my_bucket
   region: euw
@@ -68,14 +69,15 @@
 
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert region.value == 'euw'
 
 
 def test_thips_file():
+    """Test the parser with .THIPS files."""
     out = __test_file(
         {
             'test_file.thips':
             """bucket my-bucket:
 \tregion: euw
 """,
         },
@@ -89,14 +91,15 @@
 
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert region.value == 'euw'
 
 
 def test_two_types_of_file():
+    """Test the parser with both .THIPS and .YAML files."""
     out = __test_file(
         {
             'test_file.thips':
             """bucket my-bucket1:
 \tregion: euw
 """,
             'test_file.yml':
@@ -115,26 +118,28 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == 'euw'
 
 
 def test_no_parsable_file():
+    """Test the parser with no parsable files."""
     with pytest.raises(NoFileFoundError):
         __test_file(
             {
                 'test_file.txt':
                 """ """,
                 'test_file2.txt':
                 """ """,
             },
         )
 
 
 def test_one_parsable_file():
+    """Test the parser with one parsable file and one non-parsable file."""
     out = __test_file(
         {
             'test_file.thips':
             """bucket my-bucket1:
 \tregion: euw
 """,
             'test_file2.txt':
```

### Comparing `thipster-0.17.6/tests/parser/test_yamlparser.py` & `thipster-0.17.7/tests/parser/test_yamlparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Test the YAMLParser class."""
 import pytest
 
 import thipster.engine.parsed_file as pf
+from tests.test_tools import create_dir
 from thipster.parser import YAMLParser
 from thipster.parser.yaml_parser import YAMLParserNoNameError
 
-from ..test_tools import create_dir
 
-
-def __test_parser_raises(mocker, input: str, exception: Exception)\
-        -> pytest.ExceptionInfo:
+def __test_parser_raises(
+    mocker,  # noqa ARG01
+    input_file: str,
+    exception: Exception,
+) -> pytest.ExceptionInfo:
     with pytest.raises(exception) as exc_info:
         __test_file(
-            file=input,
+            file=input_file,
         )
 
     return exc_info
 
 
 def __test_file(file: str):
     path_input = 'test'
@@ -37,14 +40,15 @@
     finally:
         _destroy_dir()
 
     return output
 
 
 def test_parse_simple_file():
+    """Test the parser with a simple yaml file."""
     out = __test_file(
         file="""bucket:
   name: my-bucket
   region: euw
 """,
     )
     assert len(out.resources) == 1
@@ -57,14 +61,15 @@
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'euw'
 
 
 def test_parse_simple_jinja_file():
+    """Test the parser with a simple file with jinja variables."""
     out = __test_file(
         file="""
 {% set name = "test_name" %}
 {% set region = "europe-west1" %}
 bucket:
   name: {{ name|lower }}
   region: {{ region }}
@@ -80,14 +85,15 @@
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'europe-west1'
 
 
 def test_parse_two_resources():
+    """Test the parser with a list of two resources."""
     out = __test_file(
         file="""bucket:
   - name: my-bucket1
     region: euw
   - name: my-bucket2
     region: euw
 """,
@@ -100,14 +106,15 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == 'euw'
 
 
 def test_parse_dict_in_dict():
+    """Test the parser with a dict in a dict."""
     out = __test_file(
         file="""bucket:
   name: my-bucket
   region: euw
   toto:
     aaa: val1
     bbb: val2
@@ -126,14 +133,15 @@
 
     toto = bucket.attributes[1]
     assert toto.name == 'toto'
     assert isinstance(toto._ParsedAttribute__value, pf.ParsedDict)
 
 
 def test_parse_list():
+    """Test the parser with a list."""
     out = __test_file(
         file="""bucket:
   name: my-bucket
   toto:
     - aaa
     - bbb
 """,
@@ -151,14 +159,15 @@
     assert len(toto.value) == 2
 
     for val in toto.value:
         assert isinstance(val, pf.ParsedLiteral)
 
 
 def test_parse_dict_in_list():
+    """Test the parser with a dict in a list."""
     out = __test_file(
         file="""bucket:
   name: my-bucket
   toto:
     - aaa : 12
       bbb : OK
     - ccc : 10
@@ -181,13 +190,14 @@
         assert isinstance(val, pf.ParsedDict)
         assert len(val.value) == 2
         for v in val.value:
             assert isinstance(v, pf.ParsedAttribute)
 
 
 def test_syntax_error_no_name(mocker):
-    input = """bucket:
+    """Test the parser with a missing resource name."""
+    input_file = """bucket:
   toto:
     - aaa
     - bbb
 """
-    __test_parser_raises(mocker, input, YAMLParserNoNameError)
+    __test_parser_raises(mocker, input_file, YAMLParserNoNameError)
```

### Comparing `thipster-0.17.6/tests/test_e2e.py` & `thipster-0.17.7/tests/test_e2e.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+"""End to end tests for the thipster tool.
+
+Starts from a .thips or .yaml file and tests the creation of the resources on GCP.
+"""
 import os
 import random
 import uuid
+from pathlib import Path
 
 import pytest
 import tftest
 
 from .test_tools import (
     assert_number_of_resource_type_is,
     assert_resource_created,
     assert_resource_parameters_are,
     get_function_name,
     process_file,
 )
 
-AUTH_FILE_PATH = os.path.join(os.getcwd(), 'tests/credentials.json')
+AUTH_FILE_PATH = Path(Path.cwd(), 'tests/credentials.json')
 
 
 @pytest.fixture
 def apply_output():
+    """Apply terraform and return output."""
     def _apply_output(function_name):
         tf = tftest.TerraformTest(
             tfdir='.',
             basedir=f'test/{function_name}',
         )
 
         tf.setup()
@@ -35,45 +41,46 @@
             tf.destroy()
 
     return _apply_output
 
 
 @pytest.fixture
 def authentication():
+    """Authenticate to GCP."""
     delete_credentials = False
     if (
-        not os.path.exists(
-            os.path.join(
-                os.getenv('HOME'),
-                '.config/gcloud/application_default_credentials.json',
-            ),
-        )
+        not Path(
+            os.getenv('HOME'),
+            '.config/gcloud/application_default_credentials.json',
+        ).exists()
         and (
             os.getenv('GOOGLE_APPLICATION_CREDENTIALS') is not None
             or os.getenv('GOOGLE_APPLICATION_CREDENTIALS') != ''
         )
     ):
 
         delete_credentials = True
         if os.getenv('GOOGLE_APPLICATION_CREDENTIALS_CONTENT') is None:
-            raise Exception('No credentials available')
+            msg = 'No credentials available'
+            raise Exception(msg)
 
-        with open(AUTH_FILE_PATH, 'w') as auth_file:
+        with Path(AUTH_FILE_PATH).open('w') as auth_file:
             auth_file.write(
                 os.environ['GOOGLE_APPLICATION_CREDENTIALS_CONTENT'],
             )
-        os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = AUTH_FILE_PATH
+        os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = AUTH_FILE_PATH.as_posix()
 
     yield
 
     if delete_credentials:
-        os.remove(AUTH_FILE_PATH)
+        Path(AUTH_FILE_PATH).unlink()
 
 
 def test_bucket(apply_output, authentication):
+    """Test bucket creation."""
     _ = authentication
     function_name = get_function_name()
 
     bucket_name = f'test-bucket-{uuid.uuid4().int}'
     clean_up = process_file(
         directory=function_name,
         file=f"""
@@ -85,23 +92,24 @@
     try:
         # Assertions on plan
         assert_number_of_resource_type_is('google_storage_bucket', 1)
         bucket = assert_resource_created('google_storage_bucket', bucket_name)
         assert_resource_parameters_are(bucket, ['location'])
 
         # Test apply
-        _ = [o for o in apply_output(function_name)]
+        _ = list(apply_output(function_name))
 
     except Exception as e:
         raise e
     finally:
         clean_up()
 
 
 def test_lb(apply_output, authentication):
+    """Test load balancer creation."""
     _ = authentication
     function_name = get_function_name()
 
     test_id = random.randint(0, 10000)
     clean_up = process_file(
         directory=function_name,
         file=f"""
@@ -125,13 +133,13 @@
 
         assert_number_of_resource_type_is('google_compute_subnetwork', 1)
         assert_resource_created(
             'google_compute_subnetwork', f'lb-subnet-{test_id}',
         )
 
         # Test apply
-        _ = [o for o in apply_output(function_name)]
+        _ = list(apply_output(function_name))
 
     except Exception as e:
         raise e
     finally:
         clean_up()
```

### Comparing `thipster-0.17.6/thipster/auth/google.py` & `thipster-0.17.7/thipster/auth/google.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+"""Google Cloud Platform (GCP) authentication module."""
 import google.auth
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
 from thipster.engine import AuthPort
 
 
 class GoogleAuth(AuthPort):
-    """Authenticate to Google Cloud Platform (GCP) projects
+    """Authenticate to Google Cloud Platform (GCP) projects.
 
     To use this module, you need to have a GCP account and a project created.
     You also need to have gcloud installed : https://cloud.google.com/sdk/docs/install
     Then login using glcloud : gcloud auth application-default login
     """
 
     @classmethod
     def authenticate(cls, app):
-        """Generates the google provider block for the Terraform CDK
+        """Generate the google provider block for the Terraform CDK.
 
         Parameters
         ----------
         app: Construct
             CDK Construct where the provider is created
 
         """
-
         credentials, project_id = google.auth.default()
 
         GoogleProvider(
             app, 'default_google',
             project=project_id,
             access_token=credentials.token,
         )
```

### Comparing `thipster-0.17.6/thipster/engine/engine.py` & `thipster-0.17.7/thipster/engine/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,102 @@
-"""_Engine.py module.
-"""
+"""Engine.py module."""
 
 import thipster.engine.parsed_file as pf
 
 from .i_auth import AuthPort
 from .i_parser import ParserPort
 from .i_repository import RepositoryPort
 from .i_terraform import TerraformPort
 from .resource_model import ResourceModel
 
 
 class Engine():
-    """The engine of thipster
+    """THipster's Engine.
 
     The core of the application, it is used to call and link all
     interfaces together.
     """
 
     def __init__(
             self, parser: ParserPort,
             repository: RepositoryPort,
             auth: AuthPort,
             terraform:  TerraformPort,
     ):
-        """
+        """THipster's Engine.
+
+        The core of the application, it is used to call and link all
+        interfaces together.
+
         Parameters
         ----------
         parser : ParserPort
             Instance of a Parser class
         repository : RepositoryPort
             Instance of a Respository class
         auth : AuthPort
             Instance of an Auth class
         terraform : TerraformPort
             Instance of a Terraform class
-
         """
         self.__parser = parser
         self.__repository = repository
         self.__auth = auth
         self.__terraform = terraform
 
     @property
     def parser(self):
+        """Get the parser."""
         return self.__parser
 
     @parser.setter
     def parser(self, value):
         if not isinstance(value, ParserPort):
-            raise Exception()
+            raise Exception
 
         self.__parser = value
 
     @property
     def repository(self):
+        """Get the repository."""
         return self.__repository
 
     @repository.setter
     def repository(self, value):
         if not isinstance(value, RepositoryPort):
-            raise Exception()
+            raise Exception
 
         self.__repository = value
 
     @property
     def auth(self):
+        """Get the authentification module."""
         return self.__auth
 
     @auth.setter
     def auth(self, value):
         if not isinstance(value, AuthPort):
-            raise Exception()
+            raise Exception
 
         self.__auth = value
 
     @property
     def terraform(self):
+        """Get the Terraform module."""
         return self.__terraform
 
     @terraform.setter
     def terraform(self, value):
         if not isinstance(value, TerraformPort):
-            raise Exception()
+            raise Exception
 
         self.__terraform = value
 
     def run(self, path: str) -> tuple[list[str], str]:
-        """Returns json Terraform files from the input file name
+        """Return json Terraform files from the input file name.
 
         Calls the different run methods of the parser, repository,
         auth and terraform modules.
         Transforms the inputed filename into a Cloud architecture plan.
 
         Parameters
         ----------
@@ -100,28 +106,28 @@
         Returns
         -------
         tuple[list[str], str]
             A tuple made up of the list of directories containing the Terraform json
             files and a string with the results of the Terraform plan
         """
         # Parse file or directory
-        parsed_file = self._parse_files(path)
+        parsed_file = self.parse_files(path)
 
         # Get needed models
-        models = self._get_models(parsed_file)
+        models = self.get_models(parsed_file)
 
         # Generate Terraform files
-        self._generate_tf_files(parsed_file, models)
+        self.generate_tf_files(parsed_file, models)
 
         self.__terraform.init()
 
         return self.__terraform.plan()
 
-    def _parse_files(self, path: str) -> pf.ParsedFile:
-        """Parse the input file or directory
+    def parse_files(self, path: str) -> pf.ParsedFile:
+        """Parse the input file or directory.
 
         Parameters
         ----------
         path : str
             The path of the files to be processed
 
         Returns
@@ -130,74 +136,62 @@
             The ParsedFile object containing the resources defined in the input file
         """
         parsed_file = self.__parser.run(path)
         assert type(parsed_file) == pf.ParsedFile
 
         return parsed_file
 
-    def _get_models(
+    def get_models(
         self, file: pf.ParsedFile,
     ) -> dict[str, ResourceModel]:
-        """Get the models from the repository
+        """Get the models from the repository.
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
 
         Returns
         -------
         dict[str, ResourceModel]
             The dictionary of models
         """
         types = [r.resource_type for r in file.resources]
-        models = self.__repository.get(types)
-
-        return models
+        return self.__repository.get(types)
 
-    def _generate_tf_files(
+    def generate_tf_files(
         self, file: pf.ParsedFile, models: dict[str, ResourceModel],
-    ) -> list[str]:
-        """Generate Terraform files
+    ) -> None:
+        """Generate Terraform files.
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         models : dict[str, ResourceModel]
             The dictionary of models
-
-        Returns
-        -------
-        list[str]
-            A list of directories containing the Terraform json files
         """
         self.__terraform.generate(file, models, self.__auth)
 
-    def _init_terraform(self) -> None:
-        """Initialize Terraform
-        """
+    def init_terraform(self) -> None:
+        """Initialize Terraform."""
         self.__terraform.init()
 
-    def _plan_terraform(self) -> str:
-        """Plan Terraform
+    def plan_terraform(self) -> str:
+        """Plan Terraform.
 
         Returns
         -------
         str
             The results of the Terraform plan
         """
-        results = self.__terraform.plan()
-
-        return results
+        return self.__terraform.plan()
 
-    def _apply_terraform(self) -> str:
-        """Apply Terraform
+    def apply_terraform(self) -> str:
+        """Apply Terraform.
 
         Returns
         -------
         str
             The results of the Terraform apply
         """
-        results = self.__terraform.apply()
-
-        return results
+        return self.__terraform.apply()
```

### Comparing `thipster-0.17.6/thipster/engine/i_parser.py` & `thipster-0.17.7/thipster/engine/i_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""Parser module interface."""
 from abc import ABC, abstractclassmethod
 
 from thipster.engine.parsed_file import ParsedFile
 
 
 class ParserPort(ABC):
-    """Parser module interface
-    """
+    """Parser port."""
+
     @classmethod
     @abstractclassmethod
-    def run(cls, path: str) -> ParsedFile:
-        """Abstract run method
+    def run(
+        cls,
+        path: str,  # noqa: ARG003
+    ) -> ParsedFile:
+        """Abstract run method.
 
         Parameters
         ----------
         path : str
             The path of the filesor directory to be processed
 
         Returns
@@ -24,8 +28,9 @@
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
-        raise NotImplementedError('Should implement run()')
+        msg = 'Should implement run()'
+        raise NotImplementedError(msg)
```

### Comparing `thipster-0.17.6/thipster/engine/i_repository.py` & `thipster-0.17.7/thipster/engine/i_repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+"""Repository module interface."""
 from abc import ABC, abstractmethod
 
 from thipster.engine.resource_model import ResourceModel
 
 
 class RepositoryPort(ABC):
-    """Repository module interface
-    """
+    """Repository port."""
+
     @abstractmethod
     def get(self, resource_names: list[str]) -> dict[str, ResourceModel]:
-        """Abstract get method
+        """Abstract get method.
 
         Parameters
         ----------
         resourceNames : list[str]
             List of resource names to be retrieved from the repository
 
         Returns
```

### Comparing `thipster-0.17.6/thipster/engine/i_terraform.py` & `thipster-0.17.7/thipster/engine/i_terraform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,87 @@
+"""Terraform module interface."""
 from abc import ABC, abstractclassmethod
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 
 from .i_auth import AuthPort
 
 
 class TerraformPort(ABC):
-    """Terraform module interface
-    """
+    """Terraform port."""
+
     @classmethod
     @abstractclassmethod
-    def apply(cls, plan_file_path: str | None = None):
-        """Apply generated terraform code
+    def apply(
+        cls,
+        plan_file_path: str | None = None,  # noqa: ARG003
+    ):
+        """Apply generated terraform code.
 
         Parameters
         ----------
         plan_file_path : str, optional
             Path to plan file, by default None
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
-        raise NotImplementedError('Should implement apply()')
+        msg = 'Should implement apply()'
+        raise NotImplementedError(msg)
 
     @classmethod
     @abstractclassmethod
     def generate(
-        cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
+        cls,
+        file: pf.ParsedFile,  # noqa: ARG003
+        models: dict[str, rm.ResourceModel],  # noqa: ARG003
         _authenticator: AuthPort,
     ):
-        """Generates Terraform code from parsed file and models
+        """Generate Terraform code from parsed file and models.
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
         models : dict[str, rm.ResourceModel]
             The dictionary of models
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
-        raise NotImplementedError('Should implement generate()')
+        msg = 'Should implement generate()'
+        raise NotImplementedError(msg)
 
     @classmethod
     @abstractclassmethod
     def init(cls):
-        """Init Terraform for generated terraform code
+        """Init Terraform for generated terraform code.
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
-        raise NotImplementedError('Should implement generate()')
+        msg = 'Should implement generate()'
+        raise NotImplementedError(msg)
 
     @classmethod
     @abstractclassmethod
     def plan(cls):
-        """Get plan from generated terraform code
+        """Get plan from generated terraform code.
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
-        raise NotImplementedError('Should implement plan()')
+        msg = 'Should implement plan()'
+        raise NotImplementedError(msg)
```

### Comparing `thipster-0.17.6/thipster/engine/parsed_file.py` & `thipster-0.17.7/thipster/engine/parsed_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-"""parsedFile.py Module
-"""
+"""parsedFile.py Module."""
 
 from abc import ABC
 
 
 class ParsedValue(ABC):
-    """Parsed Value Interface
-    """
+    """Parsed Value Interface."""
 
     pass
 
 
 class Position():
-    """Class representing the position of a token
+    """Represents the position of a token.
 
     Indicates the initial position of a token, resource or character in the input files.
     It includes the file name, line and column numbers of the designated element.
     """
 
     def __init__(self, filename: str, ln: int, col: int):
-        """
+        """Represent the position of a token.
+
+        Indicates the initial position of a token, resource or character in the input
+        files.
+        It includes the file name, line and column numbers of the designated element.
+
         Parameters
         ----------
         fileName : str
             file name
         ln : int
             line number
         col : int
             column number
         """
-
         self.filename = filename
         self.ln = ln
         self.col = col
 
     def __str__(self) -> str:
-        """Returns a string of the position object
+        """Return a string of the position object.
 
         Returns
         -------
         str
             (File : {}, Ln {}, Col {})
         """
-
         return f'(File : {self.filename}, Ln {self.ln}, Col {self.col})'
 
     def __eq__(self, __value: object) -> bool:
-        """Check if 2 positions are equal
+        """Check if 2 positions are equal.
 
         Parameters
         ----------
         __value : object
             Position to compare
 
         Returns
@@ -59,139 +60,143 @@
             True if both positions are equal or False otherwise
 
         Raises
         ------
         TypeError
             If '__value' is not a Position
         """
-
-        if isinstance(__value, Position):
-            return (
-                self.filename == __value.filename and
-                self.ln == __value.ln and
-                self.col == __value.col
-            )
-        else:
-            raise TypeError('Value must be a Position')
+        if not isinstance(__value, Position):
+            msg = 'Value must be a Position'
+            raise TypeError(msg)
+
+        return (
+            self.filename == __value.filename and
+            self.ln == __value.ln and
+            self.col == __value.col
+        )
 
 
 class ParsedAttribute():
-    """Class reprensenting a Parsed Attribute Object
-    """
+    """Reprensents a Parsed Attribute Object."""
 
     def __init__(self, name: str, position: Position | None, value: ParsedValue):
         """
+        Represent a Parsed Attribute Object.
+
         Parameters
         ----------
         name : str
-        position : Position
+            name of the attribute
+        position : Position | None
+            position of the attribute in its origin file
         value : ParsedValue
+            value of the attribute
         """
-
         self.name: str = name
         self.position: Position | None = position
         self.__value = value
 
     @property
     def value(self):
-        """Value of the parsed attribute
-        """
-
+        """Value of the parsed attribute."""
         return self.__value.value
 
 
 class ParsedList(ParsedValue):
-    """Class representing a Parsed List Object
-    """
+    """Represents a Parsed List Object."""
 
     def __init__(self, value: list[ParsedValue]):
         """
+        Represent a Parsed List Object.
+
         Parameters
         ----------
         value : list[ParsedValue]
+            value of the parsed list
         """
-
         super().__init__()
         self.value: list[ParsedValue] = value
 
     def __iter__(self):
+        """Return an iterator object."""
         self.i = 0
         return self
 
     def __next__(self):
+        """Return the next value of the iterator."""
         if self.i > len(self.__value):
             raise StopIteration
-        else:
-            ret = self.value[self.i]
-            self.i += 1
 
-        return ret
+        self.i += 1
+        return self.value[self.i-1]
 
 
 class ParsedLiteral(ParsedValue):
-    """Class representing a Parsed Literal Object
-    """
+    """Represents a Parsed Literal Object."""
 
     def __init__(self, value: bool | int | float | str):
         """
+        Represent a Parsed Literal Object.
+
         Parameters
         ----------
         value : Literal
+            value of the parsed literal
         """
-
         super().__init__()
         self.value: bool | int | float | str = value
 
 
 class ParsedDict(ParsedValue):
-    """Class representing a Parsed Dictionnary Object
-    """
+    """Represents a Parsed Dictionnary Object."""
 
     def __init__(self, value: list[ParsedAttribute]):
         """
+        Represent a Parsed Dictionnary Object.
+
         Parameters
         ----------
         value : list[ParsedAttribute]
+            value of the parsed dictionnary
         """
-
         super().__init__()
         self.value: list[ParsedAttribute] = value
 
 
 class ParsedResource():
-    """Class representing a Parsed Resource
-    """
+    """Represents a Parsed Resource."""
 
     def __init__(
             self,
-            type: str,
+            parsed_resource_type: str,
             name: str,
             position: Position | None,
             attributes: list[ParsedAttribute],
     ):
         """
+        Represent a Parsed Resource.
+
         Parameters
         ----------
-        type : str
+        parsed_resource_type : str
         name : str
             name of the resource
         position : Position
             position of the resource in its origin file
         attributes : list[ParsedAttribute]
             list of attributes of the resource
         """
-
-        self.resource_type: str = type
+        self.resource_type: str = parsed_resource_type
         self.name: str = name
         self.position: Position | None = position
         self.attributes: list[ParsedAttribute] = attributes
 
 
 class ParsedFile():
-    """Class representing a Parsed File
+    """Represents a Parsed File.
 
     Object containing a list of parsed resources making up a file.
-
     """
 
     def __init__(self):
+        """Represent a Parsed File."""
         self.resources: list[ParsedResource] = []
```

### Comparing `thipster-0.17.6/thipster/helpers.py` & `thipster-0.17.7/thipster/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+"""Helper functions for thipster."""
 import logging
 
 
 def create_logger(class_name: str) -> logging.Logger:
-    logger = logging.getLogger(class_name)
-    return logger
+    """Create a logger for the given class."""
+    return logging.getLogger(class_name)
 
 
 def set_logging_config(
     log_level: str = 'INFO',
     filename: str | None = None,
     filemode: str = 'w',
 ) -> None:
-    """Set logging configuration
+    """Set logging configuration.
 
     Parameters
     ----------
     log_level : str
         Log level, defaults to INFO
     filename : str, optional
         Log filename, defaults to None
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.7/thipster/parser/dsl_parser/interpreter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,55 @@
+"""Interpreter for the DSL Parser."""
 import thipster.engine.parsed_file as pf
 import thipster.parser.dsl_parser.ast as ast
 
 from .exceptions import (
     DSLArithmeticError,
     DSLParserVariableAlreadyUsedError,
     DSLParserVariableNotDeclaredError,
 )
 from .token import TOKENTYPES as TT
 
 
 class Interpreter():
-    """Interpreter class for the DSL Parser
+    """Interpreter class for the DSL Parser.
 
     Implements a visitor design pattern on the AST nodes
     """
 
     def __init__(self) -> None:
+        """Interpreter class for the DSL Parser.
+
+        Implements a visitor design pattern on the AST nodes
+        """
         super().__init__()
 
         self.__variables = dict[str, int]()
 
     def run(self, tree: ast.FileNode) -> pf.ParsedFile:
-        """Runs the interpreter on an Abstract Syntax Tree
+        """Run the interpreter on an Abstract Syntax Tree.
 
         Parameters
         ----------
         tree: FileNode
             The root node of the abstract syntax tree
 
         Returns
         -------
         ParsedFile
             The parsed file stucture assiociated to the given AST
         """
         return tree.accept(self)
 
     def visit_comp_expr(self, element: ast.CompExprNode) -> bool:
-        """Visitor for a StringNode
+        """Visitor for a CompExprNode.
 
         Parameters
         ----------
-        element: StringNode
+        element: CompExprNode
             The visited node
 
         Returns
         -------
         bool
             The boolean value of the node
         """
@@ -97,19 +102,19 @@
             case TT.GTE:
                 return pf.ParsedLiteral(
                     element.left_value.accept(self).value >=
                     element.right_value.accept(self).value,
                 )
 
     def visit_arith_expr(self, element: ast.ArithExprNode) -> int | float:
-        """Visitor for a StringNode
+        """Visitor for an ArithExprNode.
 
         Parameters
         ----------
-        element: StringNode
+        element: ArithExprNode
             The visited node
 
         Returns
         -------
         int | float
             The arithmetic value of the node
         """
@@ -130,19 +135,19 @@
                     if isinstance(rm, pf.ParsedLiteral):
                         rm = rm.value
                     total -= rm
 
         return pf.ParsedLiteral(total)
 
     def visit_term(self, element: ast.TermNode) -> int | float:
-        """Visitor for a StringNode
+        """Visitor for a TermNode.
 
         Parameters
         ----------
-        element: StringNode
+        element: TermNode
             The visited node
 
         Returns
         -------
         int | float
             The arithmetic value of the node
         """
@@ -163,19 +168,19 @@
                     if isinstance(div, pf.ParsedLiteral):
                         div = div.value
                     total /= div
 
         return total
 
     def visit_factor(self, element: ast.FactorNode) -> int | float:
-        """Visitor for a StringNode
+        """Visitor for a Factor node.
 
         Parameters
         ----------
-        element: StringNode
+        element: FactorNode
             The visited node
 
         Returns
         -------
         int | float
             The arithmetic value of the node
         """
@@ -188,22 +193,22 @@
                 return pf.ParsedLiteral(total)
 
             case TT.MINUS:
                 return pf.ParsedLiteral(-total)
 
             case TT.POW:
                 for f in element.factors[1:]:
-                    pow = f.accept(self)
-                    if isinstance(pow, pf.ParsedLiteral):
-                        pow = pow.value
-                    total = total**pow
+                    power = f.accept(self)
+                    if isinstance(power, pf.ParsedLiteral):
+                        power = power.value
+                    total = total**power
                 return pf.ParsedLiteral(total)
 
     def visit_string_expr(self, element: ast.StringExprNode) -> str:
-        """Visitor for a StringExprNode
+        """Visitor for a StringExprNode.
 
         Parameters
         ----------
         element: StringExprNode
             The visited node
 
         Returns
@@ -214,15 +219,15 @@
         ret = ''
         for value in element.values:
             ret += str(value.accept(self))
 
         return pf.ParsedLiteral(ret)
 
     def visit_variable_definition(self, element: ast.VariableDefinitionNode) -> str:
-        """Visitor for a VariableDefinitionNode
+        """Visitor for a VariableDefinitionNode.
 
         Parameters
         ----------
         element: VariableDefinitionNode
             The visited node
 
         Returns
@@ -239,15 +244,15 @@
             raise DSLParserVariableAlreadyUsedError(element.name)
 
         self.__variables[element.name] = element.value.accept(self)
 
         return element.name
 
     def visit_variable(self, element: ast.VariableNode) -> object:
-        """Visitor for a VariableNode
+        """Visitor for a VariableNode.
 
         Parameters
         ----------
         element: VariableNode
             The visited node
 
         Returns
@@ -262,75 +267,75 @@
         """
         if element.name not in self.__variables:
             raise DSLParserVariableNotDeclaredError(element.name)
 
         return self.__variables[element.name]
 
     def visit_int(self, element: ast.IntNode) -> int:
-        """Visitor for an IntNode
+        """Visitor for an IntNode.
 
         Parameters
         ----------
         element: IntNode
             The visited node
 
         Returns
         -------
         int
             The value of the node
         """
         return int(element.token.value)
 
     def visit_float(self, element: ast.FloatNode) -> float:
-        """Visitor for a FloatNode
+        """Visitor for a FloatNode.
 
         Parameters
         ----------
         element: FloatNode
             The visited node
 
         Returns
         -------
         float
             The value of the node
         """
         return float(element.token.value)
 
     def visit_bool(self, element: ast.BoolNode) -> bool:
-        """Visitor for a BoolNode
+        """Visitor for a BoolNode.
 
         Parameters
         ----------
         element: BoolNode
             The visited node
 
         Returns
         -------
         bool
             The value of the node
         """
         return bool(element.token.value)
 
     def visit_string(self, element: ast.StringNode) -> str:
-        """Visitor for a BoolNode
+        """Visitor for a BoolNode.
 
         Parameters
         ----------
         element: BoolNode
             The visited node
 
         Returns
         -------
         bool
             The value of the node
         """
         return str(element.token.value)
 
     def visit_if(self, element: ast.IfNode) -> object | None:
-        """Visitor for an IfNode
+        """Visitor for an IfNode.
 
         Parameters
         ----------
         element: IfNode
             The visited node
 
         Returns
@@ -338,32 +343,32 @@
         object | None
             The value of the child node if the condition is true, else None
         """
         return element.if_case.accept(self) if element.condition.accept(self).value\
             else None
 
     def visit_ifelse(self, element: ast.IfElseNode):
-        """Visitor for an IfElseNode
+        """Visitor for an IfElseNode.
 
         Parameters
         ----------
         element: IfElseNode
             The visited node
 
         Returns
         -------
         object | None
             The value of the "if" child node if the condition is true, else the value\
-                  of the "else" child node
+            of the "else" child node
         """
         return element.if_case.accept(self) if element.condition.accept(self).value\
             else element.else_case.accept(self)
 
     def visit_amount(self, element: ast.AmountNode) -> list[object]:
-        """Visitor for an AmountNode
+        """Visitor for an AmountNode.
 
         Parameters
         ----------
         element: AmountNode
             The visited node
 
         Returns
@@ -382,15 +387,15 @@
         for _ in range(amount):
             res += element.node.accept(self)
             if var:
                 self.__variables[var] += 1
         return res
 
     def visit_parameter(self, element: ast.ParameterNode) -> pf.ParsedAttribute:
-        """Visitor for an ParameterNode
+        """Visitor for a ParameterNode.
 
         Parameters
         ----------
         element: ParameterNode
             The visited node
 
         Returns
@@ -402,91 +407,91 @@
         return pf.ParsedAttribute(
             name=element.name.accept(self),
             position=element.position,
             value=element.value.accept(self),
         )
 
     def visit_dict(self, element: ast.DictNode) -> pf.ParsedDict:
-        """Visitor for an DictNode
+        """Visitor for a DictNode.
 
         Parameters
         ----------
         element: DictNode
             The visited node
 
         Returns
         -------
         ParsedDict
             A ParsedDict object based on the node attributes
         """
         return pf.ParsedDict([v.accept(self) for v in element.values])
 
     def visit_literal(self, element: ast.LiteralNode) -> pf.ParsedLiteral:
-        """Visitor for an LiteralNode
+        """Visitor for a LiteralNode.
 
         Parameters
         ----------
         element: LiteralNode
             The visited node
 
         Returns
         -------
         ParsedLiteral
             A ParsedLiteral object based on the node value
         """
         return pf.ParsedLiteral(element.value.accept(self))
 
     def visit_list(self, element: ast.ListNode) -> pf.ParsedList:
-        """Visitor for an ListNode
+        """Visitor for a ListNode.
 
         Parameters
         ----------
         element: ListNode
             The visited node
 
         Returns
         -------
         ParsedList
             A ParsedLiteral object based on the node elements
         """
         return pf.ParsedList([v.accept(self) for v in element.values])
 
     def visit_resource(self, element: ast.ResourceNode) -> list[pf.ParsedResource]:
-        """Visitor for an ResourceNode
+        """Visitor for a ResourceNode.
 
         Parameters
         ----------
         element: ResourceNode
             The visited node
 
         Returns
         -------
         int
             A ParsedResource object based on the node's attributes
         """
         return [
             pf.ParsedResource(
-                type=element.type.accept(self).value,
+                parsed_resource_type=element.type.accept(self).value,
                 name=element.name.accept(self).value,
                 position=element.position,
                 attributes=[v.accept(self) for v in element.parameters.values],
             ),
         ]
 
     def visit_file(self, element: ast.FileNode):
-        """Visitor for an FileNode
+        """Visitor for a FileNode.
 
         Parameters
         ----------
         element: FileNode
             The visited node
 
         Returns
         -------
         ParsedFile
             A ParsedFile object based on the node's resources
         """
-        file = pf.ParsedFile()
+        parsed_file = pf.ParsedFile()
         for res in element.resources:
-            file.resources += res.accept(self)
+            parsed_file.resources += res.accept(self)
 
-        return file
+        return parsed_file
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.7/thipster/parser/dsl_parser/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+"""Lexer module for the DSL Parser."""
 from thipster.engine.parsed_file import Position
 from thipster.helpers import create_logger
 
 from .exceptions import DSLParserNoEndingQuotesError
 from .lexer_position import LexerPosition
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
 class Lexer():
-    """Lexer class for the DSL Parser
-    """
+    """Lexer for the DSL Parser."""
 
     def __init__(self, files: dict[str, str]):
-        """
+        """Lexer for the DSL Parser.
+
         Parameters
         ----------
         files : dict[str, str]
             Dictionnary of files to tokenize, fileName : fileContent
         """
         self.__logger = create_logger(__name__)
         self.files = files
         self.tokenList = []
         self.__lexerPosition = LexerPosition()
         self.__currentChar = ''
 
     def run(self) -> list[Token]:
-        """Launch the Lexer
+        """Launch the Lexer.
 
         Returns
         -------
         list[Token]
             List of Tokens representing the input files
         """
         self.__logger.info('Start Lexer')
@@ -44,29 +45,28 @@
         return self.tokenList
 
     def lex(
         self,
         filename: str,
         file_content: str,
     ) -> None:
-        """Tokenize a file contents
+        """Tokenize a file contents.
 
         Parameters
         ----------
         filename : str
             Name of the file
         file_content : str
             Content of the file
 
         Raises
         ------
         DSLParserNoEndingQuotes
             Syntax error : detected a starting quote but no ending one
         """
-
         self.__logger.debug('Lex file %s', filename)
         self.__lexerPosition = LexerPosition(filename)
 
         for char in file_content:
             self.__logger.debug('char %s', char)
             self.__currentChar = char
             if not self.__lexerPosition.isQuotedString:
@@ -95,24 +95,24 @@
 
             self.__add_next_char()
 
         self.__end_file()
         self.__logger.debug('Finished lexing file %s', filename)
 
     def __add_next_char(self):
-        """Add the current character to the current Token
-        """
+        """Add the current character to the current Token."""
         self.__lexerPosition.add_to_current_token(self.__currentChar)
         self.__lexerPosition.next_column()
 
     def __handle_empty_token(self):
+        """Pass EMPTY tokens ''."""
         pass
 
     def __handle_syntax_tokens(self) -> None:
-        """Handle single character tokens
+        """Handle single character tokens.
 
         Check if the current character is a special token and calls the corresponding
         function.
         If it isn't, it calls the '__iterateNextChar' function
         """
         single_char_tokens = {
             ':': self.__handle_colon_oken,
@@ -139,15 +139,15 @@
             '>': self.__handle_gt_token,
             '!': self.__handle_exclamation_token,
         }
 
         single_char_tokens.get(self.__currentChar, self.__add_next_char)()
 
     def __handle_current_token(self) -> None:
-        """Process the current stored token
+        """Process the current stored token.
 
         Check if the current token is a keyword, calls the cprresponding function, or
         the '__handleLiteralsAndVariables' otherwise.
         """
         current_token = self.__lexerPosition.currentToken.lower()
 
         keywords = {
@@ -162,15 +162,15 @@
             'false': self.__handle_boolean_token,
             'not': self.__handle_not_token,
         }
 
         keywords.get(current_token, self.__handle_literals_and_variables)()
 
     def __handle_literals_and_variables(self) -> None:
-        """Create a literal or var token
+        """Create a literal or var token.
 
         Checks the current token to create a var, int, float or string token
         """
         current_token = self.__lexerPosition.currentToken
         if self.__lexerPosition.isVariable:
             self.__add_literal_token_to_list(TT.VAR, current_token)
             self.__lexerPosition.isVariable = False
@@ -181,15 +181,15 @@
         elif self.__isfloat(current_token):
             self.__add_literal_token_to_list(TT.FLOAT, current_token)
 
         else:
             self.__add_literal_token_to_list(TT.STRING, current_token)
 
     def __add_literal_token_to_list(self, token_type: str, value: str):
-        """Add a literal token to the token list
+        """Add a literal token to the token list.
 
         Parameters
         ----------
         tokenType : str
             Type of the token
         value : str
             Value of the token
@@ -203,15 +203,15 @@
 
     def __add_base_token(
         self,
         token_type: str,
         value: str | None = None,
         is_current_token: bool = False,
     ) -> None:
-        """Add a token to the token list
+        """Add a token to the token list.
 
         Parameters
         ----------
         tokenType : str
             Type of the token
         value : str, optional
             Value of the token, by default None
@@ -236,15 +236,15 @@
             ),
         )
 
     def __update_position(
         self,
         reset_current_token: bool = True,
     ) -> None:
-        """Update the lexer's current position
+        """Update the lexer's current position.
 
         Parameters
         ----------
         resetCurrentToken : bool, optional
             Indicates if the current stored token should be reset, by default True
         """
         self.__lexerPosition.next_column()
@@ -258,15 +258,15 @@
         self,
         token_type: str,
         value: str | None = None,
         is_current_token: bool = False,
         handle_current_token: bool = True,
         reset_current_token: bool = True,
     ) -> None:
-        """Handle a token creation and lexer position
+        """Handle a token creation and lexer position.
 
         Parameters
         ----------
         token_type : str
             Type of the token
         value : str, optional
             Value of the token, by default None
@@ -279,99 +279,84 @@
         """
         if handle_current_token:
             self.__handle_current_token()
         self.__add_base_token(token_type, value, is_current_token)
         self.__update_position(reset_current_token)
 
     def __handle_colon_oken(self):
-        """Handle a COLON token ':'
-        """
+        """Handle a COLON token ':'."""
         self.__handle_base_token(TT.COLON)
 
     def __handle_comma_token(self):
-        """Handle a COMMA token ','
-        """
+        """Handle a COMMA token ','."""
         self.__handle_base_token(TT.COMMA)
 
     def __handle_brackets_start_token(self):
-        """Handle a BRACKETS_START token '['
-        """
+        """Handle a BRACKETS_START token '['."""
         self.__handle_base_token(TT.BRACKETS_START)
 
     def __handle_brackets_end_token(self):
-        """Handle a BRACKETS_END token ']'
-        """
+        """Handle a BRACKETS_END token ']'."""
         self.__handle_base_token(TT.BRACKETS_END)
 
     def __handle_parentheses_start_token(self):
-        """Handle a PARENTHESES_START token '('
-        """
+        """Handle a PARENTHESES_START token '('."""
         self.__handle_base_token(TT.PARENTHESES_START)
 
     def __handle_parentheses_end_token(self):
-        """Handle a PARENTHESES_END token ')'
-        """
+        """Handle a PARENTHESES_END token ')'."""
         self.__handle_base_token(TT.PARENTHESES_END)
 
     def __handle_plus_token(self):
-        """Handle a PLUS token '+'
-        """
+        """Handle a PLUS token '+'."""
         self.__handle_base_token(TT.PLUS)
 
     def __handle_minus_token(self):
-        """Handle a MINUS token '-'
-        """
+        """Handle a MINUS token '-'."""
         self.__handle_base_token(TT.MINUS)
 
     def __handle_mul_token(self):
-        """Handle a MUL token '*'
-        """
+        """Handle a MUL token '*'."""
         self.__handle_base_token(TT.MUL)
 
     def __handle_div_token(self):
-        """Handle a DIV token '/'
-        """
+        """Handle a DIV token '/'."""
         self.__handle_base_token(TT.DIV)
 
     def __handle_eq_token(self):
-        """Handle a EQ token '='
-        """
+        """Handle a EQ token '='."""
         self.__handle_base_token(TT.EQ)
 
     def __handle_exclamation_token(self):
-        """Handle a EXCLAMATION token '!'
-        """
+        """Handle a EXCLAMATION token '!'."""
         self.__handle_base_token(TT.EXCLAMATION)
 
     def __handle_lt_token(self):
-        """Handle a LT token '<'
-        """
+        """Handle a LT token '<'."""
         self.__handle_base_token(TT.LT)
 
     def __handle_gt_token(self):
-        """Handle a GT token '>'
-        """
+        """Handle a GT token '>'."""
         self.__handle_base_token(TT.GT)
 
     def __handle_pow_token(self):
-        """Handle a POW token '^'
-        """
+        """Handle a POW token '^'."""
         self.__handle_base_token(TT.POW)
 
     def __handle_hash_token(self) -> None:
-        """Handle a HASH token '#'
+        """Handle a HASH token '#'.
 
         Sets a variable to indicate that the following literal is a Variable
         """
         self.__handle_current_token()
         self.__update_position()
         self.__lexerPosition.isVariable = True
 
     def __handle_whitespace(self) -> None:
-        """Handle a WHITESPACE token ' '
+        """Handle a WHITESPACE token ' '.
 
         Replaces 4 following whitespaces by a TAB token
         """
         self.__handle_current_token()
         self.__add_base_token(TT.WHITESPACE)
         self.__lexerPosition.next_column()
         self.__lexerPosition.reset_current_token()
@@ -382,40 +367,38 @@
             self.__rm_last_tokens(4)
             self.__add_base_token(TT.TAB)
             self.__lexerPosition.next_column(4)
             self.__lexerPosition.reset_consecutive_whitespaces()
             self.__lexerPosition.set_current_token_index()
 
     def __handle_newline_token(self) -> None:
-        """Handle a NEWLINE token '\\n'
-        """
+        r"""Handle a NEWLINE token '\\n'."""
         if not self.__lexerPosition.isMultiLine:
             self.__handle_base_token(TT.NEWLINE)
 
         self.__lexerPosition.new_line()
         if not self.__lexerPosition.isMultiLine:
             self.__lexerPosition.set_current_token_index()
 
         self.__lexerPosition.isMultiLine = False
 
     def __handle_backslash_token(self) -> None:
-        """Handle a BACKSLASH token '\\'
+        r"""Handle a BACKSLASH token '\\'.
 
         Sets a variable to indicate that the following line is part of the same token.
         """
         self.__lexerPosition.isMultiLine = True
         self.__lexerPosition.next_column()
 
     def __handle_tab_token(self) -> None:
-        """Handle a TAB token '\\t'
-        """
+        r"""Handle a TAB token '\\t'."""
         self.__handle_base_token(TT.TAB)
 
     def __handle_quotes(self, char) -> None:
-        """Handle a DOUBLEQUOTES token '"'
+        """Handle a DOUBLEQUOTES token '"'.
 
         Sets a variable to indicate that the following characters are a STRING token.
         """
 
         def quote_handler(self=self):
 
             if self.__lexerPosition.isQuotedString:
@@ -432,94 +415,84 @@
                 self.__lexerPosition.next_column()
                 self.__lexerPosition.isQuotedString = char
                 self.__lexerPosition.reset_current_token()
 
         return quote_handler
 
     def __handle_amount_token(self):
-        """Handle an AMOUNT token 'amount'
-        """
+        """Handle an AMOUNT token 'amount'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.AMOUNT, is_current_token=True)
 
     def __handle_and_token(self):
-        """Handle an AND token 'and'
-        """
+        """Handle an AND token 'and'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.AND, is_current_token=True)
 
     def __handle_if_token(self):
-        """Handle an IF token 'if'
-        """
+        """Handle an IF token 'if'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.IF, is_current_token=True)
 
     def __handle_elif_token(self):
-        """Handle an ELIF token 'elif'
-        """
+        """Handle an ELIF token 'elif'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.ELIF, is_current_token=True)
 
     def __handle_else_token(self):
-        """Handle an ELSE token 'else'
-        """
+        """Handle an ELSE token 'else'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.ELSE, is_current_token=True)
 
     def __handle_not_token(self):
-        """Handle an OR token 'or'
-        """
+        """Handle an OR token 'or'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.NOT, is_current_token=True)
 
     def __handle_or_token(self):
-        """Handle an OR token 'or'
-        """
+        """Handle an OR token 'or'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(TT.OR, is_current_token=True)
 
     def __handle_boolean_token(self):
-        """Handle a BOOLEAN token 'true' or 'false'
-        """
+        """Handle a BOOLEAN token 'true' or 'false'."""
         self.__lexerPosition.reset_consecutive_whitespaces()
         self.__add_base_token(
             TT.BOOLEAN, self.__lexerPosition.currentToken, True,
         )
 
     def __handle_eof_token(self) -> None:
-        """Add an EOF token at the end of each file
-        """
+        """Add an EOF token at the end of each file."""
         self.__add_base_token(TT.EOF)
 
     def __add_token_to_list(self, token: Token | None) -> None:
-        """Add a new token to the parser's token list
+        """Add a new token to the parser's token list.
 
         Parameters
         ----------
         token : Token | None
             New token to add
         """
         if not token:
             pass
         self.tokenList.append(token)
 
     def __rm_last_tokens(self, amount: int = 1):
         self.tokenList = self.tokenList[:-amount]
 
     def __end_file(self) -> None:
-        """Add a NEWLINE and an EOF token at the end of each file
-        """
+        """Add a NEWLINE and an EOF token at the end of each file."""
         if len(self.__lexerPosition.currentToken.strip()) > 0:
             self.__handle_current_token()
             self.__lexerPosition.reset_current_token()
         self.__handle_newline_token()
         self.__handle_eof_token()
 
     def __isfloat(self, num: str) -> bool:
-        """Check if the string is a float
+        """Check if the string is a float.
 
         Parameters
         ----------
         num : str
             The input string to check
 
         Returns
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.7/thipster/parser/dsl_parser/lexer_position.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Module to represent the state and position of the lexer."""
 from thipster.engine.parsed_file import Position
 
 
 class LexerPosition():
+    """Represents the state and position of the DSL lexer."""
+
     def __init__(
         self,
         filename: str = '',
     ) -> None:
-        """Class to represent the state and position of the lexer
+        """Represent the state and position of the DSL lexer.
 
         Parameters
         ----------
         filename : str
             Name of the current file
         """
         self.currentFile = filename
@@ -22,84 +25,83 @@
         self.isVariable = False
         self.isQuotedString = False
         self.isMultiLine = False
         self.consecutiveWhitespaces = 0
 
     @property
     def currentCharPosition(self) -> Position:  # noqa: N802
+        """Get the current position of the lexer."""
         return Position(
             self.currentFile,
             self.currentLine,
             self.currentColumn,
         )
 
     @property
     def currentTokenPosition(self) -> Position:  # noqa: N802
+        """Get the position of the current stored token."""
         return Position(
             self.currentFile,
             self.__currentTokenLine,
             self.currentTokenIndex,
         )
 
     def new_line(self) -> None:
-        """Get the position to the next line
-        """
+        """Get the position to the next line."""
         self.currentLine += 1
         self.currentColumn = 1
 
     def next_column(self, step: int = 1) -> None:
-        """Get the position to a new column
+        """Get the position to a new column.
 
         Parameters
         ----------
         step : int
             Step to modify the current column, by default 1
         """
         if (self.currentColumn + step) > 0:
             self.currentColumn += step
         else:
             self.currentColumn = 0  # Raise exception ?
 
     def add_to_current_token(self, char) -> None:
-        """Add a char to the current stored token
+        """Add a char to the current stored token.
 
         Parameters
         ----------
         char : _type_
             Char to add to the token
         """
         self.currentToken += char
 
     def set_current_token_index(self, new_index: int | None = None) -> None:
-        """Modify the stored token index
+        """Modify the stored token index.
 
         Parameters
         ----------
         new_index : int, optional
             New index of the stored token, by default None
         """
         if new_index:
             self.currentTokenIndex = new_index
         else:
             self.currentTokenIndex = self.currentColumn
             self.__currentTokenLine = self.currentLine
 
     def reset_current_token(self, new_index: int | None = None) -> None:
-        """Reset the current stored token and its index
+        """Reset the current stored token and its index.
 
         Parameters
         ----------
         new_index : int, optional
             New index of the stored token, by default None
         """
         self.currentToken = ''
         self.set_current_token_index(new_index)
 
     def increment_consecutive_whitespaces(self) -> None:
-        """Add a consecutive whitespace to the lexer state
-        """
+        """Add a consecutive whitespace to the lexer state."""
         self.consecutiveWhitespaces += 1
 
     def reset_consecutive_whitespaces(self) -> None:
-        """Reset consecutive whitespaces of the lexer state to 0
-        """
+        """Reset consecutive whitespaces of the lexer state to 0."""
         self.consecutiveWhitespaces = 0
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.7/thipster/parser/dsl_parser/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,72 @@
+"""Module that contains the THipster DSL Parser."""
 import os
+from pathlib import Path
 
 from thipster.engine import ParserPort
 from thipster.engine.parsed_file import ParsedFile
 
 from .exceptions import DSLParserBaseError, DSLParserPathNotFoundError
 from .interpreter import Interpreter
 from .lexer import Lexer
 from .token_parser import TokenParser
 
 
 class DSLParser(ParserPort):
+    """Parser for the THipster's DSL."""
 
     @classmethod
     def __getfiles(cls, path: str) -> dict[str, str]:
-        """Recursively get all files in the requested directory and its sudirectories
-        Can be run on a path file aswell
+        """Recursively get all files in the requested directory and its sudirectories.
+
+        Can be run on a path file aswell.
 
         Parameters
         ----------
         path: str
-            Path to run this function into
+            Path to run this function onto
 
         Returns
         -------
         dict[str, str]
             A dictionary that links a filename to its content, fileName : fileContent
         """
+        path = Path(path).resolve().as_posix()
 
-        path = os.path.abspath(path)
-
-        if not os.path.exists(path):
+        if not Path(path).exists():
             raise DSLParserPathNotFoundError(path)
 
         files = {}
 
-        if os.path.isdir(path):
+        if Path(path).is_dir():
             for content in os.listdir(path):
                 files.update(DSLParser.__getfiles(f'{path}/{content}'))
 
-        if os.path.isfile(path):
-            with open(path) as f:
+        if Path(path).is_file():
+            with Path(path).open() as f:
                 files.update({path: f.read()})
 
                 f.close()
 
         return files
 
     @classmethod
     def run(cls, path: str) -> ParsedFile:
-        """Run the DSLParser
+        """Run the DSLParser.
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
-
         try:
             files = DSLParser.__getfiles(path)
             lexer = Lexer(files)
             token_list = lexer.run()
             parser = TokenParser(token_list)
             ast = parser.run()
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/token.py` & `thipster-0.17.7/thipster/parser/dsl_parser/token.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Module containing the Token class and the TOKENTYPES enum."""
 from enum import Enum
 
 from thipster.engine.parsed_file import Position
 
 
 class TOKENTYPES(Enum):
+    """Contains all the possible token types."""
+
     AMOUNT = 'AMOUNT'
     AND = 'AND'
     BOOLEAN = 'BOOLEAN'
     BRACKETS_START = 'BRACKETS_START'
     BRACKETS_END = 'BRACKETS_END'
     COLON = 'COLON'
     COMMA = 'COMMA'
@@ -38,26 +41,27 @@
     NE = 'NE'
     LT = 'LT'
     LTE = 'LTE'
     GT = 'GT'
     GTE = 'GTE'
 
     def __str__(self) -> str:
+        """Return the string representation of the token type."""
         return self.value
 
 
 class Token():
-    """Class representing a Token
-    """
+    """Represents a Token of the THipster DSL."""
 
     def __init__(
         self, position: Position,
         token_type: TOKENTYPES, value: str | None = None,
     ):
         """
+        Represent a Token.
 
         Parameters
         ----------
         position : Position
             Position of the token in its input file
         tokenType : str
             Token type
@@ -65,26 +69,30 @@
             Token value, by default None
         """
         self.position = position
         self.token_type = token_type
         self.value = value
 
     def __eq__(self, __value: object) -> bool:
-        if isinstance(__value, Token):
-            return (
-                self.position == __value.position and
-                self.token_type == __value.token_type and
-                self.value == __value.value
-            )
-        else:
-            raise TypeError('Value must be a Token')
+        """Check if two tokens are equal."""
+        if not isinstance(__value, Token):
+            msg = 'Value must be a Token'
+            raise TypeError(msg)
+
+        return (
+            self.position == __value.position and
+            self.token_type == __value.token_type and
+            self.value == __value.value
+        )
 
     def __repr__(self) -> str:
-        token_string = f'(Type: {str(self.token_type)}, Position: {str(self.position)}'
+        """Return the string representation of the token."""
+        token_string = f'(Type: {self.token_type!s}, Position: {self.position!s}'
         if self.value:
             token_string += f', Value: {self.value}'
         token_string += ')'
 
         return token_string
 
     def __str__(self) -> str:
+        """Return the string value of the token."""
         return f'({self.token_type} {self.value})'
```

### Comparing `thipster-0.17.6/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.7/thipster/parser/dsl_parser/token_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+"""THipster DSL token parser module."""
 import thipster.parser.dsl_parser.ast as ast
 
 from .exceptions import (
     DSLConditionError,
     DSLSyntaxError,
     DSLUnexpectedEOFError,
 )
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
 class TokenParser():
+    """Parse the tokens into an AST (Abstract Syntax Tree)."""
+
     def __init__(self, tokens: list[Token]) -> None:
+        """Parse the tokens into an AST (Abstract Syntax Tree).
+
+        Parameters
+        ----------
+        tokens : list[Token]
+            The list of tokens to parse.
+        """
         self.__tokens = tokens
 
     def run(self) -> ast.FileNode:
+        """Run the parser."""
         self.__rm_empty_lines()
         tree = ast.FileNode()
         try:
             self.__trim_newlines()
             while self.__get_next_type() != TT.EOF:
                 self.__trim_newlines()
 
@@ -25,36 +36,73 @@
                 self.__trim_newlines()
         except Exception as e:
             raise e
 
         return tree
 
     def __next(self, expected: TT | list[TT] | None = None) -> Token:
-        """Get next token and pop it from the list"""
+        """Get next token and pop it from the list.
+
+        Parameters
+        ----------
+        expected : TT | list[TT] | None
+            Expected token type(s), by default None
+
+        Returns
+        -------
+        Token
+            The next token
+        """
         next_token_type = self.__get_next_type()
 
         if expected:
             if type(expected) is list:
                 if next_token_type not in expected:
                     raise DSLSyntaxError(self.__tokens[0], expected)
             elif next_token_type != expected:
                 raise DSLSyntaxError(self.__tokens[0], expected)
         return self.__tokens.pop(0)
 
     def __check(self, expected: TT, index: int = 0) -> Token | None:
-        """Check if the type of the next token is equal to the expected parameter. \
-        Pop it from the list in that case"""
+        """Check if the next token is the expected one.
+
+        If the type of the next token is equal to the expected parameter, it is popped
+        from the list.
+
+        Parameters
+        ----------
+        expected : TT
+            Expected token type
+        index : int, optional
+            Index of the token to check, by default 0
+
+        Returns
+        -------
+        Token | None
+            The next token if it is the expected one, None otherwise
+        """
         token = self.__get_next_type(index=index)
         if token != expected:
             return None
 
         return self.__next(expected)
 
-    def __get_next_type(self, index: int = 0):
-        """Get the type of the next token"""
+    def __get_next_type(self, index: int = 0) -> TT:
+        """Get the type of the next token.
+
+        Parameters
+        ----------
+        index : int, optional
+            Index of the token to get, by default 0
+
+        Returns
+        -------
+        TT
+            The type of the next token
+        """
         if len(self.__tokens) <= index:
             raise DSLUnexpectedEOFError
 
         return self.__tokens[index].token_type
 
     def __trim_newlines(self):
         while self.__check(TT.NEWLINE):
@@ -81,28 +129,32 @@
         return newline
 
     def __get_whitespaces(self):
         while self.__check(TT.WHITESPACE):
             pass
 
     def __get_tabs(self, indent: int) -> bool:
-        """Check if the number of tabs is correct/ if it is the end of the block"""
-
+        """Check if the number of tabs is correct/ if it is the end of the block."""
         if self.__get_next_type() == TT.EOF:
             return False
-        elif self.__get_next_type(indent-1) == TT.TAB:
+        if self.__get_next_type(indent-1) == TT.TAB:
             for _ in range(indent):
                 self.__next(TT.TAB)
             return True
         return False
 
-    def __create_resource(self, indent=0) \
-            -> ast.ResourceNode | ast.IfNode | ast.AmountNode:
-        """type, name, ":", [amt_ctrl], [if_ctrl] ,"\\n"
-                                (list | dict | {parameter, "\\n"})"""
+    def __create_resource(
+        self,
+        indent=0,
+    ) -> ast.ResourceNode | ast.IfNode | ast.AmountNode:
+        r"""Create an AST Resouce, If or Amount node.
+
+        Format: type, name, ":", [amt_ctrl], [if_ctrl] ,"\\n"
+        (list | dict | {parameter, "\\n"}).
+        """
         try:
             for _ in range(indent):
                 self.__next(TT.TAB)
 
             resource_type = self.__get_type()
             self.__get_whitespaces()
             name = self.__get_string_expr()
@@ -135,15 +187,18 @@
         if nb_ctrl:
             nb_ctrl.node = resource
             resource = nb_ctrl
 
         return resource
 
     def __get_parameter(self, indent: int) -> ast.ParameterNode:
-        """name, ":", (value, [if_else_ctrl] | [if_ctrl], "\\n", (list | dict))"""
+        r"""Create an AST Parameter node.
+
+        Format: name, ":", (value, [if_else_ctrl] | [if_ctrl], "\\n", (list | dict)).
+        """
         try:
             name = self.__next(TT.STRING)
             self.__get_whitespaces()
             self.__next(TT.COLON)
             self.__get_whitespaces()
         except DSLSyntaxError as e:
             raise e
@@ -197,15 +252,17 @@
         if if_ctrl:
             if_ctrl.if_case = parameter
             parameter = if_ctrl
 
         return parameter
 
     def __get_properties(self, indent: int) -> list[ast.ParameterNode]:
-        """(list | dict)
+        """Create a list of AST Parameter nodes.
+
+        Format: (list | dict).
         """
         i = indent
         try:
             next_token_type = self.__get_next_type(indent)
             while next_token_type == TT.WHITESPACE:
                 i += 1
                 next_token_type = self.__get_next_type(i)
@@ -227,15 +284,18 @@
                 raise DSLUnexpectedEOFError from eof.__cause__
 
             props = ast.DictNode([])
 
         return props
 
     def __get_list(self, indent: int) -> ast.ListNode:
-        """{ "-", value, [amt_ctrl], [if_else_ctrl], "\\n"}"""
+        r"""Create an AST List node.
+
+        Format: { "-", value, [amt_ctrl], [if_else_ctrl], "\\n"}.
+        """
         list_items = []
 
         try:
             while self.__get_tabs(indent):
                 self.__check(TT.MINUS)
                 self.__get_whitespaces()
 
@@ -297,15 +357,17 @@
                 self.__get_whitespaces()
         else:
             self.__next(TT.BRACKETS_END)
 
         return ast.ListNode(list_items)
 
     def __get_dict(self, indent: int) -> ast.DictNode:
-        """{ parameter, "\\n" }
+        r"""Create an AST Dict node.
+
+        Format: { parameter, "\\n" }.
         """
         parameters = []
 
         try:
             while self.__get_tabs(indent):
                 self.__get_whitespaces()
                 parameters.append(self.__get_parameter(indent))
@@ -320,16 +382,18 @@
                 token_type=TT.NEWLINE,
             ),
         )
 
         return ast.DictNode(parameters)
 
     def __get_nb_ctrl(self) -> ast.AmountNode | None:
-        """"amount", ":", int, ["#", var]"""
+        """Create an AST Amount node.
 
+        Format: "amount", ":", int, ["#", var].
+        """
         try:
             amount_token = self.__check(TT.AMOUNT)
             if not amount_token:
                 return None
 
             self.__get_whitespaces()
             self.__next(TT.COLON)
@@ -350,16 +414,18 @@
                 amount_variable, ast.IntNode(Token(None, TT.INT, 1)),
             )
             if amount_variable else None,
             node=None,
         )
 
     def __get_if_ctrl(self) -> ast.IfNode | None:
-        """"if", condition"""
+        """Create an AST If node.
 
+        Format: "if", condition.
+        """
         condition = self.__check(TT.IF)
         if not condition:
             return None
 
         self.__get_whitespaces()
         try:
             condition = self.__get_comp_expr()
@@ -369,15 +435,18 @@
 
         return ast.IfNode(
             condition=condition,
             if_case=None,
         )
 
     def __get_if_else_ctrl(self) -> ast.IfElseNode | None:
-        """if_ctrl, ["else" , valeur]"""
+        """Create an AST IfElse node.
+
+        Format: if_ctrl, ["else" , value].
+        """
         if_ctrl = self.__get_if_ctrl()
         self.__get_whitespaces()
         if not if_ctrl:
             return None
 
         if self.__check(TT.ELSE):
             self.__get_whitespaces()
```

### Comparing `thipster-0.17.6/thipster/parser/parser_factory.py` & `thipster-0.17.7/thipster/parser/parser_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,82 @@
+"""ParserFactory module."""
 import os
+from pathlib import Path
 
 from thipster.engine import ParserPort
 from thipster.engine.parsed_file import ParsedFile
 
 from .dsl_parser import DSLParser
 from .exceptions import (
     NoFileFoundError,
     ParserPathNotFoundError,
 )
 from .yaml_parser import YAMLParser
 
 
 class NoParser(ParserPort):
+    """Used when no parser is found for a file extension."""
+
     @classmethod
-    def run(cls, path) -> ParsedFile:
+    def run(cls, path) -> ParsedFile:  # noqa: ARG003
+        """Run the Parser."""
         return ParsedFile()
 
 
 class ParserFactory(ParserPort):
+    """Parser factory, used to run the right parser on the right file."""
 
     __parsers = {
         '.yaml': YAMLParser,
         '.yml': YAMLParser,
         '.jinja': YAMLParser,
         '.thips': DSLParser,
     }
 
     @classmethod
     def add_parser(cls, parser: ParserPort, extensions: list[str]):
+        """Add a parser to the ParserFactory."""
         cls.__parsers.update({e: parser for e in extensions})
 
     @classmethod
     def __getfiles(cls, path: str) -> list[str]:
-        """Recursively get all files names in the requested directory and its\
-              sudirectories
-        Can be run on a path file aswell
+        """Get the file(s) on the requested path.
+
+        Recursively get all files names in the requested directory and its
+        sudirectories. Can be run on a path file as well.
 
         Parameters
         ----------
         path: str
-            Path to run this function into
+            Path to run this function onto
 
         Returns
         -------
         list[str]
             A list of all the filenames
         """
+        path = Path(path).resolve().as_posix()
 
-        path = os.path.abspath(path)
-
-        if not os.path.exists(path):
+        if not Path(path).exists():
             raise ParserPathNotFoundError(path)
 
         files = []
 
-        if os.path.isdir(path):
+        if Path(path).is_dir():
             for content in os.listdir(path):
                 files += cls.__getfiles(f'{path}/{content}')
 
-        if os.path.isfile(path):
+        if Path(path).is_file():
             return [path]
 
         return files
 
     @classmethod
     def run(cls, path: str) -> ParsedFile:
-        """Run the ParserFactory
+        """Run the ParserFactory.
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
@@ -88,12 +95,12 @@
             raise NoFileFoundError(path)
 
         return res
 
     @classmethod
     def __get_parser(cls, path) -> ParserPort:
 
-        _, path_extension = os.path.splitext(path)
+        path_extension = Path(path).suffix
 
         return cls.__parsers.get(
             path_extension, NoParser,
         )
```

### Comparing `thipster-0.17.6/thipster/parser/yaml_parser.py` & `thipster-0.17.7/thipster/parser/yaml_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,88 @@
+"""YAML Parser module."""
 import os
 from abc import ABC
+from pathlib import Path
 
 import yaml
 from jinja2 import Environment, FileSystemLoader
 
 import thipster.engine.parsed_file as pf
 from thipster.engine import ParserPort, THipsterError
 
 from .exceptions import ParserPathNotFoundError
 
 
 class YAMLParserBaseError(THipsterError, ABC):
+    """Base error for YAMLParser."""
+
     def __init__(self, *args: object) -> None:
+        """Shared base exception for the YAML parser."""
         super().__init__(*args)
 
 
 class YAMLParserNoNameError(YAMLParserBaseError):
+    """Error raised when a resource has no name."""
+
     def __init__(self, resource, *args: object) -> None:
+        """Error raised when a resource has no name.
+
+        Parameters
+        ----------
+        resource
+            The resource that has no name.
+        """
         super().__init__(*args)
         self.resource = resource
 
     @property
     def message(self) -> str:
+        """Return the error message."""
         return f'No name for resource : {self.resource}'
 
 
 class YAMLParser(ParserPort):
+    """YAMLParser class, used to parse YAML files."""
+
     @classmethod
     def __getfiles(cls, path: str) -> list[str]:
-        """Recursively get all files names in the requested directory and its\
-              sudirectories
-        Can be run on a path file aswell
+        """Get the file(s) on the requested path.
+
+        Recursively get all files names in the requested directory and its
+        sudirectories. Can be run on a path file as well.
 
         Parameters
         ----------
         path: str
-            Path to run this function into
+            Path to run this function onto
 
         Returns
         -------
         list[str]
             A list of all the filenames
         """
-        path = os.path.abspath(path)
+        path = Path(path).resolve().as_posix()
 
-        if not os.path.exists(path):
+        if not Path(path).exists():
             raise ParserPathNotFoundError(path)
 
         files = []
 
-        if os.path.isdir(path):
+        if Path(path).is_dir():
             for content in os.listdir(path):
                 files += cls.__getfiles(f'{path}/{content}')
 
-        if os.path.isfile(path):
+        if Path(path).is_file():
             return [path]
 
         return files
 
     @classmethod
     def run(cls, path: str) -> pf.ParsedFile:
-        """Run the YAMLParser
+        """Run the YAMLParser.
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
@@ -95,15 +113,15 @@
         except YAMLParserBaseError as e:
             raise e
         except Exception as e:
             raise e
 
     @classmethod
     def __convert(cls, file: dict) -> list[pf.ParsedResource]:
-        """Converts a dictionnary into a list of ParsedResources
+        """Convert a dictionnary into a list of ParsedResources.
 
         Parameters
         ----------
         file: dict
             Dict to convert
 
         Returns
@@ -112,44 +130,44 @@
             Converted dict
         """
         resources = []
 
         for key, val in file.items():
             if type(val) == list:
                 for res in val:
-                    if 'name' in res:
-                        name = res['name']
-                        del res['name']
-                    else:
+                    if 'name' not in res:
                         raise YAMLParserNoNameError(key)
 
+                    name = res['name']
+                    del res['name']
+
                     resources.append(
                         cls.__get_resource(
                             content=res, resource_type=key, name=name,
                         ),
                     )
             elif type(val) == dict:
-                if 'name' in val:
-                    name = val['name']
-                    del val['name']
-                else:
+                if 'name' not in val:
                     raise YAMLParserNoNameError(key)
 
+                name = val['name']
+                del val['name']
+
                 resources.append(
                     cls.__get_resource(
                         content=val, resource_type=key, name=name,
                     ),
                 )
 
         return resources
 
     @classmethod
     def __get_resource(cls, content: dict, resource_type: str, name: str)\
             -> pf.ParsedResource:
-        """Converts a dict in a ParsedResource
+        """Convert a dict in a ParsedResource.
 
         Parameters
         ----------
         content: dict
             Dict of attributes of the resource
         resourceType: str
             Type of the resource
@@ -163,23 +181,23 @@
         """
         attr = []
 
         for key, val in content.items():
             attr.append(cls.__get__attr(key, val))
 
         return pf.ParsedResource(
-            type=resource_type,
+            parsed_resource_type=resource_type,
             name=name,
             position=None,
             attributes=attr,
         )
 
     @classmethod
     def __get__attr(cls, name: str, value: object) -> pf.ParsedAttribute:
-        """Converts an object in a ParsedAttribute
+        """Convert an object in a ParsedAttribute.
 
         Parameters
         ----------
         value: object
             Object to convert
         name: str
             Name of the attribute
@@ -199,50 +217,50 @@
         return pf.ParsedAttribute(
             name=name,
             value=val,
             position=None,
         )
 
     @classmethod
-    def __get_dict(cls, input: dict) -> pf.ParsedDict:
-        """Converts a dict into a list of ParsedDict
+    def __get_dict(cls, input_dict: dict) -> pf.ParsedDict:
+        """Convert a dict into a list of ParsedDict.
 
         Parameters
         ----------
-        input: dict
+        input_dict: dict
             Dict to convert
 
         Returns
         -------
         ParsedDict
             Converted dict
         """
         attr = []
 
-        for key, val in input.items():
+        for key, val in input_dict.items():
             attr.append(cls.__get__attr(key, val))
 
         return pf.ParsedDict(attr)
 
     @classmethod
-    def __get_list(cls, input: list) -> pf.ParsedList:
-        """Converts a dictionnary into a ParsedList
+    def __get_list(cls, input_list: list) -> pf.ParsedList:
+        """Convert a dictionnary into a ParsedList.
 
         Parameters
         ----------
-        input: list
+        input_list: list
             List to convert
 
         Returns
         -------
         ParsedList
             Converted list
         """
         attr = []
 
-        for val in input:
+        for val in input_list:
             if isinstance(val, dict):
                 attr.append(cls.__get_dict(val))
             else:
                 attr.append(pf.ParsedLiteral(val))
 
         return pf.ParsedList(attr)
```

### Comparing `thipster-0.17.6/thipster/repository/github.py` & `thipster-0.17.7/thipster/repository/github.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-"""GithubRepo.py module
-"""
+"""GithubRepo.py module."""
 
 import requests
 
 from .exceptions import ModelNotFoundError
 from .json import JSONRepo
 
 
 class GithubRepo(JSONRepo):
-    """Class representing a GitHub resources Repository
+    """Represents a GitHub resources Repository.
 
     JSON Models of resources and services offered by supported cloud providers are
     stored in a repository.
     This class is used to access those models if they are located in a GitHub repo.
     """
 
     def __init__(self, repo: str, branch: str = 'main') -> None:
-        """
+        """Represent a GitHub resources Repository.
+
+        JSON Models of resources and services offered by supported cloud providers are
+        stored in a repository.
+        This class is used to access those models if they are located in a GitHub repo.
+
         Parameters
         ----------
         repo : str
             Name of the repository, for example : 'THipster/models'
         branch : str, optional
             Name of the branch, by default 'main'
         """
         super().__init__()
         self.__repo = repo
         self.__branch = branch
 
     def get_json(self, name: str) -> str | bytes | bytearray:
-        """Method to get the json file from the GitHub repository
+        """Get the json file from the GitHub repository.
 
         Parameters
         ----------
         name : str
             Name of the desired resource
 
         Returns
```

### Comparing `thipster-0.17.6/thipster/repository/json.py` & `thipster-0.17.7/thipster/repository/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-"""JSONRepo.py module.
-"""
+"""JSONRepo.py module."""
 
 import json
 from abc import ABC, abstractmethod
 
 import thipster.engine.resource_model as rm
 from thipster.engine import RepositoryPort
 
 
 class JSONRepo(RepositoryPort, ABC):
-    _parent_stack = []
-    """Class representing a JSON resources Repository
+    """Represents a JSON resources Repository.
 
     JSON Models of resources and services offered by supported cloud providers are
     stored in a repository.
     """
 
+    _parent_stack = []
+
     def __init__(self) -> None:
+        """Represent a JSON resources Repository.
+
+        JSON Models of resources and services offered by supported cloud providers are
+        stored in a repository.
+        """
         super().__init__()
         self.model_list = {}
 
     @abstractmethod
     def get_json(self, name: str) -> str | bytes | bytearray:
-        raise Exception()
+        """Get the JSON file corresponding to the name given."""
+        raise Exception
 
     def get(self, resource_names: list[str]) -> dict[str, rm.ResourceModel]:
-        """Get the corresponding resource Models from a list of names
+        """Get the corresponding resource Models from a list of names.
 
         Parameters
         ----------
         resourceNames : list[str]
             List of the desired resource models names
 
         Returns
@@ -39,125 +45,117 @@
         """
         for resource in resource_names:
             self.__add_model(resource)
 
         return self.model_list
 
     def __create_value(self, val: object | None) -> rm.ModelValue | None:
-        """Creates the right Model value implementation from the raw JSON
+        """Create the right Model value implementation from the raw JSON.
 
         Parameters
         ----------
         val : object
             Raw JSON model's attribute value
 
         Returns
         -------
         ModelValue | None
             Value of the attribute, implementation of ModelValue : ModelDict,
             ModelList, ModelLiteral or None
         """
         if val is None:
             return None
-        elif isinstance(val, dict):
+        if isinstance(val, dict):
             return rm.ModelDict(None)
-        elif isinstance(val, list):
+        if isinstance(val, list):
             return rm.ModelList([self.__create_value(i) for i in val])
 
         return rm.ModelLiteral(val)
 
     def __create_attribute(self, raw: dict[str, str]) -> list[rm.ModelAttribute]:
-        """Creates a model's attributes from the raw JSON input
+        """Create a model's attributes from the raw JSON input.
 
         Parameters
         ----------
         raw : dict[str, str]
             Json model's raw attributes
 
         Returns
         -------
         list[ModelAttribute]
             Attributes of the resource model
         """
-
         attributes = {}
 
         for name, attr in raw.items():
-            optional = attr['optional'] if 'optional' in attr.keys(
-            ) else True
+            optional = attr['optional'] if 'optional' in attr else True
 
-            value = attr['default'] if 'default' in attr.keys(
-            ) else None
+            value = attr['default'] if 'default' in attr else None
 
-            is_list = 'list' in attr['var_type'] if 'var_type' in attr.keys(
-            ) else False
+            is_list = 'list' in attr['var_type'] if 'var_type' in attr else False
 
             default = self.__create_value(value)
 
             attributes[name] = rm.ModelAttribute(
                 attr['cdk_key'],
                 default=default,
                 optional=optional,
                 is_list=is_list,
             )
 
         return attributes
 
     def __create_model(self, name: str) -> rm.ResourceModel:
-        """Get's the json file and creates a Resource Model
+        """Get the json file and create a Resource Model.
 
         Parameters
         ----------
         name : str
             Name of the model to find
 
         Returns
         -------
         ResourceModel
             Resource model corresponding to the name given
         """
-
         model = self.get_json(name)
 
         json_model = json.loads(model)
 
         for _, dep in json_model['dependencies'].items():
             if dep['resource'] not in self.model_list.keys():
                 self.__add_model(dep['resource'])
 
         for _, internal_object in json_model['internalObjects'].items():
             if internal_object['resource'] not in self.model_list.keys():
                 self.__add_model(internal_object['resource'])
 
-        res = rm.ResourceModel(
+        return rm.ResourceModel(
             name,
             attributes=self.__create_attribute(json_model['attributes']),
             dependencies=json_model['dependencies'],
             internal_objects=json_model['internalObjects'],
             name_key=json_model['cdk_name_key']
             if 'cdk_name_key' in json_model else None,
             cdk_provider=json_model['cdk_provider'],
             cdk_module=json_model['cdk_module'],
             cdk_name=json_model['cdk_class'],
         )
 
-        return res
-
     def __add_model(self, model: str) -> rm.ResourceModel:
-        """Add a model to the list
+        """Add a model to the list.
 
         Parameters
         ----------
         model : str
             Name of the model to add
 
         Returns
         -------
         ResourceModel
             Resource model corresponding to the name given
         """
-
         if model not in self.model_list.keys():
             self.model_list[model] = None
             self.model_list[model] = self.__create_model(model)
 
         return self.model_list[model]
```

### Comparing `thipster-0.17.6/thipster/terraform/cdk.py` & `thipster-0.17.7/thipster/terraform/cdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""THipster's Terraform CDK module."""
 import copy
 import importlib
 import os
 import shutil
 import subprocess
 import sys
 import uuid
@@ -15,27 +16,54 @@
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
 from thipster.engine import AuthPort, TerraformPort
 from thipster.helpers import create_logger
 
 
 class ResourceCreationContext:
+    """Context from which a resource is created."""
+
     def __init__(
         self,
         stack_self: TerraformStack,
         resource_name: str | None = None,
         resource_type: str | None = None,
         resource_class: type | None = None,
         parent_name: str | None = None,
         parent_type: str | None = None,
         parent_args: dict | None = {},
         arg_to_complete: str | None = None,
         no_modif: bool = True,
         no_dependencies: bool = False,
     ):
+        """Context from which a resource is created.
+
+        Parameters
+        ----------
+        stack_self : TerraformStack
+            Stack in which the resource is created
+        resource_name : str, optional
+            Name of the resource, default None
+        resource_type : str, optional
+            Type of the resource, default None
+        resource_class : type, optional
+            Class of the resource (Python CDK), default None
+        parent_name : str, optional
+            Name of the parent resource, default None
+        parent_type : str, optional
+            Type of the parent resource, default None
+        parent_args : dict, optional
+            Arguments of the parent resource, default {}
+        arg_to_complete : str, optional
+            Name of the argument to complete, default None
+        no_modif : bool, optional
+            If the resource is created with default values, default True
+        no_dependencies : bool, optional
+            If the resource is created without dependencies, default False
+        """
         self.stack_self = stack_self
 
         self.model: rm.ResourceModel = None
         self.dependencies = None
         self.__resource_type = None
 
         # Parent resource info
@@ -69,44 +97,51 @@
             parent_name=parent_name,
             parent_type=parent.resource_type,
             parent_args=parent.resource_args,
             **args,
         )
 
     def regenerate(self):
+        """Regenerate resource name."""
         self.resource_name = f'{self.parent_name}-{uuid.uuid4().hex[:8]}'
         return self
 
     @property
     def resource_type(self):
+        """Return resource type."""
         return self.__resource_type
 
     @resource_type.setter
     def resource_type(self, value):
         self.__resource_type = value
 
         if value is not None:
             self.model: rm.ResourceModel = CDK._models[self.resource_type]
             self.dependencies = copy.deepcopy(self.model.dependencies)
             if self.arg_to_complete in self.dependencies:
                 del self.dependencies[self.arg_to_complete]
 
 
 class CDK(TerraformPort):
+    """Terraform code generation and usage.
+
+    Works using the CDK for Terraform in python, and the python_terraform library.
+    """
+
     _models = []
     _parent_resources_stack = []
     _resources_to_create: list[ResourceCreationContext] = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = create_logger(__name__)
 
     @classmethod
     def apply(cls, plan_file_path: str | None = None):
-        """Applies generated Terraform plan.
+        """Apply generated Terraform plan.
 
         Parameters
         ----------
         plan_file_path : str, optional
             Path to the plan file, default None
 
         Returns
@@ -179,26 +214,30 @@
             'Created %s terraform file(s)',
             len(output_directories),
         )
 
         # Move files
         for dirname in output_directories:
             shutil.move(
-                os.path.join(os.getcwd(), dirname, 'cdk.tf.json'),
-                os.path.join(os.getcwd(), 'thipster.tf.json'),
+                Path(Path.cwd(), dirname, 'cdk.tf.json'),
+                Path(Path.cwd(), 'thipster.tf.json'),
             )
 
         # Delete cdktf.out directory
-            for content in os.listdir(os.path.join(os.getcwd(), dirname)):
-                os.remove(f'{dirname}/{content}')
-            os.rmdir(dirname)
-        for content in os.listdir(os.path.join(os.getcwd(), 'cdktf.out')):
+            for content in os.listdir(Path(Path.cwd(), dirname)):
+                if Path(f'{dirname}/{content}').is_dir():
+                    shutil.rmtree(f'{dirname}/{content}')
+                    continue
+
+                Path(f'{dirname}/{content}').unlink()
+            Path(dirname).rmdir()
+        for content in os.listdir(Path(Path.cwd(), 'cdktf.out')):
             d = f'cdktf.out/{content}'
-            os.rmdir(d) if os.path.isdir(d) else os.remove(d)
-        os.rmdir('cdktf.out')
+            Path(d).rmdir() if Path(d).is_dir() else Path(d).unlink()
+        Path('cdktf.out').rmdir()
 
     @classmethod
     def init(cls):
         """Initilize terraform.
 
         Returns
         -------
@@ -251,17 +290,15 @@
 
         Returns
         -------
         type :
             the imported class
         """
         module = importlib.import_module(f'{package_name}.{module_name}')
-        class_ = getattr(module, class_name)
-
-        return class_
+        return getattr(module, class_name)
 
 
 def _create_default_resource(ctx: ResourceCreationContext):
     """Create a resource with all default values.
 
     Parameters
     ----------
@@ -300,38 +337,36 @@
         ]
 
         raise cdk_exceptions.CDKMissingAttributeInDependencyError(
             ctx.resource_type,
             missing_atributes,
         )
 
-    # Import package and class
-    CDK._pip_install(ctx.model.cdk_provider)
-    ctx.resource_class = CDK._import(
-        ctx.model.cdk_provider, ctx.model.cdk_module, ctx.model.cdk_name,
-    )
-
-    if ctx.model.name_key:
-        ctx.resource_args[ctx.model.name_key] = ctx.resource_name
-
     for attribute_name, attribute_value in attributes.items():
-        if not ctx.no_dependencies and attribute_name in ctx.dependencies:
-            _check_explicit_dependency(
-                ctx, attribute_name, attribute_value.default,
-            )
-
-            del ctx.dependencies[attribute_name]
-
-        if attribute_name in ctx.model.attributes:
-            ctx.resource_args[attribute_value.cdk_name] = attribute_value.default
+        _process_attribute(
+            ctx, pf.ParsedAttribute(
+                name=attribute_name,
+                position=None,
+                value=pf.ParsedLiteral(attribute_value.default),
+            ),
+        )
 
     # Create default defendencies if needed
     if not ctx.no_dependencies:
         _generate_default_dependencies(ctx)
 
+    if ctx.model.name_key:
+        ctx.resource_args[ctx.model.name_key] = ctx.resource_name
+
+    # Import package and class
+    CDK._pip_install(ctx.model.cdk_provider)
+    ctx.resource_class = CDK._import(
+        ctx.model.cdk_provider, ctx.model.cdk_module, ctx.model.cdk_name,
+    )
+
     CDK._logger.debug(
         f'Created default {ctx.resource_class} named {ctx.resource_name}',
     )
 
 
 def _create_resource(ctx: ResourceCreationContext, resource_args: object):
     """Create a resource with the given values.
@@ -419,59 +454,49 @@
     -------
     object :
         Created resource
     """
     ctx.resource_name = resource.name
     ctx.resource_type = resource.resource_type
 
-    ctx.no_modif = False
-    ctx.no_dependencies = True
-
-    # Create resource with default values
-    _create_default_resource(ctx)
-    ctx.no_modif = True
-    ctx.no_dependencies = False
-
-    if ctx.model.name_key:
-        ctx.resource_args[ctx.model.name_key] = ctx.resource_name
-
-    def attributes(attribute_list):
-        for attribute in attribute_list:
-            _process_attribute(ctx, attribute)
-
-    attributes(resource.attributes)
-    attributes(CDK._inherited_attributes)
-
-    CDK._inherited_attributes += resource.attributes
-    _generate_default_dependencies(ctx)
-    CDK._inherited_attributes = CDK._inherited_attributes[
-        :-len(
-            resource.attributes,
-        )
-    ]
-
-    return _instantiate_class(ctx)
+    return _create_resource_from_args(ctx, resource.attributes)
 
 
 def _instantiate_class(ctx: ResourceCreationContext):
-    """Instantiates a class.
+    """Instantiate a class.
 
     Parameters
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
 
     Returns
     -------
     object :
         Created resource
     """
     CDK._parent_resources_stack.remove(ctx.resource_type)
 
     if not ctx.arg_to_complete:
+
+        # check args
+        if ctx.no_modif and not all(
+            value.get('optional') or ctx.resource_args.get(name)
+            for name, value in ctx.model.internal_objects.items()
+        ):
+            missing_internal_objects = [
+                name for name, value in ctx.model.internal_objects.items()
+                if not value.get('optional') and not ctx.resource_args.get(name)
+            ]
+
+            raise cdk_exceptions.CDKMissingAttributeInDependencyError(
+                ctx.resource_type,
+                missing_internal_objects,
+            )
+
         if not ctx.model.name_key:
             class_ = ctx.resource_class(**ctx.resource_args)
         else:
             class_ = ctx.resource_class(
                 ctx.stack_self, ctx.resource_name, **ctx.resource_args,
             )
 
@@ -499,15 +524,15 @@
     Parameters
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
     attribute : ParsedAttribute
         Attribute to process
     """
-    if attribute.name in ctx.dependencies:
+    if not ctx.no_dependencies and attribute.name in ctx.dependencies:
         _check_explicit_dependency(ctx, attribute.name, attribute.value)
         del ctx.dependencies[attribute.name]
         return
 
     # Checks if attribute is an internal object
     if attribute.name in ctx.model.internal_objects:
         _create_internal_object(
@@ -663,26 +688,24 @@
             else:
                 _process_attribute(ctx, attribute)
 
     if dependency_attributes:
         attributes(dependency_attributes)
     attributes(CDK._inherited_attributes)
 
-    dependency = ctx.resource_class(
-        ctx.stack_self, ctx.resource_name, **ctx.resource_args,
-    )
-    CDK._parent_resources_stack.remove(ctx.resource_type)
+    dependency = _instantiate_class(ctx)
     return dependency.id
 
 
 def _check_explicit_dependency(
     ctx: ResourceCreationContext, attribute_name: str, attribute_value: str | dict,
 ):
-    """Check if a dependency attribute was explicited before.\
-    Create the dependency if it wasn't.
+    """Check if a dependency attribute was explicited before.
+
+    If it wasn't : create a default dependency.
 
     Parameters
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
     attribute_name: str
         Name of the attribute to check
@@ -700,15 +723,14 @@
                 attribute_name, attribute_value,
             )
 
         dep_ctx = ResourceCreationContext.from_parent(
             ctx,
             resource_type=dependency_type,
         )
-        dep_ctx.resource_args = attribute_value
 
         # Creates explicit dependency
         ctx.resource_args[attribute_name] = _create_dependency(
             dep_ctx, attribute_value,
         )
 
     ctx.resource_args[attribute_name] = CDK._created_resources[created_name]
```

### Comparing `thipster-0.17.6/thipster.egg-info/PKG-INFO` & `thipster-0.17.7/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.6
+Version: 0.17.7
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: test
 Provides-Extra: google
+Provides-Extra: dev
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.7 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-dev Provides-Extra: doc Provides-Extra: google License-File: LICENSE # THipster
-THipster is a tool dedicated to simplifying the difficulty associated with
-writing Terraform files. It allows users to write infrastructure as code in a
-simplified format, using either YAML (with JINJA) or the dedicated Thipster
-DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
-create Terraform files and apply them to the chosen provider.
+Description-Content-Type: text/markdown Provides-Extra: doc Provides-Extra:
+test Provides-Extra: google Provides-Extra: dev License-File: LICENSE #
+THipster THipster is a tool dedicated to simplifying the difficulty associated
+with writing Terraform files. It allows users to write infrastructure as code
+in a simplified format, using either YAML (with JINJA) or the dedicated
+Thipster DSL. Written entirely in Python, it leverages the Python CDK for
+Terraform to create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
                                    versions]
 ## Technology Stack Written in Python 3.11, thipster is designed as a python
 package, to be used either as a standalone tool, or as a module inside a
 running process like a CI/CD pipeline. ## Project Status THipster is currently
 in an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for
```

### Comparing `thipster-0.17.6/thipster.egg-info/SOURCES.txt` & `thipster-0.17.7/thipster.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 tests/parser/test_yamlparser.py
 tests/parser/dsl_parser/__init__.py
 tests/parser/dsl_parser/test_ast.py
 tests/parser/dsl_parser/test_dslparser.py
 tests/parser/dsl_parser/test_lexer.py
 tests/parser/dsl_parser/test_token.py
 tests/parser/dsl_parser/test_tokenparser.py
+tests/repository/__init__.py
+tests/repository/test_github_repository.py
+tests/repository/test_local_repository.py
+tests/repository/test_resourcemodel.py
 thipster/__init__.py
 thipster/helpers.py
 thipster.egg-info/PKG-INFO
 thipster.egg-info/SOURCES.txt
 thipster.egg-info/dependency_links.txt
 thipster.egg-info/requires.txt
 thipster.egg-info/top_level.txt
```

