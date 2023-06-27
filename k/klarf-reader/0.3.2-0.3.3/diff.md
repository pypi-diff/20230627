# Comparing `tmp/klarf-reader-0.3.2.tar.gz` & `tmp/klarf-reader-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.2.tar", last modified: Tue Jun 27 08:29:10 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.3.tar", last modified: Tue Jun 27 09:15:51 2023, max compression
```

## Comparing `klarf-reader-0.3.2.tar` & `klarf-reader-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.845491 klarf-reader-0.3.2/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-06-27 08:29:10.842538 klarf-reader-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.762265 klarf-reader-0.3.2/klarf_reader/
--rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.2/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.808107 klarf-reader-0.3.2/klarf_reader/models/
--rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.2/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.813659 klarf-reader-0.3.2/klarf_reader/readers/
--rw-rw-rw-   0        0        0    13879 2023-06-27 08:23:33.000000 klarf-reader-0.3.2/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.824351 klarf-reader-0.3.2/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.2/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.800292 klarf-reader-0.3.2/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-06-27 08:29:10.000000 klarf-reader-0.3.2/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-06-27 08:29:10.000000 klarf-reader-0.3.2/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:29:10.000000 klarf-reader-0.3.2/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-27 08:29:10.000000 klarf-reader-0.3.2/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 08:29:10.000000 klarf-reader-0.3.2/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 08:29:10.846403 klarf-reader-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-27 08:27:33.000000 klarf-reader-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:29:10.830185 klarf-reader-0.3.2/tests/
--rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.2/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.872519 klarf-reader-0.3.3/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-06-27 09:15:51.870253 klarf-reader-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.801402 klarf-reader-0.3.3/klarf_reader/
+-rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.3/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.844044 klarf-reader-0.3.3/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.3/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.850029 klarf-reader-0.3.3/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    13942 2023-06-27 09:10:51.000000 klarf-reader-0.3.3/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.857626 klarf-reader-0.3.3/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.3/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.837530 klarf-reader-0.3.3/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:15:51.873654 klarf-reader-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-27 09:13:11.000000 klarf-reader-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.862890 klarf-reader-0.3.3/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.3/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.2/LICENSE.txt` & `klarf-reader-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.2/PKG-INFO` & `klarf-reader-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.2
+Version: 0.3.3
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.2/README.md` & `klarf-reader-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.2/klarf_reader/klarf.py` & `klarf-reader-0.3.3/klarf_reader/klarf.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.2/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.3/klarf_reader/models/klarf_content.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.2/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.3/klarf_reader/readers/klarf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         "XSIZE",
         "YSIZE",
         "DEFECTAREA",
         "DSIZE",
         "CLASSNUMBER",
         "TEST",
         "CLUSTERNUMBER",
+        "ROUGHBINNUMBER",
+        "FINEBINNUMBER",
         "IMAGECOUNT",
     ]
 
     setup_id = "no_setup"
     next_line_has_coords, next_line_has_numb = False, False
     has_sample_test_plan, next_line_has_sample_test_plan = False, False
     sample_plan_test_x, sample_plan_test_y = [], []
@@ -255,19 +257,19 @@
                     sample_center_location=sample_center_location,
                     xrel=float(defect_paramters_values.get("xrel")),
                     yrel=float(defect_paramters_values.get("yrel")),
                     xindex=int(defect_paramters_values.get("xindex")),
                     yindex=int(defect_paramters_values.get("yindex")),
                 )
 
-                roughbin = defect_paramters_values.get("roughbin")
-                roughbin = int(roughbin) if roughbin is not None else -1
+                roughbin = defect_paramters_values.get("roughbinnumber")
+                roughbin = int(roughbin) if roughbin is not None else 0
 
-                finebin = defect_paramters_values.get("finebin")
-                finebin = int(finebin) if finebin is not None else -1
+                finebin = defect_paramters_values.get("finebinnumber")
+                finebin = int(finebin) if finebin is not None else 0
 
                 defects.append(
                     Defect(
                         id=int(defect_paramters_values.get("defectid")),
                         x_rel=float(defect_paramters_values.get("xrel")),
                         y_rel=float(defect_paramters_values.get("yrel")),
                         x_index=int(defect_paramters_values.get("xindex")),
```

### Comparing `klarf-reader-0.3.2/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.3/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.2/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.3/klarf_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.2
+Version: 0.3.3
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.2/setup.py` & `klarf-reader-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.2"
+version = "0.3.3"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.2/tests/test_klarf.py` & `klarf-reader-0.3.3/tests/test_klarf.py`

 * *Files identical despite different names*

