# Comparing `tmp/roktools-5.5.3.post2-py2.py3-none-any.whl.zip` & `tmp/roktools-5.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20937 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 12:14 roktools/__init__.py
+Zip file size: 20972 bytes, number of entries: 17
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 11:53 roktools/__init__.py
 -rw-r--r--  2.0 unx     4641 b- defN 23-May-29 14:14 roktools/cl.py
 -rw-r--r--  2.0 unx      400 b- defN 23-May-29 14:14 roktools/file.py
 -rw-r--r--  2.0 unx    33542 b- defN 23-May-29 14:14 roktools/geodetic.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-May-29 14:14 roktools/logger.py
 -rw-r--r--  2.0 unx     3613 b- defN 23-May-29 14:14 roktools/rinex.py
 -rw-r--r--  2.0 unx      861 b- defN 23-May-29 14:14 roktools/stats.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-May-29 14:14 roktools/tensorial.py
--rw-r--r--  2.0 unx     8792 b- defN 23-Jun-20 12:13 roktools/time.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 12:14 roktools/gnss/__init__.py
+-rw-r--r--  2.0 unx     9281 b- defN 23-Jun-21 11:51 roktools/time.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 11:53 roktools/gnss/__init__.py
 -rw-r--r--  2.0 unx     1769 b- defN 23-Jun-20 12:13 roktools/gnss/types.py
--rw-rw-rw-  2.0 unx     1067 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2683 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/WHEEL
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1350 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/RECORD
-17 files, 62023 bytes uncompressed, 18729 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 unx     1067 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2677 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1314 b- defN 23-Jun-21 11:53 roktools-5.6.0.dist-info/RECORD
+17 files, 62470 bytes uncompressed, 18836 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: roktools/gnss/__init__.py
 Comment: 
 
 Filename: roktools/gnss/types.py
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/LICENSE
+Filename: roktools-5.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/METADATA
+Filename: roktools-5.6.0.dist-info/METADATA
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/WHEEL
+Filename: roktools-5.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/entry_points.txt
+Filename: roktools-5.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/top_level.txt
+Filename: roktools-5.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: roktools-5.5.3.post2.dist-info/RECORD
+Filename: roktools-5.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## roktools/time.py

```diff
@@ -10,17 +10,17 @@
 GPS_TIME_START = datetime.datetime(1980, 1, 6, 0, 0, 0)
 J2000_TIME_START = datetime.datetime(2000, 1, 1, 12, 0, 0)
 SECONDS_IN_DAY = 24 * 60 * 60
 SECONDS_IN_WEEK = 86400 * 7
 GPS_AS_J2000 = -630763200
 
 
-class TimeScale(enum.Enum):
-    GPS = enum.auto()
-    UTC = enum.auto()
+class TimeScale(str,enum.Enum):
+    GPS = "GPS"
+    UTC = "UTC"
 
 
 class Timespan:
     def __init__(self, start: datetime.datetime, end: datetime.datetime):
         self.start = start
         self.end = end
 
@@ -53,22 +53,22 @@
         end = min(self.end, other.end)
         return Timespan(start, end)
 
     def __repr__(self) -> str:
         return self.__str__
 
 
-def get_gps_leapseconds(utc_date:datetime.date) -> datetime.timedelta:
+def get_gps_leapseconds(utc_date:datetime.datetime) -> datetime.timedelta:
 
-    if utc_date >= datetime.date(2017, 1, 1): return datetime.timedelta(seconds=18)
-    elif utc_date >= datetime.date(2015, 7, 1): return datetime.timedelta(seconds=17)
-    elif utc_date >= datetime.date(2012, 7, 1): return datetime.timedelta(seconds=16)
-    elif utc_date >= datetime.date(2009, 1, 1): return datetime.timedelta(seconds=15)
-    elif utc_date >= datetime.date(2006, 1, 1): return datetime.timedelta(seconds=14)
-    elif utc_date >= datetime.date(1999, 1, 1): return datetime.timedelta(seconds=13)
+    if utc_date >= datetime.datetime(2017, 1, 1): return datetime.timedelta(seconds=18)
+    elif utc_date >= datetime.datetime(2015, 7, 1): return datetime.timedelta(seconds=17)
+    elif utc_date >= datetime.datetime(2012, 7, 1): return datetime.timedelta(seconds=16)
+    elif utc_date >= datetime.datetime(2009, 1, 1): return datetime.timedelta(seconds=15)
+    elif utc_date >= datetime.datetime(2006, 1, 1): return datetime.timedelta(seconds=14)
+    elif utc_date >= datetime.datetime(1999, 1, 1): return datetime.timedelta(seconds=13)
 
     raise ValueError('No Leap second information for epochs prior to 1999-01-01')
 
 
 def to_week_tow(epoch: datetime.datetime) -> WeekTow:
     """
     Convert from datetime to GPS week
@@ -77,15 +77,15 @@
     WeekTow(week=1307, tow=480613.0, day_of_week=5)
 
     Conversion method based on algorithm provided in this link
     http://www.novatel.com/support/knowledge-and-learning/published-papers-and-documents/unit-conversions/
     """
 
     timedelta = epoch - GPS_TIME_START
-    leap_delta = get_gps_leapseconds(epoch.date())
+    leap_delta = get_gps_leapseconds(epoch)
 
     gpsw = int(timedelta.days / 7)
     day = timedelta.days - 7 * gpsw
     tow = timedelta.microseconds * 1e-6 + timedelta.seconds + day * SECONDS_IN_DAY + leap_delta.total_seconds()
 
     return WeekTow(gpsw, tow, day)
 
@@ -96,15 +96,15 @@
 
     >>> from_week_tow(1307, 480613.0)
     datetime.datetime(2005, 1, 28, 13, 30)
 
     """
     delta = datetime.timedelta(weeks=week, seconds=tow)
     gps_epoch = GPS_TIME_START + delta
-    leap_delta = -get_gps_leapseconds(gps_epoch.date())
+    leap_delta = -get_gps_leapseconds(gps_epoch)
 
     return gps_epoch + leap_delta
 
 
 def weektow_to_datetime(tow: float, week: int) -> datetime.datetime:
     import warnings
     warnings.warn("This function will be replaced by 'from_week_tow'", DeprecationWarning, stacklevel=2)
@@ -127,38 +127,47 @@
 
     # Rebase seconds from GPS start origin to J2000 start origin
     j2000s += GPS_AS_J2000
 
     return j2000s
 
 
-def to_j2000(epoch: datetime.datetime) -> float:
+def to_j2000(epoch: datetime.datetime, timescale: TimeScale = TimeScale.GPS) -> float:
     """
-    Convert from datetime toj2000 seconds
+    Convert from datetime  in UTC toj2000 seconds
+    The output will be in the TimeScale passed as parameter (default GPS)
 
     >>> to_j2000(datetime.datetime(2005, 1, 28, 13, 30, 0, 100001))
+    160191013.100001
+    >>> to_j2000(datetime.datetime(2005, 1, 28, 13, 30, 0, 100001), timescale=TimeScale.UTC)
     160191000.100001
     """
 
+    if timescale == TimeScale.GPS:
+        epoch = epoch + get_gps_leapseconds(epoch)
+      
     return (epoch - J2000_TIME_START).total_seconds()
     
 
-def from_j2000(j2000s: int, fraction_of_seconds: float = 0.0) -> datetime.datetime:
+def from_j2000(j2000s: int, fraction_of_seconds: float = 0.0, timescale: TimeScale = TimeScale.GPS) -> datetime.datetime:
     """
     Convert from J2000 epoch to datetime
 
     >>> from_j2000(160191000)
-    datetime.datetime(2005, 1, 28, 13, 30)
+    datetime.datetime(2005, 1, 28, 13, 29, 47)
 
-    >>> from_j2000(160191000, fraction_of_seconds = 0.1)
+    >>> from_j2000(160191000, fraction_of_seconds = 0.1, timescale = TimeScale.UTC)
     datetime.datetime(2005, 1, 28, 13, 30, 0, 100000)
     """
 
     microseconds = int(fraction_of_seconds * 1.0e6)
     epoch = J2000_TIME_START + datetime.timedelta(seconds=j2000s, microseconds=microseconds)
+    if timescale == TimeScale.GPS:
+        epoch = epoch - get_gps_leapseconds(epoch)
+
     return epoch
 
 
 def epoch_range(start_epoch, end_epoch, interval_s):
     """
     Iterate between 2 epochs with a given interval
```

