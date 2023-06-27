# Comparing `tmp/PointBlaster-0.1.9.tar.gz` & `tmp/PointBlaster-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.9.tar", last modified: Tue Jun 27 05:39:44 2023, max compression
+gzip compressed data, was "PointBlaster-0.2.0.tar", last modified: Tue Jun 27 16:45:19 2023, max compression
```

## Comparing `PointBlaster-0.1.9.tar` & `PointBlaster-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.892825 PointBlaster-0.1.9/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:38:26.000000 PointBlaster-0.1.9/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.9/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 05:39:44.892663 PointBlaster-0.1.9/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.872643 PointBlaster-0.1.9/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.9/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    25250 2023-06-27 05:38:05.000000 PointBlaster-0.1.9/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-27 05:38:24.000000 PointBlaster-0.1.9/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.873425 PointBlaster-0.1.9/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.9/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.874040 PointBlaster-0.1.9/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.881832 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.890234 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.873310 PointBlaster-0.1.9/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.9/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.892282 PointBlaster-0.1.9/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.9/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.9/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-27 05:39:44.892872 PointBlaster-0.1.9/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.9/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.798725 PointBlaster-0.2.0/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 16:38:24.000000 PointBlaster-0.2.0/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.2.0/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 16:45:19.798597 PointBlaster-0.2.0/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.778759 PointBlaster-0.2.0/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.0/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    25121 2023-06-27 16:41:32.000000 PointBlaster-0.2.0/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-27 16:41:51.000000 PointBlaster-0.2.0/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.779518 PointBlaster-0.2.0/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.0/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.779793 PointBlaster-0.2.0/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.788847 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.796538 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.779417 PointBlaster-0.2.0/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-27 16:45:19.000000 PointBlaster-0.2.0/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.2.0/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 16:45:19.798277 PointBlaster-0.2.0/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:40:56.000000 PointBlaster-0.2.0/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.2.0/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-27 16:45:19.799476 PointBlaster-0.2.0/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.2.0/setup.py
```

### Comparing `PointBlaster-0.1.9/.DS_Store` & `PointBlaster-0.2.0/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 00000600: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
 00000610: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
 00000620: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
 00000630: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
 00000640: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
 00000650: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
 00000660: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00000670: 6562 6172 0809 0809 5f10 187b 7b35 3537  ebar...._..{{557
-00000680: 2c20 3234 307d 2c20 7b39 3230 2c20 3436  , 240}, {920, 46
-00000690: 347d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  4}}...#/;R_klmno
+00000670: 6562 6172 0809 0809 5f10 187b 7b32 3936  ebar...._..{{296
+00000680: 2c20 3339 337d 2c20 7b39 3230 2c20 3433  , 393}, {920, 43
+00000690: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
 000006a0: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
 000006b0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 8b00 0000 0c00 5000 6f00 6900 6e00 7400  ......P.o.i.n.t.
 000006d0: 4200 6c00 6100 7300 7400 6500 726c 6731  B.l.a.s.t.e.rlg1
 000006e0: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
 000006f0: 0c00 5000 6f00 6900 6e00 7400 4200 6c00  ..P.o.i.n.t.B.l.
 00000700: 6100 7300 7400 6500 726d 6f44 4462 6c6f  a.s.t.e.rmoDDblo
```

### Comparing `PointBlaster-0.1.9/PKG-INFO` & `PointBlaster-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.9
+Version: 0.2.0
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.9/PointBlaster/.DS_Store` & `PointBlaster-0.2.0/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/PointBlaster.py` & `PointBlaster-0.2.0/PointBlaster/PointBlaster.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,17 @@
     for item in result_dict.keys():
         gene = result_dict[item]['GENE']
         if gene not in gene_list.keys():
 
             sbjct_start = result_dict[item]['SBJSTART']
             sbjct_string = result_dict[item]['SBJCT_SEQ']
             query_string = result_dict[item]['QUERY_SEQ']
+            # print(len(query_string))
             coverage = result_dict[item]['%COVERAGE']
+            # print(coverage)
             identity = result_dict[item]['%IDENTITY']
             gene_list[gene] = (gene, sbjct_start, sbjct_string,
                                query_string, coverage, identity)
         else:
             new_sbjct_start = result_dict[item]['SBJSTART']
             new_sbjct_string = result_dict[item]['SBJCT_SEQ']
             new_query_string = result_dict[item]['QUERY_SEQ']
@@ -131,14 +133,15 @@
                 sbjct_string = gene_list[gene][2] + raw_sbjct_seq[len(
                     gene_list[gene][2]):new_sbjct_start - 1] + raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)]
                 query_string = gene_list[gene][3] + raw_sbjct_seq[len(
                     gene_list[gene][2]):new_sbjct_start - 1] + new_query_string
 
             identity = compute_identity(query_string, sbjct_string)
             coverage = len(sbjct_string) * 100 / len(raw_sbjct_seq)
