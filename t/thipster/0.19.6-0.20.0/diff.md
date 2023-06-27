# Comparing `tmp/thipster-0.19.6.tar.gz` & `tmp/thipster-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.19.6.tar", last modified: Mon Jun 26 12:25:50 2023, max compression
+gzip compressed data, was "thipster-0.20.0.tar", last modified: Tue Jun 27 07:58:24 2023, max compression
```

## Comparing `thipster-0.19.6.tar` & `thipster-0.20.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.906457 thipster-0.19.6/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-26 12:25:46.000000 thipster-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-26 12:25:46.000000 thipster-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 12:25:50.906457 thipster-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4544 2023-06-26 12:25:46.000000 thipster-0.19.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-26 12:25:46.000000 thipster-0.19.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-26 12:25:46.000000 thipster-0.19.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 12:25:50.910457 thipster-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-26 12:25:47.000000 thipster-0.19.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.890457 thipster-0.19.6/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.894457 thipster-0.19.6/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.894457 thipster-0.19.6/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.894457 thipster-0.19.6/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    16811 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.898457 thipster-0.19.6/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-26 12:25:46.000000 thipster-0.19.6/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.898457 thipster-0.19.6/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.898457 thipster-0.19.6/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.902457 thipster-0.19.6/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5610 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.902457 thipster-0.19.6/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.906457 thipster-0.19.6/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    16910 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    21596 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.906457 thipster-0.19.6/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.906457 thipster-0.19.6/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24467 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-26 12:25:46.000000 thipster-0.19.6/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 12:25:50.898457 thipster-0.19.6/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 12:25:50.000000 thipster-0.19.6/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-26 12:25:50.000000 thipster-0.19.6/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 12:25:50.000000 thipster-0.19.6/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-26 12:25:50.000000 thipster-0.19.6/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-26 12:25:50.000000 thipster-0.19.6/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.620068 thipster-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-27 07:58:20.000000 thipster-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-27 07:58:20.000000 thipster-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-27 07:58:24.620068 thipster-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-06-27 07:58:20.000000 thipster-0.20.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-27 07:58:20.000000 thipster-0.20.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-27 07:58:20.000000 thipster-0.20.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:58:24.620068 thipster-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-27 07:58:21.000000 thipster-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.608067 thipster-0.20.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.608067 thipster-0.20.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.608067 thipster-0.20.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.612067 thipster-0.20.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    17236 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15129 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.612067 thipster-0.20.0/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-27 07:58:20.000000 thipster-0.20.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.612067 thipster-0.20.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.612067 thipster-0.20.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.616068 thipster-0.20.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5610 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.616068 thipster-0.20.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.616068 thipster-0.20.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14004 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    14943 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21940 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.620068 thipster-0.20.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.620068 thipster-0.20.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24467 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-27 07:58:20.000000 thipster-0.20.0/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:58:24.612067 thipster-0.20.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-27 07:58:24.000000 thipster-0.20.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-27 07:58:24.000000 thipster-0.20.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:58:24.000000 thipster-0.20.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-27 07:58:24.000000 thipster-0.20.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-27 07:58:24.000000 thipster-0.20.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.19.6/LICENSE` & `thipster-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/PKG-INFO` & `thipster-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.6
+Version: 0.20.0
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
-Metadata-Version: 2.1 Name: thipster Version: 0.19.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.20.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.6/README.md` & `thipster-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/pyproject.toml` & `thipster-0.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/setup.py` & `thipster-0.20.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.19.6'
+__version__ = '0.20.0'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.19.6/tests/engine/test_engine.py` & `thipster-0.20.0/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/engine/test_generation.py` & `thipster-0.20.0/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/dsl_parser/test_ast.py` & `thipster-0.20.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.20.0/tests/parser/dsl_parser/test_dslparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -367,14 +367,37 @@
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert region.value is True
 
 
+def test_parse_comment():
+    """Test the parsing of an amount."""
+    out = __test_file(
+        file="""bucket my-bucket:
+\ttoto: aaaaa // MY COMMENT
+\ttata: bbbbb
+""",
+    )
+
+    assert len(out.resources) == 1
+    bucket = out.resources[0]
+    assert bucket.resource_type == 'bucket'
+    assert 'my-bucket' in bucket.name
+    assert len(bucket.attributes) == 2
+
+    region = bucket.attributes[0]
+    assert region.name == 'toto'
+    assert region.value == 'aaaaa'
+    region = bucket.attributes[1]
+    assert region.name == 'tata'
+    assert region.value == 'bbbbb'
+
+
 def test_parse_amount():
     """Test the parsing of an amount."""
     out = __test_file(
         file="""bucket my-bucket: amount: 3
 \tregion: euw
 """,
     )
