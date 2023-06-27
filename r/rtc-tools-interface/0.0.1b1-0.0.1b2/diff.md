# Comparing `tmp/rtc-tools-interface-0.0.1b1.tar.gz` & `tmp/rtc-tools-interface-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-interface-0.0.1b1.tar", last modified: Tue Jun 27 12:58:59 2023, max compression
+gzip compressed data, was "rtc-tools-interface-0.0.1b2.tar", last modified: Tue Jun 27 13:43:06 2023, max compression
```

## Comparing `rtc-tools-interface-0.0.1b1.tar` & `rtc-tools-interface-0.0.1b2.tar`

### file list

```diff
@@ -1,15 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:59.890485 rtc-tools-interface-0.0.1b1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-27 12:58:58.000000 rtc-tools-interface-0.0.1b1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-27 12:58:59.890485 rtc-tools-interface-0.0.1b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3906 2023-06-27 12:58:58.000000 rtc-tools-interface-0.0.1b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:59.890485 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-27 12:58:59.000000 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-27 12:58:59.000000 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:58:59.000000 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-27 12:58:59.000000 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:58:59.000000 rtc-tools-interface-0.0.1b1/rtc_tools_interface.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:59.891485 rtc-tools-interface-0.0.1b1/rtctools_interface/
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-27 12:58:59.891485 rtc-tools-interface-0.0.1b1/rtctools_interface/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-27 12:58:59.891485 rtc-tools-interface-0.0.1b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-27 12:58:58.000000 rtc-tools-interface-0.0.1b1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-27 12:58:58.000000 rtc-tools-interface-0.0.1b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.155802 rtc-tools-interface-0.0.1b2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-27 13:43:06.155802 rtc-tools-interface-0.0.1b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3906 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.152802 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-27 13:43:06.000000 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-27 13:43:06.000000 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:43:06.000000 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-27 13:43:06.000000 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-27 13:43:06.000000 rtc-tools-interface-0.0.1b2/rtc_tools_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.155802 rtc-tools-interface-0.0.1b2/rtctools_interface/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-27 13:43:06.155802 rtc-tools-interface-0.0.1b2/rtctools_interface/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.153802 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/base_goal.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/goal_generator_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/read_goals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/rtctools_interface/optimization/read_plot_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-27 13:43:06.155802 rtc-tools-interface-0.0.1b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.153802 rtc-tools-interface-0.0.1b2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:43:06.154802 rtc-tools-interface-0.0.1b2/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/optimization/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/optimization/test_base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/optimization/test_plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/tests/optimization/test_read_goals.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-27 13:43:04.000000 rtc-tools-interface-0.0.1b2/versioneer.py
```

### Comparing `rtc-tools-interface-0.0.1b1/COPYING.LESSER` & `rtc-tools-interface-0.0.1b2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.0.1b1/README.md` & `rtc-tools-interface-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.0.1b1/versioneer.py` & `rtc-tools-interface-0.0.1b2/versioneer.py`

 * *Files identical despite different names*

