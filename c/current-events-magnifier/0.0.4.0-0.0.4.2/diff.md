# Comparing `tmp/current_events_magnifier-0.0.4.0.tar.gz` & `tmp/current_events_magnifier-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.4.0.tar", last modified: Mon Jun 26 14:39:15 2023, max compression
+gzip compressed data, was "current_events_magnifier-0.0.4.2.tar", last modified: Tue Jun 27 06:19:39 2023, max compression
```

## Comparing `current_events_magnifier-0.0.4.0.tar` & `current_events_magnifier-0.0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.4.0/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7433 2023-06-20 08:13:10.000000 current_events_magnifier-0.0.4.0/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7526 2023-06-26 14:34:21.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9229 2023-06-26 14:26:04.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-06-23 06:41:12.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7734 2023-06-26 08:43:23.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10227 2023-06-26 10:42:38.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13861 2023-06-26 10:18:43.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-26 14:39:15.443795 current_events_magnifier-0.0.4.0/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1191 2023-06-26 14:38:54.000000 current_events_magnifier-0.0.4.0/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-27 06:19:39.024736 current_events_magnifier-0.0.4.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.4.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9046 2023-06-27 06:19:39.024736 current_events_magnifier-0.0.4.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8391 2023-06-26 15:18:16.000000 current_events_magnifier-0.0.4.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-27 06:19:39.020736 current_events_magnifier-0.0.4.2/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7642 2023-06-26 15:12:52.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9356 2023-06-26 15:00:49.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-06-23 06:41:12.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10227 2023-06-26 10:42:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13861 2023-06-26 10:18:43.000000 current_events_magnifier-0.0.4.2/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-27 06:19:39.020736 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9046 2023-06-27 06:19:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-27 06:19:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-27 06:19:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-06-27 06:19:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-27 06:19:38.000000 current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-27 06:19:39.024736 current_events_magnifier-0.0.4.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1191 2023-06-27 06:19:35.000000 current_events_magnifier-0.0.4.2/setup.py
```

### Comparing `current_events_magnifier-0.0.4.0/LICENSE` & `current_events_magnifier-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/PKG-INFO` & `current_events_magnifier-0.0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: current_events_magnifier
-Version: 0.0.4.0
-Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
-Home-page: https://github.com/lrslab/current_events_magnifier
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
@@ -29,21 +15,24 @@
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
-For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
-
+For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
+This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
+### Base shift (Designed for f5c)
+The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
+For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2**. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 
 ```sh
-pip install current_events_magnifier==0.0.3.8
+pip install current_events_magnifier==0.0.4.1
 pip install ont-fast5-api
 conda install -c bioconda ont_vbz_hdf_plugin f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 CE_magnifier.py tombo -h
@@ -63,14 +52,15 @@
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 Turn on the RNA mode
 ```
 ### read_f5c_resquiggle
 ```sh
 CE_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -82,79 +72,89 @@
   --chrom CHROM         Gene or chromosome name(head of your fasta file)
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 
+                        Turn on the RNA mode
+  --base_shift BASE_SHIFT
+                        base shift if required (default:0)
 
 ```
 ## Quick start
-### Run Basecaller on your ONT data
+### 1. Run Basecaller and alignment on your ONT data
 ```sh
-# assumed your fast5 file folder name is fast5/
+# assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
-### Decide the chrom or transcript name and region of your interest
+### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
-### 1. F5c resquiggle (v1.2) (support R10)
-Step 1 and 2 should run on your two sample respectively, before the step 3.
-1. Data format conversion.
+### 3. Subsample (Optional)
+Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
+So I provide a simple py file to help extract the reads you want to visualize.
+And the new reads will be copied to ```subsample_single/```
 ```sh
-slow5tools f2s fast5/ -d blow5_dir
-slow5tools merge blow5_dir -o file.blow5
-slow5tools index file.blow5
-```
-2. Run f5c resquiggle
-```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
-f5c resquiggle -c all.fastq file.blow5 -o file.paf
-```
-3. Run current_events_magnifier to plot
-```sh
-# run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
---chrom NR_103073.1 --strand + \
---pos 3929 --len 10 \
---ref reference.fasta 
-```
-### 2. Tombo resquiggle (v1.5.0)
-Step 1 and 3 should run on your two sample respectively, before the step 4.
-1. Data format conversion.
-```sh
-# assumed your fast5 file folder name is fast5/
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
-2. Subsample (Optional)
+### 4 Re-squiggle
+#### 4.1 Tombo resquiggle (v1.5.0)
+Step 1 and 2 should run on your two sample respectively, before the step 5.
+1. Data format conversion
 
-Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
-After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
 ```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+# assumed your fast5 file folder name is fast5/
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
-3. Run tombo resquiggle
+2. Run tombo resquiggle
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
 tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
-4. Run current_events_magnifier to plot
+3. Run current_events_magnifier to plot
 ```sh
-CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result\
+ --chrom NR_103073.1 --strand + --pos 2030 \
+ --len 5 --cpu 4 --ref reference.fasta --rna
+```
+#### 4.2 F5c resquiggle (v1.2) (support R10)
+Step 1 and 2 should run on your two sample respectively, before the step 3.
+1. Data format conversion.
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
+```sh
+slow5tools f2s fast5/ -d blow5_dir
+slow5tools merge blow5_dir -o file.blow5
+slow5tools index file.blow5
 ```
+2. Run f5c resquiggle
+```sh
+f5c resquiggle -c all.fastq file.blow5 -o file.paf
+```
+3. Run current_events_magnifier to plot
+```sh
+# run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
+CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+--chrom NR_103073.1 --strand + \
+--pos 3929 --len 10 \
+--ref reference.fasta --base_shift 2 --rna
+```
+
```

### Comparing `current_events_magnifier-0.0.4.0/README.md` & `current_events_magnifier-0.0.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: current_events_magnifier
+Version: 0.0.4.2
+Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
+Home-page: https://github.com/lrslab/current_events_magnifier
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
@@ -15,21 +31,24 @@
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
-For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
-
+For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
+This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
+### Base shift (Designed for f5c)
+The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
+For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2**. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 
 ```sh
-pip install current_events_magnifier==0.0.3.8
+pip install current_events_magnifier==0.0.4.1
 pip install ont-fast5-api
 conda install -c bioconda ont_vbz_hdf_plugin f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 CE_magnifier.py tombo -h
@@ -49,14 +68,15 @@
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 Turn on the RNA mode
 ```
 ### read_f5c_resquiggle
 ```sh
 CE_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -68,79 +88,91 @@
   --chrom CHROM         Gene or chromosome name(head of your fasta file)
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 
+                        Turn on the RNA mode
+  --base_shift BASE_SHIFT
+                        base shift if required (default:0)
 
 ```
 ## Quick start
-### Run Basecaller on your ONT data
+### 1. Run Basecaller and alignment on your ONT data
 ```sh
-# assumed your fast5 file folder name is fast5/
+# assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
-### Decide the chrom or transcript name and region of your interest
+### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
-### 1. F5c resquiggle (v1.2) (support R10)
+### 3. Subsample (Optional)
+Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
+So I provide a simple py file to help extract the reads you want to visualize.
+And the new reads will be copied to ```subsample_single/```
+```sh
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+```
+### 4 Re-squiggle
+#### 4.1 Tombo resquiggle (v1.5.0)
+Step 1 and 2 should run on your two sample respectively, before the step 5.
+1. Data format conversion
+
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
+```sh
+# assumed your fast5 file folder name is fast5/
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+```
+2. Run tombo resquiggle
+```sh
+# if fast5 is not single format need to transfer to single format by ont-fast-api
+# single is fast5s-base-directory
+
+tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
+tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
+# Notes:
+# Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
+# Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
+# If you ran step2, run the tombo command on subsample_single but single
+```
+3. Run current_events_magnifier to plot
+```sh
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result\
+ --chrom NR_103073.1 --strand + --pos 2030 \
+ --len 5 --cpu 4 --ref reference.fasta --rna
+```
+#### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 ```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
 f5c resquiggle -c all.fastq file.blow5 -o file.paf
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
---ref reference.fasta 
+--ref reference.fasta --base_shift 2 --rna
 ```
-### 2. Tombo resquiggle (v1.5.0)
-Step 1 and 3 should run on your two sample respectively, before the step 4.
-1. Data format conversion.
-```sh
-# assumed your fast5 file folder name is fast5/
-multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
-```
-2. Subsample (Optional)
 
-Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
-After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
-```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
-```
-3. Run tombo resquiggle
-```sh
-# if fast5 is not single format need to transfer to single format by ont-fast-api
-# single is fast5s-base-directory
 
-tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
-tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
-# Notes:
-# Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
-# Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
-# If you ran step2, run the tombo command on subsample_single but single
-```
-4. Run current_events_magnifier to plot
-```sh
-CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
-```
+
```

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/CE_magnifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
-    parser_f5c.add_argument('--base_shift',type=int, default=0, help="base shift if required")
+    parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
     add_public_argument(parser_f5c)
 
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
@@ -145,11 +145,15 @@
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
     if args.function == 'f5c':
         if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
             args.pos = args.pos - args.base_shift
         else:
             args.pos = args.pos + args.base_shift
-    signal_plot(df, results_path, args.pos, base_list, title, 'merged')
+    percentile_filter=False
+    if aligned_num_wt>50 and aligned_num_ivt>50:
+        percentile_filter=True
+
+    signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier_test.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/CE_magnifier_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,11 +159,15 @@
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
     if args.function == 'f5c':
         if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
             args.pos = args.pos - args.base_shift
         else:
             args.pos = args.pos + args.base_shift