@@ -402,14 +425,52 @@
         assert len(bucket.attributes) == 1
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == i
 
 
+def test_parse_amount_if_value():
+    """Test the parsing of an amount."""
+    out = __test_file(
+        file="""bucket my-bucket: amount: 3 if 1==1 else 2
+\tregion: euw
+""",
+    )
+
+    assert len(out.resources) == 3
+
+    out = __test_file(
+        file="""bucket my-bucket: amount: 3 if 1==2 else 2
+\tregion: euw
+""",
+    )
+
+    assert len(out.resources) == 2
+
+
+def test_parse_if_and_amount_resource():
+    """Test the parsing of an amount."""
+    out = __test_file(
+        file="""bucket my-bucket:  if 1==1 amount: 3
+\tregion: euw
+""",
+    )
+
+    assert len(out.resources) == 3
+
+    out = __test_file(
+        file="""bucket my-bucket: if 1==2 amount: 3
+\tregion: euw
+""",
+    )
+
+    assert len(out.resources) == 0
+
+
 def test_var_in_name():
     """Test the parsing of a variable in a name."""
     out = __test_file(
         file="""bucket my-bucket#i: amount: 3 #i
 \tregion: #i
 """,
     )
@@ -470,84 +531,44 @@
     # NE
     test_cmp('3!=2', 'truCase')
     test_cmp('2!=2', 'falsCase')
 
 
 def test_arithmetic():
     """Test the parsing of arithmetic expressions."""
-    # PLUS
-    out = __test_file(
-        file="""bucket my-bucket:
-\tvalue: -1+1-3
-""",
-    )
-
-    assert len(out.resources) == 1
-
-    bucket = out.resources[0]
-    assert bucket.resource_type == 'bucket'
-    assert bucket.name == 'my-bucket'
-    assert len(bucket.attributes) == 1
-
-    region = bucket.attributes[0]
-    assert region.name == 'value'
-    assert region.value == 3
-
-    # OPERATION ORDER
-    out = __test_file(
-        file="""bucket my-bucket:
-\tvalue2: 10/2+3*3
+    def arithmetic_test(calcul: str, expected: int):
+        out = __test_file(
+            file=f"""bucket my-bucket:
+\tvalue: {calcul}
 """,
-    )
-
-    assert len(out.resources) == 1
-
-    bucket = out.resources[0]
-    assert bucket.resource_type == 'bucket'
-    assert bucket.name == 'my-bucket'
-    assert len(bucket.attributes) == 1
+        )
 
-    region = bucket.attributes[0]
-    assert region.name == 'value2'
-    assert region.value == 14
+        assert len(out.resources) == 1
 
-    out = __test_file(
-        file="""bucket my-bucket:
-\tvalue: 10/(2+3)*3
-""",
-    )
+        bucket = out.resources[0]
+        assert bucket.resource_type == 'bucket'
+        assert bucket.name == 'my-bucket'
+        assert len(bucket.attributes) == 1
 
-    assert len(out.resources) == 1
+        region = bucket.attributes[0]
+        assert region.name == 'value'
+        assert region.value == expected
 
-    bucket = out.resources[0]
-    assert bucket.resource_type == 'bucket'
-    assert bucket.name == 'my-bucket'
-    assert len(bucket.attributes) == 1
+    # PLUS
+    arithmetic_test('-1+1-3', 3)
 
-    region = bucket.attributes[0]
-    assert region.name == 'value'
-    assert region.value == 6
+    # OPERATION ORDER
+    arithmetic_test('10/2+3*3', 14)
+    arithmetic_test('10/(2+3)*3', 6)
 
     # POW
-    out = __test_file(
-        file="""bucket my-bucket:
-\tvalue: (-2)^4
-""",
-    )
-
-    assert len(out.resources) == 1
-
-    bucket = out.resources[0]
-    assert bucket.resource_type == 'bucket'
-    assert bucket.name == 'my-bucket'
-    assert len(bucket.attributes) == 1
+    arithmetic_test('(-2)^4', 16)
 
-    region = bucket.attributes[0]
-    assert region.name == 'value'
-    assert region.value == 16
+    # MODULO
+    arithmetic_test('25%17', 8)
 
 
 def __test_parser_raises(
     mocker,  # noqa: ARG001
     input_file: str,
     exception: Exception,
 ) -> pytest.ExceptionInfo:
@@ -651,17 +672,18 @@
     )
 
     # NO INTEGER
     input_file = """
 bucket my-bucket: amount: str
 \tregion: euw
 """
-    __test_syntax_error(
-        mocker, input_file=input_file, ln=2, col=27,
-        expected=[TT.INT, TT.FLOAT, TT.PARENTHESES_START], got=TT.STRING,
+    __test_parser_raises(
+        mocker,
+        input_file=input_file,
+        exception=DSLArithmeticError,
     )
 
 
 def test_syntax_error_if(mocker):
     """Test the syntax errors in an if statement."""
     # MISSING CONDITION
     input_file = """
```

### Comparing `thipster-0.19.6/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.20.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         '=': TT.EQ,
         '*': TT.MUL,
         '/': TT.DIV,
         '!': TT.EXCLAMATION,
         '<': TT.LT,
         '>': TT.GT,
         '^': TT.POW,
+        '%': TT.PERCENT,
     }.items():
         __single_token_test(input_char, output)
 
 
 def test_lex_brackets():
     """Test the lexing of brackets."""
     lexer = Lexer({'': ''})
