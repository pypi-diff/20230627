# Comparing `tmp/flardl-0.0.0.tar.gz` & `tmp/flardl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.0.tar", max compression
+gzip compressed data, was "flardl-0.0.2.tar", max compression
```

## Comparing `flardl-0.0.0.tar` & `flardl-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1958 2023-03-16 19:04:52.347324 flardl-0.0.0/LICENSE
--rw-r--r--   0        0        0      243 2023-03-17 16:05:11.897657 flardl-0.0.0/LICENSE.logo.txt
--rw-r--r--   0        0        0     3842 2023-03-17 23:13:17.934525 flardl-0.0.0/README.md
--rw-r--r--   0        0        0     2607 2023-03-17 18:27:32.182557 flardl-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-03-16 20:55:30.632782 flardl-0.0.0/src/flardl/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 18:59:05.343736 flardl-0.0.0/src/flardl/py.typed
--rwxr-xr-x   0        0        0    10985 2023-03-17 22:15:51.165992 flardl-0.0.0/src/flardl/queue_stats.py
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 flardl-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-06-26 23:44:15.902744 flardl-0.0.2/LICENSE
+-rw-r--r--   0        0        0      243 2023-06-26 23:44:15.902744 flardl-0.0.2/LICENSE.logo.txt
+-rw-r--r--   0        0        0     5376 2023-06-26 23:44:15.902744 flardl-0.0.2/README.md
+-rw-r--r--   0        0        0     2732 2023-06-26 23:44:30.726867 flardl-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      748 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     3420 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/downloaders.py
+-rwxr-xr-x   0        0        0    11759 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/py.typed
+-rwxr-xr-x   0        0        0    11572 2023-06-26 23:44:15.910744 flardl-0.0.2/src/flardl/queue_stats.py
+-rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.2/PKG-INFO
```

### Comparing `flardl-0.0.0/LICENSE` & `flardl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.0/pyproject.toml` & `flardl-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.0"
+version = "0.0.2"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
@@ -14,38 +14,42 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
 ]
 keywords = [
     "downloads",
     "adaptive",
     "federated"
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/hydrationdynamics/flardl/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
-aiofiles = ">=22.1.0"
+python = ">=3.9,<4"
+anyio = ">=3.7.0"
+attrs = "^22.2.0"
 httpx = {extras = ["http2"], version = ">=0.23.3"}
 loguru = ">=0.6.0"
 tqdm = ">=4.64.1"
+uvloop = { version = ">=0.17.0", markers = "sys_platform != 'win32'"}
+trio = "^0.22.0"
+
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
-darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
@@ -59,22 +63,22 @@
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 # test deps for this package
-pytest-cov = ">=3.0.0"
 loguru-mypy = ">=0.0.4"
 pandas = ">=1.4.0"
 pandas-stubs = ">=1.5.2.221124"
 pytest-datadir-mgr = ">1.3.1"
 
 [tool.bandit]
 exclude_dirs = ["tests/", "noxfile.py"]
+skips = ["B101", "B311"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 source = ["flardl"]
```

### Comparing `flardl-0.0.0/PKG-INFO` & `flardl-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: flardl
-Version: 0.0.0
-Summary: Flardl
-Home-page: https://github.com/hydrationdynamics/flardl
-License: BSD-3-Clause
-Keywords: downloads,adaptive,federated
-Author: Joel Berendzen
-Author-email: joel@generisbio.com
-Requires-Python: >=3.9,<3.12
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: aiofiles (>=22.1.0)
-Requires-Dist: httpx[http2] (>=0.23.3)
-Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: tqdm (>=4.64.1)
-Project-URL: Changelog, https://github.com/hydrationdynamics/flardl/releases
-Project-URL: Documentation, https://flardl.readthedocs.io
-Project-URL: Repository, https://github.com/hydrationdynamics/flardl
-Description-Content-Type: text/markdown
-
 # Flardl - Adaptive Multi-Site Downloading of Lists
 
 [![PyPI](https://img.shields.io/pypi/v/flardl.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/flardl)][pypi status]
 [![Docs](https://img.shields.io/readthedocs/flardl/latest.svg?label=Read%20the%20Docs)][read the docs]
 [![Tests](https://github.com/hydrationdynamics/flardl/workflows/Tests/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/hydrationdynamics/flardl/branch/main/graph/badge.svg)][codecov]
@@ -70,25 +37,50 @@
 The main speed-up is obtained by asynchronous I/O; the use of multiple servers
 provides stability and dynamic adaptability in the face of unknown server loads
 and net weather.
 
 The name _flardl_ could be either an acronym involving downloading, or a
 nonsense word. You pick.
 
+## Theory
+
+Much has been written under the rubric of queueing theory, which we are purposefully discarding here.
+We take a semi-empirical approach based around chemical rate theory; this is in many was inadequate,
+but a full model of the downloading process requires prior knowledge (such as file sizes) we don't
+usually possess.
+
+The simplest version of downloading simply launches every request as quickly as possible at a
+single server and lets
+the server handle the queueing. The server handles overlapped responses, which quickly drives the
+bandwidth to the maximum set by intervening network policy and hardware (such as ISP throttling),
+where it stays until all requests are completed. However, several effects make this a bit too
+simple:
+
+- Most servers will apply a policy that dumps requests once the queue depth gets too high.
+  These requests must be re-queued, and if that is done stupidly then the available
+  bandwidth gets eaten with unfulfilled requests. The queue depth policy is not known
+  in advance, and it may depend on total queue depth that includes other users.
+
+- A server may decide you are executing a Denial-Of-Service (DOS) attack and respond by
+  severely throttling further requests from your IP address. This throttling can last
+  for hours or days, or even permanent black-listing. This "death penalty" can sometimes
+  be triggered by activity of other users at the same institution that hides behind the
+  same public IP address. I have seen practical classes brought to a complete halt by
+
 ## Requirements
 
-_Flardl_ is tested under python 3.9 to 3.11, on Linux, MacOS, and
-Windows. Under the hood, _flardl_ relies on [httpx] and is supported
+_Flardl_ is tested under python 3.11, on Linux, MacOS, and
+Windows and under 3.9 and 3.10 on Linux. Under the hood,
+_flardl_ relies on
+[https://www.python-httpx.org/] [httpx] and is supported
 on whatever platforms that library works under, for both HTTP/1.1 and HTTP/2.
-HTTP/3 support could easily be added via [aioquic] once enough servers are
+HTTP/3 support could easily be added via
+[https://github.com/aiortc/aioquic][aioquic] once enough servers are
 running HTTP/3 to make that worthwhile.
 
-[httpx]: https://www.python-httpx.org/
-[aioquic]: https://github.com/aiortc/aioquic
-
 ## Installation
 
 You can install _Flardl_ via [pip] from [PyPI]:
 
 ```console
 $ pip install flardl
 ```
@@ -124,8 +116,7 @@
 [file an issue]: https://github.com/hydrationdynamics/flardl/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [license]: https://github.com/hydrationdynamics/flardl/blob/main/LICENSE
 [contributor guide]: https://github.com/hydrationdynamics/flardl/blob/main/CONTRIBUTING.md
-
```

