# Comparing `tmp/PointBlaster-0.1.8.tar.gz` & `tmp/PointBlaster-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.8.tar", last modified: Mon Jun 26 05:59:52 2023, max compression
+gzip compressed data, was "PointBlaster-0.1.9.tar", last modified: Tue Jun 27 05:39:44 2023, max compression
```

## Comparing `PointBlaster-0.1.8.tar` & `PointBlaster-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.363556 PointBlaster-0.1.8/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:48.000000 PointBlaster-0.1.8/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.8/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-26 05:59:52.363424 PointBlaster-0.1.8/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.352262 PointBlaster-0.1.8/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.8/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    22363 2023-06-26 05:58:18.000000 PointBlaster-0.1.8/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-26 05:58:37.000000 PointBlaster-0.1.8/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.353017 PointBlaster-0.1.8/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.8/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.353127 PointBlaster-0.1.8/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.357233 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.363134 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.352909 PointBlaster-0.1.8/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-26 05:59:52.000000 PointBlaster-0.1.8/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.8/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-26 05:59:52.363245 PointBlaster-0.1.8/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.8/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.8/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-26 05:59:52.363597 PointBlaster-0.1.8/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.8/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.892825 PointBlaster-0.1.9/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:38:26.000000 PointBlaster-0.1.9/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.9/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 05:39:44.892663 PointBlaster-0.1.9/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.872643 PointBlaster-0.1.9/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.9/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    25250 2023-06-27 05:38:05.000000 PointBlaster-0.1.9/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-27 05:38:24.000000 PointBlaster-0.1.9/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.873425 PointBlaster-0.1.9/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.1.9/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.874040 PointBlaster-0.1.9/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.881832 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.890234 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.873310 PointBlaster-0.1.9/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-27 05:39:44.000000 PointBlaster-0.1.9/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.9/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-27 05:39:44.892282 PointBlaster-0.1.9/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.9/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.9/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-27 05:39:44.892872 PointBlaster-0.1.9/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.9/setup.py
```

### Comparing `PointBlaster-0.1.8/.DS_Store` & `PointBlaster-0.1.9/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -75,56 +75,56 @@
 000004a0: 3637 347d 2c20 7b39 3230 2c20 3433 367d  674}, {920, 436}
 000004b0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
 000004c0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
 000004d0: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
 000004e0: 0000 0500 6200 7500 6900 6c00 6476 5372  ....b.u.i.l.dvSr
 000004f0: 6e6c 6f6e 6700 0000 0100 0000 0400 6400  nlong.........d.
 00000500: 6900 7300 7462 7773 7062 6c6f 6200 0000  i.s.tbwspblob...
-00000510: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000510: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
 00000520: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
 00000530: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
 00000540: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00000550: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00000560: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00000570: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
