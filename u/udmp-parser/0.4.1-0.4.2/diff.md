# Comparing `tmp/udmp_parser-0.4.1-cp32-abi3-win_amd64.whl.zip` & `tmp/udmp_parser-0.4.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 92465 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   206336 b- defN 23-Jun-23 14:32 udmp_parser.cp39-win_amd64.pyd
--rw-rw-r--  2.0 fat    10211 b- defN 23-Jun-23 14:32 udmp_parser-0.4.1.dist-info/METADATA
--rw-rw-r--  2.0 fat      103 b- defN 23-Jun-23 14:32 udmp_parser-0.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 fat        0 b- defN 23-Jun-23 14:32 udmp_parser-0.4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 fat      407 b- defN 23-Jun-23 14:32 udmp_parser-0.4.1.dist-info/RECORD
+-rw-rw-rw-  2.0 fat   206336 b- defN 23-Jun-27 03:33 udmp_parser.cp39-win_amd64.pyd
+-rw-rw-r--  2.0 fat    10211 b- defN 23-Jun-27 03:33 udmp_parser-0.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 fat      103 b- defN 23-Jun-27 03:33 udmp_parser-0.4.2.dist-info/WHEEL
+-rw-rw-r--  2.0 fat        0 b- defN 23-Jun-27 03:33 udmp_parser-0.4.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 fat      407 b- defN 23-Jun-27 03:33 udmp_parser-0.4.2.dist-info/RECORD
 5 files, 217057 bytes uncompressed, 91709 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: udmp_parser.cp39-win_amd64.pyd
 Comment: 
 
-Filename: udmp_parser-0.4.1.dist-info/METADATA
+Filename: udmp_parser-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: udmp_parser-0.4.1.dist-info/WHEEL
+Filename: udmp_parser-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: udmp_parser-0.4.1.dist-info/entry_points.txt
+Filename: udmp_parser-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: udmp_parser-0.4.1.dist-info/RECORD
+Filename: udmp_parser-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `udmp_parser-0.4.1.dist-info/METADATA` & `udmp_parser-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: udmp-parser
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Cross-Platform C++ parser library for Windows user minidumps.
 Author-Email: 0vercl0k <0vercl0k@not-your-biz.net>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Assemblers
 Classifier: Natural Language :: English
 Project-URL: Homepage, https://github.com/0vercl0k/udmp-parser
-Requires-Python: >=3.2
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Python Bindings for `udmp-parser`
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Licence MIT](https://img.shields.io/packagist/l/doctrine/orm.svg?maxAge=2592000?style=plastic)](https://github.com/0vercl0k/udmp-parser/blob/master/LICENSE)
 
 `udmp-parser` is a cross-platform C++ parser library for Windows [user minidumps](https://docs.microsoft.com/en-us/windows/win32/debug/minidump-files) written by [0vercl0k](https://github.com/0vercl0k). The Python bindings were added by [hugsy](https://github.com/hugsy). Refer to the [project page on Github](https://github.com/0vercl0k/udmp-parser) for documentation, issues and pull requests.
```

