# Comparing `tmp/pyuff-2.1.tar.gz` & `tmp/pyuff-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuff-2.1.tar", last modified: Sat Dec 24 05:17:44 2022, max compression
+gzip compressed data, was "pyuff-2.2.tar", last modified: Tue Jun 27 05:04:22 2023, max compression
```

## Comparing `pyuff-2.1.tar` & `pyuff-2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-12-24 05:17:44.331735 pyuff-2.1/
--rw-rw-rw-   0        0        0      755 2016-12-12 19:26:26.000000 pyuff-2.1/LICENSE
--rw-rw-rw-   0        0        0     4865 2022-12-24 05:17:44.331004 pyuff-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4495 2021-08-26 19:25:15.000000 pyuff-2.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-24 05:17:44.301707 pyuff-2.1/pyuff/
--rw-rw-rw-   0        0        0       70 2022-12-24 05:13:17.000000 pyuff-2.1/pyuff/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-24 05:17:44.330197 pyuff-2.1/pyuff/datasets/
--rw-rw-rw-   0        0        0      433 2022-12-24 05:04:12.000000 pyuff-2.1/pyuff/datasets/__init__.py
--rw-rw-rw-   0        0        0     5814 2022-01-26 18:44:56.000000 pyuff-2.1/pyuff/datasets/dataset_15.py
--rw-rw-rw-   0        0        0     7565 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_151.py
--rw-rw-rw-   0        0        0     4654 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_164.py
--rw-rw-rw-   0        0        0     2073 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_18.py
--rw-rw-rw-   0        0        0     4381 2022-12-24 05:04:12.000000 pyuff-2.1/pyuff/datasets/dataset_2411.py
--rw-rw-rw-   0        0        0     5283 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_2412.py
--rw-rw-rw-   0        0        0    32083 2022-12-24 05:12:11.000000 pyuff-2.1/pyuff/datasets/dataset_2414.py
--rw-rw-rw-   0        0        0     6963 2022-12-24 05:04:12.000000 pyuff-2.1/pyuff/datasets/dataset_2420.py
--rw-rw-rw-   0        0        0    10947 2022-12-24 05:04:12.000000 pyuff-2.1/pyuff/datasets/dataset_2429.py
--rw-rw-rw-   0        0        0    18252 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_55.py
--rw-rw-rw-   0        0        0    31884 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_58.py
--rw-rw-rw-   0        0        0     4366 2021-07-12 12:06:48.000000 pyuff-2.1/pyuff/datasets/dataset_82.py
--rw-rw-rw-   0        0        0    20086 2022-12-24 05:04:12.000000 pyuff-2.1/pyuff/pyuff.py
--rw-rw-rw-   0        0        0     5770 2022-01-26 18:44:56.000000 pyuff-2.1/pyuff/tools.py
-drwxrwxrwx   0        0        0        0 2022-12-24 05:17:44.320017 pyuff-2.1/pyuff.egg-info/
--rw-rw-rw-   0        0        0     4865 2022-12-24 05:17:44.000000 pyuff-2.1/pyuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2022-12-24 05:17:44.000000 pyuff-2.1/pyuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-24 05:17:44.000000 pyuff-2.1/pyuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-12-24 05:17:44.000000 pyuff-2.1/pyuff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-24 05:17:44.000000 pyuff-2.1/pyuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-24 05:17:44.331735 pyuff-2.1/setup.cfg
--rw-rw-rw-   0        0        0     2231 2021-07-12 12:06:48.000000 pyuff-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:04:22.874030 pyuff-2.2/
+-rw-rw-rw-   0        0        0      755 2016-12-12 19:26:26.000000 pyuff-2.2/LICENSE
+-rw-rw-rw-   0        0        0     4892 2023-06-27 05:04:22.874030 pyuff-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2023-01-27 18:17:03.000000 pyuff-2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 05:04:22.849975 pyuff-2.2/pyuff/
+-rw-rw-rw-   0        0        0       70 2023-06-27 04:59:17.000000 pyuff-2.2/pyuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:04:22.874030 pyuff-2.2/pyuff/datasets/
+-rw-rw-rw-   0        0        0      433 2022-12-24 05:04:12.000000 pyuff-2.2/pyuff/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5814 2022-01-26 18:44:56.000000 pyuff-2.2/pyuff/datasets/dataset_15.py
+-rw-rw-rw-   0        0        0     7565 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_151.py
+-rw-rw-rw-   0        0        0     4654 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_164.py
+-rw-rw-rw-   0        0        0     2073 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_18.py
+-rw-rw-rw-   0        0        0     4400 2023-01-27 18:17:00.000000 pyuff-2.2/pyuff/datasets/dataset_2411.py
+-rw-rw-rw-   0        0        0     5283 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_2412.py
+-rw-rw-rw-   0        0        0    33289 2023-05-07 06:54:07.000000 pyuff-2.2/pyuff/datasets/dataset_2414.py
+-rw-rw-rw-   0        0        0     6963 2022-12-24 05:04:12.000000 pyuff-2.2/pyuff/datasets/dataset_2420.py
+-rw-rw-rw-   0        0        0    10947 2022-12-24 05:04:12.000000 pyuff-2.2/pyuff/datasets/dataset_2429.py
+-rw-rw-rw-   0        0        0    18252 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_55.py
+-rw-rw-rw-   0        0        0    32190 2023-06-27 04:58:18.000000 pyuff-2.2/pyuff/datasets/dataset_58.py
+-rw-rw-rw-   0        0        0     4366 2021-07-12 12:06:48.000000 pyuff-2.2/pyuff/datasets/dataset_82.py
+-rw-rw-rw-   0        0        0    20547 2023-06-27 04:58:18.000000 pyuff-2.2/pyuff/pyuff.py
+-rw-rw-rw-   0        0        0     5770 2023-05-07 08:55:06.000000 pyuff-2.2/pyuff/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 05:04:22.864524 pyuff-2.2/pyuff.egg-info/
+-rw-rw-rw-   0        0        0     4892 2023-06-27 05:04:22.000000 pyuff-2.2/pyuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-27 05:04:22.000000 pyuff-2.2/pyuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 05:04:22.000000 pyuff-2.2/pyuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-27 05:04:22.000000 pyuff-2.2/pyuff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 05:04:22.000000 pyuff-2.2/pyuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 05:04:22.874030 pyuff-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2231 2021-07-12 12:06:48.000000 pyuff-2.2/setup.py
```

### Comparing `pyuff-2.1/LICENSE` & `pyuff-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/PKG-INFO` & `pyuff-2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuff
-Version: 2.1
+Version: 2.2
 Summary: UFF (Universal File Format) read/write.
 Home-page: https://github.com/ladisk/pyuff
 Author: Primož Čermelj, Janko Slavič
 Author-email: primoz.cermelj@gmail.com, janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Keywords: UFF,UNV,Universal File Format,read/write
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 pyuff
 =====
 
 Universal File Format read and write
 ------------------------------------
 This module defines an UFF class to manipulate with the UFF (Universal File Format) files.
 
-Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420** are supported.
+Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420, 2429** are supported.
 
 Check out the `documentation <https://pyuff.readthedocs.io/en/latest/index.html>`_.
 
 To install the package, run:
 
 .. code:: python
 
@@ -153,20 +153,17 @@
 
 
 
 
 
 
 
-
-
-
-|travis|
+|pytest|
 
 |binder| to test the *pyuff Showcase.ipynb* online.
 
 .. |binder| image:: http://mybinder.org/badge.svg
    :target: http://mybinder.org:/repo/ladisk/pyuff
-.. |travis| image:: https://www.travis-ci.com/ladisk/pyuff.svg?branch=master
-    :target: https://travis-ci.com/ladisk/pyuff
+.. |pytest| image:: https://github.com/ladisk/pyuff/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/ladisk/pyuff/actions
```

### Comparing `pyuff-2.1/README.rst` & `pyuff-2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pyuff
 =====
 
 Universal File Format read and write
 ------------------------------------
 This module defines an UFF class to manipulate with the UFF (Universal File Format) files.
 
-Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420** are supported.
+Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420, 2429** are supported.
 
 Check out the `documentation <https://pyuff.readthedocs.io/en/latest/index.html>`_.
 
 To install the package, run:
 
 .. code:: python
 
@@ -141,18 +141,15 @@
 
 
 
 
 
 
 
-
-
-
-|travis|
+|pytest|
 
 |binder| to test the *pyuff Showcase.ipynb* online.
 
 .. |binder| image:: http://mybinder.org/badge.svg
    :target: http://mybinder.org:/repo/ladisk/pyuff
