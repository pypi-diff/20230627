# Comparing `tmp/py-helper-mod-0.0.33.tar.gz` & `tmp/py-helper-mod-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp33ds5ly2/py-helper-mod-0.0.33.tar", last modified: Tue May 30 02:27:06 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.35.tar", last modified: Mon Jun 26 22:26:58 2023, max compression
```

## Comparing `py-helper-mod-0.0.33.tar` & `py-helper-mod-0.0.35.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.33/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.33/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.33/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.33/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-30 02:27:06.000000 py-helper-mod-0.0.33/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81141 2023-05-30 02:26:34.000000 py-helper-mod-0.0.33/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    88590 2023-06-26 22:19:23.000000 py-helper-mod-0.0.35/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-06-26 22:26:58.588314 py-helper-mod-0.0.35/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-06-26 22:26:58.000000 py-helper-mod-0.0.35/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.35/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-06-26 22:26:58.592314 py-helper-mod-0.0.35/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.35/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-helper-mod-0.0.33/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.35/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.33
+Version: 0.0.35
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Py_Helper Package
 
 A collection of functions, classes and other small items I use for easing my coding experience.
-
-
```

### Comparing `py-helper-mod-0.0.33/LICENSE` & `py-helper-mod-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.33/PKG-INFO` & `py-helper-mod-0.0.35/py_helper_mod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.33
+Version: 0.0.35
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Py_Helper Package
 
 A collection of functions, classes and other small items I use for easing my coding experience.
-
-
```

### Comparing `py-helper-mod-0.0.33/py_helper.py` & `py-helper-mod-0.0.35/py_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3.8
+#!/usr/bin/env python3
 
 # The Usual Suspects
 # import keyser_soze
 import os, sys, io
 import shutil, subprocess, getpass
 import random
 import math
@@ -489,23 +489,24 @@
 			r"^\d{1,2}/\d{1,2}/\d{4}$\+\d{1,2}\:\d{1,2}\:\d{1,2}\s+([aA]|[pP])[mM]$" : r"%m/%d/%Y %H:%M:%S %p",
 			r"^\w+\s+\d{1,2}\s+\d{4}$" : r"%b %d %Y",
 			r"^\w+\s+\d{1,2}\s+\d{4}\s+\d{1,2}:\d{1,2}$" : r"%b %d %Y %H:%M",
 			r"^\w+\s+\d{1,2}\s+\d{4}\s+\d{1,2}:\d{1,2}\s+([aA]|[pP])[mM]$" : r"%b %d %Y %H:%M %p",
 			r"^\w+\s+\d{1,2}\s+\d{4}\s+\d{1,2}:\d{1,2}:\d{1,2}$" : r"%b %d %Y %H:%M:%S",
 			r"^\w+\s+\d{1,2}\s+\d{4}\s+\d{1,2}:\d{1,2}:\d{1,2}\s+([aA]|[pP])[mM]$" : r"%b %d %Y %H:%M:%S %p",
 			r"^\d{4}-\d{2}-\d{2}\s+\d{2}:\d{2}:\d{2}$" : r"%Y-%m-%d %H:%M:%S",
-			r"^\d{1,2}/\d{1,2}/\d{4}$\s+ \d{1,2}\:\d{1,2}\:\d{1,2}\s+([aA]|[pP])[mM]$" : r"%m/%d/%Y %H:%M:%S %p"
+			r"^\d{1,2}/\d{1,2}/\d{4}$\s+ \d{1,2}\:\d{1,2}\:\d{1,2}\s+([aA]|[pP])[mM]$" : r"%m/%d/%Y %H:%M:%S %p",
 		}
 
 	# Shortcut map
 	__ShortcutHandlers__ = {
 		"today" : None,
 		"lasthour" : None,
 		"yesterday" : None,
 		"weekago" : None,
+		"lastweek" : None,
 		"fortniteago" : None,
 		"monthago" : None,
 		"lastmonth" : None,
 		"yearago" : None,
 		"lastyear" : None,
 		"last24" : None,
 		"last48" : None,
@@ -517,27 +518,59 @@
 		"last2days" : None,
 		"last3days" : None,
 		"last4days" : None,
 		"last5days" : None,
 		"last10days" : None
 	}
 
