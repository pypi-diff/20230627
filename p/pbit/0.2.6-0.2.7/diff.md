# Comparing `tmp/pbit-0.2.6.tar.gz` & `tmp/pbit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.6.tar", last modified: Wed Apr 12 02:25:18 2023, max compression
+gzip compressed data, was "pbit-0.2.7.tar", last modified: Mon Jun 26 22:54:25 2023, max compression
```

## Comparing `pbit-0.2.6.tar` & `pbit-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.586870 pbit-0.2.6/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-12 02:25:18.568714 pbit-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.6/README.md
--rw-rw-rw-   0        0        0      518 2023-04-12 02:24:56.000000 pbit-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 02:25:18.587887 pbit-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.492756 pbit-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.504831 pbit-0.2.6/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.6/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.566720 pbit-0.2.6/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14167 2023-04-12 02:24:48.000000 pbit-0.2.6/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.6/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.6/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.6/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.6/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.6/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.6/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.6/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.6/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.540415 pbit-0.2.6/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.234394 pbit-0.2.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-06-26 22:54:25.233416 pbit-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.7/README.md
+-rw-rw-rw-   0        0        0      518 2023-06-26 22:53:18.000000 pbit-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 22:54:25.235390 pbit-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.094685 pbit-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.108646 pbit-0.2.7/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.7/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.231396 pbit-0.2.7/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14167 2023-04-12 02:24:48.000000 pbit-0.2.7/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.7/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.7/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.7/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.7/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.7/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2442 2023-06-26 22:53:09.000000 pbit-0.2.7/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.7/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.7/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:54:25.136677 pbit-0.2.7/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 22:54:25.000000 pbit-0.2.7/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.6/LICENSE` & `pbit-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/pyproject.toml` & `pbit-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.6/src/pbit/__init__.py` & `pbit-0.2.7/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.7/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/column.py` & `pbit-0.2.7/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/measure.py` & `pbit-0.2.7/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/partition.py` & `pbit-0.2.7/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.7/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.7/src/pbit/datamodelschema/relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 			"toColumn": self.to_column,
 			"crossFilteringBehavior": "bothDirections",
 			"joinOnDateBehavior": "datePartOnly",
 			"state": "ready"
 		}
 
 		if not self.is_both_directions:
-			self.reference_data["crossFilteringBehavior"] = "rememberToAddThisLater"
+			self.reference_data["crossFilteringBehavior"] = "oneDirection"
 		else:
 			self.reference_data["crossFilteringBehavior"] = "bothDirections"
 
 	def load(self, data: RelationshipData):
 		self.reference_data = deepcopy(data)
 		self.name = self.reference_data["name"]
 		self.from_table = self.reference_data["fromTable"]
```

### Comparing `pbit-0.2.6/src/pbit/datamodelschema/table.py` & `pbit-0.2.7/src/pbit/datamodelschema/table.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.6/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.7/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

