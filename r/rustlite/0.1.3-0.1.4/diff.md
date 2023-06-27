# Comparing `tmp/rustlite-0.1.3.tar.gz` & `tmp/rustlite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustlite-0.1.3.tar", last modified: Tue Jun 27 08:09:26 2023, max compression
+gzip compressed data, was "rustlite-0.1.4.tar", last modified: Tue Jun 27 08:18:44 2023, max compression
```

## Comparing `rustlite-0.1.3.tar` & `rustlite-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.228732 rustlite-0.1.3/
--rw-rw-rw-   0        0        0      978 2023-06-27 08:09:26.228732 rustlite-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-27 08:07:58.000000 rustlite-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.217840 rustlite-0.1.3/rustlite/
--rw-rw-rw-   0        0        0       58 2023-06-26 20:35:57.000000 rustlite-0.1.3/rustlite/__init__.py
--rw-rw-rw-   0        0        0     3183 2023-06-27 07:37:24.000000 rustlite-0.1.3/rustlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.227733 rustlite-0.1.3/rustlite.egg-info/
--rw-rw-rw-   0        0        0      978 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 08:09:26.229970 rustlite-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-06-27 08:09:22.000000 rustlite-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.158654 rustlite-0.1.4/
+-rw-rw-rw-   0        0        0      978 2023-06-27 08:18:44.158069 rustlite-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-27 08:07:58.000000 rustlite-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.144532 rustlite-0.1.4/rustlite/
+-rw-rw-rw-   0        0        0       58 2023-06-26 20:35:57.000000 rustlite-0.1.4/rustlite/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-06-27 08:15:30.000000 rustlite-0.1.4/rustlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:18:44.156055 rustlite-0.1.4/rustlite.egg-info/
+-rw-rw-rw-   0        0        0      978 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 08:18:44.000000 rustlite-0.1.4/rustlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:18:44.159161 rustlite-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-06-27 08:18:21.000000 rustlite-0.1.4/setup.py
```

### Comparing `rustlite-0.1.3/PKG-INFO` & `rustlite-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlite
-Version: 0.1.3
+Version: 0.1.4
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `rustlite-0.1.3/rustlite/enumerable.py` & `rustlite-0.1.4/rustlite/enumerable.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,18 +58,24 @@
     
     def concat(self, other: Iterable[T]) -> Iter[T]:
         return Iter(itertools.chain(self, other))
     
     def count(self) -> int:
         return sum(1 for _ in self)
     
+    def group_by(self, key: Callable[[T], R]) -> tuple[R, Iter[T]]:
+        return itertools.groupby(self, key)
+    
+    def pairwise(self) -> Iter[tuple[T, T]]:
+        return itertools.pairwise(self)
+
     def to_list(self) -> SList[T]:
-        return SList(self._iter)
+        return SList(self)
     def to_dict(self) -> SDict[T]:
-        return dict(self._iter)
+        return dict(self)
     def to_collection(self) -> IterCollection:
         return IterCollection(self.to_list())
     def collect(self, call: Callable[[Iterable], R]) -> R:
         return call(self)
 
 class SList(list[T], Iter[T]):
     """
```

### Comparing `rustlite-0.1.3/rustlite.egg-info/PKG-INFO` & `rustlite-0.1.4/rustlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlite
-Version: 0.1.3
+Version: 0.1.4
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `rustlite-0.1.3/setup.py` & `rustlite-0.1.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='rustlite',
-    version='0.1.3',    
+    version='0.1.4',    
     description='rust like iterators for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/peturparkur/python-rustlite',
     author='Peter Nagymathe',
     author_email='peter@nagymathe.xyz',
     license='AGPLv3+',
```

