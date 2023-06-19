# Comparing `tmp/thipster-0.17.1.tar.gz` & `tmp/thipster-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.1.tar", last modified: Thu Jun 15 12:01:58 2023, max compression
+gzip compressed data, was "thipster-0.17.2.tar", last modified: Mon Jun 19 16:04:22 2023, max compression
```

## Comparing `thipster-0.17.1.tar` & `thipster-0.17.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 12:01:55.000000 thipster-0.17.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-15 12:01:55.000000 thipster-0.17.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 12:01:58.978078 thipster-0.17.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-15 12:01:55.000000 thipster-0.17.1/README.md
--rw-r--r--   0 root         (0) root         (0)      995 2023-06-15 12:01:55.000000 thipster-0.17.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 12:01:55.000000 thipster-0.17.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 12:01:58.978078 thipster-0.17.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 12:01:55.000000 thipster-0.17.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    15280 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    13619 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_yamlparser.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9180 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13507 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17026 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20074 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22616 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.378397 thipster-0.17.2/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-19 16:04:19.000000 thipster-0.17.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-19 16:04:19.000000 thipster-0.17.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-19 16:04:22.378397 thipster-0.17.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-19 16:04:19.000000 thipster-0.17.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      995 2023-06-19 16:04:19.000000 thipster-0.17.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-19 16:04:19.000000 thipster-0.17.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 16:04:22.378397 thipster-0.17.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-19 16:04:19.000000 thipster-0.17.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.370397 thipster-0.17.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.370397 thipster-0.17.2/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    15280 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/parser/test_yamlparser.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-19 16:04:19.000000 thipster-0.17.2/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.378397 thipster-0.17.2/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.378397 thipster-0.17.2/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9180 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13507 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17026 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20074 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.378397 thipster-0.17.2/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.378397 thipster-0.17.2/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20445 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-19 16:04:19.000000 thipster-0.17.2/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:04:22.374397 thipster-0.17.2/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-19 16:04:22.000000 thipster-0.17.2/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-19 16:04:22.000000 thipster-0.17.2/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:04:22.000000 thipster-0.17.2/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-19 16:04:22.000000 thipster-0.17.2/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-19 16:04:22.000000 thipster-0.17.2/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.1/LICENSE` & `thipster-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/PKG-INFO` & `thipster-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.1
+Version: 0.17.2
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
-Metadata-Version: 2.1 Name: thipster Version: 0.17.1 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.2 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.1/README.md` & `thipster-0.17.2/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/pyproject.toml` & `thipster-0.17.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/setup.py` & `thipster-0.17.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.17.1'
+__version__ = '0.17.2'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.1/tests/engine/test_engine.py` & `thipster-0.17.2/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/engine/test_generation.py` & `thipster-0.17.2/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.2/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.17.2/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.2/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.2/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.2/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/test_parsedfile.py` & `thipster-0.17.2/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/test_parserfactory.py` & `thipster-0.17.2/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/parser/test_yamlparser.py` & `thipster-0.17.2/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/test_e2e.py` & `thipster-0.17.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/tests/test_tools.py` & `thipster-0.17.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/auth/google.py` & `thipster-0.17.2/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/engine.py` & `thipster-0.17.2/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/i_parser.py` & `thipster-0.17.2/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/i_repository.py` & `thipster-0.17.2/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/i_terraform.py` & `thipster-0.17.2/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/parsed_file.py` & `thipster-0.17.2/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/engine/resource_model.py` & `thipster-0.17.2/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/helpers.py` & `thipster-0.17.2/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.2/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.2/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.2/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.2/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.2/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.2/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/token.py` & `thipster-0.17.2/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.2/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/exceptions.py` & `thipster-0.17.2/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/parser_factory.py` & `thipster-0.17.2/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/parser/yaml_parser.py` & `thipster-0.17.2/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/repository/github.py` & `thipster-0.17.2/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/repository/json.py` & `thipster-0.17.2/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster/terraform/cdk.py` & `thipster-0.17.2/thipster/terraform/cdk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,117 @@
 import copy
 import importlib
 import os
 import shutil
 import subprocess
 import sys
 import uuid
+from pathlib import Path
 
 from cdktf import App, TerraformStack
 from constructs import Construct
 from python_terraform import Terraform
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
 from thipster.engine import AuthPort, TerraformPort
 from thipster.helpers import create_logger
 
 
 class ResourceCreationContext():
