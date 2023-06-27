# Comparing `tmp/hearthstone-7.1.0.tar.gz` & `tmp/hearthstone-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.1.0.tar", last modified: Fri Jun  2 18:48:02 2023, max compression
+gzip compressed data, was "hearthstone-7.2.0.tar", last modified: Tue Jun 27 19:54:14 2023, max compression
```

## Comparing `hearthstone-7.1.0.tar` & `hearthstone-7.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.364363 hearthstone-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-02 18:47:56.000000 hearthstone-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 18:48:02.364363 hearthstone-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 18:47:56.000000 hearthstone-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.360362 hearthstone-7.1.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    60583 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.364363 hearthstone-7.1.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.360362 hearthstone-7.1.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-02 18:48:02.364363 hearthstone-7.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-02 18:47:56.000000 hearthstone-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:54:14.753106 hearthstone-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-27 19:54:08.000000 hearthstone-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-27 19:54:14.753106 hearthstone-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-27 19:54:08.000000 hearthstone-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:54:14.753106 hearthstone-7.2.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:54:14.753106 hearthstone-7.2.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-27 19:54:08.000000 hearthstone-7.2.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:54:14.753106 hearthstone-7.2.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:54:14.000000 hearthstone-7.2.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 19:54:14.753106 hearthstone-7.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-27 19:54:08.000000 hearthstone-7.2.0/setup.py
```

### Comparing `hearthstone-7.1.0/LICENSE` & `hearthstone-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/PKG-INFO` & `hearthstone-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.1.0
+Version: 7.2.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.1.0/README.md` & `hearthstone-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/bountyxml.py` & `hearthstone-7.2.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/cardxml.py` & `hearthstone-7.2.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/dbf.py` & `hearthstone-7.2.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/deckstrings.py` & `hearthstone-7.2.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/entities.py` & `hearthstone-7.2.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/enums.py` & `hearthstone-7.2.0/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1069,14 +1069,15 @@
 	CORE = 1637
 	VANILLA = 1646
 	THE_SUNKEN_CITY = 1658  # Voyage to the Sunken City
 	REVENDRETH = 1691  # Murder at Castle Nathria
 	MERCENARIES_DEV = 1705
 	RETURN_OF_THE_LICH_KING = 1776
 	BATTLE_OF_THE_BANDS = 1809
+	TITANS = 1858
 	PATH_OF_ARTHAS = 1869
 
 	# Not actually present...
 	TAVERNS_OF_TIME = 1143
 	PLACEHOLDER_202204 = 1810
 
 	# Aliased from the original enums
@@ -1561,15 +1562,18 @@
 	BGT_PVPDR = 55
 	BGT_MERCENARIES_PVP = 56
 	BGT_MERCENARIES_PVE = 57
 	BGT_RANKED_CLASSIC = 58
 	BGT_CASUAL_CLASSIC = 59
 	BGT_MERCENARIES_PVE_COOP = 60
 	BGT_MERCENARIES_FRIENDLY = 61
-	# BGT_LAST = 62
+	BGT_BATTLEGROUNDS_PLAYER_VS_AI = 62,
+	BGT_RANKED_TWIST = 63,
+	BGT_CASUAL_TWIST = 64,
+	# BGT_LAST = 65
 
 	BGT_NEWBIE = BGT_CASUAL_STANDARD_NEWBIE
 	BGT_CASUAL_STANDARD = BGT_CASUAL_STANDARD_NORMAL
 
 	BGT_RESERVED_18_22 = BGT_MERCENARIES_PVP
 	BGT_RESERVED_18_23 = BGT_MERCENARIES_PVE
 
@@ -1583,36 +1587,44 @@
 ]
 
 STANDARD_GAME_TYPES = [
 	BnetGameType.BGT_CASUAL_STANDARD,
 	BnetGameType.BGT_RANKED_STANDARD,
 ]
 
+TWIST_GAME_TYPES = [
+	BnetGameType.BGT_CASUAL_TWIST,
+	BnetGameType.BGT_RANKED_TWIST,
+]
+
 WILD_GAME_TYPES = [
 	BnetGameType.BGT_CASUAL_WILD,
 	BnetGameType.BGT_RANKED_WILD,
 ]
 
 
 class FormatType(IntEnum):
 	"""PegasusShared.FormatType"""
 
 	FT_UNKNOWN = 0
 	FT_WILD = 1
 	FT_STANDARD = 2
 	FT_CLASSIC = 3
+	FT_TWIST = 4
 
 	@property
 	def name_global(self):
 		if self.name == "FT_WILD":
 			return "GLOBAL_WILD"
 		elif self.name == "FT_STANDARD":
 			return "GLOBAL_STANDARD"
 		elif self.name == "FT_CLASSIC":
 			return "GLOBAL_CLASSIC"
+		elif self.name == "FT_TWIST":
+			return "GLOBAL_TWIST"
 
 
 class GameType(IntEnum):
 	"""PegasusShared.GameType"""
 	GT_UNKNOWN = 0
 	GT_VS_AI = 1
 	GT_VS_FRIEND = 2
@@ -1653,23 +1665,27 @@
 		if self == GameType.GT_RANKED:
 			if format == FormatType.FT_WILD:
 				return BnetGameType.BGT_RANKED_WILD
 			elif format == FormatType.FT_STANDARD:
 				return BnetGameType.BGT_RANKED_STANDARD
 			elif format == FormatType.FT_CLASSIC:
 				return BnetGameType.BGT_RANKED_CLASSIC
+			elif format == FormatType.FT_TWIST:
+				return BnetGameType.BGT_RANKED_TWIST
 			else:
 				raise ValueError()
 		if self == GameType.GT_CASUAL:
 			if format == FormatType.FT_WILD:
 				return BnetGameType.BGT_CASUAL_WILD
 			elif format == FormatType.FT_STANDARD:
 				return BnetGameType.BGT_CASUAL_STANDARD
 			elif format == FormatType.FT_CLASSIC:
 				return BnetGameType.BGT_CASUAL_CLASSIC
+			elif format == FormatType.FT_TWIST:
+				return BnetGameType.BGT_CASUAL_TWIST
 			else:
 				raise ValueError()
 
 		return {
 			GameType.GT_UNKNOWN: BnetGameType.BGT_UNKNOWN,
 			GameType.GT_VS_AI: BnetGameType.BGT_VS_AI,
 			GameType.GT_VS_FRIEND: BnetGameType.BGT_FRIENDS,
@@ -2081,14 +2097,15 @@
 	YEAR_OF_THE_PHOENIX = 688
 	THE_SUNKEN_CITY = 694
 	STANDARD_PACK = 713
 	WILD_PACK = 714
 	GOLDEN_STANDARD_PACK = 716
 	REVENDRETH = 729
 	STORMWIND_GOLDEN = 737
+	TITANS = 819
 	RETURN_OF_THE_LICH_KING = 821
 	ALTERAC_VALLEY_GOLDEN = 841
 	BATTLE_OF_THE_BANDS = 854
 	PATH_OF_ARTHAS = 903
 
 	# Renamed
 	KOBOLDS_CATACOMBS = KOBOLDS_AND_CATACOMBS
```

### Comparing `hearthstone-7.1.0/hearthstone/mercenaryxml.py` & `hearthstone-7.2.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/stringsfile.py` & `hearthstone-7.2.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/utils/__init__.py` & `hearthstone-7.2.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone/xmlutils.py` & `hearthstone-7.2.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-7.2.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.1.0
+Version: 7.2.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.1.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-7.2.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.1.0/setup.cfg` & `hearthstone-7.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.1.0
+version = 7.2.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