```

### Comparing `thipster-0.19.6/tests/parser/dsl_parser/test_token.py` & `thipster-0.20.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.20.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/test_parsedfile.py` & `thipster-0.20.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/test_parserfactory.py` & `thipster-0.20.0/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/parser/test_yamlparser.py` & `thipster-0.20.0/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/repository/test_github_repository.py` & `thipster-0.20.0/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/repository/test_local_repository.py` & `thipster-0.20.0/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/repository/test_resourcemodel.py` & `thipster-0.20.0/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/test_e2e.py` & `thipster-0.20.0/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/tests/test_tools.py` & `thipster-0.20.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/auth/google.py` & `thipster-0.20.0/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/engine.py` & `thipster-0.20.0/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/i_parser.py` & `thipster-0.20.0/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/i_repository.py` & `thipster-0.20.0/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/i_terraform.py` & `thipster-0.20.0/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/parsed_file.py` & `thipster-0.20.0/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/engine/resource_model.py` & `thipster-0.20.0/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/helpers.py` & `thipster-0.20.0/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/ast.py` & `thipster-0.20.0/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.20.0/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.20.0/thipster/parser/dsl_parser/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DSLArithmeticError,
     DSLParserVariableAlreadyUsedError,
     DSLParserVariableNotDeclaredError,
 )
 from .token import TOKENTYPES as TT
 
 
-class Interpreter():
+class Interpreter:
     """Interpreter class for the DSL Parser.
 
     Implements a visitor design pattern on the AST nodes
     """
 
     def __init__(self) -> None:
         """Interpreter class for the DSL Parser.
@@ -165,14 +165,20 @@
 
                 case TT.DIV:
                     div = element.factors[i+1].accept(self)
                     if isinstance(div, pf.ParsedLiteral):
                         div = div.value
                     total /= div
 
+                case TT.PERCENT:
+                    mod = element.factors[i+1].accept(self)
+                    if isinstance(mod, pf.ParsedLiteral):
+                        mod = mod.value
+                    total %= mod
+
         return total
 
     def visit_factor(self, element: ast.FactorNode) -> int | float:
         """Visitor for a Factor node.
 
         Parameters
         ----------
