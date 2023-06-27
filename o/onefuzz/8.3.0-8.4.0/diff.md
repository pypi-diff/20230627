# Comparing `tmp/onefuzz-8.3.0.tar.gz` & `tmp/onefuzz-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.3.0.tar", last modified: Tue Jun  6 20:30:01 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.4.0.tar", last modified: Mon Jun 26 18:58:59 2023, max compression
```

## Comparing `onefuzz-8.3.0.tar` & `onefuzz-8.4.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/
--rw-rw-rw-   0        0        0     1162 2023-06-06 20:28:10.000000 onefuzz-8.3.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-06-06 20:28:10.000000 onefuzz-8.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-06-06 20:30:01.000000 onefuzz-8.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-06-06 20:28:10.000000 onefuzz-8.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-06-06 20:28:10.000000 onefuzz-8.3.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/extra/
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-06-06 20:28:10.000000 onefuzz-8.3.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      431 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-06-06 20:28:11.000000 onefuzz-8.3.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    67797 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22112 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1223 2023-06-06 20:30:00.000000 onefuzz-8.3.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    31058 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0     1682 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10491 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    42114 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8788 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9530 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10649 2023-06-06 20:28:10.000000 onefuzz-8.3.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      344 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 20:30:01.000000 onefuzz-8.3.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-06-06 20:28:10.000000 onefuzz-8.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-06-06 20:28:10.000000 onefuzz-8.3.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      508 2023-06-06 20:28:11.000000 onefuzz-8.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 20:30:01.000000 onefuzz-8.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-06-06 20:28:10.000000 onefuzz-8.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:30:01.000000 onefuzz-8.3.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-06 20:28:10.000000 onefuzz-8.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-06-06 20:28:10.000000 onefuzz-8.3.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/
+-rw-rw-rw-   0        0        0     1162 2023-06-26 18:58:16.000000 onefuzz-8.4.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-06-26 18:58:16.000000 onefuzz-8.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-06-26 18:58:59.000000 onefuzz-8.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-06-26 18:58:16.000000 onefuzz-8.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/extra/
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-06-26 18:58:16.000000 onefuzz-8.4.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-06-26 18:58:17.000000 onefuzz-8.4.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    68993 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1059 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22112 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1232 2023-06-26 18:58:57.000000 onefuzz-8.4.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31463 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0     1682 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10491 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     7003 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    42457 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8812 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9630 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10709 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      344 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-06-26 18:58:16.000000 onefuzz-8.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-06-26 18:58:16.000000 onefuzz-8.4.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      508 2023-06-26 18:58:17.000000 onefuzz-8.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:58:59.000000 onefuzz-8.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-06-26 18:58:16.000000 onefuzz-8.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-06-26 18:58:16.000000 onefuzz-8.4.0/tests/test_template_helper.py
```

### Comparing `onefuzz-8.3.0/LICENSE` & `onefuzz-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/PKG-INFO` & `onefuzz-8.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.3.0
+Version: 8.4.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.3.0/README.md` & `onefuzz-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/domato.py` & `onefuzz-8.4.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/get-running.py` & `onefuzz-8.4.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/honggfuzz.py` & `onefuzz-8.4.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.4.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.4.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.4.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/examples/oss-fuzz-target.py` & `onefuzz-8.4.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/api.py` & `onefuzz-8.4.0/onefuzz/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,14 +542,46 @@
         )
 
         self.logger.debug("get repro vm: %s", vm_id_expanded)
         return self._req_model(
             "GET", models.Repro, data=requests.ReproGet(vm_id=vm_id_expanded)
         )
 
