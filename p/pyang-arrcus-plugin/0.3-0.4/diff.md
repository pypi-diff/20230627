# Comparing `tmp/pyang-arrcus-plugin-0.3.tar.gz` & `tmp/pyang-arrcus-plugin-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyang-arrcus-plugin-0.3.tar", last modified: Tue Jun 27 19:20:56 2023, max compression
+gzip compressed data, was "pyang-arrcus-plugin-0.4.tar", last modified: Tue Jun 27 19:23:31 2023, max compression
```

## Comparing `pyang-arrcus-plugin-0.3.tar` & `pyang-arrcus-plugin-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:20:56.649138 pyang-arrcus-plugin-0.3/
--rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:20:56.649291 pyang-arrcus-plugin-0.3/PKG-INFO
--rw-r--r--   0 mahesh     (501) user      (1000)      746 2022-04-01 17:43:32.000000 pyang-arrcus-plugin-0.3/README.md
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:20:56.646555 pyang-arrcus-plugin-0.3/plugins/
--rw-r--r--   0 mahesh     (501) user      (1000)        0 2017-03-14 23:50:57.000000 pyang-arrcus-plugin-0.3/plugins/__init__.py
--rw-r--r--   0 mahesh     (501) user      (1000)     2714 2023-06-27 19:18:49.000000 pyang-arrcus-plugin-0.3/plugins/arrcus.py
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:20:56.648864 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/
--rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/PKG-INFO
--rw-r--r--   0 mahesh     (501) user      (1000)      326 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 mahesh     (501) user      (1000)        1 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 mahesh     (501) user      (1000)       69 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/entry_points.txt
--rw-r--r--   0 mahesh     (501) user      (1000)       13 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/requires.txt
--rw-r--r--   0 mahesh     (501) user      (1000)        8 2023-06-27 19:20:56.000000 pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/top_level.txt
--rw-r--r--   0 mahesh     (501) user      (1000)      100 2023-06-27 19:20:56.649818 pyang-arrcus-plugin-0.3/setup.cfg
--rw-r--r--   0 mahesh     (501) user      (1000)      804 2022-11-09 09:46:17.000000 pyang-arrcus-plugin-0.3/setup.py
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.289306 pyang-arrcus-plugin-0.4/
+-rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:23:31.289460 pyang-arrcus-plugin-0.4/PKG-INFO
+-rw-r--r--   0 mahesh     (501) user      (1000)      746 2022-04-01 17:43:32.000000 pyang-arrcus-plugin-0.4/README.md
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.279644 pyang-arrcus-plugin-0.4/plugins/
+-rw-r--r--   0 mahesh     (501) user      (1000)        0 2017-03-14 23:50:57.000000 pyang-arrcus-plugin-0.4/plugins/__init__.py
+-rw-r--r--   0 mahesh     (501) user      (1000)     2714 2023-06-27 19:18:49.000000 pyang-arrcus-plugin-0.4/plugins/arrcus.py
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.289039 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/
+-rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 mahesh     (501) user      (1000)      326 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)        1 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)       69 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)       13 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/requires.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)        8 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/top_level.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)      100 2023-06-27 19:23:31.289984 pyang-arrcus-plugin-0.4/setup.cfg
+-rw-r--r--   0 mahesh     (501) user      (1000)      804 2023-06-27 19:23:03.000000 pyang-arrcus-plugin-0.4/setup.py
```

### Comparing `pyang-arrcus-plugin-0.3/PKG-INFO` & `pyang-arrcus-plugin-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pyang-arrcus-plugin
-Version: 0.3
+Version: 0.4
 Summary: A pyang plugin to validate Arrcus native models
 Home-page: https://github.com/mjethanandani/pyang-arrcus-plugin
 Author: Mahesh Jethanandani
 Author-email: mjethanandani@gmail.com
 License: New-style BSD
-Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.2.tar.gz
+Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.4.tar.gz
 Description: # A pyang plugin to validate Arrcus native YANG models.
         
         This pyang plugin validates Arrcus device specific YANG modules per the naming conventions established within Arrcus.
         
         
         
         ```
```

### Comparing `pyang-arrcus-plugin-0.3/README.md` & `pyang-arrcus-plugin-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyang-arrcus-plugin-0.3/plugins/arrcus.py` & `pyang-arrcus-plugin-0.4/plugins/arrcus.py`

 * *Files identical despite different names*

### Comparing `pyang-arrcus-plugin-0.3/pyang_arrcus_plugin.egg-info/PKG-INFO` & `pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pyang-arrcus-plugin
-Version: 0.3
+Version: 0.4
 Summary: A pyang plugin to validate Arrcus native models
 Home-page: https://github.com/mjethanandani/pyang-arrcus-plugin
 Author: Mahesh Jethanandani
 Author-email: mjethanandani@gmail.com
 License: New-style BSD
-Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.2.tar.gz
+Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.4.tar.gz
 Description: # A pyang plugin to validate Arrcus native YANG models.
         
         This pyang plugin validates Arrcus device specific YANG modules per the naming conventions established within Arrcus.
         
         
         
         ```
```

