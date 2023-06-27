# Comparing `tmp/lfinancial-0.1.1.tar.gz` & `tmp/lfinancial-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.1.tar", last modified: Tue Jun 27 03:27:01 2023, max compression
+gzip compressed data, was "lfinancial-0.1.2.tar", last modified: Tue Jun 27 12:37:04 2023, max compression
```

## Comparing `lfinancial-0.1.1.tar` & `lfinancial-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:27:01.649618 lfinancial-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 03:26:44.000000 lfinancial-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-27 03:27:01.649618 lfinancial-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 03:26:44.000000 lfinancial-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:27:01.649618 lfinancial-0.1.1/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 03:26:44.000000 lfinancial-0.1.1/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-27 03:26:44.000000 lfinancial-0.1.1/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-27 03:26:44.000000 lfinancial-0.1.1/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:27:01.649618 lfinancial-0.1.1/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-27 03:27:01.000000 lfinancial-0.1.1/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 03:27:01.000000 lfinancial-0.1.1/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:27:01.000000 lfinancial-0.1.1/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 03:27:01.000000 lfinancial-0.1.1/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:27:01.649618 lfinancial-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-27 03:26:44.000000 lfinancial-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:27:01.649618 lfinancial-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 03:26:44.000000 lfinancial-0.1.1/tests/test_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 12:36:43.000000 lfinancial-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-27 12:37:04.785813 lfinancial-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-27 12:36:43.000000 lfinancial-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:37:04.785813 lfinancial-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-27 12:36:43.000000 lfinancial-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 12:36:43.000000 lfinancial-0.1.2/tests/test_document_type.py
```

### Comparing `lfinancial-0.1.1/LICENSE.txt` & `lfinancial-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.1/README.md` & `lfinancial-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LFinancial is a Python package that generates financial fake data.
+lfinancial is a Python package that generates financial fake data.
 
 ---
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |    
 } '--. } '_}  | } | }\  { /  /\  \ | }\  { | },-. | } /  /\  \ } '--. 
 `----' `--'   `-' `-' `-' `-'  `-' `-' `-' `----' `-' `-'  `-' `----' 
@@ -33,8 +33,23 @@
 # EG4130431
 
 f.nric()
 # SD44949622
 
 f.my_number()
 # 399495927695
+
+f.cn_name()
+# 于诚玲
+
+f.first_name()
+# Cakadiq
+
+f.middle_name()
+# Baviv
+
+f.last_name()
+# Hucacuqa
+
+f.kana_name()
+# ハジ
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lfinancial-0.1.1/setup.py` & `lfinancial-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.1.1',
+    version='0.1.2',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