@@ -381,15 +387,17 @@
         amount = element.amount.accept(self).value
         if not isinstance(amount, int):
             raise DSLArithmeticError(
                 element.amount.position, 'Integer expected',
             )
 
         for _ in range(amount):
-            res += element.node.accept(self)
+            node = element.node.accept(self)
+            if node:
+                res += node
             if var:
                 self.__variables[var] += 1
         return res
 
     def visit_parameter(self, element: ast.ParameterNode) -> pf.ParsedAttribute:
         """Visitor for a ParameterNode.
```

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/lexer.py` & `thipster-0.20.0/thipster/parser/dsl_parser/lexer.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .exceptions import DSLParserNoEndingQuotesError
 from .lexer_position import LexerPosition
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
-class Lexer():
+class Lexer:
     """Lexer for the DSL Parser."""
 
     def __init__(self, files: dict[str, str]):
         """Lexer for the DSL Parser.
 
         Parameters
         ----------
@@ -65,14 +65,31 @@
         """
         self.__logger.debug('Lex file %s', filename)
         self.__lexerPosition = LexerPosition(filename)
 
         for char in file_content:
             self.__logger.debug('char %s', char)
             self.__currentChar = char
+
+            if self.__lexerPosition.isComment:
+                if char == '\n':
+                    self.__lexerPosition.isComment = False
+                    self.__handle_newline_token()
+                continue
+
+            if self.__lexerPosition.escaped:
+                match char:
+                    case '\n':
+                        self.__lexerPosition.isMultiLine = True
+                        self.__lexerPosition.new_line()
+                    case _:
+                        self.__add_next_char()
+                self.__lexerPosition.escaped = False
+                continue
+
             if not self.__lexerPosition.isQuotedString:
                 self.__handle_syntax_tokens()
                 continue
 
             if char in ['"', "'"]:
                 self.__handle_quotes(char)()
                 continue
@@ -103,68 +120,81 @@
         self.__lexerPosition.add_to_current_token(self.__currentChar)
         self.__lexerPosition.next_column()
 
     def __handle_empty_token(self):
         """Pass EMPTY tokens ''."""
         pass
 
+    def __handle_simple_token(self, tokentype: TT):
+        def handle_token():
+            self.__handle_base_token(tokentype)
+        return handle_token
+
+    def __handle_word_token(self, tokentype: TT, value=None):
+        def handle_token():
+            """Handle an AMOUNT token 'amount'."""
+            self.__lexerPosition.reset_consecutive_whitespaces()
+            self.__add_base_token(tokentype, value, is_current_token=True)
+        return handle_token
+
     def __handle_syntax_tokens(self) -> None:
         """Handle single character tokens.
 
         Check if the current character is a special token and calls the corresponding
         function.
         If it isn't, it calls the '__iterateNextChar' function
         """
         single_char_tokens = {
-            ':': self.__handle_colon_oken,
-            ',': self.__handle_comma_token,
-            '[': self.__handle_brackets_start_token,
-            ']': self.__handle_brackets_end_token,
-            '(': self.__handle_parentheses_start_token,
-            ')': self.__handle_parentheses_end_token,
+            ':': self.__handle_simple_token(TT.COLON),
+            ',': self.__handle_simple_token(TT.COMMA),
+            '[': self.__handle_simple_token(TT.BRACKETS_START),
+            ']': self.__handle_simple_token(TT.BRACKETS_END),
+            '(': self.__handle_simple_token(TT.PARENTHESES_START),
+            ')': self.__handle_simple_token(TT.PARENTHESES_END),
             '"': self.__handle_quotes('"'),
             "'": self.__handle_quotes("'"),
             '#': self.__handle_hash_token,
             '\n': self.__handle_newline_token,
             '\\': self.__handle_backslash_token,
-            '\t': self.__handle_tab_token,
+            '\t': self.__handle_simple_token(TT.TAB),
             ' ': self.__handle_whitespace,
 
-            '=': self.__handle_eq_token,
+            '=': self.__handle_simple_token(TT.EQ),
             '/': self.__handle_div_token,
-            '-': self.__handle_minus_token,
-            '+': self.__handle_plus_token,
-            '*': self.__handle_mul_token,
-            '^': self.__handle_pow_token,
-            '<': self.__handle_lt_token,
-            '>': self.__handle_gt_token,
-            '!': self.__handle_exclamation_token,
+            '-': self.__handle_simple_token(TT.MINUS),
+            '+': self.__handle_simple_token(TT.PLUS),
+            '*': self.__handle_simple_token(TT.MUL),
+            '^': self.__handle_simple_token(TT.POW),
+            '%': self.__handle_simple_token(TT.PERCENT),
+            '<': self.__handle_simple_token(TT.LT),
+            '>': self.__handle_simple_token(TT.GT),
+            '!': self.__handle_simple_token(TT.EXCLAMATION),
         }
 
         single_char_tokens.get(self.__currentChar, self.__add_next_char)()
 
     def __handle_current_token(self) -> None:
         """Process the current stored token.
 
         Check if the current token is a keyword, calls the cprresponding function, or
         the '__handleLiteralsAndVariables' otherwise.
         """
         current_token = self.__lexerPosition.currentToken.lower()
 
         keywords = {
             '': self.__handle_empty_token,
-            'amount': self.__handle_amount_token,
-            'and': self.__handle_and_token,
-            'if': self.__handle_if_token,
-            'elif': self.__handle_elif_token,
-            'else': self.__handle_else_token,
-            'or': self.__handle_or_token,
-            'true': self.__handle_boolean_token,
-            'false': self.__handle_boolean_token,
-            'not': self.__handle_not_token,
+            'amount': self.__handle_word_token(TT.AMOUNT),
+            'and': self.__handle_word_token(TT.AND),
+            'if': self.__handle_word_token(TT.IF),
+            'elif': self.__handle_word_token(TT.ELIF),
+            'else': self.__handle_word_token(TT.ELSE),
+            'or': self.__handle_word_token(TT.OR),
+            'true': self.__handle_word_token(TT.BOOLEAN, 'true'),
+            'false': self.__handle_word_token(TT.BOOLEAN, 'false'),
+            'not': self.__handle_word_token(TT.NOT),
         }
 
         keywords.get(current_token, self.__handle_literals_and_variables)()
 
     def __handle_literals_and_variables(self) -> None:
         """Create a literal or var token.
 
