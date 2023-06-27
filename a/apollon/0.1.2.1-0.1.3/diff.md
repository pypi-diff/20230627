# Comparing `tmp/apollon-0.1.2.1.tar.gz` & `tmp/apollon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollon-0.1.2.1.tar", last modified: Mon Mar 22 05:38:46 2021, max compression
+gzip compressed data, was "apollon-0.1.3.tar", last modified: Tue Jun 27 13:15:55 2023, max compression
```

## Comparing `apollon-0.1.2.1.tar` & `apollon-0.1.3.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.306300 apollon-0.1.2.1/
--rw-r--r--   0 michael    (501) staff       (20)      714 2021-03-19 13:53:34.000000 apollon-0.1.2.1/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1522 2021-03-19 13:53:34.000000 apollon-0.1.2.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)       74 2021-03-19 13:53:34.000000 apollon-0.1.2.1/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     1898 2021-03-22 05:38:46.306504 apollon-0.1.2.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      627 2021-03-19 13:58:43.000000 apollon-0.1.2.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.145229 apollon-0.1.2.1/include/
--rw-r--r--   0 michael    (501) staff       (20)     1774 2021-03-19 13:53:34.000000 apollon-0.1.2.1/include/cdim.h
--rw-r--r--   0 michael    (501) staff       (20)      543 2021-03-19 13:53:34.000000 apollon-0.1.2.1/include/correlogram.h
--rw-r--r--   0 michael    (501) staff       (20)      269 2021-03-19 13:53:34.000000 apollon-0.1.2.1/include/distance.h
--rw-r--r--   0 michael    (501) staff       (20)      103 2021-03-19 13:53:34.000000 apollon-0.1.2.1/pyproject.toml
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.145619 apollon-0.1.2.1/scripts/
--rwxr-xr-x   0 michael    (501) staff       (20)     3280 2021-03-22 05:28:32.000000 apollon-0.1.2.1/scripts/apollon
--rw-r--r--   0 michael    (501) staff       (20)     1402 2021-03-22 05:38:46.307386 apollon-0.1.2.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      645 2021-03-19 13:53:34.000000 apollon-0.1.2.1/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.141195 apollon-0.1.2.1/src/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.207044 apollon-0.1.2.1/src/apollon/
--rw-r--r--   0 michael    (501) staff       (20)      324 2021-03-19 13:58:43.000000 apollon-0.1.2.1/src/apollon/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      678 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/_defaults.py
--rw-r--r--   0 michael    (501) staff       (20)     8339 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/aplot.py
--rw-r--r--   0 michael    (501) staff       (20)     4355 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/audio.py
--rw-r--r--   0 michael    (501) staff       (20)     4988 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/container.py
--rw-r--r--   0 michael    (501) staff       (20)      945 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/datasets.py
--rw-r--r--   0 michael    (501) staff       (20)     3829 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/fractal.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.212433 apollon-0.1.2.1/src/apollon/hmm/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/hmm/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    14664 2021-03-22 05:22:26.000000 apollon-0.1.2.1/src/apollon/hmm/poisson.py
--rw-r--r--   0 michael    (501) staff       (20)    14319 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/hmm/utilities.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.214879 apollon-0.1.2.1/src/apollon/io/
--rw-r--r--   0 michael    (501) staff       (20)       19 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/io/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     6240 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/io/io.py
--rw-r--r--   0 michael    (501) staff       (20)     3927 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/io/json.py
--rw-r--r--   0 michael    (501) staff       (20)     8907 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/onsets.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.218920 apollon-0.1.2.1/src/apollon/schema/
--rw-r--r--   0 michael    (501) staff       (20)      934 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/schema/corrdim.schema.json
--rw-r--r--   0 michael    (501) staff       (20)      725 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/schema/corrgram.schema.json
--rw-r--r--   0 michael    (501) staff       (20)      793 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/schema/dft_params.schema.json
--rw-r--r--   0 michael    (501) staff       (20)      784 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/schema/ndarray.schema.json
--rw-r--r--   0 michael    (501) staff       (20)     1461 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/schema/stft_params.schema.json
--rw-r--r--   0 michael    (501) staff       (20)    15145 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/segment.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.229397 apollon-0.1.2.1/src/apollon/signal/
--rw-r--r--   0 michael    (501) staff       (20)      265 2021-03-21 10:29:57.000000 apollon-0.1.2.1/src/apollon/signal/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     6605 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/_features_module.c
--rw-r--r--   0 michael    (501) staff       (20)     8864 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/cdim.c
--rw-r--r--   0 michael    (501) staff       (20)     1274 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/container.py
--rw-r--r--   0 michael    (501) staff       (20)     1741 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/correlogram.c
--rw-r--r--   0 michael    (501) staff       (20)     3281 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/critical_bands.py
--rw-r--r--   0 michael    (501) staff       (20)    13736 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/features.py
--rw-r--r--   0 michael    (501) staff       (20)     1342 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/filter.py
--rw-r--r--   0 michael    (501) staff       (20)     8291 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/spectral.py
--rw-r--r--   0 michael    (501) staff       (20)     7506 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/signal/tools.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.305922 apollon-0.1.2.1/src/apollon/som/
--rw-r--r--   0 michael    (501) staff       (20)      143 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/som/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4346 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/_distance_module.c
--rw-r--r--   0 michael    (501) staff       (20)     1565 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/datasets.py
--rw-r--r--   0 michael    (501) staff       (20)      194 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/defaults.py
--rw-r--r--   0 michael    (501) staff       (20)      673 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/distance.c
--rw-r--r--   0 michael    (501) staff       (20)     4335 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/som/neighbors.py
--rw-r--r--   0 michael    (501) staff       (20)     7303 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/som/plot.py
--rw-r--r--   0 michael    (501) staff       (20)    14153 2021-03-22 05:28:32.000000 apollon-0.1.2.1/src/apollon/som/som.py
--rw-r--r--   0 michael    (501) staff       (20)     1367 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/topologies.py
--rw-r--r--   0 michael    (501) staff       (20)     8448 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/som/utilities.py
--rw-r--r--   0 michael    (501) staff       (20)     8182 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/tools.py
--rw-r--r--   0 michael    (501) staff       (20)      723 2021-03-19 13:53:34.000000 apollon-0.1.2.1/src/apollon/types.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-03-22 05:38:46.210332 apollon-0.1.2.1/src/apollon.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1898 2021-03-22 05:38:46.000000 apollon-0.1.2.1/src/apollon.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1568 2021-03-22 05:38:46.000000 apollon-0.1.2.1/src/apollon.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2021-03-22 05:38:46.000000 apollon-0.1.2.1/src/apollon.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2020-06-03 13:46:44.000000 apollon-0.1.2.1/src/apollon.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)      126 2021-03-22 05:38:46.000000 apollon-0.1.2.1/src/apollon.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       28 2021-03-22 05:38:46.000000 apollon-0.1.2.1/src/apollon.egg-info/top_level.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.962967 apollon-0.1.3/
+-rw-r--r--   0 pmind      (502) staff       (20)     1484 2023-06-11 11:45:26.000000 apollon-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 pmind      (502) staff       (20)     1522 2023-06-27 09:43:23.000000 apollon-0.1.3/LICENSE.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       74 2023-06-11 11:45:26.000000 apollon-0.1.3/MANIFEST.in
+-rw-r--r--   0 pmind      (502) staff       (20)     3337 2023-06-27 13:15:55.961408 apollon-0.1.3/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)      517 2023-06-11 11:45:26.000000 apollon-0.1.3/README.md
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.907177 apollon-0.1.3/include/
+-rw-r--r--   0 pmind      (502) staff       (20)     1774 2023-06-11 11:45:26.000000 apollon-0.1.3/include/cdim.h
+-rw-r--r--   0 pmind      (502) staff       (20)      543 2023-06-11 11:45:26.000000 apollon-0.1.3/include/correlogram.h
+-rw-r--r--   0 pmind      (502) staff       (20)      269 2023-06-11 11:45:26.000000 apollon-0.1.3/include/distance.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1256 2023-06-27 11:02:41.000000 apollon-0.1.3/pyproject.toml
+-rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-27 13:15:55.963478 apollon-0.1.3/setup.cfg
+-rw-r--r--   0 pmind      (502) staff       (20)      551 2023-06-27 11:01:01.000000 apollon-0.1.3/setup.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.896547 apollon-0.1.3/src/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.914255 apollon-0.1.3/src/apollon/
+-rw-r--r--   0 pmind      (502) staff       (20)      324 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)      678 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/_defaults.py
+-rw-r--r--   0 pmind      (502) staff       (20)     8339 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/aplot.py
+-rw-r--r--   0 pmind      (502) staff       (20)     4355 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/audio.py
+-rw-r--r--   0 pmind      (502) staff       (20)     4988 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/container.py
+-rw-r--r--   0 pmind      (502) staff       (20)      945 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/datasets.py
+-rw-r--r--   0 pmind      (502) staff       (20)     3829 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/fractal.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.919115 apollon-0.1.3/src/apollon/hmm/
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/hmm/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)    14664 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/hmm/poisson.py
+-rw-r--r--   0 pmind      (502) staff       (20)    14319 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/hmm/utilities.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.922001 apollon-0.1.3/src/apollon/io/
+-rw-r--r--   0 pmind      (502) staff       (20)       19 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/io/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)     6240 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/io/io.py
+-rw-r--r--   0 pmind      (502) staff       (20)     3927 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/io/json.py
+-rw-r--r--   0 pmind      (502) staff       (20)     8907 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/onsets.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.928967 apollon-0.1.3/src/apollon/schema/
+-rw-r--r--   0 pmind      (502) staff       (20)      934 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/corrdim.schema.json
+-rw-r--r--   0 pmind      (502) staff       (20)      725 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/corrgram.schema.json
+-rw-r--r--   0 pmind      (502) staff       (20)      793 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/dft_params.schema.json
+-rw-r--r--   0 pmind      (502) staff       (20)      784 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/ndarray.schema.json
+-rw-r--r--   0 pmind      (502) staff       (20)     1461 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/stft_params.schema.json
+-rw-r--r--   0 pmind      (502) staff       (20)    15145 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/segment.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.938725 apollon-0.1.3/src/apollon/signal/
+-rw-r--r--   0 pmind      (502) staff       (20)      265 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)     6605 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/_features_module.c
+-rw-r--r--   0 pmind      (502) staff       (20)     8864 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/cdim.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1274 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/container.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1741 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/correlogram.c
+-rw-r--r--   0 pmind      (502) staff       (20)     3281 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/critical_bands.py
+-rw-r--r--   0 pmind      (502) staff       (20)    13736 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/features.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1342 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/filter.py
+-rw-r--r--   0 pmind      (502) staff       (20)     8291 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/spectral.py
+-rw-r--r--   0 pmind      (502) staff       (20)     7506 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/tools.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.952423 apollon-0.1.3/src/apollon/som/
+-rw-r--r--   0 pmind      (502) staff       (20)      143 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)     4346 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/som/_distance_module.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1565 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/datasets.py
+-rw-r--r--   0 pmind      (502) staff       (20)      194 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/defaults.py
+-rw-r--r--   0 pmind      (502) staff       (20)      673 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/som/distance.c
+-rw-r--r--   0 pmind      (502) staff       (20)     4335 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/neighbors.py
+-rw-r--r--   0 pmind      (502) staff       (20)     7303 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/plot.py
+-rw-r--r--   0 pmind      (502) staff       (20)    14153 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/som.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1367 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/topologies.py
+-rw-r--r--   0 pmind      (502) staff       (20)     8448 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/utilities.py
+-rw-r--r--   0 pmind      (502) staff       (20)     8182 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/tools.py
+-rw-r--r--   0 pmind      (502) staff       (20)      723 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/types.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.917319 apollon-0.1.3/src/apollon.egg-info/
+-rw-r--r--   0 pmind      (502) staff       (20)     3337 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)     1653 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/SOURCES.txt
+-rw-r--r--   0 pmind      (502) staff       (20)        1 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/dependency_links.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      112 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/requires.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       28 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/top_level.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.960322 apollon-0.1.3/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)     2698 2023-06-11 11:45:26.000000 apollon-0.1.3/tests/test_audio.py
+-rw-r--r--   0 pmind      (502) staff       (20)      917 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_container.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1985 2023-06-27 10:58:49.000000 apollon-0.1.3/tests/test_io.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1494 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_onsets.py
+-rw-r--r--   0 pmind      (502) staff       (20)     3362 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_schema.py
+-rw-r--r--   0 pmind      (502) staff       (20)     5042 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_segment.py
+-rw-r--r--   0 pmind      (502) staff       (20)      445 2023-06-11 11:45:26.000000 apollon-0.1.3/tests/test_tools.py
```

### Comparing `apollon-0.1.2.1/LICENSE.txt` & `apollon-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/PKG-INFO` & `apollon-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,73 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.2.1
-Summary: Feature extraction frame work for content-based music analysis.
-Home-page: UNKNOWN
-Author: Michael Blaß
-Author-email: mblass@posteo.net
+Version: 0.1.3
+Summary: Feature extraction frame work for content-based music analysis
+Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
-Project-URL: Source code, https://gitlab.rrz.uni-hamburg.de/bal7668/apollon
-Project-URL: Bug Tracker, https://gitlab.rrz.uni-hamburg.de/bal7668/apollon/-/issues
-Description: # Apollon
-        Apollon is a Python framework for audio feature extraction and music similarity estimation. It 
-        includes subpackages for
-        
-        * Audio feature extraction
-        * Hidden Markov Models
-        * Self-Organizing Map
-        
-        ## 1. Installation
-        ### 1.1 Install from PyPi
-        The latest version of apollon is available on PyPi. 
-        Download apollon or clone this repository. Navigate the package's root directory
-        and install apollon using pip.
-        ```
-        cd path/to/apollon_repo
-        pip install .
-        ```
-        Note that the period on the end of the last line is necessary.
         
