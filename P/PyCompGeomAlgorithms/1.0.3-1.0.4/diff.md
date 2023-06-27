# Comparing `tmp/PyCompGeomAlgorithms-1.0.3.tar.gz` & `tmp/PyCompGeomAlgorithms-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCompGeomAlgorithms-1.0.3.tar", last modified: Thu Jun 22 19:31:24 2023, max compression
+gzip compressed data, was "PyCompGeomAlgorithms-1.0.4.tar", last modified: Tue Jun 27 08:37:52 2023, max compression
```

## Comparing `PyCompGeomAlgorithms-1.0.3.tar` & `PyCompGeomAlgorithms-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.565957 PyCompGeomAlgorithms-1.0.3/
--rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      480 2023-06-22 19:31:24.563928 PyCompGeomAlgorithms-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.499572 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:54:06.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/__init__.py
--rw-rw-rw-   0        0        0    11303 2023-06-22 11:18:29.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/core.py
--rw-rw-rw-   0        0        0     1707 2023-06-22 10:26:23.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/graham.py
--rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/jarvis.py
--rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/kd_tree.py
--rw-rw-rw-   0        0        0     2762 2023-06-22 10:31:47.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/preparata.py
--rw-rw-rw-   0        0        0     2315 2023-06-22 11:31:48.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/quickhull.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.527246 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 19:31:24.565957 PyCompGeomAlgorithms-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-22 19:26:25.000000 PyCompGeomAlgorithms-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.531329 PyCompGeomAlgorithms-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 PyCompGeomAlgorithms-1.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.559852 PyCompGeomAlgorithms-1.0.3/tests/algorithms/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1866 2023-06-22 11:34:41.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_entities.py
--rw-rw-rw-   0        0        0     4056 2023-06-22 10:37:10.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_graham.py
--rw-rw-rw-   0        0        0      603 2023-06-22 10:37:22.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_jarvis.py
--rw-rw-rw-   0        0        0     2521 2023-06-22 10:37:32.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_kd_tree.py
--rw-rw-rw-   0        0        0     3420 2023-06-22 10:37:48.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_preparata.py
--rw-rw-rw-   0        0        0     3128 2023-06-22 11:31:06.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.349270 PyCompGeomAlgorithms-1.0.4/
+-rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      480 2023-06-27 08:37:52.346269 PyCompGeomAlgorithms-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.264270 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:54:06.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/__init__.py
+-rw-rw-rw-   0        0        0    11303 2023-06-27 08:22:07.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/core.py
+-rw-rw-rw-   0        0        0     1918 2023-06-27 08:27:25.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/graham.py
+-rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/jarvis.py
+-rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/kd_tree.py
+-rw-rw-rw-   0        0        0     2762 2023-06-27 08:36:35.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/preparata.py
+-rw-rw-rw-   0        0        0     2359 2023-06-27 08:34:18.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/quickhull.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.304268 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-27 08:37:52.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-06-27 08:37:52.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:37:52.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 08:37:52.000000 PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.4/README.md
+-rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 PyCompGeomAlgorithms-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:37:52.352268 PyCompGeomAlgorithms-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-27 08:36:47.000000 PyCompGeomAlgorithms-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.307268 PyCompGeomAlgorithms-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 PyCompGeomAlgorithms-1.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.335268 PyCompGeomAlgorithms-1.0.4/tests/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4573 2023-06-27 08:07:17.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_graham.py
+-rw-rw-rw-   0        0        0      605 2023-06-26 14:33:11.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_jarvis.py
+-rw-rw-rw-   0        0        0     2521 2023-06-27 08:19:04.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_kd_tree.py
+-rw-rw-rw-   0        0        0     3424 2023-06-27 08:19:50.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_preparata.py
+-rw-rw-rw-   0        0        0     3304 2023-06-27 08:34:51.000000 PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:37:52.341269 PyCompGeomAlgorithms-1.0.4/tests/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:32:45.000000 PyCompGeomAlgorithms-1.0.4/tests/entities/__init__.py
+-rw-rw-rw-   0        0        0     1866 2023-06-26 14:32:52.000000 PyCompGeomAlgorithms-1.0.4/tests/entities/test_entities.py
```

### Comparing `PyCompGeomAlgorithms-1.0.3/LICENSE` & `PyCompGeomAlgorithms-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/core.py` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/core.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/jarvis.py` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/jarvis.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/kd_tree.py` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/kd_tree.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/preparata.py` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/preparata.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/quickhull.py` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms/quickhull.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,20 @@
 
     hull = (
         partition(subset1, leftmost_point, rightmost_point, tree.root.left) +
         partition(subset2, rightmost_point, leftmost_point, tree.root.right)[1:-1]
     )
     tree.root.subhull = hull
 
-    yield leftmost_point, rightmost_point, subset1, subset2, tree
+    yield leftmost_point, rightmost_point, subset1, subset2
     yield tree
+    yield tree
+    yield tree
+    yield tree
+
     yield hull
 
 
 def partition(points, left, right, node):
     if len(points) == 2:
         node.subhull = [left, right]
         return node.subhull
```