@@ -278,83 +308,31 @@
             Indicates if the current stored token should be reset, by default True
         """
         if handle_current_token:
             self.__handle_current_token()
         self.__add_base_token(token_type, value, is_current_token)
         self.__update_position(reset_current_token)
 
-    def __handle_colon_oken(self):
-        """Handle a COLON token ':'."""
-        self.__handle_base_token(TT.COLON)
-
-    def __handle_comma_token(self):
-        """Handle a COMMA token ','."""
-        self.__handle_base_token(TT.COMMA)
-
-    def __handle_brackets_start_token(self):
-        """Handle a BRACKETS_START token '['."""
-        self.__handle_base_token(TT.BRACKETS_START)
-
-    def __handle_brackets_end_token(self):
-        """Handle a BRACKETS_END token ']'."""
-        self.__handle_base_token(TT.BRACKETS_END)
-
-    def __handle_parentheses_start_token(self):
-        """Handle a PARENTHESES_START token '('."""
-        self.__handle_base_token(TT.PARENTHESES_START)
-
-    def __handle_parentheses_end_token(self):
-        """Handle a PARENTHESES_END token ')'."""
-        self.__handle_base_token(TT.PARENTHESES_END)
-
-    def __handle_plus_token(self):
-        """Handle a PLUS token '+'."""
-        self.__handle_base_token(TT.PLUS)
-
-    def __handle_minus_token(self):
-        """Handle a MINUS token '-'."""
-        self.__handle_base_token(TT.MINUS)
-
-    def __handle_mul_token(self):
-        """Handle a MUL token '*'."""
-        self.__handle_base_token(TT.MUL)
-
-    def __handle_div_token(self):
-        """Handle a DIV token '/'."""
-        self.__handle_base_token(TT.DIV)
-
-    def __handle_eq_token(self):
-        """Handle a EQ token '='."""
-        self.__handle_base_token(TT.EQ)
-
-    def __handle_exclamation_token(self):
-        """Handle a EXCLAMATION token '!'."""
-        self.__handle_base_token(TT.EXCLAMATION)
-
-    def __handle_lt_token(self):
-        """Handle a LT token '<'."""
-        self.__handle_base_token(TT.LT)
-
-    def __handle_gt_token(self):
-        """Handle a GT token '>'."""
-        self.__handle_base_token(TT.GT)
-
-    def __handle_pow_token(self):
-        """Handle a POW token '^'."""
-        self.__handle_base_token(TT.POW)
-
     def __handle_hash_token(self) -> None:
         """Handle a HASH token '#'.
 
         Sets a variable to indicate that the following literal is a Variable
         """
         self.__handle_current_token()
         self.__update_position()
         self.__lexerPosition.isVariable = True
 
+    def __handle_div_token(self):
+        if len(self.tokenList) == 0 or self.tokenList[-1].token_type is not TT.DIV:
+            return self.__handle_simple_token(TT.DIV)()
+
+        self.__lexerPosition.isComment = True
+        self.__rm_last_tokens()
+        return True
+
     def __handle_whitespace(self) -> None:
         """Handle a WHITESPACE token ' '.
 
         Replaces 4 following whitespaces by a TAB token
         """
         self.__handle_current_token()
         self.__add_base_token(TT.WHITESPACE)
@@ -382,29 +360,24 @@
         self.__lexerPosition.isMultiLine = False
 
     def __handle_backslash_token(self) -> None:
         r"""Handle a BACKSLASH token '\\'.
 
         Sets a variable to indicate that the following line is part of the same token.
         """
-        self.__lexerPosition.isMultiLine = True
+        self.__lexerPosition.escaped = True
         self.__lexerPosition.next_column()
 
-    def __handle_tab_token(self) -> None:
-        r"""Handle a TAB token '\\t'."""
-        self.__handle_base_token(TT.TAB)
-
     def __handle_quotes(self, char) -> None:
         """Handle a DOUBLEQUOTES token '"'.
 
         Sets a variable to indicate that the following characters are a STRING token.
         """
 
         def quote_handler(self=self):
-
             if self.__lexerPosition.isQuotedString:
                 if char == self.__lexerPosition.isQuotedString:
                     self.__add_literal_token_to_list(
                         TT.STRING, self.__lexerPosition.currentToken,
                     )
                     self.__lexerPosition.isQuotedString = False
                     self.__update_position()
@@ -414,56 +387,14 @@
                 self.__handle_current_token()
                 self.__lexerPosition.next_column()
                 self.__lexerPosition.isQuotedString = char
                 self.__lexerPosition.reset_current_token()
 
         return quote_handler
 
-    def __handle_amount_token(self):
-        """Handle an AMOUNT token 'amount'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.AMOUNT, is_current_token=True)
-
-    def __handle_and_token(self):
-        """Handle an AND token 'and'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.AND, is_current_token=True)
-
-    def __handle_if_token(self):
-        """Handle an IF token 'if'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.IF, is_current_token=True)
-
-    def __handle_elif_token(self):
-        """Handle an ELIF token 'elif'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.ELIF, is_current_token=True)
-
-    def __handle_else_token(self):
-        """Handle an ELSE token 'else'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.ELSE, is_current_token=True)
-
-    def __handle_not_token(self):
-        """Handle an OR token 'or'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.NOT, is_current_token=True)
-
-    def __handle_or_token(self):
-        """Handle an OR token 'or'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(TT.OR, is_current_token=True)
-
-    def __handle_boolean_token(self):
-        """Handle a BOOLEAN token 'true' or 'false'."""
-        self.__lexerPosition.reset_consecutive_whitespaces()
-        self.__add_base_token(
-            TT.BOOLEAN, self.__lexerPosition.currentToken, True,
-        )
-
     def __handle_eof_token(self) -> None:
         """Add an EOF token at the end of each file."""
         self.__add_base_token(TT.EOF)
 
     def __add_token_to_list(self, token: Token | None) -> None:
         """Add a new token to the parser's token list.
 
@@ -480,14 +411,16 @@
         self.tokenList = self.tokenList[:-amount]
 
     def __end_file(self) -> None:
         """Add a NEWLINE and an EOF token at the end of each file."""
         if len(self.__lexerPosition.currentToken.strip()) > 0:
             self.__handle_current_token()
             self.__lexerPosition.reset_current_token()
+
+        self.__lexerPosition.isMultiLine = False
         self.__handle_newline_token()
         self.__handle_eof_token()
 
     def __isfloat(self, num: str) -> bool:
         """Check if the string is a float.
 
         Parameters
