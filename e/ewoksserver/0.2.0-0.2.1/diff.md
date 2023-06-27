# Comparing `tmp/ewoksserver-0.2.0.tar.gz` & `tmp/ewoksserver-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksserver-0.2.0.tar", last modified: Mon Jun 12 17:22:04 2023, max compression
+gzip compressed data, was "dist/ewoksserver-0.2.1.tar", last modified: Tue Jun 27 16:42:30 2023, max compression
```

## Comparing `ewoksserver-0.2.0.tar` & `ewoksserver-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1468 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-12 17:20:31.000000 ewoksserver-0.2.0/src/ewoksserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/events/ewoks_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/events/websocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9845 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/resources/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/icons.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/default.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/graphInput.svg
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/graphOutput.svg
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/demo.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     4256 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3332 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/workflows.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7568 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3053 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.svg
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.png
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.svg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/dummy_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_icons.py
--rw-rw-rw-   0 root         (0) root         (0)     5956 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_websocket_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2221 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 16:42:12.000000 ewoksserver-0.2.1/src/ewoksserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:42:24.000000 ewoksserver-0.2.1/src/ewoksserver/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/events/ewoks_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/events/websocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9845 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/binary/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/binary/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/binary/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:42:24.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-06-27 16:41:09.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/default.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/graphInput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/graphOutput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:42:24.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:42:24.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/data/workflows/demo.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/events/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/events/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     4256 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/json/workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/resources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7526 2023-06-27 16:16:45.000000 ewoksserver-0.2.1/src/ewoksserver/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:42:24.000000 ewoksserver-0.2.1/src/ewoksserver/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/icon1.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/icon1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/icon2.png
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/data/icon2.svg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/dummy_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5956 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_websocket_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2023-06-27 07:03:10.000000 ewoksserver-0.2.1/src/ewoksserver/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-27 16:42:30.000000 ewoksserver-0.2.1/src/ewoksserver.egg-info/top_level.txt
```

### Comparing `ewoksserver-0.2.0/LICENSE.md` & `ewoksserver-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/PKG-INFO` & `ewoksserver-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.2.0/README.md` & `ewoksserver-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/setup.cfg` & `ewoksserver-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/events/ewoks_events.py` & `ewoksserver-0.2.1/src/ewoksserver/events/ewoks_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/events/websocket.py` & `ewoksserver-0.2.1/src/ewoksserver/events/websocket.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/__init__.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/api.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/api.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/binary/icons.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/binary/icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/binary/resource.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/binary/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/binary/utils.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/binary/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/sum.png` & `ewoksserver-0.2.1/src/ewoksserver/resources/data/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/demo.json` & `ewoksserver-0.2.1/src/ewoksserver/resources/data/workflows/demo.json`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/events/resource.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/events/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/json/__init__.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/json/resource.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/json/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/json/tasks.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/json/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/json/utils.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/json/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/resources/json/workflows.py` & `ewoksserver-0.2.1/src/ewoksserver/resources/json/workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/server.py` & `ewoksserver-0.2.1/src/ewoksserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,42 +35,42 @@
 from .resources.json.tasks import discover_tasks
 from .events.websocket import add_events
 
 
 def create_app(**config) -> Tuple[flask.Flask, Api, FlaskApiSpec]:
     app = flask.Flask(__name__, static_folder=get_static_root(), static_url_path="")
     CORS(app)
-    configure_app(app, **config)
-    apidoc = add_apidoc(app)
-    api = add_api(app, apidoc)
+    _configure_app(app, **config)
+    apidoc = __add_apidoc(app)
+    api = _add_api(app, apidoc)
     return app, api, apidoc
 
 
-def add_api(app: flask.Flask, apidoc: FlaskApiSpec) -> Api:
+def _add_api(app: flask.Flask, apidoc: FlaskApiSpec) -> Api:
     api = Api(app)
     add_resources(api, apidoc)
     return api
 
 
-def configure_app(app: flask.Flask, configuration: Optional[str] = None, **config):
+def _configure_app(app: flask.Flask, configuration: Optional[str] = None, **config):
     app.config["CORS_HEADERS"] = "Content-Type"
     filename = os.environ.get("EWOKSSERVER_SETTINGS")
     if configuration:
         filename = configuration
     if filename:
         filename = os.path.relpath(filename, app.config.root_path)
         app.config.from_pyfile(filename, silent=False)
     if config:
         config = {k.upper(): v for k, v in config.items() if v is not None}
         app.config.update(config)
     if app.config.get("CELERY"):
         current_celery_app.conf.update(app.config["CELERY"])
 
 
-def print_config(app: flask.Flask):
+def _print_config(app: flask.Flask):
     resourcedir = app.config.get("RESOURCE_DIRECTORY")
     if not resourcedir:
         resourcedir = "."
     print(f"\nRESOURCE DIRECTORY:\n {os.path.abspath(resourcedir)}\n")
 
     adict = app.config.get("CELERY")
     if adict:
@@ -81,70 +81,64 @@
     adict = app.config.get("EWOKS")
     if adict:
         print(f"\nEWOKS:\n {pformat(adict)}\n")
     else:
         print("\nEWOKS:\n Not configured (no ewoks execution events)\n")
 
 
-def print_serve_message(app, port: Optional[int] = None) -> None:
-    host = "127.0.0.1"
-    if port is None:
-        server_name = app.config["SERVER_NAME"]
-        if server_name and ":" in server_name:
-            port = int(server_name.rsplit(":", 1)[1])
-        else:
-            port = 5000
+def _print_serve_message(host: str, port: int) -> None:
     print("\nTo start editing workflows, open this link in a browser:\n")
     print(f"    http://{host}:{port}\n")
 
 
-def set_log_level(app: Optional[flask.Flask] = None, log_level=logging.WARNING):
+def _set_log_level(app: Optional[flask.Flask] = None, log_level=logging.WARNING):
     logging.basicConfig(level=log_level)
     if app is not None:
         app.logger.setLevel(log_level)
 
 
 def add_socket(app: flask.Flask) -> SocketIO:
     socketio = SocketIO(app, cors_allowed_origins="*")
     add_events(socketio)
     return socketio
 
 
-def add_apidoc(app: flask.Flask) -> FlaskApiSpec:
+def __add_apidoc(app: flask.Flask) -> FlaskApiSpec:
     app.config.update(
         {
             "APISPEC_TITLE": "ewoks",
             # "APISPEC_OAS_VERSION": "3.0.3",
             "APISPEC_SWAGGER_URL": "/swagger/",
             "APISPEC_SWAGGER_UI_URL": "/swagger-ui/",
         }
     )
     return FlaskApiSpec(app)
 
 
-def save_apidoc(apidoc: FlaskApiSpec, filename: str) -> None:
+def _save_apidoc(apidoc: FlaskApiSpec, filename: str) -> None:
     save_spec_dir = os.path.dirname(filename)
     if save_spec_dir:
         os.makedirs(save_spec_dir, exist_ok=True)
     with open(filename, "w") as f:
         json.dump(apidoc.spec.to_dict(), f)
 
 
-def run_app(
+def _run_app(
     app: flask.Flask,
+    host: str,
+    port: int,
     socketio: Optional[SocketIO] = None,
-    port: int = 5000,
     init_context: Optional[ContextManager] = None,
 ) -> None:
     with run_context(app, init_context=init_context):
         if socketio is None:
-            app.run(port=port)
+            app.run(host=host, port=port)
         else:
             # allow_unsafe_werkzeug=True, see MR1877
-            socketio.run(app, port=port)
+            socketio.run(app, host=host, port=port)
 
 
 @contextmanager
 def run_context(
     app: flask.Flask,
     init_context: Optional[ContextManager] = None,
     local_pool_options: Optional[Dict] = None,
@@ -159,15 +153,15 @@
             stack.enter_context(ctx)
         if init_context is not None:
             ctx = init_context(app)
             stack.enter_context(ctx)
         yield
 
 
-def rediscover_tasks(app: flask.Flask):
+def _rediscover_tasks(app: flask.Flask):
     tasks = discover_tasks(app)
     root_url = resource_utils.root_url(app.config.get("RESOURCE_DIRECTORY"), "tasks")
     for resource in tasks:
         resource_utils.save_resource(root_url, resource["task_identifier"], resource)
 
 
 def main(argv=None):
@@ -181,14 +175,21 @@
         dest="log_level",
         type=str.upper,
         default="WARNING",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
         help="Set the logging level",
     )
     parser.add_argument(
+        "--host",
+        dest="host",
+        type=str,
+        default="127.0.0.1",
+        help="Host name",
+    )
+    parser.add_argument(
         "-p",
         "--port",
         dest="port",
         type=int,
         default=5000,
         help="Port number",
     )
@@ -240,29 +241,29 @@
             raise RuntimeError("ewoksweb is not installed")
         args.configuration = get_test_config()
 
     app, _, apidoc = create_app(
         configuration=args.configuration, resource_directory=args.resource_directory
     )
     if args.spec_filename:
-        save_apidoc(apidoc, args.spec_filename)
+        _save_apidoc(apidoc, args.spec_filename)
         return
 
     if args.without_events:
         socketio = None
     else:
         socketio = add_socket(app)
-    set_log_level(log_level=log_level)
+    _set_log_level(log_level=log_level)
 
     @contextmanager
     def init_context(app):
         if args.rediscover_tasks:
-            rediscover_tasks(app)
+            _rediscover_tasks(app)
         yield
 
-    print_config(app)
-    print_serve_message(app, port=args.port)
-    run_app(app, socketio=socketio, port=args.port, init_context=init_context)
+    _print_config(app)
+    _print_serve_message(args.host, args.port)
+    _run_app(app, args.host, args.port, socketio=socketio, init_context=init_context)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/conftest.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.png` & `ewoksserver-0.2.1/src/ewoksserver/tests/data/icon1.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.png` & `ewoksserver-0.2.1/src/ewoksserver/tests/data/icon2.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_data.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_events.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_execute.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_icons.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_tasks.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_websocket_connection.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver/tests/test_workflows.py` & `ewoksserver-0.2.1/src/ewoksserver/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.2.0/src/ewoksserver.egg-info/PKG-INFO` & `ewoksserver-0.2.1/src/ewoksserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.2.0/src/ewoksserver.egg-info/SOURCES.txt` & `ewoksserver-0.2.1/src/ewoksserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

