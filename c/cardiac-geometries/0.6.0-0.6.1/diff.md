# Comparing `tmp/cardiac_geometries-0.6.0.tar.gz` & `tmp/cardiac_geometries-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.6.0.tar", last modified: Fri Jun 23 11:48:42 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.6.1.tar", last modified: Tue Jun 27 08:40:01 2023, max compression
```

## Comparing `cardiac_geometries-0.6.0.tar` & `cardiac_geometries-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-23 11:48:42.703637 cardiac_geometries-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.695637 cardiac_geometries-0.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      602 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12783 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    21343 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    19764 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    16423 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9979 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:48:32.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      560 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.162262 cardiac_geometries-0.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      602 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    21343 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    19764 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:39:49.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.6.0/LICENSE` & `cardiac_geometries-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/PKG-INFO` & `cardiac_geometries-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.6.0/setup.cfg` & `cardiac_geometries-0.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.6.0
+version = 0.6.1
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
```

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_slab.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_mesh.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,18 +399,17 @@
                     raise RuntimeError("Cannot write object with empty path")
 
                 dict_to_h5(obj, path, p.h5group, comm=self.comm)
 
         if schema_path is None:
             schema_path = path.with_suffix(".json")
         logger.debug(f"Save schema {schema_path}")
-        # dolfin.MPI.barrier(self.comm)
-        print(self.comm.rank, schema_path, self.schema)
+
         dump_schema(schema_path, schema=self.schema)
-        # dolfin.MPI.barrier(self.comm)
+        dolfin.MPI.barrier(self.comm)
         logger.debug(f"Geometry saved to path {path} and schema to {schema_path}")
 
     @classmethod
     def from_file(
         cls,
         fname: Union[str, Path],
         schema_path: Optional[Union[str, Path]] = None,
```

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.6.1/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac-geometries
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.0/tests/test_cli.py` & `cardiac_geometries-0.6.1/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 from pathlib import Path
 
-import pytest
 from cardiac_geometries import cli
 from cardiac_geometries.geometry import Geometry
 from click.testing import CliRunner
 
-try:
-    import dolfin
 
-    _size = dolfin.MPI.size(dolfin.MPI.comm_world)
-except ImportError:
-    _size = 0
-
-
-no_mpi = pytest.mark.skipif(_size > 1, reason="Only works in serial")
-
-
-@no_mpi
 def test_create_slab(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(cli.create_slab, ["--create-fibers", tmp_path.as_posix()])
     assert res1.exit_code == 0
     outfile = tmp_path / "geo.h5"
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
-@no_mpi
 def test_create_lv_ellipsoid(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_lv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
@@ -41,15 +28,14 @@
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
-@no_mpi
 def test_create_biv_ellipsoid(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_biv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
@@ -57,15 +43,14 @@
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
-@no_mpi
 def test_create_biv_ellipsoid_torso(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_biv_ellipsoid_torso,
         [tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
```

### Comparing `cardiac_geometries-0.6.0/tests/test_geometry.py` & `cardiac_geometries-0.6.1/tests/test_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 import dolfin
 import pytest
 from cardiac_geometries.geometry import Geometry
 from cardiac_geometries.geometry import H5Path
 from cardiac_geometries.geometry import load_schema
 
 
-no_mpi = pytest.mark.skipif(
-    dolfin.MPI.size(dolfin.MPI.comm_world) > 1,
-    reason="Only works in serial",
-)
-
-
 class ExampleData(NamedTuple):
     info: Dict[str, Any]
     mesh: dolfin.Mesh
     ffun: dolfin.MeshFunction
     f0: dolfin.Function
     info2: Dict[str, Any]
     mesh2: dolfin.Mesh
@@ -53,15 +47,14 @@
         info2=info2,
         mesh2=mesh2,
         ffun2=ffun2,
         f02=f02,
     )
 
 
-@no_mpi
 def test_load_invalid_schema(mpi_tmp_path):
     schema = {
         "mesh": dict(h5group="/mesh", is_mesh=True, invalid_key=42),
         "ffun": dict(h5group="/ffun", is_meshfunction=True, dim=2),
         "f0": dict(h5group="/f0", is_function=True),
     }
     path = mpi_tmp_path / "schema.json"
@@ -99,15 +92,14 @@
     assert new_geo.schema == geo.schema
     assert new_geo.info == geo.info
     assert (new_geo.mesh.coordinates() == geo.mesh.coordinates()).all()
     # assert (new_geo.ffun.array() == geo.ffun.array()).all()
     assert (new_geo.f0.vector().get_local() == geo.f0.vector().get_local()).all()
 
 
-@no_mpi
 def test_save_load_multiple_meshes(tmp_path, example_data):
     schema = {
         "info": H5Path(h5group="/group1/info", is_dolfin=False),
         "mesh": H5Path(h5group="/group1/mesh", is_mesh=True),
         "ffun": H5Path(
             h5group="/group1/ffun",
             is_meshfunction=True,
```

### Comparing `cardiac_geometries-0.6.0/tests/test_gmsh.py` & `cardiac_geometries-0.6.1/tests/test_gmsh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from pathlib import Path
 
 import pytest
 from cardiac_geometries import gmsh
 from cardiac_geometries import has_gmsh
 
-try:
-    import dolfin
-
-    _size = dolfin.MPI.size(dolfin.MPI.comm_world)
-except ImportError:
-    _size = 0
-
 
 require_gmsh = pytest.mark.skipif(
-    not has_gmsh() or _size > 1,
+    not has_gmsh(),
     reason="gmsh is required to run the test",
 )
 
 
 @require_gmsh
 @pytest.mark.gmsh
 def test_lv_prolate_flat_base():
```