```

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.20.0/thipster/parser/dsl_parser/lexer_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         self.currentColumn = 1
         self.currentToken = ''
         self.currentTokenIndex = 1
         self.__currentTokenLine = 1
         self.isVariable = False
         self.isQuotedString = False
         self.isMultiLine = False
+        self.isComment = False
+        self.escaped = False
         self.consecutiveWhitespaces = 0
 
     @property
     def currentCharPosition(self) -> Position:  # noqa: N802
         """Get the current position of the lexer."""
         return Position(
             self.currentFile,
```

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/parser.py` & `thipster-0.20.0/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/token.py` & `thipster-0.20.0/thipster/parser/dsl_parser/token.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,29 +31,30 @@
     VAR = 'VAR'
     WHITESPACE = 'WHITESPACE'
 
     PLUS = 'PLUS'
     MINUS = 'MINUS'
     MUL = 'MUL'
     DIV = 'DIV'
+    PERCENT = 'PERCENT'
     POW = 'POW'
     EQ = 'EQ'
     EE = 'EE'
     NE = 'NE'
     LT = 'LT'
     LTE = 'LTE'
     GT = 'GT'
     GTE = 'GTE'
 
     def __str__(self) -> str:
         """Return the string representation of the token type."""
         return self.value
 
 
-class Token():
+class Token:
     """Represents a Token of the THipster DSL."""
 
     def __init__(
         self, position: Position,
         token_type: TOKENTYPES, value: str | None = None,
     ):
         """
```

### Comparing `thipster-0.19.6/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.20.0/thipster/parser/dsl_parser/token_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DSLSyntaxError,
     DSLUnexpectedEOFError,
 )
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
-class TokenParser():
+class TokenParser:
     """Parse the tokens into an AST (Abstract Syntax Tree)."""
 
     def __init__(self, tokens: list[Token]) -> None:
         """Parse the tokens into an AST (Abstract Syntax Tree).
 
         Parameters
         ----------
