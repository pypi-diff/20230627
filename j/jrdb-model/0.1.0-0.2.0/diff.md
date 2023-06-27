# Comparing `tmp/jrdb-model-0.1.0.tar.gz` & `tmp/jrdb-model-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrdb-model-0.1.0.tar", last modified: Mon Jun 20 15:35:32 2022, max compression
+gzip compressed data, was "jrdb-model-0.2.0.tar", last modified: Tue Jun 27 16:05:05 2023, max compression
```

## Comparing `jrdb-model-0.1.0.tar` & `jrdb-model-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.272036 jrdb-model-0.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1068 2022-05-02 09:15:44.000000 jrdb-model-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      956 2022-06-20 15:35:32.272036 jrdb-model-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      471 2022-06-20 14:46:57.000000 jrdb-model-0.1.0/README.md
--rw-rw-r--   0 root         (0) root         (0)       84 2022-06-16 07:11:52.000000 jrdb-model-0.1.0/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      651 2022-06-20 15:35:32.272036 jrdb-model-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.268036 jrdb-model-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.268036 jrdb-model-0.1.0/src/jrdb_model/
--rw-rw-r--   0 root         (0) root         (0)      968 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.272036 jrdb-model-0.1.0/src/jrdb_model/domain/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2119 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/bangumi.py
--rw-rw-r--   0 root         (0) root         (0)     1420 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/kaisai.py
--rw-rw-r--   0 root         (0) root         (0)      472 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/predict.py
--rw-rw-r--   0 root         (0) root         (0)      338 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/predict_race.py
--rw-rw-r--   0 root         (0) root         (0)     6322 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/racehorse.py
--rw-rw-r--   0 root         (0) root         (0)     3969 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/returninfo.py
--rw-rw-r--   0 root         (0) root         (0)     3070 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/seiseki.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/seisekirace.py
--rw-rw-r--   0 root         (0) root         (0)      899 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/trainanalysis.py
--rw-rw-r--   0 root         (0) root         (0)      919 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/trainoikiri.py
--rw-rw-r--   0 root         (0) root         (0)      469 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/umaren_odds.py
--rw-rw-r--   0 root         (0) root         (0)      471 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/wakuren_odds.py
--rw-rw-r--   0 root         (0) root         (0)      465 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/domain/wide_odds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.272036 jrdb-model-0.1.0/src/jrdb_model/master/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/master/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      816 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/master/horsebase.py
--rw-rw-r--   0 root         (0) root         (0)     1979 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/master/jockey.py
--rw-rw-r--   0 root         (0) root         (0)     1689 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/master/mastercode.py
--rw-rw-r--   0 root         (0) root         (0)     1914 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/master/trainer.py
--rw-rw-r--   0 root         (0) root         (0)      903 2022-06-16 07:03:59.000000 jrdb-model-0.1.0/src/jrdb_model/sessioncontroll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 15:35:32.268036 jrdb-model-0.1.0/src/jrdb_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      956 2022-06-20 15:35:31.000000 jrdb-model-0.1.0/src/jrdb_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      959 2022-06-20 15:35:32.000000 jrdb-model-0.1.0/src/jrdb_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-20 15:35:31.000000 jrdb-model-0.1.0/src/jrdb_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-20 15:35:31.000000 jrdb-model-0.1.0/src/jrdb_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-06-20 15:35:32.000000 jrdb-model-0.1.0/src/jrdb_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.259450 jrdb-model-0.2.0/
+-rw-rw-r--   0 root         (0) root         (0)     1068 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      956 2023-06-27 16:05:05.259450 jrdb-model-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      471 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       84 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)      652 2023-06-27 16:05:05.259450 jrdb-model-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.255450 jrdb-model-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.255450 jrdb-model-0.2.0/src/jrdb_model/
+-rw-rw-r--   0 root         (0) root         (0)     1026 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.255450 jrdb-model-0.2.0/src/jrdb_model/domain/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/bangumi.py
+-rw-rw-r--   0 root         (0) root         (0)      321 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/calculated_score.py
+-rw-rw-r--   0 root         (0) root         (0)     1420 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/kaisai.py
+-rw-rw-r--   0 root         (0) root         (0)      472 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/predict.py
+-rw-rw-r--   0 root         (0) root         (0)      338 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/predict_race.py
+-rw-rw-r--   0 root         (0) root         (0)     6450 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/racehorse.py
+-rw-rw-r--   0 root         (0) root         (0)     3969 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/returninfo.py
+-rw-rw-r--   0 root         (0) root         (0)     3070 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/seiseki.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/seisekirace.py
+-rw-rw-r--   0 root         (0) root         (0)      899 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/trainanalysis.py
+-rw-rw-r--   0 root         (0) root         (0)      919 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/trainoikiri.py
+-rw-rw-r--   0 root         (0) root         (0)      469 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/umaren_odds.py
+-rw-rw-r--   0 root         (0) root         (0)      471 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/wakuren_odds.py
+-rw-rw-r--   0 root         (0) root         (0)      465 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/domain/wide_odds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.259450 jrdb-model-0.2.0/src/jrdb_model/master/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/master/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      816 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/master/horsebase.py
+-rw-rw-r--   0 root         (0) root         (0)     1979 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/master/jockey.py
+-rw-rw-r--   0 root         (0) root         (0)     1689 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/master/mastercode.py
+-rw-rw-r--   0 root         (0) root         (0)     1914 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/master/trainer.py
+-rw-rw-r--   0 root         (0) root         (0)      903 2023-06-27 15:34:48.000000 jrdb-model-0.2.0/src/jrdb_model/sessioncontroll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:05:05.255450 jrdb-model-0.2.0/src/jrdb_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      956 2023-06-27 16:05:05.000000 jrdb-model-0.2.0/src/jrdb_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-27 16:05:05.000000 jrdb-model-0.2.0/src/jrdb_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:05:05.000000 jrdb-model-0.2.0/src/jrdb_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 16:05:05.000000 jrdb-model-0.2.0/src/jrdb_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-27 16:05:05.000000 jrdb-model-0.2.0/src/jrdb_model.egg-info/top_level.txt
```

### Comparing `jrdb-model-0.1.0/LICENSE` & `jrdb-model-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/PKG-INFO` & `jrdb-model-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jrdb-model
-Version: 0.1.0
+Version: 0.2.0
 Summary: ORM for JRDB
 Home-page: https://github.com/astroripple/horseview
 Author: requrd
 Author-email: requrd1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/astroripple/horseview/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jrdb-model-0.1.0/setup.cfg` & `jrdb-model-0.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jrdb-model