### Comparing `PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/SOURCES.txt` & `PyCompGeomAlgorithms-1.0.4/PyCompGeomAlgorithms.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 PyCompGeomAlgorithms/__init__.py
 PyCompGeomAlgorithms/core.py
 PyCompGeomAlgorithms/graham.py
 PyCompGeomAlgorithms/jarvis.py
 PyCompGeomAlgorithms/kd_tree.py
 PyCompGeomAlgorithms/preparata.py
 PyCompGeomAlgorithms/quickhull.py
 PyCompGeomAlgorithms.egg-info/PKG-INFO
 PyCompGeomAlgorithms.egg-info/SOURCES.txt
 PyCompGeomAlgorithms.egg-info/dependency_links.txt
 PyCompGeomAlgorithms.egg-info/top_level.txt
 tests/__init__.py
 tests/algorithms/__init__.py
-tests/algorithms/test_entities.py
 tests/algorithms/test_graham.py
 tests/algorithms/test_jarvis.py
 tests/algorithms/test_kd_tree.py
 tests/algorithms/test_preparata.py
-tests/algorithms/test_quickhull.py
+tests/algorithms/test_quickhull.py
+tests/entities/__init__.py
+tests/entities/test_entities.py
```

### Comparing `PyCompGeomAlgorithms-1.0.3/README.md` & `PyCompGeomAlgorithms-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/setup.py` & `PyCompGeomAlgorithms-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="PyCompGeomAlgorithms",
-    version="1.0.3",
+    version="1.0.4",
     author="artandfi (Artem Fisunenko)",
     author_email="artyom.fisunenko@gmail.com",
     description="An implementation of computational geometry algorithms in Python3.",
     packages=find_packages(),
     keywords=[
         "Python3",
         "computational geometry",
```

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_entities.py` & `PyCompGeomAlgorithms-1.0.4/tests/entities/test_entities.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_graham.py` & `PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_graham.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,36 @@
 
 
 def test_graham1():
     pts = [Point(7, 0), Point(3, 3), Point(0, 0)]
     centroid = Point(3.3333333333333335, 1.0)
     ordered = [Point(7, 0), Point(3, 3), Point(0, 0)]
     origin = Point(7, 0)
-    steps = [
-        ([ordered[0], ordered[1], ordered[2]], True),
-        ([ordered[1], ordered[2], ordered[0]], True)
+    triples = [
+        (ordered[0], ordered[1], ordered[2]),
+        (ordered[1], ordered[2], ordered[0])
     ]
+    are_angles_less_than_pi = [True, True]
     hull = [Point(7, 0), Point(3, 3), Point(0, 0)]
     
     ans = graham(pts)
     assert next(ans) == centroid
     assert next(ans) == ordered
     assert next(ans) == origin
-    assert next(ans) == steps
+    
+    assert next(ans) == triples
+    assert next(ans) == are_angles_less_than_pi
+
+    assert next(ans) is None
+    assert next(ans) is None
+    assert next(ans) is None
+    
     assert next(ans) == hull
 
+
 def test_graham2():
     pts = [
         Point(3, 10),
         Point(6, 8),
         Point(3, 5),
         Point(2, 8),
         Point(4, 8),
@@ -46,46 +55,55 @@
         Point(3, 10),
         Point(2, 8),
         Point(0, 0),
         Point(3, 5),
         Point(3, 3),
     ]
     origin = Point(5, 0)
-    steps = [
-        ([ordered[0], ordered[1], ordered[2]], False),
-        ([ordered[0], ordered[2], ordered[3]], True),
-        ([ordered[2], ordered[3], ordered[4]], True),
-        ([ordered[3], ordered[4], ordered[5]], True),
-        ([ordered[4], ordered[5], ordered[6]], False),
-        ([ordered[3], ordered[4], ordered[6]], True),
-        ([ordered[4], ordered[6], ordered[7]], True),
-        ([ordered[6], ordered[7], ordered[8]], True),
-        ([ordered[7], ordered[8], ordered[9]], True),
-        ([ordered[8], ordered[9], ordered[10]], False),
-        ([ordered[7], ordered[8], ordered[10]], True),
-        ([ordered[8], ordered[10], ordered[0]], False),
-        ([ordered[7], ordered[8], ordered[0]], True)
+    triples = [
+        (ordered[0], ordered[1], ordered[2]),
+        (ordered[0], ordered[2], ordered[3]),
+        (ordered[2], ordered[3], ordered[4]),
+        (ordered[3], ordered[4], ordered[5]),
+        (ordered[4], ordered[5], ordered[6]),
+        (ordered[3], ordered[4], ordered[6]),
+        (ordered[4], ordered[6], ordered[7]),
+        (ordered[6], ordered[7], ordered[8]),
+        (ordered[7], ordered[8], ordered[9]),
+        (ordered[8], ordered[9], ordered[10]),
+        (ordered[7], ordered[8], ordered[10]),
+        (ordered[8], ordered[10], ordered[0]),
+        (ordered[7], ordered[8], ordered[0])
     ]
+    are_angles_less_than_pi = [False, True, True, True, False, True, True, True, True, False, True, False, True]
     hull = [
         Point(5, 0),
         Point(10, 3),
         Point(7, 7),
         Point(6, 8),
         Point(3, 10),
         Point(2, 8),
         Point(0, 0)
     ]
     
     ans = graham(pts)
     assert next(ans) == centroid
     assert next(ans) == ordered
     assert next(ans) == origin
-    assert next(ans) == steps
+    
+    assert next(ans) == triples
+    assert next(ans) == are_angles_less_than_pi
+
+    assert next(ans) is None
+    assert next(ans) is None
+    assert next(ans) is None
+    
     assert next(ans) == hull
 
+
 def test_graham3():
     pts = [
         Point(2, 8),
         Point(5, 6),
         Point(7, 8),
         Point(8, 11),
         Point(7, 5),
@@ -105,36 +123,44 @@
         Point(8, 11),
         Point(2, 8),
         Point(1, 3),
         Point(5, 2),
         Point(5, 6)
     ]
     origin = Point(8, 2)
-    steps = [
-        ([ordered[0], ordered[1], ordered[2]], False),
-        ([ordered[0], ordered[2], ordered[3]], True),
-        ([ordered[2], ordered[3], ordered[4]], True),
-        ([ordered[3], ordered[4], ordered[5]], False),
-        ([ordered[2], ordered[3], ordered[5]], False),
-        ([ordered[0], ordered[2], ordered[5]], True),
-        ([ordered[2], ordered[5], ordered[6]], True),
-        ([ordered[5], ordered[6], ordered[7]], True),
-        ([ordered[6], ordered[7], ordered[8]], True),
-        ([ordered[7], ordered[8], ordered[9]], True),
-        ([ordered[8], ordered[9], ordered[0]], False),
-        ([ordered[7], ordered[8], ordered[0]], True)
+    triples = [
+        (ordered[0], ordered[1], ordered[2]),
+        (ordered[0], ordered[2], ordered[3]),
+        (ordered[2], ordered[3], ordered[4]),
+        (ordered[3], ordered[4], ordered[5]),
+        (ordered[2], ordered[3], ordered[5]),
+        (ordered[0], ordered[2], ordered[5]),
+        (ordered[2], ordered[5], ordered[6]),
+        (ordered[5], ordered[6], ordered[7]),
+        (ordered[6], ordered[7], ordered[8]),
+        (ordered[7], ordered[8], ordered[9]),
+        (ordered[8], ordered[9], ordered[0]),
+        (ordered[7], ordered[8], ordered[0])
     ]
+    are_angles_less_than_pi = [False, True, True, False, False, True, True, True, True, True, False, True]
     hull = [
         Point(8, 2),
         Point(11, 5),
         Point(8, 11),
         Point(2, 8),
         Point(1, 3),
         Point(5, 2)
     ]
     
     ans = graham(pts)
     assert next(ans) == centroid
     assert next(ans) == ordered
     assert next(ans) == origin
-    assert next(ans) == steps
+    
+    assert next(ans) == triples
+    assert next(ans) == are_angles_less_than_pi
+
+    assert next(ans) is None
+    assert next(ans) is None
+    assert next(ans) is None
+    
     assert next(ans) == hull
```

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_jarvis.py` & `PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_jarvis.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,13 +14,14 @@
         Point(9, 6),
     ]
     hull = [Point(0, 0), Point(1, 4), Point(9, 6), Point(7, 0)]
 
     ans = jarvis(pts)
     assert ans == hull
 