@@ -106,15 +106,15 @@
 
     def __trim_newlines(self):
         while self.__check(TT.NEWLINE):
             pass
 
     def __rm_empty_lines(self):
         # Detect empty line
-        empty_types = [TT.TAB]
+        empty_types = [TT.TAB, TT.WHITESPACE]
         end = 0
         while end < len(self.__tokens):
             begin = end
             while self.__get_next_type(end) in empty_types:
                 end += 1
 
             if self.__get_next_type(index=end) == TT.NEWLINE:
@@ -158,18 +158,18 @@
             resource_type = self.__get_type()
             self.__get_whitespaces()
             name = self.__get_string_expr()
             self.__get_whitespaces()
             self.__next(TT.COLON)
             self.__get_whitespaces()
 
-            nb_ctrl = self.__get_nb_ctrl()
-            self.__get_whitespaces()
             if_ctrl = self.__get_if_ctrl()
             self.__get_whitespaces()
+            nb_ctrl = self.__get_nb_ctrl()
+            self.__get_whitespaces()
 
             self.__get_newline()
 
             properties = self.__get_properties(indent+1)
 
         except DSLSyntaxError as e:
             raise e
@@ -298,19 +298,18 @@
             while self.__get_tabs(indent):
                 self.__check(TT.MINUS)
                 self.__get_whitespaces()
 
                 value = self.__get_value()
                 self.__get_whitespaces()
 
-                amount_ctrl = self.__get_nb_ctrl()
-                self.__get_whitespaces()
-
                 if_else_ctrl = self.__get_if_else_ctrl()
                 self.__get_whitespaces()
+                amount_ctrl = self.__get_nb_ctrl()
+                self.__get_whitespaces()
 
                 if if_else_ctrl:
                     if_else_ctrl.if_case = value
                     value = if_else_ctrl
 
                 if amount_ctrl:
                     amount_ctrl.node = value