-.. |travis| image:: https://www.travis-ci.com/ladisk/pyuff.svg?branch=master
-    :target: https://travis-ci.com/ladisk/pyuff
+.. |pytest| image:: https://github.com/ladisk/pyuff/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/ladisk/pyuff/actions
```

### Comparing `pyuff-2.1/pyuff/datasets/dataset_15.py` & `pyuff-2.2/pyuff/datasets/dataset_15.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_151.py` & `pyuff-2.2/pyuff/datasets/dataset_151.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_164.py` & `pyuff-2.2/pyuff/datasets/dataset_164.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_18.py` & `pyuff-2.2/pyuff/datasets/dataset_18.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_2411.py` & `pyuff-2.2/pyuff/datasets/dataset_2411.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 def _write2411(fh, dset):
     try:
         dict = {}
 
         dset = _opt_fields(dset, dict)
         fh.write('%6i\n%6i%74s\n' % (-1, 2411, ' '))
-
-        for node in range(dset['node_nums'].shape[0]):
-            fh.write('%10i%10i%10i%10i\n' % (node, dset['def_cs'][node], dset['disp_cs'][node],
+        
+        for node,node_id in enumerate(dset['node_nums']):
+            fh.write('%10i%10i%10i%10i\n' % (int(node_id), dset['def_cs'][node], dset['disp_cs'][node],
                                             dset['color'][node]))
 
             fh.write('%25.16e%25.16e%25.16e\n' % (dset['x'][node], dset['y'][node], dset['z'][node]))
 
         fh.write('%6i\n' % -1)
 
     except:
```

### Comparing `pyuff-2.1/pyuff/datasets/dataset_2412.py` & `pyuff-2.2/pyuff/datasets/dataset_2412.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_2414.py` & `pyuff-2.2/pyuff/datasets/dataset_2414.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,33 @@
                                             dset['imaginary_part_eigenvalue'], 
                                             dset['real_part_of_modal_A_or_modal_mass'], 
                                             dset['imaginary_part_of_modal_A_or_modal_mass'],
                                             dset['real_part_of_modal_B_or_modal_mass'], 
                                             dset['imaginary_part_of_modal_B_or_modal_mass']))                            
             for index in range(dset['node_nums'].shape[0]):
                 fh.write('%10i\n' % (int(dset['node_nums'][index])))
-                fh.write('%13.5e%13.5e%13.5e%13.5e%13.5e%13.5e\n' % (
-                                            np.real(dset['x'][index]),
-                                            np.imag(dset['x'][index]),
-                                            np.real(dset['y'][index]),
-                                            np.imag(dset['y'][index]),
-                                            np.real(dset['z'][index]),
-                                            np.imag(dset['z'][index])))
+                if dset['number_of_data_values_for_the_data_component'] == 3 : 
+                    fh.write('%13.5e%13.5e%13.5e%13.5e%13.5e%13.5e\n' % (
+                                                np.real(dset['x'][index]),
+                                                np.imag(dset['x'][index]),
+                                                np.real(dset['y'][index]),
+                                                np.imag(dset['y'][index]),
+                                                np.real(dset['z'][index]),
+                                                np.imag(dset['z'][index])))
+                elif dset['number_of_data_values_for_the_data_component'] == 2 : 
+                    fh.write('%13.5e%13.5e%13.5e%13.5e\n' % (
+                                                np.real(dset['x'][index]),
+                                                np.imag(dset['x'][index]),
+                                                np.real(dset['y'][index]),
+                                                np.imag(dset['y'][index]),))
+                elif dset['number_of_data_values_for_the_data_component'] == 1 : 
+                    fh.write('%13.5e%13.5e\n' % (
+                                                np.real(dset['x'][index]),
+                                                np.imag(dset['x'][index]),))
+                
             fh.write('%6i\n' % (-1))
         # Dictionairy keys have a general name.
         # The meaning of these records and fields depends on the software which writes/reads these.
         else:
             fh.write('%10i%10i%10i%10i%10i%10i%10i%10i\n' % (
                                             dset['record10_field1'], 
                                             dset['record10_field2'],
@@ -116,15 +128,15 @@
                                             dset['record13_field5'],
                                             dset['record13_field6']))                        
             
             # The data and structure of Record 14 and 15 depend on the 'dataset_location'
             if dset['dataset_location'] == 1:
                 for index in range(dset['node_nums'].shape[0]):
                     fh.write('%10i\n' % (dset['node_nums'][index]))
