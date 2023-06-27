# Comparing `tmp/ampel_lsst-0.8.4.tar.gz` & `tmp/ampel_lsst-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_lsst-0.8.4.tar", max compression
+gzip compressed data, was "ampel_lsst-0.8.5.tar", max compression
```

## Comparing `ampel_lsst-0.8.4.tar` & `ampel_lsst-0.8.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1512 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/LICENSE
--rw-r--r--   0        0        0      301 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/README.md
--rw-r--r--   0        0        0     3188 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/ElasticcAlertSupplier.py
--rw-r--r--   0        0        0     2467 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/LSSTAlertSupplier.py
--rw-r--r--   0        0        0    20365 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcDirAlertLoader.py
--rw-r--r--   0        0        0    10648 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py
--rw-r--r--   0        0        0    22184 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/KafkaAlertLoader.py
--rw-r--r--   0        0        0     1583 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/MultiAvroAlertLoader.py
--rw-r--r--   0        0        0      690 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTDPFilter.py
--rw-r--r--   0        0        0      686 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTFPFilter.py
--rw-r--r--   0        0        0      671 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTObjFilter.py
--rw-r--r--   0        0        0      750 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTCompilerOptions.py
--rwxr-xr-x   0        0        0     2986 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTDataPointShaper.py
--rw-r--r--   0        0        0     4945 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTMongoMuxer.py
--rw-r--r--   0        0        0     3110 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t0/ReallySimpleLSSTFilter.py
--rw-r--r--   0        0        0     8807 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t0/SimpleLSSTFilter.py
--rw-r--r--   0        0        0      296 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t1/LSSTT1Combiner.py
--rw-r--r--   0        0        0     2168 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertId.py
--rw-r--r--   0        0        0      912 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertJournal.py
--rw-r--r--   0        0        0     1159 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetDiaObject.py
--rw-r--r--   0        0        0      440 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/template/ElasticcAlertConsumerTemplate.py
--rw-r--r--   0        0        0      490 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/template/LSSTAlertConsumerTemplate.py
--rw-r--r--   0        0        0     3187 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/view/LSSTT2Tabulator.py
--rw-r--r--   0        0        0        0 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/py.typed
--rw-r--r--   0        0        0     1281 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/conf/ampel-lsst/ampel.yml
--rw-r--r--   0        0        0     2191 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 ampel_lsst-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/LICENSE
+-rw-r--r--   0        0        0      301 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/README.md
+-rw-r--r--   0        0        0     3311 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/ElasticcAlertSupplier.py
+-rw-r--r--   0        0        0     2467 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/LSSTAlertSupplier.py
+-rw-r--r--   0        0        0     1179 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/load/ElasticcDirAlertLoader.py
+-rw-r--r--   0        0        0    10692 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py
+-rw-r--r--   0        0        0     1878 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/load/HttpSchemaRepository.py
+-rw-r--r--   0        0        0     3014 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/load/KafkaAlertLoader.py
+-rw-r--r--   0        0        0     1583 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/alert/load/MultiAvroAlertLoader.py
+-rw-r--r--   0        0        0      690 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/aux/LSSTDPFilter.py
+-rw-r--r--   0        0        0      686 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/aux/LSSTFPFilter.py
+-rw-r--r--   0        0        0      671 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/aux/LSSTObjFilter.py
+-rw-r--r--   0        0        0      750 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTCompilerOptions.py
+-rwxr-xr-x   0        0        0     2986 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTDataPointShaper.py
+-rw-r--r--   0        0        0     4945 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTMongoMuxer.py
+-rw-r--r--   0        0        0     3110 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t0/ReallySimpleLSSTFilter.py
+-rw-r--r--   0        0        0     8807 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t0/SimpleLSSTFilter.py
+-rw-r--r--   0        0        0      296 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t1/LSSTT1Combiner.py
+-rw-r--r--   0        0        0     2168 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t2/T2GetAlertId.py
+-rw-r--r--   0        0        0      912 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t2/T2GetAlertJournal.py
+-rw-r--r--   0        0        0     1159 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/t2/T2GetDiaObject.py
+-rw-r--r--   0        0        0      440 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/template/ElasticcAlertConsumerTemplate.py
+-rw-r--r--   0        0        0      490 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/template/LSSTAlertConsumerTemplate.py
+-rw-r--r--   0        0        0     3187 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/lsst/view/LSSTT2Tabulator.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/ampel/py.typed
+-rw-r--r--   0        0        0     1281 2023-06-27 14:58:30.635846 ampel_lsst-0.8.5/conf/ampel-lsst/ampel.yml
+-rw-r--r--   0        0        0     2191 2023-06-27 14:58:30.639846 ampel_lsst-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 ampel_lsst-0.8.5/PKG-INFO
```

### Comparing `ampel_lsst-0.8.4/LICENSE` & `ampel_lsst-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/alert/ElasticcAlertSupplier.py` & `ampel_lsst-0.8.5/ampel/lsst/alert/ElasticcAlertSupplier.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 # Last Modified Date: 22.6.2022
 # Last Modified By  : j nordin <jnordin@physik.hu-berlin.de>
 
 import sys
 from typing import Literal, Optional, cast, TYPE_CHECKING
 from hashlib import blake2b
 from bson import encode