+    def get_files(
+        self,
+        report_container: primitives.Container,
+        report_name: str,
+        include_setup: bool = False,
+        output_dir: primitives.Directory = primitives.Directory("."),
+    ) -> None:
+        """downloads the files necessary to locally repro the crash from a given report"""
+        report_bytes = self.onefuzz.containers.files.get(report_container, report_name)
+        report = json.loads(report_bytes)
+
+        self.logger.info(
+            "downloading files necessary to locally repro crash %s",
+            report["input_blob"]["name"],
+        )
+
+        self.onefuzz.containers.files.download(
+            report["input_blob"]["container"],
+            report["input_blob"]["name"],
+            os.path.join(output_dir, report["input_blob"]["name"]),
+        )
+
+        if include_setup:
+            setup_container = list(
+                self.onefuzz.jobs.containers.list(
+                    report["job_id"], enums.ContainerType.setup
+                )
+            )[0]
+            self.onefuzz.containers.files.download_dir(
+                primitives.Container(setup_container), output_dir
+            )
+
     def create(
         self, container: primitives.Container, path: str, duration: int = 24
     ) -> models.Repro:
         """Create a Reproduction VM from a Crash Report"""
         self.logger.info(
             "creating repro vm: %s %s (%d hours)", container, path, duration
         )
```

### Comparing `onefuzz-8.3.0/onefuzz/azcopy.py` & `onefuzz-8.4.0/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.4.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/backend.py` & `onefuzz-8.4.0/onefuzz/backend.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/cli.py` & `onefuzz-8.4.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/data/licenses.json` & `onefuzz-8.4.0/onefuzz/data/licenses.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {'1': "{'Version': '6.7.0'}",*

 * * '3': "{'Version': '5.13.0'}",*

 * * '5': "{'License': 'BSD-3-Clause', 'Version': '0.2.1'}"}*

```diff
@@ -5,39 +5,39 @@
         "URL": "https://altgraph.readthedocs.io",
         "Version": "0.17.3"
     },
     {
         "License": "Apache Software License",
         "Name": "importlib-metadata",
         "URL": "https://github.com/python/importlib_metadata",
-        "Version": "6.6.0"
+        "Version": "6.7.0"
     },
     {
         "License": "MIT",
         "Name": "pefile",
         "URL": "https://github.com/erocarrera/pefile",
         "Version": "2023.2.7"
     },
     {
         "License": "GNU General Public License v2 (GPLv2)",
         "Name": "pyinstaller",
         "URL": "https://www.pyinstaller.org/",
-        "Version": "5.11.0"
+        "Version": "5.13.0"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
         "Version": "2023.3"
     },
     {
-        "License": "BSD",
+        "License": "BSD-3-Clause",
         "Name": "pywin32-ctypes",
         "URL": "https://github.com/enthought/pywin32-ctypes",
-        "Version": "0.2.0"
+        "Version": "0.2.1"
     },
     {
         "License": "Python Software Foundation License",
         "Name": "typing-extensions",
         "URL": "UNKNOWN",
         "Version": "4.6.3"
     },
```

### Comparing `onefuzz-8.3.0/onefuzz/data/privacy.txt` & `onefuzz-8.4.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/debug.py` & `onefuzz-8.4.0/onefuzz/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -811,28 +811,42 @@
                 handle.write(report.json())
 
             self.onefuzz.containers.files.upload_file(
                 reports, file_path, crash_name + ".json"
             )
 
     def test_template(
-        self, task_id: UUID_EXPANSION, notificationConfig: models.NotificationConfig
+        self,
+        notificationConfig: models.NotificationConfig,
+        task_id: Optional[UUID] = None,
+        report: Optional[Report] = None,
     ) -> responses.NotificationTestResponse:
         """Test a notification template"""
+
+        if task_id is None and report is None:
+            raise Exception("must specify either task_id or report")
+
         endpoint = Endpoint(self.onefuzz)
