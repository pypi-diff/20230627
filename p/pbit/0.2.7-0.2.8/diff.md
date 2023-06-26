# Comparing `tmp/pbit-0.2.7.tar.gz` & `tmp/pbit-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.7.tar", last modified: Mon Jun 26 22:54:25 2023, max compression
+gzip compressed data, was "pbit-0.2.8.tar", last modified: Mon Jun 26 22:58:50 2023, max compression
```

## Comparing `pbit-0.2.7.tar` & `pbit-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.234394 pbit-0.2.7/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      472 2023-06-26 22:54:25.233416 pbit-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.7/README.md
--rw-rw-rw-   0        0        0      518 2023-06-26 22:53:18.000000 pbit-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 22:54:25.235390 pbit-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.094685 pbit-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.108646 pbit-0.2.7/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.7/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.231396 pbit-0.2.7/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14167 2023-04-12 02:24:48.000000 pbit-0.2.7/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.7/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.7/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.7/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.7/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.7/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2442 2023-06-26 22:53:09.000000 pbit-0.2.7/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.7/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.7/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.136677 pbit-0.2.7/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 22:58:50.407086 pbit-0.2.8/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-06-26 22:58:50.406088 pbit-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.8/README.md
+-rw-rw-rw-   0        0        0      518 2023-06-26 22:58:28.000000 pbit-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 22:58:50.407086 pbit-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 22:58:49.084537 pbit-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 22:58:49.091539 pbit-0.2.8/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.8/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:58:50.107234 pbit-0.2.8/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14167 2023-04-12 02:24:48.000000 pbit-0.2.8/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.8/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.8/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.8/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.8/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.8/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2432 2023-06-26 22:58:16.000000 pbit-0.2.8/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.8/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.8/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:58:49.238760 pbit-0.2.8/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-06-26 22:58:49.000000 pbit-0.2.8/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-06-26 22:58:49.000000 pbit-0.2.8/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:58:49.000000 pbit-0.2.8/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 22:58:49.000000 pbit-0.2.8/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 22:58:49.000000 pbit-0.2.8/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.7/LICENSE` & `pbit-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/pyproject.toml` & `pbit-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.7/src/pbit/__init__.py` & `pbit-0.2.8/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.8/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/column.py` & `pbit-0.2.8/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/measure.py` & `pbit-0.2.8/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/partition.py` & `pbit-0.2.8/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.8/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.8/src/pbit/datamodelschema/relationship.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,12 +72,12 @@
 		relationship_data["name"] = self.name
 		relationship_data["fromTable"] = self.from_table
 		relationship_data["fromColumn"] = self.from_column
 		relationship_data["toTable"] = self.to_table
 		relationship_data["toColumn"] = self.to_column
 
 		if not self.is_both_directions:
-			relationship_data["crossFilteringBehavior"] = "rememberToAddThisLater"
+			relationship_data["crossFilteringBehavior"] = "oneDirection"
 		else:
 			relationship_data["crossFilteringBehavior"] = "bothDirections"
 
 		return relationship_data
```

### Comparing `pbit-0.2.7/src/pbit/datamodelschema/table.py` & `pbit-0.2.8/src/pbit/datamodelschema/table.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.7/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.8/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

