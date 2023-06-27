# Comparing `tmp/gumpy-1.1.0.tar.gz` & `tmp/gumpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumpy-1.1.0.tar", last modified: Wed Mar 22 11:56:40 2023, max compression
+gzip compressed data, was "gumpy-1.2.0.tar", last modified: Tue Jun 27 14:55:49 2023, max compression
```

## Comparing `gumpy-1.1.0.tar` & `gumpy-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:56:40.224451 gumpy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-03-22 11:55:55.000000 gumpy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-22 11:56:40.224451 gumpy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-22 11:55:55.000000 gumpy-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 11:55:55.000000 gumpy-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:56:40.224451 gumpy-1.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-03-22 11:55:55.000000 gumpy-1.1.0/bin/gumpy-save-genome.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-03-22 11:55:55.000000 gumpy-1.1.0/bin/to_piezo_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:56:40.224451 gumpy-1.1.0/gumpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-22 11:55:55.000000 gumpy-1.1.0/gumpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-03-22 11:55:55.000000 gumpy-1.1.0/gumpy/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    30207 2023-03-22 11:55:55.000000 gumpy-1.1.0/gumpy/gene.py
--rw-r--r--   0 runner    (1001) docker     (123)    38940 2023-03-22 11:55:55.000000 gumpy-1.1.0/gumpy/genome.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-03-22 11:55:55.000000 gumpy-1.1.0/gumpy/variantfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:56:40.224451 gumpy-1.1.0/gumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-22 11:56:40.000000 gumpy-1.1.0/gumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-22 11:56:40.000000 gumpy-1.1.0/gumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:56:40.000000 gumpy-1.1.0/gumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:56:03.000000 gumpy-1.1.0/gumpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 11:56:40.000000 gumpy-1.1.0/gumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 11:56:40.000000 gumpy-1.1.0/gumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-22 11:55:55.000000 gumpy-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-22 11:56:40.228451 gumpy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-27 14:55:02.000000 gumpy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-27 14:55:49.593083 gumpy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-27 14:55:02.000000 gumpy-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:55:02.000000 gumpy-1.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.589083 gumpy-1.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-06-27 14:55:02.000000 gumpy-1.2.0/bin/gumpy-save-genome.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-27 14:55:02.000000 gumpy-1.2.0/bin/to_piezo_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/gumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51609 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34067 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/gene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/variantfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/gumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:55:10.000000 gumpy-1.2.0/gumpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 14:55:02.000000 gumpy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-27 14:55:49.593083 gumpy-1.2.0/setup.cfg
```

### Comparing `gumpy-1.1.0/LICENSE` & `gumpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gumpy-1.1.0/PKG-INFO` & `gumpy-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 Metadata-Version: 2.1
 Name: gumpy