+	__DeltaShortcutHandlers__ = {
+		"microseconds" : [ r"^(?P<count>\d+)mic(ro|rosec|roseconds){0,1}$", None, "Microseconds"],
+		"milliseconds" : [ r"^(?P<count>\d+)(ms|milliseconds){0,1}$", None, "Milliseconds" ],
+		"second" : [ r"^second$", None, "1 second" ],
+		"seconds" : [ r"^(?P<count>\d+)s(econd|econds){0,1}$", None, "Seconds" ],
+		"minute" : [ r"^m(min|minute){0,1}$", None, "1 minute"],
+		"minutes" : [ r"^(?P<count>\d+)m(inute|inutes){0,1}$", None, "minutes" ],
+		"hour" : [ r"^h(our){0,1}$", None, "1 Hour" ],
+		"hours" : [ r"^(?P<count>\d+)h(our|ours){0,1}$", None, "Hours" ],
+		"last24" : [ r"^last(?P<count>\d+)$", None, "Last 24 Hours" ],
+		"last48" : [ r"^last(?P<count>\d+)$", None, "Last 48 Hours" ],
+		"last72" : [ r"^last(?P<count>\d+)$", None, "Last 72 Hours" ],
+		"day" : [ r"^d(ay){0,1}$", None, "One day, 24 hours" ],
+		"days" : [ r"^(?P<count>\d+)d(ay|ays|s){0,1}$", None, "Days" ],
+		"week" : [ r"^w(eek){0,1}$", None, "1 Week, 7 days" ],
+		"weekago" : [ r"^weekago$", None, "One 7 day interval" ],
+		"weeks" : [ r"^(?P<count>\d+)w(eek|eeks|s){0,1}$", None, "7 day intervals" ],
+		"month" : [ r"^mon(th){0,1}$", None, "30 day interval" ],
+		"months" : [ r"^(?P<count>\d+)(M|mon){1}(onth|onths|th|ths){0,1}$", None, "30 day intervals, not accurate, I know" ],
+		"year" : [ r"^y(ear){0,1}$", None, "One year, 365 days" ],
+		"years" : [ r"^(?P<count>\d+)y(ear|ears){0,1}$", None, "Year intervals" ],
+		"decade" : [ r"^decade$", None, "One decade, 10 years"],
+		"decades" : [ r"^(?P<count>\d+)dec(ade|ades){0,1}$", None, "Decade intervals" ],
+		"century" : [ r"^century$", None, "One century, 100 years" ],
+		"centuries" : [ r"^(?P<count>\d+)cen(tury|turies){0,1}$", None, "Century intervals"],
+		"millenia" : [ r"^(?P<count>\d+)mil(lenia){0,1}$", None, "1000 year intervals" ]
+	}
+
 	# Short Cut Callbacks
 	Shortcuts = None
 
+	# Time Delta Shortcuts
+	DeltaShortcuts = None
+
 	# Last Converted Timestamp
 	Converted = None
 
 	# Init Shortcuts
 	def __init__(self,timestamp_str = None):
 		"""Init instance"""
 
 		super().__init__()
 
 		self.Shortcuts = dict(self.__ShortcutHandlers__)
+		self.DeltaShortcuts = dict(self.__DeltaShortcutHandlers__)
 
 		self.__FillMaps__()
 
 		if timestamp_str != None:
 			self.ConvertTimestamp(timestamp_str)
 
 	# Print Conversion map and shortcuts
@@ -545,14 +578,21 @@
 		"""Print Filters and Shortcuts"""
 
 		msg = CombiBar("Shortcuts") + "\n"
 
 		for shortcut in self.__ShortcutHandlers__.keys():
 			msg += f"{shortcut}\n"
 
+		msg += ("\n" + CombiBar("Time Delta Shortcuts") + "\n")
+
+		for name,list in self.__DeltaShortcutHandles__.keys():
+			pattern,func,comment = list
+
+			msg += f"{name:<20}\t{pattern:<25}\t{comment}\n"
+
 		msg += ("\n" + CombiBar("Conversion Formats") + "\n")
 
 		for reg,tsf in self.__time_formats__.items():
 			msg += f"{tsf:<20}\t{reg}\n"
 
 		if output:
 			Msg(msg)
@@ -731,14 +771,190 @@
 		if mapped_func:
 			value = mapped_func()
 		else:
 			pass
 
 		return value
 
