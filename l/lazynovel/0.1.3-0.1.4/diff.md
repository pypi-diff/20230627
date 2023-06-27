# Comparing `tmp/lazynovel-0.1.3.tar.gz` & `tmp/lazynovel-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazynovel-0.1.3.tar", last modified: Mon May 29 10:33:16 2023, max compression
+gzip compressed data, was "lazynovel-0.1.4.tar", last modified: Tue Jun 27 08:26:26 2023, max compression
```

## Comparing `lazynovel-0.1.3.tar` & `lazynovel-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.983145 lazynovel-0.1.3/
--rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.3/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-29 10:33:16.983034 lazynovel-0.1.3/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.3/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.982157 lazynovel-0.1.3/lazynovel/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.3/lazynovel/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.3/lazynovel/crawler_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/crawler_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1932 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/crawler_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_dianzhong.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.3/lazynovel/open_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yangguang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yiqbook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yuewen.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.982858 lazynovel-0.1.3/lazynovel.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-05-29 10:33:16.983196 lazynovel-0.1.3/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-05-29 10:32:37.000000 lazynovel-0.1.3/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-27 08:26:26.688337 lazynovel-0.1.4/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.4/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-06-27 08:26:26.688196 lazynovel-0.1.4/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.4/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-27 08:26:26.687309 lazynovel-0.1.4/lazynovel/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.4/lazynovel/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.4/lazynovel/crawler_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/crawler_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5902 2023-06-27 08:25:54.000000 lazynovel-0.1.4/lazynovel/crawler_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_dianzhong.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.4/lazynovel/open_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_yangguang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_yiqbook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.4/lazynovel/open_yuewen.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-27 08:26:26.688031 lazynovel-0.1.4/lazynovel.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-06-27 08:26:26.000000 lazynovel-0.1.4/lazynovel.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-06-27 08:26:26.000000 lazynovel-0.1.4/lazynovel.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-27 08:26:26.000000 lazynovel-0.1.4/lazynovel.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-06-27 08:26:26.000000 lazynovel-0.1.4/lazynovel.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-06-27 08:26:26.000000 lazynovel-0.1.4/lazynovel.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-27 08:26:26.688389 lazynovel-0.1.4/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-06-27 08:24:54.000000 lazynovel-0.1.4/setup.py
```

### Comparing `lazynovel-0.1.3/LICENSE` & `lazynovel-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/PKG-INFO` & `lazynovel-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.3
+Version: 0.1.4
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.3/README.md` & `lazynovel-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/crawler_changdu.py` & `lazynovel-0.1.4/lazynovel/crawler_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/crawler_mbookcn.py` & `lazynovel-0.1.4/lazynovel/crawler_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_changdu.py` & `lazynovel-0.1.4/lazynovel/open_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_dianzhong.py` & `lazynovel-0.1.4/lazynovel/open_dianzhong.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_mbookcn.py` & `lazynovel-0.1.4/lazynovel/open_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_reading163.py` & `lazynovel-0.1.4/lazynovel/open_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_yangguang.py` & `lazynovel-0.1.4/lazynovel/open_yangguang.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_yiqbook.py` & `lazynovel-0.1.4/lazynovel/open_yiqbook.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel/open_yuewen.py` & `lazynovel-0.1.4/lazynovel/open_yuewen.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.3/lazynovel.egg-info/PKG-INFO` & `lazynovel-0.1.4/lazynovel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.3
+Version: 0.1.4
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.3/setup.py` & `lazynovel-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazynovel",
-    version="0.1.3",
+    version="0.1.4",
     description="小说平台接口封包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazynovel",
     packages=setuptools.find_packages(),
```

