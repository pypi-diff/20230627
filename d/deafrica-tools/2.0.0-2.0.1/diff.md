# Comparing `tmp/deafrica_tools-2.0.0.tar.gz` & `tmp/deafrica_tools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica_tools-2.0.0.tar", max compression
+gzip compressed data, was "deafrica_tools-2.0.1.tar", max compression
```

## Comparing `deafrica_tools-2.0.0.tar` & `deafrica_tools-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/LICENSE
--rw-r--r--   0        0        0     2587 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/README.md
--rw-r--r--   0        0        0      676 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/deafrica_tools/__init__.py
--rw-r--r--   0        0        0       22 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/__init__.py
--rw-r--r--   0        0        0    31449 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/animations.py
--rw-r--r--   0        0        0    10984 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0        0        0    10494 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/crophealth.py
--rw-r--r--   0        0        0    20287 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0        0        0    37843 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0        0        0     8673 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/geomedian.py
--rw-r--r--   0        0        0    13383 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/imageexport.py
--rw-r--r--   0        0        0    13148 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0        0        0     9882 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0        0        0     2043 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/areaofinterest.py
--rw-r--r--   0        0        0    24548 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/bandindices.py
--rw-r--r--   0        0        0    61473 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/classification.py
--rw-r--r--   0        0        0    23515 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/coastal.py
--rw-r--r--   0        0        0     3404 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/dask.py
--rw-r--r--   0        0        0    35752 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/datahandling.py
--rw-r--r--   0        0        0    14369 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_era5.py
--rw-r--r--   0        0        0     2793 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_isda.py
--rw-r--r--   0        0        0     2027 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_soil_moisture.py
--rw-r--r--   0        0        0     1783 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0        0        0     2841 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0        0        0    50697 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/plotting.py
--rw-r--r--   0        0        0    36957 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/spatial.py
--rw-r--r--   0        0        0    17245 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/temporal.py
--rw-r--r--   0        0        0    25961 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/wetlands.py
--rw-r--r--   0        0        0     3310 2023-06-19 06:48:50.186113 deafrica_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 deafrica_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3097 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/README.md
+-rw-r--r--   0        0        0      676 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/app/__init__.py
+-rw-r--r--   0        0        0    31449 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/app/animations.py
+-rw-r--r--   0        0        0    10984 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0        0        0    10494 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/crophealth.py
+-rw-r--r--   0        0        0    20287 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0        0        0    37843 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0        0        0     8673 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/geomedian.py
+-rw-r--r--   0        0        0    13383 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/imageexport.py
+-rw-r--r--   0        0        0    13148 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0        0        0     9882 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0        0        0     2043 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/areaofinterest.py
+-rw-r--r--   0        0        0    24548 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/bandindices.py
+-rw-r--r--   0        0        0    61473 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/classification.py
+-rw-r--r--   0        0        0    23515 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/coastal.py
+-rw-r--r--   0        0        0     3404 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/dask.py
+-rw-r--r--   0        0        0    35752 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/datahandling.py
+-rw-r--r--   0        0        0    14369 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_era5.py
+-rw-r--r--   0        0        0     2793 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_isda.py
+-rw-r--r--   0        0        0     2027 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_soil_moisture.py
+-rw-r--r--   0        0        0     1783 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0        0        0     3315 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0        0        0    50697 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/plotting.py
+-rw-r--r--   0        0        0    36957 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/spatial.py
+-rw-r--r--   0        0        0    17245 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/temporal.py
+-rw-r--r--   0        0        0    25961 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/wetlands.py
+-rw-r--r--   0        0        0     3310 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 deafrica_tools-2.0.1/PKG-INFO
```

### Comparing `deafrica_tools-2.0.0/LICENSE` & `deafrica_tools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/README.md` & `deafrica_tools-2.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,46 +2,55 @@
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
 
-This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't avilable, you can also `pip install` the module.
-To do this on the Digital Earth Africa Sandbox, run `pip` from the terminal:
+This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, you can also `pip install` the module from the terminal.
+
+You can install the `deafrica-tools` package from PyPI using:
+
+```
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" deafrica-tools 
+```
+or install the package from the `Tools` directory:
 
 ```
-pip install -e Tools/
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" -e Tools/
 ```
        
 To install this module from the source on any other system with `pip`:
 
 ```
-pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
 ```
 
 
