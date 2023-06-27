# Comparing `tmp/write_githubstat-0.1.1.tar.gz` & `tmp/write_githubstat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "write_githubstat-0.1.1.tar", max compression
+gzip compressed data, was "write_githubstat-0.1.2.tar", max compression
```

## Comparing `write_githubstat-0.1.1.tar` & `write_githubstat-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-26 18:02:38.283801 write_githubstat-0.1.1/LICENSE
--rw-r--r--   0        0        0      689 2023-06-26 18:02:38.283801 write_githubstat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-06-26 18:02:38.283801 write_githubstat-0.1.1/src/writegithubstat/__init__.py
--rw-r--r--   0        0        0     6910 2023-06-26 18:02:38.283801 write_githubstat-0.1.1/src/writegithubstat/githubstat.py
--rw-r--r--   0        0        0        0 2023-06-26 18:02:38.283801 write_githubstat-0.1.1/src/writegithubstat/py.typed
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 write_githubstat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1292 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/README.md
+-rw-r--r--   0        0        0      710 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/__init__.py
+-rw-r--r--   0        0        0     6943 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/githubstat.py
+-rw-r--r--   0        0        0        0 2023-06-27 06:49:31.641754 write_githubstat-0.1.2/src/writegithubstat/py.typed
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 write_githubstat-0.1.2/PKG-INFO
```

### Comparing `write_githubstat-0.1.1/LICENSE` & `write_githubstat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `write_githubstat-0.1.1/pyproject.toml` & `write_githubstat-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "write-githubstat"
 packages = [
     { include = "writegithubstat", from = "src" },
 ]
-version = "0.1.1"
+version = "0.1.2"
+readme = "README.md"
 description = "write-githubstat makes it easy to collect, filter and save github statistics to csv files."
 license = "Apache 2.0"
 authors = ["David Vegh <david.andras.vegh+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pandas = "^1.5.0"
```

### Comparing `write_githubstat-0.1.1/src/writegithubstat/githubstat.py` & `write_githubstat-0.1.2/src/writegithubstat/githubstat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 import os
 from pathlib import Path
 import logging
-from datetime import date
+from datetime import date, timedelta
 from typing import Dict, Any, List, Union
 
 import requests
 import pandas as pd
 
 
 class GithubAuth:
@@ -182,15 +182,15 @@
             response.raise_for_status()
             responses.append(response.json())
         return stat_type.process_stat(responses)
 
 
 class WriteGithubStat:
     def __init__(self, auth: GithubAuth) -> None:
-        self._date = date.today().strftime("%Y-%m-%d")
+        self._date = (date.today() - timedelta(days=1)).strftime("%Y-%m-%d")
         self._auth = auth
 
     @property
     def date(self) -> str:
         return self._date
 
     def write_stat(self, stat_type: GithubStatType, csv: Path) -> None:
```

