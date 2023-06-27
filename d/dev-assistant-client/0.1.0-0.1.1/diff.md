# Comparing `tmp/dev-assistant-client-0.1.0.tar.gz` & `tmp/dev-assistant-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.0.tar", last modified: Mon Jun 26 03:17:36 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.1.tar", last modified: Tue Jun 27 03:27:17 2023, max compression
```

## Comparing `dev-assistant-client-0.1.0.tar` & `dev-assistant-client-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 03:17:36.524993 dev-assistant-client-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-06-26 03:08:53.000000 dev-assistant-client-0.1.0/LICENCE
--rw-rw-rw-   0        0        0      337 2023-06-26 03:17:36.523993 dev-assistant-client-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-26 03:08:42.000000 dev-assistant-client-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 03:17:36.504994 dev-assistant-client-0.1.0/dev_assistant_client/
--rw-rw-rw-   0        0        0        0 2023-06-26 03:07:42.000000 dev-assistant-client-0.1.0/dev_assistant_client/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-26 03:07:42.000000 dev-assistant-client-0.1.0/dev_assistant_client/main.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:17:36.522993 dev-assistant-client-0.1.0/dev_assistant_client.egg-info/
--rw-rw-rw-   0        0        0      337 2023-06-26 03:17:36.000000 dev-assistant-client-0.1.0/dev_assistant_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-26 03:17:36.000000 dev-assistant-client-0.1.0/dev_assistant_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 03:17:36.000000 dev-assistant-client-0.1.0/dev_assistant_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-26 03:17:36.000000 dev-assistant-client-0.1.0/dev_assistant_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 03:17:36.524993 dev-assistant-client-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-06-26 03:16:34.000000 dev-assistant-client-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.884971 dev-assistant-client-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      343 2023-06-27 03:27:17.882970 dev-assistant-client-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1559 2023-06-27 03:12:02.000000 dev-assistant-client-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.872971 dev-assistant-client-0.1.1/dev_assistant_client/
+-rw-rw-rw-   0        0        0        0 2023-06-26 03:07:42.000000 dev-assistant-client-0.1.1/dev_assistant_client/__init__.py
+-rw-rw-rw-   0        0        0     3039 2023-06-27 03:19:57.000000 dev-assistant-client-0.1.1/dev_assistant_client/main.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.880972 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 03:27:17.885968 dev-assistant-client-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      577 2023-06-27 03:22:34.000000 dev-assistant-client-0.1.1/setup.py
```