## Comparing `roktools-5.5.3.post2.dist-info/LICENSE` & `roktools-5.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `roktools-5.5.3.post2.dist-info/METADATA` & `roktools-5.6.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 5.5.3.post2
+Version: 5.6.0
 Summary: Set of tools used in internal Rokubun projects
 Home-page: https://www.rokubun.cat
 Author: Àlex López, Miquel García
 Author-email: alex.lopez@rokubun.cat, miquel.garcia@rokubun.cat
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `roktools-5.5.3.post2.dist-info/RECORD` & `roktools-5.6.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 roktools/cl.py,sha256=LuRhDicv8eJAxvI7gbnG7RnOiRmEtyuUKg-nNcJlL1U,4641
 roktools/file.py,sha256=hJuPUBGz7MC600sfvOgwa2Md4uSHr10iChrW36sAeRQ,400
 roktools/geodetic.py,sha256=dxSoPxxooEyeKyEQqGfcb1WYmH9-Hl-kREtQu9kHpE4,33542
 roktools/logger.py,sha256=4kvcTWXPoiG-MlyP6B330l4Fu7MfCuDjuIlIiLA8f1Y,1479
 roktools/rinex.py,sha256=74IU4Nw-KKiAW1mTJd3UZYPH83oFQHppsfBejE8RH_Q,3613
 roktools/stats.py,sha256=I-XJdwktJIZgO7BIaEZYyGXQOpWBRLQCMStzRfmLvJk,861
 roktools/tensorial.py,sha256=RZ8-9Z926mQigYX9S0tjAa068jUMu5JkBElXLSLbYDY,1580
-roktools/time.py,sha256=9hEAAl-q8DxJuef28dSCtfdJU4sgz-tAf-bpnXyYVNc,8792
+roktools/time.py,sha256=UI6ywx8p4k57519GrDgwWOyKFkvZt4Zn9CLXkORXSHM,9281
 roktools/gnss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 roktools/gnss/types.py,sha256=ecRfonSn66LV5wQNexvbZPb_kClQxC1uvJcBY2HgoTk,1769
-roktools-5.5.3.post2.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
-roktools-5.5.3.post2.dist-info/METADATA,sha256=EXonOgkZ9JYtbJ0RFRIe5yKOR1SKOSuZA5ICOLZCZ7U,2683
-roktools-5.5.3.post2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-roktools-5.5.3.post2.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
-roktools-5.5.3.post2.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
-roktools-5.5.3.post2.dist-info/RECORD,,
+roktools-5.6.0.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
+roktools-5.6.0.dist-info/METADATA,sha256=_wguOyS2_lCpzWjXQbpGytK36S6fRQH5SEgId6RSA9g,2677
+roktools-5.6.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+roktools-5.6.0.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
+roktools-5.6.0.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
+roktools-5.6.0.dist-info/RECORD,,
```