-        ## 2. Documentation
-        Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
+        Copyright (c) 2019, Michael Blaß 
+        All rights reserved.
         
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Repository, http://github.com/ifsm/apollo
+Project-URL: Documentation, https://apollon.readthedocs.io
 Keywords: music,analysis,feature extraction
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Apollon
+Apollon is a Python framework for audio feature extraction and music similarity
+estimation. It includes subpackages for
+
+* Audio feature extraction
+* Hidden Markov Models
+* Self-Organizing Map
+
+## 1. Installation
+### 1.1 Install from PyPi
+The latest version of apollon is available on PyPi. Just open a terminal an run
+the following command to download and install apollon:
+
+```
+pip install apollon 
+```
+
+## 2. Documentation
+Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.2.1/include/cdim.h` & `apollon-0.1.3/include/cdim.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/include/correlogram.h` & `apollon-0.1.3/include/correlogram.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/_defaults.py` & `apollon-0.1.3/src/apollon/_defaults.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/aplot.py` & `apollon-0.1.3/src/apollon/aplot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/audio.py` & `apollon-0.1.3/src/apollon/audio.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/container.py` & `apollon-0.1.3/src/apollon/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/datasets.py` & `apollon-0.1.3/src/apollon/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/fractal.py` & `apollon-0.1.3/src/apollon/fractal.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/hmm/poisson.py` & `apollon-0.1.3/src/apollon/hmm/poisson.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/hmm/utilities.py` & `apollon-0.1.3/src/apollon/hmm/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/io/io.py` & `apollon-0.1.3/src/apollon/io/io.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/io/json.py` & `apollon-0.1.3/src/apollon/io/json.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/onsets.py` & `apollon-0.1.3/src/apollon/onsets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/schema/corrdim.schema.json` & `apollon-0.1.3/src/apollon/schema/corrdim.schema.json`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/schema/corrgram.schema.json` & `apollon-0.1.3/src/apollon/schema/corrgram.schema.json`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/schema/dft_params.schema.json` & `apollon-0.1.3/src/apollon/schema/dft_params.schema.json`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/schema/ndarray.schema.json` & `apollon-0.1.3/src/apollon/schema/ndarray.schema.json`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/schema/stft_params.schema.json` & `apollon-0.1.3/src/apollon/schema/stft_params.schema.json`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/segment.py` & `apollon-0.1.3/src/apollon/segment.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/_features_module.c` & `apollon-0.1.3/src/apollon/signal/_features_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/cdim.c` & `apollon-0.1.3/src/apollon/signal/cdim.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/container.py` & `apollon-0.1.3/src/apollon/signal/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/correlogram.c` & `apollon-0.1.3/src/apollon/signal/correlogram.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/critical_bands.py` & `apollon-0.1.3/src/apollon/signal/critical_bands.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/features.py` & `apollon-0.1.3/src/apollon/signal/features.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/filter.py` & `apollon-0.1.3/src/apollon/signal/filter.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/spectral.py` & `apollon-0.1.3/src/apollon/signal/spectral.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/signal/tools.py` & `apollon-0.1.3/src/apollon/signal/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/_distance_module.c` & `apollon-0.1.3/src/apollon/som/_distance_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/datasets.py` & `apollon-0.1.3/src/apollon/som/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/distance.c` & `apollon-0.1.3/src/apollon/som/distance.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/neighbors.py` & `apollon-0.1.3/src/apollon/som/neighbors.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/plot.py` & `apollon-0.1.3/src/apollon/som/plot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/som.py` & `apollon-0.1.3/src/apollon/som/som.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/topologies.py` & `apollon-0.1.3/src/apollon/som/topologies.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/som/utilities.py` & `apollon-0.1.3/src/apollon/som/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/tools.py` & `apollon-0.1.3/src/apollon/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon/types.py` & `apollon-0.1.3/src/apollon/types.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.2.1/src/apollon.egg-info/PKG-INFO` & `apollon-0.1.3/src/apollon.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,73 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.2.1
-Summary: Feature extraction frame work for content-based music analysis.
-Home-page: UNKNOWN
-Author: Michael Blaß
-Author-email: mblass@posteo.net
+Version: 0.1.3
+Summary: Feature extraction frame work for content-based music analysis
+Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
-Project-URL: Source code, https://gitlab.rrz.uni-hamburg.de/bal7668/apollon
-Project-URL: Bug Tracker, https://gitlab.rrz.uni-hamburg.de/bal7668/apollon/-/issues
-Description: # Apollon
-        Apollon is a Python framework for audio feature extraction and music similarity estimation. It 
-        includes subpackages for
-        
-        * Audio feature extraction
-        * Hidden Markov Models
-        * Self-Organizing Map
-        
-        ## 1. Installation
-        ### 1.1 Install from PyPi
-        The latest version of apollon is available on PyPi. 
-        Download apollon or clone this repository. Navigate the package's root directory
-        and install apollon using pip.
-        ```
-        cd path/to/apollon_repo
-        pip install .
-        ```
-        Note that the period on the end of the last line is necessary.
         
-        ## 2. Documentation
-        Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
+        Copyright (c) 2019, Michael Blaß 
+        All rights reserved.
         
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Repository, http://github.com/ifsm/apollo
+Project-URL: Documentation, https://apollon.readthedocs.io
 Keywords: music,analysis,feature extraction
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Apollon
+Apollon is a Python framework for audio feature extraction and music similarity
+estimation. It includes subpackages for
+
+* Audio feature extraction
+* Hidden Markov Models
+* Self-Organizing Map
+
+## 1. Installation
+### 1.1 Install from PyPi
+The latest version of apollon is available on PyPi. Just open a terminal an run
+the following command to download and install apollon:
+
+```
+pip install apollon 
+```
+
+## 2. Documentation
+Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.2.1/src/apollon.egg-info/SOURCES.txt` & `apollon-0.1.3/src/apollon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 include/cdim.h
 include/correlogram.h
 include/distance.h
-scripts/apollon
 src/apollon/__init__.py
 src/apollon/_defaults.py
 src/apollon/aplot.py
 src/apollon/audio.py
 src/apollon/container.py
 src/apollon/datasets.py
 src/apollon/fractal.py
 src/apollon/onsets.py
 src/apollon/segment.py
 src/apollon/tools.py
 src/apollon/types.py
 src/apollon.egg-info/PKG-INFO
 src/apollon.egg-info/SOURCES.txt
 src/apollon.egg-info/dependency_links.txt
-src/apollon.egg-info/not-zip-safe
 src/apollon.egg-info/requires.txt
 src/apollon.egg-info/top_level.txt
 src/apollon/hmm/__init__.py
 src/apollon/hmm/poisson.py
 src/apollon/hmm/utilities.py
 src/apollon/io/__init__.py
 src/apollon/io/io.py
@@ -52,8 +49,15 @@
 src/apollon/som/datasets.py
 src/apollon/som/defaults.py
 src/apollon/som/distance.c
 src/apollon/som/neighbors.py
 src/apollon/som/plot.py
 src/apollon/som/som.py
 src/apollon/som/topologies.py
-src/apollon/som/utilities.py
+src/apollon/som/utilities.py
+tests/test_audio.py
+tests/test_container.py
+tests/test_io.py
+tests/test_onsets.py
+tests/test_schema.py
+tests/test_segment.py
+tests/test_tools.py
```

