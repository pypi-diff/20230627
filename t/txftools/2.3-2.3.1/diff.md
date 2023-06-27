# Comparing `tmp/txftools-2.3.tar.gz` & `tmp/txftools-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txftools-2.3.tar", last modified: Wed Apr 26 02:05:26 2023, max compression
+gzip compressed data, was "txftools-2.3.1.tar", last modified: Tue Jun 27 01:53:33 2023, max compression
```

## Comparing `txftools-2.3.tar` & `txftools-2.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.126616 txftools-2.3/
--rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.3/LICENSE
--rw-rw-rw-   0        0        0      427 2023-04-26 02:05:26.125619 txftools-2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 02:05:26.126616 txftools-2.3/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-04-26 02:04:56.000000 txftools-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.111655 txftools-2.3/txftools/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.3/txftools/__init__.py
--rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.3/txftools/currency_sorted.py
--rw-rw-rw-   0        0        0    21033 2023-04-26 02:01:19.000000 txftools-2.3/txftools/encryption.py
--rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.3/txftools/execute_redis.py
--rw-rw-rw-   0        0        0    23966 2023-01-14 06:53:46.000000 txftools-2.3/txftools/format_data.py
--rw-rw-rw-   0        0        0     4800 2022-11-21 03:28:29.000000 txftools-2.3/txftools/lazy_test.py
--rw-rw-rw-   0        0        0      514 2023-04-22 06:18:06.000000 txftools-2.3/txftools/pipfile_lock_requirements.py
--rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.3/txftools/province.py
--rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.3/txftools/send_emals.py
--rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.3/txftools/ssh_online.py
--rw-rw-rw-   0        0        0    13181 2023-04-26 02:04:13.000000 txftools-2.3/txftools/timer.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.125619 txftools-2.3/txftools.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.3/txftools.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-27 01:53:33.797562 txftools-2.3.1/
+-rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      429 2023-06-27 01:53:33.795569 txftools-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:53:33.797562 txftools-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-27 01:53:11.000000 txftools-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:53:33.773804 txftools-2.3.1/txftools/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.3.1/txftools/__init__.py
+-rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.3.1/txftools/currency_sorted.py
+-rw-rw-rw-   0        0        0    21033 2023-04-26 02:01:19.000000 txftools-2.3.1/txftools/encryption.py
+-rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.3.1/txftools/execute_redis.py
+-rw-rw-rw-   0        0        0    23966 2023-01-14 06:53:46.000000 txftools-2.3.1/txftools/format_data.py
+-rw-rw-rw-   0        0        0     4800 2022-11-21 03:28:29.000000 txftools-2.3.1/txftools/lazy_test.py
+-rw-rw-rw-   0        0        0     3046 2023-06-27 01:52:12.000000 txftools-2.3.1/txftools/only_id.py
+-rw-rw-rw-   0        0        0      514 2023-04-22 06:18:06.000000 txftools-2.3.1/txftools/pipfile_lock_requirements.py
+-rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.3.1/txftools/province.py
+-rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.3.1/txftools/send_emals.py
+-rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.3.1/txftools/ssh_online.py
+-rw-rw-rw-   0        0        0    13181 2023-04-26 02:04:13.000000 txftools-2.3.1/txftools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:53:33.793571 txftools-2.3.1/txftools.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-06-27 01:53:33.000000 txftools-2.3.1/txftools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-06-27 01:53:33.000000 txftools-2.3.1/txftools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:53:33.000000 txftools-2.3.1/txftools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-27 01:53:33.000000 txftools-2.3.1/txftools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 01:53:33.000000 txftools-2.3.1/txftools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.3.1/txftools.egg-info/zip-safe
```

### Comparing `txftools-2.3/LICENSE` & `txftools-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `txftools-2.3/setup.py` & `txftools-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(name='txftools',  # 名字
-      version='2.3',  # 版本
+      version='2.3.1',  # 版本
       long_description_content_type="text/markdown",
       long_description='README',
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
```

### Comparing `txftools-2.3/txftools/__init__.py` & `txftools-2.3.1/txftools/__init__.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/currency_sorted.py` & `txftools-2.3.1/txftools/currency_sorted.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/encryption.py` & `txftools-2.3.1/txftools/encryption.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/execute_redis.py` & `txftools-2.3.1/txftools/execute_redis.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/format_data.py` & `txftools-2.3.1/txftools/format_data.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/lazy_test.py` & `txftools-2.3.1/txftools/lazy_test.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/pipfile_lock_requirements.py` & `txftools-2.3.1/txftools/pipfile_lock_requirements.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/province.py` & `txftools-2.3.1/txftools/province.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/send_emals.py` & `txftools-2.3.1/txftools/send_emals.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/ssh_online.py` & `txftools-2.3.1/txftools/ssh_online.py`

 * *Files identical despite different names*

### Comparing `txftools-2.3/txftools/timer.py` & `txftools-2.3.1/txftools/timer.py`

 * *Files identical despite different names*

