# Comparing `tmp/BlueDesc_pywrapper-0.0.2.tar.gz` & `tmp/BlueDesc_pywrapper-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlueDesc_pywrapper-0.0.2.tar", last modified: Tue Jun 27 13:50:35 2023, max compression
+gzip compressed data, was "BlueDesc_pywrapper-0.0.2.post1.tar", last modified: Tue Jun 27 13:59:06 2023, max compression
```

## Comparing `BlueDesc_pywrapper-0.0.2.tar` & `BlueDesc_pywrapper-0.0.2.post1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.318803 BlueDesc_pywrapper-0.0.2/
--rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3015 2023-06-27 13:50:35.319819 BlueDesc_pywrapper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-06-27 13:48:39.000000 BlueDesc_pywrapper-0.0.2/README.md
--rw-rw-rw-   0        0        0     1323 2023-06-27 13:50:35.332129 BlueDesc_pywrapper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.273000 BlueDesc_pywrapper-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.286550 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/
--rw-rw-rw-   0        0        0      142 2023-06-27 13:49:37.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/__init__.py
--rw-rw-rw-   0        0        0     8450 2023-06-27 13:46:44.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
--rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.317291 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3015 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.454673 BlueDesc_pywrapper-0.0.2.post1/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/LICENSE
+-rw-rw-rw-   0        0        0     3021 2023-06-27 13:59:06.454673 BlueDesc_pywrapper-0.0.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-27 13:48:39.000000 BlueDesc_pywrapper-0.0.2.post1/README.md
+-rw-rw-rw-   0        0        0     1361 2023-06-27 13:59:06.456675 BlueDesc_pywrapper-0.0.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.415681 BlueDesc_pywrapper-0.0.2.post1/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.429620 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/
+-rw-rw-rw-   0        0        0      148 2023-06-27 13:58:36.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0     8450 2023-06-27 13:46:44.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
+-rw-rw-rw-   0        0        0     1990 2023-06-27 13:14:52.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/desc_names.json
+-rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/dtypes.json
+-rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.452681 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3021 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/top_level.txt
```

### Comparing `BlueDesc_pywrapper-0.0.2/LICENSE` & `BlueDesc_pywrapper-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2/PKG-INFO` & `BlueDesc_pywrapper-0.0.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc_pywrapper
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `BlueDesc_pywrapper-0.0.2/README.md` & `BlueDesc_pywrapper-0.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2/setup.cfg` & `BlueDesc_pywrapper-0.0.2.post1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -67,17 +67,20 @@
 00000420: 7264 6b69 740d 0a09 696e 7374 616c 6c2d  rdkit...install-
 00000430: 6a64 6b3d 3d30 2e33 2e30 0d0a 0962 6f75  jdk==0.3.0...bou
 00000440: 6e64 6564 2d70 6f6f 6c2d 6578 6563 7574  nded-pool-execut
 00000450: 6f72 3d3d 302e 302e 330d 0a09 426c 7565  or==0.0.3...Blue
 00000460: 4465 7363 0d0a 0d0a 5b6f 7074 696f 6e73  Desc....[options
 00000470: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
 00000480: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000490: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
-000004a0: 7265 7175 6972 655d 0d0a 646f 6373 203d  require]..docs =
-000004b0: 200d 0a09 7370 6869 6e78 0d0a 0973 7068   ...sphinx...sph
-000004c0: 696e 782d 7274 642d 7468 656d 650d 0a09  inx-rtd-theme...
-000004d0: 7370 6869 6e78 2d61 7574 6f64 6f63 2d74  sphinx-autodoc-t
-000004e0: 7970 6568 696e 7473 0d0a 7465 7374 696e  ypehints..testin
-000004f0: 6720 3d20 0d0a 0970 7974 6573 740d 0a0d  g = ...pytest...
-00000500: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000510: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000520: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000490: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000004a0: 5f64 6174 615d 0d0a 2a20 3d20 2a2e 6a73  _data]..* = *.js
+000004b0: 6f6e 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  on....[options.e
+000004c0: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
+000004d0: 646f 6373 203d 200d 0a09 7370 6869 6e78  docs = ...sphinx
+000004e0: 0d0a 0973 7068 696e 782d 7274 642d 7468  ...sphinx-rtd-th
+000004f0: 656d 650d 0a09 7370 6869 6e78 2d61 7574  eme...sphinx-aut
+00000500: 6f64 6f63 2d74 7970 6568 696e 7473 0d0a  odoc-typehints..
+00000510: 7465 7374 696e 6720 3d20 0d0a 0970 7974  testing = ...pyt
+00000520: 6573 740d 0a0d 0a5b 6567 675f 696e 666f  est....[egg_info
+00000530: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000540: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000550: 0a                                       .
```

### Comparing `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/bluedesc_pywrapper.py` & `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/utils.py` & `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/PKG-INFO` & `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc-pywrapper
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