-                    for field in range(dset['data_at_node'][index]):
+                    for field in dset['data_at_node'][index]:
                         # number of values unknown, so loop
                         fh.write('%13.5e' % (field))
                     fh.write('\n')
                 fh.write('%6i\n' % (-1))
 
             elif dset['dataset_location'] == 2:
                 for index in range(dset['element_nums'].shape[0]):
@@ -194,20 +206,28 @@
             dset.update(_parse_header_line(split_header[14], 6, [13, 13, 13, 13, 13, 13], [0.5,0.5, 0.5, 0.5, 0.5, 0.5],
                                             ['real_part_eigenvalue', 'imaginary_part_eigenvalue', 
                                                 'real_part_of_modal_A_or_modal_mass', 'imaginary_part_of_modal_A_or_modal_mass', 
                                                 'real_part_of_modal_B_or_modal_mass', 'imaginary_part_of_modal_B_or_modal_mass']))
 
             split_data = ''.join(block_data.splitlines(True)[15:])
             split_data = split_data.split()
-            if dset['data_type'] == 5 and dset['number_of_data_values_for_the_data_component'] == 3:
+            # generic reading method
+            n_skip = dset['number_of_data_values_for_the_data_component'] * 2 + 1 # x2 real/imag
+            
+            if dset['data_type'] == 5 :
                 values = np.asarray([float(str) for str in split_data], 'd')
-                dset['node_nums'] = np.array(values[::7].copy(), dtype=int)
-                dset['x'] = values[1::7].copy()+values[2::7].copy()*1j
-                dset['y'] = values[3::7].copy()+values[4::7].copy()*1j
-                dset['z'] = values[5::7].copy()+values[6::7].copy()*1j   
+                dset['node_nums'] = np.array(values[::n_skip].copy(), dtype=int)
+                
+                dset['x'] = values[1::n_skip].copy()+values[2::n_skip].copy()*1j
+                
+                if dset['number_of_data_values_for_the_data_component'] >= 2 :
+                    dset['y'] = values[3::n_skip].copy()+values[4::n_skip].copy()*1j
+                
+                if dset['number_of_data_values_for_the_data_component'] >= 3 :
+                    dset['z'] = values[5::n_skip].copy()+values[6::n_skip].copy()*1j   
 
         # Processing unnamed records and fields
         # Dictionairy keys have a general name.
         # The meaning of these records and fields depends on the software which writes/reads these.
         # This section processes the data in record 14 and 15 as general as possible.
         # general reading functionality min_values is set to 1 in _parse_header_line to keep it as general as possible
         else:
```

### Comparing `pyuff-2.1/pyuff/datasets/dataset_2420.py` & `pyuff-2.2/pyuff/datasets/dataset_2420.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_2429.py` & `pyuff-2.2/pyuff/datasets/dataset_2429.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_55.py` & `pyuff-2.2/pyuff/datasets/dataset_55.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/datasets/dataset_58.py` & `pyuff-2.2/pyuff/datasets/dataset_58.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import struct
 import sys
 import os
 
 from ..tools import _opt_fields, _parse_header_line, check_dict_for_none
 from .. import pyuff
 
-def _write58(fh, dset, mode='add', _filename=None):
+def _write58(fh, dset, mode='add', _filename=None, force_double=True):
     """Writes function at nodal DOF - data-set 58 - to an open file fh."""
     try:
-        if not (dset['func_type'] in [1, 2, 3, 4, 6]):
+        if not (dset['func_type'] in [1, 2, 3, 4, 6, 9]):
             raise ValueError('Unsupported function type')
         # handle optional fields - only those that are not calculated
         # automatically
         dict = {'units_description': '',
                 'id1': 'NONE',
                 'id2': 'NONE',
                 'id3': 'NONE',
@@ -49,30 +49,40 @@
                 'spec_data_type': 0,
                 'abscissa_spec_data_type': 0,
                 'ordinate_spec_data_type': 0,
                 'z_axis_spec_data_type': 0,
                 'version_num': 0,
                 'abscissa_spacing': 0}
         dset = _opt_fields(dset, dict)
-        # Write strings to the file - always in double precision => ord_data_type = 2
-        # for real data and 6 for complex data
+
+        # Write strings to the file - always in double precision 
+        # => ord_data_type = 2 (single) and 4 (double) for real data 
+        # => ord_data_type = 5 (single) and 6 (double) for complex data
         num_pts = len(dset['data'])
         is_r = not np.iscomplexobj(dset['data'])
         if is_r:
             # real data