-version = 0.1.0
+version = 0.2.0
 author = requrd
 author_email = requrd1989@gmail.com
 description = ORM for JRDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/astroripple/horseview
 project_urls = 
@@ -15,15 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 install_requires = 
-	Flask-Migrate==3.1.0
+	Flask-Migrate >=4.0.4
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `jrdb-model-0.1.0/src/jrdb_model/__init__.py` & `jrdb-model-0.2.0/src/jrdb_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .domain.wakuren_odds import WakurenOddsData
 from .domain.seiseki import SeisekiData
 from .domain.seisekirace import SeisekiRaceData
 from .domain.trainanalysis import TrainAnalysisData
 from .domain.trainoikiri import TrainOikiriData
 from .domain.predict import PredictData
 from .domain.predict_race import PredictRaceData
+from .domain.calculated_score import CalculatedScoreData
 
 from .master.horsebase import HorsebaseData
 from .master.mastercode import *
 from .master.trainer import TrainerData
 from .master.jockey import JockeyData
 
 # 更新処理用のセッションオブジェクト
```

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/bangumi.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/bangumi.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/kaisai.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/kaisai.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/racehorse.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/racehorse.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     )
     result = relobj(
         "SeisekiData", uselist=False, backref=bkrobj("racehorse"), innerjoin=False
     )
     predict = relobj(
         "PredictData", uselist=False, backref=bkrobj("racehorse"), innerjoin=False
     )
+    calculated_score = relobj(
+        "CalculatedScoreData", uselist=False, backref=bkrobj("racehorse"), innerjoin=False
+    )
     bacode = colobj(intobj)
     year = colobj(intobj)
     kai = colobj(intobj)
     day = colobj(strobj)
     race = colobj(intobj)
     num = colobj(intobj)
     blood = colobj(intobj, fkyobj("horsebase.blood"))
```

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/returninfo.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/returninfo.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/seiseki.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/seiseki.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/seisekirace.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/seisekirace.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/trainanalysis.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/trainanalysis.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/domain/trainoikiri.py` & `jrdb-model-0.2.0/src/jrdb_model/domain/trainoikiri.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/master/horsebase.py` & `jrdb-model-0.2.0/src/jrdb_model/master/horsebase.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/master/jockey.py` & `jrdb-model-0.2.0/src/jrdb_model/master/jockey.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/master/mastercode.py` & `jrdb-model-0.2.0/src/jrdb_model/master/mastercode.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/master/trainer.py` & `jrdb-model-0.2.0/src/jrdb_model/master/trainer.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model/sessioncontroll.py` & `jrdb-model-0.2.0/src/jrdb_model/sessioncontroll.py`

 * *Files identical despite different names*

### Comparing `jrdb-model-0.1.0/src/jrdb_model.egg-info/PKG-INFO` & `jrdb-model-0.2.0/src/jrdb_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jrdb-model
-Version: 0.1.0
+Version: 0.2.0
 Summary: ORM for JRDB
 Home-page: https://github.com/astroripple/horseview
 Author: requrd
 Author-email: requrd1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/astroripple/horseview/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jrdb-model-0.1.0/src/jrdb_model.egg-info/SOURCES.txt` & `jrdb-model-0.2.0/src/jrdb_model.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/jrdb_model.egg-info/PKG-INFO
 src/jrdb_model.egg-info/SOURCES.txt
 src/jrdb_model.egg-info/dependency_links.txt
 src/jrdb_model.egg-info/requires.txt
 src/jrdb_model.egg-info/top_level.txt
 src/jrdb_model/domain/__init__.py
 src/jrdb_model/domain/bangumi.py
+src/jrdb_model/domain/calculated_score.py
 src/jrdb_model/domain/kaisai.py
 src/jrdb_model/domain/predict.py
 src/jrdb_model/domain/predict_race.py
 src/jrdb_model/domain/racehorse.py
 src/jrdb_model/domain/returninfo.py
 src/jrdb_model/domain/seiseki.py
 src/jrdb_model/domain/seisekirace.py
```

