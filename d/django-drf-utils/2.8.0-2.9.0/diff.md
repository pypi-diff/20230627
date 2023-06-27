# Comparing `tmp/django-drf-utils-2.8.0.tar.gz` & `tmp/django-drf-utils-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-utils-2.8.0.tar", last modified: Thu Dec 22 16:01:19 2022, max compression
+gzip compressed data, was "django-drf-utils-2.9.0.tar", last modified: Thu Jan 12 09:26:35 2023, max compression
```

## Comparing `django-drf-utils-2.8.0.tar` & `django-drf-utils-2.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.037895 django-drf-utils-2.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2288 2022-12-22 16:01:19.037895 django-drf-utils-2.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1293 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.031894 django-drf-utils-2.8.0/django_drf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2324 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/email.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/exception_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/logging_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.034894 django-drf-utils-2.8.0/django_drf_utils/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/serializers/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/serializers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/serializers/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.035894 django-drf-utils-2.8.0/django_drf_utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/tests/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.036895 django-drf-utils-2.8.0/django_drf_utils/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/tests/models/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.037895 django-drf-utils-2.8.0/django_drf_utils/views/
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/views/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/django_drf_utils/views/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 16:01:19.033894 django-drf-utils-2.8.0/django_drf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2288 2022-12-22 16:01:18.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      988 2022-12-22 16:01:18.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 16:01:18.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 16:01:17.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      244 2022-12-22 16:01:18.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-12-22 16:01:18.000000 django-drf-utils-2.8.0/django_drf_utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1207 2022-12-22 16:01:06.000000 django-drf-utils-2.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1459 2022-12-22 16:01:19.038895 django-drf-utils-2.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.065249 django-drf-utils-2.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-01-12 09:26:35.066249 django-drf-utils-2.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.060248 django-drf-utils-2.9.0/django_drf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/email.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/exception_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/logging_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.063249 django-drf-utils-2.9.0/django_drf_utils/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/serializers/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/serializers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/serializers/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.064249 django-drf-utils-2.9.0/django_drf_utils/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/tests/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.064249 django-drf-utils-2.9.0/django_drf_utils/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/tests/models/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.065249 django-drf-utils-2.9.0/django_drf_utils/views/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/views/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2581 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/django_drf_utils/views/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 09:26:35.062249 django-drf-utils-2.9.0/django_drf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-01-12 09:26:35.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      988 2023-01-12 09:26:35.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 09:26:35.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 09:26:33.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      244 2023-01-12 09:26:35.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-01-12 09:26:35.000000 django-drf-utils-2.9.0/django_drf_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-01-12 09:26:22.000000 django-drf-utils-2.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-01-12 09:26:35.066249 django-drf-utils-2.9.0/setup.cfg
```

### Comparing `django-drf-utils-2.8.0/LICENSE` & `django-drf-utils-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/PKG-INFO` & `django-drf-utils-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-utils
-Version: 2.8.0
+Version: 2.9.0
 Summary: Utilities for commonly used functionality in django and django-rest-framework among BIWG projects.
 Home-page: https://gitlab.com/biomedit/django-drf-utils
 Author: Robin Engler, Jarosław Surkont, Gerhard Bräunlich, Christian Ribeaud, François Martin, Simone Guzzi, Swen Vermeul
 Author-email: robin.engler@sib.swiss, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com, simone.guzzi@sib.swiss, swen@ethz.ch
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-drf-utils-2.8.0/README.md` & `django-drf-utils-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/config.py` & `django-drf-utils-2.9.0/django_drf_utils/config.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/email.py` & `django-drf-utils-2.9.0/django_drf_utils/email.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/exception_handler.py` & `django-drf-utils-2.9.0/django_drf_utils/exception_handler.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/exceptions.py` & `django-drf-utils-2.9.0/django_drf_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/models.py` & `django-drf-utils-2.9.0/django_drf_utils/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 def NameField(**kwargs):
     unique = kwargs.pop("unique", True)
     return models.CharField(
         max_length=512,
         unique=unique,
         validators=(
             validators.RegexValidator(
-                regex=r"^[a-zA-Z0-9\- ()ßàÀéÉèÈäÄëËïÏöÖüÜçÇâÂêÊîÎôÔûÛ']*$",
+                regex=r"^[a-zA-Z0-9\-_ ()ßàÀéÉèÈäÄëËïÏöÖüÜçÇâÂêÊîÎôÔûÛ']*$",
                 message="Allowed characters: "
-                """"a-z", "A-Z", "0-9", "-", "(", ")", "'", """
+                """"a-z", "A-Z", "0-9", "-", "_", "(", ")", "'", """
                 "spaces and diacritics.",
             ),
         ),
         **kwargs,
     )
```

### Comparing `django-drf-utils-2.8.0/django_drf_utils/serializers/fields.py` & `django-drf-utils-2.9.0/django_drf_utils/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/serializers/utils.py` & `django-drf-utils-2.9.0/django_drf_utils/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/serializers/validators.py` & `django-drf-utils-2.9.0/django_drf_utils/serializers/validators.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/tests/models/utils.py` & `django-drf-utils-2.9.0/django_drf_utils/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/tests/utils.py` & `django-drf-utils-2.9.0/django_drf_utils/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/views/log.py` & `django-drf-utils-2.9.0/django_drf_utils/views/log.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils/views/utils.py` & `django-drf-utils-2.9.0/django_drf_utils/views/utils.py`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/django_drf_utils.egg-info/PKG-INFO` & `django-drf-utils-2.9.0/django_drf_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-utils
-Version: 2.8.0
+Version: 2.9.0
 Summary: Utilities for commonly used functionality in django and django-rest-framework among BIWG projects.
 Home-page: https://gitlab.com/biomedit/django-drf-utils
 Author: Robin Engler, Jarosław Surkont, Gerhard Bräunlich, Christian Ribeaud, François Martin, Simone Guzzi, Swen Vermeul
 Author-email: robin.engler@sib.swiss, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com, simone.guzzi@sib.swiss, swen@ethz.ch
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-drf-utils-2.8.0/django_drf_utils.egg-info/SOURCES.txt` & `django-drf-utils-2.9.0/django_drf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/pyproject.toml` & `django-drf-utils-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-drf-utils-2.8.0/setup.cfg` & `django-drf-utils-2.9.0/setup.cfg`

 * *Files identical despite different names*

