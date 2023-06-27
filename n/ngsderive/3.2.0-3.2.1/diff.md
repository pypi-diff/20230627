# Comparing `tmp/ngsderive-3.2.0.tar.gz` & `tmp/ngsderive-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngsderive-3.2.0.tar", max compression
+gzip compressed data, was "ngsderive-3.2.1.tar", max compression
```

## Comparing `ngsderive-3.2.0.tar` & `ngsderive-3.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1077 2023-06-26 14:48:03.089408 ngsderive-3.2.0/LICENSE.md
--rw-r--r--   0        0        0     4846 2023-06-26 14:48:03.089408 ngsderive-3.2.0/README.md
--rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/__init__.py
--rwxr-xr-x   0        0        0     9781 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/__main__.py
--rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/__init__.py
--rw-r--r--   0        0        0     2482 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/encoding.py
--rwxr-xr-x   0        0        0     9658 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/instrument.py
--rw-r--r--   0        0        0    11008 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/junction_annotation.py
--rwxr-xr-x   0        0        0     2260 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/readlen.py
--rwxr-xr-x   0        0        0    11914 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/strandedness.py
--rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/readers/__init__.py
--rwxr-xr-x   0        0        0       13 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/readers/bam.py
--rwxr-xr-x   0        0        0    14826 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/utils.py
--rw-r--r--   0        0        0     1585 2023-06-26 14:48:49.776485 ngsderive-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     5908 1970-01-01 00:00:00.000000 ngsderive-3.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-06-27 14:02:33.286389 ngsderive-3.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4846 2023-06-27 14:02:33.286389 ngsderive-3.2.1/README.md
+-rwxr-xr-x   0        0        0        0 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/__init__.py
+-rwxr-xr-x   0        0        0     9842 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/__init__.py
+-rw-r--r--   0        0        0     2455 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/encoding.py
+-rwxr-xr-x   0        0        0     9633 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/instrument.py
+-rw-r--r--   0        0        0    10970 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/junction_annotation.py
+-rwxr-xr-x   0        0        0     2230 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/readlen.py
+-rwxr-xr-x   0        0        0    11807 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/commands/strandedness.py
+-rwxr-xr-x   0        0        0        0 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/readers/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/readers/bam.py
+-rwxr-xr-x   0        0        0    14826 2023-06-27 14:02:33.286389 ngsderive-3.2.1/ngsderive/utils.py
+-rw-r--r--   0        0        0     1585 2023-06-27 14:03:11.633033 ngsderive-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5908 1970-01-01 00:00:00.000000 ngsderive-3.2.1/PKG-INFO
```

### Comparing `ngsderive-3.2.0/LICENSE.md` & `ngsderive-3.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.2.0/README.md` & `ngsderive-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.2.0/ngsderive/__main__.py` & `ngsderive-3.2.1/ngsderive/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,28 +63,28 @@
         "--majority-vote-cutoff",
         type=float,
         help="To call a majority readlen, the maximum read length must have at least `majority-vote-cutoff`%% reads in support.",
         default=0.7,
     )
     readlen.add_argument(
         "-n",
-        "--n-samples",
+        "--n-reads",
         type=int,
-        help="How many reads to sample. Any n < 1 to parse whole file.",
-        default=1000000,
+        help="How many reads to analyze from the start of the file. Any n < 1 to parse whole file.",
+        default=-1,
     )
 
     instrument = subparsers.add_parser(
         "instrument", parents=[common], formatter_class=SaneFormatter
     )
     instrument.add_argument(
         "-n",
-        "--n-samples",
+        "--n-reads",
         type=int,
-        help="How many reads to sample. Any n < 1 to parse whole file.",
+        help="How many reads to analyze from the start of the file. Any n < 1 to parse whole file.",
         default=10000,
     )
 
     strandedness = subparsers.add_parser(
         "strandedness", parents=[common], formatter_class=SaneFormatter
     )
     strandedness.add_argument(
@@ -145,17 +145,17 @@
     strandedness.set_defaults(only_protein_coding_genes=True, split_by_rg=False)
 
     encoding = subparsers.add_parser(
         "encoding", parents=[common], formatter_class=SaneFormatter
     )
     encoding.add_argument(
         "-n",
-        "--n-samples",
+        "--n-reads",
         type=int,
-        help="How many reads to sample. Any n < 1 to parse whole file.",
+        help="How many reads to analyze from the start of the file. Any n < 1 to parse whole file.",
         default=1000000,
     )
 
     junction_annotation = subparsers.add_parser(
         "junction-annotation", parents=[common], formatter_class=SaneFormatter
     )
     junction_annotation.add_argument(
@@ -276,22 +276,22 @@
     args = get_args()
     process_args(args)
 
     if args.subcommand == "readlen":
         readlen.main(
             args.ngsfiles,
             outfile=args.outfile,
-            n_samples=args.n_samples,
+            n_reads=args.n_reads,
             majority_vote_cutoff=args.majority_vote_cutoff,
         )
     if args.subcommand == "instrument":
         instrument.main(
             args.ngsfiles,
             outfile=args.outfile,
-            n_samples=args.n_samples,
+            n_reads=args.n_reads,
         )
     if args.subcommand == "strandedness":
         max_iters = args.max_iterations_per_try
         if not max_iters:
             max_iters = 10 * args.n_genes
         strandedness.main(
             args.ngsfiles,
@@ -304,15 +304,15 @@
             split_by_rg=args.split_by_rg,
             max_iterations_per_try=max_iters,
         )
     if args.subcommand == "encoding":
         encoding.main(
             args.ngsfiles,
             outfile=args.outfile,
-            n_samples=args.n_samples,
+            n_reads=args.n_reads,
         )
     if args.subcommand == "junction-annotation":
         junction_annotation.main(
             args.ngsfiles,
             args.gene_model,
             outfile=args.outfile,
             min_intron=args.min_intron,
```

### Comparing `ngsderive-3.2.0/ngsderive/commands/encoding.py` & `ngsderive-3.2.1/ngsderive/commands/encoding.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 # sets are created by doing PHRED+33 decoding of each encoding's ASCII ranges
 SANGER_SET = set([i for i in range(0, 93)])
 ILLUMINA_1_0_SET = set([i for i in range(26, 93)])
 ILLUMINA_1_3_SET = set([i for i in range(31, 93)])
 
 
-def main(ngsfiles, outfile=sys.stdout, n_samples=1000000):
+def main(ngsfiles, outfile, n_reads):
 
     writer = csv.DictWriter(
         outfile,
         fieldnames=["File", "Evidence", "ProbableEncoding"],
         delimiter="\t",
     )
     writer.writeheader()
     outfile.flush()
 
-    if n_samples < 1:
-        n_samples = None
+    if n_reads < 1:
+        n_reads = None
 
     for ngsfilepath in ngsfiles:
         try:
             ngsfile = NGSFile(ngsfilepath, store_qualities=True)
         except FileNotFoundError:
             result = {
                 "File": ngsfilepath,
@@ -40,15 +40,15 @@
                 "ProbableEncoding": "N/A",
             }
             writer.writerow(result)
             outfile.flush()
             continue
 
         score_set = set()
-        for read in itertools.islice(ngsfile, n_samples):
+        for read in itertools.islice(ngsfile, n_reads):
             score_set.update(read["quality"])
 
         highest_ascii = str(max(score_set) + 33)
         lowest_ascii = str(min(score_set) + 33)
         if score_set <= ILLUMINA_1_3_SET:
             result = {
                 "File": ngsfilepath,
```

### Comparing `ngsderive-3.2.0/ngsderive/commands/instrument.py` & `ngsderive-3.2.1/ngsderive/commands/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,25 +191,25 @@
         return (
             overlapping_instruments,
             "high confidence",
             "instrument id and flowcell id",
         )
 
 
-def main(ngsfiles, outfile=sys.stdout, n_samples=10000):
+def main(ngsfiles, outfile, n_reads):
     writer = csv.DictWriter(
         outfile,
         fieldnames=["File", "Instrument", "Confidence", "Basis"],
         delimiter="\t",
     )
     writer.writeheader()
     outfile.flush()
 
-    if n_samples < 1:
-        n_samples = None
+    if n_reads < 1:
+        n_reads = None
 
     for ngsfilepath in ngsfiles:
         try:
             ngsfile = NGSFile(ngsfilepath)
         except FileNotFoundError:
             result = {
                 "File": ngsfilepath,
@@ -224,15 +224,15 @@
 
         instruments = set()
         flowcells = set()
         malformed_read_names = False
 
         # accumulate instrument and flowcell IDs
         try:
-            for read in itertools.islice(ngsfile, n_samples):
+            for read in itertools.islice(ngsfile, n_reads):
                 parts = read["query_name"].split(":")
                 if len(parts) != 7:  # not Illumina format
                     malformed_read_names = True
                     iid = parts[0]  # attempt to recover machine name
                     instruments.add(iid)
                     for rg in ngsfile.handle.header.to_dict()["RG"]:
                         if rg["ID"] == read["read_group"]:
```

### Comparing `ngsderive-3.2.0/ngsderive/commands/junction_annotation.py` & `ngsderive-3.2.1/ngsderive/commands/junction_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,22 +252,22 @@
     }
     return result
 
 
 def main(
     ngsfiles,
     gene_model_file,
-    outfile=sys.stdout,
-    min_intron=50,
-    min_mapq=30,
-    min_reads=2,
-    fuzzy_range=0,
-    consider_unannotated_references_novel=False,
-    junction_dir="./",
-    disable_junction_files=False,
+    outfile,
+    min_intron,
+    min_mapq,
+    min_reads,
+    fuzzy_range,
+    consider_unannotated_references_novel,
+    junction_dir,
+    disable_junction_files,
 ):
     logger.info("Arguments:")
     logger.info("  - Gene model file: {}".format(gene_model_file))
     logger.info("  - Minimum intron length: {}".format(min_intron))
     logger.info("  - Minimum MAPQ: {}".format(min_mapq))
     logger.info("  - Minimum reads per junction: {}".format(min_reads))
     logger.info("  - Fuzzy junction range: +-{}".format(fuzzy_range))
```

### Comparing `ngsderive-3.2.0/ngsderive/commands/readlen.py` & `ngsderive-3.2.1/ngsderive/commands/readlen.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from ..utils import NGSFile
 
 logger = logging.getLogger("readlen")
 
 
 def main(
     ngsfiles,
-    outfile=sys.stdout,
-    n_samples=100000,
-    majority_vote_cutoff=0.7,
+    outfile,
+    n_reads,
+    majority_vote_cutoff,
 ):
 
     writer = csv.DictWriter(
         outfile,
         fieldnames=["File", "Evidence", "MajorityPctDetected", "ConsensusReadLength"],
         delimiter="\t",
     )
     writer.writeheader()
     outfile.flush()
 
-    if n_samples < 1:
-        n_samples = None
+    if n_reads < 1:
+        n_reads = None
 
     for ngsfilepath in ngsfiles:
         read_lengths = defaultdict(int)
         try:
             ngsfile = NGSFile(ngsfilepath)
         except FileNotFoundError:
             result = {
@@ -42,15 +42,15 @@
 
             writer.writerow(result)
             outfile.flush()
             continue
 
         # accumulate read lengths
         total_reads_sampled = 0
-        for read in itertools.islice(ngsfile, n_samples):
+        for read in itertools.islice(ngsfile, n_reads):
             total_reads_sampled += 1
             read_lengths[len(read["query"])] += 1
 
         read_length_keys_sorted = sorted(
             [int(k) for k in read_lengths.keys()], reverse=True
         )
         putative_max_readlen = read_length_keys_sorted[0]
```

### Comparing `ngsderive-3.2.0/ngsderive/commands/strandedness.py` & `ngsderive-3.2.1/ngsderive/commands/strandedness.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict
 
 from ..utils import NGSFile, NGSFileType, GFF
 
 logger = logging.getLogger("strandedness")
 
 
-def get_filtered_reads_from_region(samfile, gene, min_quality=30, apply_filters=True):
+def get_filtered_reads_from_region(samfile, gene, min_quality, apply_filters=True):
     for read in samfile.fetch(gene["seqname"], gene["start"], gene["end"]):
         if apply_filters and (
             read.is_qcfail
             or read.is_duplicate
             or read.is_secondary
             or read.is_unmapped
             or read.mapq < min_quality
@@ -74,21 +74,21 @@
 
     return predicted
 
 
 def determine_strandedness(
     ngsfilepath,
     gff,
-    n_genes=100,
-    min_mapq=30,
-    minimum_reads_per_gene=10,
-    split_by_rg=False,
-    max_iterations_per_try=1000,
-    checked_genes=set(),
-    overall_evidence=defaultdict(lambda: defaultdict(int)),
+    n_genes,
+    min_mapq,
+    minimum_reads_per_gene,
+    split_by_rg,
+    max_iterations_per_try,
+    checked_genes,
+    overall_evidence,
 ):
     try:
         ngsfile = NGSFile(ngsfilepath)
     except FileNotFoundError:
         result = {
             "File": ngsfilepath,
             "TotalReads": "N/A",
@@ -290,22 +290,22 @@
             overall_evidence,
         )
 
 
 def main(
     ngsfiles,
     gene_model_file,
-    outfile=sys.stdout,
-    n_genes=100,
-    minimum_reads_per_gene=10,
-    only_protein_coding_genes=True,
-    min_mapq=30,
-    split_by_rg=False,
-    max_tries=3,
-    max_iterations_per_try=1000,
+    outfile,
+    n_genes,
+    minimum_reads_per_gene,
+    only_protein_coding_genes,
+    min_mapq,
+    split_by_rg,
+    max_tries,
+    max_iterations_per_try,
 ):
     logger.info("Arguments:")
     logger.info("  - Gene model file: {}".format(gene_model_file))
     logger.info("  - Number of genes: {}".format(n_genes))
     logger.info("  - Minimum reads per gene: {}".format(minimum_reads_per_gene))
     logger.info(
         "  - Only consider protein coding genes: {}".format(only_protein_coding_genes)
```

### Comparing `ngsderive-3.2.0/ngsderive/utils.py` & `ngsderive-3.2.1/ngsderive/utils.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.2.0/pyproject.toml` & `ngsderive-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "ngsderive"
-version = "3.2.0"
+version = "3.2.1"
 description = "Forensic analysis tool useful in backwards computing information from next-generation sequencing data."
 license = "MIT"
 authors = [
     "Clay McLeod <Clay.McLeod@STJUDE.org>",
     "Andrew Frantz <andrew.frantz@STJUDE.org"
 ]
 readme = "README.md"
```

### Comparing `ngsderive-3.2.0/PKG-INFO` & `ngsderive-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngsderive
-Version: 3.2.0
+Version: 3.2.1
 Summary: Forensic analysis tool useful in backwards computing information from next-generation sequencing data.
 Home-page: https://github.com/claymcleod/ngsderive
 License: MIT
 Keywords: bioinformatics,genomics,sam,bam,fastq
 Author: Clay McLeod
 Author-email: Clay.McLeod@STJUDE.org
 Requires-Python: >=3.8,<3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngsderive Version: 3.2.0 Summary: Forensic analysis
+Metadata-Version: 2.1 Name: ngsderive Version: 3.2.1 Summary: Forensic analysis
 tool useful in backwards computing information from next-generation sequencing
 data. Home-page: https://github.com/claymcleod/ngsderive License: MIT Keywords:
 bioinformatics,genomics,sam,bam,fastq Author: Clay McLeod Author-email:
 Clay.McLeod@STJUDE.org Requires-Python: >=3.8,<3.10 Classifier: Development
 Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