-    def __init__(self) -> None:
-        pass
+    def __init__(
+        self,
+        stack_self: TerraformStack,
+        resource_name: str | None = None,
+        resource_type: str | None = None,
+        resource_class: type | None = None,
+        parent_name: str | None = None,
+        parent_type: str | None = None,
+        parent_args: dict | None = {},
+        arg_to_complete: str | None = None,
+        no_modif: bool = True,
+        no_dependencies: bool = False,
+    ):
+        self.stack_self = stack_self
+
+        self.model: rm.ResourceModel = None
+        self.dependencies = None
+        self.__resource_type = None
+
+        # Parent resource info
+        self.parent_name = parent_name
+        self.parent_type = parent_type
+        self.parent_args = parent_args
+
+        self.arg_to_complete = arg_to_complete
+        self.no_modif: bool = no_modif
+        self.no_dependencies: bool = no_dependencies
+
+        # Resource info
+        self.resource_name = resource_name
+        self.resource_type = resource_type
+        self.resource_class = resource_class
+        self.resource_args = {}
+
+    @classmethod
+    def from_parent(cls, parent, **args):
+        """Create context from a parent context.
+
+        Parameters
+        ----------
+        ctx: ResourceCreationContext
+            Context from which the resource is created
+        """
+        parent_name = parent.parent_name if parent.parent_name else parent.resource_name
+        return ResourceCreationContext(
+            parent.stack_self,
+            resource_name=f'{parent_name}-{uuid.uuid4().hex[:8]}',
+            parent_name=parent_name,
+            parent_type=parent.resource_type,
+            parent_args=parent.resource_args,
+            **args,
+        )
+
+    def regenerate(self):
+        self.resource_name = f'{self.parent_name}-{uuid.uuid4().hex[:8]}'
+        return self
+
+    @property
+    def resource_type(self):
+        return self.__resource_type
+
+    @resource_type.setter
+    def resource_type(self, value):
+        self.__resource_type = value
+
+        if value is not None:
+            self.model: rm.ResourceModel = CDK._models[self.resource_type]
+            self.dependencies = copy.deepcopy(self.model.dependencies)
+            if self.arg_to_complete in self.dependencies:
+                del self.dependencies[self.arg_to_complete]
 
 
 class CDK(TerraformPort):
     _models = []
     _parent_resources_stack = []
-    _resources_to_create = []
+    _resources_to_create: list[ResourceCreationContext] = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = create_logger(__name__)
 
     @classmethod
     def apply(cls, plan_file_path: str | None = None):
-        """Applies generated Terraform plan
+        """Applies generated Terraform plan.
 
         Parameters
         ----------
         plan_file_path : str, optional
-            path to the plan file, default None
+            Path to the plan file, default None
 
         Returns
         -------
         str
             Terraform apply output
         """
         t = Terraform()
@@ -50,47 +119,51 @@
         return stdout + stderr
 
     @classmethod
     def generate(
         cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
         _authenticator: AuthPort,
     ):
-        """Generate Terraform file from given parsed file and models
+        """Generate Terraform file from given parsed file and models.
 
         Parameters
         ----------
         file : pf.ParsedFile
-            parsedFile object to transform
+            ParsedFile object to transform
         models : dict[str, rm.ResourceModel]
-            associated models
+            Associated models
         _auth : AuthPort
-            authenticator to use
+            Authenticator to use
         """
         cls._created_resources = {}
         cls._models = models
         cls._parent_resources_stack = []
 
         # Init CDK
         app = App()
 
         f_position = file.resources[0].position
-        file_name = f_position.filename if f_position else 'thipster_infrastructure'
+        file_name = Path(f_position.filename).parts[-1] if f_position \
+            else 'thipster_infrastructure'
 
         cls._logger.debug('Creating tf code for file %s', file_name)
 
         # Declare new stack in CDK
+
         class _ResourceStack(TerraformStack):
             def __init__(self, scope: Construct, ns: str):
+
                 super().__init__(scope, ns)
 
                 _authenticator.authenticate(self)
 
                 for resource in file.resources:
+                    ctx = ResourceCreationContext(self)
                     created_resource = _create_resource_from_resource(
-                        self,
+                        ctx,
                         resource=resource,
                     )
 
                     cls._created_resources[f'{resource.resource_type}/{resource.name}']\
                         = created_resource.id
 
         _ResourceStack(app, file_name)
