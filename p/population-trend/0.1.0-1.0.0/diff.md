# Comparing `tmp/population_trend-0.1.0.tar.gz` & `tmp/population_trend-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-0.1.0.tar` & `population_trend-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1037 2023-06-23 21:23:08.767541 population_trend-0.1.0/README.md
--rw-r--r--   0        0        0      101 2023-06-23 21:23:08.767541 population_trend-0.1.0/population_trend/__init__.py
--rw-r--r--   0        0        0     4122 2023-06-23 21:23:08.767541 population_trend-0.1.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      486 2023-06-23 21:23:08.767541 population_trend-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1483 1970-01-01 00:00:00.000000 population_trend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-06-27 19:34:25.060105 population_trend-1.0.0/README.md
+-rw-r--r--   0        0        0      136 2023-06-27 19:34:25.060105 population_trend-1.0.0/population_trend/__init__.py
+-rw-r--r--   0        0        0      936 2023-06-27 19:34:25.060105 population_trend-1.0.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     4051 2023-06-27 19:34:25.060105 population_trend-1.0.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-06-27 19:34:25.060105 population_trend-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-1.0.0/PKG-INFO
```

### Comparing `population_trend-0.1.0/README.md` & `population_trend-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-0.1.0/population_trend/population_growth_model.py` & `population_trend-1.0.0/population_trend/population_growth_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import numpy as np
 from geci_plots import geci_plot, roundup, ticks_positions_array, order_magnitude
 from bootstrapping_tools import lambda_calculator, power_law
 import matplotlib.pyplot as plt
 
 
-def filter_data_by_islet(df, islet):
-    return df[df.Isla == islet]
-
-
 def resample_seasons(df):
     first_season = int(df.Temporada.min())
     last_season = int(df.Temporada.max())
     return np.linspace(first_season, last_season, last_season - first_season + 1).astype(int)
 
 
 def calculate_upper_limit(data_interest_variable):
```

### Comparing `population_trend-0.1.0/PKG-INFO` & `population_trend-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 0.1.0
+Version: 1.0.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/population_trend
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: bootstrapping-tools==0.5.7
 Requires-Dist: geci-plots
+Requires-Dist: typer
 
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 # Dummy Transformations
 
 Para usar este repo como plantilla debemos hacer lo siguiente:
 
 1. Presiona el botón verde que dice _Use this template_
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: population_trend Version: 0.1.0 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 1.0.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
-bootstrapping-tools==0.5.7 Requires-Dist: geci-plots [https://www.islas.org.mx/
-img/logo.svg] # Dummy Transformations Para usar este repo como plantilla
-debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que dice _Use this
-template_ 1. Selecciona como dueÃ±o a la organizaciÃ³n IslasGECI 1. Agrega el
-nombre del nuevo mÃ³dulo de python 1. Presiona el botÃ³n _Create repository
-from template_ 1. Reemplaza `dummy_transformations` por el nombre del nuevo
-mÃ³dulo en: - `Makefile` - `pyproject.toml` - `tests\test_transformations.py`
-1. Renombra el archivo `dummy_transformations\transformations.py` al nombre del
-primer archivo del nuevo mÃ³dulo 1. Cambia la descripciÃ³n del archivo
+bootstrapping-tools==0.5.7 Requires-Dist: geci-plots Requires-Dist: typer
+[https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
+repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
+dice _Use this template_ 1. Selecciona como dueÃ±o a la organizaciÃ³n IslasGECI
+1. Agrega el nombre del nuevo mÃ³dulo de python 1. Presiona el botÃ³n _Create
+repository from template_ 1. Reemplaza `dummy_transformations` por el nombre
+del nuevo mÃ³dulo en: - `Makefile` - `pyproject.toml` -
+`tests\test_transformations.py` 1. Renombra el archivo
+`dummy_transformations\transformations.py` al nombre del primer archivo del
+nuevo mÃ³dulo 1. Cambia la descripciÃ³n del archivo
 `dummy_transformations\__init__.py` 1. Renombra el directorio
 `dummy_transformations` al nombre del nuevo mÃ³dulo 1. Cambia el
 `codecov_token` del archivo `Makefile` Los archivos del nuevo mÃ³dulo los
 agregarÃ¡s en la carpeta que antes se llamaba `dummy_transformations` y las
 pruebas en la carpeta `tests`.
```

