# Comparing `tmp/yi-foo-0.0.1.tar.gz` & `tmp/yi-foo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yi-foo-0.0.1.tar", last modified: Mon Jun 26 13:54:51 2023, max compression
+gzip compressed data, was "dist/yi-foo-0.0.2.tar", last modified: Tue Jun 27 13:33:05 2023, max compression
```

## Comparing `yi-foo-0.0.1.tar` & `yi-foo-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:54:51.960695 yi-foo-0.0.1/
--rw-rw-r--   0 ychen     (1001) ychen     (1001)    14228 2023-06-26 13:54:51.960695 yi-foo-0.0.1/PKG-INFO
--rw-rw-r--   0 ychen     (1001) ychen     (1001)    10608 2023-06-26 13:48:18.000000 yi-foo-0.0.1/README.md
-drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:54:51.960695 yi-foo-0.0.1/gestalt/
--rw-rw-r--   0 ychen     (1001) ychen     (1001)    25398 2023-06-26 13:48:18.000000 yi-foo-0.0.1/gestalt/__init__.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)      801 2023-06-26 13:48:18.000000 yi-foo-0.0.1/gestalt/provider.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)      561 2023-06-26 13:48:18.000000 yi-foo-0.0.1/gestalt/utils.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)     8218 2023-06-26 13:48:18.000000 yi-foo-0.0.1/gestalt/vault.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)      212 2023-06-26 13:54:51.960695 yi-foo-0.0.1/setup.cfg
--rw-rw-r--   0 ychen     (1001) ychen     (1001)     1239 2023-06-26 13:54:43.000000 yi-foo-0.0.1/setup.py
-drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:54:51.960695 yi-foo-0.0.1/tests/
--rw-rw-r--   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:48:18.000000 yi-foo-0.0.1/tests/__init__.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)     2432 2023-06-26 13:48:18.000000 yi-foo-0.0.1/tests/conftest.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)    17818 2023-06-26 13:48:18.000000 yi-foo-0.0.1/tests/test_gestalt.py
--rw-rw-r--   0 ychen     (1001) ychen     (1001)      921 2023-06-26 13:48:18.000000 yi-foo-0.0.1/tests/test_vault.py
-drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:54:51.960695 yi-foo-0.0.1/yi_foo.egg-info/
--rw-rw-r--   0 ychen     (1001) ychen     (1001)    14228 2023-06-26 13:54:51.000000 yi-foo-0.0.1/yi_foo.egg-info/PKG-INFO
--rw-rw-r--   0 ychen     (1001) ychen     (1001)      329 2023-06-26 13:54:51.000000 yi-foo-0.0.1/yi_foo.egg-info/SOURCES.txt
--rw-rw-r--   0 ychen     (1001) ychen     (1001)        1 2023-06-26 13:54:51.000000 yi-foo-0.0.1/yi_foo.egg-info/dependency_links.txt
--rw-rw-r--   0 ychen     (1001) ychen     (1001)       84 2023-06-26 13:54:51.000000 yi-foo-0.0.1/yi_foo.egg-info/requires.txt
--rw-rw-r--   0 ychen     (1001) ychen     (1001)       14 2023-06-26 13:54:51.000000 yi-foo-0.0.1/yi_foo.egg-info/top_level.txt
+drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-27 13:33:05.695760 yi-foo-0.0.2/
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)    14228 2023-06-27 13:33:05.695760 yi-foo-0.0.2/PKG-INFO
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)    10608 2023-06-26 13:48:18.000000 yi-foo-0.0.2/README.md
+drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-27 13:33:05.691760 yi-foo-0.0.2/gestalt/
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)    25398 2023-06-26 13:48:18.000000 yi-foo-0.0.2/gestalt/__init__.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)      801 2023-06-26 13:48:18.000000 yi-foo-0.0.2/gestalt/provider.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)      561 2023-06-26 13:48:18.000000 yi-foo-0.0.2/gestalt/utils.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)     8218 2023-06-26 13:48:18.000000 yi-foo-0.0.2/gestalt/vault.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)      212 2023-06-27 13:33:05.695760 yi-foo-0.0.2/setup.cfg
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)     1239 2023-06-27 13:32:18.000000 yi-foo-0.0.2/setup.py
+drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-27 13:33:05.691760 yi-foo-0.0.2/tests/
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)        0 2023-06-26 13:48:18.000000 yi-foo-0.0.2/tests/__init__.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)     2432 2023-06-26 13:48:18.000000 yi-foo-0.0.2/tests/conftest.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)    17818 2023-06-26 13:48:18.000000 yi-foo-0.0.2/tests/test_gestalt.py
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)      921 2023-06-26 13:48:18.000000 yi-foo-0.0.2/tests/test_vault.py
+drwxrwxr-x   0 ychen     (1001) ychen     (1001)        0 2023-06-27 13:33:05.695760 yi-foo-0.0.2/yi_foo.egg-info/
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)    14228 2023-06-27 13:33:05.000000 yi-foo-0.0.2/yi_foo.egg-info/PKG-INFO
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)      329 2023-06-27 13:33:05.000000 yi-foo-0.0.2/yi_foo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)        1 2023-06-27 13:33:05.000000 yi-foo-0.0.2/yi_foo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)       84 2023-06-27 13:33:05.000000 yi-foo-0.0.2/yi_foo.egg-info/requires.txt
+-rw-rw-r--   0 ychen     (1001) ychen     (1001)       14 2023-06-27 13:33:05.000000 yi-foo-0.0.2/yi_foo.egg-info/top_level.txt
```

### Comparing `yi-foo-0.0.1/PKG-INFO` & `yi-foo-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yi-foo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A foo package
 Home-page: https://github.com/clear-street/foo
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Description: # Gestalt
```

### Comparing `yi-foo-0.0.1/README.md` & `yi-foo-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/gestalt/__init__.py` & `yi-foo-0.0.2/gestalt/__init__.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/gestalt/provider.py` & `yi-foo-0.0.2/gestalt/provider.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/gestalt/utils.py` & `yi-foo-0.0.2/gestalt/utils.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/gestalt/vault.py` & `yi-foo-0.0.2/gestalt/vault.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/setup.py` & `yi-foo-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("requirements.txt") as reqs_file:
     reqs = filter(lambda x: not x.startswith("-"), reqs_file.readlines())
     reqs_list = list(map(lambda x: x.rstrip(), reqs))
 
 setup(name='yi-foo',
-      version='0.0.1',
+      version='0.0.2',
       description='A foo package',
       long_description=readme(),
       long_description_content_type="text/markdown",
       url='https://github.com/clear-street/foo',
       author='Clear Street',
       author_email='engineering@clearstreet.io',
       license='MIT',
```

### Comparing `yi-foo-0.0.1/tests/conftest.py` & `yi-foo-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/tests/test_gestalt.py` & `yi-foo-0.0.2/tests/test_gestalt.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/tests/test_vault.py` & `yi-foo-0.0.2/tests/test_vault.py`

 * *Files identical despite different names*

### Comparing `yi-foo-0.0.1/yi_foo.egg-info/PKG-INFO` & `yi-foo-0.0.2/yi_foo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yi-foo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A foo package
 Home-page: https://github.com/clear-street/foo
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Description: # Gestalt
```

