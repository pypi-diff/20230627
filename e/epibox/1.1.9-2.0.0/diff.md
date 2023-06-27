# Comparing `tmp/epibox-1.1.9.tar.gz` & `tmp/epibox-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epibox-1.1.9.tar", last modified: Mon Jul  4 14:11:58 2022, max compression
+gzip compressed data, was "epibox-2.0.0.tar", last modified: Tue Jun 27 17:15:12 2023, max compression
```

## Comparing `epibox-1.1.9.tar` & `epibox-2.0.0.tar`

### file list

```diff
@@ -1,68 +1,59 @@
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.290702 epibox-1.1.9/
--rw-r--r--   0 anasofiacc   (501) staff       (20)      161 2021-12-10 17:05:43.000000 epibox-1.1.9/AUTHORS.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3518 2021-12-10 17:05:43.000000 epibox-1.1.9/CONTRIBUTING.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)       89 2021-12-10 17:05:43.000000 epibox-1.1.9/HISTORY.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1074 2021-12-10 17:05:43.000000 epibox-1.1.9/LICENSE
--rw-r--r--   0 anasofiacc   (501) staff       (20)      262 2021-12-10 17:05:43.000000 epibox-1.1.9/MANIFEST.in
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3386 2022-07-04 14:11:58.290826 epibox-1.1.9/PKG-INFO
--rw-r--r--   0 anasofiacc   (501) staff       (20)     2507 2021-12-10 17:05:43.000000 epibox-1.1.9/README.md
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.261906 epibox-1.1.9/docs/
--rw-r--r--   0 anasofiacc   (501) staff       (20)      607 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/Makefile
--rw-r--r--   0 anasofiacc   (501) staff       (20)       28 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/authors.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)     4781 2022-05-20 12:26:51.000000 epibox-1.1.9/docs/conf.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)       33 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/contributing.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)       28 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/history.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)      303 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/index.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1114 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/installation.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)      768 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/make.bat
--rw-r--r--   0 anasofiacc   (501) staff       (20)       27 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/readme.rst
--rw-r--r--   0 anasofiacc   (501) staff       (20)       67 2021-12-10 17:05:43.000000 epibox-1.1.9/docs/usage.rst
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.262925 epibox-1.1.9/epibox/
--rw-r--r--   0 anasofiacc   (501) staff       (20)      134 2022-07-04 14:08:06.000000 epibox-1.1.9/epibox/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)       90 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/__main__.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.279108 epibox-1.1.9/epibox/bit/
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/bit/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      740 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/bit/get_battery.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     2804 2022-05-22 10:58:54.000000 epibox-1.1.9/epibox/bit/header2bitalino.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3656 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/bit/manage_devices.py
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/bit/test.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      412 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/cli.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.288076 epibox-1.1.9/epibox/common/
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/common/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      103 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/close_file.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1625 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/connect_device.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      531 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/create_folder.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      423 2022-07-04 14:08:41.000000 epibox-1.1.9/epibox/common/disconnect_system.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      726 2022-05-22 14:20:35.000000 epibox-1.1.9/epibox/common/get_defaults.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      893 2022-05-22 10:47:57.000000 epibox-1.1.9/epibox/common/open_file.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      402 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/pair_device.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1557 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/process_data.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3444 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/read_modules.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1480 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/run_system.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     4893 2022-05-22 09:44:51.000000 epibox-1.1.9/epibox/common/setup.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1393 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/common/write_file.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      249 2022-07-04 14:08:53.000000 epibox-1.1.9/epibox/config_debug.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.288705 epibox-1.1.9/epibox/exceptions/
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/exceptions/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     2104 2022-07-04 11:01:09.000000 epibox-1.1.9/epibox/exceptions/exception_manager.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      171 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/exceptions/system_exceptions.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.289322 epibox-1.1.9/epibox/mqtt_manager/
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/mqtt_manager/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     2775 2022-05-22 09:55:16.000000 epibox-1.1.9/epibox/mqtt_manager/message_handler.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      174 2022-05-20 12:20:04.000000 epibox-1.1.9/epibox/mqtt_manager/utils.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.289739 epibox-1.1.9/epibox/run/
--rw-rw-r--   0 anasofiacc   (501) staff       (20)        0 2022-04-01 11:14:02.000000 epibox-1.1.9/epibox/run/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)     6732 2022-07-04 10:59:42.000000 epibox-1.1.9/epibox/run/run_bitalino.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.270518 epibox-1.1.9/epibox.egg-info/
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3386 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/PKG-INFO
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1341 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/SOURCES.txt
--rw-r--r--   0 anasofiacc   (501) staff       (20)        1 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/dependency_links.txt
--rw-r--r--   0 anasofiacc   (501) staff       (20)       43 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/entry_points.txt
--rw-r--r--   0 anasofiacc   (501) staff       (20)        1 2022-02-02 11:45:31.000000 epibox-1.1.9/epibox.egg-info/not-zip-safe
--rw-r--r--   0 anasofiacc   (501) staff       (20)     1018 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/requires.txt
--rw-r--r--   0 anasofiacc   (501) staff       (20)        7 2022-07-04 14:11:57.000000 epibox-1.1.9/epibox.egg-info/top_level.txt
--rw-r--r--   0 anasofiacc   (501) staff       (20)      378 2022-07-04 14:11:58.291257 epibox-1.1.9/setup.cfg
--rw-r--r--   0 anasofiacc   (501) staff       (20)     3146 2022-07-04 14:08:06.000000 epibox-1.1.9/setup.py
-drwxr-xr-x   0 anasofiacc   (501) staff       (20)        0 2022-07-04 14:11:58.290365 epibox-1.1.9/tests/
--rw-r--r--   0 anasofiacc   (501) staff       (20)       36 2021-12-10 17:05:43.000000 epibox-1.1.9/tests/__init__.py
--rw-r--r--   0 anasofiacc   (501) staff       (20)      892 2021-12-10 17:05:43.000000 epibox-1.1.9/tests/test_epibox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 17:15:02.000000 epibox-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 17:15:02.000000 epibox-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 17:15:02.000000 epibox-2.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 17:15:02.000000 epibox-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 17:15:02.000000 epibox-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:15:12.003492 epibox-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-27 17:15:02.000000 epibox-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/get_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/read_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/run_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/config_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/connect_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/manage_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/system_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/epibox/mqtt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/epibox/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:15:12.003492 epibox-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 17:15:02.000000 epibox-2.0.0/setup.py
```

### Comparing `epibox-1.1.9/CONTRIBUTING.rst` & `epibox-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/LICENSE` & `epibox-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/PKG-INFO` & `epibox-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 1.1.9
+Version: 2.0.0
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # EpiBOX, the Python package
 ## A Research Tool to Stimulate Collaboration Within Biosignal Collection
