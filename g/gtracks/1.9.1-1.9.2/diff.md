# Comparing `tmp/gtracks-1.9.1.tar.gz` & `tmp/gtracks-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtracks-1.9.1.tar", last modified: Tue May  3 02:43:42 2022, max compression
+gzip compressed data, was "gtracks-1.9.2.tar", last modified: Tue Jun  7 19:42:17 2022, max compression
```

## Comparing `gtracks-1.9.1.tar` & `gtracks-1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-05-03 02:43:42.306755 gtracks-1.9.1/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2022-02-10 01:43:49.000000 gtracks-1.9.1/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      289 2022-02-10 01:43:49.000000 gtracks-1.9.1/MANIFEST.in
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5506 2022-05-03 02:43:42.306432 gtracks-1.9.1/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5059 2022-02-17 17:33:40.000000 gtracks-1.9.1/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-05-03 02:43:42.302344 gtracks-1.9.1/gtracks/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      234 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2395 2022-05-03 00:46:55.000000 gtracks-1.9.1/gtracks/gff3_to_bed12.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1511 2022-03-31 20:49:25.000000 gtracks-1.9.1/gtracks/gff3_to_bed6.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     8330 2022-05-03 00:35:09.000000 gtracks-1.9.1/gtracks/gtracks.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  2636512 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/hg19.bed12.bed.gz
--rw-r--r--   0 anthonyaylward   (501) staff       (20)  5047093 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/hg38.bed12.bed.gz
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    19422 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/pancreatic_islet_atac_seq_ins_igf2.bw
--rw-r--r--   0 anthonyaylward   (501) staff       (20)   706002 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/sp9512.a02u1.bed12.bed.gz
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    43444 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/sp9512_frond_example.bw
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       44 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/sp9512_frond_turion_dmr.bed
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    43230 2022-02-10 01:43:49.000000 gtracks-1.9.1/gtracks/sp9512_turion_example.bw
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-05-03 02:43:42.305958 gtracks-1.9.1/gtracks.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5506 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      547 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      150 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       44 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2022-05-03 02:43:42.000000 gtracks-1.9.1/gtracks.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2022-05-03 02:43:42.306872 gtracks-1.9.1/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      962 2022-05-03 00:36:43.000000 gtracks-1.9.1/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-06-07 19:42:17.167287 gtracks-1.9.2/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2022-02-10 01:43:49.000000 gtracks-1.9.2/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      289 2022-02-10 01:43:49.000000 gtracks-1.9.2/MANIFEST.in
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5506 2022-06-07 19:42:17.167034 gtracks-1.9.2/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5059 2022-02-17 17:33:40.000000 gtracks-1.9.2/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-06-07 19:42:17.163562 gtracks-1.9.2/gtracks/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      234 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2857 2022-06-07 19:40:06.000000 gtracks-1.9.2/gtracks/gff3_to_bed12.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1574 2022-06-07 19:40:14.000000 gtracks-1.9.2/gtracks/gff3_to_bed6.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     8330 2022-05-03 00:35:09.000000 gtracks-1.9.2/gtracks/gtracks.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  2636512 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/hg19.bed12.bed.gz
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)  5047093 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/hg38.bed12.bed.gz
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    19422 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/pancreatic_islet_atac_seq_ins_igf2.bw
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)   706002 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/sp9512.a02u1.bed12.bed.gz
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    43444 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/sp9512_frond_example.bw
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       44 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/sp9512_frond_turion_dmr.bed
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    43230 2022-02-10 01:43:49.000000 gtracks-1.9.2/gtracks/sp9512_turion_example.bw
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-06-07 19:42:17.166665 gtracks-1.9.2/gtracks.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5506 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      547 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      150 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       44 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2022-06-07 19:42:16.000000 gtracks-1.9.2/gtracks.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2022-06-07 19:42:17.167377 gtracks-1.9.2/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      962 2022-06-07 19:38:57.000000 gtracks-1.9.2/setup.py
```

### Comparing `gtracks-1.9.1/LICENSE` & `gtracks-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/PKG-INFO` & `gtracks-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtracks
-Version: 1.9.1
+Version: 1.9.2
 Summary: Plot genome track data
 Home-page: https://github.com/anthony-aylward/gtracks.git
 Author: Anthony Aylward
 Author-email: aaylward@eng.ucsd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gtracks-1.9.1/README.md` & `gtracks-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/gff3_to_bed12.py` & `gtracks-1.9.2/gtracks/gff3_to_bed12.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,55 @@
 
 
 
 # Imports ======================================================================
 
 from argparse import ArgumentParser
 from pybedtools import BedTool
