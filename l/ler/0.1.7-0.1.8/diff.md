# Comparing `tmp/ler-0.1.7-py2.py3-none-any.whl.zip` & `tmp/ler-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32105 bytes, number of entries: 10
+Zip file size: 33742 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      315 b- defN 23-Jun-21 13:48 ler/__init__.py
 -rw-r--r--  2.0 unx     5504 b- defN 23-Jun-21 13:48 ler/helperroutines.py
 -rw-r--r--  2.0 unx    43958 b- defN 23-Jun-23 18:18 ler/lens_galaxy_population.py
 -rw-r--r--  2.0 unx    62630 b- defN 23-Jun-26 16:39 ler/ler.py
 -rw-r--r--  2.0 unx    16064 b- defN 23-Jun-21 13:48 ler/multiprocessing_routine.py
 -rw-r--r--  2.0 unx    34396 b- defN 23-Jun-27 11:04 ler/source_population.py
--rw-r--r--  2.0 unx      580 b- defN 23-Jun-27 14:48 ler-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 14:48 ler-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-27 14:48 ler-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      755 b- defN 23-Jun-27 14:48 ler-0.1.7.dist-info/RECORD
-10 files, 164316 bytes uncompressed, 30841 bytes compressed:  81.2%
+-rw-r--r--  2.0 unx     4419 b- defN 23-Jun-27 15:44 ler-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 15:44 ler-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-27 15:44 ler-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      756 b- defN 23-Jun-27 15:44 ler-0.1.8.dist-info/RECORD
+10 files, 168156 bytes uncompressed, 32478 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: ler/multiprocessing_routine.py
 Comment: 
 
 Filename: ler/source_population.py
 Comment: 
 
-Filename: ler-0.1.7.dist-info/METADATA
+Filename: ler-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: ler-0.1.7.dist-info/WHEEL
+Filename: ler-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: ler-0.1.7.dist-info/top_level.txt
+Filename: ler-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: ler-0.1.7.dist-info/RECORD
+Filename: ler-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ler-0.1.7.dist-info/RECORD` & `ler-0.1.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ler/__init__.py,sha256=-hsS7aG12rYYb8jcWQrK9fN_ideB0dOULBoUeb0wPqc,315
 ler/helperroutines.py,sha256=8gcDcEhAL4Nq25WH3vNr2H5lJKBCzDBkKZ-GnaSvHXQ,5504
 ler/lens_galaxy_population.py,sha256=bLxcvPw0tOM_gTFtHIe9CShgb2bJtsThtoXFPRbXJgM,43958
 ler/ler.py,sha256=x9oXntzK3SqxxO4q4I7JX21d2WrDtcqnHUgRPqhEVzU,62630
 ler/multiprocessing_routine.py,sha256=xazcM5V0w_ACiqo6DuBqP1DkX4-B-rCuTKSXRexxNxA,16064
 ler/source_population.py,sha256=vmUDmiKDkhlMS1KprFm6lmLbnqyWY-U0JxWT011wPxU,34396
-ler-0.1.7.dist-info/METADATA,sha256=W0Q-Exg1sJcIz7o0rNIaOlS20b7hnkOzQYThWuGOHd0,580
-ler-0.1.7.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-ler-0.1.7.dist-info/top_level.txt,sha256=VWeWLF_gNMjzquGmqrLXqp2J5WegY86apTUimMTh68I,4
-ler-0.1.7.dist-info/RECORD,,
+ler-0.1.8.dist-info/METADATA,sha256=zdFUgMLBU2nu660sGPRBGI0SbZ3IKDtz6sA09CAqCwU,4419
+ler-0.1.8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+ler-0.1.8.dist-info/top_level.txt,sha256=VWeWLF_gNMjzquGmqrLXqp2J5WegY86apTUimMTh68I,4
+ler-0.1.8.dist-info/RECORD,,
```

