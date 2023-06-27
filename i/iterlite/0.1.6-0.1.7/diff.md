# Comparing `tmp/iterlite-0.1.6.tar.gz` & `tmp/iterlite-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterlite-0.1.6.tar", last modified: Tue Jun 27 16:54:09 2023, max compression
+gzip compressed data, was "iterlite-0.1.7.tar", last modified: Tue Jun 27 17:23:45 2023, max compression
```

## Comparing `iterlite-0.1.6.tar` & `iterlite-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:54:09.092599 iterlite-0.1.6/
--rw-rw-rw-   0        0        0     1968 2023-06-27 16:54:09.092599 iterlite-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-06-27 16:50:34.000000 iterlite-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 16:54:09.085501 iterlite-0.1.6/iterlite/
--rw-rw-rw-   0        0        0       58 2023-06-27 16:37:31.000000 iterlite-0.1.6/iterlite/__init__.py
--rw-rw-rw-   0        0        0     4114 2023-06-27 16:53:50.000000 iterlite-0.1.6/iterlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:54:09.091567 iterlite-0.1.6/iterlite.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-06-27 16:54:09.000000 iterlite-0.1.6/iterlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-27 16:54:09.000000 iterlite-0.1.6/iterlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:54:09.000000 iterlite-0.1.6/iterlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 16:54:09.000000 iterlite-0.1.6/iterlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 16:54:09.093607 iterlite-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-27 16:32:40.000000 iterlite-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:23:45.573618 iterlite-0.1.7/
+-rw-rw-rw-   0        0        0     1968 2023-06-27 17:23:45.573618 iterlite-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-06-27 16:54:51.000000 iterlite-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:23:45.555219 iterlite-0.1.7/iterlite/
+-rw-rw-rw-   0        0        0       58 2023-06-27 16:37:31.000000 iterlite-0.1.7/iterlite/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-06-27 17:22:57.000000 iterlite-0.1.7/iterlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:23:45.572450 iterlite-0.1.7/iterlite.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-06-27 17:23:45.000000 iterlite-0.1.7/iterlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-27 17:23:45.000000 iterlite-0.1.7/iterlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:23:45.000000 iterlite-0.1.7/iterlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 17:23:45.000000 iterlite-0.1.7/iterlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:23:45.573618 iterlite-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-27 17:23:02.000000 iterlite-0.1.7/setup.py
```

### Comparing `iterlite-0.1.6/PKG-INFO` & `iterlite-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.1.6
+Version: 0.1.7
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.1.6/README.md` & `iterlite-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `iterlite-0.1.6/iterlite/enumerable.py` & `iterlite-0.1.7/iterlite/enumerable.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,20 @@
     
     def nth(self, n: int) -> Optional[T]:
         return self.skip(n).first()
     
     def slice(self, start: int, end: int) -> Iter[T]:
         return self.skip(start).take(end - start)
     
+    def enumerate(self, start: int = 0) -> Iter[tuple[int, T]]:
+        return Iter(enumerate(self, start))
+
+    def batch(self, n: int) -> Iter[Iter[T]]:
+        return self.enumerate().group_by(lambda x: x[0] // n).map(lambda x: x[1])
+    
     def concat(self, other: Iterable[T]) -> Iter[T]:
         return Iter(itertools.chain(self, other))
     
     def count(self) -> int:
         return sum(1 for _ in self)
     
     def group_by(self, key: Callable[[T], R]) ->Iter[tuple[R, Iter[T]]]:
```

### Comparing `iterlite-0.1.6/iterlite.egg-info/PKG-INFO` & `iterlite-0.1.7/iterlite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterlite
-Version: 0.1.6
+Version: 0.1.7
 Summary: rust like iterators for python
 Home-page: https://github.com/peturparkur/python-rustlite
 Author: Peter Nagymathe
 Author-email: peter@nagymathe.xyz
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `iterlite-0.1.6/setup.py` & `iterlite-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='iterlite',
-    version='0.1.6',    
+    version='0.1.7',    
     description='rust like iterators for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/peturparkur/python-rustlite',
     author='Peter Nagymathe',
     author_email='peter@nagymathe.xyz',
     license='AGPLv3+',
```