-        task = self.onefuzz.tasks.get(task_id)
-        input_blob_ref = BlobRef(
-            account="dummy-storage-account",
-            container="test-notification-crashes",
-            name="fake-crash-sample",
-        )
-
-        report = self._create_report(
-            task.job_id, task.task_id, "fake_target.exe", input_blob_ref
-        )
+        if task_id is not None:
+            task = self.onefuzz.tasks.get(task_id)
+            input_blob_ref = BlobRef(
+                account="dummy-storage-account",
+                container="test-notification-crashes",
+                name="fake-crash-sample",
+            )
+
+        if report is None:
+            report = self._create_report(
+                task.job_id, task.task_id, "fake_target.exe", input_blob_ref
+            )
+
+        if task is not None:
+            report.task_id = task.task_id
+            report.job_id = task.job_id
+
         report.report_url = "https://dummy-container.blob.core.windows.net/dummy-reports/dummy-report.json"
 
         return endpoint._req_model(
             "POST",
             responses.NotificationTestResponse,
             data=requests.NotificationTest(
                 report=report,
```

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/builder.py` & `onefuzz-8.4.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/cache.py` & `onefuzz-8.4.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.4.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.4.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/main.py` & `onefuzz-8.4.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/job_templates/manage.py` & `onefuzz-8.4.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/rdp.py` & `onefuzz-8.4.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/ssh.py` & `onefuzz-8.4.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/cache.py` & `onefuzz-8.4.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/cmd.py` & `onefuzz-8.4.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/raw.py` & `onefuzz-8.4.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/signalr.py` & `onefuzz-8.4.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/top.py` & `onefuzz-8.4.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/status/top_view.py` & `onefuzz-8.4.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/template.py` & `onefuzz-8.4.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/templates/__init__.py` & `onefuzz-8.4.0/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/onefuzz/templates/afl.py` & `onefuzz-8.4.0/onefuzz/templates/afl.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         wait_for_files: Optional[List[ContainerType]] = None,
         afl_container: Optional[Container] = None,
         existing_inputs: Optional[Container] = None,
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         Basic AFL job
 
         :param Container afl_container: Specify the AFL container to use in the job
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
@@ -131,17 +131,20 @@
         containers = [
             (ContainerType.tools, afl_container),
             (ContainerType.setup, helper.containers[ContainerType.setup]),
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (ContainerType.inputs, helper.containers[ContainerType.inputs]),
         ]
 
-        if extra_container is not None:
+        if extra_setup_container is not None:
             containers.append(
-                (ContainerType.extra, helper.containers[ContainerType.extra])
+                (
+                    ContainerType.extra_setup,
+                    helper.containers[ContainerType.extra_setup],
+                )
             )
 
         self.logger.info("creating afl fuzz task")
         fuzzer_task = self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.generic_supervisor,
             target_exe_blob_name,
@@ -169,17 +172,20 @@
             (ContainerType.reports, helper.containers[ContainerType.reports]),
             (
                 ContainerType.unique_reports,
                 helper.containers[ContainerType.unique_reports],
             ),
         ]
 
-        if extra_container is not None:
+        if extra_setup_container is not None:
             report_containers.append(
-                (ContainerType.extra, helper.containers[ContainerType.extra])
+                (
+                    ContainerType.extra_setup,
+                    helper.containers[ContainerType.extra_setup],
+                )
             )
 
         self.logger.info("creating generic_crash_report task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.generic_crash_report,
             target_exe_blob_name,
```

### Comparing `onefuzz-8.3.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.4.0/onefuzz/templates/libfuzzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 import os
 import tempfile
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple
 
 from onefuzztypes.enums import OS, ContainerType, TaskDebugFlag, TaskType
 from onefuzztypes.models import Job, NotificationConfig
 from onefuzztypes.primitives import Container, Directory, File, PoolName
 
 from onefuzz.api import Command
 
@@ -39,14 +39,22 @@
         )
         with open(target_exe, "rb") as handle:
             data = handle.read()
 
         if LIBFUZZER_MAGIC_STRING not in data:
             raise Exception("not a libfuzzer binary: %s" % target_exe)
 
+    def _add_optional_containers(
+        self,
+        dest: List[Tuple[ContainerType, Container]],
+        source: Dict[ContainerType, Container],
+        types: List[ContainerType],
+    ) -> None:
+        dest.extend([(c, source[c]) for c in types if c in source])
+
     def _create_tasks(
         self,
         *,
         job: Job,
         containers: Dict[ContainerType, Container],
         pool_name: PoolName,
         target_exe: str,
@@ -82,18 +90,19 @@
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (
                 ContainerType.regression_reports,
                 containers[ContainerType.regression_reports],
             ),
         ]
 
-        if ContainerType.extra in containers:
-            regression_containers.append(
-                (ContainerType.extra, containers[ContainerType.extra])
-            )
+        self._add_optional_containers(
+            regression_containers,
+            containers,
+            [ContainerType.extra_setup, ContainerType.extra_output],
+        )
 
         # We don't really need a separate timeout for crash reporting, and we could just
         # use `target_timeout`. But `crash_report_timeout` was introduced first, so we
         # can't remove it without a breaking change. Since both timeouts may be present,
         # prefer the more task-specific timeout.
         effective_crash_report_timeout = crash_report_timeout or target_timeout
 
@@ -120,26 +129,23 @@
 
         fuzzer_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.inputs, containers[ContainerType.inputs]),
         ]
 