+from astropy.table import Table
 
 from ampel.alert.AmpelAlert import AmpelAlert
 from ampel.alert.BaseAlertSupplier import BaseAlertSupplier
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 from ampel.view.ReadOnlyDict import ReadOnlyDict
 
-if TYPE_CHECKING:
-    from astropy.table import Table
 
 
 
 class ElasticcAlertSupplier(BaseAlertSupplier):
     """
     Iterable class that, for each lightcurve provided by the underlying alert_loader,
     returns an AmpelAlert instance.
@@ -40,15 +39,18 @@
 
         lc = cast(Table, self._deserialize(next(self.alert_loader)))
 
         # Are these actually unique?
         sntype = lc.meta['sim_type_index']   # Again do not know how consistent these are
         # Try to generate a unique stock. Not sure how well this will work.
         # Lets see whether we still get dubplicates...
-        stock = int( lc.meta['snid']+str(abs(lc.meta['ra'])*10000)[0:2] )
+        if lc.meta['ra']==0.0:          # Unclear why this happens
+            stock = int( lc.meta['snid']+'99' )            
+        else:
+            stock = int( lc.meta['snid']+str(abs(lc.meta['ra'])*10000)[0:2] )
 
         # Generate datapoints.
         # Would be much more efficient if dps generation was done in Loader?
         dps = []
         all_ids = b""
         df = lc.to_pandas()
         for k, row in df.iterrows():
```

### Comparing `ampel_lsst-0.8.4/ampel/lsst/alert/LSSTAlertSupplier.py` & `ampel_lsst-0.8.5/ampel/lsst/alert/LSSTAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py` & `ampel_lsst-0.8.5/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
  'SIM_TEMPLATEMAG_r': float,
  'SIM_TEMPLATEMAG_i': float,
  'SIM_TEMPLATEMAG_z': float,
  'SIM_TEMPLATEMAG_Y': float,
  'SIM_HOSTLIB(g_obs)': float,
  'SIM_HOSTLIB(r_obs)': float,
  'SIM_HOSTLIB(i_obs)': float,
+ 'SIM_MJD_EXPLODE': float,
 }
 
 # Some meta key names were also changed between the training set and
 # the test stream. We here try to track and change these
 meta_namechange = {
     'dec': 'decl',
     'redshift_final': 'z_final',
@@ -257,14 +258,15 @@
 
         # Typecast meta and change to lower case
         self.lightcurve.meta = {
                 k.lower(): meta_dcast[k](v)
                    if (k in meta_dcast and v is not None)
                    else v for k, v in self.lightcurve.meta.items()
             }
+                
         # Rename fields
         for oldkey, newkey in meta_namechange.items():
             if oldkey in self.lightcurve.meta:
                 self.lightcurve.meta[newkey] = self.lightcurve.meta.pop(oldkey)
 
         # Guess whether this is an alert
         self.lightcurve['cause_alert'] = ( self.lightcurve['PHOTFLAG'] >= 4096)
```

### Comparing `ampel_lsst-0.8.4/ampel/lsst/alert/load/MultiAvroAlertLoader.py` & `ampel_lsst-0.8.5/ampel/lsst/alert/load/MultiAvroAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTDPFilter.py` & `ampel_lsst-0.8.5/ampel/lsst/aux/LSSTDPFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTFPFilter.py` & `ampel_lsst-0.8.5/ampel/lsst/aux/LSSTFPFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTObjFilter.py` & `ampel_lsst-0.8.5/ampel/lsst/aux/LSSTObjFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTCompilerOptions.py` & `ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTCompilerOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTDataPointShaper.py` & `ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTMongoMuxer.py` & `ampel_lsst-0.8.5/ampel/lsst/ingest/LSSTMongoMuxer.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/t0/ReallySimpleLSSTFilter.py` & `ampel_lsst-0.8.5/ampel/lsst/t0/ReallySimpleLSSTFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/t0/SimpleLSSTFilter.py` & `ampel_lsst-0.8.5/ampel/lsst/t0/SimpleLSSTFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertId.py` & `ampel_lsst-0.8.5/ampel/lsst/t2/T2GetAlertId.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertJournal.py` & `ampel_lsst-0.8.5/ampel/lsst/t2/T2GetAlertJournal.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetDiaObject.py` & `ampel_lsst-0.8.5/ampel/lsst/t2/T2GetDiaObject.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/ampel/lsst/view/LSSTT2Tabulator.py` & `ampel_lsst-0.8.5/ampel/lsst/view/LSSTT2Tabulator.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/conf/ampel-lsst/ampel.yml` & `ampel_lsst-0.8.5/conf/ampel-lsst/ampel.yml`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.4/pyproject.toml` & `ampel_lsst-0.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-lsst"
-version = "0.8.4"
+version = "0.8.5"
 description = "Legacy Survey of Space and Time support for the Ampel system"
 authors = [
     "Marcus Fenner <mf@physik.hu-berlinn.de>",
     "Valery Brinnel",
     "Jakob van Santen <jakob.van.santen@desy.de>",
     "Jakob Nordin",
 ]
@@ -41,19 +41,19 @@
 python = ">=3.10,<3.12"
 astropy = "^5.0.2"
 fastavro = "^1.3.2"
 ampel-ztf = {version = "^0.8.5", extras = ["kafka"]}
 ampel-alerts = {version = "^0.8.5"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.11.1"
 mongomock = "^4.1.2"
-mypy = "^1.1.1"
+mypy = "^1.4.0"
 pytest-timeout = "^2.1.0"
 pytest-asyncio = "^0.21.0"
 types-requests = "^2.25.9"
 before_after = "^1.0.1"
 isort = "^5.12.0"
 
 [build-system]
```

### Comparing `ampel_lsst-0.8.4/PKG-INFO` & `ampel_lsst-0.8.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: ampel-lsst
-Version: 0.8.4
+Version: 0.8.5
 Summary: Legacy Survey of Space and Time support for the Ampel system
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Marcus Fenner
 Author-email: mf@physik.hu-berlinn.de
 Maintainer: Marcus Fenner
 Maintainer-email: mf@physik.hu-berlinn.de
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Requires-Dist: ampel-alerts (>=0.8.5,<0.9.0)
 Requires-Dist: ampel-ztf[kafka] (>=0.8.5,<0.9.0)
 Requires-Dist: astropy (>=5.0.2,<6.0.0)
```