-            dset['ord_data_type'] = 4
-            n_bytes = num_pts * 8
-            if 'n_bytes' in dset.keys():
-                dset['n_bytes'] = n_bytes
-            ord_data_type = dset['ord_data_type']
+            if force_double:
+                dset['ord_data_type'] = 4
         else:
             # complex data
-            dset['ord_data_type'] = 6
+            if force_double:
+                dset['ord_data_type'] = 6
+
+        if dset['ord_data_type'] in [4, 6]: # double precision
+            is_double = True
             n_bytes = num_pts * 8
-            ord_data_type = 6
+        elif dset['ord_data_type'] in [2, 5]: # sigle precision
+            is_double = False
+            n_bytes = num_pts * 4
+
+        if 'n_bytes' in dset.keys():
+            dset['n_bytes'] = n_bytes
+
+        ord_data_type = dset['ord_data_type']
 
         is_even = bool(dset['abscissa_spacing'])  # handling even/uneven abscissa spacing manually
 
         # handling abscissa spacing automatically
         # is_even = len( set( [ dset['x'][ii]-dset['x'][ii-1] for ii in range(1,len(dset['x'])) ] ) ) == 1
         # decode utf to ascii
         for k, v in dset.items():
@@ -149,44 +159,46 @@
                 [fh.write(struct.pack('>d', datai)) for datai in data]
             fh.close()
             if mode.lower() == 'overwrite':
                 fh = open(_filename, 'wt')
             elif mode.lower() == 'add':
                 fh = open(_filename, 'at')
         else:
-            n4_blocks = len(data) // 4
-            rem_vals = len(data) % 4
-            if is_r:
-                if is_even:
-                    fh.write(n4_blocks * '%20.11e%20.11e%20.11e%20.11e\n' % tuple(data[:4 * n4_blocks]))
-                    if rem_vals > 0:
-                        fh.write((rem_vals * '%20.11e' + '\n') % tuple(data[4 * n4_blocks:]))
-                else:
-                    fh.write(n4_blocks * '%13.5e%20.11e%13.5e%20.11e\n' % tuple(data[:4 * n4_blocks]))
-                    if rem_vals > 0:
-                        fmt = ['%13.5e', '%20.11e', '%13.5e', '%20.11e']
-                        fh.write((''.join(fmt[rem_vals]) + '\n') % tuple(data[4 * n4_blocks:]))
-            else:
-                if is_even:
-                    fh.write(n4_blocks * '%20.11e%20.11e%20.11e%20.11e\n' % tuple(data[:4 * n4_blocks]))
-                    if rem_vals > 0:
-                        fh.write((rem_vals * '%20.11e' + '\n') % tuple(data[4 * n4_blocks:]))
+            if is_double: # write double precision
+                n4_blocks = len(data) // 4
+                rem_vals = len(data) % 4
+                if is_r:
+                    if is_even:
+                        fh.write(n4_blocks * '%20.11e%20.11e%20.11e%20.11e\n' % tuple(data[:4 * n4_blocks]))
+                        if rem_vals > 0:
+                            fh.write((rem_vals * '%20.11e' + '\n') % tuple(data[4 * n4_blocks:]))
+                    else:
+                        fh.write(n4_blocks * '%13.5e%20.11e%13.5e%20.11e\n' % tuple(data[:4 * n4_blocks]))
+                        if rem_vals > 0:
+                            fmt = ['%13.5e', '%20.11e', '%13.5e', '%20.11e']
+                            fh.write((''.join(fmt[rem_vals]) + '\n') % tuple(data[4 * n4_blocks:]))
                 else:
-                    n3_blocks = len(data) / 3
-                    rem_vals = len(data) % 3
-                    # TODO: It breaks here for long measurements. Implement exceptions.
-                    # n3_blocks seems to be a natural number but of the wrong type. Convert for now,
-                    # but make assertion to prevent werid things from happening.
-                    if float(n3_blocks - int(n3_blocks)) != 0.0:
-                        print('Warning: Something went wrong when savning the uff file.')
-                    n3_blocks = int(n3_blocks)
-                    fh.write(n3_blocks * '%13.5e%20.11e%20.11e\n' % tuple(data[:3 * n3_blocks]))
-                    if rem_vals > 0:
-                        fmt = ['%13.5e', '%20.11e', '%20.11e']
-                        fh.write((''.join(fmt[rem_vals]) + '\n') % tuple(data[3 * n3_blocks:]))
+                    if is_even:
+                        fh.write(n4_blocks * '%20.11e%20.11e%20.11e%20.11e\n' % tuple(data[:4 * n4_blocks]))
+                        if rem_vals > 0:
+                            fh.write((rem_vals * '%20.11e' + '\n') % tuple(data[4 * n4_blocks:]))
+                    else:
+                        n3_blocks = len(data) // 3
+                        rem_vals = len(data) % 3
+                        fh.write(n3_blocks * '%13.5e%20.11e%20.11e\n' % tuple(data[:3 * n3_blocks]))
+                        if rem_vals != 0: # There should be no rem
+                            print('Warning: Something went wrong when savning the uff file.')
+
+            else: # single precision
+                n6_blocks = len(data) // 6
+                rem_vals = len(data) % 6
+                fh.write(n6_blocks * '%13.5e%13.5e%13.5e%13.5e%13.5e%13.5e\n' % tuple(data[:6 * n6_blocks]))
+                if rem_vals > 0:
+                    fh.write((rem_vals * '%13.5e' + '\n') % tuple(data[6 * n6_blocks:]))
+
         fh.write('%6i\n' % -1)
         del data
     except KeyError as msg:
         raise Exception('The required key \'' + msg.args[0] + '\' not present when writing data-set #58')
     except:
         raise Exception('Error writing data-set #58')
```

### Comparing `pyuff-2.1/pyuff/datasets/dataset_82.py` & `pyuff-2.2/pyuff/datasets/dataset_82.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff/pyuff.py` & `pyuff-2.2/pyuff/pyuff.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ==========
 
 This module is part of the www.openmodal.com project and
 defines an UFF class to manipulate with the
 UFF (Universal File Format) files, i.e., to read from and write
 to UFF files. Among the variety of UFF formats, only some of the
 formats (data-set types) frequently used in structural dynamics
-are supported: **151, 15, 55, 58, 58b, 82, 164, 2412, 2420.** Data-set **58b**
+are supported: **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420, 2429** Data-set **58b**
 is actually a hybrid format [1]_ where the signal is written in the
 binary form, while the header-part is slightly different from 58 but still in the
 ascii format.
 
 An UFF file is a file that can have many data-sets of either ascii or binary
 data where data-set is a block of data between the start and end tags ``____-1``
 (``_`` representing the space character). Refer to [1]_ and [2]_ for
@@ -74,16 +74,15 @@
 from .datasets.dataset_164 import _write164, _extract164
 from .datasets.dataset_2411 import _write2411, _extract2411
 from .datasets.dataset_2412 import _write2412, _extract2412
 from .datasets.dataset_2414 import _write2414, _extract2414
 from .datasets.dataset_2420 import _write2420, _extract2420
 from .datasets.dataset_2429 import _write2429, _extract2429
 
-__version__ = '1.26'
-_SUPPORTED_SETS = ['151', '15', '55', '58', '58b', '82', '164', '2411', '2412', '2414', '2420', '2429']
+_SUPPORTED_SETS = ['15', '55', '58', '58b', '82', '151','164', '2411', '2412', '2414', '2420', '2429']
 
 
 class UFF:
     """
     Manages data reading and writing from/to the UFF file.
     
     The UFF class instance requires exactly 1 parameter - a file name of a
@@ -281,45 +280,52 @@
             raise Exception('Error when reading ' + str(ii) + '-th data-set: ' + msg.value)
         except:
             raise Exception('Error when reading data-set(s)')
         if len(dset) == 1:
             dset = dset[0]
         return dset
 
-    def write_sets(self, dsets, mode='add'):
+    def write_sets(self, dsets, mode='add', force_double=True):
         """
         Writes several UFF data-sets to the file.  The mode can be
         either 'add' (default) or 'overwrite'. The dsets is a
         list of dictionaries, each representing one data-set. Unsupported
         data-sets will be ignored. When only 1 data-set is to be written, no
         lists are necessary, i.e., only one dictionary is required.
 
         For each data-set, there are some optional and some required fields at
         dset dictionary. Also, in general, the sum of the required
         and the optional fields together can be less then the number of fields
         read from the same type of data-set; the reason is that for some
         data-sets some fields are set automatically. Optional fields are
         calculated automatically and the dset is updated - as dset is actually
         an alias (aka pointer), this is reflected at the caller too.