-Version: 1.1.0
+Version: 1.2.0
 Summary: Genetics with Numpy
 Home-page: https://github.com/oxfordmmm/gumpy
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml)
-[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) [![Documentation Status](https://readthedocs.org/projects/gumpy/badge/?version=latest)](https://gumpy.readthedocs.io/en/latest/?badge=latest) 
+[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) 
+[![Docs](https://github.com/oxfordmmm/gumpy/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gumpy/)
 [![PyPI version](https://badge.fury.io/py/gumpy.svg)](https://badge.fury.io/py/gumpy)
 
 # gumpy
 Genetics with Numpy
 
 ## Installation
 ```
 git clone https://github.com/oxfordmmm/gumpy
 cd gumpy
 pip install .
 ```
 ## Documentation
-Easy access to documentation for public methods can be found using the `pydoc` module from a terminal:
-```
-python -m pydoc -b gumpy
-```
-This should open a browser window showing documentation for all loaded modules. Navigating to `gumpy (package)` should bring up available files to view documentation.
-
-Docstrings contain documentation for almost all methods if documentation of private methods is required.
+https://oxfordmmm.github.io/gumpy/
 
 ## Testing
 A suite of tests can be run from a terminal:
 ```
 python -m pytest --cov=gumpy -vv
 ```
```

### Comparing `gumpy-1.1.0/README.md` & `gumpy-1.2.0/gumpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+Metadata-Version: 2.1
+Name: gumpy
+Version: 1.2.0
+Summary: Genetics with Numpy
+Home-page: https://github.com/oxfordmmm/gumpy
+Author: Philip W Fowler
+Author-email: philip.fowler@ndm.ox.ac.uk
+License: University of Oxford, see LICENSE.md
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Tests](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml)
-[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) [![Documentation Status](https://readthedocs.org/projects/gumpy/badge/?version=latest)](https://gumpy.readthedocs.io/en/latest/?badge=latest) 
+[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) 
+[![Docs](https://github.com/oxfordmmm/gumpy/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gumpy/)
 [![PyPI version](https://badge.fury.io/py/gumpy.svg)](https://badge.fury.io/py/gumpy)
 
 # gumpy
 Genetics with Numpy
 
 ## Installation
 ```
 git clone https://github.com/oxfordmmm/gumpy
 cd gumpy
 pip install .
 ```
 ## Documentation
-Easy access to documentation for public methods can be found using the `pydoc` module from a terminal:
-```
-python -m pydoc -b gumpy
-```
-This should open a browser window showing documentation for all loaded modules. Navigating to `gumpy (package)` should bring up available files to view documentation.
-
-Docstrings contain documentation for almost all methods if documentation of private methods is required.
+https://oxfordmmm.github.io/gumpy/
 
 ## Testing
 A suite of tests can be run from a terminal:
 ```
 python -m pytest --cov=gumpy -vv
 ```
```

### Comparing `gumpy-1.1.0/bin/gumpy-save-genome.py` & `gumpy-1.2.0/bin/gumpy-save-genome.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.1.0/bin/to_piezo_catalogue.py` & `gumpy-1.2.0/bin/to_piezo_catalogue.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.1.0/gumpy/__init__.py` & `gumpy-1.2.0/gumpy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #! /usr/bin/env python3
 '''Genetics with numpy.
 Utilises numpy arrays internally for improved speed when parsing genomes and assigning promoters.
 
 Provides features including:
-    Parsing genbank files to produce Genome (and Gene) objects;
-    Handle assignment of promoter regions to genes within a genome;
-    Parsing VCF files to produce VCFFile (and VCFRecord) objects;
-    Applying a VCF file to a reference genome to produce a new genome;
-    Finding in-depth differences between two genomes such as indels;
-    Finding in-depth differences caused by a VCF such as SNPs, het and null calls;
-    Finding in-depth differences between two genes such as SNPs, indels and mutations in GARC;
-    Handle intricacies of genomes such as reverse complement genes and -1 PRF.
+    * Parsing genbank files to produce Genome (and Gene) objects;
+    * Handle assignment of promoter regions to genes within a genome;
+    * Parsing VCF files to produce VCFFile (and VCFRecord) objects;
+    * Applying a VCF file to a reference genome to produce a new genome;
+    * Finding in-depth differences between two genomes such as indels;
+    * Finding in-depth differences caused by a VCF such as SNPs, het and null calls;
+    * Finding in-depth differences between two genes such as SNPs, indels and mutations in GARC;
+    * Handle intricacies of genomes such as reverse complement genes and -1 PRF.
 
 
 Classes:
-    Genome
-    Gene
-    VCFFile
-    VCFRecord
-    GenomeDifference
-    GeneDifference
+    * Genome
+    * Gene
+    * VCFFile
+    * VCFRecord
+    * GenomeDifference
+    * GeneDifference
 '''
 import importlib.metadata
 
 #Use of semantic versioning, MAJOR.MINOR.MAINTAINANCE where MAJOR is not backwards compatible, but MINOR and MAINTAINANCE are
 __version__ = importlib.metadata.version("gumpy")
```

### Comparing `gumpy-1.1.0/gumpy/gene.py` & `gumpy-1.2.0/gumpy/gene.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Gene object
 '''
 import copy
 import re
 
 import numpy
 
+from collections import defaultdict, Counter
 from gumpy import GeneDifference
 
 
 # FIXME: problems with rrs, mfpB
 class Gene(object):
 
     """Gene object that uses underlying numpy arrays"""
 
-    def __init__(self, name: str=None, nucleotide_sequence: numpy.array=None, nucleotide_index: numpy.array=None, nucleotide_number: numpy.array=None, is_cds: numpy.array=None, is_promoter: numpy.array=None, is_indel: numpy.array=None, indel_length: numpy.array=None, indel_nucleotides: numpy.array=None, reverse_complement: bool=False, codes_protein: bool=True, feature_type: str=None, ribosomal_shifts: [int]=None, minority_populations: list=None):
+    def __init__(self, name: str=None, nucleotide_sequence: numpy.array=None, nucleotide_index: numpy.array=None, nucleotide_number: numpy.array=None, is_cds: numpy.array=None, is_promoter: numpy.array=None, is_indel: numpy.array=None, indel_length: numpy.array=None, indel_nucleotides: numpy.array=None, reverse_complement: bool=False, codes_protein: bool=True, feature_type: str=None, ribosomal_shifts: [int]=None, minority_populations: list=None, is_deleted: numpy.array=None, vcf_evidence: dict=None):
         '''Constructor for the Gene object.
 
         Args:
             name (str, optional): Name of the gene. Defaults to None
             nucleotide_sequence (numpy.array, optional): Numpy array of the nucleotide sequence. Defaults to None
             nucleotide_index (numpy.array, optional): Numpy array of the gene indices. Defaults to None
             nucleotide_number (numpy.array, optional): Numpy array of the gene numbering. Defaults to None
@@ -28,18 +29,22 @@
             indel_length (numpy.array, optional): Numpy array denoting the lengths of the indels whenever is_indel==True. Defaults to None
             indel_nucleotides (numpy.array, optional): Numpy array describing the nucleotides inserted or deleted whenever is_indel==True. Defaults to None
             reverse_complement (boolean, optional): Boolean showing whether this gene is reverse complement. Defaults to False
             codes_protein (boolean, optional): Boolean showing whether this gene codes a protein. Defaults to True
             feature_type (str, optional): The name of the type of feature that this gene represents. Defaults to None
             ribosomal_shifts (list(int), optional): Indices of repeated bases due to ribosomal frame shifting. Defaults to []
             minority_populations ([int, str, str|(str,str), int, float], optional): List of minor populations. Each minor population is defined as [position, type, bases - either str or tuple of (ref, alt), depth supporting this, fractional read support]
+            is_deleted (numpy.array, optional): Numpy array of booleans showing if a given nucleotide index is deleted. Defaults to None
+            vcf_evidence (dict, optional): Dictionary tracking genome indices which have VCF evidence to support these calls. Defaults to None
         '''
         #Using [] as a default value is dangerous, so convert from None
         if ribosomal_shifts is None:
             ribosomal_shifts = []
+        if is_deleted is None:
+            is_deleted = [i for i in nucleotide_index]
 
         assert name is not None, "must provide a gene name!"
         assert isinstance(name, str)
         self.name=name
 
         assert isinstance(feature_type, str)
         self.feature_type=feature_type
@@ -63,32 +68,43 @@
         assert len(nucleotide_index) == len(nucleotide_sequence), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(nucleotide_number), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(is_cds), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(is_promoter), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(is_indel), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(indel_length), 'all inputs arrays must be the same length!'
         assert len(nucleotide_index) == len(indel_nucleotides), 'all inputs arrays must be the same length!'
+        assert len(nucleotide_index) == len(is_deleted), 'all inputs arrays must be the same length!'
 
         nucleotide_sequence = numpy.char.lower(nucleotide_sequence)
         assert numpy.count_nonzero(numpy.isin(nucleotide_sequence,['a','t','c','g','x','z','o']))==len(nucleotide_sequence), name+": sequence can only contain a,t,c,g,z,x"
 
         self.nucleotide_sequence = nucleotide_sequence
         self.nucleotide_index = nucleotide_index
         self.nucleotide_number = nucleotide_number
         self.is_cds = is_cds
         self.is_promoter = is_promoter
         self.is_indel = is_indel
         self.indel_nucleotides = indel_nucleotides
         self.indel_length = indel_length
         self.minority_populations = [] if minority_populations is None else minority_populations
+        self.is_deleted = is_deleted
+        self.vcf_evidence = {} if vcf_evidence is None else vcf_evidence
+
+        self.minor_nc_changes = {}
+
+        #Track the original nucleotide position of each indel if this gene is revcomp
+        self.revcomp_indel_nc_index = {}
+
 
         #As revcomp changes some of the positions for indels, track separately
         # so we can track the genome position they came from
         self.indel_index = copy.deepcopy(self.nucleotide_index)
 
+        self.__adjust_dels()
+
         #Make appropriate changes to the arrays to encorporate the frame shift
         for shift in ribosomal_shifts:
             self.__duplicate(shift)
         if self.reverse_complement:
             self.nucleotide_sequence=self._complement(self.nucleotide_sequence[::-1])
             self.nucleotide_index=self.nucleotide_index[::-1]
             self.nucleotide_number=self.nucleotide_number[::-1]
@@ -134,14 +150,46 @@
                 else:
                     #Is an indel so a little more complex
                     bases = ''.join(self._complement(bases))[::-1]
                     if type_ == "del":
                         pos = pos - len(bases) + 1
             fixed.append([pos, type_, bases, pop[3], pop[4]])
         self.minority_populations = sorted(fixed, key= lambda x: x[0])
+    
+    def __adjust_dels(self) -> None:
+        '''Adjust some of the deletions, such as deletions starting/ending in another gene. 
+        Also adjust the vcf evidences so they aren't present unless it is the start of the del
+        '''
+        #Starting in another gene
+        if self.is_deleted[0] and self.indel_length[0] == 0:
+            #Find first N contiguous deletions
+            n = 0
+            for i in self.is_deleted:
+                if not i:
+                    break
+                n += 1
+            self.indel_length[0] = -1 * n
+            self.indel_nucleotides[0] = ''.join(self.nucleotide_sequence[:n])
+        
+        #Ending in another (truncating indel_length)
+        for idx, indel in enumerate(self.indel_length):
+            if indel < 0 and -1 * indel > len(self.indel_length[idx :]):
+                #Too long so truncate
+                self.indel_length[idx] = -1 * len(self.indel_length[idx:])
+                self.indel_nucleotides[idx] = ''.join(self.nucleotide_sequence[idx:])
+        
+        #Clean up vcf_evidences so only the start of a del has the evidence (to avoid erroneous evidences)
+        for i, (deleted, length) in enumerate(zip(self.is_deleted, self.indel_length)):
+            if deleted and length >= 0:
+                #Deleted but this isn't the start
+                nucleotide_index = self.nucleotide_index[i]
+                if self.vcf_evidence.get(nucleotide_index, None) is not None:
+                    #Delete if exists
+                    del self.vcf_evidence[nucleotide_index]
+            
 
     def minority_populations_GARC(self, interpretation: str='reads', reference=None) -> [str]:
         '''Fetch the mutations caused by minority populations in GARC
 
         Args:
             interpretation (str, optional): Which way to interpret the coverage calls. 'reads' gives absolute read coverage. 'percentage' gives fractional read support. Defaults to 'reads'.
             reference (gumpy.Gene, optional): The reference to denote mutations from. Defaults to self.
@@ -158,91 +206,86 @@
         
         #Make sure we have a reference to compare against
         if reference is None:
             reference = self
         else:
             assert len(reference.minority_populations) == 0, "Minority populations can only be compared when 1 Gene does not have them!"
 
-        if self.codes_protein:
-            #Copy the codons to allow minor changes
-            minor_codons = copy.deepcopy(self.codons)
-            #Set an arbitrarily high default coverage (we care about smallest available)
-            codon_cov = [9999999 for i in minor_codons]
-        mutations = []
+        #Map gene_position-->[minor populations at this position]
+        #This also groups codons together
+        gene_pos_map = defaultdict(list)
         for population in self.minority_populations:
-            pos = population[0]
-            type_ = population[1]
-            bases = population[2]
-            cov = population[coverage]
-            if type_ in ['ins', 'del']:
-                #Indels don't need any special treatment
-                mutations.append(f"{self.name}@{pos}_{type_}_{bases}:{cov}")
+            pos = self.gene_position[self.nucleotide_number == population[0]][0]
+            gene_pos_map[pos].append(population)
+        
+        mutations = []
+        for gene_pos in gene_pos_map.keys():
+            populations = gene_pos_map[gene_pos]
+            #As these don't have alt codons for Z calls, track the number of nucleotide changes separately
+            nc_changes = len([i for i in populations if i[1] == 'snp'])
+            if len(populations) == 1:
+                #We have exactly one so return it
+                pos, type_, bases, cov, frs = populations[0]
+                if type_ == "snp":
+                    if self.codes_protein and gene_pos > 0:
+                        self.minor_nc_changes[gene_pos] = nc_changes
+                        #Get the ref codon to build the ref/alt AAs
+                        ref_codon = list(reference.codons[self.amino_acid_number == gene_pos][0])
+                        codon_idx = (pos-1) % 3
+                        alt_codon = copy.deepcopy(ref_codon)
+                        alt_codon[codon_idx] = bases[1]
+                        ref = self.codon_to_amino_acid[''.join(ref_codon)]
+                        alt = self.codon_to_amino_acid[''.join(alt_codon)]
+                        mutations.append(ref + str(gene_pos) + alt + ":" + str(populations[0][coverage]))
+                    else:
+                        self.minor_nc_changes[pos] = nc_changes
+                        ref = reference.nucleotide_sequence[self.nucleotide_number == pos][0]
+                        alt = bases[1]
+                        mutations.append(ref + str(pos) + alt + ":" + str(populations[0][coverage]))
+                else:
+                    self.minor_nc_changes[pos] = nc_changes
+                    mutations.append(str(pos) + "_" + type_ + "_" + bases + ":" + str(populations[0][coverage]))
             else:
-                #Check for coding as those need extra support
-                if self.codes_protein and pos > 0:
-                    #Find the codon and change the right nucleotide
-                    codon_idx = self.codon_number[self.codon_number == (pos+2)//3][0] - 1
-                    codon = list(minor_codons[codon_idx])
-                    #Index within the codon
-                    p = (pos % 3) - 1
-                    #Update codon
-                    codon[p] = bases[1]
-                    codon = ''.join(codon)
-                    minor_codons[codon_idx] = codon
-
-                    #Update codon cov as req
-                    if codon_cov[codon_idx] > cov:
-                        codon_cov[codon_idx] = cov
+                self.minor_nc_changes[gene_pos] = nc_changes
+                #We have a mixture here so report as Zs
+                #Other than if we have conflicting indels at a gene index (in that case, crash)
+                c = Counter([(nc_idx, type_) for nc_idx, type_, bases, cov, frs in gene_pos_map[gene_pos]])
+                for (i, t), count in c.items():
+                    if t in ["ins", "del"] and count > 1:
+                        #We have a single index with > 1 indel so complain
+                        assert False, f"A minor population exists in gene {self.name} which has > 1 indel at gene index {i}!"
+                
+                cov = max([pop[coverage] for pop in populations])
+                if self.codes_protein and gene_pos > 0:
+                    #These need a little extra effort to pull out the ref AA
+                    ref = self.codon_to_amino_acid[reference.codons[self.amino_acid_number == gene_pos][0]]
+                    mutations.append(ref + str(gene_pos) + "Z:" + str(cov))
                 else:
-                    #Not coding, so just SNPs
-                    ref = reference.nucleotide_sequence[reference.nucleotide_number == pos][0]
-                    #We don't care if these are synonymous
-                    if ref == bases[1]:
-                        continue
-                    mutations.append(f"{self.name}@{ref}{pos}{bases[1]}:{cov}")
-        
-        if self.codes_protein:
-            #Now check for codon changes
-            for (i, (minor, original)) in enumerate(zip(minor_codons, self.codons)):
-                if minor != original:
-                    #We have a minor AA change!
-                    #Check to make sure this is also different from the reference
-                    ref_codon = reference.codons[i]
-                    if minor != ref_codon:
-                        minor_aa = self.codon_to_amino_acid[minor]
-                        original_aa = reference.codon_to_amino_acid[ref_codon]
-
-                        if original_aa == minor_aa:
-                            #Synonymous so find nucleotide changes and form a multi
-                            synon = f"{self.name}@{i+1}=:{codon_cov[i]}"
-                            for j, (ref, alt) in enumerate(zip(ref_codon, minor)):
-                                if ref != alt:
-                                    synon += f"&{self.name}@{ref}{i * 3 + 1 + j}{alt}:{codon_cov[i]}"
-                            mutations.append(synon)
-                        else:
-                            #Non-synonymous
-                            mutations.append(f"{self.name}@{original_aa}{i+1}{minor_aa}:{codon_cov[i]}")
+                    ref = reference.nucleotide_sequence[self.gene_position == gene_pos][0]
+                    mutations.append(ref + str(gene_pos) + "z:" + str(cov))
+                    
         return sorted(mutations)
 
 
         
     def __revcomp_indel(self) -> None:
-        '''Make some adjustments for deletions within revcomp genes
-        The largest of which is that the gene position of the deletion needs adjusting for revcomp
-        In a normal gene, the position x says delete to the left y bases
-        In a revcomp gene we want to say the position x says delete to the right y bases
-        So the pos needs changing, and indel_nucleotides need revcomping
+        '''Make some adjustments for deletions within revcomp genes. 
+        The largest of which is that the gene position of the deletion needs adjusting for revcomp. 
+        In a normal gene, the position x says delete to the left y bases. 
+        In a revcomp gene we want to say the position x says delete to the right y bases. 
+        So the pos needs changing, and indel_nucleotides need revcomping. 
 
-        Because its going the opposite direction, the same indel will refer to a different nucleotide position
+        Because its going the opposite direction, the same indel will refer to a different nucleotide position.
         '''
         #Reverse the indel arrays
         is_indel=self.is_indel[::-1]
         indel_length=self.indel_length[::-1]
         indel_nucleotides = self.indel_nucleotides[::-1]
         fixed_indel_index = self.indel_index[::-1]
+        self.is_deleted = self.is_deleted[::-1]
 
         #Check for positions where there actually is an indel
         positions = numpy.where(indel_length != 0)
         if len(positions) == 1 and len(positions[0]) == 0:
             #No indels to adjust, so return
             self.is_indel = is_indel
             self.indel_length = indel_length
@@ -252,29 +295,34 @@
         #Fixed arrays to avoid collision cases
         fixed_indel_nucleotides = numpy.array([None for i in self.indel_nucleotides])
         fixed_is_indel = numpy.array([False for i in is_indel])
         fixed_indel_length = numpy.array([0 for i in indel_length])
         for pos in positions[0]:
             if indel_length[pos] > 0:
                 #An insertion at this pos so only revcomp the inserted bases
-                fixed_indel_nucleotides[pos] = ''.join(self._complement(indel_nucleotides[pos][::-1]))
+                #Because this is backwards now, pos needs adjusting to point to the right base for inserting after
+                old_pos = pos
+                pos = pos - 1
+                fixed_indel_nucleotides[pos] = ''.join(self._complement(indel_nucleotides[old_pos][::-1]))
                 fixed_is_indel[pos] = True
-                fixed_indel_length[pos] = indel_length[pos]
+                fixed_indel_length[pos] = indel_length[old_pos]
+                self.vcf_evidence[self.nucleotide_index[pos]] = self.vcf_evidence[self.nucleotide_index[old_pos]]
+                del self.vcf_evidence[self.nucleotide_index[old_pos]]
+                self.revcomp_indel_nc_index[str(self.nucleotide_number[pos])] = str(self.nucleotide_index[old_pos])
             else:
                 #A deletion at this pos so adjust position
                 new_pos = pos - len(indel_nucleotides[pos]) + 1
-                if new_pos < 0:
-                    #This is an issue because this lies outside of the gene now
-                    #So just retain the deletions within this gene, and mark to be at the start
-                    indel_nucleotides[pos] = indel_nucleotides[pos][:pos+1]
-                    new_pos = 0
                 fixed_indel_nucleotides[new_pos] = ''.join(self._complement(indel_nucleotides[pos][::-1]))
-                fixed_is_indel[new_pos] = True
+                #Only set is_indel if it was set before 
+                #In cases of large deletions, we don't want this set
+                if is_indel[pos]:
+                    fixed_is_indel[new_pos] = True
                 fixed_indel_length[new_pos] = indel_length[pos]
                 fixed_indel_index[new_pos] = fixed_indel_index[pos]
+                self.revcomp_indel_nc_index[str(self.nucleotide_number[new_pos])] = str(self.nucleotide_index[pos])
 
         #Update instance variables
         self.is_indel = fixed_is_indel
         self.indel_length = fixed_indel_length
         self.indel_nucleotides = fixed_indel_nucleotides
         self.indel_index = fixed_indel_index
                 
@@ -349,15 +397,15 @@
 
         return check
 
     @staticmethod
     def _complement(nucleotides_array: [str]) -> numpy.array:
         """Simple private method for returning the complement of an array of bases.
 
-        Note that takes account of HET and NULL calls via z and x, respectively
+        * Note that takes account of HET and NULL calls via z and x, respectively
 
         Args:
             nucleotides_array (Iterable(str)): Some iterable of nucleotide bases. Usually a numpy.array or list
         
         Returns:
             numpy.array: Array of complemented bases
         """
@@ -492,15 +540,15 @@
                 #Valid minority population, so continue without it
                 variant = variant[0]
             else:
                 return False
 
         #Match promoter/non-coding SNP format
         promoter = re.compile(r"""
-                ([a-zA-Z_0-9]+@)? #Possibly a leading gene name
+                ([a-zA-Z_0-9.()]+@)? #Possibly a leading gene name
                 ([acgtzx]) #Reference base
                 (-?[0-9]+) #Position
                 ([acgtzx]) #Alt base
                 """, re.VERBOSE)
         if promoter.fullmatch(variant):
             #The variant is either promoter or non-coding
             #Check that the mutation is valid
@@ -514,15 +562,15 @@
             #Check that the ref matches the seq at the given pos
             valid = valid and self.nucleotide_sequence[self.nucleotide_number == int(pos)] == ref
             #Mutation should not have same ref and alt
             valid = valid and ref != alt
             return valid
         #Match amino acid SNP
         snp = re.compile(r"""
-                    ([a-zA-Z_0-9]+@)? #Possibly leading gene name
+                    ([a-zA-Z_0-9.()]+@)? #Possibly leading gene name
                     ([A-Z!]) #Reference amino acid
                     ([0-9]+) #Position
                     ([A-Z!]) #Alt amino acid
                     """, re.VERBOSE)
         if self.codes_protein and snp.fullmatch(variant):
             #The variant is an amino acid SNP
             #Check it is valid
@@ -535,15 +583,15 @@
             valid = valid and int(pos) in self.amino_acid_number
             #Check ref matches the aa seq at the given pos
             valid = valid and self.amino_acid_sequence[self.amino_acid_number == int(pos)] == ref
             return valid
 
         #Match amino acid synon-mutation
         synon = re.compile(r"""
-                        ([a-zA-Z_0-9]+@)? #Possibly leading gene name
+                        ([a-zA-Z_0-9.()]+@)? #Possibly leading gene name
                         ([0-9]+) #Pos
                         = #Synonymous amino acid
                         """, re.VERBOSE)
         if self.codes_protein and synon.fullmatch(variant):
             #Variant is a synonymous mutation
             #Check it is valid
             name, pos = synon.fullmatch(variant).groups()
@@ -551,15 +599,15 @@
             if name is not None and name != "":
                 valid = valid and name[:-1] == self.name
             valid = valid and int(pos) in self.amino_acid_number
             return valid
 
         #Match indel
         indel = re.compile(r"""
-                    ([a-zA-Z_0-9]+@)? #Possibly leading gene name
+                    ([a-zA-Z_0-9.()]+@)? #Possibly leading gene name
                     (-?[0-9]+) #Position
                     _(ins|del|indel)_? #Type
                     ([0-9]+|[acgtzx]+)? #Bases deleted/inserted
                     """, re.VERBOSE)
         if indel.fullmatch(variant):
             #Variant is an indel
             #Check it is valid
@@ -601,9 +649,23 @@
                             continue
                         valid = valid and int(pos)+index+offset in self.nucleotide_number
                         valid = valid and self.nucleotide_sequence[self.nucleotide_number == int(pos)+index+offset] == base
             if type_ == "ins":
                 #Just check that the position specified lies within the gene
                 valid = valid and pos in self.nucleotide_number
             return valid
+        #Checking for percentage deletion
+        deletion = re.compile(r"""
+                            ([a-zA-Z_0-9.()]+@)? #Possibly leading gene name
+                            del_ #Deletion
+                            ([01]\.[0-9]+)
+                            """, re.VERBOSE)
+        if deletion.fullmatch(variant):
+            name, percent = deletion.fullmatch(variant).groups()
+            valid = True
+            if name is not None:
+                valid = valid and name[:-1] == self.name
+            percent = float(percent)
+            valid = valid and percent <= 1 and percent >= 0
+            return valid
         #If none of the mutations have matched, return False
         return False
```

### Comparing `gumpy-1.1.0/gumpy/genome.py` & `gumpy-1.2.0/gumpy/genome.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         '''
 
         assert isinstance(other, Genome), 'RHS must be a gumpy.Genome object'
 
         return(GenomeDifference(self,other))
 
     def __eq__(self, other) -> bool:
-        '''Overloading the equality operator so two Genome objects can be compared directly
+        '''Overloading the equality operator so two Genome objects can be compared directly. 
         Checks for the equality based on fields, but does not check for filename equality
         Args:
             other (gumpy.Genome) : The other Genome object to compare to
         Returns:
             bool : Boolean showing equality of the objects
         '''
         assert isinstance(other, Genome)
@@ -508,15 +508,15 @@
             self.stacked_is_reverse_complement[i][start-1:end-1] = True
         else:
             self.stacked_nucleotide_number[i][start-1:end-1] = numpy.mod(1+self.nucleotide_index[start-1:end-1]-start,self.length)
 
     def __fit_gene(self, mask: numpy.array, genes: numpy.array, genes_mask: numpy.array, start: int, end: int, gene_name: str, rev_comp: bool) -> (numpy.array, numpy.array):
         '''
         Private function to fit a gene into the genes based on the dot product of the masks
-            numpy.dot([bool], [bool])-> bool showing if there are collisions of True values within args
+            numpy.dot([bool], [bool])-> bool showing if there are collisions of True values within args.
             This takes 10^-5 seconds which is a significant improvement on use of numpy.all() iteration of 10^-2 seconds for TB length genome
         Args:
             mask (numpy.array) : Boolean array showing positions where the gene lies
             genes (numpy.array) : 2D numpy array of the format used for all stacked values
             genes_mask (numpy.array) : The corresponding boolean mask arrays for the `genes` arg
             start (int) : Start index of the gene
             end (int) : End index of the gene
@@ -545,17 +545,17 @@
         genes = numpy.vstack((genes, new_row))
         i += 1
         self.__handle_rev_comp(rev_comp, start, end, i)
         return genes_mask, genes, i
 
     def __find_overlaps(self):
         '''
-        Private function to find the sections of the genome in which there are overlapping genes
-        This should be more efficient than the older version as it avoids consistent genome iteration
-        Use of the dot product on boolean arrays returns a single boolean showing collisions in almost constant time (10^-5 secs for TB size)
+        Private function to find the sections of the genome in which there are overlapping genes. 
+        This should be more efficient than the older version as it avoids consistent genome iteration. 
+        Use of the dot product on boolean arrays returns a single boolean showing collisions in almost constant time (10^-5 secs for TB size). 
             This can be used to determine which row the gene should be in
         '''
 
         # Boolean mask to show gene presence at indicies (default to all False values)
         genes_mask = numpy.array([numpy.array([False for x in range(self.length)])])
 
         # gene names
@@ -608,14 +608,20 @@
         self.stacked_nucleotide_index=numpy.tile(self.nucleotide_index,(self.n_rows,1))
 
         self.stacked_nucleotide_sequence=numpy.tile(self.nucleotide_sequence,(self.n_rows,1))
 
         #Use a list to track minority populations
         self.minor_populations = []
 
+        #Track which nucleotides are deleted
+        self.is_deleted = numpy.array([False for i in self.nucleotide_index])
+
+        #Use a dict to track VCF evidence as req
+        self.vcf_evidence = dict()
+
     def __assign_promoter_regions(self):
         '''
         Private function to assign promoter regions to genes
         '''
         assert isinstance(self.max_promoter_length,int), 'max_promoter_length must be an integer!'
 
         assert self.max_promoter_length>0, 'max_promoter_length must be greater than zero'
@@ -726,33 +732,60 @@
         
         gene_nucleotides = self.nucleotide_index[mask]
         gene_minor_populations = []
         for population in self.minor_populations:
             if population[0] in gene_nucleotides:
                 #This minor population is within the gene
                 gene_minor_populations.append(population)
-
+        
+        vcf_evidence = {idx : self.vcf_evidence[idx] for idx in self.vcf_evidence.keys() if idx in gene_nucleotides}
+            
         # instantiate a Gene object
         g = Gene(name=gene,
                     nucleotide_sequence=nucleotide_seq,
                     nucleotide_index=gene_nucleotides,
                     nucleotide_number=self.stacked_nucleotide_number[stacked_mask],
                     is_cds=is_cd,
                     is_promoter=self.stacked_is_promoter[stacked_mask],
                     is_indel=self.is_indel[mask],
                     indel_length=self.indel_length[mask],
                     indel_nucleotides=self.indel_nucleotides[mask],
                     codes_protein=self.genes[gene]['codes_protein'],
                     reverse_complement=self.genes[gene]['reverse_complement'],
                     feature_type=self.genes[gene]['type'],
                     ribosomal_shifts=self.genes[gene]['ribosomal_shifts'],
-                    minority_populations=gene_minor_populations
+                    minority_populations=gene_minor_populations,
+                    is_deleted=self.is_deleted[mask],
+                    vcf_evidence=vcf_evidence
                 )
 
         return g
+    
+    def __assign_deleted(self, genome) -> None:
+        '''Assign a boolean array of which nucleotides are deleted by indels.
+        This holds the same 1-1 relationship as nucleotide_index <-> nucleotide_sequence
+
+        Args:
+            genome (gumpy.Genome): Genome to apply this to
+        '''
+        marking = 0
+        current_evidence = None
+        for idx, length in enumerate(genome.indel_length):
+            if length < 0:
+                #We found a deletion, so mark the next N bases as deleted
+                #Deletions are -N here
+                marking -= length
+                current_evidence = genome.vcf_evidence[genome.nucleotide_index[idx]]
+
+            if marking > 0:
+                #We mark this as deleted
+                genome.is_deleted[idx] = True
+                #Update evidence too so we can pull out VCF rows from downstream genes
+                genome.vcf_evidence[genome.nucleotide_index[idx]] = current_evidence
+                marking -= 1
 
     def __add__(self, vcf: VCFFile):
         '''Function to apply a VCF file to the genome  - producing a replica genome with the specified changes
 
         Args:
             vcf (gumpy.VCFFile): The VCFFile object for the VCF
 
@@ -789,14 +822,15 @@
         '''
 
         if self.verbose:
             print("Updating the genome...")
 
         # use the calls dict to change the nucleotide indicies in the copy of the genome
         for (idx,type_) in tqdm(vcf.calls.keys(), disable=(not self.show_progress_bar)):
+            genome.vcf_evidence[genome.nucleotide_index[idx-1]] = vcf.calls[(idx, type_)]['original_vcf_row']
 
             # deal with changes at a single nucleotide site
             if type_ in ['snp','null','het']:
                 # only set values if the idx is to a single nucleotide
                 genome.nucleotide_sequence[idx-1] = vcf.calls[(idx,type_)]['call']
 
             # deal with insertions and deletions
@@ -812,14 +846,18 @@
             
             elif type_ == 'ref':
                 #These only exist due to reference calls
                 #They only made it this far as they are required to pull out minors at these positions
                 pass
 
         genome.minor_populations = vcf.minor_populations
+        genome.vcf_file = vcf
+
+        #Let's assign some deleted regions (if exist)
+        self.__assign_deleted(genome)
 
         # the genome has been altered so not a reference genome
         genome.is_reference = False
 
         return genome
 
     def minority_populations_GARC(self, interpretation: str='reads', reference=None) -> [str]:
```

### Comparing `gumpy-1.1.0/gumpy/variantfile.py` & `gumpy-1.2.0/gumpy/variantfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 '''
 Classes used to parse and store VCF data
 '''
 import copy
 import pathlib
+import warnings
 from collections import defaultdict
 
 import numpy
 import pandas
 import pysam
 
 
 class VCFRecord(object):
     '''
-    Class for VCF records
-    Instance variables:
-        `chrom` (str): Name of the sample.
-        `pos` (int): Genome index for the change.
-        `ref` (str): Reference value for the nucleotide.
-        `alts` (tuple(str)): Alternative calls. Tuple can contain single values and indels.
-        `qual` (None): Values for quality (values other than None have yet to be found in testing files...).
-        `filter` (str): Whether this record has pass the filter.
-        `info` (dict): Dictionary of key->value for the info fields.
-        `values` (dict): Dictionary of key->value for the values. Usually this is the FORMAT field names with their corresponding values.
-        `is_filter_pass` (bool): does the filter column contain PASS?
-        `call1` (int): the index of the first call
-        `call2` (int): the index of the second call
-        `is_reference` (bool): is the call for the reference?
-        `is_null` (bool): is the call a null call?
-        `is_heterozygous` (bool): is it a is_heterozygous call i.e. call1!=call2?
-        `is_alt` (bool): or, is the call for a single specified alt
+    * Class for VCF records
+    * Instance variables:
+        * `chrom` (str): Name of the sample.
+        * `pos` (int): Genome index for the change.
+        * `ref` (str): Reference value for the nucleotide.
+        * `alts` (tuple(str)): Alternative calls. Tuple can contain single values and indels.
+        * `qual` (None): Values for quality (values other than None have yet to be found in testing files...).
+        * `filter` (str): Whether this record has pass the filter.
+        * `info` (dict): Dictionary of key->value for the info fields.
+        * `values` (dict): Dictionary of key->value for the values. Usually this is the FORMAT field names with their corresponding values.
+        * `is_filter_pass` (bool): does the filter column contain PASS?
+        * `call1` (int): the index of the first call
+        * `call2` (int): the index of the second call
+        * `is_reference` (bool): is the call for the reference?
+        * `is_null` (bool): is the call a null call?
+        * `is_heterozygous` (bool): is it a is_heterozygous call i.e. call1!=call2?
+        * `is_alt` (bool): or, is the call for a single specified alt
     '''
     def __init__(self, record: pysam.libcbcf.VariantRecord, sample: str):
         '''Constructor for the VCFRecord object.
 
         Parses the supplied pysam object and presents in a more Pythonic format
 
         Args:
@@ -80,14 +81,15 @@
                 self.is_null = True if set([self.call1, self.call2]) == {-1} else False
                 self.is_alt = True if not self.is_reference and not self.is_heterozygous and not self.is_null else False
 
             #Due to how pysam reads floats, there are some erroneously long dps, so round
             elif isinstance(item,float):
                 item = round(item, 3)
             self.values[key] = item
+        self.values['POS'] = self.pos
 
     def __repr__(self) -> str:
         '''Pretty print the record
 
         Returns:
             str: String representation of the record
         '''
@@ -100,45 +102,50 @@
         else:
             s+=str(self.qual)+'\t'
         if self.filter == None:
             s+='.\t'
         else:
             s+=self.filter+'\t'
         for val in self.values.keys():
+            if val == "POS":
+                continue
             s += str(val)+":"
         s = s[:-1] + "\t"
-        for val in self.values.values():
+        for key in self.values.keys():
+            val = self.values[key]
+            if key == "POS":
+                continue
             s += str(val)+":"
         s = s[:-1]
         s += "\n"
         return s
 
 class VCFFile(object):
     '''
-    Class to instanciate a variant file (VCF)
-    Used to apply a VCF file to a genome
-    Instance variables:
-        `filename` (str): path to the VCF file
-        `vcf_version` (tuple(int)): Tuple of ints to show the VCF version of the file. e.g 3.2 would be (3, 2).
-        `contig_lengths` (dict): Dictionary mapping contig_name->length for all defined contigs.
-        `format_fields_description` (dict): Dictionary mapping format_name->dict(description, id, type).
-        `records` (list(VCFRecord)): List of VCFRecord objects for each record within the file.
-        `calls` (dict): Dict of definite calls made in the VCF file, after any additional filtering has been applied
-        `ignore_filter` (bool): whether to ignore the FILTER in the VCF file
-        `format_fields_min_thresholds` (dict): dictionary specifying minimum thresholds to be applied to fields in the FORMAT field e.g. {'GTCONF':5}
-        `variants` (numpy.array): Numpy array of the detected variants in the VCF file
-        `nucleotide_index` (numpy.array): Array of genome indices which are affected by the VCF
-        `ref_nucleotides` (numpy.array): Array of REF bases
-        `alt_nucleotides` (numpy.array): Array of ALT bases
-        `indel_length` (numpy.array): Array of lengths of insertions (+ve) or deletions (-ve) at each site
-        `is_snp` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are SNPs
-        `is_het` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are heterozygous calls
-        `is_null` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are null calls
-        `is_indel` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are indel calls
-        `snp_distance` (int): SNP distance caused by the VCF
+    * Class to instanciate a variant file (VCF)
+    * Used to apply a VCF file to a genome
+    * Instance variables:
+        * `filename` (str): path to the VCF file
+        * `vcf_version` (tuple(int)): Tuple of ints to show the VCF version of the file. e.g 3.2 would be (3, 2).
+        * `contig_lengths` (dict): Dictionary mapping contig_name->length for all defined contigs.
+        * `format_fields_description` (dict): Dictionary mapping format_name->dict(description, id, type).
+        * `records` (list(VCFRecord)): List of VCFRecord objects for each record within the file.
+        * `calls` (dict): Dict of definite calls made in the VCF file, after any additional filtering has been applied
+        * `ignore_filter` (bool): whether to ignore the FILTER in the VCF file
+        * `format_fields_min_thresholds` (dict): dictionary specifying minimum thresholds to be applied to fields in the FORMAT field e.g. {'GTCONF':5}
+        * `variants` (numpy.array): Numpy array of the detected variants in the VCF file
+        * `nucleotide_index` (numpy.array): Array of genome indices which are affected by the VCF
+        * `ref_nucleotides` (numpy.array): Array of REF bases
+        * `alt_nucleotides` (numpy.array): Array of ALT bases
+        * `indel_length` (numpy.array): Array of lengths of insertions (+ve) or deletions (-ve) at each site
+        * `is_snp` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are SNPs
+        * `is_het` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are heterozygous calls
+        * `is_null` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are null calls
+        * `is_indel` (numpy.array): Array to act as a mask for `nucleotide_index` to show which are indel calls
+        * `snp_distance` (int): SNP distance caused by the VCF
     '''
     def __init__(self, filename: str, ignore_filter: bool=False, bypass_reference_calls: bool=False, format_fields_min_thresholds: {str: int}=None, minor_population_indices: {int}=None):
         '''
         Constructor for the VCFFile object.
 
         Parses the VCF file using pysam.
 
@@ -250,28 +257,28 @@
             output += str(self.records[-1])
         else:
             for record in self.records:
                 output += str(record)+'\n'
         return output
     
     def _find_minor_populations(self):
-        '''Find the minor populations for this VCF based on the minor population positions given
+        '''Find the minor populations for this VCF based on the minor population positions given. 
         Deconstructs these into actual mutations of SNP/INDEL too as this logic already exists here
 
-        Minor populations are intentionally kept very separate from other variants.
-        They are very infrequent compared to other variants so storing in similar structures would be resource heavy.
-        They are instead stored consistently in the form of calls:
-            [position, type, bases, depth, frs]
-            position: Genome position (or Gene position if within genes)
-            type: String denoting type of variant. One of ['ref', 'snp', 'ins', 'del']
-            bases: Descripton of the bases.
-                If type in ['ref', 'snp'], of the format (ref base, alt base)
-                If type in ['ins', 'del'], string of the bases inserted or deleted
-            depth: number of reads supporting this call
-            frs: fractional read support (i.e depth/total coverage at this point)
+        * Minor populations are intentionally kept very separate from other variants.
+        * They are very infrequent compared to other variants so storing in similar structures would be resource heavy.
+        * They are instead stored consistently in the form of calls:
+            * [position, type, bases, depth, frs]
+                * position: Genome position (or Gene position if within genes)
+                * type: String denoting type of variant. One of ['ref', 'snp', 'ins', 'del']
+                * bases: Descripton of the bases.
+                    * If type in ['ref', 'snp'], of the format (ref base, alt base)
+                    * If type in ['ins', 'del'], string of the bases inserted or deleted
+                * depth: number of reads supporting this call
+                * frs: fractional read support (i.e depth/total coverage at this point)
         '''
         self.minor_populations = []
         simple_calls = []
         for (idx, type_) in self.calls.keys():
             #Get the simple format of this call for comparison
             if isinstance(self.calls[(idx, type_)]['call'], tuple):
                 #Indels
@@ -289,14 +296,20 @@
         for (idx, type_) in self.calls.keys():
             #Check if we've delt with this vcf already
             if self.calls[(idx, type_)]['original_vcf_row'] in seen:
                 continue
             else:
                 seen.append(self.calls[(idx, type_)]['original_vcf_row'])
 
+            #Checking for het calls
+            if self.calls[(idx, type_)]['call'] == "z":
+                if 0 not in self.calls[(idx, type_)]['original_vcf_row']['GT']:
+                    #Het call without a wildtype call, so warn about weird behaviour
+                    warnings.warn(f"Minor population detected at position {idx}, which doesn't include a wildtype call. Call: {self.calls[(idx, type_)]['original_vcf_row']['GT']}. Note that there may be multiple mutations given at this index", UserWarning)
+
             #Reference base(s)
             ref = self.calls[(idx, type_)]['original_vcf_row']["REF"]
 
             #Get all of the calls
             calls = [self.calls[(idx, type_)]['original_vcf_row']["REF"]] + list(self.calls[(idx, type_)]['original_vcf_row']["ALTS"])
 
             #Break down the calls as appropriate
@@ -320,14 +333,17 @@
                     if depth >= 2:
                         #These are minor calls!!
                         pos = idx + int(call[0])
                         if pos not in self.minor_population_indices:
                             #We don't actually care though
                             #This has to be done here as simplifying calls can move the position
                             continue
+                        if call[1] == 'snp' and call[2][0] == call[2][1]:
+                            #Ref calls aren't interesting
+                            continue
                         #Only tracking absolute number of reads
                         self.minor_populations.append((pos, call[1], call[2], int(depth), round(depth/total_depth, 3)))
         
     def __find_calls(self):
         '''
         Private method to find changes within the genome based on the variant file.
```

### Comparing `gumpy-1.1.0/gumpy.egg-info/PKG-INFO` & `gumpy-1.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,23 @@
-Metadata-Version: 2.1
-Name: gumpy
-Version: 1.1.0
-Summary: Genetics with Numpy
-Home-page: https://github.com/oxfordmmm/gumpy
-Author: Philip W Fowler
-Author-email: philip.fowler@ndm.ox.ac.uk
-License: University of Oxford, see LICENSE.md
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Tests](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gumpy/actions/workflows/tests.yaml)
-[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) [![Documentation Status](https://readthedocs.org/projects/gumpy/badge/?version=latest)](https://gumpy.readthedocs.io/en/latest/?badge=latest) 
+[![codecov](https://codecov.io/gh/oxfordmmm/gumpy/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/gumpy) 
+[![Docs](https://github.com/oxfordmmm/gumpy/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gumpy/)
 [![PyPI version](https://badge.fury.io/py/gumpy.svg)](https://badge.fury.io/py/gumpy)
 
 # gumpy
 Genetics with Numpy
 
 ## Installation
 ```
 git clone https://github.com/oxfordmmm/gumpy
 cd gumpy
 pip install .
 ```
 ## Documentation
-Easy access to documentation for public methods can be found using the `pydoc` module from a terminal:
-```
-python -m pydoc -b gumpy
-```
-This should open a browser window showing documentation for all loaded modules. Navigating to `gumpy (package)` should bring up available files to view documentation.
-
-Docstrings contain documentation for almost all methods if documentation of private methods is required.
+https://oxfordmmm.github.io/gumpy/
 
 ## Testing
 A suite of tests can be run from a terminal:
 ```
 python -m pytest --cov=gumpy -vv
 ```
```

### Comparing `gumpy-1.1.0/setup.cfg` & `gumpy-1.2.0/setup.cfg`

 * *Files identical despite different names*

