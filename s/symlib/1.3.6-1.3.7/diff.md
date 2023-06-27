# Comparing `tmp/symlib-1.3.6.tar.gz` & `tmp/symlib-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.6.tar", last modified: Fri Jun 23 23:11:25 2023, max compression
+gzip compressed data, was "symlib-1.3.7.tar", last modified: Tue Jun 27 17:16:38 2023, max compression
```

## Comparing `symlib-1.3.6.tar` & `symlib-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.623422 symlib-1.3.6/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.6/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-23 23:11:25.623304 symlib-1.3.6/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.6/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.6/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-23 23:11:25.623457 symlib-1.3.6/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-23 23:11:21.000000 symlib-1.3.6/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.622436 symlib-1.3.6/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.6/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.6/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    53792 2023-06-23 23:11:21.000000 symlib-1.3.6/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.6/symlib/match.py
--rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.6/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.6/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.623159 symlib-1.3.6/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.680738 symlib-1.3.7/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.7/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-27 17:16:38.680622 symlib-1.3.7/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.7/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.7/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-27 17:16:38.680773 symlib-1.3.7/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-27 17:16:32.000000 symlib-1.3.7/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.679675 symlib-1.3.7/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.7/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.7/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53792 2023-06-23 23:11:21.000000 symlib-1.3.7/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.7/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)    36177 2023-06-27 17:16:14.000000 symlib-1.3.7/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.7/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.680472 symlib-1.3.7/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.6/LICENSE` & `symlib-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/PKG-INFO` & `symlib-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.6
+Version: 1.3.7
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.6/setup.py` & `symlib-1.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.6"
+version = "1.3.7"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.6/symlib/__init__.py` & `symlib-1.3.7/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/symlib/file_management.py` & `symlib-1.3.7/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/symlib/lib.py` & `symlib-1.3.7/symlib/lib.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/symlib/match.py` & `symlib-1.3.7/symlib/match.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/symlib/star_tagging.py` & `symlib-1.3.7/symlib/star_tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
 
 def tag_stars(sim_dir, galaxy_halo_model, star_snap=None, E_snap=None,
               target_subs=None):
     # Basic simulation information
     param = lib.simulation_parameters(sim_dir)
     h, hist = lib.read_subhalos(sim_dir)
     h_cmov, _ = lib.read_subhalos(sim_dir, comoving=True)
-    c = lib.read_cores(sim_dir)
+    #c = lib.read_cores(sim_dir)
     scale = lib.scale_factors(sim_dir)
 
     if target_subs is None:
         # Don't read in the host: wouldn't make sense.
         target_subs = np.arange(1, len(h), dtype=int)
 
     if 0 in target_subs:
```

### Comparing `symlib-1.3.6/symlib/util.py` & `symlib-1.3.7/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.6/symlib.egg-info/PKG-INFO` & `symlib-1.3.7/symlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.6
+Version: 1.3.7
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

