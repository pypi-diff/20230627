# Comparing `tmp/cirq-1.2.0.dev20230627183427-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230627191637-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8386 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/LICENSE
--rw-r--r--  2.0 unx     7885 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jun-27 18:34 cirq-1.2.0.dev20230627183427.dist-info/RECORD
-6 files, 20190 bytes uncompressed, 7348 bytes compressed:  63.6%
+Zip file size: 8378 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7834 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jun-27 19:16 cirq-1.2.0.dev20230627191637.dist-info/RECORD
+6 files, 20139 bytes uncompressed, 7340 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.2.0.dev20230627183427.dist-info/AUTHORS
+Filename: cirq-1.2.0.dev20230627191637.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.2.0.dev20230627183427.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230627191637.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230627183427.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230627191637.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230627183427.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230627191637.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230627183427.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230627191637.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230627183427.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230627191637.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230627183427.dist-info/LICENSE` & `cirq-1.2.0.dev20230627191637.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230627183427.dist-info/METADATA` & `cirq-1.2.0.dev20230627191637.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230627183427
+Version: 1.2.0.dev20230627191637
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-core (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-ft (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-google (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230627183427)
-Requires-Dist: cirq-web (==1.2.0.dev20230627183427)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-core (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-ft (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-google (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230627191637)
+Requires-Dist: cirq-web (==1.2.0.dev20230627191637)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
@@ -33,15 +33,14 @@
 Requires-Dist: freezegun (~=0.3.15) ; extra == 'dev_env'
 Requires-Dist: importlib-metadata ; extra == 'dev_env'
 Requires-Dist: virtualenv ; extra == 'dev_env'
 Requires-Dist: virtualenv-clone ; extra == 'dev_env'
 Requires-Dist: flynt (~=0.60) ; extra == 'dev_env'
 Requires-Dist: black (==22.3.0) ; extra == 'dev_env'
 Requires-Dist: pylint (~=2.13.0) ; extra == 'dev_env'
-Requires-Dist: dill (==0.3.4) ; extra == 'dev_env'
 Requires-Dist: grpcio-tools (~=1.37.0) ; extra == 'dev_env'
 Requires-Dist: mypy-protobuf (==1.10) ; extra == 'dev_env'
 Requires-Dist: ipython (>=7.34.0) ; extra == 'dev_env'
 Requires-Dist: notebook (<=6.4.7,>=6.4.1) ; extra == 'dev_env'
 Requires-Dist: ipykernel (==5.3.4) ; extra == 'dev_env'
 Requires-Dist: papermill (~=2.3.2) ; extra == 'dev_env'
 Requires-Dist: seaborn (~=0.11.1) ; extra == 'dev_env'
```