@@ -121,635 +194,490 @@
         for content in os.listdir(os.path.join(os.getcwd(), 'cdktf.out')):
             d = f'cdktf.out/{content}'
             os.rmdir(d) if os.path.isdir(d) else os.remove(d)
         os.rmdir('cdktf.out')
 
     @classmethod
     def init(cls):
-        """Initilize terraform
+        """Initilize terraform.
 
         Returns
         -------
         str
             Terraform init output
         """
         t = Terraform()
         _, stdout, stderr = t.init()
         return stdout + stderr
 
     @classmethod
     def plan(cls):
-        """Get plan from generated terraform code
+        """Get plan from generated terraform code.
 
         Returns
         -------
         str
             Terraform plan output
         """
         t = Terraform()
         _, stdout, stderr = t.plan(out='thipster.tfplan')
         return stdout + stderr
 
     @classmethod
     def _pip_install(cls, package: str):
-        """Install a package if it wasn't already installed by thipster
+        """Install a package if it wasn't already installed by thipster.
 
         Parameters
         ----------
         package : str
-            package to install
+            Package to install
         """
         if package not in sys.modules:
             subprocess.check_call(
                 [sys.executable, '-m', 'pip', 'install', '-qqq', package],
             )
 
     @classmethod
     def _import(cls, package_name: str, module_name: str, class_name: str) -> type:
-        """Import a class from any package
+        """Import a class from any package.
 
         Parameters
         ----------
         package_name : str
-            package that contains the class
+            Package that contains the class
         module_name : str
-            module that contains the class
+            Module that contains the class
         class_name : str
-            class to import
+            Class to import
 
         Returns
         -------
         type :
             the imported class
         """
         module = importlib.import_module(f'{package_name}.{module_name}')
         class_ = getattr(module, class_name)
 
         return class_
 
 
-def _create_default_resource(
-    resource_self, resource_type: str, parent_name: str | None = None,
-    no_modif: bool = True, no_dependencies: bool = False, arg_to_complete: str = None,
-):
-    """Create a resource with all default values
+def _create_default_resource(ctx: ResourceCreationContext):
+    """Create a resource with all default values.
 
     Parameters
     ----------