+            # print(coverage)
 
             gene_list[gene] = (gene, sbjct_start, sbjct_string,
                                query_string, coverage, identity)
 
     return gene_list
 
 
@@ -220,42 +223,46 @@
     """
     This function find indel or substitution of query seq compared to sbjct seq and return
     mutation type, indel seq, mutation position.
     """
     mutations = []
 
     shift = 0
+    seq_pos = sbjct_start
     for index in range(sbjct_start - 1, len(sbjct_string)):
 
         # Shift index according to gaps
         i = index + shift
 
         if i == len(sbjct_string):
             break
 
         sbjct_nuc = sbjct_string[i]
         query_nuc = query_string[i]
 
+        mutation_type = ''
+
         if sbjct_nuc.upper() != query_nuc.upper():
             if sbjct_nuc == '-' or query_nuc == '-':
 
                 # insert mutation
+
                 if sbjct_nuc == '-':
                     mutation_type = 'ins'
                     mut_pos = i + 1
-                    indel_start_pos = i
+                    indel_start_pos = seq_pos
                     indel = get_indel(
                         sbjct_string[i:], query_string[i:])
-                    indel_end_pos = i + 1
+                    indel_end_pos = seq_pos + len(indel) - 1
 
                 # deletion mutation
                 else:
                     mutation_type = 'del'
                     mut_pos = i + 1
-                    indel_start_pos = i + 1
+                    indel_start_pos = seq_pos
                     indel = get_indel(query_string[i:], sbjct_string[i:])
                     indel_end_pos = indel_start_pos + len(indel) - 1
 
                 # shift the index to the end of the gaps
                 shift += len(indel) - 1
 
                 # generate mutation name
@@ -271,76 +278,75 @@
                 # print(mutation_name)
 
             # substitute mutation
             # print(sbjct_nuc + '->' + query_nuc)
             else:
                 mutation_type = 'sub'
                 mut_pos = i + 1
-                sub_start_pos = i + 1
+                sub_start_pos = seq_pos
                 sub_seq = get_substitution(sbjct_string[i:], query_string[i:])
-                sub_end_pos = i + len(sub_seq)
+                sub_end_pos = seq_pos + len(sub_seq) - 1
                 shift = len(sub_seq) - 1
 
                 # print(sub_start_pos, sub_seq, sub_end_pos)
                 if gene in genes_list:
                     # calculate condon if gene is not RNA sequence
-                    if sub_start_pos % 3 == 0:
+                    if seq_pos % 3 == 0:
                         if sub_end_pos % 3 != 0:
