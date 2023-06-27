# Comparing `tmp/pyhelayerslite-1.5.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/pyhelayerslite-1.5.2.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 872652 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      585 b- defN 22-Dec-01 07:38 pyhelayerslite/__init__.py
--rw-rw-rw-  2.0 fat    10240 b- defN 22-Dec-01 08:22 pyhelayerslite/libs/_dummy.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  2147840 b- defN 22-Dec-01 08:13 pyhelayerslite/libs/pyhelayerslite_cppwrappers.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     9892 b- defN 22-Dec-01 08:22 pyhelayerslite-1.5.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1600 b- defN 22-Dec-01 08:22 pyhelayerslite-1.5.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Dec-01 08:22 pyhelayerslite-1.5.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 22-Dec-01 08:22 pyhelayerslite-1.5.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      742 b- defN 22-Dec-01 08:22 pyhelayerslite-1.5.1.0.dist-info/RECORD
-8 files, 2171014 bytes uncompressed, 871342 bytes compressed:  59.9%
+Zip file size: 970153 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      587 b- defN 23-Feb-13 08:33 pyhelayerslite/__init__.py
+-rw-rw-rw-  2.0 fat    10240 b- defN 23-Feb-20 08:52 pyhelayerslite/libs/_dummy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  2374144 b- defN 23-Feb-20 08:45 pyhelayerslite/libs/pyhelayerslite_cppwrappers.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     9892 b- defN 23-Feb-20 08:52 pyhelayerslite-1.5.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1542 b- defN 23-Feb-20 08:52 pyhelayerslite-1.5.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-20 08:52 pyhelayerslite-1.5.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Feb-20 08:52 pyhelayerslite-1.5.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      742 b- defN 23-Feb-20 08:52 pyhelayerslite-1.5.2.0.dist-info/RECORD
+8 files, 2397262 bytes uncompressed, 968843 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyhelayerslite/libs/_dummy.cp39-win_amd64.pyd
 Comment: 
 
 Filename: pyhelayerslite/libs/pyhelayerslite_cppwrappers.cp39-win_amd64.pyd
 Comment: 
 
-Filename: pyhelayerslite-1.5.1.0.dist-info/LICENSE
+Filename: pyhelayerslite-1.5.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyhelayerslite-1.5.1.0.dist-info/METADATA
+Filename: pyhelayerslite-1.5.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pyhelayerslite-1.5.1.0.dist-info/WHEEL
+Filename: pyhelayerslite-1.5.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyhelayerslite-1.5.1.0.dist-info/top_level.txt
+Filename: pyhelayerslite-1.5.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyhelayerslite-1.5.1.0.dist-info/RECORD
+Filename: pyhelayerslite-1.5.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyhelayerslite/__init__.py

```diff
@@ -6,12 +6,13 @@
 # The source code for this program is not published or other-wise divested
 # of its trade secrets, irrespective of what has been deposited with the
 # U.S. Copyright Office.
 #
 
 from .libs.pyhelayerslite_cppwrappers import *
 import os
+
 if 'HELAYERS_RESOURCES_DIR' not in os.environ:
     os.environ['HELAYERS_RESOURCES_DIR'] = os.path.join(os.path.dirname(os.path.abspath(__file__)) , "resources")
 
 # Declare DefaultContext as an alias to the widely used SealCkksContext
 DefaultContext = SealCkksContext
```

## Comparing `pyhelayerslite-1.5.1.0.dist-info/LICENSE` & `pyhelayerslite-1.5.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyhelayerslite-1.5.1.0.dist-info/METADATA` & `pyhelayerslite-1.5.2.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelayerslite
-Version: 1.5.1.0
+Version: 1.5.2.0
 Summary: HElayers SDK for homomorphic encryption
 Author: IBM
 Author-email: FHEstart@us.ibm.com
 License: Community edition license for non-commercial use
 Keywords: helayers,fhe,ai
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Developers
@@ -24,11 +24,12 @@
 
 IBM HElayers is software development kit (SDK) for the practical and efficient
 execution of encrypted workloads using fully homomorphic encrypted data.
 HElayers is designed to enable application developers and data scientists to
 seamlessly apply advanced privacy preserving techniques without requiring
 specialized skills in cryptography.
 
-This package is provided under a community edition license for non-commercial use;
-see [license](https://ibm.ent.box.com/s/zfl6rt2p09811nyy8yow8t3mpsmkmsw6). For commercial deployments and access to the source code, please 
-contact [jbuselli@us.ibm.com](mailto:jbuselli@us.ibm.com) and [rohit.panjala@ibm.com](mailto:rohit.panjala@ibm.com) for the Premium Edition
+This package is provided under a community edition license for non-commercial
+use; see [license](https://ibm.ent.box.com/s/zfl6rt2p09811nyy8yow8t3mpsmkmsw6).
+For commercial deployments and access to the source code, please contact
+[chamliam@ie.ibm.com](mailto:chamliam@ie.ibm.com) for the Premium Edition
 license.
```