-    self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    resource_type : str
-        type of the resource to create
-    parent_name : str
-        name of the parent resource
-    parent_name : str, optional
-        name of its parent, default None
-    no_modif : bool, optional
-        if True, raise errors if resource can't be created with default values, \
-default False
-    no_dependencies : bool, optional
-        if True, create the default dependencies, default False
-    arg_to_complete: str
-        name of the argument that will get a value after parent resource creation
-
-    Returns
-    -------
-    (type, str, dict[str, object]) :
-        all the information needed to instantiate the class with default values
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     """
     # Checks for cyclic dependency
-    if resource_type in CDK._parent_resources_stack:
+    if ctx.resource_type in CDK._parent_resources_stack:
         CDK._logger.error(
-            '%s already present in parent Stack', resource_type,
+            '{ctx.resource_type} already present in parent Stack',
         )
         raise cdk_exceptions.CDKCyclicDependenciesError(
             CDK._parent_resources_stack,
         )
 
-    CDK._parent_resources_stack.append(resource_type)
-
-    model = CDK._models[resource_type]
+    CDK._parent_resources_stack.append(ctx.resource_type)
 
-    attributes = copy.deepcopy(model.attributes)
+    attributes = copy.deepcopy(ctx.model.attributes)
 
     for a in CDK._inherited_attributes:
-        if a.name in attributes.keys():
+        if a.name in attributes:
             attributes[a.name].default = rm.ModelLiteral(a.value)
 
         else:
             attributes[a.name] = rm.ModelAttribute(
                 cdk_name=a.name,
                 default=rm.ModelLiteral(a.value),
             )
 
     # Checks that all attributes have a default value
-    if (
-        no_modif
-        and not all(map(lambda x: x.default is not None, attributes.values()))
-    ):
+    if ctx.no_modif and not all(x.default is not None for x in attributes.values()):
         raise cdk_exceptions.CDKMissingAttributeInDependencyError(
-            resource_type,
+            ctx.resource_type,
         )
 
     # Import package and class
-    CDK._pip_install(model.cdk_provider)
-    resource_class = CDK._import(
-        model.cdk_provider, model.cdk_module, model.cdk_name,
+    CDK._pip_install(ctx.model.cdk_provider)
+    ctx.resource_class = CDK._import(
+        ctx.model.cdk_provider, ctx.model.cdk_module, ctx.model.cdk_name,
     )
 
-    # Process name + default values
-    dependencies = _get_dependency_list(model, arg_to_complete)
-    resource_args = {}
-
-    name = f'{parent_name}-{uuid.uuid4()}'
-    if model.name_key:
-        resource_args[model.name_key] = name
+    if ctx.model.name_key:
+        ctx.resource_args[ctx.model.name_key] = ctx.resource_name
 
     for attribute_name, attribute_value in attributes.items():
-
-        if not no_dependencies and attribute_name in dependencies:
-
+        if not ctx.no_dependencies and attribute_name in ctx.dependencies:
             _check_explicit_dependency(
-                resource_self, resource_args, dependencies[attribute_name]['resource'],
-                attribute_value.default, attribute_name,
+                ctx, attribute_name, attribute_value.default,
             )
 
-            del dependencies[attribute_name]
+            del ctx.dependencies[attribute_name]
 
-        if attribute_name in model.attributes:
-            resource_args[attribute_value.cdk_name] = attribute_value.default
+        if attribute_name in ctx.model.attributes:
+            ctx.resource_args[attribute_value.cdk_name] = attribute_value.default
 
     # Create default defendencies if needed
-    if not no_dependencies:
-        _generate_default_dependencies(
-            resource_self, dependencies, model, resource_args, parent_name,
-        )
-
-    CDK._logger.debug('Created default %s named %s', resource_class, name)
+    if not ctx.no_dependencies:
+        _generate_default_dependencies(ctx)
 
-    return (resource_class, name, resource_args)
+    CDK._logger.debug(
+        f'Created default {ctx.resource_class} named {ctx.resource_name}',
+    )
 
 
-def _create_resource(
-        resource_self, resource_args: object, parent_name: str,
-        resource_type: str = None, arg_to_complete: bool = True,
-):
-    """Create a resource with the given values
+def _create_resource(ctx: ResourceCreationContext, resource_args: object):
+    """Create a resource with the given values.
 
     Parameters
     ----------
-    self : _ResourceStack
-        Terraform CDK stack that contains the resource
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     resource_args : object
-        data source to create the resource
-    parent_name : str
-        name of the parent resource
-    resource_type : str, optional
-        type of the resource to create, default None
-    arg_to_complete: str
-        name of the argument that will get a value after parent resource creation
+        Data source to create the resource
 
     Returns
     -------
     object :
-        the created resource
+        Created resource
     """
-
     if isinstance(resource_args, pf.ParsedResource):
         return _create_resource_from_resource(
-            resource_self, resource_args, parent_name, arg_to_complete,
+            ctx, resource_args,
         )
 
-    return _create_resource_from_args(
-        resource_self, resource_type, parent_name, resource_args, arg_to_complete,
-    )
+    if isinstance(resource_args, list):
+        return _create_resource_from_args(
+            ctx, resource_args,
+        )
+    return None
 
 
 def _create_resource_from_args(
-    resource_self, resource_type: str, parent_name: str,
-    input_args: list[pf.ParsedAttribute] | None, arg_to_complete: str = None,
+    ctx: ResourceCreationContext, input_args: list[pf.ParsedAttribute] | None,
 ):
-    """Create a resource from a list of ParsedAttributes
+    """Create a resource from a list of ParsedAttributes.
 
     Parameters
     ----------
-    self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    resource_type : str, optional
-        type of the resource to create, default None
-    parent_name : str
-        name of the parent resource
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     input_args : list[ParsedAttribute]
         data source to create the resource
-    arg_to_complete: str
-        name of the argument that will get a value after parent resource creation
 
     Returns
     -------
     object :
