# Comparing `tmp/pyang-arrcus-plugin-0.4.tar.gz` & `tmp/pyang-arrcus-plugin-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyang-arrcus-plugin-0.4.tar", last modified: Tue Jun 27 19:23:31 2023, max compression
+gzip compressed data, was "pyang-arrcus-plugin-0.5.tar", last modified: Tue Jun 27 19:57:36 2023, max compression
```

## Comparing `pyang-arrcus-plugin-0.4.tar` & `pyang-arrcus-plugin-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.289306 pyang-arrcus-plugin-0.4/
--rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:23:31.289460 pyang-arrcus-plugin-0.4/PKG-INFO
--rw-r--r--   0 mahesh     (501) user      (1000)      746 2022-04-01 17:43:32.000000 pyang-arrcus-plugin-0.4/README.md
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.279644 pyang-arrcus-plugin-0.4/plugins/
--rw-r--r--   0 mahesh     (501) user      (1000)        0 2017-03-14 23:50:57.000000 pyang-arrcus-plugin-0.4/plugins/__init__.py
--rw-r--r--   0 mahesh     (501) user      (1000)     2714 2023-06-27 19:18:49.000000 pyang-arrcus-plugin-0.4/plugins/arrcus.py
-drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:23:31.289039 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/
--rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/PKG-INFO
--rw-r--r--   0 mahesh     (501) user      (1000)      326 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 mahesh     (501) user      (1000)        1 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 mahesh     (501) user      (1000)       69 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/entry_points.txt
--rw-r--r--   0 mahesh     (501) user      (1000)       13 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/requires.txt
--rw-r--r--   0 mahesh     (501) user      (1000)        8 2023-06-27 19:23:31.000000 pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/top_level.txt
--rw-r--r--   0 mahesh     (501) user      (1000)      100 2023-06-27 19:23:31.289984 pyang-arrcus-plugin-0.4/setup.cfg
--rw-r--r--   0 mahesh     (501) user      (1000)      804 2023-06-27 19:23:03.000000 pyang-arrcus-plugin-0.4/setup.py
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:57:36.013311 pyang-arrcus-plugin-0.5/
+-rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:57:36.013486 pyang-arrcus-plugin-0.5/PKG-INFO
+-rw-r--r--   0 mahesh     (501) user      (1000)      746 2022-04-01 17:43:32.000000 pyang-arrcus-plugin-0.5/README.md
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:57:36.006963 pyang-arrcus-plugin-0.5/plugins/
+-rw-r--r--   0 mahesh     (501) user      (1000)        0 2017-03-14 23:50:57.000000 pyang-arrcus-plugin-0.5/plugins/__init__.py
+-rw-r--r--   0 mahesh     (501) user      (1000)     2560 2023-06-27 19:52:57.000000 pyang-arrcus-plugin-0.5/plugins/arrcus.py
+drwxr-xr-x   0 mahesh     (501) user      (1000)        0 2023-06-27 19:57:36.012946 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/
+-rw-r--r--   0 mahesh     (501) user      (1000)     1273 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 mahesh     (501) user      (1000)      326 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)        1 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)       69 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)       13 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/requires.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)        8 2023-06-27 19:57:35.000000 pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/top_level.txt
+-rw-r--r--   0 mahesh     (501) user      (1000)      100 2023-06-27 19:57:36.014018 pyang-arrcus-plugin-0.5/setup.cfg
+-rw-r--r--   0 mahesh     (501) user      (1000)      804 2023-06-27 19:57:22.000000 pyang-arrcus-plugin-0.5/setup.py
```

### Comparing `pyang-arrcus-plugin-0.4/PKG-INFO` & `pyang-arrcus-plugin-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pyang-arrcus-plugin
-Version: 0.4
+Version: 0.5
 Summary: A pyang plugin to validate Arrcus native models
 Home-page: https://github.com/mjethanandani/pyang-arrcus-plugin
 Author: Mahesh Jethanandani
 Author-email: mjethanandani@gmail.com
 License: New-style BSD
-Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.4.tar.gz
+Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.5.tar.gz
 Description: # A pyang plugin to validate Arrcus native YANG models.
         
         This pyang plugin validates Arrcus device specific YANG modules per the naming conventions established within Arrcus.
         
         
         
         ```
```

### Comparing `pyang-arrcus-plugin-0.4/README.md` & `pyang-arrcus-plugin-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyang-arrcus-plugin-0.4/plugins/arrcus.py` & `pyang-arrcus-plugin-0.5/plugins/arrcus.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 
 from pyang import plugin
 from pyang import statements
 from pyang import error
 from pyang.error import err_add
 from pyang.plugins import lint
-from pyang import grammar
 
 def pyang_plugin_init():
     plugin.register_plugin(ArrcusPlugin())
 
 class ArrcusPlugin(lint.LintPlugin):
     def __init__(self):
         lint.LintPlugin.__init__(self)
@@ -48,17 +47,14 @@
             lambda ctx, s: lint.v_chk_required_substmt(ctx, s))
 
         # register our error codes
         error.add_error_code(
             'LINT_MISSING_REQUIRED_SUBSTMT', 3,
             '%s: '
             + 'statement "%s" must have a "%s" substatement')
-        error.add_error_code(
-            'LINT_NOT_HYPHENATED', 4,
-            '%s is not hyphenated, e.g., using underscore')
 
 _required_substatements = {
     'module': (('contact', 'organization', 'description', 'revision'),
                "RFC 8407: 4.8"),
     'submodule': (('contact', 'organization', 'description', 'revision'),
                   "RFC 8407: 4.8"),
     'extension':(('description',), "RFC 8407: 4.14"),
```

### Comparing `pyang-arrcus-plugin-0.4/pyang_arrcus_plugin.egg-info/PKG-INFO` & `pyang-arrcus-plugin-0.5/pyang_arrcus_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pyang-arrcus-plugin
-Version: 0.4
+Version: 0.5
 Summary: A pyang plugin to validate Arrcus native models
 Home-page: https://github.com/mjethanandani/pyang-arrcus-plugin
 Author: Mahesh Jethanandani
 Author-email: mjethanandani@gmail.com
 License: New-style BSD
-Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.4.tar.gz
+Download-URL: https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.5.tar.gz
 Description: # A pyang plugin to validate Arrcus native YANG models.
         
         This pyang plugin validates Arrcus device specific YANG modules per the naming conventions established within Arrcus.
         
         
         
         ```
```

### Comparing `pyang-arrcus-plugin-0.4/setup.py` & `pyang-arrcus-plugin-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pyang-arrcus-plugin',
-    version='0.4',
+    version='0.5',
     description=('A pyang plugin to validate Arrcus native models'),
     long_description=read('README.md'),
     packages=['plugins'],
     author='Mahesh Jethanandani',
     author_email='mjethanandani@gmail.com',
     license='New-style BSD',
     url='https://github.com/mjethanandani/pyang-arrcus-plugin',
-    download_url='https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.4.tar.gz',
+    download_url='https://github.com/mjethanandani/pyang-arrcus-plugin/archive/0.5.tar.gz',
     install_requires=['pyang>=2.5.3'],
     include_package_data=True,
     keywords=['yang', 'validation'],
     classifiers=[],
     entry_points={'pyang.plugin': 'arrcus_pyang_plugin=plugins.arrcus:pyang_plugin_init'}
 )
```