-00000580: 5f10 197b 7b31 3439 302c 2036 3734 7d2c  _..{{1490, 674},
-00000590: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
-000005a0: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
-000005b0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-000005c0: 0000 0000 0000 0000 008c 0000 0004 0064  ...............d
-000005d0: 0069 0073 0074 7653 726e 6c6f 6e67 0000  .i.s.tvSrnlong..
-000005e0: 0001 0000 000c 0050 006f 0069 006e 0074  .......P.o.i.n.t
-000005f0: 0042 006c 0061 0073 0074 0065 0072 6277  .B.l.a.s.t.e.rbw
-00000600: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
-00000610: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
-00000620: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00000630: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00000640: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00000650: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00000660: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00000670: 6465 6261 7208 0908 095f 1018 7b7b 3532  debar...._..{{52
-00000680: 382c 2032 3937 7d2c 207b 3932 302c 2034  8, 297}, {920, 4
-00000690: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
-000006a0: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
-000006b0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
-000006c0: 008b 0000 000c 0050 006f 0069 006e 0074  .......P.o.i.n.t
-000006d0: 0042 006c 0061 0073 0074 0065 0072 6c67  .B.l.a.s.t.e.rlg
-000006e0: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
-000006f0: 000c 0050 006f 0069 006e 0074 0042 006c  ...P.o.i.n.t.B.l
-00000700: 0061 0073 0074 0065 0072 6d6f 4444 626c  .a.s.t.e.rmoDDbl
-00000710: 6f62 0000 0008 8bc5 5825 0724 c541 0000  ob......X%.$.A..
-00000720: 000c 0050 006f 0069 006e 0074 0042 006c  ...P.o.i.n.t.B.l
-00000730: 0061 0073 0074 0065 0072 6d6f 6444 626c  .a.s.t.e.rmodDbl
-00000740: 6f62 0000 0008 8bc5 5825 0724 c541 0000  ob......X%.$.A..
-00000750: 000c 0050 006f 0069 006e 0074 0042 006c  ...P.o.i.n.t.B.l
-00000760: 0061 0073 0074 0065 0072 7068 3153 636f  .a.s.t.e.rph1Sco
-00000770: 6d70 0000 0000 0000 0000 0000 000c 0050  mp.............P
-00000780: 006f 0069 006e 0074 0042 006c 0061 0073  .o.i.n.t.B.l.a.s
-00000790: 0074 0065 0072 7653 726e 6c6f 6e67 0000  .t.e.rvSrnlong..
-000007a0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 5f10 187b 7b35 3537 2c20 3234 307d 2c20  _..{{557, 240}, 
+00000590: 7b39 3230 2c20 3436 347d 7d09 0815 232f  {920, 464}}...#/
+000005a0: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+000005b0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 8b00 0000 0400 6400  ..............d.
+000005d0: 6900 7300 7476 5372 6e6c 6f6e 6700 0000  i.s.tvSrnlong...
+000005e0: 0100 0000 0c00 5000 6f00 6900 6e00 7400  ......P.o.i.n.t.
+000005f0: 4200 6c00 6100 7300 7400 6500 7262 7773  B.l.a.s.t.e.rbws
+00000600: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
+00000610: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
+00000620: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00000630: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00000640: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00000650: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00000660: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00000670: 6562 6172 0809 0809 5f10 187b 7b35 3537  ebar...._..{{557
+00000680: 2c20 3234 307d 2c20 7b39 3230 2c20 3436  , 240}, {920, 46
+00000690: 347d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  4}}...#/;R_klmno
+000006a0: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
+000006b0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+000006c0: 8b00 0000 0c00 5000 6f00 6900 6e00 7400  ......P.o.i.n.t.
+000006d0: 4200 6c00 6100 7300 7400 6500 726c 6731  B.l.a.s.t.e.rlg1
+000006e0: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
+000006f0: 0c00 5000 6f00 6900 6e00 7400 4200 6c00  ..P.o.i.n.t.B.l.
+00000700: 6100 7300 7400 6500 726d 6f44 4462 6c6f  a.s.t.e.rmoDDblo
+00000710: 6200 0000 088b c558 2507 24c5 4100 0000  b......X%.$.A...
+00000720: 0c00 5000 6f00 6900 6e00 7400 4200 6c00  ..P.o.i.n.t.B.l.
+00000730: 6100 7300 7400 6500 726d 6f64 4462 6c6f  a.s.t.e.rmodDblo
+00000740: 6200 0000 088b c558 2507 24c5 4100 0000  b......X%.$.A...
+00000750: 0c00 5000 6f00 6900 6e00 7400 4200 6c00  ..P.o.i.n.t.B.l.
+00000760: 6100 7300 7400 6500 7270 6831 5363 6f6d  a.s.t.e.rph1Scom
+00000770: 7000 0000 0000 0000 0000 0000 0c00 5000  p.............P.
+00000780: 6f00 6900 6e00 7400 4200 6c00 6100 7300  o.i.n.t.B.l.a.s.
+00000790: 7400 6500 7276 5372 6e6c 6f6e 6700 0000  t.e.rvSrnlong...
+000007a0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `PointBlaster-0.1.8/PKG-INFO` & `PointBlaster-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.8
+Version: 0.1.9
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.8/PointBlaster/.DS_Store` & `PointBlaster-0.1.9/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/PointBlaster.py` & `PointBlaster-0.1.9/PointBlaster/PointBlaster.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,32 +75,88 @@
     cline = NcbimakeblastdbCommandline(
         dbtype="nucl", out=name, input_file=file)
     print(f'Making {name} database...')
     stdout, stderr = cline()
     print('Finish')
 
 
-def get_align_seq(result_dict):
+def get_sbjct_seq(ref_fasta, gene):
+    """
+    obtain gene sequence from reference fasta file of specific specie
+    """
+    for seq_record in SeqIO.parse(open(ref_fasta, mode='r'), 'fasta'):
+        gene_name = seq_record.id.split('___')[0]
+        if gene_name == gene:
+            seq = str(seq_record.seq)
+    return seq
+
+    # seq_record.seq
+
+
+def get_align_seq(result_dict, ref_fasta):
     """
     convert the result from cvmblaster to gene list format like:
     [gene , sbjct_start, sbjct_string, query_string, coverage, identity]
     """
-    gene_list = []
+    gene_list = {}
+
+    # need concatenate hits from same gene
+
+    # check if multiple hits from same gene exist
     for item in result_dict.keys():
         gene = result_dict[item]['GENE']
-        sbjct_start = result_dict[item]['SBJSTART']
-        sbjct_string = result_dict[item]['SBJCT_SEQ']
-        query_string = result_dict[item]['QUERY_SEQ']
-        coverage = result_dict[item]['%COVERAGE']
-        identity = result_dict[item]['%IDENTITY']
-        gene_list += [(gene, sbjct_start, sbjct_string,
-                       query_string, coverage, identity)]
+        if gene not in gene_list.keys():
+
+            sbjct_start = result_dict[item]['SBJSTART']
+            sbjct_string = result_dict[item]['SBJCT_SEQ']
+            query_string = result_dict[item]['QUERY_SEQ']
+            coverage = result_dict[item]['%COVERAGE']
+            identity = result_dict[item]['%IDENTITY']
+            gene_list[gene] = (gene, sbjct_start, sbjct_string,
+                               query_string, coverage, identity)
+        else:
+            new_sbjct_start = result_dict[item]['SBJSTART']
+            new_sbjct_string = result_dict[item]['SBJCT_SEQ']
+            new_query_string = result_dict[item]['QUERY_SEQ']
+
+            # get reference sequence of gene
+            raw_sbjct_seq = get_sbjct_seq(ref_fasta, gene)
+            if new_sbjct_start < gene_list[gene][1]:
+                sbjct_start = new_sbjct_start
+                sbjct_string = raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)] + raw_sbjct_seq[len(
+                    new_sbjct_string):gene_list[gene][1] - 1] + gene_list[gene][2]
+                query_string = new_query_string + \
+                    raw_sbjct_seq[len(new_sbjct_string):gene_list[gene][1] - 1] + gene_list[gene][3]
+            else:
+                sbjct_start = gene_list[gene][1]
+                sbjct_string = gene_list[gene][2] + raw_sbjct_seq[len(
+                    gene_list[gene][2]):new_sbjct_start - 1] + raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)]
+                query_string = gene_list[gene][3] + raw_sbjct_seq[len(
+                    gene_list[gene][2]):new_sbjct_start - 1] + new_query_string
+
+            identity = compute_identity(query_string, sbjct_string)
+            coverage = len(sbjct_string) * 100 / len(raw_sbjct_seq)
+
+            gene_list[gene] = (gene, sbjct_start, sbjct_string,
+                               query_string, coverage, identity)
+
     return gene_list
 
 
+def compute_identity(query_string, sbjct_string):
+    a = 1
+    for i in range(0, len(query_string) - 1):
+        # print(i)
+        if query_string[i] == sbjct_string[i]:
+            a += 1
+    identity = a * 100 / len(sbjct_string)
+    # print(identity)
+    return identity
+
+
 def aa(codon):
     """
     This function converts a codon to an amino acid. If the codon is not
     valid an error message is given, or else, the amino acid is returned.
     """
     codon = codon.upper()
     aa = {"ATT": "I", "ATC": "I", "ATA": "I",
@@ -541,14 +597,16 @@
 
         # check if -species var exist
         if args.s is not None:
             blastdb = os.path.join(os.path.dirname(
                 __file__), f'db/point_mutation/{args.s}/{args.s}')
             db_mutations_path = os.path.join(os.path.dirname(
                 __file__), f'db/point_mutation/{args.s}/resistens-overview.txt')
+            ref_fasta = os.path.join(os.path.dirname(
+                __file__), f'db/point_mutation/{args.s}/{args.s}.fsa')
         else:
             sys.exit(1)
 
         for file in files:
             file_base = str(os.path.basename(os.path.splitext(file)[0]))
             output_filename = file_base + '_tab.txt'
             # file_base = str(os.path.splitext(file)[0])
@@ -559,22 +617,33 @@
             with open(outfile, 'a') as f:
                 f.write(
                     f'Gene\tMutation\tNucleotide change\tAmino Acid change\tResistance\n')
                 if os.path.isfile(file_path):
                     # print("TRUE")
                     if Blaster.is_fasta(file_path):
                         print(f'Processing {file}')
+
+                        # lower the blast coverage in order to find 23S point mutaiton
                         df, result_dict = Blaster(file_path, blastdb,
-                                                  output_path, threads, minid, mincov).biopython_blast()
+                                                  output_path, threads, minid, 20).biopython_blast()
+                        # print(result_dict)
                         # print(df)
                         db_mutations = get_db_mutations(db_mutations_path)
                         # print(db_mutations)
                         genes, RNA_genes = get_gene_list(args.s)
 
-                        gene_list_result = get_align_seq(result_dict)
+                        gene_dict_result = get_align_seq(
+                            result_dict, ref_fasta)
+                        # print(gene_list_result)
+
+                        # parse gene_dict_result
+                        gene_list_result = []
+                        for key in gene_dict_result.keys():
+                            if float(gene_dict_result[key][4]) >= float(mincov):
+                                gene_list_result.append(gene_dict_result[key])
                         # print(gene_list_result)
 
                         mutation_result = find_mutations(
                             gene_list_result, genes)
                         # print(mutation_result)
 
                         # print(test)
```

### Comparing `PointBlaster-0.1.8/PointBlaster/db/.DS_Store` & `PointBlaster-0.1.9/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.1.9/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.1.9/PointBlaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.8
+Version: 0.1.9
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.8/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.1.9/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/README.md` & `PointBlaster-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/dist/.DS_Store` & `PointBlaster-0.1.9/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.8/setup.py` & `PointBlaster-0.1.9/setup.py`

 * *Files identical despite different names*