```

### Comparing `epibox-1.1.9/README.md` & `epibox-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/docs/Makefile` & `epibox-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/docs/conf.py` & `epibox-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/docs/installation.rst` & `epibox-2.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/docs/make.bat` & `epibox-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epibox-1.1.9/epibox/bit/header2bitalino.py` & `epibox-2.0.0/epibox/devices/header.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 from epibox import config_debug
 
 
-def header2bitalino(
+def get_header(
     filename,
     file_time,
     file_date,
     devices,
     mac_channels,
     sensors,
     fs,
     save_raw,
     service,
 ):
 
-    filename.write("# OpenSignals Text File Format" + "\n")
-
-    mac_dict = {}
+    header_dict = {}
     resolution = {}
+    columns = []
     fmt = []  # get format to save values in txt
 
     for n_device, device in enumerate(devices):
 
         fmt += ["%i"]
-        mac_dict[device.macAddress] = {}
-        mac_dict[device.macAddress]["sensor"] = []
+        header_dict[device.address] = {}
+        header_dict[device.address]["sensor"] = []
         for i, elem in enumerate(mac_channels):
-            if elem[0] == device.macAddress:
-                mac_dict[device.macAddress]["sensor"] += [sensors[i]]
+            if elem[0] == device.address:
+                header_dict[device.address]["sensor"] += [sensors[i]]
                 if save_raw:
                     fmt += ["%i"]
                 else:
                     fmt += ["%.2f"]
-        mac_dict[device.macAddress]["device name"] = "Device " + str(n_device + 1)
-
-        aux = ["A" + elem[1] for elem in mac_channels if elem[0] == device.macAddress]
-        mac_dict[device.macAddress]["column"] = ["nSeq"] + aux
+        header_dict[device.address]["device name"] = "Device " + \
+            str(n_device + 1)
 
-        mac_dict[device.macAddress]["sync interval"] = 2  # ???
+        aux = [elem[1]
+               for elem in mac_channels if elem[0] == device.address]
+        header_dict[device.address]["column"] = ["nSeq"] + aux
+        columns += header_dict[device.address]["column"]
 
-        mac_dict[device.macAddress]["start time"] = file_time
-        mac_dict[device.macAddress]["device connection"] = device.macAddress
+        header_dict[device.address]["start time"] = file_time
+        header_dict[device.address]["device connection"] = device.address
 
-        mac_dict[device.macAddress]["channels"] = [
-            int(elem[1]) for elem in mac_channels if elem[0] == device.macAddress
+        header_dict[device.address]["channels"] = [
+            int(elem[1]) for elem in mac_channels if elem[0] == device.address
         ]
 
-        mac_dict[device.macAddress]["date"] = file_date
-        # mac_dict[device.macAddress]["firmware version"] = device.version()
+        header_dict[device.address]["date"] = file_date
+        # header_dict[device.address]["firmware version"] = device.version()
 
-        if service == "Bitalino":
-            mac_dict[device.macAddress]["device"] = "bitalino_rev"
+        if service == "bitalino":
+            header_dict[device.address]["device"] = "bitalino_rev"
+            aux = [10, 10, 10, 10, 6, 6]  # resolution
+        elif service == "scientisst":
+            header_dict[device.address]["device"] = "scientisst_sense"
+            aux = [12, 12, 12, 12, 12, 12]
         else:
-            mac_dict[device.macAddress]["device"] = "bitalino_mini"
+            raise ValueError("Device not recognized")
+
+        aux2 = [1 for elem in mac_channels if elem[0] == device.address]
+        header_dict[device.address]["resolution"] = [4] + [
+            aux[i] for i in range(len(aux2))
+        ]
+        resolution[device.address] = header_dict[device.address]["resolution"]
 
-        mac_dict[device.macAddress]["sampling rate"] = fs
+        header_dict[device.address]["sampling rate"] = fs
 
         if save_raw:
-            mac_dict[device.macAddress]["label"] = [
-                "RAW"
-                for i, elem in enumerate(mac_channels)
-                if elem[0] == device.macAddress
+            header_dict[device.address]["label"] = [
+                "RAW" for elem in mac_channels if elem[0] == device.address
             ]
         else:
-            mac_dict[device.macAddress]["label"] = [
+            header_dict[device.address]["label"] = [
                 sensors[i]
                 for i, elem in enumerate(mac_channels)
-                if elem[0] == device.macAddress
+                if elem[0] == device.address
             ]
-        aux = [10, 10, 10, 10, 6, 6]
-        aux2 = [1 for elem in mac_channels if elem[0] == device.macAddress]
-        mac_dict[device.macAddress]["resolution"] = [4] + [
-            aux[i] for i in range(len(aux2))
-        ]
-        resolution[device.macAddress] = mac_dict[device.macAddress]["resolution"]
 
-    header = {"resolution": resolution, "save_raw": save_raw, "service": service}
+    header = {"resolution": resolution,
+              "save_raw": save_raw, "service": service}
+
+    config_debug.log(f"# {header_dict} \n")
+    config_debug.log(f"# {columns} \n")
 
-    config_debug.log(f"# {mac_dict} \n")
-    filename.write("# " + str(mac_dict) + "\n")
-    filename.write("# EndOfHeader" + "\n")
+    filename.write("# " + str(header_dict) + "\n")
+    filename.write("\t".join(columns) + "\n")
 
     return tuple(fmt), header
```

### Comparing `epibox-1.1.9/epibox/common/open_file.py` & `epibox-2.0.0/epibox/common/open_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # built-in
 from datetime import datetime
 import os
 
 # local
-from epibox.bit.header2bitalino import header2bitalino
+from epibox.devices.header import get_header
 
 
 def open_file(directory, devices, mac_channels, sensors, fs, save_raw, service):
 
     # for txt format
     now = datetime.now()
     save_time = now.strftime("%Y-%m-%d %H-%M-%S").rstrip("0")
     file_time = now.strftime("%Y-%m-%d %H:%M:%S.%f").rstrip("0")
     file_time = file_time[11:]
     file_time = '"' + file_time + '"'
     file_date = '"' + save_time[0:10] + '"'
 
-    a_file = open(os.path.join(directory, "A" + save_time + ".txt"), "w")  # data file
+    a_file = open(os.path.join(directory, "A" +
+                  save_time + ".txt"), "w")  # data file
 
     # create header for the acquisition file
-    save_fmt, header = header2bitalino(
+    save_fmt, header = get_header(
         a_file,
         file_time,
         file_date,
         devices,
         mac_channels,
         sensors,
         fs,
         save_raw,
         service,
     )
 
+
     return a_file, save_fmt, header
```

### Comparing `epibox-1.1.9/epibox/common/process_data.py` & `epibox-2.0.0/epibox/common/process_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # third-party
 from scipy import signal
 import itertools
 import numpy as np
 
+# local
 from epibox import config_debug
 
+
 def get_factors(n):
 
-    
     n2 = n
     i = 2
     factors = []
     while i * i <= n:
         if n % i:
             i += 1
         else:
-            n //= i
+            n = i
             factors.append(i)
     if n > 1:
         factors.append(n)
-    
-    factors.sort(reverse=True) 
+
+    factors.sort(reverse=True)
     final_factors = [f for f in factors if f > 13]
     to_combine = [f for f in factors if f < 13]
     combos = list(itertools.combinations(to_combine, 2))
 
     while np.prod(final_factors) != n2:
-        
-        config_debug.log(f'combos: {combos}')
-        combination = [[i,p] for i,p in enumerate([x * y for x,y in combos]) if p <= 13]
+
+        config_debug.log(f"combos: {combos}")
+        combination = [
+            [i, p] for i, p in enumerate([x * y for x, y in combos]) if p <= 13
+        ]
 
         final_factors += [combination[0][1]]
-        config_debug.log(f'final_factors: {final_factors}')
+        config_debug.log(f"final_factors: {final_factors}")
 
         combos.remove(combos[combination[0][0]])
-    
+
     return final_factors
 
+
 def decimate(t, fs):
     # if phisiological signal downsample to 100Hz, if acc decimate 10Hz
     t_display = []
 
     for i in range(t.shape[1]):
-        t_aux = t[:,i]
-#         for n in get_factors(fs / 100):
-#             try:
-#                 t_aux = signal.decimate(t_aux, int(n))
-#                 config_debug.log('after decimate: {}'.format(t_aux))
-#             except Exception as e:
-#                 config_debug.log(e)
-#                 pass
+        t_aux = t[:, i]
         if fs >= 1000:
             t_aux = signal.decimate(t_aux, 10)
-            
-        t_display += [t_aux.tolist()]
 
+        t_display += [t_aux.tolist()]
 
-    return t_display
+    return t_display
```

### Comparing `epibox-1.1.9/epibox/common/read_modules.py` & `epibox-2.0.0/epibox/common/read_modules.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,131 @@
 # built-in
 from copy import copy
 
 # third-party
 import numpy as np
 
 from epibox import config_debug
-
+from epibox.exceptions.system_exceptions import DeviceNotInAcquisitionError
 
 
 def read_modules(devices, mac_channels, sensors, header):
 
-    
     t = np.array([])
     t_display = np.array([])
-    # 
-    # config_debug.log('devices: {}'.format([d.macAddress for d in devices]))
-    channels2get = [int(mac_chn[1])-1 for mac_chn in mac_channels]
-        
-    for i, device in enumerate(devices):
-
-        t_read = device.read(100)
+    channels2get = [int(mac_chn[1]) - 1 for mac_chn in mac_channels]
 
-        if header['service'] == 'Bitalino' or header['service'] == 'Mini':
-            t_read = np.delete(t_read, np.arange(1,5), axis=1) # remove digital channels
-            t_nseq = t_read[:,1:] # remove nSeq column (add again in the end)
+    for i, device in enumerate(devices):
 
-        else:
-            seq = []
-            t_nseq = []
-            
-            for f in t_read:
-
-                frame = f.toMap()
-                seq += [frame['sequence']]
-
-                if len(t_nseq) == 0:
-                    t_nseq_aux = np.reshape(np.array(frame['analog']), (1,-1))
-                    t_nseq = np.reshape(np.take(t_nseq_aux, channels2get), (1,-1))
-                else:
-                    t_nseq_aux = np.reshape(np.take(np.reshape(np.array(frame['analog']), (1,-1)), channels2get), (1,-1))
-                    t_nseq = np.vstack((t_nseq, t_nseq_aux))
+        try:
+            if header["service"] == "bitalino":
+                t_read = device.read(100)
+            elif header["service"] == "scientisst":
+                t_read = device.read(convert=False, matrix=True)
+
+        except Exception as e:
+            config_debug.log(e)
+            raise DeviceNotInAcquisitionError
+
+        t_read = np.delete(
+            t_read, np.arange(1, 5), axis=1
+        )  # remove digital channels
+        t_nseq = t_read[:, 1:]  # remove nSeq column (add again in the end)
+
+
+        # else:
+        #     seq = []
+        #     t_nseq = []
+
+        #     for f in t_read:
+
+        #         frame = f.toMap()
+        #         seq += [frame["sequence"]]
+
+        #         if len(t_nseq) == 0:
+        #             t_nseq_aux = np.reshape(np.array(frame["analog"]), (1, -1))
+        #             t_nseq = np.reshape(
+        #                 np.take(t_nseq_aux, channels2get), (1, -1))
+        #         else:
+        #             t_nseq_aux = np.reshape(
+        #                 np.take(
+        #                     np.reshape(
+        #                         np.array(frame["analog"]), (1, -1)), channels2get
+        #                 ),
+        #                 (1, -1),
+        #             )
+        #             t_nseq = np.vstack((t_nseq, t_nseq_aux))
 
-            t_read = np.hstack((np.reshape(np.array(seq), (-1,1)), t_nseq))
+        #t_read = np.hstack((np.reshape(np.array(seq), (-1, 1)), t_nseq))
 
-        #config_debug.log(t_read)
+        config_debug.log(t_nseq)
 
         n = 0
         display_aux = np.array([])
 
-        for j,chn in enumerate(mac_channels):
+        for j, chn in enumerate(mac_channels):
 
-            if chn[0] == device.macAddress:
+            if chn[0] == device.address:
 
-                if header['save_raw']:
-                    signal_type = 'RAW'
+                if header["save_raw"]:
+                    signal_type = "RAW"
 
                 else:
                     signal_type = sensors[j]
 
-                r = header['resolution'][device.macAddress][n+1]
-                t_aux = get_transform(t_nseq[:,n], signal_type, r) # receives and returns a column with 100 samples
+                r = header["resolution"][device.address][n + 1]
+                t_aux = get_transform(
+                    t_nseq[:, n], signal_type, r
+                )  # receives and returns a column with 100 samples
 
                 n += 1
                 if len(display_aux) == 0:
                     display_aux = copy(t_aux)
 
                 else:
                     display_aux = np.concatenate((display_aux, t_aux), axis=1)
 
-  
         if len(t_display) == 0:
             t_display = copy(display_aux)
-            t = np.concatenate((np.reshape(t_read[:,0], (-1,1)), display_aux), axis=1)
+            t = np.concatenate(
+                (np.reshape(t_read[:, 0], (-1, 1)), display_aux), axis=1)
 
         else:
             t_display = np.concatenate((t_display, display_aux), axis=1)
-            aux = np.concatenate((np.reshape(t_read[:,0], (-1,1)), display_aux), axis=1)
+            aux = np.concatenate(
+                (np.reshape(t_read[:, 0], (-1, 1)), display_aux), axis=1
+            )
             t = np.concatenate((t, aux), axis=1)
 
-    t_str = '\n'.join(' '.join('%0.1f' %x for x in y) for y in t)
+    t_str = "\n".join(" ".join("%0.1f" % x for x in y) for y in t)
     return t, t_str, t_display
 
 
-
 def get_transform(raw, signal_type, res):
 
-    if signal_type == 'ECG':
-        aux = list(map(lambda x: (((x/(2**res)-0.5)*3.3)/1100)*1000, raw))
-
-    elif signal_type == 'EEG':
-        aux = list(map(lambda x: (((x/(2**res)-0.5)*3.3)/41782)*(10**(6)), raw))
-
-    elif signal_type == 'EOG':
-        aux = list(map(lambda x: (((x/(2**res)-0.5)*3.3)/2040)*1000, raw))
+    if signal_type == "ECG":
+        aux = list(
+            map(lambda x: (((x / (2**res) - 0.5) * 3.3) / 1100) * 1000, raw))
+
+    elif signal_type == "EEG":
+        aux = list(
+            map(lambda x: (((x / (2**res) - 0.5) * 3.3) / 41782) * (10 ** (6)), raw)
+        )
+
+    elif signal_type == "EOG":
+        aux = list(
+            map(lambda x: (((x / (2**res) - 0.5) * 3.3) / 2040) * 1000, raw))
+
+    elif signal_type == "EMG":
+        aux = list(
+            map(lambda x: (((x / (2**res) - 0.5) * 3.3) / 1009) * 1000, raw))
 
-    elif signal_type == 'EMG':
-        aux = list(map(lambda x: (((x/(2**res)-0.5)*3.3)/1009)*1000, raw))
+    elif signal_type == "PZT":
+        aux = list(map(lambda x: (x / (2**res) - 0.5) * 100, raw))
 
-    elif signal_type == 'PZT':
-        aux = list(map(lambda x: (x/(2**res)-0.5)*100, raw))
-
-    elif signal_type == 'EDA':
-        aux = list(map(lambda x: (((x/(2**res))*3.3)/0.132), raw))
+    elif signal_type == "EDA":
+        aux = list(map(lambda x: (((x / (2**res)) * 3.3) / 0.132), raw))
 
     else:
         aux = list(raw)
 
-    return np.reshape(np.asarray(aux), (-1,1))
-
-        
-
+    return np.reshape(np.asarray(aux), (-1, 1))
```

### Comparing `epibox-1.1.9/epibox/common/setup.py` & `epibox-2.0.0/epibox/common/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # built-in
-from http import client
 import time
-import pwd
 import os
-import ast
+from sys import platform
 
 # third-party
-import json
 import paho.mqtt.client as mqtt
 from epibox.common.get_defaults import get_default
-from epibox.exceptions.exception_manager import error_kill
+from epibox.exceptions.system_exceptions import (
+    MQTTConnectionError,
+    PlatformNotSupportedError,
+    StorageTimeout,
+)
 
 # local
 from epibox.mqtt_manager.message_handler import on_message, send_default
 from epibox.mqtt_manager.utils import random_str
 from epibox import config_debug
 
 
@@ -21,40 +22,44 @@
     # Set up MQTT client =========================================================================
 
     client_name = random_str(6)
     config_debug.log(f"Client name (acquisition): {client_name}")
     host_name = "192.168.0.10"
     topic = "rpi"
 
+    # raises ValueError and ConnectionRefusedError
     client = mqtt.Client(client_name)
 
     setattr(client, "keepAlive", True)
     setattr(client, "pauseAcq", False)
     setattr(client, "newAnnot", None)
 
-    client.username_pw_set(username="preepiseizures", password="preepiseizures")
-    client.connect(host_name)
-    client.subscribe(topic)
+    client.username_pw_set(username="preepiseizures",
+                           password="preepiseizures")
+    client.connect(host_name)  # raises ValueError
+    client.subscribe(topic)  # raises ValueError
     client.on_message = on_message
     client.loop_start()
     config_debug.log(f"Successfully subcribed to topic {topic}")
 
-    client.publish("rpi", str(["STARTING"]))
+    message_info = client.publish(
+        "rpi", str(["STARTING"])
+    )  # raises ValueError and TypeError
+    if message_info.rc == 4:
+        raise MQTTConnectionError
 
     return client
 
 
 def setup_config(client):
     # Access default configurations on EpiBOX Core and save them to variables ======================
 
-    username = pwd.getpwuid(os.getuid())[0]
-
     # inform the EpiBOX App which are the current default devices
-    send_default(client, username)
-    opt = get_default(username)
+    send_default(client)
+    opt = get_default()
 
     if not opt["channels"]:
         # if default "channels" is empty, acquire all
         channels = []
         for device in opt["devices_mac"].values():
             for i in range(1, 7):
                 channels += [[device, str(i)]]
@@ -67,15 +72,16 @@
         try:
             for triplet in opt["channels"]:
                 triplet[0] = opt["devices_mac"][
                     triplet[0]
                 ]  # replace MAC ID for corresponding MAC
                 channels += [triplet[:2]]
                 sensors += [triplet[2]]
-        except Exception as e:
+
+        except Exception as e:  # TODO what kind of errors are raised?
             config_debug.log(e)
             for tt, triplet in enumerate(opt["channels"]):
                 if tt < 7:
                     triplet[0] = opt["devices_mac"]["MAC1"]
                 else:
                     triplet[0] = opt["devices_mac"]["MAC2"]
                 channels += [triplet[:2]]
@@ -83,15 +89,15 @@
 
     save_raw = bool(opt["save_raw"])
     service = opt["service"]
 
     opt["devices_mac"] = [m for m in opt["devices_mac"].values() if m != ""]
 
     # check if default storage is available | if not, terminate setup loop and acquisition
-    opt = check_storage(client, [], opt)
+    opt = check_storage(client, opt)
 
     config_debug.log("ID: {}".format(opt["patient_id"]))
     config_debug.log("folder: {}".format(opt["initial_dir"]))
     config_debug.log("fs: {}".format(opt["fs"]))
     config_debug.log(f"save_raw: {save_raw}")
     config_debug.log(f"channels: {channels}")
     config_debug.log("devices: {}".format(opt["devices_mac"]))
@@ -101,53 +107,47 @@
     return opt, channels, sensors, service, save_raw
 
 
 def setup_variables():
 
     already_notified_pause = False
     system_started = False
-    files_open = False
     t_all = []
 
-    return t_all, already_notified_pause, system_started, files_open
+    return t_all, already_notified_pause, system_started
 
 
-def check_storage(client, devices, opt):
+def check_storage(client, opt):
     # Check if default storage is available | loop runs continuosly until it find the storage or until timeout
     # If timeout, setup loop and acquisition are terminated
 
-    username = pwd.getpwuid(os.getuid())[0]
+    if platform == "linux" or platform == "linux2":
+        # linux
+        drive_path = f"/media/{os.environ.get('USERNAME')}"
+    elif platform == "darwin":
+        # macos
+        drive_path = "/Volumes"
+    else:
+        # import win32api
+        drive_path = ""
 
     init_connect_time = time.time()
     config_debug.log(f'Searching for storage module: {opt["initial_dir"]}')
 
-    i = 0
-    while client.keepAlive:
-
-        i += 1
+    for i in range(100000):
 
         if (time.time() - init_connect_time) > 120:
-            error_kill(
-                client,
-                devices,
-                "Failed to find storage",
-                "ERROR",
-                files_open=False,
-                devices_connected=False,
-            )
+            raise StorageTimeout
 
-        try:
-            if os.path.isdir("/media/{}/".format(username) + opt["initial_dir"]):
-                opt["initial_dir"] = (
-                    "/media/{}/".format(username) + opt["initial_dir"] + "/acquisitions"
-                )
-                break
-
-            else:
-                if time.time() - init_connect_time > 3 * i:
-                    client.publish("rpi", str(["INSERT STORAGE"]))
-                raise Exception
+        if os.path.isdir(f"/{drive_path}/" + opt["initial_dir"]):
+            opt["initial_dir"] = (
+                f"/{drive_path}/" + opt["initial_dir"] + "/acquisitions"
+            )
+            break
 
-        except Exception as e:
-            continue
+        else:
+            if time.time() - init_connect_time > 3 * i:
+                message_info = client.publish("rpi", str(["INSERT STORAGE"]))
+                if message_info.rc == 4:
+                    raise MQTTConnectionError
 
     return opt
```

### Comparing `epibox-1.1.9/epibox/run/run_bitalino.py` & `epibox-2.0.0/epibox/run/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 # built-in
 import json
-from time import sleep
 
 # local
-from epibox.bit.manage_devices import pause_devices, connect_devices, start_devices
+from epibox.devices.manage_devices import connect_devices, start_devices
 from epibox.exceptions.exception_manager import (
-    error_disconnect,
-    error_kill,
-    client_kill,
+    handle_case_6,
+    kill_case_1,
+    kill_case_2,
+    kill_case_3,
+    kill_case_4,
+    kill_case_5,
+    kill_case_7,
 )
 from epibox.common.setup import setup_client, setup_config, setup_variables
 from epibox.common.create_folder import create_folder
 from epibox.common.open_file import open_file
 from epibox.common.write_file import write_annot_file
 from epibox.common.run_system import run_system
 from epibox.common import process_data
 from epibox import config_debug
+from epibox.exceptions.system_exceptions import (
+    BITalinoParameterError,
+    DeviceConnectionTimeout,
+    DeviceNotIDLEError,
+    DeviceNotInAcquisitionError,
+    MQTTConnectionError,
+    PlatformNotSupportedError,
+    StorageTimeout,
+)
 
 
 # ****************************** MAIN SCRIPT ***********************************
 # This is the main script. It is lauched by EpiBOX Core, through the epibox_startup.sh Bash script.
 
 # This script attempts to connect to the default biosignal acquisition devices in a continuous loop.
 # The loop stops only if:
@@ -33,140 +45,156 @@
 #       - user stops the acquisition
 #       - at least one of the devices disconnects
 
 
 def main():
 
     devices = []
-
+    # Setup MQTT client | read default configurations | initiate variables ===========================
     try:
-        # Setup MQTT client | read default configurations | initiate variables ===========================
         client = setup_client()
+
+    except (MQTTConnectionError, ConnectionRefusedError, ValueError, TypeError) as e:
+        config_debug.log(e)
+        kill_case_1()
+
+    try:
         opt, channels, sensors, service, save_raw = setup_config(client)
 
-        t_all, already_notified_pause, system_started, files_open = setup_variables()
+        (
+            t_all,
+            already_notified_pause,
+            system_started,
+        ) = setup_variables()  # raises no errors
 
         # Create folder with patient ID
         directory = create_folder(
-            opt["initial_dir"], "{}".format(opt["patient_id"]), service
-        )
-        already_timed_out = False
+            opt["initial_dir"], "{}".format(opt["patient_id"]))
 
-        # Start loop to connect PyEpiBOX to acquisition devices =========================================
-        devices = connect_devices(
-            client, devices, opt, already_timed_out, files_open=False
-        )
+    except MQTTConnectionError as e:
+        kill_case_1()
+    except (
+        ConnectionRefusedError,
+        ValueError,
+        TypeError,
+        OSError,
+        StorageTimeout,
+        PlatformNotSupportedError,
+    ) as e:
+        config_debug.log(e)
+        kill_case_2(client)
 
-    except Exception as e:
-        sleep(3)
-        error_kill(
-            client,
-            devices,
-            msg="Failed initial setup",
-            files_open=False,
-            devices_connected=False,
-        )
+    already_timed_out = False
 
+    # Start loop to connect PyEpiBOX to acquisition devices =========================================
     try:
-        # Open acquisition file | get format and header info ============================================
-        a_file, save_fmt, header = open_file(
-            directory, devices, channels, sensors, opt["fs"], save_raw, service
+        devices = connect_devices(  # exceptions handled inside
+            client, devices, opt, already_timed_out,
         )
-        files_open = True
 
-    except Exception as e:
-        error_kill(client, devices, msg="Failed to open the files", files_open=False)
+    except (
+        DeviceConnectionTimeout,
+        ValueError,
+        TypeError,
+        BITalinoParameterError,
+    ) as e:
+        config_debug.log(e)
+        kill_case_3(client, devices)
 
-    # Starting acquisition loop ===========================================================================
-    # This loop runs continuously unless the user stops the acquisition on the EpiBOX App or at least one of
-    # the devices disconnects
-    try:
-        while client.keepAlive == True:
+    except MQTTConnectionError as e:
+        config_debug.log(e)
+        kill_case_4(devices)
+
+    config_debug.log("Initial setup complete!")
+
+    while client.keepAlive:
+
+        try:
 
             if client.newAnnot != None:
                 # Write user annotation to file if one is received via MQTT ===============================
+                # TODO exception handling
                 config_debug.log(f"annot: {client.newAnnot}")
                 write_annot_file(a_file.name, client.newAnnot)
                 client.newAnnot = None
 
-            config_debug.log("im here")
             if client.pauseAcq and not already_notified_pause:
                 # Pause acquisition if command is received via MQTT ========================================
-                devices = pause_devices(client, devices)
+
+                # devices = pause_devices(client, devices)
+                system_started = handle_case_6(devices, a_file, system_started)
+                message_info = client.publish("rpi", str(["PAUSED"]))
+                if message_info.rc == 4:
+                    raise MQTTConnectionError
                 already_notified_pause = True
 
-            elif not client.pauseAcq:
+            if not client.pauseAcq:
 
                 if already_notified_pause:
-                    client.publish("rpi", str(["RECONNECTING"]))
+                    message_info = client.publish("rpi", str(["RECONNECTING"]))
+                    if message_info.rc == 4:
+                        raise MQTTConnectionError
                     already_notified_pause = False
 
                 if not system_started:
                     # If the devices have not yet started acquiring or they are paused, start acquisition
-                    try:
-                        sync_param = start_devices(
-                            client, devices, opt["fs"], channels, header
-                        )
-                        system_started = True
-                        already_timed_out = False
-
-                    except Exception as e:
-                        config_debug.log(e)
-                        pass
-
-                try:
-                    # Read batch of samples from the acquisition devices and store on the active session's file
-                    _, t_disp, a_file, sync_param = run_system(
-                        devices,
-                        a_file,
-                        sync_param,
-                        directory,
-                        channels,
-                        sensors,
-                        opt["fs"],
-                        save_raw,
-                        service,
-                        save_fmt,
-                        header,
-                        client,
-                    )
-
-                    # Subsample batch of samples and send to the EpiBOX App for visualization purposes ==========
-                    t_display = process_data.decimate(t_disp, opt["fs"])
-                    t_all += t_display[0]
-                    json_data = json.dumps(["DATA", t_display, channels, sensors])
-                    client.publish("rpi", json_data)
-
-                    already_timed_out = False
-
-                # Handle misconnection of the devices ============================================================
-                except Exception as e:
-                    devices, system_started = error_disconnect(
-                        client, devices, e, a_file
-                    )
-                    devices = connect_devices(
-                        client, devices, opt, already_timed_out, a_file
-                    )
-                    system_started = False
                     a_file, save_fmt, header = open_file(
                         directory,
                         devices,
                         channels,
                         sensors,
                         opt["fs"],
                         save_raw,
                         service,
                     )
+                    sync_param = start_devices(
+                        client, devices, opt["fs"], channels, header
+                    )
+                    system_started = True
+                    already_timed_out = False
 
-            else:
-                pass
-
-        client_kill(
-            client, devices, "You have stopped the acquisition", a_file, files_open
-        )
-
-    except KeyboardInterrupt:
-        client_kill(
-            client, devices, "You have stopped the acquisition", a_file, files_open
-        )
+                # Read batch of samples from the acquisition devices and store on the active session's file
+                _, t_disp, a_file, sync_param = run_system(
+                    devices,
+                    a_file,
+                    sync_param,
+                    channels,
+                    sensors,
+                    save_fmt,
+                    header,
+                    client,
+                )
+
+                # Subsample batch of samples and send to the EpiBOX App for visualization purposes ================
+                t_display = process_data.decimate(t_disp, opt["fs"])
+                t_all += t_display[0]
+                json_data = json.dumps(["DATA", t_display, channels, sensors])
+                message_info = client.publish("rpi", json_data)
+                if message_info.rc == 4:
+                    raise MQTTConnectionError
+
+                already_timed_out = False
+
+        except (
+            DeviceNotIDLEError,
+            BITalinoParameterError,
+            FileNotFoundError,
+            PermissionError,
+            OSError,
+            KeyboardInterrupt,
+        ) as e:
+            config_debug.log(e)
+            kill_case_5(client, devices, a_file)
+
+        except DeviceNotInAcquisitionError as e:
+            config_debug.log(e)
+            message_info = client.publish("rpi", str(["RECONNECTING"]))
+            if message_info.rc == 4:
+                raise MQTTConnectionError
+            system_started = handle_case_6(devices, a_file, system_started)
+            continue
+
+        except MQTTConnectionError as e:
+            config_debug.log(e)
+            kill_case_7(client, devices, a_file)
 
     # =========================================================================================================
```

### Comparing `epibox-1.1.9/epibox.egg-info/PKG-INFO` & `epibox-2.0.0/epibox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 1.1.9
+Version: 2.0.0
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # EpiBOX, the Python package
 ## A Research Tool to Stimulate Collaboration Within Biosignal Collection
```

### Comparing `epibox-1.1.9/epibox.egg-info/SOURCES.txt` & `epibox-2.0.0/epibox.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 epibox/__init__.py
 epibox/__main__.py
-epibox/cli.py
 epibox/config_debug.py
 epibox.egg-info/PKG-INFO
 epibox.egg-info/SOURCES.txt
 epibox.egg-info/dependency_links.txt
 epibox.egg-info/entry_points.txt
 epibox.egg-info/not-zip-safe
 epibox.egg-info/requires.txt
 epibox.egg-info/top_level.txt
-epibox/bit/__init__.py
-epibox/bit/get_battery.py
-epibox/bit/header2bitalino.py
-epibox/bit/manage_devices.py
-epibox/bit/test.py
 epibox/common/__init__.py
-epibox/common/close_file.py
-epibox/common/connect_device.py
 epibox/common/create_folder.py
-epibox/common/disconnect_system.py
 epibox/common/get_defaults.py
 epibox/common/open_file.py
-epibox/common/pair_device.py
 epibox/common/process_data.py
 epibox/common/read_modules.py
 epibox/common/run_system.py
 epibox/common/setup.py
 epibox/common/write_file.py
+epibox/devices/__init__.py
+epibox/devices/connect_device.py
+epibox/devices/header.py
+epibox/devices/manage_devices.py
 epibox/exceptions/__init__.py
 epibox/exceptions/exception_manager.py
 epibox/exceptions/system_exceptions.py
 epibox/mqtt_manager/__init__.py
 epibox/mqtt_manager/message_handler.py
 epibox/mqtt_manager/utils.py
 epibox/run/__init__.py
-epibox/run/run_bitalino.py
-tests/__init__.py
-tests/test_epibox.py
+epibox/run/run.py
```

