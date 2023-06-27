# Comparing `tmp/polywrap_client-0.1.0a34.tar.gz` & `tmp/polywrap_client-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client-0.1.0a34.tar", max compression
+gzip compressed data, was "polywrap_client-0.1.0a4.tar", max compression
```

## Comparing `polywrap_client-0.1.0a34.tar` & `polywrap_client-0.1.0a4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1230 2023-06-27 11:59:05.056871 polywrap_client-0.1.0a34/README.md
--rw-r--r--   0        0        0       86 2023-06-27 11:59:05.056871 polywrap_client-0.1.0a34/polywrap_client/__init__.py
--rw-r--r--   0        0        0     9490 2023-06-27 11:59:05.056871 polywrap_client-0.1.0a34/polywrap_client/client.py
--rw-r--r--   0        0        0        0 2023-06-27 11:59:05.056871 polywrap_client-0.1.0a34/polywrap_client/py.typed
--rw-r--r--   0        0        0     1364 2023-06-27 12:04:57.303667 polywrap_client-0.1.0a34/pyproject.toml
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a34/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-02-24 13:52:49.839099 polywrap_client-0.1.0a4/README.md
+-rw-r--r--   0        0        0       22 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/__init__.py
+-rw-r--r--   0        0        0     5313 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/client.py
+-rw-r--r--   0        0        0     1283 2023-02-24 14:00:34.812101 polywrap_client-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/setup.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/PKG-INFO
```