+
 def test_jarvis2():
     pts = [Point(3, 3), Point(1, 1), Point(5, 0)]
     hull = [Point(1, 1), Point(3, 3), Point(5, 0)]
 
     ans = jarvis(pts)
     assert ans == hull
```

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_kd_tree.py` & `PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_kd_tree.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_preparata.py` & `PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_preparata.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == (left_paths, right_paths)
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
+
 def test_preparata2():
     # Corner case for convex (>--X) where one of the angles is equal to pi
     points = [Point(2, 2), Point(0, 1), Point(4, 3), Point(1, 0)]
     hull0 = [Point(0, 1), Point(2, 2), Point(1, 0)]
     hull = [Point(0, 1), Point(4, 3), Point(1, 0)]
     tree0 = ThreadedBinTree.from_iterable(hull0)
     left_paths = [[Point(2, 2), Point(1, 0)]]
@@ -55,14 +56,15 @@
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == (left_paths, right_paths)
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
+
 def test_preparata4():
     # Corner cases for collinear first points and left and right supporting where one of the angles is 0
     points = [Point(1, 1), Point(1, 5), Point(5, 3), Point(1, 11), Point(6, 1), Point(10, 1)]
     hull0 = [Point(1, 1), Point(1, 5), Point(5, 3)]
     hull = [Point(1, 1), Point(1, 11), Point(10, 1)]
     tree0 = ThreadedBinTree.from_iterable(hull0)
     left_paths = [
```

