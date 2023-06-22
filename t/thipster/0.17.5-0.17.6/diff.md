# Comparing `tmp/thipster-0.17.5.tar.gz` & `tmp/thipster-0.17.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.5.tar", last modified: Wed Jun 21 15:27:52 2023, max compression
+gzip compressed data, was "thipster-0.17.6.tar", last modified: Thu Jun 22 08:45:33 2023, max compression
```

## Comparing `thipster-0.17.5.tar` & `thipster-0.17.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.091825 thipster-0.17.5/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 15:27:48.000000 thipster-0.17.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-21 15:27:48.000000 thipster-0.17.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 15:27:52.087824 thipster-0.17.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-21 15:27:48.000000 thipster-0.17.5/README.md
--rw-r--r--   0 root         (0) root         (0)      995 2023-06-21 15:27:48.000000 thipster-0.17.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-21 15:27:48.000000 thipster-0.17.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 15:27:52.091825 thipster-0.17.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 15:27:49.000000 thipster-0.17.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.079825 thipster-0.17.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.079825 thipster-0.17.5/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.079825 thipster-0.17.5/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.083824 thipster-0.17.5/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    15280 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    13619 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/parser/test_yamlparser.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-06-21 15:27:48.000000 thipster-0.17.5/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.083824 thipster-0.17.5/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.083824 thipster-0.17.5/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.083824 thipster-0.17.5/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3105 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.087824 thipster-0.17.5/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.087824 thipster-0.17.5/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9180 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13507 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17026 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20074 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.087824 thipster-0.17.5/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.087824 thipster-0.17.5/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20635 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-21 15:27:48.000000 thipster-0.17.5/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:27:52.083824 thipster-0.17.5/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 15:27:52.000000 thipster-0.17.5/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-21 15:27:52.000000 thipster-0.17.5/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 15:27:52.000000 thipster-0.17.5/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 15:27:52.000000 thipster-0.17.5/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 15:27:52.000000 thipster-0.17.5/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 08:45:29.000000 thipster-0.17.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 08:45:29.000000 thipster-0.17.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 08:45:33.252659 thipster-0.17.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 08:45:29.000000 thipster-0.17.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      995 2023-06-22 08:45:29.000000 thipster-0.17.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 08:45:29.000000 thipster-0.17.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 08:45:33.252659 thipster-0.17.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-22 08:45:29.000000 thipster-0.17.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.240659 thipster-0.17.6/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    15280 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/parser/test_yamlparser.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-22 08:45:29.000000 thipster-0.17.6/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.248659 thipster-0.17.6/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9180 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13507 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17026 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20074 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.252659 thipster-0.17.6/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21404 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-22 08:45:29.000000 thipster-0.17.6/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:45:33.244659 thipster-0.17.6/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 08:45:33.000000 thipster-0.17.6/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.5/LICENSE` & `thipster-0.17.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/PKG-INFO` & `thipster-0.17.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.5
+Version: 0.17.6
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.5 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.6 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.5/README.md` & `thipster-0.17.6/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/pyproject.toml` & `thipster-0.17.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/setup.py` & `thipster-0.17.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.17.5'
+__version__ = '0.17.6'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.5/tests/engine/test_engine.py` & `thipster-0.17.6/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/engine/test_generation.py` & `thipster-0.17.6/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.6/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.17.6/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.6/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.6/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.6/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/test_parsedfile.py` & `thipster-0.17.6/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/test_parserfactory.py` & `thipster-0.17.6/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/parser/test_yamlparser.py` & `thipster-0.17.6/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/test_e2e.py` & `thipster-0.17.6/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/tests/test_tools.py` & `thipster-0.17.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/auth/google.py` & `thipster-0.17.6/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/engine.py` & `thipster-0.17.6/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/i_parser.py` & `thipster-0.17.6/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/i_repository.py` & `thipster-0.17.6/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/i_terraform.py` & `thipster-0.17.6/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/parsed_file.py` & `thipster-0.17.6/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/engine/resource_model.py` & `thipster-0.17.6/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/helpers.py` & `thipster-0.17.6/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.6/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.6/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.6/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.6/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.6/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.6/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/token.py` & `thipster-0.17.6/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.6/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/exceptions.py` & `thipster-0.17.6/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/parser_factory.py` & `thipster-0.17.6/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/parser/yaml_parser.py` & `thipster-0.17.6/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/repository/github.py` & `thipster-0.17.6/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/repository/json.py` & `thipster-0.17.6/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster/terraform/cdk.py` & `thipster-0.17.6/thipster/terraform/cdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,24 +631,46 @@
     )
     if not internal_object_base_ctx.arg_to_complete:
         ctx.resource_args[internal_object_name] = res
 
     return True
 
 
-def _create_dependency(ctx: ResourceCreationContext):
+def _create_dependency(
+        ctx: ResourceCreationContext,
+        dependency_attributes: list[pf.ParsedAttribute] = None,
+):
     """Create a dependency in a resource.
 
     Parameters
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
+    dependency_attributes: list[pf.ParsedAttribute]
+        list of attributes to pass to the dependency creation. Defaults to None
     """
+    if dependency_attributes:
+        ctx.no_modif = False
+
     _create_default_resource(ctx)
 
+    ctx.no_modif = True
+
+    # Process attributes
+    def attributes(attribute_list: list[pf.ParsedAttribute]):
+        for attribute in attribute_list:
+            if attribute.name == ctx.model.name_key:
+                ctx.resource_args[ctx.model.name_key] = attribute.name
+            else:
+                _process_attribute(ctx, attribute)
+
+    if dependency_attributes:
+        attributes(dependency_attributes)
+    attributes(CDK._inherited_attributes)
+
     dependency = ctx.resource_class(
         ctx.stack_self, ctx.resource_name, **ctx.resource_args,
     )
     CDK._parent_resources_stack.remove(ctx.resource_type)
     return dependency.id
 
 
@@ -681,10 +703,12 @@
         dep_ctx = ResourceCreationContext.from_parent(
             ctx,
             resource_type=dependency_type,
         )
         dep_ctx.resource_args = attribute_value
 
         # Creates explicit dependency
-        ctx.resource_args[attribute_name] = _create_dependency(dep_ctx)
+        ctx.resource_args[attribute_name] = _create_dependency(
+            dep_ctx, attribute_value,
+        )
 
     ctx.resource_args[attribute_name] = CDK._created_resources[created_name]
```

### Comparing `thipster-0.17.5/thipster/terraform/exceptions.py` & `thipster-0.17.6/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.5/thipster.egg-info/PKG-INFO` & `thipster-0.17.6/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.5
+Version: 0.17.6
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.5 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.6 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.5/thipster.egg-info/SOURCES.txt` & `thipster-0.17.6/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

