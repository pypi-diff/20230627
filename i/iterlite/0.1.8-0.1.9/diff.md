# Comparing `tmp/iterlite-0.1.8.tar.gz` & `tmp/iterlite-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterlite-0.1.8.tar", last modified: Tue Jun 27 17:58:00 2023, max compression
+gzip compressed data, was "iterlite-0.1.9.tar", last modified: Tue Jun 27 18:09:25 2023, max compression
```

## Comparing `iterlite-0.1.8.tar` & `iterlite-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:58:00.832235 iterlite-0.1.8/
--rw-rw-rw-   0        0        0     1968 2023-06-27 17:58:00.830753 iterlite-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-06-27 16:54:51.000000 iterlite-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 17:58:00.819237 iterlite-0.1.8/iterlite/
--rw-rw-rw-   0        0        0       58 2023-06-27 16:37:31.000000 iterlite-0.1.8/iterlite/__init__.py
--rw-rw-rw-   0        0        0     4363 2023-06-27 17:57:10.000000 iterlite-0.1.8/iterlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:58:00.829753 iterlite-0.1.8/iterlite.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-06-27 17:58:00.000000 iterlite-0.1.8/iterlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-27 17:58:00.000000 iterlite-0.1.8/iterlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:58:00.000000 iterlite-0.1.8/iterlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 17:58:00.000000 iterlite-0.1.8/iterlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 17:58:00.832743 iterlite-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-27 17:57:48.000000 iterlite-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:09:25.311889 iterlite-0.1.9/
+-rw-rw-rw-   0        0        0     1968 2023-06-27 18:09:25.311889 iterlite-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-06-27 16:54:51.000000 iterlite-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:09:25.287091 iterlite-0.1.9/iterlite/
+-rw-rw-rw-   0        0        0       58 2023-06-27 16:37:31.000000 iterlite-0.1.9/iterlite/__init__.py
+-rw-rw-rw-   0        0        0     4428 2023-06-27 18:09:03.000000 iterlite-0.1.9/iterlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:09:25.308868 iterlite-0.1.9/iterlite.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-06-27 18:09:25.000000 iterlite-0.1.9/iterlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-27 18:09:25.000000 iterlite-0.1.9/iterlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:09:25.000000 iterlite-0.1.9/iterlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 18:09:25.000000 iterlite-0.1.9/iterlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 18:09:25.313092 iterlite-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-27 18:09:07.000000 iterlite-0.1.9/setup.py
```

### Comparing `iterlite-0.1.8/PKG-INFO` & `iterlite-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.1.8
+Version: 0.1.9
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.1.8/README.md` & `iterlite-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `iterlite-0.1.8/iterlite/enumerable.py` & `iterlite-0.1.9/iterlite/enumerable.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,26 +60,28 @@
     
     def slice(self, start: int, end: int) -> Iter[T]:
         return self.skip(start).take(end - start)
     
     def enumerate(self, start: int = 0) -> Iter[tuple[int, T]]:
         return Iter(enumerate(self, start))
 
-    def batch(self, n: int) -> Iter[Iter[T]]:
-        return self.enumerate().group_by(lambda x: x[0] // n).map(lambda x: x[1])
+    def group_by(self, key: Callable[[T], R]) -> Iter[tuple[R, Iter[T]]]:
+        return Iter(itertools.groupby(self, key)).map(lambda x: (x[0], Iter(x[1])))
+
+    def batch(self, n: int):
+        return self.enumerate() \
+            .group_by(lambda x: x[0] // n) \
+            .map(lambda x: x[1].map(lambda y: y[1]))
     
     def concat(self, other: Iterable[T]) -> Iter[T]:
         return Iter(itertools.chain(self, other))
     
     def count(self) -> int:
         return sum(1 for _ in self)
     
-    def group_by(self, key: Callable[[T], R]) -> Iter[tuple[R, Iter[T]]]:
-        return Iter(itertools.groupby(self, key))
-    
     def pairwise(self) -> Iter[tuple[T, T]]:
         return Iter(itertools.pairwise(self))
 
     def to_list(self) -> SList[T]:
         return SList(self)
     def to_dict(self, f: Callable[[T], tuple[K, V]]) -> SDict[K, V]:
         return SDict[K, V](self.map(f))
```

### Comparing `iterlite-0.1.8/iterlite.egg-info/PKG-INFO` & `iterlite-0.1.9/iterlite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.1.8
+Version: 0.1.9
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.1.8/setup.py` & `iterlite-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='iterlite',
-    version='0.1.8',    
+    version='0.1.9',    
     description='rust like iterators for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/peturparkur/python-rustlite',
     author='Peter Nagymathe',
     author_email='peter@nagymathe.xyz',
     license='AGPLv3+',
```

