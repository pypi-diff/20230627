# Comparing `tmp/pybw_comic-23.6.27.1.tar.gz` & `tmp/pybw_comic-23.6.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybw_comic-23.6.27.1.tar", last modified: Tue Jun 27 09:41:14 2023, max compression
+gzip compressed data, was "pybw_comic-23.6.27.2.tar", last modified: Tue Jun 27 09:46:29 2023, max compression
```

## Comparing `pybw_comic-23.6.27.1.tar` & `pybw_comic-23.6.27.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:41:14.826714 pybw_comic-23.6.27.1/
--rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw_comic-23.6.27.1/- command.txt
--rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw_comic-23.6.27.1/LICENSE
--rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw_comic-23.6.27.1/MANIFEST.in
--rw-rw-rw-   0        0        0      765 2023-06-27 09:41:14.824715 pybw_comic-23.6.27.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-21 09:53:53.000000 pybw_comic-23.6.27.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 09:41:14.703706 pybw_comic-23.6.27.1/pybw_comic/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.1/pybw_comic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:41:14.809713 pybw_comic-23.6.27.1/pybw_comic/engine/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.1/pybw_comic/engine/__init__.py
--rw-rw-rw-   0        0        0    18753 2023-06-20 12:37:25.000000 pybw_comic-23.6.27.1/pybw_comic/engine/_todo_dmzj_cn.py
--rw-rw-rw-   0        0        0    18538 2023-06-21 10:30:25.000000 pybw_comic-23.6.27.1/pybw_comic/engine/_todo_dmzj_requests.py
--rw-rw-rw-   0        0        0    17144 2022-09-21 08:09:06.000000 pybw_comic-23.6.27.1/pybw_comic/engine/cnanjie.py
--rw-rw-rw-   0        0        0    20850 2023-06-27 09:27:08.000000 pybw_comic-23.6.27.1/pybw_comic/engine/copymanga.py
--rw-rw-rw-   0        0        0    22139 2023-06-21 12:15:34.000000 pybw_comic-23.6.27.1/pybw_comic/engine/dmzj_selenium.py
--rw-rw-rw-   0        0        0    23738 2022-09-21 08:08:24.000000 pybw_comic-23.6.27.1/pybw_comic/engine/manhuaDB.py
--rw-rw-rw-   0        0        0    24178 2022-09-21 08:09:13.000000 pybw_comic-23.6.27.1/pybw_comic/engine/maofly.py
--rw-rw-rw-   0        0        0    20791 2022-09-21 08:08:55.000000 pybw_comic-23.6.27.1/pybw_comic/engine/mhkan.py
--rw-rw-rw-   0        0        0    20845 2022-09-21 08:08:09.000000 pybw_comic-23.6.27.1/pybw_comic/engine/www_1kkk.py
--rw-rw-rw-   0        0        0    20667 2023-06-21 12:06:21.000000 pybw_comic-23.6.27.1/pybw_comic/engine/xmanhua.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:41:14.815713 pybw_comic-23.6.27.1/pybw_comic/scripts/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.1/pybw_comic/scripts/__init__.py
--rw-rw-rw-   0        0        0     3404 2023-06-27 09:26:19.000000 pybw_comic-23.6.27.1/pybw_comic/scripts/comic.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:41:14.730708 pybw_comic-23.6.27.1/pybw_comic.egg-info/
--rw-rw-rw-   0        0        0      765 2023-06-27 09:41:14.000000 pybw_comic-23.6.27.1/pybw_comic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-06-27 09:41:14.000000 pybw_comic-23.6.27.1/pybw_comic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:41:14.000000 pybw_comic-23.6.27.1/pybw_comic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 09:41:14.000000 pybw_comic-23.6.27.1/pybw_comic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       23 2023-06-21 09:53:36.000000 pybw_comic-23.6.27.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:41:14.826714 pybw_comic-23.6.27.1/setup.cfg
--rw-rw-rw-   0        0        0     1508 2023-06-27 09:37:57.000000 pybw_comic-23.6.27.1/setup.py
--rwxrwxrwx   0        0        0      353 2023-06-27 09:41:06.000000 pybw_comic-23.6.27.1/upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2023-06-27 09:46:29.957878 pybw_comic-23.6.27.2/
+-rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw_comic-23.6.27.2/- command.txt
+-rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw_comic-23.6.27.2/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw_comic-23.6.27.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      765 2023-06-27 09:46:29.956877 pybw_comic-23.6.27.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-21 09:53:53.000000 pybw_comic-23.6.27.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:46:29.816867 pybw_comic-23.6.27.2/pybw_comic/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.2/pybw_comic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:46:29.937876 pybw_comic-23.6.27.2/pybw_comic/engine/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.2/pybw_comic/engine/__init__.py
+-rw-rw-rw-   0        0        0    18753 2023-06-20 12:37:25.000000 pybw_comic-23.6.27.2/pybw_comic/engine/_todo_dmzj_cn.py
+-rw-rw-rw-   0        0        0    18538 2023-06-21 10:30:25.000000 pybw_comic-23.6.27.2/pybw_comic/engine/_todo_dmzj_requests.py
+-rw-rw-rw-   0        0        0    17144 2022-09-21 08:09:06.000000 pybw_comic-23.6.27.2/pybw_comic/engine/cnanjie.py
+-rw-rw-rw-   0        0        0    20851 2023-06-27 09:45:55.000000 pybw_comic-23.6.27.2/pybw_comic/engine/copymanga.py
+-rw-rw-rw-   0        0        0    22139 2023-06-21 12:15:34.000000 pybw_comic-23.6.27.2/pybw_comic/engine/dmzj_selenium.py
+-rw-rw-rw-   0        0        0    23738 2022-09-21 08:08:24.000000 pybw_comic-23.6.27.2/pybw_comic/engine/manhuaDB.py
+-rw-rw-rw-   0        0        0    24178 2022-09-21 08:09:13.000000 pybw_comic-23.6.27.2/pybw_comic/engine/maofly.py
+-rw-rw-rw-   0        0        0    20791 2022-09-21 08:08:55.000000 pybw_comic-23.6.27.2/pybw_comic/engine/mhkan.py
+-rw-rw-rw-   0        0        0    20845 2022-09-21 08:08:09.000000 pybw_comic-23.6.27.2/pybw_comic/engine/www_1kkk.py
+-rw-rw-rw-   0        0        0    20667 2023-06-21 12:06:21.000000 pybw_comic-23.6.27.2/pybw_comic/engine/xmanhua.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:46:29.945876 pybw_comic-23.6.27.2/pybw_comic/scripts/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.6.27.2/pybw_comic/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3404 2023-06-27 09:26:19.000000 pybw_comic-23.6.27.2/pybw_comic/scripts/comic.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:46:29.848870 pybw_comic-23.6.27.2/pybw_comic.egg-info/
+-rw-rw-rw-   0        0        0      765 2023-06-27 09:46:29.000000 pybw_comic-23.6.27.2/pybw_comic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-06-27 09:46:29.000000 pybw_comic-23.6.27.2/pybw_comic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:46:29.000000 pybw_comic-23.6.27.2/pybw_comic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 09:46:29.000000 pybw_comic-23.6.27.2/pybw_comic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       23 2023-06-21 09:53:36.000000 pybw_comic-23.6.27.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:46:29.958879 pybw_comic-23.6.27.2/setup.cfg
+-rw-rw-rw-   0        0        0     1508 2023-06-27 09:46:17.000000 pybw_comic-23.6.27.2/setup.py
+-rwxrwxrwx   0        0        0      353 2023-06-27 09:41:06.000000 pybw_comic-23.6.27.2/upload_pypi.bat
```

### Comparing `pybw_comic-23.6.27.1/- command.txt` & `pybw_comic-23.6.27.2/- command.txt`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/LICENSE` & `pybw_comic-23.6.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/PKG-INFO` & `pybw_comic-23.6.27.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw_comic
-Version: 23.6.27.1
+Version: 23.6.27.2
 Summary: comic spider
 Home-page: https://gitee.com/pubowei/comic
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/comic
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/_todo_dmzj_cn.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/_todo_dmzj_cn.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/_todo_dmzj_requests.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/_todo_dmzj_requests.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/cnanjie.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/cnanjie.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/copymanga.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/copymanga.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 warnings.filterwarnings("ignore")
 
 
 Headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36'}
 
 
 _xpath_catelogue = {
-    'book_name': '/html/body/main/div[1]/div/div[2]/ul/li[2]/p',
+    'book_name': '/html/body/main/div[1]/div/div[2]/ul/li[1]/h6',
     'author': '/html/body/main/div[1]/div/div[2]/ul/li[3]/span[2]/a',
     'state': '/html/body/main/div[1]/div/div[2]/ul/li[6]/span[2]',
     'topic': '/html/body/main/div[1]/div/div[2]/ul/li[7]/span[2]/a',
     'last_update': '/html/body/main/div[1]/div/div[2]/ul/li[5]/span[2]',
     
     'columns': '/html/body/main/div[2]/div[3]/div/div[1]/ul/li/a',
     'chapters': {-1: '/html/body/main/div[2]/div[3]/div/div[2]/div/div/ul[1]/a',
```

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/dmzj_selenium.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/dmzj_selenium.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/manhuaDB.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/manhuaDB.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/maofly.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/maofly.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/mhkan.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/mhkan.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/www_1kkk.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/www_1kkk.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/engine/xmanhua.py` & `pybw_comic-23.6.27.2/pybw_comic/engine/xmanhua.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic/scripts/comic.py` & `pybw_comic-23.6.27.2/pybw_comic/scripts/comic.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/pybw_comic.egg-info/PKG-INFO` & `pybw_comic-23.6.27.2/pybw_comic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw-comic
-Version: 23.6.27.1
+Version: 23.6.27.2
 Summary: comic spider
 Home-page: https://gitee.com/pubowei/comic
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/comic
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw_comic-23.6.27.1/pybw_comic.egg-info/SOURCES.txt` & `pybw_comic-23.6.27.2/pybw_comic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.6.27.1/setup.py` & `pybw_comic-23.6.27.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='pybw_comic',
-    version='23.6.27.1',
+    version='23.6.27.2',
     python_requires='>=3.6',
     
     author='Bowei Pu',
     author_email='pubowei@foxmail.com',
     
     description='comic spider',
     long_description=readme,
```

