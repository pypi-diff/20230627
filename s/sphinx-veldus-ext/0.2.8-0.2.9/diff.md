# Comparing `tmp/sphinx_veldus_ext-0.2.8.tar.gz` & `tmp/sphinx_veldus_ext-0.2.9.tar.gz`

## Comparing `sphinx_veldus_ext-0.2.8.tar` & `sphinx_veldus_ext-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/__init__.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/azgaar_map/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/azgaar_map/azgaar-map.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/azgaar_map/css/azgaar-map.css
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/npc_statblock/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/npc_statblock/npc.html
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/npc_statblock/summary-table.html
--rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/place_statblock/__init__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/place_statblock/place.html
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/place_statblock/summary-table.html
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/README.md
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/__init__.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/azgaar_map/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/azgaar_map/azgaar-map.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/azgaar_map/css/azgaar-map.css
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/npc_statblock/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/npc_statblock/npc.html
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/npc_statblock/summary-table.html
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/place_statblock/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/place_statblock/place.html
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/place_statblock/summary-table.html
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/LICENSE
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 sphinx_veldus_ext-0.2.9/PKG-INFO
```

### Comparing `sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/azgaar_map/__init__.py` & `sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/azgaar_map/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,19 @@
 
 def handle_build_finished(app, exc):
     """
     After the build has finished we need to add the AzgaarMap's CSS to the project's asset files, but only if a Web Viewer has been used in the project.
     """
     # We will provide basic styling for the Web Viewer container
     # Sphinx provides a utility method to copy asset files during build: copy_asset_file()
-    # 
+    #
     # source: https://groups.google.com/g/sphinx-users/c/Z-wcktOhIAc/m/pGDWO0yVBQAJ
     if exc is None: # build succeeded
-        azgaar_mapStylesheet = os.path.join(os.path.dirname(__file__), 'css/azgaar-map.css')
-        destionation = os.path.join(app.outdir, '_static/css/azgaar-map.css')
+        # azgaar_mapStylesheet = os.path.join(os.path.dirname(__file__), 'css/azgaar-map.css')
+        # destionation = os.path.join(app.outdir, '_static/css/azgaar-map.css')
 
         # Ignore if it is a linkcheck build
         if 'linkcheck' in destionation:
             return
 
         copy_asset_file(azgaar_mapStylesheet, destionation)
```

### Comparing `sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/npc_statblock/__init__.py` & `sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/npc_statblock/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/npc_statblock/summary-table.html` & `sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/npc_statblock/summary-table.html`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/place_statblock/__init__.py` & `sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/place_statblock/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/sphinx_veldus_ext/place_statblock/summary-table.html` & `sphinx_veldus_ext-0.2.9/sphinx_veldus_ext/place_statblock/summary-table.html`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/.gitignore` & `sphinx_veldus_ext-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/LICENSE` & `sphinx_veldus_ext-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_veldus_ext-0.2.8/pyproject.toml` & `sphinx_veldus_ext-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sphinx_veldus_ext"
-version = "0.2.8"
+version = "0.2.9"
 authors = [{ name = "Adam DuQuette", email = "duquetteadam@gmail.com" }]
 description = "A Sphinx Extension built for veldus.net"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sphinx_veldus_ext-0.2.8/PKG-INFO` & `sphinx_veldus_ext-0.2.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: sphinx_veldus_ext
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Sphinx Extension built for veldus.net
 Project-URL: Homepage, https://github.com/Veldus/sphinx_veldus_ext
 Project-URL: Bug Tracker, https://github.com/Veldus/sphinx_veldus_ext/issues
 Author-email: Adam DuQuette <duquetteadam@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Veldus
 
-View here: [http://veldus.net/](http://veldus.net/)
+View here: [http://veldus.net/](http://veldus.net/)
+
+[PyPi repository](https://pypi.org/project/sphinx-veldus-ext/)
```