@@ -395,15 +394,15 @@
             if not amount_token:
                 return None
 
             self.__get_whitespaces()
             self.__next(TT.COLON)
 
             self.__get_whitespaces()
-            amount = self.__get_arith_expr()
+            amount = self.__get_value()
 
             self.__get_whitespaces()
         except DSLSyntaxError as e:
             raise e
 
         amount_variable = self.__check(TT.VAR)
 
@@ -461,24 +460,24 @@
             else_case=else_case,
         )
 
     def __get_value(self) -> ast.LiteralNode:
         next_token_type = self.__get_next_type()
         match next_token_type:
             case TT.STRING:
-                return self.__get_string_expr()
+                value = self.__get_string_expr()
 
             case TT.VAR:
-                return ast.LiteralNode(ast.VariableNode(self.__next(TT.VAR)))
+                value = ast.LiteralNode(ast.VariableNode(self.__next(TT.VAR)))
 
             case TT.BRACKETS_START:
-                return self.__get_inline_list()
+                value = self.__get_inline_list()
 
             case TT.NOT | TT.BOOLEAN:
-                return self.__get_comp_expr()
+                value = self.__get_comp_expr()
 
             case _:
                 value = self.__get_arith_expr()
                 self.__get_whitespaces()
 
                 next_token_type = self.__get_next_type()
                 if next_token_type in [TT.EE, TT.LT, TT.GT, TT.LTE, TT.GTE]:
@@ -487,16 +486,24 @@
                     )
                     self.__get_whitespaces()
                     right_expression = self.__get_comp_expr()
                     self.__get_whitespaces()
                     self.__next(TT.PARENTHESES_END)
                     self.__get_whitespaces()
 
-                    return ast.CompExprNode(value, operator, right_expression)
-                return value
+                    value = ast.CompExprNode(value, operator, right_expression)
+
+        if_else_ctrl = self.__get_if_else_ctrl()
+        if not if_else_ctrl:
+            return value
+
+        if_else_ctrl.if_case = value
+        if if_else_ctrl.else_case is None:
+            raise DSLSyntaxError([TT.STRING, TT.VAR])
+        return if_else_ctrl
 
     def __get_comp_expr(self) -> ast.CompExprNode:
         try:
             next_token_type = self.__get_next_type()
             match next_token_type:
 
                 case TT.NOT:
@@ -575,16 +582,20 @@
     def __get_term(self) -> ast.TermNode:
         factors = []
         operator = []
         factors.append(self.__get_factor())
         self.__get_whitespaces()
 
         next_token_type = self.__get_next_type()
-        while next_token_type in [TT.MUL, TT.DIV]:
-            operator.append(self.__next([TT.MUL, TT.DIV]).token_type)
+        while next_token_type in [TT.MUL, TT.DIV, TT.PERCENT]:
+            operator.append(
+                self.__next(
+                    [TT.MUL, TT.DIV, TT.PERCENT],
+                ).token_type,
+            )
             self.__get_whitespaces()
             factors.append(self.__get_factor())
             self.__get_whitespaces()
             next_token_type = self.__get_next_type()
 
         return ast.TermNode(factors, operator)
```

### Comparing `thipster-0.19.6/thipster/parser/exceptions.py` & `thipster-0.20.0/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/parser_factory.py` & `thipster-0.20.0/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/parser/yaml_parser.py` & `thipster-0.20.0/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/repository/exceptions.py` & `thipster-0.20.0/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/repository/github.py` & `thipster-0.20.0/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/repository/json.py` & `thipster-0.20.0/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/repository/local.py` & `thipster-0.20.0/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/terraform/cdk.py` & `thipster-0.20.0/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster/terraform/exceptions.py` & `thipster-0.20.0/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.6/thipster.egg-info/PKG-INFO` & `thipster-0.20.0/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.6
+Version: 0.20.0
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
-Metadata-Version: 2.1 Name: thipster Version: 0.19.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.20.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.6/thipster.egg-info/SOURCES.txt` & `thipster-0.20.0/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

