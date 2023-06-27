# Comparing `tmp/waivek-0.1.4.tar.gz` & `tmp/waivek-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waivek-0.1.4.tar", last modified: Mon Jun 26 17:14:25 2023, max compression
+gzip compressed data, was "waivek-0.1.5.tar", last modified: Tue Jun 27 16:39:31 2023, max compression
```

## Comparing `waivek-0.1.4.tar` & `waivek-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.381242 waivek-0.1.4/
--rw-rw-rw-   0        0        0      996 2023-06-26 17:14:25.381242 waivek-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-06-26 17:13:33.000000 waivek-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 17:14:25.381242 waivek-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1207 2023-06-26 17:14:14.000000 waivek-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.349557 waivek-0.1.4/waivek/
--rw-rw-rw-   0        0        0      377 2023-06-26 17:09:35.000000 waivek-0.1.4/waivek/__init__.py
--rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.4/waivek/color.py
--rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.4/waivek/common.py
--rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.4/waivek/db.py
--rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.4/waivek/error.py
--rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.4/waivek/frame.py
--rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.4/waivek/get.py
--rw-rw-rw-   0        0        0    28068 2023-06-26 13:01:20.000000 waivek-0.1.4/waivek/ic.py
--rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.4/waivek/print_utils.py
--rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.4/waivek/reltools.py
--rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.4/waivek/reqs.py
--rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.4/waivek/tdd.py
--rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.4/waivek/template.py
--rw-rw-rw-   0        0        0    21659 2023-06-26 13:01:55.000000 waivek-0.1.4/waivek/test.py
--rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.4/waivek/timer.py
--rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.4/waivek/trace.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.381242 waivek-0.1.4/waivek.egg-info/
--rw-rw-rw-   0        0        0      996 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 16:39:31.875562 waivek-0.1.5/
+-rw-rw-rw-   0        0        0     1470 2023-06-27 16:39:31.873567 waivek-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2023-06-27 07:27:31.000000 waivek-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:39:31.875562 waivek-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2023-06-27 16:39:28.000000 waivek-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:39:31.849558 waivek-0.1.5/waivek/
+-rw-rw-rw-   0        0        0      377 2023-06-26 17:09:35.000000 waivek-0.1.5/waivek/__init__.py
+-rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.5/waivek/color.py
+-rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.5/waivek/common.py
+-rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.5/waivek/db.py
+-rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.5/waivek/error.py
+-rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.5/waivek/frame.py
+-rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.5/waivek/get.py
+-rw-rw-rw-   0        0        0    28068 2023-06-27 06:18:33.000000 waivek-0.1.5/waivek/ic.py
+-rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.5/waivek/print_utils.py
+-rw-rw-rw-   0        0        0     1883 2023-06-27 04:31:33.000000 waivek-0.1.5/waivek/reltools.py
+-rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.5/waivek/reqs.py
+-rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.5/waivek/tdd.py
+-rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.5/waivek/template.py
+-rw-rw-rw-   0        0        0    23039 2023-06-27 07:29:46.000000 waivek-0.1.5/waivek/test.py
+-rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.5/waivek/timer.py
+-rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.5/waivek/trace.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:39:31.871560 waivek-0.1.5/waivek.egg-info/
+-rw-rw-rw-   0        0        0     1470 2023-06-27 16:39:31.000000 waivek-0.1.5/waivek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-27 16:39:31.000000 waivek-0.1.5/waivek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:39:31.000000 waivek-0.1.5/waivek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-27 16:39:31.000000 waivek-0.1.5/waivek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 16:39:31.000000 waivek-0.1.5/waivek.egg-info/top_level.txt
```

### Comparing `waivek-0.1.4/PKG-INFO` & `waivek-0.1.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,92 @@
-Metadata-Version: 2.1
-Name: waivek
-Version: 0.1.4
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-
-color
+Code - Print colored text
 
 ```
-from color import Code
+from waivek import Code
 print(Code.RED + "Hello, World!")
 ```
 
 common
 
 ```
-from common import Date, Timestamp
+from waivek import Date, Timestamp
 dt = Date("2020-01-01"
 timestamp = Timestamp(3600)
 ```
 
 ```
-from common import create_partitions, smart_pad, enumerate_count
+>>> Date(1672511400) == Date('2023-01-01')
+True
+
+>>> date = Date(1672511400)
+>>> date
+12:00 AM, Jan 01 (5 months ago)
+
+>>> date.epoch
+1672511400
+
+>>> date.string
+2023-01-01T00:00:00+05:30
+
+>>> date.timeago()
+5 months ago
+
+>>> str(date)
+12:00 AM, Jan 01 (5 months ago)
+
+>>> date.dt
+2023-01-01 00:00:00+05:30
+```
+
+
+```
+from waivek import create_partitions, smart_pad, enumerate_count
 ```
 
 db
 
 ```
-from db import db_init, insert_dictionaries
+from waivek import db_init, insert_dictionaries
 cursor, connection = db_init(db_path)
 insert_dictionaries(cursor, table_name, dictionaries)
 ```
 
 error
 
 ```
-from error import handler
+from waivek import handler
 with handler():
     main()
 ```
 
 get
 
 ```
-from get import aget
+from waivek import aget
 aget(urls)
 ```
 
 ic
 
 ```
-from ic import ic, ib
+from waivek import ic, ib
 ic({"key": "value"})
 ib(str)
 ```
 