-                            ref_seq = sbjct_string[sub_start_pos - 3: sub_start_pos +
-                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            ref_seq = sbjct_string[i - 3 + 1: i +
+                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
 
-                            query_seq = query_string[sub_start_pos - 3: sub_start_pos +
-                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            query_seq = query_string[i - 3 + 1: i +
+                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
                         else:
-                            ref_seq = sbjct_string[sub_start_pos -
-                                                   3: sub_end_pos]
-                            query_seq = query_string[sub_start_pos -
-                                                     3: sub_end_pos]
-                    elif sub_start_pos % 3 == 1:
+                            ref_seq = sbjct_string[i -
+                                                   3 + 1: i + len(sub_seq) - 1 + 1]
+                            query_seq = query_string[i -
+                                                     3 + 1: i + len(sub_seq) - 1 + 1]
+                    elif seq_pos % 3 == 1:
                         if sub_end_pos % 3 != 0:
-                            ref_seq = sbjct_string[sub_start_pos - 1: sub_start_pos +
-                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            ref_seq = sbjct_string[i: i +
+                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
 
-                            query_seq = query_string[sub_start_pos - 1: sub_start_pos +
-                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            query_seq = query_string[i: i +
+                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
                         else:
-                            ref_seq = sbjct_string[sub_start_pos -
-                                                   1: sub_end_pos]
-                            query_seq = query_string[sub_start_pos -
-                                                     1: sub_end_pos]
+                            ref_seq = sbjct_string[i: i + len(sub_seq)]
+                            query_seq = query_string[i: i + len(sub_seq)]
                     else:
                         if sub_end_pos % 3 != 0:
-                            ref_seq = sbjct_string[sub_start_pos - 2: sub_start_pos +
-                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            ref_seq = sbjct_string[i - 1: i +
+                                                   len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
 
-                            query_seq = query_string[sub_start_pos - 2: sub_start_pos +
-                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3))]
+                            query_seq = query_string[i - 1: i +
+                                                     len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
                         else:
-                            ref_seq = sbjct_string[sub_start_pos -
-                                                   2: sub_end_pos]
-                            query_seq = query_string[sub_start_pos -
-                                                     2: sub_end_pos]
+                            ref_seq = sbjct_string[i - 1: i + len(seq)]
+                            query_seq = query_string[i - 1: i + len(seq)]
                 else:
-                    ref_seq = sbjct_string[sub_start_pos - 1: sub_start_pos +
-                                           len(sub_seq) - 1]
+                    ref_seq = sbjct_nuc
 
-                    query_seq = query_string[sub_start_pos - 1: sub_start_pos +
-                                             len(sub_seq) - 1]
+                    query_seq = query_nuc
 
                 # print(ref_seq, query_seq)
                 if len(sub_seq) == 1:
-                    mutation_name = str(sub_start_pos) + \
-                        ref_seq + '->' + query_seq
+                    mutation_name = str(seq_pos) + \
+                        sbjct_nuc + '->' + query_nuc
 
                 else:
-                    mutation_name = str(sub_start_pos) + '_' + \
+                    mutation_name = str(seq_pos) + '_' + \
                         str(sub_end_pos) + ref_seq + '->' + query_seq
 
                 mutations += [[mutation_type, mutation_name, sub_start_pos,
                                sub_end_pos, query_seq, ref_seq]]
+
+        # increment seq_position
+        if mutation_type != 'ins':
+            seq_pos += 1
+    # print(mutations)
     return mutations
 
 
 def get_db_mutations(mut_db_path):
     """
     transform the table of resistance_overview.txt to dict format
     """
@@ -425,15 +431,15 @@
                            query_string, coverage, identity)]
 
     """
     mutation_result = {}
     for item in gene_list_result:
         coverage = float(item[4])
         identity = float(item[5])
-        if (coverage == 100.00) & (identity != 100):
+        if (coverage == 100.00) or (identity != 100):
             mutation_result[item[0]] = find_mismatch(
                 item[1], item[2], item[3], item[0], genes_list)
 
     return mutation_result
 
 
 def get_aa_seq(ref_seq, query_seq):
@@ -622,33 +628,36 @@
                     if Blaster.is_fasta(file_path):
                         print(f'Processing {file}')
 
                         # lower the blast coverage in order to find 23S point mutaiton
                         df, result_dict = Blaster(file_path, blastdb,
                                                   output_path, threads, minid, 20).biopython_blast()
                         # print(result_dict)
+                        # print(result_dict)
                         # print(df)
                         db_mutations = get_db_mutations(db_mutations_path)
                         # print(db_mutations)
                         genes, RNA_genes = get_gene_list(args.s)
 
                         gene_dict_result = get_align_seq(
                             result_dict, ref_fasta)
                         # print(gene_list_result)
+                        # print(gene_dict_result)
 
                         # parse gene_dict_result
                         gene_list_result = []
                         for key in gene_dict_result.keys():
                             if float(gene_dict_result[key][4]) >= float(mincov):
                                 gene_list_result.append(gene_dict_result[key])
                         # print(gene_list_result)
 
                         mutation_result = find_mutations(
                             gene_list_result, genes)
                         # print(mutation_result)
+                        # print(mutation_result)
 
                         # print(test)
                         # print(gene_list_result)
                         f.write(filter_result(
                             mutation_result, db_mutations, genes))
 
                         print(
```

### Comparing `PointBlaster-0.1.9/PointBlaster/db/.DS_Store` & `PointBlaster-0.2.0/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.2.0/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.2.0/PointBlaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.9
+Version: 0.2.0
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.9/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.2.0/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/README.md` & `PointBlaster-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/dist/.DS_Store` & `PointBlaster-0.2.0/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.9/setup.py` & `PointBlaster-0.2.0/setup.py`

 * *Files identical despite different names*