+	def DeltaMicroseconds(self,count):
+		"""Microseconds Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(microseconds=count)
+
+		return delta
+
+	def DeltaMilliseconds(self,count):
+		"""Millisecond Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(milliseconds=count)
+
+		return delta
+
+	def DeltaSeconds(self,count):
+		"""Seconds Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(seconds=count)
+
+		return delta
+
+	def DeltaMinutes(self,count):
+		"""Minutes Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(minutes=count)
+
+		return delta
+
+	def DeltaHours(self,count):
+		"""Hours Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(hours=count)
+
+		return delta
+
+	def DeltaLastHoursX(self,count):
+		"""LastHour X Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(hours=count)
+
+		return delta
+
+	def DeltaDays(self,count):
+		"""Days Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=count)
+
+		return delta
+
+	def DeltaWeeks(self,count):
+		"""Weeks Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(weeks=count)
+
+		return delta
+
+	def DeltaMonths(self,count):
+		"""Months Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=(count*30))
+
+		return delta
+
+	def DeltaYears(self,count):
+		"""Years Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=(count*365))
+
+		return delta
+
+	def DeltaDecades(self,count):
+		"""Decades Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=((365*10)*count))
+
+		return delta
+
+	def DeltaCenturies(self,count):
+		"""Centuries Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=(((365*10)*100)*count))
+
+		return delta
+	def DeltaMillenia(self,count):
+		""" Delta Handler"""
+
+		delta = None
+
+		if count is not None:
+			delta = timedelta(days=(((365*10)*1000)*count))
+
+		return delta
+
+	def GetDelta(self,data):
+		"""Delta Handler Finder"""
+
+		entry = None
+		pattern = None
+		func = None
+		comment = None
+		delta = None
+
+		if data in self.DeltaShortcuts:
+			pattern, func, comment = self.DeltaShortcuts[data]
+
+			match = re.search(pattern,data)
+
+			if match is not None:
+				count = 1
+
+				if "count" in match.groupdict().keys():
+					count = int(match.group("count"))
+
+				delta = func(count)
+			else:
+				delta = func(1)
+		else:
+			for entry in self.DeltaShortcuts.items():
+				name,value = entry
+				pattern, func, comment = value
+
+				match = None
+
+				try:
+					match = re.search(pattern,data)
+				except Exception as err:
+					ErrMsg(err,f"Pattern, {pattern} caused an error")
+
+				if match is not None:
+					count = 1
+
+					if "count" in match.groupdict().keys():
+						count = int(match.group("count"))
+
+					delta = func(count)
+
+					break
+
+		return delta
+
 	# Convert a string Timestamp (or shortcut) into a datetime TimeStamp
 	def ConvertTimestamp(self,timestamp_str,zone=None):
 		"""Convert String timestamp to DateTime"""
 
 		key = None
 		parse_fmt = None
 		value = None
@@ -771,52 +987,91 @@
 			timestamp /= divider
 
 		new_timestamp = datetime.fromtimestamp(timestamp)
 
 		return new_timestamp
 
 	# Convert to Epoch Time
-	def ToEpoch(self,timestamp_str,multiplier=1):
+	def ToEpoch(self,timestamp,multiplier=1):
 		"""Convert Timestamp string to Epoch Time"""
 
-		value = self.ConvertTimestamp(timestamp_str)
+		value = 0
 
-		value = int(value.timestamp()) * multiplier
+		if type(timestamp) is str:
+			value = self.ConvertTimestamp(timestamp)
+			value = int(value.timestamp()) * multiplier
+		elif type(timestamp) is datetime:
+			value = timestamp.timestamp() * multiplier
 
 		return value
 
 	# Convert to Epoch Milliseconds
-	def ToEpochMilliseconds(self,timestamp_str):
+	def ToEpochMilliseconds(self,timestamp):
 		"""Convert timestamp string to Epoch Time in Milliseconds"""
 
-		value = self.ToEpoch(timestamp_str,multiplier=1000)
+		value = self.ToEpoch(timestamp,multiplier=1000)
 
 		return value
 
 	# Add/Replce Shortcut to shortcut table
 	def AddShortcut(self,shortcut,func):
 		"""Add/Replace a function to the shortcut table"""
 
 		self.Shortcuts[shortcut] = func
 
+	# Add Delta Shortcut
+	def AddDelta(self,name,func):
+		"""Add/Replace a function to the Delta Shortcuts table"""
+
+		self.DeltaShortcuts[name][1] = func
+
 	# Add Time Format Extractor
 	def AddTimeFormat(self,reg_exp,formatter):
 		"""Add Time Format Extractor"""
 
 		self.__time_formats__[reg_exp] = formatter
 
+	# Check Shortcut Strings
+	def InShortcuts(self,pattern):
+		"""Check to see if supplied string is in Shortcuts"""
+
+		if pattern.lower() in self.Shortcuts.keys():
+			return True
+
+		return False
+
+	def InDeltas(self,pattern):
+		"""Check to see if supplied string is in Delta Shortcuts"""
+
+		flag = False
+
+		if pattern.lower() in self.DeltaShortcuts.keys():
+			return not flag
+
+		for sc in self.DeltaShortcuts.keys():
+			entry = self.DeltaShortcuts[sc]
+
+			rep,func,comment = entry
+
+			if re.search(rep,pattern) is not None:
+				flag = True
+				break
+
+		return flag
+
 	# Fill in Maps
 	def __FillMaps__(self):
 		"""Fill shortcut map (router map) with shortcut replacement functions"""
 
 		# Time Shortcuts
 		self.AddShortcut("today",self.Today)
 		self.AddShortcut("lasthour",self.LastHour)
 		self.AddShortcut("yesterday",self.Yesterday)
 		self.AddShortcut("weekago",self.WeekAgo)
