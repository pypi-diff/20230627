# Comparing `tmp/raymics-0.7.2.tar.gz` & `tmp/raymics-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raymics-0.7.2.tar", last modified: Tue Jun 27 08:22:57 2023, max compression
+gzip compressed data, was "raymics-0.7.3.tar", last modified: Tue Jun 27 08:24:41 2023, max compression
```

## Comparing `raymics-0.7.2.tar` & `raymics-0.7.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:22:57.294863 raymics-0.7.2/
--rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-27 08:22:57.294695 raymics-0.7.2/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     6013 2023-06-25 03:11:09.000000 raymics-0.7.2/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:22:57.293816 raymics-0.7.2/raymics/
--rw-r--r--   0 john       (501) staff       (20)       47 2023-06-26 05:44:33.000000 raymics-0.7.2/raymics/__init__.py
--rw-r--r--   0 john       (501) staff       (20)      727 2023-06-25 03:11:09.000000 raymics-0.7.2/raymics/constants.py
--rw-r--r--   0 john       (501) staff       (20)     3921 2023-06-25 03:11:09.000000 raymics-0.7.2/raymics/dataset.py
--rw-r--r--   0 john       (501) staff       (20)    21616 2023-06-26 09:25:05.000000 raymics-0.7.2/raymics/extract_radiomics_features.py
--rw-r--r--   0 john       (501) staff       (20)      232 2023-06-25 03:11:09.000000 raymics-0.7.2/raymics/log.py
--rw-r--r--   0 john       (501) staff       (20)     5569 2023-06-25 03:11:09.000000 raymics-0.7.2/raymics/task.py
--rw-r--r--   0 john       (501) staff       (20)     2477 2023-06-25 03:11:09.000000 raymics-0.7.2/raymics/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:22:57.294469 raymics-0.7.2/raymics.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-27 08:22:57.000000 raymics-0.7.2/raymics.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      318 2023-06-27 08:22:57.000000 raymics-0.7.2/raymics.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-27 08:22:57.000000 raymics-0.7.2/raymics.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)      193 2023-06-27 08:22:57.000000 raymics-0.7.2/raymics.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        8 2023-06-27 08:22:57.000000 raymics-0.7.2/raymics.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-27 08:22:57.294899 raymics-0.7.2/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      608 2023-06-27 08:22:49.000000 raymics-0.7.2/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:24:41.937390 raymics-0.7.3/
+-rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-27 08:24:41.937236 raymics-0.7.3/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     6013 2023-06-25 03:11:09.000000 raymics-0.7.3/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:24:41.936361 raymics-0.7.3/raymics/
+-rw-r--r--   0 john       (501) staff       (20)       47 2023-06-26 05:44:33.000000 raymics-0.7.3/raymics/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      727 2023-06-25 03:11:09.000000 raymics-0.7.3/raymics/constants.py
+-rw-r--r--   0 john       (501) staff       (20)     3921 2023-06-25 03:11:09.000000 raymics-0.7.3/raymics/dataset.py
+-rw-r--r--   0 john       (501) staff       (20)    21616 2023-06-26 09:25:05.000000 raymics-0.7.3/raymics/extract_radiomics_features.py
+-rw-r--r--   0 john       (501) staff       (20)      232 2023-06-25 03:11:09.000000 raymics-0.7.3/raymics/log.py
+-rw-r--r--   0 john       (501) staff       (20)     5569 2023-06-25 03:11:09.000000 raymics-0.7.3/raymics/task.py
+-rw-r--r--   0 john       (501) staff       (20)     2477 2023-06-25 03:11:09.000000 raymics-0.7.3/raymics/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-27 08:24:41.937055 raymics-0.7.3/raymics.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     6128 2023-06-27 08:24:41.000000 raymics-0.7.3/raymics.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      318 2023-06-27 08:24:41.000000 raymics-0.7.3/raymics.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-27 08:24:41.000000 raymics-0.7.3/raymics.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)      193 2023-06-27 08:24:41.000000 raymics-0.7.3/raymics.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        8 2023-06-27 08:24:41.000000 raymics-0.7.3/raymics.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-27 08:24:41.937433 raymics-0.7.3/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      608 2023-06-27 08:24:15.000000 raymics-0.7.3/setup.py
```

### Comparing `raymics-0.7.2/PKG-INFO` & `raymics-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raymics
-Version: 0.7.2
+Version: 0.7.3
 Summary: Raymics Tools
 Description-Content-Type: text/markdown
 
 # 提取Radiomics特征
 
 ## 1. 安装特征提取工具包
```

### Comparing `raymics-0.7.2/README.md` & `raymics-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics/constants.py` & `raymics-0.7.3/raymics/constants.py`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics/dataset.py` & `raymics-0.7.3/raymics/dataset.py`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics/extract_radiomics_features.py` & `raymics-0.7.3/raymics/extract_radiomics_features.py`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics/task.py` & `raymics-0.7.3/raymics/task.py`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics/utils.py` & `raymics-0.7.3/raymics/utils.py`

 * *Files identical despite different names*

### Comparing `raymics-0.7.2/raymics.egg-info/PKG-INFO` & `raymics-0.7.3/raymics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raymics
-Version: 0.7.2
+Version: 0.7.3
 Summary: Raymics Tools
 Description-Content-Type: text/markdown
 
 # 提取Radiomics特征
 
 ## 1. 安装特征提取工具包
```

### Comparing `raymics-0.7.2/setup.py` & `raymics-0.7.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         with open(fname, 'r') as f:
             targets = f.read().splitlines()
     return targets
 
 
 setup(
     name="raymics",
-    version="0.7.2",
+    version="0.7.3",
     description="Raymics Tools",
     install_requires=get_install_requires(),
     packages=["raymics"],
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown'
 )
```