-        if ContainerType.readonly_inputs in containers:
-            fuzzer_containers.append(
-                (
-                    ContainerType.readonly_inputs,
-                    containers[ContainerType.readonly_inputs],
-                )
-            )
-
-        if ContainerType.extra in containers:
-            fuzzer_containers.append(
-                (ContainerType.extra, containers[ContainerType.extra])
-            )
+        self._add_optional_containers(
+            fuzzer_containers,
+            containers,
+            [
+                ContainerType.extra_setup,
+                ContainerType.extra_output,
+                ContainerType.readonly_inputs,
+            ],
+        )
 
         self.logger.info("creating libfuzzer task")
 
         # disable ensemble sync if only one VM is used
         if ensemble_sync_delay is None and vm_count == 1:
             ensemble_sync_delay = 0
 
@@ -176,26 +182,23 @@
 
         coverage_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.coverage, containers[ContainerType.coverage]),
             (ContainerType.readonly_inputs, containers[ContainerType.inputs]),
         ]
 
-        if ContainerType.extra in containers:
-            coverage_containers.append(
-                (ContainerType.extra, containers[ContainerType.extra])
-            )
-
-        if ContainerType.readonly_inputs in containers:
-            coverage_containers.append(
-                (
-                    ContainerType.readonly_inputs,
-                    containers[ContainerType.readonly_inputs],
-                )
-            )
+        self._add_optional_containers(
+            coverage_containers,
+            containers,
+            [
+                ContainerType.extra_setup,
+                ContainerType.extra_output,
+                ContainerType.readonly_inputs,
+            ],
+        )
 
         self.logger.info("creating coverage task")
 
         # The `coverage` task is not libFuzzer-aware, so invocations of the target fuzzer
         # against an input do not automatically add an `{input}` specifier to the command
         # args. That means on the VM, the fuzzer will get run in fuzzing mode each time we
         # try to test an input.
@@ -241,18 +244,19 @@
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.reports, containers[ContainerType.reports]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (ContainerType.no_repro, containers[ContainerType.no_repro]),
         ]
 