+		self.AddShortcut("lastweek",self.WeekAgo)
 		self.AddShortcut("fortniteago",self.FortniteAgo)
 		self.AddShortcut("monthago",self.MonthAgo)
 		self.AddShortcut("lastmonth",self.LastMonth)
 		self.AddShortcut("yearago",self.YearAgo)
 		self.AddShortcut("lastyear",self.LastYear)
 		self.AddShortcut("last24",self.Last24)
 		self.AddShortcut("last48",self.Last48)
@@ -827,14 +1082,41 @@
 		self.AddShortcut("lastday",self.Last24)
 		self.AddShortcut("last2days",self.Last2Days)
 		self.AddShortcut("last3days",self.Last3Days)
 		self.AddShortcut("last4days",self.Last4Days)
 		self.AddShortcut("last5days",self.Last5Days)
 		self.AddShortcut("last10days",self.Last10Days)
 
+		# Time Delta Shortcuts
+		self.AddDelta("microseconds",self.DeltaMicroseconds)
+		self.AddDelta("milliseconds",self.DeltaMilliseconds)
+		self.AddDelta("seconds",self.DeltaSeconds)
+		self.AddDelta("seconds",self.DeltaSeconds)
+		self.AddDelta("minute",self.DeltaMinutes)
+		self.AddDelta("minutes",self.DeltaMinutes)
+		self.AddDelta("hour",self.DeltaHours)
+		self.AddDelta("hours",self.DeltaHours)
+		self.AddDelta("last24",self.DeltaLastHoursX)
+		self.AddDelta("last48",self.DeltaLastHoursX)
+		self.AddDelta("last72",self.DeltaLastHoursX)
+		self.AddDelta("day",self.DeltaDays)
+		self.AddDelta("days",self.DeltaDays)
+		self.AddDelta("week",self.DeltaWeeks)
+		self.AddDelta("weekago",self.DeltaWeeks)
+		self.AddDelta("weeks",self.DeltaWeeks)
+		self.AddDelta("month",self.DeltaMonths)
+		self.AddDelta("months",self.DeltaMonths)
+		self.AddDelta("year",self.DeltaYears)
+		self.AddDelta("years",self.DeltaYears)
+		self.AddDelta("decade",self.DeltaDecades)
+		self.AddDelta("decades",self.DeltaDecades)
+		self.AddDelta("century",self.DeltaCenturies)
+		self.AddDelta("centuries",self.DeltaCenturies)
+		self.AddDelta("millenia",self.DeltaMillenia)
+
 # Rate Limiter Class
 class RateLimiter:
 	"""
 	Used to help regular the number of times a sequence of commands can be used in a given interval.
 	"""
 
 	times_per_interval = 1
@@ -899,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,33)
+VERSION=(0,0,34)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -973,14 +1255,17 @@
 # Get CreationTime For File As DateTime
 CreationTime = lambda filename : datetime.fromtimestamp(os.path.getctime(filename))
 # Get ModificationTime For File As DateTime
 ModificationTime = lambda filename : datetime.fromtimestamp(os.path.getmtime(filename))
 # Get AccessTime For File As DateTime
 AccessTime = lambda filename : datetime.fromtimestamp(os.path.getatime(filename))
 
+# Kewl (Stupid Diagnostic stuff)
+Kewl = lambda : print("Kewl")
+
 #
 # Functions
 #
 
 #
 # Debug, CmdLine and Module Mode Items
 #
@@ -3280,15 +3565,27 @@
 #
 
 # Test Stub
 def test(args):
 	CmdLineMode(True)
 	DebugMode(True)
 
-	Msg("Currently Empty")
+	#Msg("Currently Empty")
+
+	items = [ "1s", "2m", "3h", "4d", "5w", "6mon", "7y", "8dec", "9cen", "10centuries", "11mil", "decade", "week", "year", "month" ]
+
+	tsc = TimestampConverter()
+
+	for item in items:
+		if tsc.InDeltas(item):
+			td = tsc.GetDelta(item)
+
+			Msg(f"{item} = {td}")
+		else:
+			Msg(f"Hmmm, {item} not in deltas")
 
 #
 # Requisite Main Loop
 #
 
 if __name__ == "__main__":
 	CmdLineMode(True)
```