+import gzip
 
 
 
 
 # Functions ====================================================================
 
 def parse_gff_attributes(attr):
+    """Parse an entry from the "attr" column of a GFF3 file and yield it as
+    a dict
+
+    Parameters
+    ----------
+    attr : str
+        feature attribute string
+
+    Returns
+    ------
+    dict
+        attr entries as a dict
+    """
+
     return dict(pair.split('=') for pair in attr.split(';'))
 
 
 def parse_gff(gff: str, type='gene'):
-    with open(gff) as f:
+    """Parse a GFF3 file and yield its lines as tuples
+
+    Parameters
+    ----------
+    gff : str
+        path to GFF3 file
+    type
+        string indcicating feature type to include, or None to include all
+        features
+    """
+
+    with (gzip.open(gff, 'rt') if gff.endswith('.gz') else open(gff)) as f:
         for l in f:
              if not l.startswith('#'):
-                seqid, _, t, start, end, _, strand, _, attr = l.rstrip().split(
-                                                                           '\t')
+                seqid, _, t, start, end, _, strand, _, attr = l.rstrip().split('\t')
                 if ((t == type) or (type is None)):
                     yield (seqid, int(start), int(end), strand,
                            parse_gff_attributes(attr))
 
 
 def generate_bed(gff, type='gene'):
     for seqid, start, end, strand, attr in parse_gff(gff, type=type):
```

### Comparing `gtracks-1.9.1/gtracks/gff3_to_bed6.py` & `gtracks-1.9.2/gtracks/gff3_to_bed6.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 
 
 # Imports ======================================================================
 
 from argparse import ArgumentParser
 from pybedtools import BedTool
+import gzip
 
 
 
 
 # Functions ====================================================================
 
 def parse_gff_attributes(attr):
     return dict(pair.split('=') for pair in attr.split(';'))
 
 
 def parse_gff(gff: str, type='gene'):
-    with open(gff) as f:
+    with (gzip.open(gff, 'rt') if gff.endswith('.gz') else open(gff)) as f:
         for l in f:
              if not l.startswith('#'):
                 seqid, _, t, start, end, _, strand, _, attr = l.rstrip().split(
                                                                            '\t')
                 if ((t == type) or (type is None)):
                     yield (seqid, int(start), int(end), strand,
                            parse_gff_attributes(attr))
```

### Comparing `gtracks-1.9.1/gtracks/gtracks.py` & `gtracks-1.9.2/gtracks/gtracks.py`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/hg19.bed12.bed.gz` & `gtracks-1.9.2/gtracks/hg19.bed12.bed.gz`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/hg38.bed12.bed.gz` & `gtracks-1.9.2/gtracks/hg38.bed12.bed.gz`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/pancreatic_islet_atac_seq_ins_igf2.bw` & `gtracks-1.9.2/gtracks/pancreatic_islet_atac_seq_ins_igf2.bw`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/sp9512.a02u1.bed12.bed.gz` & `gtracks-1.9.2/gtracks/sp9512.a02u1.bed12.bed.gz`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/sp9512_frond_example.bw` & `gtracks-1.9.2/gtracks/sp9512_frond_example.bw`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks/sp9512_turion_example.bw` & `gtracks-1.9.2/gtracks/sp9512_turion_example.bw`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/gtracks.egg-info/PKG-INFO` & `gtracks-1.9.2/gtracks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtracks
-Version: 1.9.1
+Version: 1.9.2
 Summary: Plot genome track data
 Home-page: https://github.com/anthony-aylward/gtracks.git
 Author: Anthony Aylward
 Author-email: aaylward@eng.ucsd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gtracks-1.9.1/gtracks.egg-info/SOURCES.txt` & `gtracks-1.9.2/gtracks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtracks-1.9.1/setup.py` & `gtracks-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='gtracks',
-    version='1.9.1',
+    version='1.9.2',
     author='Anthony Aylward',
     author_email='aaylward@eng.ucsd.edu',
     description='Plot genome track data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/anthony-aylward/gtracks.git',
     packages=setuptools.find_packages(),
```

