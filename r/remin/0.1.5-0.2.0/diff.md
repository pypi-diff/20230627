# Comparing `tmp/remin-0.1.5.tar.gz` & `tmp/remin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.1.5.tar", last modified: Thu Jun 22 12:04:26 2023, max compression
+gzip compressed data, was "remin-0.2.0.tar", last modified: Tue Jun 27 19:12:03 2023, max compression
```

## Comparing `remin-0.1.5.tar` & `remin-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1854 2023-06-22 11:31:23.000000 remin-0.1.5/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.1.5/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.1.5/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-22 12:04:26.274546 remin-0.1.5/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.1.5/README.md
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.270545 remin-0.1.5/examples/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/examples/heat/
--rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.1.5/examples/heat/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.1.5/examples/heat/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1515 2023-05-06 19:07:30.000000 remin-0.1.5/examples/heat/training.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/examples/schrodinger/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1918 2023-06-22 11:46:30.000000 remin-0.1.5/examples/schrodinger/functrain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      373 2023-06-22 11:37:25.000000 remin-0.1.5/examples/schrodinger/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      834 2023-06-22 11:39:25.000000 remin-0.1.5/examples/schrodinger/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1912 2023-06-22 11:40:09.000000 remin-0.1.5/examples/schrodinger/train.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/examples/wave/
--rw-rw-r--   0 salih     (1000) salih     (1000)      562 2023-06-22 11:54:24.000000 remin-0.1.5/examples/wave/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1605 2023-06-22 11:54:24.000000 remin-0.1.5/examples/wave/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     2100 2023-06-22 11:54:24.000000 remin-0.1.5/examples/wave/train.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     2144 2023-06-22 11:54:24.000000 remin-0.1.5/examples/wave/train_batched.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-06-22 12:01:57.000000 remin-0.1.5/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.1.5/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-06-22 12:04:26.274546 remin-0.1.5/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.270545 remin-0.1.5/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-06-22 12:01:41.000000 remin-0.1.5/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     5795 2023-05-23 18:09:37.000000 remin-0.1.5/src/remin/callbacks.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     7307 2023-06-22 12:01:19.000000 remin-0.1.5/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1045 2023-05-11 10:55:40.000000 remin-0.1.5/src/remin/func.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     5286 2023-06-22 10:30:58.000000 remin-0.1.5/src/remin/residual.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/src/remin/solver/
--rw-rw-r--   0 salih     (1000) salih     (1000)      117 2023-05-08 21:15:07.000000 remin-0.1.5/src/remin/solver/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1794 2023-05-11 14:29:44.000000 remin-0.1.5/src/remin/solver/residual_loss.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     3456 2023-05-23 18:12:53.000000 remin-0.1.5/src/remin/solver/solver.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     3475 2023-05-11 14:29:36.000000 remin-0.1.5/src/remin/solver/trainer.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-22 12:04:26.274546 remin-0.1.5/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-22 12:04:26.000000 remin-0.1.5/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      770 2023-06-22 12:04:26.000000 remin-0.1.5/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-06-22 12:04:26.000000 remin-0.1.5/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-06-22 12:04:26.000000 remin-0.1.5/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-06-22 12:04:26.000000 remin-0.1.5/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1854 2023-06-22 11:31:23.000000 remin-0.2.0/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.2.0/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.2.0/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-27 19:12:03.071271 remin-0.2.0/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.2.0/README.md
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/heat/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.2.0/examples/heat/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.2.0/examples/heat/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1515 2023-05-06 19:07:30.000000 remin-0.2.0/examples/heat/training.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/schrodinger/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1918 2023-06-22 11:46:30.000000 remin-0.2.0/examples/schrodinger/functrain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      373 2023-06-22 11:37:25.000000 remin-0.2.0/examples/schrodinger/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      834 2023-06-22 11:39:25.000000 remin-0.2.0/examples/schrodinger/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1912 2023-06-22 11:40:09.000000 remin-0.2.0/examples/schrodinger/train.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/wave/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      562 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1605 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2100 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/train.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2144 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/train_batched.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1295 2023-06-27 15:23:02.000000 remin-0.2.0/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.2.0/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-06-27 19:12:03.071271 remin-0.2.0/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     7272 2023-06-27 15:22:50.000000 remin-0.2.0/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     5795 2023-05-23 18:09:37.000000 remin-0.2.0/src/remin/callbacks.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     7307 2023-06-22 12:01:19.000000 remin-0.2.0/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1045 2023-05-11 10:55:40.000000 remin-0.2.0/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     5286 2023-06-22 10:30:58.000000 remin-0.2.0/src/remin/residual.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin/solver/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      117 2023-05-08 21:15:07.000000 remin-0.2.0/src/remin/solver/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1794 2023-05-11 14:29:44.000000 remin-0.2.0/src/remin/solver/residual_loss.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3456 2023-05-23 18:12:53.000000 remin-0.2.0/src/remin/solver/solver.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3475 2023-05-11 14:29:36.000000 remin-0.2.0/src/remin/solver/trainer.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      806 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       37 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/entry_points.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.1.5/.gitignore` & `remin-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/LICENSE` & `remin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/PKG-INFO` & `remin-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.1.5
+Version: 0.2.0
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `remin-0.1.5/README.md` & `remin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/heat/model.py` & `remin-0.2.0/examples/heat/model.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/heat/postprocess.py` & `remin-0.2.0/examples/heat/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/heat/training.py` & `remin-0.2.0/examples/heat/training.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/schrodinger/functrain.py` & `remin-0.2.0/examples/schrodinger/functrain.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/schrodinger/postprocess.py` & `remin-0.2.0/examples/schrodinger/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/schrodinger/train.py` & `remin-0.2.0/examples/schrodinger/train.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/wave/model.py` & `remin-0.2.0/examples/wave/model.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/wave/postprocess.py` & `remin-0.2.0/examples/wave/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/wave/train.py` & `remin-0.2.0/examples/wave/train.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/examples/wave/train_batched.py` & `remin-0.2.0/examples/wave/train_batched.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/pyproject.toml` & `remin-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -25,14 +25,17 @@
     "numpy",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SalihTasdelen/remin"
 "Bug Tracker" = "https://github.com/SalihTasdelen/remin/issues"
 
+[project.scripts]
+remin = "remin:main"
+
 [project.optional-dependencies]
 dev = [
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
     "yapf ~=0.32.0",
 ]
```

