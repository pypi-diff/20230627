# Comparing `tmp/MacAppOpener-0.0.4-py3-none-any.whl.zip` & `tmp/MacAppOpener-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3091 bytes, number of entries: 6
+Zip file size: 3115 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     2811 b- defN 23-Jun-26 23:02 AppOpener/__init__.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Jun-26 23:14 MacAppOpener-0.0.4.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx     1124 b- defN 23-Jun-26 23:14 MacAppOpener-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 23:14 MacAppOpener-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-26 23:14 MacAppOpener-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      493 b- defN 23-Jun-26 23:14 MacAppOpener-0.0.4.dist-info/RECORD
-6 files, 5592 bytes uncompressed, 2195 bytes compressed:  60.7%
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jun-26 23:29 MacAppOpener-0.0.5.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx     1159 b- defN 23-Jun-26 23:29 MacAppOpener-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 23:29 MacAppOpener-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-26 23:29 MacAppOpener-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      493 b- defN 23-Jun-26 23:29 MacAppOpener-0.0.5.dist-info/RECORD
+6 files, 5627 bytes uncompressed, 2219 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: AppOpener/__init__.py
 Comment: 
 
-Filename: MacAppOpener-0.0.4.dist-info/LICENCE.txt
+Filename: MacAppOpener-0.0.5.dist-info/LICENCE.txt
 Comment: 
 
-Filename: MacAppOpener-0.0.4.dist-info/METADATA
+Filename: MacAppOpener-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: MacAppOpener-0.0.4.dist-info/WHEEL
+Filename: MacAppOpener-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: MacAppOpener-0.0.4.dist-info/top_level.txt
+Filename: MacAppOpener-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: MacAppOpener-0.0.4.dist-info/RECORD
+Filename: MacAppOpener-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `MacAppOpener-0.0.4.dist-info/LICENCE.txt` & `MacAppOpener-0.0.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `MacAppOpener-0.0.4.dist-info/METADATA` & `MacAppOpener-0.0.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: MacAppOpener
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple python module that offers a MacOS alternative to the AppOpener module.
 Home-page: 
 Author: Ryann Elguessab
 Author-email: ryannelguessab@gmail.com
 License: MIT
 Keywords: appMacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
-Project Description
- A simple python module that offers a MacOS alternative to the AppOpener module using the os module and difflib providing an easy way to open and close applications on MacOS using python. The module will search within the applications for the closeset module giving programmers a little leeway. 
+
+A simple python module that offers a MacOS alternative to the AppOpener module using the os module and difflib providing an easy way to open and close applications on MacOS using python. The module will search within the applications for the closeset module giving programmers a little leeway. 
  
 Examples:
 
 open("brave") #opens Brave Browser
 
 close("discord") #closes Discord application
+
+Github Repo: https://github.com/CoderEgloo/MacOpener
 	 
 
+
 Change Log
 ==========
 
 0.0.4 (06/26/2023)
 -------------------
 - Cleaning up files and addding close function
```