+
 ## Citing Digital Earth Africa Tools
 
 The code in this module is an adaptation of code from the [Digital Earth Australia](https://github.com/GeoscienceAustralia/dea-notebooks) `dea-tools` package. If you use any of the code in this repository in your work, please reference them using the following citation:
 
     Krause, C., Dunn, B., Bishop-Taylor, R., Adams, C., Burton, C., Alger, M., Chua, S., Phillips, C., Newey, V., Kouzoubov, K., Leith, A., Ayers, D., Hicks, A., DEA Notebooks contributors 2021. Digital Earth Australia notebooks and tools repository. Geoscience Australia, Canberra. https://doi.org/10.26186/145234
     
     
 ## Translation
 
 Translation of the module into other languages is done using `gettext` and `pot/po/mo` files.
 
-The template `pot` file can be generated by running `pybabel extract -o deafrica_tools.pot *` from the Tools directory.
+We welcome contributors to help in translating the project by joining this project https://poeditor.com/join/project?hash=0Q33A7sRM6.
+
+The template `.pot` file can be generated by running `pybabel extract -o deafrica_tools.pot *` from the `Tools/` directory.
 
-This file can then be uploaded to POEditor.com, by joining this project: https://poeditor.com/join/project?hash=0Q33A7sRM6.
+This file can then be uploaded to the [deafrica_tools project](https://poeditor.com/join/project?hash=0Q33A7sRM6) on POEditor.com
 
-(TODO: Automate this step as in other projects such as [deafrica-docs](https://github.com/digitalearthafrica/deafrica-docs/blob/main/.github/workflows/main.yml))
+To get the most recent terms and translations, download the files from the [deafrica_tools project](https://poeditor.com/join/project?hash=0Q33A7sRM6) and export the the `deafrica_tools.po` and `deafrica_tools.mo` files to the `deafrica_tools/locales/fr/LC_MESSAGES/` directory.
 
-Currently, the `po` and `mo` files must be exported to `deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`
+Currently, uploading and downloading terms and translations is accomplished using Github Actions. 
 
 In python code, strings surrounded by an underscore function `_('')` will be translated.
 
 This `_()` function is declared as a global after [`deafrica_tools.set_lang('fr')`](deafrica_tools/__init__.py) is called. 
 
 Calling `deafrica_tools.set_lang()` with no argument will use the language set by JupyterLab under **Settings -> Language**.
```

### Comparing `deafrica_tools-2.0.0/deafrica_tools/__init__.py` & `deafrica_tools-2.0.1/deafrica_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 __locales__ = __path__[0] + '/locales'
 
 
 def set_lang(lang=None):
     if lang is None:
         import os
```

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/animations.py` & `deafrica_tools-2.0.1/deafrica_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/changefilmstrips.py` & `deafrica_tools-2.0.1/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/crophealth.py` & `deafrica_tools-2.0.1/deafrica_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/deacoastlines.py` & `deafrica_tools-2.0.1/deafrica_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/forestmonitoring.py` & `deafrica_tools-2.0.1/deafrica_tools/app/forestmonitoring.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/geomedian.py` & `deafrica_tools-2.0.1/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/imageexport.py` & `deafrica_tools-2.0.1/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica_tools-2.0.1/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/app/widgetconstructors.py` & `deafrica_tools-2.0.1/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/areaofinterest.py` & `deafrica_tools-2.0.1/deafrica_tools/areaofinterest.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/bandindices.py` & `deafrica_tools-2.0.1/deafrica_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/classification.py` & `deafrica_tools-2.0.1/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/coastal.py` & `deafrica_tools-2.0.1/deafrica_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/dask.py` & `deafrica_tools-2.0.1/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/datahandling.py` & `deafrica_tools-2.0.1/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/load_era5.py` & `deafrica_tools-2.0.1/deafrica_tools/load_era5.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/load_isda.py` & `deafrica_tools-2.0.1/deafrica_tools/load_isda.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/load_soil_moisture.py` & `deafrica_tools-2.0.1/deafrica_tools/load_soil_moisture.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,117 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.4.1\n"
+"X-Generator: POEditor.com\n"
 "Project-Id-Version: deafrica_tools\n"
 "Language: fr\n"
-"POT-Creation-Date: \n"
-"PO-Revision-Date: \n"
-"Last-Translator: \n"
-"Language-Team: \n"
 
-#: app/wetlandsinsighttool.py:100
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:83
 msgid "None"
 msgstr "Aucun"
 
-#: app/wetlandsinsighttool.py:101
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:84
 msgid "ESRI World Imagery"
 msgstr "Imagerie mondiale ESRI"
 
-#: app/wetlandsinsighttool.py:102
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:85
 msgid "Sentinel-2 Geomedian"
 msgstr "Sentinel-2 Geomedian"
 
-#: app/wetlandsinsighttool.py:103
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:86
 msgid "Water Observations from Space"
 msgstr "Observations de l'eau depuis l'espace-WOfS"
 
-#: app/wetlandsinsighttool.py:116
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:99
 msgid "Wetlands Insight Tool"
 msgstr "Outil d'analyse des zones humides"
 
-#: app/wetlandsinsighttool.py:117
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:100
 msgid "Select parameters and AOI"
 msgstr "Sélectionner les paramètres et la zone d'intérêt"
 
-#: app/wetlandsinsighttool.py:141
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:124
 msgid "Total polygon area"
 msgstr "Superficie totale du polygone"
 
-#: app/wetlandsinsighttool.py:145
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:128
 msgid "Area falls within recommended limit"
 msgstr "La zone se situe dans la limite recommandée"
 
-#: app/wetlandsinsighttool.py:148
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:131
 msgid "Area is too large, please update your polygon"
 msgstr "La zone est trop grande, veuillez réduire votre polygone"
 
-#: app/wetlandsinsighttool.py:168
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:151
 msgid "Map Overlays"
 msgstr "Superpositions de cartes"
 
-#: app/wetlandsinsighttool.py:193
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:176
 msgid "Run"
 msgstr "Exécuter"
 
-#: app/wetlandsinsighttool.py:200
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:183
 msgid "Map Overlay:"
 msgstr "Carte superposée :"
 
-#: app/wetlandsinsighttool.py:202
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:185
 msgid "Start Date:"
 msgstr "Date de début :"
 
-#: app/wetlandsinsighttool.py:204
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:187
 msgid "End Date:"
 msgstr "Date de fin :"
 
-#: app/wetlandsinsighttool.py:206
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:189
 msgid "Minimum Good Data:"
 msgstr "Minimum de bonnes données :"
 
-#: app/wetlandsinsighttool.py:208
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:191
 msgid "Resampling Frequency:"
 msgstr "Fréquence de rééchantillonnage :"
 
-#: app/wetlandsinsighttool.py:210
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:193
 msgid "Output CSV:"
 msgstr "Sortie CSV :"
 
-#: app/wetlandsinsighttool.py:212
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:195
 msgid "Output Plot:"
 msgstr "Tracé de sortie :"
 
-#: app/wetlandsinsighttool.py:325
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:308
 msgid "Progress"
 msgstr "Progrès"
 
-#: app/wetlandsinsighttool.py:343
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:326
 msgid "WIT complete"
 msgstr "WIT achevée"
 
-#: app/wetlandsinsighttool.py:345
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:328
 msgid "No polygon selected"
 msgstr "Aucun polygone sélectionné"
 
-#: app/wetlandsinsighttool.py:382
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:365
 msgid "open water"
 msgstr "eau libre"
 
-#: app/wetlandsinsighttool.py:383
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:366
 msgid "wet"
 msgstr "humide"
 
-#: app/wetlandsinsighttool.py:384
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:367
 msgid "green veg"
 msgstr "végétation verts"
 
-#: app/wetlandsinsighttool.py:385
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:368
 msgid "dry veg"
 msgstr "végétation seche"
 
-#: app/wetlandsinsighttool.py:386
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:369
 msgid "bare soil"
 msgstr "sol nu"
 
-#: app/wetlandsinsighttool.py:399
+#: Tools/deafrica_tools/app/wetlandsinsighttool.py:382
 msgid "Percentage Fractional Cover, Wetness, and Water"
 msgstr "Pourcentage de couverture fractionnée, humidité et eau"
+
```

### Comparing `deafrica_tools-2.0.0/deafrica_tools/plotting.py` & `deafrica_tools-2.0.1/deafrica_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/spatial.py` & `deafrica_tools-2.0.1/deafrica_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/temporal.py` & `deafrica_tools-2.0.1/deafrica_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/deafrica_tools/wetlands.py` & `deafrica_tools-2.0.1/deafrica_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.0/pyproject.toml` & `deafrica_tools-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml tells “frontend” build tools like pip and build what “backend” tool to use to create distribution packages for your project.
 
 # Using poetry for dependency management and packaging.
 
 # Package metadata.
 [tool.poetry]
 name = "deafrica-tools"
-version = "2.0.0"
+version = "2.0.1"
 description = "Functions and algorithms for analysing Digital Earth Africa data."
 license = "Apache-2.0"
 authors = ["Digital Earth Africa <systems@digitalearthafrica.org>"]
 readme = "README.md"
 homepage = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 repository = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 documentation = "https://docs.digitalearthafrica.org/en/latest/sandbox/notebooks/Tools/index.html"
```

### Comparing `deafrica_tools-2.0.0/PKG-INFO` & `deafrica_tools-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 2.0.0
+Version: 2.0.1
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 License: Apache-2.0
 Author: Digital Earth Africa
 Author-email: systems@digitalearthafrica.org
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -65,46 +65,55 @@
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
 
-This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't avilable, you can also `pip install` the module.
-To do this on the Digital Earth Africa Sandbox, run `pip` from the terminal:
+This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, you can also `pip install` the module from the terminal.
+
+You can install the `deafrica-tools` package from PyPI using:
+
+```
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" deafrica-tools 
+```
+or install the package from the `Tools` directory:
 
 ```
-pip install -e Tools/
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" -e Tools/
 ```
        
 To install this module from the source on any other system with `pip`:
 
 ```
-pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
 ```
 
 
+
 ## Citing Digital Earth Africa Tools
 
 The code in this module is an adaptation of code from the [Digital Earth Australia](https://github.com/GeoscienceAustralia/dea-notebooks) `dea-tools` package. If you use any of the code in this repository in your work, please reference them using the following citation:
 
     Krause, C., Dunn, B., Bishop-Taylor, R., Adams, C., Burton, C., Alger, M., Chua, S., Phillips, C., Newey, V., Kouzoubov, K., Leith, A., Ayers, D., Hicks, A., DEA Notebooks contributors 2021. Digital Earth Australia notebooks and tools repository. Geoscience Australia, Canberra. https://doi.org/10.26186/145234
     
     
 ## Translation
 
 Translation of the module into other languages is done using `gettext` and `pot/po/mo` files.
 
-The template `pot` file can be generated by running `pybabel extract -o deafrica_tools.pot *` from the Tools directory.
+We welcome contributors to help in translating the project by joining this project https://poeditor.com/join/project?hash=0Q33A7sRM6.
+
+The template `.pot` file can be generated by running `pybabel extract -o deafrica_tools.pot *` from the `Tools/` directory.
 
-This file can then be uploaded to POEditor.com, by joining this project: https://poeditor.com/join/project?hash=0Q33A7sRM6.
+This file can then be uploaded to the [deafrica_tools project](https://poeditor.com/join/project?hash=0Q33A7sRM6) on POEditor.com
 
-(TODO: Automate this step as in other projects such as [deafrica-docs](https://github.com/digitalearthafrica/deafrica-docs/blob/main/.github/workflows/main.yml))
+To get the most recent terms and translations, download the files from the [deafrica_tools project](https://poeditor.com/join/project?hash=0Q33A7sRM6) and export the the `deafrica_tools.po` and `deafrica_tools.mo` files to the `deafrica_tools/locales/fr/LC_MESSAGES/` directory.
 
-Currently, the `po` and `mo` files must be exported to `deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`
+Currently, uploading and downloading terms and translations is accomplished using Github Actions. 
 
 In python code, strings surrounded by an underscore function `_('')` will be translated.
 
 This `_()` function is declared as a global after [`deafrica_tools.set_lang('fr')`](deafrica_tools/__init__.py) is called. 
 
 Calling `deafrica_tools.set_lang()` with no argument will use the language set by JupyterLab under **Settings -> Language**.
```

