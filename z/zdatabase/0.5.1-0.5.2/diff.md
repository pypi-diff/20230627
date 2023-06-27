# Comparing `tmp/zdatabase-0.5.1.tar.gz` & `tmp/zdatabase-0.5.2.tar.gz`

## Comparing `zdatabase-0.5.1.tar` & `zdatabase-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/model.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.1/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.2/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.5.2/PKG-INFO
```

### Comparing `zdatabase-0.5.1/src/zdatabase/__init__.py` & `zdatabase-0.5.2/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.1/src/zdatabase/model.py` & `zdatabase-0.5.2/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.1/src/zdatabase/utility.py` & `zdatabase-0.5.2/src/zdatabase/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         page_size=100&page_num=1
         """
         page_num = int(params.get('page_num', '1'))
         page_size = int(params.get('page_size', '10'))
         pagination = query.paginate(page_num, per_page=page_size)  
         rst = {
             'items': [getattr(item, method)() for item in pagination.items],
-            'total': pagination.total
+            'total': pagination.total,
+            'pages': pagination.pages
         }
         return rst
 
 
 class MapperUtility:
     @staticmethod
     def jsonlize(items):
```

### Comparing `zdatabase-0.5.1/LICENSE` & `zdatabase-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.1/pyproject.toml` & `zdatabase-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.5.1/PKG-INFO` & `zdatabase-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.1
+Version: 0.5.2
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