-        the created resource
+        Created resource
     """
-    resource_class, resource_name, resource_args = _create_default_resource(
-        resource_self,
-        resource_type,
-        parent_name=parent_name,
-        no_modif=False,
-        no_dependencies=True,
-        arg_to_complete=arg_to_complete,
-    )
-    model = CDK._models[resource_type]
+    ctx.no_modif = False
+    ctx.no_dependencies = True
 
-    # Process attributes
-    dependencies = _get_dependency_list(model, arg_to_complete)
+    # Create resource with default values
+    _create_default_resource(ctx)
+    ctx.no_modif = True
+    ctx.no_dependencies = False
 
-    def attributes(attribute_list):
+    # Process attributes
+    def attributes(attribute_list: list[pf.ParsedAttribute]):
         for attribute in attribute_list:
-            if attribute.name == model.name_key:
-                resource_args[model.name_key] = attribute.name
+            if attribute.name == ctx.model.name_key:
+                ctx.resource_args[ctx.model.name_key] = attribute.name
             else:
-                _process_attribute(
-                    resource_self, model,
-                    attribute, resource_args, dependencies, parent_name,
-                )
+                _process_attribute(ctx, attribute)
 
     attributes(input_args)
     attributes(CDK._inherited_attributes)
 
     CDK._inherited_attributes += input_args
-    _generate_default_dependencies(
-        resource_self, dependencies, model, resource_args, resource_name,
-    )
-    CDK._inherited_attributes = CDK._inherited_attributes[
-        :-len(
-            input_args,
-        )
-    ]
+    _generate_default_dependencies(ctx)
+    CDK._inherited_attributes = CDK._inherited_attributes[:-len(input_args)]
 
-    # Create resource
-    CDK._parent_resources_stack.remove(resource_type)
-
-    CDK._logger.debug(
-        'Created default %s named %s',
-        resource_class, resource_name,
-    )
-
-    if not arg_to_complete:
-        if not model.name_key:
-            class_ = resource_class(**resource_args)
-        else:
-            class_ = resource_class(
-                resource_self, resource_name, **resource_args,
-            )
-
-        while len(CDK._resources_to_create) != 0:
-            to_create_class, to_create_name, to_create_args, to_create_complete = \
-                CDK._resources_to_create.pop()
-            to_create_args[to_create_complete] = class_.id
-
-            to_create_class(
-                resource_self, to_create_name, **to_create_args,
-            )
-        return class_
-
-    CDK._resources_to_create.append(
-        (resource_class, resource_name, resource_args, arg_to_complete),
-    )
+    return _instantiate_class(ctx)
 
 
 def _create_resource_from_resource(
-        resource_self, resource: pf.ParsedResource,
-        parent_name: str = None, arg_to_complete: str = None,
+        ctx: ResourceCreationContext, resource: pf.ParsedResource,
 ):
-    """Create a resource from a list of ParsedAttributes
+    """Create a resource from a list of ParsedAttributes.
 
     Parameters
     ----------
-    resource_self : _ResourceStack
-        Terraform CDK stack that contains the resource
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     resource : ParsedResource
-        data source to create the resource
-    parent_name : str
-        name of the parent resource
-    arg_to_complete: str
-        name of the argument that will get a value after parent resource creation
+        Data source to create the resource
 
     Returns
     -------
     object :
-        the created resource
+        Created resource
     """
+    ctx.resource_name = resource.name
+    ctx.resource_type = resource.resource_type
 
-    # Create resource with default values
-    resource_class, _, resource_args = _create_default_resource(
-        resource_self,
-        resource.resource_type,
-        parent_name=parent_name,
-        no_modif=False,
-        no_dependencies=True,
-        arg_to_complete=arg_to_complete,
-    )
-    model = CDK._models[resource.resource_type]
+    ctx.no_modif = False
+    ctx.no_dependencies = True
 
-    if model.name_key:
-        resource_args[model.name_key] = resource.name
+    # Create resource with default values
+    _create_default_resource(ctx)
+    ctx.no_modif = True
+    ctx.no_dependencies = False
 
-    # Process attributes
-    dependencies = _get_dependency_list(model, arg_to_complete)
+    if ctx.model.name_key:
+        ctx.resource_args[ctx.model.name_key] = ctx.resource_name
 
     def attributes(attribute_list):
         for attribute in attribute_list:
-            _process_attribute(
-                resource_self,
-                model,
-                attribute,
-                resource_args,
-                dependencies,
-                resource.name,
-            )
+            _process_attribute(ctx, attribute)
 
     attributes(resource.attributes)
     attributes(CDK._inherited_attributes)
 
     CDK._inherited_attributes += resource.attributes