-print\_utils
+print\_utils - Print and manipulate text.
 
 ```
-from print_utils import head, truncate, abbreviate
+from waivek import head, truncate, abbreviate
 ```
 
-reltools
+reltools - Do path manipulation relative to 
 
 ```
-from reltools import rel2abs, read, write
+from waivek import rel2abs, read, write
 ```
 
-timer
+timer - Measure execution time of code snippets
 
 ```
-from timer import Timer
+from waivek import Timer
 ```
-
-
```

### Comparing `waivek-0.1.4/waivek/color.py` & `waivek-0.1.5/waivek/color.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/common.py` & `waivek-0.1.5/waivek/common.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/db.py` & `waivek-0.1.5/waivek/db.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/error.py` & `waivek-0.1.5/waivek/error.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/frame.py` & `waivek-0.1.5/waivek/frame.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/get.py` & `waivek-0.1.5/waivek/get.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/ic.py` & `waivek-0.1.5/waivek/ic.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/print_utils.py` & `waivek-0.1.5/waivek/print_utils.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/reltools.py` & `waivek-0.1.5/waivek/reltools.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/reqs.py` & `waivek-0.1.5/waivek/reqs.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/tdd.py` & `waivek-0.1.5/waivek/tdd.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/test.py` & `waivek-0.1.5/waivek/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 # ./coc-enter.vim
+
+# print("__package__: " + __package__)
+
+if __package__ is None:
+    from os.path import sep
+    *_, __package__, _ = __file__.split(sep)
+
 from .timer import Timer   # Single Use
 timer = Timer()
 timer.start("test.py")
 from .color import Code    # Multi-Use
 from .error import handler # Single Use
 from .ic import ic         # Multi-Use
 import time
@@ -691,17 +698,65 @@
          "month": now - timedelta(days=30),
          "year": now - timedelta(days=365),
          "all": datetime(year=2005, month=1, day=1)
     }
     range_table = [ { "rangename": rangename, "start_epoch": int(dt.timestamp()), "end_epoch": int(now.timestamp()) } for rangename, dt in range_D.items() ]
     return { "range": range_table, "day": day_table }
 
+
+def simulate(expression):
+    import sys
+    from .frame import Frame
+    frame = Frame(sys._getframe(1))
+    start_line = frame.line.strip().replace("simulate(", "")[:-1]
+    end_line = expression
+    print(f">>> {start_line}")
+    print(end_line)
+    print()
+
+def test_summaries():
+    from .common import Date
+    from .ic import ic; ic
+    from datetime import datetime
+    dt = datetime.now()
+    year = dt.year
+    date_string = f"{year}-01-01"
+    date = Date(date_string)
+    epoch = date.epoch
+    epoch_string = f"Date({repr(date.epoch)})"
+    str_string = f"Date({repr(date_string)})"
+    strings = [epoch_string, str_string]
+    # print("\n".join([ "date = " + string for string in  strings]))
+    # ic(date.epoch)
+    # ic(date.string)
+    # ic(date.timeago())
+    # ic(str(date))
+    # ic(date.dt)
+
+    # print()
+    # print(">>> date.epoch")
+    # print(f"{date.epoch}")
+    # print()
+
+    print(f">>> Date({repr(epoch)}) == Date({repr(date_string)})")
+    print("True")
+    print()
+    print(f">>> date = Date({epoch})")
+    simulate(date)
+    simulate(date.epoch)
+    simulate(date.string)
+    simulate(date.timeago())
+    simulate(str(date))
+    simulate(date.dt)
+
+
+
 # Vim Command: NTF --- call s:PythonNewTestFunction()
 def main():
-    test_datenames()
+    test_summaries()
     # test_yield_list()
     # test_color_bash()
     # test_static_variable()
     # test_os_path()
     # test_pathlib()
     # test_pudb()
     # test_sys()
```

### Comparing `waivek-0.1.4/waivek/timer.py` & `waivek-0.1.5/waivek/timer.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.4/waivek/trace.py` & `waivek-0.1.5/waivek/trace.py`

 * *Files identical despite different names*

