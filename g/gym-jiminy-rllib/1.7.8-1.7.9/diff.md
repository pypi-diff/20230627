# Comparing `tmp/gym_jiminy_rllib-1.7.8-py3-none-any.whl.zip` & `tmp/gym_jiminy_rllib-1.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 19667 bytes, number of entries: 9
--rw-r--r--  2.0 unx      213 b- defN 22-Apr-06 06:38 gym_jiminy/rllib/__init__.py
--rw-r--r--  2.0 unx     2898 b- defN 22-Apr-06 06:38 gym_jiminy/rllib/callbacks.py
--rw-r--r--  2.0 unx    11753 b- defN 22-Apr-06 06:38 gym_jiminy/rllib/curriculum.py
--rw-r--r--  2.0 unx    24372 b- defN 22-Apr-06 06:38 gym_jiminy/rllib/ppo.py
--rw-r--r--  2.0 unx    28823 b- defN 22-Apr-06 06:38 gym_jiminy/rllib/utilities.py
--rw-r--r--  2.0 unx      983 b- defN 22-Apr-06 06:39 gym_jiminy_rllib-1.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-06 06:39 gym_jiminy_rllib-1.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Apr-06 06:39 gym_jiminy_rllib-1.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 22-Apr-06 06:39 gym_jiminy_rllib-1.7.8.dist-info/RECORD
-9 files, 69904 bytes uncompressed, 18355 bytes compressed:  73.7%
+Zip file size: 19668 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      213 b- defN 22-Apr-06 15:40 gym_jiminy/rllib/__init__.py
+-rw-r--r--  2.0 unx     2898 b- defN 22-Apr-06 15:40 gym_jiminy/rllib/callbacks.py
+-rw-r--r--  2.0 unx    11753 b- defN 22-Apr-06 15:40 gym_jiminy/rllib/curriculum.py
+-rw-r--r--  2.0 unx    24372 b- defN 22-Apr-06 15:40 gym_jiminy/rllib/ppo.py
+-rw-r--r--  2.0 unx    28823 b- defN 22-Apr-06 15:40 gym_jiminy/rllib/utilities.py
+-rw-r--r--  2.0 unx      983 b- defN 22-Apr-06 15:41 gym_jiminy_rllib-1.7.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Apr-06 15:41 gym_jiminy_rllib-1.7.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 22-Apr-06 15:41 gym_jiminy_rllib-1.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 22-Apr-06 15:41 gym_jiminy_rllib-1.7.9.dist-info/RECORD
+9 files, 69904 bytes uncompressed, 18356 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gym_jiminy/rllib/ppo.py
 Comment: 
 
 Filename: gym_jiminy/rllib/utilities.py
 Comment: 
 
-Filename: gym_jiminy_rllib-1.7.8.dist-info/METADATA
+Filename: gym_jiminy_rllib-1.7.9.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_rllib-1.7.8.dist-info/WHEEL
+Filename: gym_jiminy_rllib-1.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_rllib-1.7.8.dist-info/top_level.txt
+Filename: gym_jiminy_rllib-1.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_rllib-1.7.8.dist-info/RECORD
+Filename: gym_jiminy_rllib-1.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gym_jiminy_rllib-1.7.8.dist-info/METADATA` & `gym_jiminy_rllib-1.7.9.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-rllib
-Version: 1.7.8
+Version: 1.7.9
 Summary: Specialized Reinforcement learning toolbox based on Ray RLlib for Gym Jiminy.
 Home-page: UNKNOWN
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
@@ -15,13 +15,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6,<3.10
-Requires-Dist: gym-jiminy (==1.7.8)
+Requires-Dist: gym-jiminy (==1.7.9)
 Requires-Dist: ray[default,rllib] (<1.11.0,>=1.10.0)
 Requires-Dist: plotext
 
 UNKNOWN
```

## Comparing `gym_jiminy_rllib-1.7.8.dist-info/RECORD` & `gym_jiminy_rllib-1.7.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 gym_jiminy/rllib/__init__.py,sha256=MlZMjBD7YIi-covQtuLcANdxKb80hgUIvXBpukGlt5A,213
 gym_jiminy/rllib/callbacks.py,sha256=ZqmM4TaxLR4nVCeT3Tioh5Bal00l2dpk8XJN6GA_1bo,2898
 gym_jiminy/rllib/curriculum.py,sha256=mRgbMiX3Ukz8-JJNZkNlAre1QzwGuJ1Ib9ykJXvoMgA,11753
 gym_jiminy/rllib/ppo.py,sha256=YM678IiOCRRyzvOoSphGSz5CjjzKuTAWsZnV-NMdS38,24372
 gym_jiminy/rllib/utilities.py,sha256=PIjoc0rdLdSgPGsj2_W6Ht_wX-8jOvgsnj4MpViLzG0,28823
-gym_jiminy_rllib-1.7.8.dist-info/METADATA,sha256=lREk543PFSVRcePTKCbVkHIOMqo4a5ES2KFwUHBY43A,983
-gym_jiminy_rllib-1.7.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-gym_jiminy_rllib-1.7.8.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
-gym_jiminy_rllib-1.7.8.dist-info/RECORD,,
+gym_jiminy_rllib-1.7.9.dist-info/METADATA,sha256=QTe78607X6vhfgXXBWMRbAR8c41lWzG37Rc0htF4Q_Q,983
+gym_jiminy_rllib-1.7.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+gym_jiminy_rllib-1.7.9.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
+gym_jiminy_rllib-1.7.9.dist-info/RECORD,,
```