-    _generate_default_dependencies(
-        resource_self, dependencies, model, resource_args, resource.name,
-    )
+    _generate_default_dependencies(ctx)
     CDK._inherited_attributes = CDK._inherited_attributes[
         :-len(
             resource.attributes,
         )
     ]
 
-    # Create resource
-    CDK._parent_resources_stack.remove(resource.resource_type)
+    return _instantiate_class(ctx)
 
-    CDK._logger.debug(
-        'Created resource %s named %s',
-        resource_class, resource.name,
-    )
 
-    if not arg_to_complete:
-        if not model.name_key:
-            class_ = resource_class(**resource_args)
+def _instantiate_class(ctx: ResourceCreationContext):
+    """Instantiates a class.
+
+    Parameters
+    ----------
+    ctx: ResourceCreationContext
+        Context from which the resource is created
+
+    Returns
+    -------
+    object :
+        Created resource
+    """
+    CDK._parent_resources_stack.remove(ctx.resource_type)
+
+    if not ctx.arg_to_complete:
+        if not ctx.model.name_key:
+            class_ = ctx.resource_class(**ctx.resource_args)
         else:
-            class_ = resource_class(
-                resource_self, resource.name, **resource_args,
+            class_ = ctx.resource_class(
+                ctx.stack_self, ctx.resource_name, **ctx.resource_args,
             )
 
         while len(CDK._resources_to_create) != 0:
-            to_create_class, to_create_name, to_create_args, to_create_complete = \
-                CDK._resources_to_create.pop()
-            to_create_args[to_create_complete] = class_.id
+            to_create = CDK._resources_to_create.pop()
+            to_create.resource_args[to_create.arg_to_complete] = class_.id
 
-            to_create_class(
-                resource_self, to_create_name, **to_create_args,
+            to_create.resource_class(
+                to_create.stack_self, to_create.resource_name,
+                **to_create.resource_args,
             )
+
+        CDK._logger.debug(
+            f'Created {ctx.resource_class} named {ctx.resource_name}',
+        )
         return class_
 
-    CDK._resources_to_create.append(
-        (resource_class, resource.name, resource_args, arg_to_complete),
-    )
+    CDK._resources_to_create.append(ctx)
     return True
 
 
-def _process_attribute(
-    resource_self,
-    model: rm.ResourceModel,
-    attribute: pf.ParsedAttribute,
-    resource_args: dict[str, object],
-    dependencies: dict[str, dict[str, object]] | None,
-    parent_name: str,
-):
-    """Process an attribute
+def _process_attribute(ctx: ResourceCreationContext, attribute: pf.ParsedAttribute):
+    """Process an attribute.
 
     Parameters
     ----------
-    resource_self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    model : ResourceModel
-        model of the resource that is being created
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     attribute : ParsedAttribute
-        attribute to handle
-    resource_args : object
-        data source needed to create the resource
-    dependencies : dict[str, dict[str, object]]
-        dependencies needed to create the resource
-    parent_name : str
-        name of the parent resource
+        Attribute to process
     """
-    if attribute.name in dependencies:
-        _check_explicit_dependency(
-            resource_self, resource_args, dependencies[attribute.name]['resource'],
-            attribute.value, attribute.name,
-        )
-        del dependencies[attribute.name]
+    if attribute.name in ctx.dependencies:
+        _check_explicit_dependency(ctx, attribute.name, attribute.value)
+        del ctx.dependencies[attribute.name]
         return
 
     # Checks if attribute is an internal object
-    if attribute.name in model.internal_objects:
+    if attribute.name in ctx.model.internal_objects:
         _create_internal_object(
-            resource_self,
+            ctx,
             attribute.name,
-            model.internal_objects[attribute.name],
             attribute.value,
-            resource_args,
-            parent_name,
         )
         return
 
     # Checks if attribute is expected as an attibute
-    if attribute.name not in model.attributes:
+    if attribute.name not in ctx.model.attributes:
         return
 
     # Processes list attribute
     attribute_value = attribute.value
-    if model.attributes[attribute.name].is_list:
+    if ctx.model.attributes[attribute.name].is_list:
         if type(attribute.value) is list:
             attribute_value = [i.value for i in attribute.value]
         else:
             attribute_value = [attribute.value]
 
     # Sets attribute value
-    resource_args[model.attributes[attribute.name].cdk_name] = attribute_value
+    ctx.resource_args[ctx.model.attributes[attribute.name].cdk_name] = attribute_value
 
 
-def _generate_default_dependencies(
-        resource_self,
-        dependencies,
-        model: rm.ResourceModel,
-        resource_args,
-        resource_name,
-):
-    """Generate default dependencies and internal objects in a resource
+def _generate_default_dependencies(ctx: ResourceCreationContext):
+    """Generate default dependencies and internal objects in a resource.
 
     Parameters
     ----------
-    self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    dependencies :
-        list of dependencies to create
-    model : str
-        model of the resource that is being created
-    resource_args : _type_
-        data source needed to create the resource
-    resource_name : dict
-        name of the resource that is being created
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     """
     # Create missing dependencies
-    for dependency_name, dependency_object in dependencies.items():
-        _create_dependency(
-            resource_self, dependency_name,
-            dependency_object, resource_args, resource_name,
+    for dependency_name, dependency_object in ctx.dependencies.items():
+        dep_ctx = ResourceCreationContext.from_parent(
+            ctx,
+            resource_type=dependency_object['resource'],
         )
+        ctx.resource_args[dependency_name] = _create_dependency(dep_ctx)
 
     # Create default internal objects if needed
-    for internal_object_name, internal_object in model.internal_objects.items():
-        if internal_object_name not in resource_args:
+    for internal_object_name, internal_object in ctx.model.internal_objects.items():
+        if internal_object_name not in ctx.resource_args:
             for default_args_json in internal_object['defaults']:
 
                 # Transform in list of ParsedAttributes
                 default_args = []
                 for arg_key, arg_value in default_args_json.items():
                     default_args.append(
                         pf.ParsedAttribute(
                             arg_key, None, pf.ParsedLiteral(arg_value),
                         ),
                     )
 
                 _create_internal_object(
-                    resource_self,
+                    ctx,
                     internal_object_name,
-                    model.internal_objects[internal_object_name],
                     default_args,
-                    resource_args,
-                    resource_name,
                 )
 
 
 def _create_internal_object(
-    resource_self,
-    name: str,
-    internal_object_model: dict,
+    ctx: ResourceCreationContext,
+    internal_object_name: str,
     internal_object_args,
-    resource_args: dict,
-    parent_name: str,
 ):
-    """Create an internal object in a resource
+    """Create an internal object in a resource.
 
     Parameters
     ----------
-    resource_self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    name : str
-        name of the internal object
-    internal_object_model : ResourceModel
-        model of the internal object
+    ctx: ResourceCreationContext
+        Context from which the resource is created
+    internal_object_name : str
+        Name of the internal object
     internal_object_args : object
-        data source to create the internal object
-    resource_args : dict
-        data source needed to create the resource
-    parent_name : str
-        name of the parent resource
+        Data source to create the internal object
     """
+    internal_object_model = ctx.model.internal_objects[internal_object_name]
+
+    internal_object_base_ctx = ResourceCreationContext.from_parent(
+        ctx,
+        resource_type=internal_object_model['resource'],
+        arg_to_complete=internal_object_model.get('arg_to_complete'),
+    )
+
     internal_object_type = internal_object_model['var_type'] \
         if 'var_type' in internal_object_model else 'Unknown'
 
-    arg_to_complete = internal_object_model.get('arg_to_complete')
-
-    if internal_object_type.startswith('list'):
-        if name not in resource_args and not arg_to_complete:
-            resource_args[name] = []
+    if internal_object_type.startswith('list') or internal_object_model['is_list']:
+        if internal_object_name not in ctx.resource_args\
+                and not internal_object_base_ctx.arg_to_complete:
+            ctx.resource_args[internal_object_name] = []
 
         if isinstance(internal_object_args, list) \
                 and isinstance(internal_object_args[0], pf.ParsedDict):
 
             for internal_object in internal_object_args:
+                internal_object_ctx = copy.copy(internal_object_base_ctx)
+                internal_object_ctx.regenerate()
                 res = _create_resource(
-                    resource_self,
+                    internal_object_ctx,
                     internal_object.value,
-                    parent_name,
-                    internal_object_model['resource'],
-                    arg_to_complete=arg_to_complete,
                 )
-                if not arg_to_complete:
-                    resource_args[name] += [res]
+                if not internal_object_base_ctx.arg_to_complete:
+                    ctx.resource_args[internal_object_name] += [res]
+
             return True
 
         res = _create_resource(
-            resource_self,
+            internal_object_base_ctx,
             internal_object_args,
-            parent_name,
-            internal_object_model['resource'],
-            arg_to_complete=arg_to_complete,
         )
-        if not arg_to_complete:
-            resource_args[name] += [res]
+        if not internal_object_base_ctx.arg_to_complete:
+            ctx.resource_args[internal_object_name] += [res]
         return True
 
     res = _create_resource(
-        resource_self,
+        internal_object_base_ctx,
         internal_object_args,
-        parent_name,
-        internal_object_model['resource'],
-        arg_to_complete=arg_to_complete,
     )
-    if not arg_to_complete:
-        resource_args[name] = res
+    if not internal_object_base_ctx.arg_to_complete:
+        ctx.resource_args[internal_object_name] = res
 
     return True
 
 
-def _get_dependency_list(model, arg_to_complete):
-    dependencies = copy.deepcopy(model.dependencies)
-    if arg_to_complete in dependencies.keys():
-        del dependencies[arg_to_complete]
-    return dependencies
-
-
-def _create_dependency(resource_self, dep_name, dep_value, resource_args, parent_name):
-    """Create an internal object in a resource
+def _create_dependency(ctx: ResourceCreationContext):
+    """Create a dependency in a resource.
 
     Parameters
     ----------
-    self : _ResourceStack
-        Terraform CDK stack that contains the resource
-    dep_name : str
-        name of the dependency
-    dep_value : ResourceModel
-        model of the dependency
-    resource_args : dict
-        data source needed to create the resource
-    parent_name : str
-        name of its parent
+    ctx: ResourceCreationContext
+        Context from which the resource is created
     """
-    class_, class_name, class_attributes = _create_default_resource(
-        resource_self, dep_value['resource'], parent_name,
-    )
-
-    id = class_(resource_self, class_name, **class_attributes).id
-    if dep_name:
-        resource_args[dep_name] = id
+    _create_default_resource(ctx)
 
-    CDK._parent_resources_stack.remove(dep_value['resource'])
+    dependency = ctx.resource_class(
+        ctx.stack_self, ctx.resource_name, **ctx.resource_args,
+    )
+    CDK._parent_resources_stack.remove(ctx.resource_type)
+    return dependency.id
 
 
 def _check_explicit_dependency(
-    resource_self, resource_args, dependency_type, dependency_value, attribute_name,
+    ctx: ResourceCreationContext, attribute_name: str, attribute_value: str | dict,
 ):
-    created_name = f'{dependency_type}/'\
-        f'{dependency_value}'
+    """Check if a dependency attribute was explicited before.\
+    Create the dependency if it wasn't.
+
+    Parameters
+    ----------
+    ctx: ResourceCreationContext
+        Context from which the resource is created
+    attribute_name: str
+        Name of the attribute to check
+    attribute_value: str | dict
+        Value of the attribute to check
+    """
+    dependency_type = ctx.dependencies[attribute_name]['resource']
+    created_name = f'{dependency_type}/{attribute_value}'
 
     # Checks if attribute is an explicit dependency
     if created_name not in CDK._created_resources.keys():
 
-        if isinstance(dependency_value, str):
+        if isinstance(attribute_value, str):
             raise cdk_exceptions.CDKDependencyNotDeclaredError(
-                attribute_name, dependency_value,
+                attribute_name, attribute_value,
             )
 
-        # Creates explicit dependency
-        _create_dependency(
-            resource_self, attribute_name, dependency_value,
-            resource_args, attribute_name,
+        dep_ctx = ResourceCreationContext.from_parent(
+            ctx,
+            resource_args=attribute_value,
+            resource_type=dependency_type,
         )
 
-    resource_args[attribute_name] = CDK._created_resources[created_name]
+        # Creates explicit dependency
+        ctx.resource_args[attribute_name] = _create_dependency(dep_ctx)
+
+    ctx.resource_args[attribute_name] = CDK._created_resources[created_name]
```

### Comparing `thipster-0.17.1/thipster/terraform/exceptions.py` & `thipster-0.17.2/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.1/thipster.egg-info/PKG-INFO` & `thipster-0.17.2/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.1
+Version: 0.17.2
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
-Metadata-Version: 2.1 Name: thipster Version: 0.17.1 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.2 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.1/thipster.egg-info/SOURCES.txt` & `thipster-0.17.2/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

