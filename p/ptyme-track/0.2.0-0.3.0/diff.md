# Comparing `tmp/ptyme_track-0.2.0.tar.gz` & `tmp/ptyme_track-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyme_track-0.2.0.tar", max compression
+gzip compressed data, was "ptyme_track-0.3.0.tar", max compression
```

## Comparing `ptyme_track-0.2.0.tar` & `ptyme_track-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/LICENSE
--rw-r--r--   0        0        0     2184 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/README.md
--rw-r--r--   0        0        0       43 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/cement.py
--rw-r--r--   0        0        0     7050 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/client.py
--rw-r--r--   0        0        0      221 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/cur_times.py
--rw-r--r--   0        0        0     2771 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/git_ci_diff.py
--rw-r--r--   0        0        0     3906 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/main.py
--rw-r--r--   0        0        0      936 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/ptyme_env.py
--rw-r--r--   0        0        0     1222 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/secret.py
--rw-r--r--   0        0        0     2561 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/server.py
--rw-r--r--   0        0        0      204 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/signature.py
--rw-r--r--   0        0        0      300 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/signed_time.py
--rw-r--r--   0        0        0     2091 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/time_blocks.py
--rw-r--r--   0        0        0     1829 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/validation.py
--rw-r--r--   0        0        0      798 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 ptyme_track-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2249 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/README.md
+-rw-r--r--   0        0        0       43 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/cement.py
+-rw-r--r--   0        0        0     7050 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/client.py
+-rw-r--r--   0        0        0      221 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/cur_times.py
+-rw-r--r--   0        0        0     2771 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/git_ci_diff.py
+-rw-r--r--   0        0        0     4465 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/main.py
+-rw-r--r--   0        0        0      936 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/ptyme_env.py
+-rw-r--r--   0        0        0     1222 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/secret.py
+-rw-r--r--   0        0        0     2561 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/server.py
+-rw-r--r--   0        0        0      204 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/signature.py
+-rw-r--r--   0        0        0      300 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/signed_time.py
+-rw-r--r--   0        0        0     4794 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/time_blocks.py
+-rw-r--r--   0        0        0     1829 2023-06-27 01:19:18.639442 ptyme_track-0.3.0/ptyme_track/validation.py
+-rw-r--r--   0        0        0      798 2023-06-27 01:19:18.643442 ptyme_track-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 ptyme_track-0.3.0/PKG-INFO
```

### Comparing `ptyme_track-0.2.0/LICENSE` & `ptyme_track-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/README.md` & `ptyme_track-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Ptyme Track
+![versions](https://img.shields.io/pypi/pyversions/ptyme-track)
+
 The obnoxiously hard to spell time tracking based on file modifications and signed time reporting. The P is silent like in Pterodactyl
 
 ## Usage
 
 ### Installation
 `pip install ptyme-track`
```

### Comparing `ptyme_track-0.2.0/ptyme_track/cement.py` & `ptyme_track-0.3.0/ptyme_track/cement.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/client.py` & `ptyme_track-0.3.0/ptyme_track/client.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/git_ci_diff.py` & `ptyme_track-0.3.0/ptyme_track/git_ci_diff.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/main.py` & `ptyme_track-0.3.0/ptyme_track/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,24 @@
         "--standalone", action="store_true", help="Run as both a client and a server"
     )
     parser.add_argument(
         "--git-ci-times",
         action="store_true",
         help="Get the current times on this PR from git. Note that currently times are not validated",
     )
+    parser.add_argument(
+        "--bufferless-block-min-size",
+        help="The minimum number of minutes (inclusive) gapped block must be to lose its buffer",
+        default="5",
+    )
+    parser.add_argument(
+        "--bufferless-block-gap",
+        help="The number of minutes an isolated time block that falls below the min size must be to lose its buffer",
+        default="90",
+    )
 
     args = parser.parse_args()
 
     if args.server:
         from ptyme_track.server import run_forever
 
         run_forever()
@@ -79,15 +89,19 @@
 
         generate_secret()
         return
     if args.time_blocks:
         from ptyme_track.time_blocks import get_time_blocks
 
         time_blocks = get_time_blocks(
-            Path(args.time_blocks), get_secret(), check_against_secret=(not args.no_validate)
+            Path(args.time_blocks),
+            get_secret(),
+            check_against_secret=(not args.no_validate),
+            bufferless_block_min_size=int(args.bufferless_block_min_size),
+            bufferless_block_gap=int(args.bufferless_block_gap),
         )
         total_time = timedelta(minutes=0)
         for block in time_blocks:
             total_time += block.duration
             print(
                 json.dumps(
                     {
```

### Comparing `ptyme_track-0.2.0/ptyme_track/ptyme_env.py` & `ptyme_track-0.3.0/ptyme_track/ptyme_env.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/secret.py` & `ptyme_track-0.3.0/ptyme_track/secret.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/server.py` & `ptyme_track-0.3.0/ptyme_track/server.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/ptyme_track/validation.py` & `ptyme_track-0.3.0/ptyme_track/validation.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.2.0/pyproject.toml` & `ptyme_track-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 # soft limit, wrap just before 100 chars
 line-length = 98
 
 [tool.poetry]
 name = "ptyme-track"
-version = "0.2.0"
+version = "0.3.0"
 description = "The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl"
 authors = ["James Hutchison <JamesGHutchison@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ptyme_track" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ptyme_track-0.2.0/PKG-INFO` & `ptyme_track-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ptyme-track
-Version: 0.2.0
+Version: 0.3.0
 Summary: The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl
 License: MIT
 Author: James Hutchison
 Author-email: JamesGHutchison@proton.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Ptyme Track
+![versions](https://img.shields.io/pypi/pyversions/ptyme-track)
+
 The obnoxiously hard to spell time tracking based on file modifications and signed time reporting. The P is silent like in Pterodactyl
 
 ## Usage
 
 ### Installation
 `pip install ptyme-track`
```

