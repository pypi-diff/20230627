# Comparing `tmp/wise-pizza-0.1.8.tar.gz` & `tmp/wise-pizza-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.8.tar", last modified: Tue Jun 27 13:35:02 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.9.tar", last modified: Tue Jun 27 13:41:34 2023, max compression
```

## Comparing `wise-pizza-0.1.8.tar` & `wise-pizza-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.643746 wise-pizza-0.1.8/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:35:02.643522 wise-pizza-0.1.8/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-27 13:35:02.643807 wise-pizza-0.1.8/setup.cfg
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1185 2023-06-27 13:33:55.000000 wise-pizza-0.1.8/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.634882 wise-pizza-0.1.8/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4745 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-27 13:33:37.000000 wise-pizza-0.1.8/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:35:02.643173 wise-pizza-0.1.8/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-27 13:35:02.000000 wise-pizza-0.1.8/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.163817 wise-pizza-0.1.9/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:41:34.163297 wise-pizza-0.1.9/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/README.md
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-27 13:41:34.163955 wise-pizza-0.1.9/setup.cfg
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-27 13:41:09.000000 wise-pizza-0.1.9/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.133784 wise-pizza-0.1.9/tests/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7047 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/tests/test_fit.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.140942 wise-pizza-0.1.9/wise_pizza/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/explain.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/find_alpha.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4745 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/make_matrix.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/plotting.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/segment_data.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/slicer.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/solver.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.162560 wise-pizza-0.1.9/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      436 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.8/LICENSE` & `wise-pizza-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/PKG-INFO` & `wise-pizza-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.8/README.md` & `wise-pizza-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/setup.py` & `wise-pizza-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from setuptools import find_packages, setup
 
-
-def _read_requirements_file(path: str):
-    with open(path) as f:
-        return list(map(
-            lambda req: req.strip(),
-            f.readlines(),
-        ))
-
-
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.8",
+    version="0.1.9",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    install_requires=_read_requirements_file('requirements.txt'),
+    install_requires=[
+        "ipython",
+        "kaleido",
+        "numpy",
+        "pandas",
+        "pytest",
+        "plotly",
+        "scikit_learn",
+        "scipy>=1.8.0",
+        "tqdm",
+        "cloudpickle",
+        "pivottablejs"
+    ],
     extras_require={
-        "test": _read_requirements_file('requirements-dev.txt'),
+        "test": [
+            "flake8",
+            "pytest",
+            "pytest-cov"
+        ],
     },
     packages=find_packages(
         include=[
             'wise_pizza',
             'wise_pizza.*'
         ],
         exclude=['tests*'],
```

### Comparing `wise-pizza-0.1.8/wise_pizza/explain.py` & `wise-pizza-0.1.9/wise_pizza/explain.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/find_alpha.py` & `wise-pizza-0.1.9/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/make_matrix.py` & `wise-pizza-0.1.9/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/plotting.py` & `wise-pizza-0.1.9/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/segment_data.py` & `wise-pizza-0.1.9/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/slicer.py` & `wise-pizza-0.1.9/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/solver.py` & `wise-pizza-0.1.9/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza/utils.py` & `wise-pizza-0.1.9/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.8/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.9/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

