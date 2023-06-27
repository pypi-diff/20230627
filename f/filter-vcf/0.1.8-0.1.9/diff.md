# Comparing `tmp/filter-vcf-0.1.8.tar.gz` & `tmp/filter-vcf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter-vcf-0.1.8.tar", last modified: Tue May 23 14:12:50 2023, max compression
+gzip compressed data, was "filter-vcf-0.1.9.tar", last modified: Tue May 23 18:16:19 2023, max compression
```

## Comparing `filter-vcf-0.1.8.tar` & `filter-vcf-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       13 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/PYPI.md
--rw-r--r--   0        0        0        0 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/__init__.py
--rw-r--r--   0        0        0      675 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/filter_vcf.py
--rw-r--r--   0        0        0     6044 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/process.py
--rw-r--r--   0        0        0        0 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/__init__.py
--rw-r--r--   0        0        0     1791 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/addDepth.py
--rw-r--r--   0        0        0     3692 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/checkArgs.py
--rw-r--r--   0        0        0     2435 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/cleanAD.py
--rw-r--r--   0        0        0     4257 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/cleanGT.py
--rw-r--r--   0        0        0     1753 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/convertChrName.py
--rw-r--r--   0        0        0      631 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/detectVcf.py
--rw-r--r--   0        0        0      814 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/readVcf.py
--rw-r--r--   0        0        0      720 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/removeNonRef.py
--rw-r--r--   0        0        0     1002 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/sortVcf.py
--rw-r--r--   0        0        0      781 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/unique.py
--rw-r--r--   0        0        0     1485 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/userFilter.py
--rw-r--r--   0        0        0      273 2023-05-23 14:10:30.988090 filter-vcf-0.1.8/filter_vcf/util/writeVcf.py
--rw-r--r--   0        0        0      914 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/GRCh37.fa.gz
--rw-r--r--   0        0        0    62676 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/carisSample.lifted.modified.somatic.vcf.gz
--rw-r--r--   0        0        0     3490 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/decomp.vcf
--rw-r--r--   0        0        0     1443 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/foundationSample.tcf.gz
--rw-r--r--   0        0        0   270284 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/full.vcf
--rw-r--r--   0        0        0     1682 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/presorted.vcf
--rw-r--r--   0        0        0    62601 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/sample.nrm.vcf.gz
--rw-r--r--   0        0        0     1682 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/unsorted.vcf
--rw-r--r--   0        0        0      514 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/unsorted.vcf.gz
--rw-r--r--   0        0        0       40 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/resources/vcf.txt
--rw-r--r--   0        0        0    47400 2023-05-23 14:10:30.992090 filter-vcf-0.1.8/tests/test_process.py
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-05-23 18:13:47.436330 filter-vcf-0.1.9/PYPI.md
+-rw-r--r--   0        0        0        0 2023-05-23 18:13:47.436330 filter-vcf-0.1.9/filter_vcf/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-23 18:13:47.436330 filter-vcf-0.1.9/filter_vcf/filter_vcf.py
+-rw-r--r--   0        0        0     6044 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/process.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/__init__.py
+-rw-r--r--   0        0        0     1791 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/addDepth.py
+-rw-r--r--   0        0        0     3692 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/checkArgs.py
+-rw-r--r--   0        0        0     2435 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/cleanAD.py
+-rw-r--r--   0        0        0     4257 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/cleanGT.py
+-rw-r--r--   0        0        0     1753 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/convertChrName.py
+-rw-r--r--   0        0        0      631 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/detectVcf.py
+-rw-r--r--   0        0        0      814 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/readVcf.py
+-rw-r--r--   0        0        0      720 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/removeNonRef.py
+-rw-r--r--   0        0        0     1002 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/sortVcf.py
+-rw-r--r--   0        0        0      781 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/unique.py
+-rw-r--r--   0        0        0     1485 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/userFilter.py
+-rw-r--r--   0        0        0      323 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/filter_vcf/util/writeVcf.py
+-rw-r--r--   0        0        0      914 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/tests/resources/GRCh37.fa.gz
+-rw-r--r--   0        0        0    62676 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/tests/resources/carisSample.lifted.modified.somatic.vcf.gz
+-rw-r--r--   0        0        0     3490 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/tests/resources/decomp.vcf
+-rw-r--r--   0        0        0     1443 2023-05-23 18:13:47.440330 filter-vcf-0.1.9/tests/resources/foundationSample.tcf.gz
+-rw-r--r--   0        0        0   270284 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/full.vcf
+-rw-r--r--   0        0        0     1682 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/presorted.vcf
+-rw-r--r--   0        0        0    62601 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/sample.nrm.vcf.gz
+-rw-r--r--   0        0        0     1682 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/unsorted.vcf
+-rw-r--r--   0        0        0      514 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/unsorted.vcf.gz
+-rw-r--r--   0        0        0       40 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/resources/vcf.txt
+-rw-r--r--   0        0        0    47400 2023-05-23 18:13:47.444330 filter-vcf-0.1.9/tests/test_process.py
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.9/PKG-INFO
```

### Comparing `filter-vcf-0.1.8/filter_vcf/filter_vcf.py` & `filter-vcf-0.1.9/filter_vcf/filter_vcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/process.py` & `filter-vcf-0.1.9/filter_vcf/process.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/addDepth.py` & `filter-vcf-0.1.9/filter_vcf/util/addDepth.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/checkArgs.py` & `filter-vcf-0.1.9/filter_vcf/util/checkArgs.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/cleanAD.py` & `filter-vcf-0.1.9/filter_vcf/util/cleanAD.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/cleanGT.py` & `filter-vcf-0.1.9/filter_vcf/util/cleanGT.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/convertChrName.py` & `filter-vcf-0.1.9/filter_vcf/util/convertChrName.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/detectVcf.py` & `filter-vcf-0.1.9/filter_vcf/util/detectVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/readVcf.py` & `filter-vcf-0.1.9/filter_vcf/util/readVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/removeNonRef.py` & `filter-vcf-0.1.9/filter_vcf/util/removeNonRef.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/sortVcf.py` & `filter-vcf-0.1.9/filter_vcf/util/sortVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/unique.py` & `filter-vcf-0.1.9/filter_vcf/util/unique.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/filter_vcf/util/userFilter.py` & `filter-vcf-0.1.9/filter_vcf/util/userFilter.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/pyproject.toml` & `filter-vcf-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "filter-vcf"
-version = "0.1.8"
+version = "0.1.9"
 description = "LifeOmic VCF filtering"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging==0.3.2",
     "vcfpy>=0.13.4",
```

### Comparing `filter-vcf-0.1.8/tests/resources/carisSample.lifted.modified.somatic.vcf.gz` & `filter-vcf-0.1.9/tests/resources/carisSample.lifted.modified.somatic.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/decomp.vcf` & `filter-vcf-0.1.9/tests/resources/decomp.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/foundationSample.tcf.gz` & `filter-vcf-0.1.9/tests/resources/foundationSample.tcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/full.vcf` & `filter-vcf-0.1.9/tests/resources/full.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/presorted.vcf` & `filter-vcf-0.1.9/tests/resources/presorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/sample.nrm.vcf.gz` & `filter-vcf-0.1.9/tests/resources/sample.nrm.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/unsorted.vcf` & `filter-vcf-0.1.9/tests/resources/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/resources/unsorted.vcf.gz` & `filter-vcf-0.1.9/tests/resources/unsorted.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.8/tests/test_process.py` & `filter-vcf-0.1.9/tests/test_process.py`

 * *Files identical despite different names*

