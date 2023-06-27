# Comparing `tmp/aplr-4.0.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-4.1.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 345459 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   388608 b- defN 23-May-24 16:13 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   410624 b- defN 23-May-24 16:17 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-24 16:08 aplr/__init__.py
--rw-rw-rw-  2.0 fat    10794 b- defN 23-May-24 16:08 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      655 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      691 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/RECORD
-9 files, 812646 bytes uncompressed, 344287 bytes compressed:  57.6%
+Zip file size: 4951408 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 16:16 aplr-4.1.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 16:16 aplr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 16:16 aplr.libs/
+-rwxr-xr-x  2.0 unx 22865864 b- defN 23-Jun-27 16:16 aplr_cpp.cpython-39-i386-linux-gnu.so
+-rwxr-xr-x  2.0 unx   722256 b- defN 23-Jun-27 16:16 aplr_cpp.pypy39-pp73-x86-linux-gnu.so
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-27 16:16 aplr-4.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 16:16 aplr-4.1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      655 b- defN 23-Jun-27 16:16 aplr-4.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1113 b- defN 23-Jun-27 16:16 aplr-4.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      715 b- defN 23-Jun-27 16:16 aplr-4.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-27 16:16 aplr/__init__.py
+-rw-r--r--  2.0 unx    10794 b- defN 23-Jun-27 16:16 aplr/aplr.py
+12 files, 23601588 bytes uncompressed, 4949910 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
-Filename: aplr_cpp.cp39-win_amd64.pyd
+Filename: aplr-4.1.0.dist-info/
 Comment: 
 
-Filename: aplr_cpp.pypy39-pp73-win_amd64.pyd
+Filename: aplr/
 Comment: 
 
-Filename: aplr/__init__.py
+Filename: aplr.libs/
 Comment: 
 
-Filename: aplr/aplr.py
+Filename: aplr_cpp.cpython-39-i386-linux-gnu.so
+Comment: 
+
+Filename: aplr_cpp.pypy39-pp73-x86-linux-gnu.so
+Comment: 
+
+Filename: aplr-4.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-4.0.0.dist-info/LICENSE
+Filename: aplr-4.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-4.0.0.dist-info/METADATA
+Filename: aplr-4.1.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-4.0.0.dist-info/WHEEL
+Filename: aplr-4.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-4.0.0.dist-info/top_level.txt
+Filename: aplr-4.1.0.dist-info/RECORD
 Comment: 
 
-Filename: aplr-4.0.0.dist-info/RECORD
+Filename: aplr/__init__.py
+Comment: 
+
+Filename: aplr/aplr.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `aplr-4.0.0.dist-info/LICENSE` & `aplr-4.1.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Mathias von Ottenbreit <ottenbreitdatascience@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Mathias von Ottenbreit <ottenbreitdatascience@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `aplr-4.0.0.dist-info/METADATA` & `aplr-4.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 4.0.0
+Version: 4.1.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

