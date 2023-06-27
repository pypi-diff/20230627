# Comparing `tmp/balepy-0.5.tar.gz` & `tmp/balepy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.5.tar", last modified: Tue Jun 27 19:44:54 2023, max compression
+gzip compressed data, was "balepy-0.5.1.tar", last modified: Tue Jun 27 19:52:55 2023, max compression
```

## Comparing `balepy-0.5.tar` & `balepy-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:44:54.536596 balepy-0.5/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.5/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-27 19:44:54.536596 balepy-0.5/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.5/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:44:54.533263 balepy-0.5/balepy/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     2104 2023-06-27 19:44:14.000000 balepy-0.5/balepy/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:44:54.536596 balepy-0.5/balepy.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-27 19:44:54.000000 balepy-0.5/balepy.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-27 19:44:54.000000 balepy-0.5/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-27 19:44:54.000000 balepy-0.5/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-27 19:44:54.000000 balepy-0.5/balepy.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-27 19:44:54.536596 balepy-0.5/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      987 2023-06-27 19:44:34.000000 balepy-0.5/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:52:55.789019 balepy-0.5.1/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.5.1/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-27 19:52:55.789019 balepy-0.5.1/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.5.1/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:52:55.785686 balepy-0.5.1/balepy/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     2109 2023-06-27 19:51:51.000000 balepy-0.5.1/balepy/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:52:55.785686 balepy-0.5.1/balepy.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-27 19:52:55.000000 balepy-0.5.1/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-27 19:52:55.000000 balepy-0.5.1/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-27 19:52:55.000000 balepy-0.5.1/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-27 19:52:55.000000 balepy-0.5.1/balepy.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-27 19:52:55.789019 balepy-0.5.1/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      989 2023-06-27 19:52:21.000000 balepy-0.5.1/setup.py
```

### Comparing `balepy-0.5/LICENSE` & `balepy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-0.5/PKG-INFO` & `balepy-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.5
+Version: 0.5.1
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.5/balepy/__init__.py` & `balepy-0.5.1/balepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     #
     def send_Message(self , chat_id:int , text:str):
         text.replace(" ", "+")
         a = requests.get(f"https://tapi.bale.ai/bot{self.token}/sendMessage?chat_id={chat_id}&text={text}")
         return a
 	#
     def getupdate(self):
-        a = requests.get(f"https://tapi.bale.ai/bot{token}/getupdates")
+        a = requests.get(f"https://tapi.bale.ai/bot{self.token}/getupdates")
         a = a.json()
         a = a['result']
         return a
 	#
     def get_lastupdate(self):
         a = requests.get(f"https://tapi.bale.ai/bot{self.token}/getupdates")
         a = a.json()
```

### Comparing `balepy-0.5/balepy.egg-info/PKG-INFO` & `balepy-0.5.1/balepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.5
+Version: 0.5.1
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.5/setup.py` & `balepy-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.5',
+    version = '0.5.1',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

