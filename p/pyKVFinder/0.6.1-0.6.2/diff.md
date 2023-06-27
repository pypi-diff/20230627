# Comparing `tmp/pyKVFinder-0.6.1.tar.gz` & `tmp/pyKVFinder-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.6.1.tar", last modified: Mon Jun 12 18:58:23 2023, max compression
+gzip compressed data, was "pyKVFinder-0.6.2.tar", last modified: Tue Jun 27 14:28:19 2023, max compression
```

## Comparing `pyKVFinder-0.6.1.tar` & `pyKVFinder-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.505375 pyKVFinder-0.6.1/C/
--rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/RadzickaWolfenden.toml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/C/
+-rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/setup.py
```

### Comparing `pyKVFinder-0.6.1/C/numpy.i` & `pyKVFinder-0.6.2/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/C/pyKVFinder.c` & `pyKVFinder-0.6.2/C/pyKVFinder.c`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/C/pyKVFinder.h` & `pyKVFinder-0.6.2/C/pyKVFinder.h`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/C/pyKVFinder.i` & `pyKVFinder-0.6.2/C/pyKVFinder.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/LICENSE.txt` & `pyKVFinder-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/PKG-INFO` & `pyKVFinder-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python package to detect and characterize cavities in biomolecular structures
-Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
+Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,20 +685,19 @@
 Keywords: structural biology,proteins,biomolecules,cavity detection,cavity characterization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ##########
 pyKVFinder
 ##########
@@ -749,16 +748,21 @@
   git clone https://github.com/LBC-LNBio/pyKVFinder.git
   pip install pyKVFinder
 
 ********
 Citation
 ********
 
-If you use pyKVFinder, please cite:
+If you use pyKVFinder package, please cite:
+
+Guerra, J. V. S., Ribeiro-Filho, H. V., Jara, G. E., Bortot, L. O., Pereira, J. G. C., & Lopes-de-Oliveira, P. S. (2021). pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC bioinformatics, 22(1), 607. https://doi.org/10.1186/s12859-021-04519-4.
+
+If you use *pyKVFinder.Molecule*, please also cite:
+
+Guerra, J. V. S., Alves, L. F. G., Bourissou, D., Lopes-de-Oliveira, P. S., & Szalóki, G. (2023). Cavity Characterization in Supramolecular Cages. Journal of chemical information and modeling, 63(12), 3772-3785. https://doi.org/10.1021/acs.jcim.3c00328.
 
-Guerra, J.V.d., Ribeiro-Filho, H.V., Jara, G.E. et al. pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC Bioinformatics 22, 607 (2021). https://doi.org/10.1186/s12859-021-04519-4.
 
 *******
 License
 *******
 
 The software is licensed under the terms of the GNU General Public License version 3 (GPL3) and is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `pyKVFinder-0.6.1/README.rst` & `pyKVFinder-0.6.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -48,16 +48,21 @@
   git clone https://github.com/LBC-LNBio/pyKVFinder.git
   pip install pyKVFinder
 
 ********
 Citation
 ********
 
-If you use pyKVFinder, please cite:
+If you use pyKVFinder package, please cite:
+
+Guerra, J. V. S., Ribeiro-Filho, H. V., Jara, G. E., Bortot, L. O., Pereira, J. G. C., & Lopes-de-Oliveira, P. S. (2021). pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC bioinformatics, 22(1), 607. https://doi.org/10.1186/s12859-021-04519-4.
+
+If you use *pyKVFinder.Molecule*, please also cite:
+
+Guerra, J. V. S., Alves, L. F. G., Bourissou, D., Lopes-de-Oliveira, P. S., & Szalóki, G. (2023). Cavity Characterization in Supramolecular Cages. Journal of chemical information and modeling, 63(12), 3772-3785. https://doi.org/10.1021/acs.jcim.3c00328.
 
-Guerra, J.V.d., Ribeiro-Filho, H.V., Jara, G.E. et al. pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC Bioinformatics 22, 607 (2021). https://doi.org/10.1186/s12859-021-04519-4.
 
 *******
 License
 *******
 
 The software is licensed under the terms of the GNU General Public License version 3 (GPL3) and is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyKVFinder-0.6.1/pyKVFinder/__init__.py` & `pyKVFinder-0.6.2/pyKVFinder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.6.1/pyKVFinder/argparser.py` & `pyKVFinder-0.6.2/pyKVFinder/argparser.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.6.2/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.6.2/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/grid.py` & `pyKVFinder-0.6.2/pyKVFinder/grid.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder/main.py` & `pyKVFinder-0.6.2/pyKVFinder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4316,17 +4316,17 @@
 00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010dc0: 2028 7365 6c66 2e67 7269 6420 3d3d 2030   (self.grid == 0
 00010dd0: 292e 6173 7479 7065 286e 756d 7079 2e69  ).astype(numpy.i
 00010de0: 6e74 3332 2920 2a20 322c 2073 656c 662e  nt32) * 2, self.
 00010df0: 7374 6570 2c20 312c 2073 656c 662e 6e74  step, 1, self.nt
 00010e00: 6872 6561 6473 0a20 2020 2020 2020 2020  hreads.         
 00010e10: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00010e20: 2072 6574 7572 6e20 666c 6f61 7428 766f   return float(vo
-00010e30: 6c75 6d65 2e72 6f75 6e64 2864 6563 696d  lume.round(decim
-00010e40: 616c 733d 3229 290a 0a20 2020 2064 6566  als=2))..    def
+00010e20: 2072 6574 7572 6e20 766f 6c75 6d65 2e72   return volume.r
+00010e30: 6f75 6e64 2864 6563 696d 616c 733d 3229  ound(decimals=2)
+00010e40: 2e69 7465 6d28 290a 0a20 2020 2064 6566  .item()..    def
 00010e50: 2070 7265 7669 6577 2873 656c 662c 202a   preview(self, *
 00010e60: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
 00010e70: 3a0a 2020 2020 2020 2020 2222 2250 7265  :.        """Pre
 00010e80: 7669 6577 2074 6865 206d 6f6c 6563 756c  view the molecul
 00010e90: 6172 2073 7572 6661 6365 2069 6e20 7468  ar surface in th
 00010ea0: 6520 3344 2067 7269 642e 0a0a 2020 2020  e 3D grid...    
 00010eb0: 2020 2020 4578 616d 706c 650a 2020 2020      Example.
```

