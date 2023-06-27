# Comparing `tmp/write_githubstat-0.1.2.tar.gz` & `tmp/write_githubstat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "write_githubstat-0.1.2.tar", max compression
+gzip compressed data, was "write_githubstat-0.1.3.tar", max compression
```

## Comparing `write_githubstat-0.1.2.tar` & `write_githubstat-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/LICENSE
--rw-r--r--   0        0        0     1292 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/README.md
--rw-r--r--   0        0        0      710 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       95 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/__init__.py
--rw-r--r--   0        0        0     6943 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/githubstat.py
--rw-r--r--   0        0        0        0 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/py.typed
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 write_githubstat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1292 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/README.md
+-rw-r--r--   0        0        0      710 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/src/writegithubstat/__init__.py
+-rw-r--r--   0        0        0     6972 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/src/writegithubstat/githubstat.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:06:16.097181 write_githubstat-0.1.3/src/writegithubstat/py.typed
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 write_githubstat-0.1.3/PKG-INFO
```

### Comparing `write_githubstat-0.1.2/LICENSE` & `write_githubstat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `write_githubstat-0.1.2/README.md` & `write_githubstat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `write_githubstat-0.1.2/pyproject.toml` & `write_githubstat-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "write-githubstat"
 packages = [
     { include = "writegithubstat", from = "src" },
 ]
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 description = "write-githubstat makes it easy to collect, filter and save github statistics to csv files."
 license = "Apache 2.0"
 authors = ["David Vegh <david.andras.vegh+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `write_githubstat-0.1.2/src/writegithubstat/githubstat.py` & `write_githubstat-0.1.3/src/writegithubstat/githubstat.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,23 +87,24 @@
     def urls(self) -> List[str]:
         return [
             f"https://api.github.com/repos/{self._owner}/{self._repo}/traffic/popular/paths"
         ]
 
     @property
     def dimensions(self) -> List[str]:
-        return ["path", "title"]
+        return ["path"]
 
     @property
     def measures(self) -> List[str]:
         return ["count", "uniques"]
 
     def process_stat(self, responses: List[Dict[str, Any]]) -> pd.DataFrame:
         data = responses[0]
         df = pd.DataFrame(data)
+        df = df.drop("title", axis=1)
         return df
 
 
 class StarsForks(GithubStatType):
     @property
     def urls(self) -> List[str]:
         return [f"https://api.github.com/repos/{self._owner}/{self._repo}"]
```

### Comparing `write_githubstat-0.1.2/PKG-INFO` & `write_githubstat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-githubstat
-Version: 0.1.2
+Version: 0.1.3
 Summary: write-githubstat makes it easy to collect, filter and save github statistics to csv files.
 License: Apache 2.0
 Author: David Vegh
 Author-email: david.andras.vegh+github@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

