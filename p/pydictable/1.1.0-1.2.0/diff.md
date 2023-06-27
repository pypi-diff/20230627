# Comparing `tmp/pydictable-1.1.0.tar.gz` & `tmp/pydictable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydictable-1.1.0.tar", last modified: Fri May 19 09:57:25 2023, max compression
+gzip compressed data, was "pydictable-1.2.0.tar", last modified: Tue Jun 27 18:11:46 2023, max compression
```

## Comparing `pydictable-1.1.0.tar` & `pydictable-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.231090 pydictable-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 09:57:15.000000 pydictable-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-19 09:57:25.227090 pydictable-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-19 09:57:15.000000 pydictable-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.227090 pydictable-1.1.0/pydictable/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.227090 pydictable-1.1.0/pydictable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:57:25.231090 pydictable-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-19 09:57:15.000000 pydictable-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:11:35.000000 pydictable-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 18:11:46.135373 pydictable-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-27 18:11:35.000000 pydictable-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/pydictable/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/pydictable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:11:46.135373 pydictable-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 18:11:35.000000 pydictable-1.2.0/setup.py
```

### Comparing `pydictable-1.1.0/LICENSE` & `pydictable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydictable-1.1.0/README.md` & `pydictable-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydictable-1.1.0/pydictable/core.py` & `pydictable-1.2.0/pydictable/core.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.1.0/pydictable/field.py` & `pydictable-1.2.0/pydictable/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,7 +328,13 @@
                 raise DataValidationError(f'{k}.{e.path}', f'Invalid value, {str(e.err)}')
 
     def validate(self, field_name: str, value):
         assert type(value) is dict
         for k, v in value.items():
             self.key_type.validate(None, k)
             self.value_type.validate(None, v)
+
+    def of(self):
+        return {
+            'key': self.key_type.spec(),
+            'value': self.value_type.spec()
+        }
```

### Comparing `pydictable-1.1.0/pydictable/test_core.py` & `pydictable-1.2.0/pydictable/test_core.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.1.0/pydictable/type.py` & `pydictable-1.2.0/pydictable/type.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.1.0/setup.py` & `pydictable-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pydictable',
-    version='1.1.0',
+    version='1.2.0',
     author='Pramod Kumar',
     author_email='pramodkumar.damam73@gmail.com',
     description='Make your classes from/to dict',
     url='https://github.com/pskd73/pydictable.git',
     packages=['pydictable'],
     include_package_data=True,
     long_description='A tool to create data modals from dict and convert it to dict. '
```

