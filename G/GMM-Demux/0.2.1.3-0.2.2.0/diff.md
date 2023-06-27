# Comparing `tmp/GMM_Demux-0.2.1.3.tar.gz` & `tmp/GMM_Demux-0.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GMM_Demux-0.2.1.3.tar", last modified: Thu Aug  6 03:02:44 2020, max compression
+gzip compressed data, was "dist/GMM_Demux-0.2.2.0.tar", last modified: Tue Jun 27 16:22:04 2023, max compression
```

## Comparing `GMM_Demux-0.2.1.3.tar` & `GMM_Demux-0.2.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/example_input/
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/example_input/outs/
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/
--rw-r--r--   0 hxin      (1001) hxin      (1001)       80 2019-05-31 17:40:06.000000 GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/features.tsv.gz
--rw-r--r--   0 hxin      (1001) hxin      (1001)   237570 2019-05-29 18:52:48.000000 GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz
--rw-r--r--   0 hxin      (1001) hxin      (1001)    60384 2019-05-29 18:52:48.000000 GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz
--rw-r--r--   0 hxin      (1001) hxin      (1001)    65191 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/phony_type.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)    12053 2019-11-12 19:41:03.000000 GMM_Demux-0.2.1.3/class_output.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)     6489 2019-06-01 05:39:40.000000 GMM_Demux-0.2.1.3/features.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)    63771 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/pure_type.png
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/
--rw-r--r--   0 hxin      (1001) hxin      (1001)       10 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/top_level.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)        1 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/dependency_links.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    15002 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/PKG-INFO
--rw-r--r--   0 hxin      (1001) hxin      (1001)       72 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/requires.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1439 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/SOURCES.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)       56 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux.egg-info/entry_points.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    12436 2020-05-08 16:12:32.000000 GMM_Demux-0.2.1.3/README.md
--rw-rw-r--   0 hxin      (1001) hxin      (1001)   212591 2019-11-12 21:59:36.000000 GMM_Demux-0.2.1.3/term.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)      980 2020-08-06 03:02:26.000000 GMM_Demux-0.2.1.3/setup.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)   453771 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/phony.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)   517818 2019-11-26 20:34:24.000000 GMM_Demux-0.2.1.3/example_hto.csv
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/example_cell_types/
--rw-r--r--   0 hxin      (1001) hxin      (1001)     3382 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD11+CD14-CD16-.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     2451 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD56+CD16-.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)   110238 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD3+CD4+.txt
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1216 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD14+CD56+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     8550 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD14+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     5282 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD56+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1007 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD56+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     8702 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD8+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     2698 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD14+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1976 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD19+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)      247 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD14+CD56+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)      798 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD19+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     5225 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD14+CD16+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    37316 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD3+CD8+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)   183445 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD3+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    37449 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD14+CD16-.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)     7923 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD19+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    24491 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/example_cell_types/CD56+CD16+.txt
--rw-r--r--   0 hxin      (1001) hxin      (1001)    24413 2019-06-01 05:39:40.000000 GMM_Demux-0.2.1.3/summary.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)    15002 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/PKG-INFO
-drwxr-xr-x   0 hxin      (1001) hxin      (1001)        0 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/GMM_Demux/
--rw-r--r--   0 hxin      (1001) hxin      (1001)    13429 2019-11-26 21:14:42.000000 GMM_Demux-0.2.1.3/GMM_Demux/GMM_Demux.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)     2243 2019-11-26 21:14:44.000000 GMM_Demux-0.2.1.3/GMM_Demux/GMM_IO.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)     9214 2019-11-12 05:18:39.000000 GMM_Demux-0.2.1.3/GMM_Demux/estimator.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1084 2019-05-31 17:40:06.000000 GMM_Demux-0.2.1.3/GMM_Demux/check_multi_comp.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)     6170 2020-08-06 02:59:46.000000 GMM_Demux-0.2.1.3/GMM_Demux/classify_drops.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)     7544 2019-11-26 20:30:09.000000 GMM_Demux-0.2.1.3/GMM_Demux/compute_venn.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)        0 2019-05-31 17:40:06.000000 GMM_Demux-0.2.1.3/GMM_Demux/__init__.py
--rw-r--r--   0 hxin      (1001) hxin      (1001)  1009859 2019-05-29 19:16:33.000000 GMM_Demux-0.2.1.3/GMM_simplified.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)   105559 2019-05-29 18:54:55.000000 GMM_Demux-0.2.1.3/planner.png
--rw-rw-r--   0 hxin      (1001) hxin      (1001)  1785236 2019-11-12 22:27:35.000000 GMM_Demux-0.2.1.3/path.png
--rw-r--r--   0 hxin      (1001) hxin      (1001)     1072 2019-11-26 20:30:09.000000 GMM_Demux-0.2.1.3/LICENSE
--rw-r--r--   0 hxin      (1001) hxin      (1001)       38 2020-08-06 03:02:44.000000 GMM_Demux-0.2.1.3/setup.cfg
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.502512 GMM_Demux-0.2.2.0/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.442159 GMM_Demux-0.2.2.0/GMM_Demux/
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    13604 2023-06-27 16:20:06.000000 GMM_Demux-0.2.2.0/GMM_Demux/GMM_Demux.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2243 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/GMM_IO.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)        0 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/__init__.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1084 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/check_multi_comp.py
+-rw-r--r--   0 hxin      (1000) hxin      (1000)     7166 2023-06-27 16:20:06.000000 GMM_Demux-0.2.2.0/GMM_Demux/classify_drops.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7544 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/compute_venn.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     9214 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/estimator.py
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.466183 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/PKG-INFO
+-rw-r--r--   0 hxin      (1000) hxin      (1000)     1439 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/SOURCES.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)        1 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/dependency_links.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       55 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/entry_points.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       81 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/requires.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       10 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/top_level.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1009859 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_simplified.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1072 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/LICENSE
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-06-27 16:22:04.498525 GMM_Demux-0.2.2.0/PKG-INFO
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12436 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/README.md
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12053 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/class_output.png
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.478833 GMM_Demux-0.2.2.0/example_cell_types/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     3382 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD11+CD14-CD16-.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5225 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37449 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16-.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7923 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   183445 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   110238 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+CD4+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37316 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+CD8+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24491 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2451 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16-.txt
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.494516 GMM_Demux-0.2.2.0/example_cell_types/Doublets/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1216 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD14+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8550 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)      247 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1976 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5282 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8702 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD8+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2698 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD14+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)      798 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1007 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   517818 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_hto.csv
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.412660 GMM_Demux-0.2.2.0/example_input/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.412660 GMM_Demux-0.2.2.0/example_input/outs/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.498525 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    60384 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)       80 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/features.tsv.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   237570 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     6489 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/features.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1785236 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/path.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   453771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/phony.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    65191 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/phony_type.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   105559 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/planner.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    63771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/pure_type.png
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       38 2023-06-27 16:22:04.502512 GMM_Demux-0.2.2.0/setup.cfg
+-rw-r--r--   0 hxin      (1000) hxin      (1000)      989 2023-06-27 16:20:35.000000 GMM_Demux-0.2.2.0/setup.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24413 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/summary.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   212591 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/term.png
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz` & `GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz` & `GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/phony_type.png` & `GMM_Demux-0.2.2.0/phony_type.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/class_output.png` & `GMM_Demux-0.2.2.0/class_output.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/features.png` & `GMM_Demux-0.2.2.0/features.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/pure_type.png` & `GMM_Demux-0.2.2.0/pure_type.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux.egg-info/PKG-INFO` & `GMM_Demux-0.2.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,275 +1,260 @@
-Metadata-Version: 2.1
-Name: GMM-Demux
-Version: 0.2.1.3
-Summary: A multiplet removal tool for processing cell hashing data
-Home-page: https://github.com/CHPGenetics/GMM-demux
-Author: Hongyi Xin
-Author-email: gohongyi@gmail.com
-License: UNKNOWN
-Description: # GMM-Demux 
-        GMM-Demux is a Gaussian-Mixture-Model-based software for processing sample barcoding data (cell hashing and MULTI-seq).
-        
-        GMM-Demux identifies Multi-Sample Multiplets (MSMs) in a sample barcoding dataset. Below shows an example distribution of MSMs in a PBMC scRNA-seq dataset. Orange dots in the scatter plot are MSMs.
-        
-        <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/GMM_simplified.png" alt="GMM-Demux example" width="600"/>
-        
-        ## Description
-        GMM-Demux removes Multi-Sample-Multiplets (MSMs) in a cell hashing dataset and estimates the percentages of Same-Sample-Multiplets (SSMs) and singlets in the remaining dataset.
-        GMM-Demux also verifies if a putative cell type exists, or is it merely an artifact induced by multiplets.
-        
-        Multiplet-induced fake cell types are called "phony cell types".
-        
-        Examples of phony cell types in a PBMC CITE-seq dataset is provided in the figure below:
-        
-        <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/phony.png" width="600"/>
-        
-        In the above figure, both the CD3+CD19+ and the CD4+CD8+ cell types are multiplet-induced fake cell types.
-        
-        Phony type clusters have large percentages of MSMs, as above figure shows. Both phony type clusters have large MSM percentages.
-        
-        Percentages of MSMs are used as key features by GMM-Demux to classify GEM clusters.
-        
-        ## Terminology
-        * **Singlet**: A droplet that contains a single cell.
-        
-        * **MSM**: Multi-Sample Multiplet. A MSM is a multiplet that contains cells from different samples in sample barcoding. MSMs can be identified by GMM-Demux.
-        
-        * **SSM**: Same-Sample Multiplet. A SSM is a multiplet that contains cells from a single sample in sample barcoding. SSMs cannot be separated from singlets by sample barcoding.
-        
-        * **SSD**: Same-Sample Droplet. SSD is a combined category of both SSMs and singlets.
-        
-        * **Pure type**: a pure type cell type is a real cell type that exist in the tissue.
-        
-        * **Phony type**: a phony type cell type is an artificial cell type that is an artifact produced by multiplets.
-        
-        * **Mixture type**: a mixture type cell type is a cluster of droplets in which there exist a non-trivial fraction of phony type droplets.
-        
-        An illustration of the above terminologies in a PBMC dataset is provided in the figure below:
-        
-        <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/term.png" width="600"/>
-        
-        ## Features
-        * Remove cell-hashing-identifiable multiplets (i.e., MSMs) from the dataset.
-        * Estimate the fraction of cell-hashing-unidentifiable multiplets (SSMs) in the remaining dataset (the RSSM percentage).
-        * Test if a putative cell type is a pure (real) cell type or is it a phony (fake) cell type.
-        
-        ## Example Dataset
-        * An example cell hashing dataset is provided in the *example_input* folder. It contains the per-drop HTO count matrix of a 4-sample cell hashing library prep. The input folder has the same file format with the CellRanger v3 output.
-        
-        # Authors
-         Hongyi Xin, Qi Yan, Yale Jiang, Jiadi Luo, Carla Erb, Richard Duerr, Kong Chen* and Wei Chen*
-        
-        # Maintainer
-        Hongyi Xin <gohongyi at gmail.edu>
-        
-        ## Requirement
-        
-        GMM-Demux requires python3 (>3.5).
-        
-        ## Install
-        
-        GMM-Demux can be directly installed from PyPi. Or it can be built and installed locally.
-        
-        ### Install GMM-Demux from PyPi.
-        ```bash
-        pip3 install --user GMM_Demux
-        ```
-        
-        In some OS, the `pip3` is linked to `pip` by default. For these OS, the installation command is simply:
-        
-        ```bash
-        pip install --user GMM_Demux
-        ```
-        
-        Check if `pip3` is linked to `pip` with `pip -V`.
-        
-        If one chooses to install GMM-Demux from PyPi, it is unnecessary to download GMM-Demux from github. However, we still recommend downloading the example dataset to try out GMM-Demux.
-        
-        ### Install GMM-Demux locally using [setuptools](https://packaging.python.org/tutorials/installing-packages/) and pip3.
-        
-        You may choose to install GMM-Demux locally after cloning the github repository. However, **this is for advanced users only and support is not gauranteed**.
-        The command is provided below:
-        
-        ```bash
-        cd <GMM-Demux dir>
-        python3 setup.py sdist bdist_wheel
-        pip3 install --user . 
-        ```
-        
-        ### Post installation processes
-        
-        If this is the first time you install a python3 software through pip, make sure you add the pip binary folder to your `PATH` variable.
-        Typically, the pip binary folder is located at ```~/.local/bin```.
-        
-        The pip binary folder might locate at a different location if the user uses virtual enviroment. Pay attention to the pip installation output.
-        
-        Here is an example installation output. The path of the pip binary folder is highlighted:
-        <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/path.png" width="500"/>
-        
-        To temporarily add the pip binary folder, run the following command:
-        ```bash
-        export PATH=~/.local/bin:$PATH
-        ```
-        
-        To permenantly add the pip library folder to your `PATH` variable, append the following line to your `.bashrc` file (assuming bash is the default shell).
-        ```bash
-        PATH=~/.local/bin:$PATH
-        ```
-        
-        ## Content
-        
-        The source code of GMM-Demux is supplied in the ```GMM_Demux``` folder.
-        
-        An example cell hashing dataset is also provided, located in the ```example_input/outs/filtered_feature_bc_matrix``` folder.
-        
-        An example set of hand-curated putative cell types of the above dataset are provided in the ```example_cell_types``` folder. Cell types are annotated through manual gating using surface marker expression data.
-        
-        An example csv format of the above cell hashing dataset is provided as the ```example_hto.csv``` file.
-        
-        ## Usage
-        
-        ### Case 1: Basic Usage, Remove MSMs
-        Once installed, GMM-Demux is directly accessible with the ```GMM-demux``` command.
-        ```bash
-        GMM-demux <cell_hashing_path> <HTO_names>
-        ```
-        
-        ```<HTO_names>``` is a list of sample tags (HTOs) separated by ',' without whitespace.
-        For example, there are four sample barcoding tags in the example cell hashing dataset.
-        They are **HTO_1**, **HTO_2**, **HTO_3**, **HTO_4**. The ```<HTO_names>``` variable therefore is ```HTO_1,HTO_2,_HTO_3,HTO_4```.
-        
-        The non-MSM droplets (SSDs) of the dataset are stored in the *GMM_Demux_mtx* folder under the current directory by default.
-        The output path can also be specified through the `-o` flag.
-        
-        #### Example Command 
-        An example cell hashing data is provided in the *example_input* folder. <HTO_names> can be obtained from the features.tsv file.
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4
-        ```
-        
-        <HTO_names> are included in the features.tsv file. The content of the feature.tsv file is shown below.
-        
-        ![HTO names example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/features.png)
-        
-        #### Output
-        The default content in the output folder are the non-MSM droplets (SSDs), stored in MTX format. The output shares the same format with CellRanger 3.0. By default, the output is stored in `SSD_mtx` folder. The output location can be overwritten with the `-o` flag.
-        
-        ### Case 2: Compute the MSM and SSM rates
-        To compute the MSM and SSM rates, GMM-Demux requires the `-u` flag:
-        
-        * -u SUMMARY, --summary SUMMARY  Generate the statstic summary of the dataset. Requires an estimated total number of cells in the assay as input.
-         
-        The `-u` flag requires an additional <NUM_OF_CELL> argument, which is the estimated total count of cells in the single cell assay.
-        
-        #### Example Command
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685
-        ```
-        
-        #### Output
-        Below is an example report:
-        ![Summary example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/summary.png)
-        
-        * RSSM denotes the percentage of SSMs among the remaining SSDs (after removing all MSMs). RSSM **measures the quality of the final cell hashing dataset after removing MSMs**.
-        
-        ### Case 3: Verify if a cell type exists 
-        GMM-Demux verifies if a putative cell type exists with the `-e` flag:
-        
-        * -e EXAMINE, --examine  EXAMINE Provide the cell list. Requires a file argument. Only executes if -u is set.
-        
-        The `-e` flag requires a file name, which stores the list of droplet barcodes of the putative cell type.
-        
-        #### Example Command
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685 -e example_cell_types/CD19+.txt
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685 -e example_cell_types/Doublets/CD3+CD4+CD19+.txt
-        ```
-        
-        #### Output
-        An example output of a pure cell type:
-        ![Pure type example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/pure_type.png)
-        
-        An example output of a phony cell type:
-        ![Phone type example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/phony_type.png)
-        
-        ### Case 4: Use the csv file format as input, instead of the mtx format 
-        #### Example Command
-        ```bash
-        GMM-demux -c example_hto.csv HTO_1,HTO_2,HTO_3,HTO_4 -u 35685
-        ```
-        
-        ### Case 5: Extract droplets that are labeled by a combination of sample tags
-        Extract droplets that are labeled by multiple sample barcoding tags, with the `-x` flag:
-        
-        * -x EXTRACT, --extract EXTRACT  Names of the sample barcoding tag(s) to extract, separated by ','. Joint tags are linked with '+'.
-        
-        **When `-x` is set, other functions of GMM-Demux will be turned off.**
-        
-        #### *Case 5a: Extract a single HTO sample*
-        
-        #### Example Command
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO_1
-        ```
-        #### *Case 5b: Extract a single HTO sample that are jointly defined by multiple HTO tags*
-        Use `+` to specify the joint HTO tags.
-        
-        #### Example Command
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO_1+HTO_2
-        ```
-        #### *Case 5c: Extract multiple HTO samples*
-        Use `,` to separate sample tags. Single tag samples can be merged with joint-tag samples.
-        
-        #### Example Command
-        ```bash
-        GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO3,HTO_1+HTO_2,HTO_1+HTO_4+HTO_2
-        ```
-        
-        ## Optional Arguments
-        * -h: show help information.
-        * -f FULL, --full FULL  Generate the full classification report. Require a path argument.
-        * -s SIMPLIFIED, --simplified SIMPLIFIED  Generate the simplified classification report. Require a path argument.
-        * -o OUTPUT, --output OUTPUT  The path for storing the Same-Sample-Droplets (SSDs). SSDs are stored in mtx format. Requires a path argument. Default path: SSD_mtx.
-        * -r REPORT, --report REPORT  Specify the file to store summary report. Require a file argument.
-        * -c CSV, --csv  Take input in csv format, instead of mmx format.
-        * -s SKIP, --skip FULL\_REPORT  Load a full classification report and skip the mtx folder as input. Require a path argument.
-        * -a AMBIGUOUS, --ambiguous AMBIGUOUS  The estimated chance of having a phony GEM getting included in a pure type GEM cluster by the clustering algorithm. Requires a float in (0, 1). Default value: 0.05. Only executes if -e executes.
-        * -t THRESHOLD, --threshold THRESHOLD  Provide the confidence threshold value. Requires a float in (0,1). Default value: 0.8.
-        
-        ## Parsing the Classification Output
-        There are two files in a classification output folder. A config file (ending with .config) and a classification file (ending with .csv).
-        
-        The classification file contains the label of each droplet as well as the probability of the classification. The classification is represented with numbers which are explained in the config file.
-        
-        Below shows the classification output of the example data:
-        
-        <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/class_output.png" width="600"/>
-         
-        ## Online Cell Hashing Experiment Planner
-        A GMM-Demux based online cell hashing experiment planner is publically accessible at [here](https://www.pitt.edu/~wec47/gmmdemux.html).
-        
-        [<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/planner.png" alt="Online explanner example" width="600"/>](https://www.pitt.edu/~wec47/gmmdemux.html)
-        
-        ## Citation
-        If you find this code useful in your research, please consider citing:
-        
-            @article{xin2019sample,
-              title={Sample demultiplexing, multiplet detection, experiment planning and novel cell type verification in single cell sequencing},
-              author={Xin, Hongyi and Yan, Qi and Jiang, Yale and Lian, Qiuyu and Luo, Jiadi and Erb, Carla and Duerr, Richard and Chen, Kong and Chen, Wei},
-              journal={bioRxiv},
-              pages={828483},
-              year={2019},
-              publisher={Cold Spring Harbor Laboratory}
-            }
-        
-        ## Acknowledgement
-        
-        Special thank to Zhongli Xu for testing GMM-Demux!
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# GMM-Demux 
+GMM-Demux is a Gaussian-Mixture-Model-based software for processing sample barcoding data (cell hashing and MULTI-seq).
+
+GMM-Demux identifies Multi-Sample Multiplets (MSMs) in a sample barcoding dataset. Below shows an example distribution of MSMs in a PBMC scRNA-seq dataset. Orange dots in the scatter plot are MSMs.
+
+<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/GMM_simplified.png" alt="GMM-Demux example" width="600"/>
+
+## Description
+GMM-Demux removes Multi-Sample-Multiplets (MSMs) in a cell hashing dataset and estimates the percentages of Same-Sample-Multiplets (SSMs) and singlets in the remaining dataset.
+GMM-Demux also verifies if a putative cell type exists, or is it merely an artifact induced by multiplets.
+
+Multiplet-induced fake cell types are called "phony cell types".
+
+Examples of phony cell types in a PBMC CITE-seq dataset is provided in the figure below:
+
+<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/phony.png" width="600"/>
+
+In the above figure, both the CD3+CD19+ and the CD4+CD8+ cell types are multiplet-induced fake cell types.
+
+Phony type clusters have large percentages of MSMs, as above figure shows. Both phony type clusters have large MSM percentages.
+
+Percentages of MSMs are used as key features by GMM-Demux to classify GEM clusters.
+
+## Terminology
+* **Singlet**: A droplet that contains a single cell.
+
+* **MSM**: Multi-Sample Multiplet. A MSM is a multiplet that contains cells from different samples in sample barcoding. MSMs can be identified by GMM-Demux.
+
+* **SSM**: Same-Sample Multiplet. A SSM is a multiplet that contains cells from a single sample in sample barcoding. SSMs cannot be separated from singlets by sample barcoding.
+
+* **SSD**: Same-Sample Droplet. SSD is a combined category of both SSMs and singlets.
+
+* **Pure type**: a pure type cell type is a real cell type that exist in the tissue.
+
+* **Phony type**: a phony type cell type is an artificial cell type that is an artifact produced by multiplets.
+
+* **Mixture type**: a mixture type cell type is a cluster of droplets in which there exist a non-trivial fraction of phony type droplets.
+
+An illustration of the above terminologies in a PBMC dataset is provided in the figure below:
+
+<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/term.png" width="600"/>
+
+## Features
+* Remove cell-hashing-identifiable multiplets (i.e., MSMs) from the dataset.
+* Estimate the fraction of cell-hashing-unidentifiable multiplets (SSMs) in the remaining dataset (the RSSM percentage).
+* Test if a putative cell type is a pure (real) cell type or is it a phony (fake) cell type.
+
+## Example Dataset
+* An example cell hashing dataset is provided in the *example_input* folder. It contains the per-drop HTO count matrix of a 4-sample cell hashing library prep. The input folder has the same file format with the CellRanger v3 output.
+
+# Authors
+ Hongyi Xin, Qi Yan, Yale Jiang, Jiadi Luo, Carla Erb, Richard Duerr, Kong Chen* and Wei Chen*
+
+# Maintainer
+Hongyi Xin <gohongyi at gmail.edu>
+
+## Requirement
+
+GMM-Demux requires python3 (>3.5).
+
+## Install
+
+GMM-Demux can be directly installed from PyPi. Or it can be built and installed locally.
+
+### Install GMM-Demux from PyPi.
+```bash
+pip3 install --user GMM_Demux
+```
+
+In some OS, the `pip3` is linked to `pip` by default. For these OS, the installation command is simply:
+
+```bash
+pip install --user GMM_Demux
+```
+
+Check if `pip3` is linked to `pip` with `pip -V`.
+
+If one chooses to install GMM-Demux from PyPi, it is unnecessary to download GMM-Demux from github. However, we still recommend downloading the example dataset to try out GMM-Demux.
+
+### Install GMM-Demux locally using [setuptools](https://packaging.python.org/tutorials/installing-packages/) and pip3.
+
+You may choose to install GMM-Demux locally after cloning the github repository. However, **this is for advanced users only and support is not gauranteed**.
+The command is provided below:
+
+```bash
+cd <GMM-Demux dir>
+python3 setup.py sdist bdist_wheel
+pip3 install --user . 
+```
+
+### Post installation processes
+
+If this is the first time you install a python3 software through pip, make sure you add the pip binary folder to your `PATH` variable.
+Typically, the pip binary folder is located at ```~/.local/bin```.
+
+The pip binary folder might locate at a different location if the user uses virtual enviroment. Pay attention to the pip installation output.
+
+Here is an example installation output. The path of the pip binary folder is highlighted:
+<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/path.png" width="500"/>
+
+To temporarily add the pip binary folder, run the following command:
+```bash
+export PATH=~/.local/bin:$PATH
+```
+
+To permenantly add the pip library folder to your `PATH` variable, append the following line to your `.bashrc` file (assuming bash is the default shell).
+```bash
+PATH=~/.local/bin:$PATH
+```
+
+## Content
+
+The source code of GMM-Demux is supplied in the ```GMM_Demux``` folder.
+
+An example cell hashing dataset is also provided, located in the ```example_input/outs/filtered_feature_bc_matrix``` folder.
+
+An example set of hand-curated putative cell types of the above dataset are provided in the ```example_cell_types``` folder. Cell types are annotated through manual gating using surface marker expression data.
+
+An example csv format of the above cell hashing dataset is provided as the ```example_hto.csv``` file.
+
+## Usage
+
+### Case 1: Basic Usage, Remove MSMs
+Once installed, GMM-Demux is directly accessible with the ```GMM-demux``` command.
+```bash
+GMM-demux <cell_hashing_path> <HTO_names>
+```
+
+```<HTO_names>``` is a list of sample tags (HTOs) separated by ',' without whitespace.
+For example, there are four sample barcoding tags in the example cell hashing dataset.
+They are **HTO_1**, **HTO_2**, **HTO_3**, **HTO_4**. The ```<HTO_names>``` variable therefore is ```HTO_1,HTO_2,_HTO_3,HTO_4```.
+
+The non-MSM droplets (SSDs) of the dataset are stored in the *GMM_Demux_mtx* folder under the current directory by default.
+The output path can also be specified through the `-o` flag.
+
+#### Example Command 
+An example cell hashing data is provided in the *example_input* folder. <HTO_names> can be obtained from the features.tsv file.
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4
+```
+
+<HTO_names> are included in the features.tsv file. The content of the feature.tsv file is shown below.
+
+![HTO names example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/features.png)
+
+#### Output
+The default content in the output folder are the non-MSM droplets (SSDs), stored in MTX format. The output shares the same format with CellRanger 3.0. By default, the output is stored in `SSD_mtx` folder. The output location can be overwritten with the `-o` flag.
+
+### Case 2: Compute the MSM and SSM rates
+To compute the MSM and SSM rates, GMM-Demux requires the `-u` flag:
+
+* -u SUMMARY, --summary SUMMARY  Generate the statstic summary of the dataset. Requires an estimated total number of cells in the assay as input.
+ 
+The `-u` flag requires an additional <NUM_OF_CELL> argument, which is the estimated total count of cells in the single cell assay.
+
+#### Example Command
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685
+```
+
+#### Output
+Below is an example report:
+![Summary example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/summary.png)
+
+* RSSM denotes the percentage of SSMs among the remaining SSDs (after removing all MSMs). RSSM **measures the quality of the final cell hashing dataset after removing MSMs**.
+
+### Case 3: Verify if a cell type exists 
+GMM-Demux verifies if a putative cell type exists with the `-e` flag:
+
+* -e EXAMINE, --examine  EXAMINE Provide the cell list. Requires a file argument. Only executes if -u is set.
+
+The `-e` flag requires a file name, which stores the list of droplet barcodes of the putative cell type.
+
+#### Example Command
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685 -e example_cell_types/CD19+.txt
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -u 35685 -e example_cell_types/Doublets/CD3+CD4+CD19+.txt
+```
+
+#### Output
+An example output of a pure cell type:
+![Pure type example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/pure_type.png)
+
+An example output of a phony cell type:
+![Phone type example](https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/phony_type.png)
+
+### Case 4: Use the csv file format as input, instead of the mtx format 
+#### Example Command
+```bash
+GMM-demux -c example_hto.csv HTO_1,HTO_2,HTO_3,HTO_4 -u 35685
+```
+
+### Case 5: Extract droplets that are labeled by a combination of sample tags
+Extract droplets that are labeled by multiple sample barcoding tags, with the `-x` flag:
+
+* -x EXTRACT, --extract EXTRACT  Names of the sample barcoding tag(s) to extract, separated by ','. Joint tags are linked with '+'.
+
+**When `-x` is set, other functions of GMM-Demux will be turned off.**
+
+#### *Case 5a: Extract a single HTO sample*
+
+#### Example Command
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO_1
+```
+#### *Case 5b: Extract a single HTO sample that are jointly defined by multiple HTO tags*
+Use `+` to specify the joint HTO tags.
+
+#### Example Command
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO_1+HTO_2
+```
+#### *Case 5c: Extract multiple HTO samples*
+Use `,` to separate sample tags. Single tag samples can be merged with joint-tag samples.
+
+#### Example Command
+```bash
+GMM-demux example_input/outs/filtered_feature_bc_matrix HTO_1,HTO_2,HTO_3,HTO_4 -x HTO3,HTO_1+HTO_2,HTO_1+HTO_4+HTO_2
+```
+
+## Optional Arguments
+* -h: show help information.
+* -f FULL, --full FULL  Generate the full classification report. Require a path argument.
+* -s SIMPLIFIED, --simplified SIMPLIFIED  Generate the simplified classification report. Require a path argument.
+* -o OUTPUT, --output OUTPUT  The path for storing the Same-Sample-Droplets (SSDs). SSDs are stored in mtx format. Requires a path argument. Default path: SSD_mtx.
+* -r REPORT, --report REPORT  Specify the file to store summary report. Require a file argument.
+* -c CSV, --csv  Take input in csv format, instead of mmx format.
+* -s SKIP, --skip FULL\_REPORT  Load a full classification report and skip the mtx folder as input. Require a path argument.
+* -a AMBIGUOUS, --ambiguous AMBIGUOUS  The estimated chance of having a phony GEM getting included in a pure type GEM cluster by the clustering algorithm. Requires a float in (0, 1). Default value: 0.05. Only executes if -e executes.
+* -t THRESHOLD, --threshold THRESHOLD  Provide the confidence threshold value. Requires a float in (0,1). Default value: 0.8.
+
+## Parsing the Classification Output
+There are two files in a classification output folder. A config file (ending with .config) and a classification file (ending with .csv).
+
+The classification file contains the label of each droplet as well as the probability of the classification. The classification is represented with numbers which are explained in the config file.
+
+Below shows the classification output of the example data:
+
+<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/class_output.png" width="600"/>
+ 
+## Online Cell Hashing Experiment Planner
+A GMM-Demux based online cell hashing experiment planner is publically accessible at [here](https://www.pitt.edu/~wec47/gmmdemux.html).
+
+[<img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/planner.png" alt="Online explanner example" width="600"/>](https://www.pitt.edu/~wec47/gmmdemux.html)
+
+## Citation
+If you find this code useful in your research, please consider citing:
+
+    @article{xin2019sample,
+      title={Sample demultiplexing, multiplet detection, experiment planning and novel cell type verification in single cell sequencing},
+      author={Xin, Hongyi and Yan, Qi and Jiang, Yale and Lian, Qiuyu and Luo, Jiadi and Erb, Carla and Duerr, Richard and Chen, Kong and Chen, Wei},
+      journal={bioRxiv},
+      pages={828483},
+      year={2019},
+      publisher={Cold Spring Harbor Laboratory}
+    }
+
+## Acknowledgement
+
+Special thank to Zhongli Xu for testing GMM-Demux!
```

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux.egg-info/SOURCES.txt` & `GMM_Demux-0.2.2.0/GMM_Demux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/README.md` & `GMM_Demux-0.2.2.0/GMM_Demux.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: GMM-Demux
+Version: 0.2.2.0
+Summary: A multiplet removal tool for processing cell hashing data
+Home-page: https://github.com/CHPGenetics/GMM-demux
+Author: Hongyi Xin
+Author-email: gohongyi@gmail.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GMM-Demux 
 GMM-Demux is a Gaussian-Mixture-Model-based software for processing sample barcoding data (cell hashing and MULTI-seq).
 
 GMM-Demux identifies Multi-Sample Multiplets (MSMs) in a sample barcoding dataset. Below shows an example distribution of MSMs in a PBMC scRNA-seq dataset. Orange dots in the scatter plot are MSMs.
 
 <img src="https://raw.githubusercontent.com/CHPGenetics/GMM-Demux/master/GMM_simplified.png" alt="GMM-Demux example" width="600"/>
```

### Comparing `GMM_Demux-0.2.1.3/term.png` & `GMM_Demux-0.2.2.0/term.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/setup.py` & `GMM_Demux-0.2.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GMM_Demux",
-    version="0.2.1.3",
+    version="0.2.2.0",
     author="Hongyi Xin",
     author_email="gohongyi@gmail.com",
     description="A multiplet removal tool for processing cell hashing data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CHPGenetics/GMM-demux",
     packages=setuptools.find_packages(),
@@ -21,16 +21,16 @@
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        "pandas>=0.25",
-        "numpy",
+        "pandas>=1.4.3",
+        "numpy>=1.22.4",
         "scipy",
         "tabulate",
         "argparse",
         "statistics",
         "BitVector",
         "sklearn"
     ]
```

### Comparing `GMM_Demux-0.2.1.3/phony.png` & `GMM_Demux-0.2.2.0/phony.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_hto.csv` & `GMM_Demux-0.2.2.0/example_hto.csv`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD11+CD14-CD16-.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD11+CD14-CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD56+CD16-.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD3+CD4+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD3+CD4+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD14+CD56+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD14+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD14+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD56+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD56+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD8+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD8+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD14+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD14+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD4+CD19+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/Doublets/CD3+CD8+CD19+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD14+CD16+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD3+CD8+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD3+CD8+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD3+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD3+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD14+CD16-.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD19+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/example_cell_types/CD56+CD16+.txt` & `GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/summary.png` & `GMM_Demux-0.2.2.0/summary.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/GMM_Demux.py` & `GMM_Demux-0.2.2.0/GMM_Demux/GMM_Demux.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     parser.add_argument("-c", "--csv", help="Take input in csv format, instead of mmx format.", action='store_true')
     parser.add_argument("-t", "--threshold", help="Provide the confidence threshold value. Requires a float in (0,1). Default value: 0.8", type=float, default=0.8)
     parser.add_argument("-s", "--simplified", help="Generate the simplified classification report. Requires a path argument.", type=str)
     parser.add_argument("-u", "--summary", help = "Generate the statstic summary of the dataset. Including MSM, SSM rates. Requires an estimated total number of cells in the assay as input.", type=int)
     parser.add_argument("-r", "--report", help="Store the data summary report. Requires a file argument. Only executes if -u is set.", type=str)
     parser.add_argument("-e", "--examine", help="Provide the cell list. Requires a file argument. Only executes if -u is set.", type=str)
     parser.add_argument("-a", "--ambiguous", help="The estimated chance of having a phony GEM getting included in a pure type GEM cluster by the clustering algorithm. Requires a float in (0, 1). Default value: 0.05. Only executes if -e executes.", type=float, default=0.05)
+    parser.add_argument("-rs", "--random_seed", help = "If provided, this is passed to the GaussianMixture random_state parameter.", default=None, type=int)
     
     print("==============================GMM-Demux Initialization==============================")
 
     args = parser.parse_args()
 
     confidence_threshold = args.threshold
     print("Confidence threshold:", confidence_threshold)
@@ -66,15 +67,15 @@
         GEM_num = GMM_df.shape[0]
         sample_num = GMM_df.shape[1]
 
 
         ####### Run classifier #######
         base_bv_array = compute_venn.obtain_base_bv_array(sample_num)
         #print([int(i) for i in base_bv_array])
-        (high_array, low_array) = classify_drops.obtain_arrays(GMM_df)
+        (high_array, low_array) = classify_drops.obtain_arrays(GMM_df, args.random_seed)
 
         # Obtain extract array.
         if args.extract:
             extract_id_ary = []
             tag_name_ary = []
 
             for tag_name in args.extract.split(','):
```

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/GMM_IO.py` & `GMM_Demux-0.2.2.0/GMM_Demux/GMM_IO.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/estimator.py` & `GMM_Demux-0.2.2.0/GMM_Demux/estimator.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/check_multi_comp.py` & `GMM_Demux-0.2.2.0/GMM_Demux/check_multi_comp.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/classify_drops.py` & `GMM_Demux-0.2.2.0/GMM_Demux/classify_drops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 import numpy as np
 
 import pandas as pd
 from scipy import stats
 from sys import argv
 from sklearn.mixture import GaussianMixture
 import os
-from math import log2
+from math import log2, sqrt
 
 from GMM_Demux import check_multi_comp
 from GMM_Demux import compute_venn
 
 
-def obtain_arrays(data):
+def obtain_arrays(data, random_seed):
     gmm = []
     high_array = []
     low_array = []
 
     for i in range(data.shape[1]):
         X = data.iloc[:,i].values[:, np.newaxis]
 
         # GMM values
+<<<<<<< HEAD
         gmm.append(GaussianMixture(2).fit(X))
+        # x = np.linspace(-6, 6, 1000)[:, np.newaxis]
+        # logprob= gmm[-1].score_samples(x)
+        # responsibilities = gmm[-1].predict_proba(x)
+        # pdf = np.exp(logprob)
+        # pdf_individual = responsibilities * pdf[:, np.newaxis]
+        # print(pdf_individual)
+        # print(gmm[-1].means_)
+        # print(gmm[-1].covariances_)
+=======
+        gmm.append(GaussianMixture(2, random_state = random_seed).fit(X))
         x = np.linspace(-6, 6, 1000)[:, np.newaxis]
         logprob= gmm[-1].score_samples(x)
         responsibilities = gmm[-1].predict_proba(x)
         pdf = np.exp(logprob)
         pdf_individual = responsibilities * pdf[:, np.newaxis]
         #print(pdf_individual)
 
         #print(gmm[-1].means_)
+>>>>>>> fdd6aec963298f6429498db06ad43c000df219c9
 
         # Extract prob
         high_idx = np.argmax(gmm[-1].means_, axis=0)[0]
         post_prob = gmm[-1].predict_proba(X)
+
         high_array.append(post_prob[np.arange(post_prob.shape[0]), np.full(post_prob.shape[0], high_idx)])
+
+        # Correct outliers
+        high_outlier_cutoff = gmm[-1].means_[high_idx] + sqrt(gmm[-1].covariances_[high_idx][0])
+        high_outlier_idx = np.argwhere(X > high_outlier_cutoff)[:,0].ravel()
+        low_outlier_cutoff = gmm[-1].means_[1-high_idx] - sqrt(gmm[-1].covariances_[1-high_idx][0])
+        low_outlier_idx = np.argwhere(X < low_outlier_cutoff)[:,0].ravel()
+
+        high_array[-1][high_outlier_idx] = 1.0
+        high_array[-1][low_outlier_idx] = 0.0
+
         low_array.append(np.full(post_prob.shape[0], 1.0) - high_array[-1])
 
+        
     return high_array, low_array
 
 
 def classify_drops(base_bv_array, high_array, low_array, sample_num, GEM_num, index, column):
 
     classified_ary = np.full(GEM_num, 0)
     confidence_ary = np.full(GEM_num, 0.0)
```

### Comparing `GMM_Demux-0.2.1.3/GMM_Demux/compute_venn.py` & `GMM_Demux-0.2.2.0/GMM_Demux/compute_venn.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/GMM_simplified.png` & `GMM_Demux-0.2.2.0/GMM_simplified.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/planner.png` & `GMM_Demux-0.2.2.0/planner.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/path.png` & `GMM_Demux-0.2.2.0/path.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.1.3/LICENSE` & `GMM_Demux-0.2.2.0/LICENSE`

 * *Files identical despite different names*