-    signal_plot(df, results_path, args.pos, base_list, title, 'merged')
+    percentile_filter=False
+    if aligned_num_wt>50 and aligned_num_ivt>50:
+        percentile_filter=True
+
+    signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/extract_sub_fast5_from_bam.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 #         + p9.ylim(ylim_tuple)
 #
 #         plot = plot + p9.labs(title=title, x=str(pos + 1), y=item)
 #         # plot.render_matplotlib()
 #         plot.save(filename=results_path + "/" + item + "_violin.pdf", dpi=300)
 # print(plot)
 
-def signal_plot(df, results_path, pos, base_list, title, plot_type):
+def signal_plot(df, results_path, pos, base_list, title, plot_type,filter=False):
     item_list = ['Mean', 'STD', 'Median', 'Dwell time']
 
 
     if plot_type != 'merged':
 
         for item in item_list:
             sig_min, sig_max = np.percentile(df[item], SIG_PCTL_RANGE)
@@ -103,19 +103,19 @@
 
 
         for item in item_list:
             # collect data
             temp = df[[item, 'position', 'type']].copy()
             temp.columns = ['value', 'position', 'type']
             temp.loc[:, 'stats'] = item
-            # if df[df['position'] == pos].shape[0] > 50:
-            #     sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
-            #     sig_diff = sig_max - sig_min
-            #     ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
-            #     temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
+            if filter and item!='Dwell time':
+                sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
+                sig_diff = sig_max - sig_min
+                ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
+                temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
             if new_df is None:
                 new_df = temp
             else:
                 new_df = pd.concat([new_df, temp], axis=0)
 
         plot = p9.ggplot(new_df, p9.aes(x='position', y="value", fill='type')) \
                + p9.theme_bw() \
```

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.4.2/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.4.0
+Version: 0.0.4.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -29,21 +31,24 @@
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
-For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
-
+For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
+This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
+### Base shift (Designed for f5c)
+The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
+For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2**. However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 
 ```sh
-pip install current_events_magnifier==0.0.3.8
+pip install current_events_magnifier==0.0.4.1
 pip install ont-fast5-api
 conda install -c bioconda ont_vbz_hdf_plugin f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 CE_magnifier.py tombo -h
@@ -63,14 +68,15 @@
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 Turn on the RNA mode
 ```
 ### read_f5c_resquiggle
 ```sh
 CE_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
@@ -82,79 +88,91 @@
   --chrom CHROM         Gene or chromosome name(head of your fasta file)
   --pos POS             site of your interest
   --len LEN             region around the position (default:10)
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
+  --rna                 
+                        Turn on the RNA mode
+  --base_shift BASE_SHIFT
+                        base shift if required (default:0)
 
 ```
 ## Quick start
-### Run Basecaller on your ONT data
+### 1. Run Basecaller and alignment on your ONT data
 ```sh
-# assumed your fast5 file folder name is fast5/
+# assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
-### Decide the chrom or transcript name and region of your interest
+### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
-### 1. F5c resquiggle (v1.2) (support R10)
+### 3. Subsample (Optional)
+Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
+So I provide a simple py file to help extract the reads you want to visualize.
+And the new reads will be copied to ```subsample_single/```
+```sh
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+```
+### 4 Re-squiggle
+#### 4.1 Tombo resquiggle (v1.5.0)
+Step 1 and 2 should run on your two sample respectively, before the step 5.
+1. Data format conversion
+
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
+```sh
+# assumed your fast5 file folder name is fast5/
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+```
+2. Run tombo resquiggle
+```sh
+# if fast5 is not single format need to transfer to single format by ont-fast-api
+# single is fast5s-base-directory
+
+tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
+tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
+# Notes:
+# Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
+# Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
+# If you ran step2, run the tombo command on subsample_single but single
+```
+3. Run current_events_magnifier to plot
+```sh
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result\
+ --chrom NR_103073.1 --strand + --pos 2030 \
+ --len 5 --cpu 4 --ref reference.fasta --rna
+```
+#### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
+If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```fast5/```
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 ```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
 f5c resquiggle -c all.fastq file.blow5 -o file.paf
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
---ref reference.fasta 
-```
-### 2. Tombo resquiggle (v1.5.0)
-Step 1 and 3 should run on your two sample respectively, before the step 4.
-1. Data format conversion.
-```sh
-# assumed your fast5 file folder name is fast5/
-multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
+--ref reference.fasta --base_shift 2 --rna
 ```
-2. Subsample (Optional)
 
-Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
-After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
-```sh
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
-samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
-```
-3. Run tombo resquiggle
-```sh
-# if fast5 is not single format need to transfer to single format by ont-fast-api
-# single is fast5s-base-directory
 
-tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
-tombo resquiggle single/ reference.fasta --processes 16 --num-most-common-errors 5
-# Notes:
-# Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
-# Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
-# If you ran step2, run the tombo command on subsample_single but single
-```
-4. Run current_events_magnifier to plot
-```sh
-CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
-```
+
```

### Comparing `current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.4.2/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.4.0/setup.py` & `current_events_magnifier-0.0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.4.0",
+    version="0.0.4.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

