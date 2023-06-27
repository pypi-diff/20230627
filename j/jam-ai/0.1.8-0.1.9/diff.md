# Comparing `tmp/jam_ai-0.1.8.tar.gz` & `tmp/jam_ai-0.1.9.tar.gz`

## Comparing `jam_ai-0.1.8.tar` & `jam_ai-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/base.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/base.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/text.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/base.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/openai.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/stability_ai.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/writesonic.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/base.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/model.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/mysql.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/postgres.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/__init__.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/test_base.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.8/LICENSE
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jam_ai-0.1.8/README.md
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jam_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 jam_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.9/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/claude-monet.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/pablo-picasso.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/vincent-van-gogh.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.9/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/base.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/instrument/base.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/instrument/text.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/interface/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/interface/base.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/interface/openai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/interface/writesonic.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/base.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/memory.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/model.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/mysql.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/postgres.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/personnel/base.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/util/generate.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.9/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/interface/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/test_persistence/__init__.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 jam_ai-0.1.9/tests/test_persistence/test_base.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jam_ai-0.1.9/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 jam_ai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 jam_ai-0.1.9/PKG-INFO
```

### Comparing `jam_ai-0.1.8/cmd/main.py` & `jam_ai-0.1.9/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/albert-einstein.json` & `jam_ai-0.1.9/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/homer-simpson.json` & `jam_ai-0.1.9/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/marie-curie.json` & `jam_ai-0.1.9/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/walter-white.json` & `jam_ai-0.1.9/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/base.py` & `jam_ai-0.1.9/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/core.py` & `jam_ai-0.1.9/jam/core.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/instrument/base.py` & `jam_ai-0.1.9/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/instrument/image.py` & `jam_ai-0.1.9/jam/instrument/image.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/base.py` & `jam_ai-0.1.9/jam/interface/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/openai.py` & `jam_ai-0.1.9/jam/interface/openai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/stability_ai.py` & `jam_ai-0.1.9/jam/interface/stability_ai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/writesonic.py` & `jam_ai-0.1.9/jam/interface/writesonic.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/base.py` & `jam_ai-0.1.9/jam/persistence/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/memory.py` & `jam_ai-0.1.9/jam/persistence/memory.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/model.py` & `jam_ai-0.1.9/jam/persistence/model.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/mysql.py` & `jam_ai-0.1.9/jam/persistence/mysql.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/postgres.py` & `jam_ai-0.1.9/jam/persistence/postgres.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/sqlite.py` & `jam_ai-0.1.9/jam/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/personnel/base.py` & `jam_ai-0.1.9/jam/personnel/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/tests/instrument/test_base.py` & `jam_ai-0.1.9/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/tests/interface/test_base.py` & `jam_ai-0.1.9/tests/interface/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/tests/test_persistence/test_base.py` & `jam_ai-0.1.9/tests/test_persistence/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/.gitignore` & `jam_ai-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/LICENSE` & `jam_ai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/README.md` & `jam_ai-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/pyproject.toml` & `jam_ai-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.8"
+version = "0.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
 description = "Engaging with Multiple AI Agents with Jam."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
@@ -57,11 +57,21 @@
   "jam/*",
   "/jam/*/*",
   "/tests/*",
   "/example/*",
   "/cmd/*",
 ]
 
+[tool.hatch.extras]
+database = [
+    'pymysql',
+    'psycopg2',
+]
+
+function = [
+    'stability-sdk',
+]
+
 [project.urls]
 homepage = "https://github.com/abhishtagatya/jam"
 documentation = "https://github.com/abhishtagatya/jam"
 changelog = "https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md"
```

### Comparing `jam_ai-0.1.8/PKG-INFO` & `jam_ai-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Engaging with Multiple AI Agents with Jam.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