+
+        The required fields are:
+            dset - dictionary representing the data-set
+            mode - 'add' or 'overwrite'
+            force_double - True or False (default True). Single precision should
+                be avoided, therefore by default data is saved with double 
+                precision.
         """
         if (not type(dsets).__name__ == 'list'):
             dsets = [dsets]
         n_sets = len(dsets)
         if n_sets < 1:
             raise Exception('Nothing to write')
         if mode.lower() == 'overwrite':
             # overwrite mode; first set is written in the overwrite mode, others
             # in add mode
-            self._write_set(dsets[0], 'overwrite')
+            self._write_set(dsets[0], 'overwrite', force_double=force_double)
             for ii in range(1, n_sets):
-                self._write_set(dsets[ii], 'add')
+                self._write_set(dsets[ii], 'add', force_double=force_double)
         elif mode.lower() == 'add':
             # add mode; all the sets are written in the add mode
             for ii in range(0, n_sets):
-                self._write_set(dsets[ii], 'add')
+                self._write_set(dsets[ii], 'add', force_double=force_double)
         else:
             raise Exception('Unknown mode: ' + mode)
 
     def _read_set(self, n):
         """
         Reads n-th set from UFF file. 
         n can be an integer between 0 and n_sets-1. 
@@ -383,15 +389,15 @@
             dset = _extract2429(block_data)
         else:
             dset['type'] = self._set_types[int(n)]
             # Unsupported data-set - do nothing
             pass
         return dset
 
-    def _write_set(self, dset, mode='add'):
+    def _write_set(self, dset, mode='add', force_double=True):
         """
         Writes UFF data (UFF data-sets) to the file.  The mode can be
         either 'add' (default) or 'overwrite'. The dset is a
         dictionary of keys and corresponding values. Unsupported
         data-set will be ignored.
          
         For each data-set, there are some optional and some required fields at
@@ -429,15 +435,15 @@
                 dset['data'] = np.nan_to_num(dset['data'])
 
             if set_type == 15:
                 _write15(fh, dset)
             elif set_type == 55:
                 _write55(fh, dset)
             elif set_type == 58:
-                _write58(fh, dset, mode, _filename=self._filename)
+                _write58(fh, dset, mode, _filename=self._filename, force_double=force_double)
             elif set_type == 82:
                 _write82(fh, dset)
             elif set_type == 151:
                 _write151(fh, dset)
             elif set_type == 164:
                 _write164(fh, dset)
             elif set_type == 2411:
```

### Comparing `pyuff-2.1/pyuff/tools.py` & `pyuff-2.2/pyuff/tools.py`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/pyuff.egg-info/PKG-INFO` & `pyuff-2.2/pyuff.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuff
-Version: 2.1
+Version: 2.2
 Summary: UFF (Universal File Format) read/write.
 Home-page: https://github.com/ladisk/pyuff
 Author: Primož Čermelj, Janko Slavič
 Author-email: primoz.cermelj@gmail.com, janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Keywords: UFF,UNV,Universal File Format,read/write
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 pyuff
 =====
 
 Universal File Format read and write
 ------------------------------------
 This module defines an UFF class to manipulate with the UFF (Universal File Format) files.
 
-Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420** are supported.
+Read from and write of data-set types **15, 55, 58, 58b, 82, 151, 164, 2411, 2412, 2414, 2420, 2429** are supported.
 
 Check out the `documentation <https://pyuff.readthedocs.io/en/latest/index.html>`_.
 
 To install the package, run:
 
 .. code:: python
 
@@ -153,20 +153,17 @@
 
 
 
 
 
 
 
-
-
-
-|travis|
+|pytest|
 
 |binder| to test the *pyuff Showcase.ipynb* online.
 
 .. |binder| image:: http://mybinder.org/badge.svg
    :target: http://mybinder.org:/repo/ladisk/pyuff
-.. |travis| image:: https://www.travis-ci.com/ladisk/pyuff.svg?branch=master
-    :target: https://travis-ci.com/ladisk/pyuff
+.. |pytest| image:: https://github.com/ladisk/pyuff/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/ladisk/pyuff/actions
```

### Comparing `pyuff-2.1/pyuff.egg-info/SOURCES.txt` & `pyuff-2.2/pyuff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyuff-2.1/setup.py` & `pyuff-2.2/setup.py`

 * *Files identical despite different names*

