# Comparing `tmp/siibra-0.4a57.tar.gz` & `tmp/siibra-0.4a58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a57.tar", last modified: Mon Jun 19 11:33:05 2023, max compression
+gzip compressed data, was "siibra-0.4a58.tar", last modified: Tue Jun 27 11:07:25 2023, max compression
```

## Comparing `siibra-0.4a57.tar` & `siibra-0.4a58.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.998380 siibra-0.4a57/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 11:31:45.000000 siibra-0.4a57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-19 11:31:45.000000 siibra-0.4a57/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-19 11:33:04.998380 siibra-0.4a57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-19 11:31:45.000000 siibra-0.4a57/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:33:04.998380 siibra-0.4a57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-19 11:31:45.000000 siibra-0.4a57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/streamline_lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/connectivity/tracer_connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.994380 siibra-0.4a57/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.994380 siibra-0.4a57/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.994380 siibra-0.4a57/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.994380 siibra-0.4a57/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.994380 siibra-0.4a57/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.998380 siibra-0.4a57/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.998380 siibra-0.4a57/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    42302 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-19 11:31:45.000000 siibra-0.4a57/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.990380 siibra-0.4a57/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-19 11:33:04.000000 siibra-0.4a57/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-19 11:33:04.000000 siibra-0.4a57/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:33:04.000000 siibra-0.4a57/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-19 11:33:04.000000 siibra-0.4a57/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 11:33:04.000000 siibra-0.4a57/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:33:04.998380 siibra-0.4a57/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-19 11:31:45.000000 siibra-0.4a57/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.531540 siibra-0.4a58/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 11:05:55.000000 siibra-0.4a58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-27 11:05:55.000000 siibra-0.4a58/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-27 11:07:25.527539 siibra-0.4a58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-27 11:05:55.000000 siibra-0.4a58/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:07:25.531540 siibra-0.4a58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 11:05:55.000000 siibra-0.4a58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/tracer_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42497 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-27 11:05:55.000000 siibra-0.4a58/test/test_siibra.py
```

### Comparing `siibra-0.4a57/LICENSE` & `siibra-0.4a58/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/PKG-INFO` & `siibra-0.4a58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a57
+Version: 0.4a58
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a57/README.rst` & `siibra-0.4a58/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/setup.py` & `siibra-0.4a58/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/__init__.py` & `siibra-0.4a58/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/commons.py` & `siibra-0.4a58/siibra/commons.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/configuration/__init__.py` & `siibra-0.4a58/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/configuration/configuration.py` & `siibra-0.4a58/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/configuration/factory.py` & `siibra-0.4a58/siibra/configuration/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 from os import path
 import json
 import numpy as np
 from typing import List, Type
 import pandas as pd
 from io import BytesIO
 