### Comparing `PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_quickhull.py` & `PyCompGeomAlgorithms-1.0.4/tests/algorithms/test_quickhull.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,22 @@
     tree = BinTree(QuickhullNode([pts[1], pts[0], pts[2]], subhull=hull))
     tree.root.left = QuickhullNode([pts[1], pts[0], pts[2]], h=pts[0], subhull=hull)
     tree.root.right = QuickhullNode([pts[2], pts[1]], subhull=[pts[2], pts[1]])
     tree.root.left.left = QuickhullNode([pts[1], pts[0]], subhull=[pts[1], pts[0]])
     tree.root.left.right = QuickhullNode([pts[0], pts[2]], subhull=[pts[0], pts[2]])
 
     ans = quickhull(pts)
-    lp, rp, s1, s2, _ = next(ans)
+    lp, rp, s1, s2 = next(ans)
     
     assert (lp, rp) == (pts[1], pts[2])
     assert (s1, s2) == ([pts[1], pts[0], pts[2]], [pts[2], pts[1]])
     assert next(ans) == tree
+    assert next(ans) == tree
+    assert next(ans) == tree
+    assert next(ans) == tree
     assert next(ans) == hull
 
 
 def test_quickhull2():
     pts = [
         Point(0, 6),
         Point(8, 11),
@@ -78,13 +81,16 @@
         h=pts[5],
         subhull=[pts[7], pts[5], pts[0]]
     )
     tree.root.right.right.left = QuickhullNode([pts[7], pts[5]], subhull=[pts[7], pts[5]])
     tree.root.right.right.right = QuickhullNode([pts[5], pts[0]], subhull=[pts[5], pts[0]])
 
     ans = quickhull(pts)
-    lp, rp, s1, s2, _ = next(ans)
+    lp, rp, s1, s2 = next(ans)
 
     assert (lp, rp) == (pts[0], pts[8])
     assert (s1, s2) == (tree.root.left.points, tree.root.right.points)
     assert next(ans) == tree
-    assert next(ans) == hull
+    assert next(ans) == tree
+    assert next(ans) == tree
+    assert next(ans) == tree
+    assert next(ans) == hull
```