### Comparing `remin-0.1.5/src/remin/callbacks.py` & `remin-0.2.0/src/remin/callbacks.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/domain.py` & `remin-0.2.0/src/remin/domain.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/func.py` & `remin-0.2.0/src/remin/func.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/residual.py` & `remin-0.2.0/src/remin/residual.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/solver/residual_loss.py` & `remin-0.2.0/src/remin/solver/residual_loss.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/solver/solver.py` & `remin-0.2.0/src/remin/solver/solver.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin/solver/trainer.py` & `remin-0.2.0/src/remin/solver/trainer.py`

 * *Files identical despite different names*

### Comparing `remin-0.1.5/src/remin.egg-info/PKG-INFO` & `remin-0.2.0/src/remin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.1.5
+Version: 0.2.0
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `remin-0.1.5/src/remin.egg-info/SOURCES.txt` & `remin-0.2.0/src/remin.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 src/remin/callbacks.py
 src/remin/domain.py
 src/remin/func.py
 src/remin/residual.py
 src/remin.egg-info/PKG-INFO
 src/remin.egg-info/SOURCES.txt
 src/remin.egg-info/dependency_links.txt
+src/remin.egg-info/entry_points.txt
 src/remin.egg-info/requires.txt
 src/remin.egg-info/top_level.txt
 src/remin/solver/__init__.py
 src/remin/solver/residual_loss.py
 src/remin/solver/solver.py
 src/remin/solver/trainer.py
```

