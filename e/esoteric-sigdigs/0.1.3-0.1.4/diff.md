# Comparing `tmp/esoteric-sigdigs-0.1.3.tar.gz` & `tmp/esoteric-sigdigs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esoteric-sigdigs-0.1.3.tar", last modified: Tue Jun 27 18:03:47 2023, max compression
+gzip compressed data, was "esoteric-sigdigs-0.1.4.tar", last modified: Tue Jun 27 18:12:12 2023, max compression
```

## Comparing `esoteric-sigdigs-0.1.3.tar` & `esoteric-sigdigs-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:03:47.421061 esoteric-sigdigs-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-06-27 04:47:18.000000 esoteric-sigdigs-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6588 2023-06-27 18:03:47.422077 esoteric-sigdigs-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6087 2023-06-27 17:55:37.000000 esoteric-sigdigs-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 18:03:47.418060 esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/
--rw-rw-rw-   0        0        0     6588 2023-06-27 18:03:47.000000 esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-27 18:03:47.000000 esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:03:47.000000 esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:03:47.000000 esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      109 2023-06-27 04:49:12.000000 esoteric-sigdigs-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      621 2023-06-27 18:03:47.426060 esoteric-sigdigs-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 18:12:12.832735 esoteric-sigdigs-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2023-06-27 04:47:18.000000 esoteric-sigdigs-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6588 2023-06-27 18:12:12.833735 esoteric-sigdigs-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6087 2023-06-27 17:55:37.000000 esoteric-sigdigs-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:12:12.826735 esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/
+-rw-rw-rw-   0        0        0     6588 2023-06-27 18:12:12.000000 esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-27 18:12:12.000000 esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:12:12.000000 esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 18:12:12.000000 esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      109 2023-06-27 04:49:12.000000 esoteric-sigdigs-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      597 2023-06-27 18:12:12.835735 esoteric-sigdigs-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 18:12:12.831736 esoteric-sigdigs-0.1.4/sigdigs/
+-rw-rw-rw-   0        0        0        0 2023-06-27 04:56:54.000000 esoteric-sigdigs-0.1.4/sigdigs/__init__.py
+-rw-rw-rw-   0        0        0    10639 2023-06-27 06:57:04.000000 esoteric-sigdigs-0.1.4/sigdigs/sigdigs.py
```

### Comparing `esoteric-sigdigs-0.1.3/LICENSE` & `esoteric-sigdigs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esoteric-sigdigs-0.1.3/PKG-INFO` & `esoteric-sigdigs-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esoteric-sigdigs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package that detects and rounds numbers to significant digits.
 Home-page: https://github.com/ericli3690/esoteric-sigdigs/
 Author: Eric Li
 Author-email: ericli3690@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `esoteric-sigdigs-0.1.3/README.md` & `esoteric-sigdigs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `esoteric-sigdigs-0.1.3/esoteric_sigdigs.egg-info/PKG-INFO` & `esoteric-sigdigs-0.1.4/esoteric_sigdigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esoteric-sigdigs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package that detects and rounds numbers to significant digits.
 Home-page: https://github.com/ericli3690/esoteric-sigdigs/
 Author: Eric Li
 Author-email: ericli3690@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `esoteric-sigdigs-0.1.3/setup.cfg` & `esoteric-sigdigs-0.1.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 736f 7465 7269 632d 7369 6764   = esoteric-sigd
 00000020: 6967 730d 0a76 6572 7369 6f6e 203d 2030  igs..version = 0
-00000030: 2e31 2e33 0d0a 6175 7468 6f72 203d 2045  .1.3..author = E
+00000030: 2e31 2e34 0d0a 6175 7468 6f72 203d 2045  .1.4..author = E
 00000040: 7269 6320 4c69 0d0a 6175 7468 6f72 5f65  ric Li..author_e
 00000050: 6d61 696c 203d 2065 7269 636c 6933 3639  mail = ericli369
 00000060: 3040 676d 6169 6c2e 636f 6d0d 0a64 6573  0@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2050 7974  cription = A Pyt
 00000080: 686f 6e20 7061 636b 6167 6520 7468 6174  hon package that
 00000090: 2064 6574 6563 7473 2061 6e64 2072 6f75   detects and rou
 000000a0: 6e64 7320 6e75 6d62 6572 7320 746f 2073  nds numbers to s
 000000b0: 6967 6e69 6669 6361 6e74 2064 6967 6974  ignificant digit
 000000c0: 732e 0d0a 6c6f 6e67 5f64 6573 6372 6970  s...long_descrip
 000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000110: 6b64 6f77 6e0d 0a70 6163 6b61 6765 7320  kdown..packages 
-00000120: 3d20 5b27 7369 6764 6967 7327 5d0d 0a75  = ['sigdigs']..u
-00000130: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000140: 6875 622e 636f 6d2f 6572 6963 6c69 3336  hub.com/ericli36
-00000150: 3930 2f65 736f 7465 7269 632d 7369 6764  90/esoteric-sigd
-00000160: 6967 732f 0d0a 636c 6173 7369 6669 6572  igs/..classifier
-00000170: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000180: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000190: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-000001a0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001b0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001c0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-000001d0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001e0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-000001f0: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
-00000200: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000210: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000220: 2e30 0d0a 696e 636c 7564 655f 7061 636b  .0..include_pack
-00000230: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-00000240: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000250: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000260: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 6572 6963 6c69 3336 3930 2f65 736f 7465  ericli3690/esote
+00000140: 7269 632d 7369 6764 6967 732f 0d0a 636c  ric-sigdigs/..cl
+00000150: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+00000160: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000170: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000180: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000190: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001a0: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+000001b0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+000001c0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+000001d0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+000001e0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+000001f0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000200: 203d 203e 3d33 2e38 2e30 0d0a 696e 636c   = >=3.8.0..incl
+00000210: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00000220: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
+00000230: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000240: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000250: 300d 0a0d 0a                             0....
```