-MIN_VOLUMES_FOR_SPARSE_MAP = 125
-
 BUILDFUNCS = {
     "juelich/iav/atlas/v1.0.0": "build_atlas",
     "siibra/space/v0.0.1": "build_space",
     "siibra/parcellation/v0.0.1": "build_parcellation",
     "siibra/volume/v0.0.1": "build_volume",
     "siibra/map/v0.0.1": "build_map",
     "siibra/snapshots/ebrainsquery/v1": "build_ebrains_dataset",
@@ -70,14 +68,18 @@
             result.append(
                 datasets.EbrainsDataset(id=spec["ebrains"]["minds/core/dataset/v1.0.0"])
             )
         if "openminds/DatasetVersion" in spec.get("ebrains", {}):
             result.append(
                 datasets.EbrainsV3DatasetVersion(id=spec["ebrains"]["openminds/DatasetVersion"])
             )
+        if "openminds/Dataset" in spec.get("ebrains", {}):
+            result.append(
+                datasets.EbrainsV3Dataset(id=spec["ebrains"]["openminds/Dataset"])
+            )
         return result
 
     @classmethod
     def extract_volumes(cls, spec, space_id: str = None, name: str = None):
         volume_specs = spec.get("volumes", [])
         for vspec in volume_specs:
             if space_id:
@@ -265,52 +267,18 @@
         # maps have no configured identifier - we require the spec filename to build one
         assert "filename" in spec
         basename = path.splitext(path.basename(spec['filename']))[0]
         name = basename.replace('-', ' ').replace('_', ' ')
         identifier = f"{spec['@type'].replace('/','-')}_{basename}"
         volumes = cls.extract_volumes(spec)
 
-        if ("sparsemap" in spec) and spec.get("sparsemap").get("is_sparsemap"):
-            Maptype = sparsemap.SparseMap
-            return Maptype(
-                identifier=spec.get("@id", identifier),
-                name=spec.get("name", name),
-                space_spec=spec.get("space", {}),
-                parcellation_spec=spec.get("parcellation", {}),
-                indices=spec.get("indices", {}),
-                volumes=volumes,
-                shortname=spec.get("shortName", ""),
-                description=spec.get("description"),
-                modality=spec.get("modality"),
-                publications=spec.get("publications", []),
-                datasets=cls.extract_datasets(spec),
-                is_cached=spec.get("sparsemap").get("cached", False),
-                cache_url=spec.get("sparsemap").get("url", "")
-            )
-
-        Maptype = parcellationmap.Map
-        if len(volumes) > MIN_VOLUMES_FOR_SPARSE_MAP:
-            logger.debug(
-                f"Using sparse map for {spec.get('filename')} to code its "
-                f"{len(volumes)} volumes efficiently."
-            )
+        if spec.get("sparsemap", {}).get("is_sparsemap"):
             Maptype = sparsemap.SparseMap
         else:
-            max_z = max(
-                d.get('z', 0)
-                for l in spec.get("indices", {}).values()
-                for d in l
-            ) + 1
-            if max_z > MIN_VOLUMES_FOR_SPARSE_MAP:
-                logger.debug(
-                    f"Using sparse map for {spec.get('filename')} to code its "
-                    f"{max_z} z levels efficiently."
-                )
-                Maptype = sparsemap.SparseMap
-
+            Maptype = parcellationmap.Map
         return Maptype(
             identifier=spec.get("@id", identifier),
             name=spec.get("name", name),
             space_spec=spec.get("space", {}),
             parcellation_spec=spec.get("parcellation", {}),
             indices=spec.get("indices", {}),
             volumes=volumes,
```

### Comparing `siibra-0.4a57/siibra/core/__init__.py` & `siibra-0.4a58/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/core/atlas.py` & `siibra-0.4a58/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/core/concept.py` & `siibra-0.4a58/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/core/parcellation.py` & `siibra-0.4a58/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/core/region.py` & `siibra-0.4a58/siibra/core/region.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/core/space.py` & `siibra-0.4a58/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/__init__.py` & `siibra-0.4a58/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/anchor.py` & `siibra-0.4a58/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/__init__.py` & `siibra-0.4a58/siibra/features/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a58/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a58/siibra/features/connectivity/regional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a58/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a58/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/connectivity/tracer_connectivity.py` & `siibra-0.4a58/siibra/features/connectivity/tracer_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/dataset/__init__.py` & `siibra-0.4a58/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/dataset/ebrains.py` & `siibra-0.4a58/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/feature.py` & `siibra-0.4a58/siibra/features/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,17 +176,18 @@
     def last_match_description(self):
         return "" if self.anchor is None \
             else self.anchor.last_match_description
 
     @property
     def id(self):
         prefix = ''
-        id_set = {ds.id for ds in self.datasets if hasattr(ds, 'id')}
-        if len(id_set) == 1:
-            prefix = list(id_set)[0] + '--'
+        for ds in self.datasets:
+            if hasattr(ds, "id"):
+                prefix = ds.id + '--'
+                break
         return prefix + md5(self.name.encode("utf-8")).hexdigest()
 
     @staticmethod
     def serialize_query_context(feat: 'Feature', concept: concept.AtlasConcept) -> str:
         """
         Serialize feature from livequery and query context.
```

### Comparing `siibra-0.4a57/siibra/features/image/__init__.py` & `siibra-0.4a58/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/image/image.py` & `siibra-0.4a58/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/image/sections.py` & `siibra-0.4a58/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/image/volume_of_interest.py` & `siibra-0.4a58/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/__init__.py` & `siibra-0.4a58/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a58/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a58/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a58/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/gene_expression.py` & `siibra-0.4a58/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a58/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a58/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a58/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a58/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a58/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/features/tabular/tabular.py` & `siibra-0.4a58/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/livequeries/__init__.py` & `siibra-0.4a58/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/livequeries/allen.py` & `siibra-0.4a58/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/livequeries/bigbrain.py` & `siibra-0.4a58/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/livequeries/ebrains.py` & `siibra-0.4a58/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/livequeries/query.py` & `siibra-0.4a58/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/locations/__init__.py` & `siibra-0.4a58/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/locations/boundingbox.py` & `siibra-0.4a58/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/locations/location.py` & `siibra-0.4a58/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/locations/point.py` & `siibra-0.4a58/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/locations/pointset.py` & `siibra-0.4a58/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/retrieval/__init__.py` & `siibra-0.4a58/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/retrieval/cache.py` & `siibra-0.4a58/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/retrieval/repositories.py` & `siibra-0.4a58/siibra/retrieval/repositories.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/retrieval/requests.py` & `siibra-0.4a58/siibra/retrieval/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .. import __version__
 
 import json
 from zipfile import ZipFile
 import requests
 import os
 from nibabel import Nifti1Image, GiftiImage, streamlines
-from skimage import io
+from skimage import io as skimage_io
 import gzip
 from io import BytesIO
 import urllib.parse
 import pandas as pd
 import numpy as np
 from typing import List, Callable, Any, TYPE_CHECKING
 from enum import Enum
@@ -43,24 +43,23 @@
 
 if TYPE_CHECKING:
     from .repositories import GitlabConnector
 
 USER_AGENT_HEADER = {"User-Agent": f"siibra-python/{__version__}"}
 
 DECODERS = {
-    ".nii.gz": lambda b: Nifti1Image.from_bytes(gzip.decompress(b)),
     ".nii": lambda b: Nifti1Image.from_bytes(b),
     ".gii": lambda b: GiftiImage.from_bytes(b),
     ".json": lambda b: json.loads(b.decode()),
     ".tck": lambda b: streamlines.load(BytesIO(b)),
     ".csv": lambda b: pd.read_csv(BytesIO(b)),
     ".tsv": lambda b: pd.read_csv(BytesIO(b), delimiter="\t").dropna(axis=0, how="all"),
     ".txt": lambda b: pd.read_csv(BytesIO(b), delimiter=" ", header=None),
     ".zip": lambda b: ZipFile(BytesIO(b)),
-    ".png": lambda b: io.imread(BytesIO(b)),
+    ".png": lambda b: skimage_io.imread(BytesIO(b)),
     ".npy": lambda b: np.load(BytesIO(b))
 }
 
 
 class SiibraHttpRequestError(Exception):
 
     def __init__(self, url: str, status_code: int, msg="Cannot execute http request."):
@@ -104,48 +103,46 @@
         refresh : bool, default: False
             If True, a possibly cached content will be ignored and refreshed
         post: bool, default: False
             perform a post instead of get
         """
         assert url is not None
         self.url = url
-        suitable_decoders = [dec for sfx, dec in DECODERS.items() if url.endswith(sfx)]
-        if (func is None) and (len(suitable_decoders) > 0):
-            assert len(suitable_decoders) == 1
-            self.func = suitable_decoders[0]
-        else:
-            self.func = func
+        self._set_decoder_func(func)
         self.kwargs = kwargs
         self.cachefile = CACHE.build_filename(self.url + json.dumps(kwargs))
         self.msg_if_not_cached = msg_if_not_cached
         self.refresh = refresh
         self.post = post
-        self._set_decoder_func(func, url)
 
-    def _set_decoder_func(self, func, fileurl: str):
-        urlpath = urllib.parse.urlsplit(fileurl).path
-        if func is None:
-            suitable_decoders = [
-                dec for sfx, dec in DECODERS.items() if urlpath.endswith(sfx)
-            ]
-            if len(suitable_decoders) > 0:
-                assert len(suitable_decoders) == 1
-                self.func = suitable_decoders[0]
-                return
-        self.func = func
+    @staticmethod
+    def find_suitiable_decoder(url: str):
+        urlpath = urllib.parse.urlsplit(url).path
+        if urlpath.endswith('.gz'):
+            dec = HttpRequest.find_suitiable_decoder(urlpath[:-3])
+            return lambda b: dec(gzip.decompress(b))
+
+        suitable_decoders = [dec for sfx, dec in DECODERS.items() if urlpath.endswith(sfx)]
+        if len(suitable_decoders) > 0:
+            assert len(suitable_decoders) == 1
+            return suitable_decoders[0]
+
+    def _set_decoder_func(self, func):
+        self.func = func or self.find_suitiable_decoder(self.url)
 
     @property
     def cached(self):
         return os.path.isfile(self.cachefile)
 
     def _retrieve(self, block_size=1024, min_bytesize_with_no_progress_info=2e8):
-        # Populates the file cache with the data from http if required.
-        # noop if 1/ data is already cached and 2/ refresh flag not set
-        # The caller should load the cachefile after _retrieve successfuly executes
-
+        """
+        Populates the file cache with the data from http if required.
+        noop if 1/ data is already cached and 2/ refresh flag not set
+        The caller should load the cachefile after _retrieve successfuly executes
+        """
         if self.cached and not self.refresh:
             return
 
         # not yet in cache, perform http request.
         if self.msg_if_not_cached is not None:
             logger.debug(self.msg_if_not_cached)
 
@@ -192,29 +189,29 @@
             return data if self.func is None else self.func(data)
         except Exception as e:
             # if network error results in bad cache, it may get raised here
             # e.g. BadZipFile("File is not a zip file")
             # if that happens, remove cachefile and
             try:
                 os.unlink(self.cachefile)
-            except Exception:  # TODO: do not use bare except
+            except Exception:
                 pass
             raise e
 
     @property
     def data(self):
         # for backward compatibility with old LazyHttpRequest class
         return self.get()
 
 
 class ZipfileRequest(HttpRequest):
     def __init__(self, url, filename, func=None):
         HttpRequest.__init__(self, url, func=func)
         self.filename = filename
-        self._set_decoder_func(func, filename)
+        self._set_decoder_func(self.find_suitiable_decoder(self.filename))
 
     def get(self):
         self._retrieve()
         zipfile = ZipFile(self.cachefile)
         filenames = zipfile.namelist()
         matches = [fn for fn in filenames if fn.endswith(self.filename)]
         if len(matches) == 0:
@@ -275,14 +272,15 @@
 
     @classmethod
     def fetch_token(cls, **kwargs):
         """
         Fetch an EBRAINS token using commandline-supplied username/password
         using the data proxy endpoint.
 
+
         :ref:`Details on how to access EBRAINS are here.<accessEBRAINS>`
         """
         cls.device_flow(**kwargs)
 
     @classmethod
     def device_flow(cls, **kwargs):
         if all([
```

### Comparing `siibra-0.4a57/siibra/vocabularies/__init__.py` & `siibra-0.4a58/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/vocabularies/gene_names.json` & `siibra-0.4a58/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a58/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/vocabularies/region_aliases.json` & `siibra-0.4a58/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/volumes/__init__.py` & `siibra-0.4a58/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/volumes/gifti.py` & `siibra-0.4a58/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/volumes/neuroglancer.py` & `siibra-0.4a58/siibra/volumes/neuroglancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             res = requests.HttpRequest(f"{self.url}/transform.json").get()
         except requests.SiibraHttpRequestError:
             res = None
         if res is not None:
             self._transform_nm = np.array(res)
             return self._transform_nm
 
-        self._transform_nm = np.identity(1)
+        self._transform_nm = np.identity(4)
         logger.warning(f"No transform.json found at {self.url}, using identity.")
         return self._transform_nm
 
     @transform_nm.setter
     def transform_nm(self, val):
         self._transform_nm = val
```

### Comparing `siibra-0.4a57/siibra/volumes/nifti.py` & `siibra-0.4a58/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra/volumes/parcellationmap.py` & `siibra-0.4a58/siibra/volumes/parcellationmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,36 +767,38 @@
                 in enumerate(np.asanyarray(volimg.dataobj)[x, y, z])
             ]
 
     def _assign(
         self,
         item: Union[point.Point, pointset.PointSet, Nifti1Image],
         minsize_voxel=1,
-        lower_threshold=0.0
-    ) -> List[Union[Assignment, AssignImageResult]]:
+        lower_threshold=0.0,
+        **kwargs
+    ) -> List[Union[Assignment,AssignImageResult]]:
         """
         For internal use only. Returns a dataclass, which provides better static type checking.
         """
 
         if isinstance(item, point.Point):
             return self._assign_points(pointset.PointSet([item], item.space, sigma_mm=item.sigma), lower_threshold)
         if isinstance(item, pointset.PointSet):
             return self._assign_points(item, lower_threshold)
         if isinstance(item, Nifti1Image):
-            return self._assign_image(item, minsize_voxel, lower_threshold)
-
+            return self._assign_image(item, minsize_voxel, lower_threshold, **kwargs)
+        
         raise RuntimeError(
             f"Items of type {item.__class__.__name__} cannot be used for region assignment."
         )
 
     def assign(
         self,
         item: Union[point.Point, pointset.PointSet, Nifti1Image],
         minsize_voxel=1,
-        lower_threshold=0.0
+        lower_threshold=0.0,
+        **kwargs
     ):
         """Assign an input image to brain regions.
 
         The input image is assumed to be defined in the same coordinate space
         as this parcellation map.
 
         Parameters
@@ -836,15 +838,15 @@
         components: Nifti1Image or None
             If the input was an image, this is a labelled volume mapping the
             detected components in the input image, where pixel values correspond
             to the "component" column of the assignment table. If the input was
             a Point or PointSet, returns None.
         """
 
-        assignments = self._assign(item, minsize_voxel, lower_threshold)
+        assignments = self._assign(item, minsize_voxel, lower_threshold, **kwargs)
 
         # format assignments as pandas dataframe
         columns = [
             "input structure",
             "centroid",
             "volume",
             "fragment",
@@ -1016,15 +1018,15 @@
                 W = Nifti1Image(dataobj=kernel, affine=np.dot(self.affine, shift))
                 for entry in self._assign(W, lower_threshold=lower_threshold):
                     entry.input_structure = pointindex
                     entry.centroid = tuple(pt)
                     assignments.append(entry)
         return assignments
 
-    def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float) -> List[AssignImageResult]:
+    def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float, split_components: bool = True) -> List[AssignImageResult]:
         """
         Assign an image volume to this parcellation map.
 
         Parameters:
         -----------
         minsize_voxel: int, default: 1
             Minimum voxel size of image components to be taken into account.
@@ -1051,24 +1053,27 @@
 
         def progress(it, N: int = None, desc: str = "", min_elements=5):
             # wraps a progress indicator around the given iterator,
             # but only if the sequence is long.
             seqlen = N or len(it)
             return iter(it) if seqlen < min_elements \
                 else siibra_tqdm(it, desc=desc, total=N)
+        
+        iter_func = iterate_connected_components if split_components \
+            else lambda img: [(1, img)]
 
         with QUIET and _volume.SubvolumeProvider.UseCaching():
             for frag in self.fragments or {None}:
                 for vol, vol_img in progress(
                     enumerate(self.fetch_iter(fragment=frag)),
                     N=len(self),
                     desc=f"Assigning to {len(self)} volumes"
                 ):
                     queryimg_res = resample(queryimg, vol_img.affine, vol_img.shape)
-                    for mode, maskimg in iterate_connected_components(queryimg_res):
+                    for mode, maskimg in iter_func(queryimg_res):
                         vol_data = np.asanyarray(vol_img.dataobj)
                         position = np.array(np.where(maskimg.get_fdata())).T.mean(0)
                         labels = {v.label for L in self._indices.values() for v in L if v.volume == vol}
                         for label in progress(
                             labels,
                             desc=f"Assigning to {len(labels)} labelled structures"
                         ):
```

### Comparing `siibra-0.4a57/siibra/volumes/sparsemap.py` & `siibra-0.4a58/siibra/volumes/sparsemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,17 +221,15 @@
         parcellation_spec: dict,
         indices: Dict[str, MapIndex],
         volumes: list = [],
         shortname: str = "",
         description: str = "",
         modality: str = None,
         publications: list = [],
-        datasets: list = [],
-        is_cached: bool = False,
-        cache_url: str = "",
+        datasets: list = []
     ):
         parcellationmap.Map.__init__(
             self,
             identifier=identifier,
             name=name,
             space_spec=space_spec,
             parcellation_spec=parcellation_spec,
@@ -240,39 +238,33 @@
             description=description,
             modality=modality,
             publications=publications,
             datasets=datasets,
             volumes=volumes,
         )
         self._sparse_index_cached = None
-        self._sparseindex_zip_url = cache_url if is_cached else ""
 
     @property
     def _cache_prefix(self):
         return f"{self.parcellation.id}_{self.space.id}_{self.maptype}_{self.name}_index"
 
     @property
     def sparse_index(self):
         if self._sparse_index_cached is None:
             spind = SparseIndex._from_local_cache(self._cache_prefix)
-            if spind is None and len(self._sparseindex_zip_url) > 0:
-                logger.debug("Loading SparseIndex from precomputed source.")
-                try:
-                    spind = self.load_zipped_sparseindex(self._sparseindex_zip_url)
-                except Exception:
-                    logger.debug("Could not load SparseIndex from precomputed source.", exc_info=1)
             if spind is None:
-                logger.debug("Loading SparseIndex from Gitlab.")
+                logger.info("Downloading precomputed SparseIndex...")
                 gconn = GitlabConnector(self._GITLAB_SERVER, self._GITLAB_PROJECT, "main")
                 zip_fname = f"{self.name.replace(' ', '_')}_index.zip"
                 try:
                     assert zip_fname in gconn.search_files(), f"{zip_fname} is not in {gconn}."
                     zipfile = gconn.get_loader(zip_fname).url
                     spind = self.load_zipped_sparseindex(zipfile)
                 except Exception:
+                    logger.info("Failed to load precomputed SparseIndex from Gitlab.")
                     logger.debug(f"Could not load SparseIndex from Gitlab at {gconn}", exc_info=1)
             if spind is None:
                 with _volume.SubvolumeProvider.UseCaching():
                     spind = SparseIndex()
                     for vol in siibra_tqdm(
                         range(len(self)), total=len(self), unit="maps",
                         desc=f"Fetching {len(self)} volumetric maps"
@@ -445,15 +437,15 @@
         else:
             return list(
                 (pointindex, volume, None, value)
                 for pointindex, voxel in enumerate(vx)
                 for volume, value in spind.probs[voxel].items()
             )
 
-    def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float) -> List[parcellationmap.AssignImageResult]:
+    def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float, split_components: bool = True) -> List[parcellationmap.AssignImageResult]:
         """
         Assign an image volume to this parcellation map.
 
         Parameters:
         -----------
         queryimg: Nifti1Image
             the image to be compared with maps
@@ -478,15 +470,18 @@
                 target_affine=self.affine,
                 target_shape=self.shape,
                 interpolation=interp,
             )
 
         querydata = np.asanyarray(queryimg.dataobj).squeeze()
 
-        for mode, modeimg in iterate_connected_components(queryimg):
+        iter_func = iterate_connected_components if split_components \
+            else lambda img: [(1, img)]
+
+        for mode, modeimg in iter_func(queryimg):
 
             # determine bounding box of the mode
             modemask = np.asanyarray(modeimg.dataobj)
             XYZ2 = np.array(np.where(modemask)).T
             position = np.dot(modeimg.affine, np.r_[XYZ2.mean(0), 1])[:3]
             if XYZ2.shape[0] <= minsize_voxel:
                 continue
```

### Comparing `siibra-0.4a57/siibra/volumes/volume.py` & `siibra-0.4a58/siibra/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/siibra.egg-info/PKG-INFO` & `siibra-0.4a58/siibra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a57
+Version: 0.4a58
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a57/siibra.egg-info/SOURCES.txt` & `siibra-0.4a58/siibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siibra-0.4a57/test/test_siibra.py` & `siibra-0.4a58/test/test_siibra.py`

 * *Files identical despite different names*