### Comparing `pyKVFinder-0.6.1/pyKVFinder/utils.py` & `pyKVFinder-0.6.2/pyKVFinder/utils.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.6.2/pyKVFinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python package to detect and characterize cavities in biomolecular structures
-Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
+Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,20 +685,19 @@
 Keywords: structural biology,proteins,biomolecules,cavity detection,cavity characterization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ##########
 pyKVFinder
 ##########
@@ -749,16 +748,21 @@
   git clone https://github.com/LBC-LNBio/pyKVFinder.git
   pip install pyKVFinder
 
 ********
 Citation
 ********
 
-If you use pyKVFinder, please cite:
+If you use pyKVFinder package, please cite:
+
+Guerra, J. V. S., Ribeiro-Filho, H. V., Jara, G. E., Bortot, L. O., Pereira, J. G. C., & Lopes-de-Oliveira, P. S. (2021). pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC bioinformatics, 22(1), 607. https://doi.org/10.1186/s12859-021-04519-4.
+
+If you use *pyKVFinder.Molecule*, please also cite:
+
+Guerra, J. V. S., Alves, L. F. G., Bourissou, D., Lopes-de-Oliveira, P. S., & Szalóki, G. (2023). Cavity Characterization in Supramolecular Cages. Journal of chemical information and modeling, 63(12), 3772-3785. https://doi.org/10.1021/acs.jcim.3c00328.
 
-Guerra, J.V.d., Ribeiro-Filho, H.V., Jara, G.E. et al. pyKVFinder: an efficient and integrable Python package for biomolecular cavity detection and characterization in data science. BMC Bioinformatics 22, 607 (2021). https://doi.org/10.1186/s12859-021-04519-4.
 
 *******
 License
 *******
 
 The software is licensed under the terms of the GNU General Public License version 3 (GPL3) and is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `pyKVFinder-0.6.1/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.6.2/pyKVFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.1/pyproject.toml` & `pyKVFinder-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,53 +10,54 @@
 [project]
 name = "pyKVFinder"
 description = "Python package to detect and characterize cavities in biomolecular structures"
 authors = [
     { name = "João Victor da Silva Guerra", email = "jvsguerra@gmail.com" },
     { name = "Helder Veras Ribeiro Filho" },
     { name = "Luiz Fernando Giolo Alves" },
-    { name = "Gabriel Ernesto Jara" },
+    { name = "Gabriel Ernesto Jara" },    
+    { name = "Leandro Oliveira Bortot" },
+    { name = "José Geraldo de Carvalho Pereira" },
     { name = "Paulo Sergio Lopes-de-Oliveira" },
 ]
 maintainers = [
     { name = "João Victor da Silva Guerra", email = "jvsguerra@gmail.com" },
 ]
 license = { file = "LICENSE.txt" }
 readme = { file = "README.rst", content-type = "text/x-rst" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = [
     "structural biology",
     "proteins",
     "biomolecules",
     "cavity detection",
     "cavity characterization",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "toml==0.10.2",
-    "numpy==1.24.3",
+    "numpy==1.25.0",
     "matplotlib==3.7.1",
     "plotly==5.15.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest==7.3.2", "pytest-cov==4.1.0", "black==23.3.0", "flake8==6.0.0"]
+dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "black==23.3.0", "flake8==6.0.0"]
 
 [project.urls]
 homepage = "https://github.com/LBC-LNBio/pyKVFinder/"
 documentation = "https://lbc-lnbio.github.io/pyKVFinder/"
 issues = "https://github.com/LBC-LNBio/pyKVFinder/issues"
 
 [project.scripts]
@@ -80,15 +81,15 @@
 test-requires = "pytest"
 test-command = "pytest {project}/tests/integration -v"
 before-build = [
     "python3 -m pip install --upgrade pip",
     "pip3 install certifi",
     "git clean -fxd build",
 ]
-build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
+build = ["cp39-*", "cp310-*", "cp311-*"]
 
 [tool.cibuildwheel.linux]
 archs = ["native"]
 
 [tool.cibuildwheel.macos]
 environment = { CC = "/usr/local/bin/gcc-9", MACOS_DEVELOPMENT_TARGET = "10.9" }
 before-build = ["brew install gcc@9"]
```

### Comparing `pyKVFinder-0.6.1/setup.py` & `pyKVFinder-0.6.2/setup.py`

 * *Files identical despite different names*