-        if ContainerType.extra in containers:
-            report_containers.append(
-                (ContainerType.extra, containers[ContainerType.extra])
-            )
+        self._add_optional_containers(
+            report_containers,
+            containers,
+            [ContainerType.extra_setup, ContainerType.extra_output],
+        )
 
         self.logger.info("creating libfuzzer_crash_report task")
         self.onefuzz.tasks.create(
             job.job_id,
             TaskType.libfuzzer_crash_report,
             target_exe,
             report_containers,
@@ -284,18 +288,19 @@
             analysis_containers = [
                 (ContainerType.setup, containers[ContainerType.setup]),
                 (ContainerType.tools, tools),
                 (ContainerType.analysis, containers[ContainerType.analysis]),
                 (ContainerType.crashes, containers[ContainerType.crashes]),
             ]
 
-            if ContainerType.extra in containers:
-                analysis_containers.append(
-                    (ContainerType.extra, containers[ContainerType.extra])
-                )
+            self._add_optional_containers(
+                analysis_containers,
+                containers,
+                [ContainerType.extra_setup, ContainerType.extra_output],
+            )
 
             self.onefuzz.tasks.create(
                 job.job_id,
                 TaskType.generic_analysis,
                 target_exe,
                 analysis_containers,
                 duration=duration,
@@ -353,15 +358,16 @@
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[File] = None,
         source_allowlist: Optional[File] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
+        extra_output_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         Basic libfuzzer job
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
@@ -452,16 +458,19 @@
                 source_allowlist, setup_dir
             )
         else:
             source_allowlist_blob_name = None
 
         containers = helper.containers
 
-        if extra_container is not None:
-            containers[ContainerType.extra] = extra_container
+        if extra_setup_container is not None:
+            containers[ContainerType.extra_setup] = extra_setup_container
+
+        if extra_output_container is not None:
+            containers[ContainerType.extra_output] = extra_output_container
 
         self._create_tasks(
             job=helper.job,
             containers=containers,
             pool_name=pool_name,
             target_exe=target_exe_blob_name,
             vm_count=vm_count,
@@ -517,15 +526,15 @@
         existing_inputs: Optional[List[Container]] = None,
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         preserve_existing_outputs: bool = False,
         check_fuzzer_help: bool = False,
         no_check_fuzzer_help: bool = False,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer merge task
         """
         if check_fuzzer_help:
             self.logger.warning(
                 "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
@@ -586,16 +595,16 @@
             (ContainerType.setup, helper.containers[ContainerType.setup]),
             (
                 ContainerType.unique_inputs,
                 output_container or helper.containers[ContainerType.unique_inputs],
             ),
         ]
 
-        if extra_container is not None:
-            merge_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            merge_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         if inputs:
             merge_containers.append(
                 (ContainerType.inputs, helper.containers[ContainerType.inputs])
             )
         if existing_inputs:
             for existing_container in existing_inputs:
@@ -653,15 +662,15 @@
         readonly_inputs: Optional[Container] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
         expect_crash_on_failure: bool = False,
         notification_config: Optional[NotificationConfig] = None,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         pool = self.onefuzz.pools.get(pool_name)
 
         # verify containers exist
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
@@ -736,16 +745,16 @@
         fuzzer_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.inputs, containers[ContainerType.inputs]),
             (ContainerType.tools, fuzzer_tools_container),
         ]
 
-        if extra_container is not None:
-            fuzzer_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            fuzzer_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         helper.create_containers()
         helper.setup_notifications(notification_config)
 
         helper.upload_setup(setup_dir, target_dll)
 
         if inputs:
@@ -794,16 +803,18 @@
         coverage_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.coverage, containers[ContainerType.coverage]),
             (ContainerType.readonly_inputs, containers[ContainerType.inputs]),
             (ContainerType.tools, fuzzer_tools_container),
         ]
 
-        if extra_container is not None:
-            coverage_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            coverage_containers.append(
+                (ContainerType.extra_setup, extra_setup_container)
+            )
 
         self.logger.info("creating `dotnet_coverage` task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.dotnet_coverage,
             libfuzzer_dotnet_loader_dll,
             coverage_containers,
@@ -825,16 +836,16 @@
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.reports, containers[ContainerType.reports]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (ContainerType.no_repro, containers[ContainerType.no_repro]),
             (ContainerType.tools, fuzzer_tools_container),
         ]
 
-        if extra_container is not None:
-            report_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            report_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         self.logger.info("creating `dotnet_crash_report` task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.dotnet_crash_report,
             libfuzzer_dotnet_loader_dll,
             report_containers,
@@ -882,15 +893,15 @@
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         crash_report_timeout: Optional[int] = 1,
         check_retry_count: Optional[int] = 300,
         check_fuzzer_help: bool = False,
         no_check_fuzzer_help: bool = False,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
         readonly_inputs: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer tasks, wrapped via qemu-user (PREVIEW FEATURE)
         """
         if check_fuzzer_help:
@@ -953,16 +964,16 @@
 
         fuzzer_containers = [
             (ContainerType.setup, helper.containers[ContainerType.setup]),
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (ContainerType.inputs, helper.containers[ContainerType.inputs]),
         ]
 
-        if extra_container is not None:
-            fuzzer_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            fuzzer_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         if readonly_inputs is not None:
             self.onefuzz.containers.get(readonly_inputs)  # ensure it exists
             fuzzer_containers.append((ContainerType.readonly_inputs, readonly_inputs))
 
         helper.create_containers()
 
@@ -1053,16 +1064,16 @@
             (
                 ContainerType.unique_reports,
                 helper.containers[ContainerType.unique_reports],
             ),
             (ContainerType.no_repro, helper.containers[ContainerType.no_repro]),
         ]
 
-        if extra_container is not None:
-            report_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            report_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         self.logger.info("creating libfuzzer_crash_report task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.libfuzzer_crash_report,
             wrapper_name,
             report_containers,
```

### Comparing `onefuzz-8.3.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.4.0/onefuzz/templates/ossfuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         tags: Optional[Dict[str, str]] = None,
         dryrun: bool = False,
         max_target_count: int = 20,
         sync_inputs: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> None:
         """
         OssFuzz style libfuzzer jobs
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
@@ -210,16 +210,16 @@
                 ContainerType.crashes,
                 ContainerType.reports,
                 ContainerType.unique_reports,
                 ContainerType.no_repro,
                 ContainerType.coverage,
             )
 
-            if extra_container is not None:
-                helper.containers[ContainerType.extra] = extra_container
+            if extra_setup_container is not None:
+                helper.containers[ContainerType.extra_setup] = extra_setup_container
 
             helper.create_containers()
             helper.setup_notifications(notification_config)
 
             dst_sas = self.onefuzz.containers.get(
                 helper.containers[ContainerType.setup]
             ).sas_url
```

### Comparing `onefuzz-8.3.0/onefuzz/templates/radamsa.py` & `onefuzz-8.4.0/onefuzz/templates/radamsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         check_retry_count: Optional[int] = None,
         disable_check_debugger: bool = False,
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         target_timeout: Optional[int] = None,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         Basic radamsa job
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
@@ -153,16 +153,16 @@
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (
                 ContainerType.readonly_inputs,
                 helper.containers[ContainerType.readonly_inputs],
             ),
         ]
 
-        if extra_container is not None:
-            containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            containers.append((ContainerType.extra_setup, extra_setup_container))
 
         fuzzer_task = self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.generic_generator,
             target_exe_blob_name,
             containers,
             pool_name=pool_name,
@@ -189,16 +189,16 @@
             (
                 ContainerType.unique_reports,
                 helper.containers[ContainerType.unique_reports],
             ),
             (ContainerType.no_repro, helper.containers[ContainerType.no_repro]),
         ]
 
-        if extra_container is not None:
-            report_containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container is not None:
+            report_containers.append((ContainerType.extra_setup, extra_setup_container))
 
         self.logger.info("creating generic_crash_report task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.generic_crash_report,
             target_exe_blob_name,
             report_containers,
@@ -235,16 +235,18 @@
             analysis_containers = [
                 (ContainerType.setup, helper.containers[ContainerType.setup]),
                 (ContainerType.tools, tools),
                 (ContainerType.analysis, helper.containers[ContainerType.analysis]),
                 (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             ]
 
-            if extra_container is not None:
-                analysis_containers.append((ContainerType.extra, extra_container))
+            if extra_setup_container is not None:
+                analysis_containers.append(
+                    (ContainerType.extra_setup, extra_setup_container)
+                )
 
             self.onefuzz.tasks.create(
                 helper.job.job_id,
                 TaskType.generic_analysis,
                 target_exe_blob_name,
                 analysis_containers,
                 duration=duration,
```

### Comparing `onefuzz-8.3.0/onefuzz/templates/regression.py` & `onefuzz-8.4.0/onefuzz/templates/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         duration: int = 24,
         crash_report_timeout: Optional[int] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         check_retry_count: Optional[int] = None,
         check_fuzzer_help: bool = True,
         delete_input_container: bool = True,
         check_regressions: bool = False,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> None:
         """
         generic regression task
 
         :param File crashes: Specify crashing input files to check in the regression task
         :param str reports: Specify specific report names to verify in the regression task
         :param bool check_regressions: Specify if exceptions should be thrown on finding crash regressions
@@ -86,15 +86,15 @@
             duration=duration,
             crash_report_timeout=crash_report_timeout,
             debug=debug,
             check_retry_count=check_retry_count,
             check_fuzzer_help=check_fuzzer_help,
             delete_input_container=delete_input_container,
             check_regressions=check_regressions,
-            extra_container=extra_container,
+            extra_setup_container=extra_setup_container,
         )
 
     def libfuzzer(
         self,
         project: str,
         name: str,
         build: str,
@@ -113,15 +113,15 @@
         duration: int = 24,
         crash_report_timeout: Optional[int] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         check_retry_count: Optional[int] = None,
         check_fuzzer_help: bool = True,
         delete_input_container: bool = True,
         check_regressions: bool = False,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> None:
         """
         libfuzzer regression task
 
         :param File crashes: Specify crashing input files to check in the regression task
         :param str reports: Specify specific report names to verify in the regression task
         :param bool check_regressions: Specify if exceptions should be thrown on finding crash regressions
@@ -147,15 +147,15 @@
             duration=duration,
             crash_report_timeout=crash_report_timeout,
             debug=debug,
             check_retry_count=check_retry_count,
             check_fuzzer_help=check_fuzzer_help,
             delete_input_container=delete_input_container,
             check_regressions=check_regressions,
-            extra_container=extra_container,
+            extra_setup_container=extra_setup_container,
         )
 
     def _create_job(
         self,
         task_type: TaskType,
         project: str,
         name: str,
@@ -175,15 +175,15 @@
         duration: int = 24,
         crash_report_timeout: Optional[int] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         check_retry_count: Optional[int] = None,
         check_fuzzer_help: bool = True,
         delete_input_container: bool = True,
         check_regressions: bool = False,
-        extra_container: Optional[Container] = None,
+        extra_setup_container: Optional[Container] = None,
     ) -> None:
         if dryrun:
             return None
 
         self.logger.info("creating regression task from template")
 
         helper = JobHelper(
@@ -217,16 +217,16 @@
             ),
             (
                 ContainerType.regression_reports,
                 helper.containers[ContainerType.regression_reports],
             ),
         ]
 
-        if extra_container:
-            containers.append((ContainerType.extra, extra_container))
+        if extra_setup_container:
+            containers.append((ContainerType.extra_setup, extra_setup_container))
 
         if crashes:
             helper.containers[
                 ContainerType.readonly_inputs
             ] = helper.get_unique_container_name(ContainerType.readonly_inputs)
             containers.append(
                 (
```

### Comparing `onefuzz-8.3.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.4.0/onefuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.3.0
+Version: 8.4.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.3.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.4.0/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/setup.py` & `onefuzz-8.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.3.0/tests/test_template_helper.py` & `onefuzz-8.4.0/tests/test_template_helper.py`

 * *Files identical despite different names*

