# Comparing `tmp/hun-date-parser-0.2.0.tar.gz` & `tmp/hun-date-parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hun-date-parser-0.2.0.tar", last modified: Wed Jun  7 18:04:36 2023, max compression
+gzip compressed data, was "hun-date-parser-0.2.1.tar", last modified: Tue Jun 27 17:00:37 2023, max compression
```

## Comparing `hun-date-parser-0.2.0.tar` & `hun-date-parser-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/
--rw-rw-rw-   0        0        0     1035 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     6246 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5213 2023-06-07 17:34:49.000000 hun-date-parser-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:35.989882 hun-date-parser-0.2.0/hun_date_parser/
--rw-rw-rw-   0        0        0      354 2023-06-07 17:05:15.000000 hun-date-parser-0.2.0/hun_date_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.021130 hun-date-parser-0.2.0/hun_date_parser/date_parser/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/__init__.py
--rw-rw-rw-   0        0        0    17255 2023-06-07 16:48:16.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/date_parsers.py
--rw-rw-rw-   0        0        0    13654 2023-06-07 17:57:27.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/datetime_extractor.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.036754 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/
--rw-rw-rw-   0        0        0      222 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/__init__.py
--rw-rw-rw-   0        0        0     5789 2023-06-07 17:51:56.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
--rw-rw-rw-   0        0        0     4089 2023-05-31 06:07:00.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/patterns.py
--rw-rw-rw-   0        0        0     1212 2022-01-12 18:11:18.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/structure_parsers.py
--rw-rw-rw-   0        0        0     8862 2023-05-24 09:42:41.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/time_parsers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.036754 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/__init__.py
--rw-rw-rw-   0        0        0     1439 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/date2text.py
--rw-rw-rw-   0        0        0     2161 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/datetime_textualizer.py
--rw-rw-rw-   0        0        0     4182 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/time2text.py
--rw-rw-rw-   0        0        0     3965 2023-06-06 04:24:10.000000 hun-date-parser-0.2.0/hun_date_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.021130 hun-date-parser-0.2.0/hun_date_parser.egg-info/
--rw-rw-rw-   0        0        0     6246 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1097 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-07 17:16:42.000000 hun-date-parser-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/test/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/test/__init__.py
--rw-rw-rw-   0        0        0    13631 2023-06-07 17:51:56.000000 hun-date-parser-0.2.0/test/test_date_parsers.py
--rw-rw-rw-   0        0        0     2869 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/test/test_datetime2text.py
--rw-rw-rw-   0        0        0    11544 2023-06-07 17:56:26.000000 hun-date-parser-0.2.0/test/test_datetime_extractor.py
--rw-rw-rw-   0        0        0     1490 2022-01-11 15:16:22.000000 hun-date-parser-0.2.0/test/test_exposed.py
--rw-rw-rw-   0        0        0     4168 2022-01-15 12:11:36.000000 hun-date-parser-0.2.0/test/test_restricted_parsing.py
--rw-rw-rw-   0        0        0     1471 2022-01-26 17:28:30.000000 hun-date-parser-0.2.0/test/test_structure_parsers.py
--rw-rw-rw-   0        0        0     4315 2022-01-12 17:53:54.000000 hun-date-parser-0.2.0/test/test_time_parsers.py
--rw-rw-rw-   0        0        0     1074 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/
+-rw-rw-rw-   0        0        0     1035 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6246 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5310 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.705688 hun-date-parser-0.2.1/hun_date_parser/
+-rw-rw-rw-   0        0        0      360 2023-06-27 16:54:15.000000 hun-date-parser-0.2.1/hun_date_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.768663 hun-date-parser-0.2.1/hun_date_parser/date_parser/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/__init__.py
+-rw-rw-rw-   0        0        0    18115 2023-06-26 19:18:51.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/date_parsers.py
+-rw-rw-rw-   0        0        0    13981 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/datetime_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.784322 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/
+-rw-rw-rw-   0        0        0      226 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/__init__.py
+-rw-rw-rw-   0        0        0     5922 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
+-rw-rw-rw-   0        0        0     4242 2023-06-27 16:30:16.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/patterns.py
+-rw-rw-rw-   0        0        0     1212 2022-01-12 18:11:18.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/structure_parsers.py
+-rw-rw-rw-   0        0        0     9111 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/time_parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.799906 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/__init__.py
+-rw-rw-rw-   0        0        0     1439 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/date2text.py
+-rw-rw-rw-   0        0        0     2212 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/datetime_textualizer.py
+-rw-rw-rw-   0        0        0     4336 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/time2text.py
+-rw-rw-rw-   0        0        0     4159 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.737407 hun-date-parser-0.2.1/hun_date_parser.egg-info/
+-rw-rw-rw-   0        0        0     6246 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/test/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/test/__init__.py
+-rw-rw-rw-   0        0        0    14885 2023-06-27 16:31:59.000000 hun-date-parser-0.2.1/test/test_date_parsers.py
+-rw-rw-rw-   0        0        0     2939 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_datetime2text.py
+-rw-rw-rw-   0        0        0    11729 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_datetime_extractor.py
+-rw-rw-rw-   0        0        0     1531 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_exposed.py
+-rw-rw-rw-   0        0        0     4249 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_restricted_parsing.py
+-rw-rw-rw-   0        0        0     1498 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_structure_parsers.py
+-rw-rw-rw-   0        0        0     4417 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_time_parsers.py
+-rw-rw-rw-   0        0        0     1074 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/test/test_utils.py
```

### Comparing `hun-date-parser-0.2.0/LICENSE` & `hun-date-parser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.0/PKG-INFO` & `hun-date-parser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">Hungarian Date Parser</h1>
         
@@ -69,16 +69,16 @@
         An example:
         ```python
         from hun_date_parser import text2datetime
         from datetime import datetime
         from hun_date_parser.utils import SearchScopes
         
         text2datetime('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-        # [{'start_date': datetime.datetime(2023, 8, 1, 0, 0),
-        #   'end_date': datetime.datetime(2023, 8, 31, 23, 59, 59)}]
+        # [{'start_date': datetime.datetime(2022, 8, 1, 0, 0),
+        #   'end_date': datetime.datetime(2022, 8, 31, 23, 59, 59)}]
         
         text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
         # [{'start_date': datetime.datetime(2023, 6, 2, 0, 0),
         #   'end_date': datetime.datetime(2023, 6, 2, 23, 59, 59)}]
         
         text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED)
         # [{'start_date': datetime.datetime(2023, 6, 9, 0, 0),
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.0 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.1 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com License:
 UNKNOWN Description:
                       ****** Hungarian Date Parser ******
  A tool for extracting datetime intervals from Hungarian sentences and turning
                      datetime objects into Hungarian text.
@@ -40,16 +40,16 @@
 instance, given a scenario when May is parsed by the function, with this
 setting, if this year's May is still in the future, last year's May will be
 returned. - Please note, when there's no ambiguity, the function can still
 return future/past dates, even when a different preference is specified. An
 example: ```python from hun_date_parser import text2datetime from datetime
 import datetime from hun_date_parser.utils import SearchScopes text2datetime
 ('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-# [{'start_date': datetime.datetime(2023, 8, 1, 0, 0), # 'end_date':
-datetime.datetime(2023, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
+# [{'start_date': datetime.datetime(2022, 8, 1, 0, 0), # 'end_date':
+datetime.datetime(2022, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH) # [
 {'start_date': datetime.datetime(2023, 6, 2, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 2, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED) # [
 {'start_date': datetime.datetime(2023, 6, 9, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 9, 23, 59, 59)}] ``` The library is also capable of
 turning datetime objects into their Hungarian text representation. ```python
```

### Comparing `hun-date-parser-0.2.0/README.md` & `hun-date-parser-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-<h1 align="center">Hungarian Date Parser</h1>
-
-<p align="center">
-    <i>A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.</i>
-</p>
-
-
-<div align="center">
-    <a href="https://badge.fury.io/py/hun-date-parser"><img src="https://badge.fury.io/py/hun-date-parser.svg" alt="PyPI version" height="18"></a>
-    <img src="https://img.shields.io/github/stars/nsoma97/hun-date-parser" alt="Stars Badge"/>
-    <img src="https://img.shields.io/github/issues/nsoma97/hun-date-parser" alt="Issues Badge"/>
-    <img src="https://img.shields.io/github/license/nsoma97/hun-date-parser?color=2b9348" alt="License Badge"/>
-    <img src="https://img.shields.io/github/workflow/status/nsoma97/hun-date-parser/Datetime Parser Pipeline" alt="Tests"/>
-    <a href='https://coveralls.io/github/nsoma97/hun-date-parser'><img src='https://coveralls.io/repos/github/nsoma97/hun-date-parser/badge.svg' alt='Coverage Status' /></a>
-</div>
-
-<br>
-
-
-Install and try the package with `pip install hun-date-parser`
-
-## :fire: Usage
-
-If not specified otherwise, relative dates (eg.: tomorrow, next week, etc.) are calculated relative to the current datetime, at the time when the function is called. The `now` parameter can be used for parsing relative datetimes relative to any timestamp other than the current time.
-
-```python
-from hun_date_parser import text2datetime
-from datetime import datetime
-
-text2datetime('találkozzunk jövő kedd délután!', now=datetime(2020, 12, 27))
-# [{'start_date': datetime.datetime(2020, 12, 29, 12, 0), 'end_date': datetime.datetime(2020, 12, 29, 17, 59, 59)}]
-
-text2datetime('találkozzunk jövő héten szombaton háromnegyed nyolc előtt két perccel', now=datetime(2020, 12, 27))
-# [{'start_date': datetime.datetime(2021, 1, 2, 7, 43), 'end_date': datetime.datetime(2021, 1, 2, 7, 43, 59)}]
-
-text2datetime('találkozzunk jövő héten szombaton este háromnegyed nyolc előtt két perccel', now=datetime(2020, 12, 27))
-# [{'start_date': datetime.datetime(2021, 1, 2, 19, 43), 'end_date': datetime.datetime(2021, 1, 2, 19, 43, 59)}]
-```
-The date parser is also capable of parsing explicit intervals from the text even when only one side of the interval is specified.
-```python
-from hun_date_parser import text2datetime
-from datetime import datetime
-
-text2datetime('2020 decemberétől 2021 januárig', now=datetime(2020, 12, 27))
-# [{'start_date': datetime.datetime(2020, 12, 1, 0, 0), 'end_date': datetime.datetime(2021, 1, 31, 23, 59, 59)}]
-
-text2datetime('2021 januárig', now=datetime(2020, 12, 27))
-# [{'start_date': None, 'end_date': datetime.datetime(2021, 1, 31, 23, 59, 59)}]
-```
-
-For the function `text2datetime` the parameter `search_scope` is used to inform what is the desired time interval to parse the inputs.
-
-- The default value `SearchScopes.NOT_RESTRICTED` doesn't restrict the scope of the search.
-  - i.e.: when Tuesday is parsed the date for the Tuesday on the given week is going to be returned, not considering whether that given date is in the past or the future
-- To prefer future dates in case of ambiguity, use the value `SearchScopes.FUTURE_DAY`
-  - In this case, when Tuesday is parsed, the function will return the closest Tuesday in the future, not necessarily the current week's Tuesday.
-- Similarly to search in the future, nudging the library to prefer past dates is possible with the value `SearchScopes.PAST_SEARCH`
-  - For instance, given a scenario when May is parsed by the function, with this setting, if this year's May is still in the future, last year's May will be returned.
-  - Please note, when there's no ambiguity, the function can still return future/past dates, even when a different preference is specified.
-
-An example:
-```python
-from hun_date_parser import text2datetime
-from datetime import datetime
-from hun_date_parser.utils import SearchScopes
-
-text2datetime('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-# [{'start_date': datetime.datetime(2023, 8, 1, 0, 0),
-#   'end_date': datetime.datetime(2023, 8, 31, 23, 59, 59)}]
-
-text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-# [{'start_date': datetime.datetime(2023, 6, 2, 0, 0),
-#   'end_date': datetime.datetime(2023, 6, 2, 23, 59, 59)}]
-
-text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED)
-# [{'start_date': datetime.datetime(2023, 6, 9, 0, 0),
-#   'end_date': datetime.datetime(2023, 6, 9, 23, 59, 59)}]
-```
-
-The library is also capable of turning datetime objects into their Hungarian text representation.
-
-```python
-from hun_date_parser import datetime2text
-from datetime import datetime
-
-datetime2text(datetime(2020, 12, 20, 18, 34), now=datetime(2020, 12, 27), time_precision=2)
-# {'dates': ['múlt héten vasárnap', '2020 december 20'],
-#  'times': ['tizennyolc óra harmincnégy perc', '18:34', 'este hat óra harmincnégy perc', 'este fél 7 után 4 perccel']}
-```
-
-## :pencil: License
-
-This project is licensed under [MIT](https://choosealicense.com/licenses/mit/) license. Feel free to use it in your own projects.
-
-## :wrench: Contribute
-
-Any help or feedback in further developing the library is welcome!
+<h1 align="center">Hungarian Date Parser</h1>
+
+<p align="center">
+    <i>A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.</i>
+</p>
+
+
+<div align="center">
+    <a href="https://badge.fury.io/py/hun-date-parser"><img src="https://badge.fury.io/py/hun-date-parser.svg" alt="PyPI version" height="18"></a>
+    <img src="https://img.shields.io/github/stars/nsoma97/hun-date-parser" alt="Stars Badge"/>
+    <img src="https://img.shields.io/github/issues/nsoma97/hun-date-parser" alt="Issues Badge"/>
+    <img src="https://img.shields.io/github/license/nsoma97/hun-date-parser?color=2b9348" alt="License Badge"/>
+    <img src="https://img.shields.io/github/workflow/status/nsoma97/hun-date-parser/Datetime Parser Pipeline" alt="Tests"/>
+    <a href='https://coveralls.io/github/nsoma97/hun-date-parser'><img src='https://coveralls.io/repos/github/nsoma97/hun-date-parser/badge.svg' alt='Coverage Status' /></a>
+</div>
+
+<br>
+
+
+Install and try the package with `pip install hun-date-parser`
+
+## :fire: Usage
+
+If not specified otherwise, relative dates (eg.: tomorrow, next week, etc.) are calculated relative to the current datetime, at the time when the function is called. The `now` parameter can be used for parsing relative datetimes relative to any timestamp other than the current time.
+
+```python
+from hun_date_parser import text2datetime
+from datetime import datetime
+
+text2datetime('találkozzunk jövő kedd délután!', now=datetime(2020, 12, 27))
+# [{'start_date': datetime.datetime(2020, 12, 29, 12, 0), 'end_date': datetime.datetime(2020, 12, 29, 17, 59, 59)}]
+
+text2datetime('találkozzunk jövő héten szombaton háromnegyed nyolc előtt két perccel', now=datetime(2020, 12, 27))
+# [{'start_date': datetime.datetime(2021, 1, 2, 7, 43), 'end_date': datetime.datetime(2021, 1, 2, 7, 43, 59)}]
+
+text2datetime('találkozzunk jövő héten szombaton este háromnegyed nyolc előtt két perccel', now=datetime(2020, 12, 27))
+# [{'start_date': datetime.datetime(2021, 1, 2, 19, 43), 'end_date': datetime.datetime(2021, 1, 2, 19, 43, 59)}]
+```
+The date parser is also capable of parsing explicit intervals from the text even when only one side of the interval is specified.
+```python
+from hun_date_parser import text2datetime
+from datetime import datetime
+
+text2datetime('2020 decemberétől 2021 januárig', now=datetime(2020, 12, 27))
+# [{'start_date': datetime.datetime(2020, 12, 1, 0, 0), 'end_date': datetime.datetime(2021, 1, 31, 23, 59, 59)}]
+
+text2datetime('2021 januárig', now=datetime(2020, 12, 27))
+# [{'start_date': None, 'end_date': datetime.datetime(2021, 1, 31, 23, 59, 59)}]
+```
+
+For the function `text2datetime` the parameter `search_scope` is used to inform what is the desired time interval to parse the inputs.
+
+- The default value `SearchScopes.NOT_RESTRICTED` doesn't restrict the scope of the search.
+  - i.e.: when Tuesday is parsed the date for the Tuesday on the given week is going to be returned, not considering whether that given date is in the past or the future
+- To prefer future dates in case of ambiguity, use the value `SearchScopes.FUTURE_DAY`
+  - In this case, when Tuesday is parsed, the function will return the closest Tuesday in the future, not necessarily the current week's Tuesday.
+- Similarly to search in the future, nudging the library to prefer past dates is possible with the value `SearchScopes.PAST_SEARCH`
+  - For instance, given a scenario when May is parsed by the function, with this setting, if this year's May is still in the future, last year's May will be returned.
+  - Please note, when there's no ambiguity, the function can still return future/past dates, even when a different preference is specified.
+
+An example:
+```python
+from hun_date_parser import text2datetime
+from datetime import datetime
+from hun_date_parser.utils import SearchScopes
+
+text2datetime('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
+# [{'start_date': datetime.datetime(2022, 8, 1, 0, 0),
+#   'end_date': datetime.datetime(2022, 8, 31, 23, 59, 59)}]
+
+text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
+# [{'start_date': datetime.datetime(2023, 6, 2, 0, 0),
+#   'end_date': datetime.datetime(2023, 6, 2, 23, 59, 59)}]
+
+text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED)
+# [{'start_date': datetime.datetime(2023, 6, 9, 0, 0),
+#   'end_date': datetime.datetime(2023, 6, 9, 23, 59, 59)}]
+```
+
+The library is also capable of turning datetime objects into their Hungarian text representation.
+
+```python
+from hun_date_parser import datetime2text
+from datetime import datetime
+
+datetime2text(datetime(2020, 12, 20, 18, 34), now=datetime(2020, 12, 27), time_precision=2)
+# {'dates': ['múlt héten vasárnap', '2020 december 20'],
+#  'times': ['tizennyolc óra harmincnégy perc', '18:34', 'este hat óra harmincnégy perc', 'este fél 7 után 4 perccel']}
+```
+
+## :pencil: License
+
+This project is licensed under [MIT](https://choosealicense.com/licenses/mit/) license. Feel free to use it in your own projects.
+
+## :wrench: Contribute
+
+Any help or feedback in further developing the library is welcome!
```

#### html2text {}

```diff
@@ -39,16 +39,16 @@
 instance, given a scenario when May is parsed by the function, with this
 setting, if this year's May is still in the future, last year's May will be
 returned. - Please note, when there's no ambiguity, the function can still
 return future/past dates, even when a different preference is specified. An
 example: ```python from hun_date_parser import text2datetime from datetime
 import datetime from hun_date_parser.utils import SearchScopes text2datetime
 ('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-# [{'start_date': datetime.datetime(2023, 8, 1, 0, 0), # 'end_date':
-datetime.datetime(2023, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
+# [{'start_date': datetime.datetime(2022, 8, 1, 0, 0), # 'end_date':
+datetime.datetime(2022, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH) # [
 {'start_date': datetime.datetime(2023, 6, 2, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 2, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED) # [
 {'start_date': datetime.datetime(2023, 6, 9, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 9, 23, 59, 59)}] ``` The library is also capable of
 turning datetime objects into their Hungarian text representation. ```python
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/date_parsers.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/date_parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,412 +1,419 @@
-import re
-from typing import Dict, List, Any
-from datetime import datetime, timedelta, date
-from dateutil.relativedelta import relativedelta
-
-from .patterns import (R_ISO_DATE, R_NAMED_MONTH, R_TODAY, R_TOMORROW, R_NTOMORROW, R_YESTERDAY, R_NYESTERDAY,
-                       R_WEEKDAY, R_WEEK, R_YEAR, R_NDAYS_FROM_NOW, R_NWEEKS_FROM_NOW, R_NHOURS_FROM_NOW,
-                       R_NMINS_FROM_NOW, R_RELATIVE_MONTH, R_NMINS_PRIOR_NOW, R_NDAYS_PRIOR_NOW, R_NHOURS_PRIOR_NOW,
-                       R_NWEEKS_PRIOR_NOW, R_IN_PAST_PERIOD_MINS, R_IN_PAST_PERIOD_HOURS, R_IN_PAST_PERIOD_DAYS,
-                       R_IN_PAST_PERIOD_WEEKS, R_IN_PAST_PERIOD_MONTHS, R_IN_PAST_PERIOD_YEARS)
-from hun_date_parser.utils import (remove_accent, word_to_num, Year, Month, Week, Day, Hour, Minute,
-                                   OverrideTopWithNow, SearchScopes, return_on_value_error)
-
-
-def match_iso_date(s: str) -> List[Dict[str, Any]]:
-    """
-    Match ISO date-like format.
-    :param s: textual input
-    :return: tuple of date parts
-    """
-    match = re.findall(R_ISO_DATE, s)
-
-    res = []
-    if match:
-        for group in match:
-            group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
-
-            if len(group) == 1:
-                res.append({'match': group, 'date_parts': [Year(group[0], 'match_iso_date')]})
-            elif len(group) == 2:
-                res.append({'match': group,
-                            'date_parts': [Year(group[0], 'match_iso_date'), Month(group[1], 'match_iso_date')]})
-            elif len(group) == 3:
-                res.append({'match': group,
-                            'date_parts': [Year(group[0], 'match_iso_date'), Month(group[1], 'match_iso_date'),
-                                           Day(group[2], 'match_iso_date')]})
-
-    return res
-
-
-@return_on_value_error([])
-def match_named_month(s: str, now: datetime,
-                      search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, Any]]:
-
-    def has_month_already_pass(now, month):
-        return month < now.month
-
-    groups = re.findall(R_NAMED_MONTH, s)
-    months = ['jan', 'feb', 'mar', 'apr', 'maj', 'jun', 'jul', 'aug', 'szep', 'okt', 'nov', 'dec']
-
-    res = []
-    groups = [(mod, m, d.lstrip('0')) if
-              d else (mod, m, '') for mod, m, d in groups]
-
-    for group in groups:
-        group_res = {'match': group, 'date_parts': []}
-
-        month_detected = None
-        for i, month in enumerate(months):
-            if month in remove_accent(group[1]):
-                group_res['date_parts'].append(Month(i + 1, 'named_month'))
-                month_detected = i + 1
-                break
-
-        day_detected = None
-        if bool(group[2].strip(" ")) and month_detected is not None:
-            day_num = word_to_num(group[2])
-            if day_num != -1:
-                day_detected = day_num
-                group_res['date_parts'].append(Day(day_detected, 'named_month'))
-
-        detected_date_assumed_horizont = None
-        if month_detected is not None and day_detected is not None:
-            detected_month_day = date(now.year, month_detected, day_detected)
-            if detected_month_day == now.date():
-                detected_date_assumed_horizont = "current"
-            elif detected_month_day < now.date():
-                detected_date_assumed_horizont = "past"
-            else:
-                detected_date_assumed_horizont = "future"
-        elif month_detected is not None:
-            if now.month == month_detected:
-                detected_date_assumed_horizont = "current"
-            elif has_month_already_pass(now, month_detected):
-                detected_date_assumed_horizont = "past"
-            else:
-                detected_date_assumed_horizont = "future"
-
-        if month_detected is None:
-            continue
-
-        if bool(group[0].strip(" ")):
-            if 'jovo' in remove_accent(group[0]):
-                group_res['date_parts'].append(Year(now.year + 1, 'named_month'))
-            elif 'tavaly' in remove_accent(group[0]):
-                group_res['date_parts'].append(Year(now.year - 1, 'named_month'))
-        else:
-            if search_scope == SearchScopes.FUTURE_DAY and detected_date_assumed_horizont == "past":
-                group_res['date_parts'].append(Year(now.year + 1, 'named_month'))
-            elif search_scope == SearchScopes.PAST_SEARCH and detected_date_assumed_horizont == "future":
-                group_res['date_parts'].append(Year(now.year - 1, 'named_month'))
-
-        res.append(group_res)
-
-    return res
-
-
-def match_relative_day(s: str, now: datetime) -> List[Dict[str, Any]]:
-    groups = [*re.findall(R_TODAY, s),
-              *re.findall(R_TOMORROW, s),
-              *re.findall(R_NTOMORROW, s),
-              *re.findall(R_YESTERDAY, s),
-              *re.findall(R_NYESTERDAY, s)]
-
-    res = []
-    for group in groups:
-
-        if type(group) != str:
-            group = [m for m in group if m][0]
-
-        if 'ma' in group or 'má' in group:
-            res.append({'match': group, 'date_parts': [Year(now.year, 'relative_day'), Month(now.month, 'relative_day'),
-                                                       Day(now.day, 'relative_day')]})
-        elif 'holnapu' in group:
-            tom2 = now + timedelta(days=2)
-            res.append({'match': group,
-                        'date_parts': [Year(tom2.year, 'relative_day'), Month(tom2.month, 'relative_day'),
-                                       Day(tom2.day, 'relative_day')]})
-        elif 'holnap' in group:
-            tom = now + timedelta(days=1)
-            res.append({'match': group, 'date_parts': [Year(tom.year, 'relative_day'), Month(tom.month, 'relative_day'),
-                                                       Day(tom.day, 'relative_day')]})
-        elif 'tegnapel' in group:
-            yes2 = now - timedelta(days=2)
-            res.append({'match': group,
-                        'date_parts': [Year(yes2.year, 'relative_day'), Month(yes2.month, 'relative_day'),
-                                       Day(yes2.day, 'relative_day')]})
-        elif 'tegnap' in group:
-            yes = now - timedelta(days=1)
-            res.append({'match': group, 'date_parts': [Year(yes.year, 'relative_day'), Month(yes.month, 'relative_day'),
-                                                       Day(yes.day, 'relative_day')]})
-
-    return res
-
-
-def match_weekday(s: str, now: datetime,
-                  search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, Any]]:
-    groups = re.findall(R_WEEKDAY, s)
-
-    res = []
-    for group in groups:
-        date_parts = {'match': group, 'date_parts': []}
-        week, day = group
-        n_weeks = 0
-
-        if 'jovo' in remove_accent(week):
-            n_weeks = 1
-        elif 'mult' in remove_accent(week) or 'elozo' in remove_accent(week):
-            n_weeks = -1
-
-        def to_next_week(dt):
-            if dt.date() < now.date():
-                return dt + timedelta(days=7)
-            return dt
-
-        def to_last_week(dt):
-            if dt.date() > now.date():
-                return dt - timedelta(days=7)
-            return dt
-
-        def get_day_of_week(w, d):
-            return ((now - timedelta(days=now.weekday())) + timedelta(days=w * 7)) + timedelta(days=d)
-
-        day_num = -1
-        if 'hetfo' in remove_accent(day):
-            day_num = 0
-        elif 'kedd' in remove_accent(day):
-            day_num = 1
-        elif 'szerda' in remove_accent(day):
-            day_num = 2
-        elif 'csut' in remove_accent(day):
-            day_num = 3
-        elif 'pent' in remove_accent(day):
-            day_num = 4
-        elif 'szom' in remove_accent(day):
-            day_num = 5
-        elif 'vas' in remove_accent(day):
-            day_num = 6
-
-        if day_num != -1:
-            if search_scope == SearchScopes.PAST_SEARCH:
-                if n_weeks == 0:
-                    day = to_last_week(get_day_of_week(n_weeks, day_num))
-                else:
-                    day = get_day_of_week(n_weeks, day_num)
-            elif search_scope == SearchScopes.FUTURE_DAY:
-                if n_weeks == 0:
-                    day = to_next_week(get_day_of_week(n_weeks, day_num))
-                else:
-                    day = get_day_of_week(n_weeks, day_num)
-            else:
-                day = get_day_of_week(n_weeks, day_num)
-
-            date_parts['date_parts'] = [Year(day.year, 'weekday'), Month(day.month, 'weekday'), Day(day.day, 'weekday')]
-
-        res.append(date_parts)
-
-    return res
-
-
-def match_week(s: str, now: datetime) -> List[Dict[str, Any]]:
-    groups = re.findall(R_WEEK, s)
-
-    res = []
-    for group in groups:
-        date_parts = {'match': group, 'date_parts': []}
-
-        if 'ez' in group:
-            y, w = now.isocalendar()[0:2]
-            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
-        elif 'jovo' in remove_accent(group):
-            y, w = (now + timedelta(days=7)).isocalendar()[0:2]
-            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
-        elif 'mult' in remove_accent(group) or 'elozo' in remove_accent(group):
-            y, w = (now - timedelta(days=7)).isocalendar()[0:2]
-            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
-
-        res.append(date_parts)
-
-    return res
-
-
-def match_n_periods_compared_to_now(s: str, now: datetime) -> List[Dict[str, Any]]:
-    fn = 'n_date_periods_compared_to_now'
-
-    regexes = [
-        (R_NWEEKS_FROM_NOW, 'w', 'future'),
-        (R_NDAYS_FROM_NOW, 'd', 'future'),
-        (R_NHOURS_FROM_NOW, 'h', 'future'),
-        (R_NMINS_FROM_NOW, 'm', 'future'),
-        (R_NWEEKS_PRIOR_NOW, 'w', 'past'),
-        (R_NDAYS_PRIOR_NOW, 'd', 'past'),
-        (R_NHOURS_PRIOR_NOW, 'h', 'past'),
-        (R_NMINS_PRIOR_NOW, 'm', 'past'),
-    ]
-    res = []
-
-    for regex, freq, before_or_after in regexes:
-        multiplier = -1 if before_or_after == "past" else 1
-        groups = re.findall(regex, s)
-        for group in groups:
-            date_parts = {'match': group, 'date_parts': []}
-
-            n = group[1]
-            if n:
-                n = word_to_num(n)
-
-                if n == -1:
-                    continue
-
-                if freq == 'w':
-                    res_dt = (now + timedelta(days=multiplier * 7 * n))
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn)])
-                elif freq == 'd':
-                    res_dt = (now + timedelta(days=multiplier * n))
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn)])
-                elif freq == 'h':
-                    res_dt = (now + timedelta(hours=multiplier * n))
-                    y, m, d, h = res_dt.year, res_dt.month, res_dt.day, res_dt.hour
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn), Hour(h, fn)])
-                elif freq == 'm':
-                    res_dt = (now + timedelta(minutes=multiplier * n))
-                    y, mo, d, h, mi = res_dt.year, res_dt.month, res_dt.day, res_dt.hour, res_dt.minute
-                    date_parts['date_parts'].extend([Year(y, fn), Month(mo, fn),
-                                                     Day(d, fn), Hour(h, fn), Minute(mi, fn)])
-
-            res.append(date_parts)
-
-    return res
-
-
-def match_named_year(s: str, now: datetime) -> List[Dict[str, Any]]:
-    groups = re.findall(R_YEAR, s)
-
-    res = []
-    for group in groups:
-        date_parts = {'match': group, 'date_parts': []}
-
-        if 'tavalyelott' in remove_accent(group):
-            date_parts['date_parts'] = [Year(now.year - 2, 'named_year')]
-        elif 'tavaly' in remove_accent(group):
-            date_parts['date_parts'] = [Year(now.year - 1, 'named_year')]
-        elif 'iden' in remove_accent(group):
-            date_parts['date_parts'] = [Year(now.year, 'named_year')]
-        elif 'jovo' in remove_accent(group):
-            date_parts['date_parts'] = [Year(now.year + 1, 'named_year')]
-        elif 'mulva' in remove_accent(group):
-            num_after = word_to_num(group)
-
-            if num_after == -1:
-                continue
-
-            if num_after != -1:
-                date_parts['date_parts'] = [Year(now.year + num_after, 'named_year')]
-        elif 'ezelott' in remove_accent(group) or 'korabban' in remove_accent(group):
-            num_before = word_to_num(group)
-
-            if num_before == -1:
-                continue
-
-            if num_before != -1:
-                date_parts['date_parts'] = [Year(now.year - num_before, 'named_year')]
-
-        res.append(date_parts)
-
-    return res
-
-
-def match_relative_month(s: str, now: datetime) -> List[Dict[str, Any]]:
-    groups = re.findall(R_RELATIVE_MONTH, s)
-
-    res = []
-    for group in groups:
-        date_parts = {'match': group, 'date_parts': []}
-
-        if ('mult' in remove_accent(group)
-                or 'elozo' in remove_accent(group)
-                or 'utolso' in remove_accent(group)
-                or 'utobbi' in remove_accent(group)):
-            prev_month = now.date() + relativedelta(months=-1)
-            date_parts['date_parts'] = [Year(prev_month.year, 'relative_month'),
-                                        Month(prev_month.month, 'relative_month')]
-        elif (remove_accent(group).startswith("ezen")
-                or 'ebben' in remove_accent(group)
-                or 'aktualis' in remove_accent(group)):
-            date_parts['date_parts'] = [Year(now.year, 'relative_month'), Month(now.month, 'relative_month')]
-        elif ('jovo' in remove_accent(group)
-                or 'kovetkez' in remove_accent(group)):
-            next_month = now.date() + relativedelta(months=1)
-            date_parts['date_parts'] = [Year(next_month.year, 'relative_month'),
-                                        Month(next_month.month, 'relative_month')]
-
-        res.append(date_parts)
-
-    return res
-
-
-def match_in_past_n_periods(s: str, now: datetime) -> List[Dict[str, Any]]:
-    fn = 'in_past_n_periods'
-
-    regexes = [
-        (R_IN_PAST_PERIOD_YEARS, 'year', 'past'),
-        (R_IN_PAST_PERIOD_MONTHS, 'month', 'past'),
-        (R_IN_PAST_PERIOD_WEEKS, 'week', 'past'),
-        (R_IN_PAST_PERIOD_DAYS, 'day', 'past'),
-        (R_IN_PAST_PERIOD_HOURS, 'hour', 'past'),
-        (R_IN_PAST_PERIOD_MINS, 'minute', 'past'),
-    ]
-    res = []
-
-    for regex, freq, before_or_after in regexes:
-        multiplier = -1 if before_or_after == "past" else 1
-        groups = re.findall(regex, s)
-        for group in groups:
-            date_parts = {'match': group, 'date_parts': []}
-
-            n = group[1]
-            if n:
-                n = word_to_num(n) if n != " " else 1
-
-                if n == -1:
-                    continue
-
-                if freq == 'year':
-                    res_dt = (now + relativedelta(years=multiplier * n))
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
-                                                     OverrideTopWithNow(None, fn)])
-
-                elif freq == 'month':
-                    res_dt = now + relativedelta(months=multiplier * n)
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
-                                                     OverrideTopWithNow(None, fn)])
-
-                elif freq == 'week':
-                    res_dt = (now + timedelta(days=multiplier * 7 * n))
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
-                                                     OverrideTopWithNow(None, fn)])
-                elif freq == 'day':
-                    res_dt = (now + timedelta(days=multiplier * n))
-                    y, m, d = res_dt.year, res_dt.month, res_dt.day
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
-                                                     OverrideTopWithNow(None, fn)])
-                elif freq == 'hour':
-                    res_dt = (now + timedelta(hours=multiplier * n))
-                    y, m, d, h = res_dt.year, res_dt.month, res_dt.day, res_dt.hour
-                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn), Hour(h, fn),
-                                                     OverrideTopWithNow(None, fn)])
-                elif freq == 'minute':
-                    res_dt = (now + timedelta(minutes=multiplier * n))
-                    y, mo, d, h, mi = res_dt.year, res_dt.month, res_dt.day, res_dt.hour, res_dt.minute
-                    date_parts['date_parts'].extend([Year(y, fn), Month(mo, fn),
-                                                     Day(d, fn), Hour(h, fn), Minute(mi, fn),
-                                                     OverrideTopWithNow(None, fn)])
-
-            res.append(date_parts)
-
-    return res
+import re
+from typing import Dict, List, Any
+from datetime import datetime, timedelta, date
+from dateutil.relativedelta import relativedelta
+
+from .patterns import (R_ISO_DATE, R_REV_ISO_DATE, R_NAMED_MONTH, R_TODAY, R_TOMORROW, R_NTOMORROW, R_YESTERDAY,
+                       R_NYESTERDAY, R_WEEKDAY, R_WEEK, R_YEAR, R_NDAYS_FROM_NOW, R_NWEEKS_FROM_NOW, R_NHOURS_FROM_NOW,
+                       R_NMINS_FROM_NOW, R_RELATIVE_MONTH, R_NMINS_PRIOR_NOW, R_NDAYS_PRIOR_NOW, R_NHOURS_PRIOR_NOW,
+                       R_NWEEKS_PRIOR_NOW, R_IN_PAST_PERIOD_MINS, R_IN_PAST_PERIOD_HOURS, R_IN_PAST_PERIOD_DAYS,
+                       R_IN_PAST_PERIOD_WEEKS, R_IN_PAST_PERIOD_MONTHS, R_IN_PAST_PERIOD_YEARS)
+from hun_date_parser.utils import (remove_accent, word_to_num, Year, Month, Week, Day, Hour, Minute,
+                                   OverrideTopWithNow, SearchScopes, return_on_value_error)
+
+
+def match_iso_date(s: str) -> List[Dict[str, Any]]:
+    """
+    Match ISO date-like format.
+    :param s: textual input
+    :return: tuple of date parts
+    """
+    match = re.findall(R_ISO_DATE, s)
+    match_rev = re.findall(R_REV_ISO_DATE, s)
+
+    res = []
+    if match_rev:
+        for group in match_rev:
+            group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
+            res.append({'match': group,
+                        'date_parts': [Year(group[2], 'match_iso_date'),
+                                       Month(group[1], 'match_iso_date'),
+                                       Day(group[0], 'match_iso_date')]})
+    elif match:
+        for group in match:
+            group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
+
+            if len(group) == 1:
+                res.append({'match': group, 'date_parts': [Year(group[0], 'match_iso_date')]})
+            elif len(group) == 2:
+                res.append({'match': group,
+                            'date_parts': [Year(group[0], 'match_iso_date'), Month(group[1], 'match_iso_date')]})
+            elif len(group) == 3:
+                res.append({'match': group,
+                            'date_parts': [Year(group[0], 'match_iso_date'), Month(group[1], 'match_iso_date'),
+                                           Day(group[2], 'match_iso_date')]})
+
+    return res
+
+
+@return_on_value_error([])
+def match_named_month(s: str, now: datetime,
+                      search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, Any]]:
+    def has_month_already_pass(now, month):
+        return month < now.month
+
+    groups = re.findall(R_NAMED_MONTH, s)
+    months = ['jan', 'feb', 'mar', 'apr', 'maj', 'jun', 'jul', 'aug', 'szep', 'okt', 'nov', 'dec']
+
+    res = []
+    groups = [(mod, m, d.lstrip('0')) if
+              d else (mod, m, '') for mod, m, d in groups]
+
+    for group in groups:
+        group_res = {'match': group, 'date_parts': []}
+
+        month_detected = None
+        for i, month in enumerate(months):
+            if month in remove_accent(group[1]):
+                group_res['date_parts'].append(Month(i + 1, 'named_month'))
+                month_detected = i + 1
+                break
+
+        day_detected = None
+        if bool(group[2].strip(" ")) and month_detected is not None:
+            day_num = word_to_num(group[2])
+            if day_num != -1:
+                day_detected = day_num
+                group_res['date_parts'].append(Day(day_detected, 'named_month'))
+
+        detected_date_assumed_horizont = None
+        if month_detected is not None and day_detected is not None:
+            detected_month_day = date(now.year, month_detected, day_detected)
+            if detected_month_day == now.date():
+                detected_date_assumed_horizont = "current"
+            elif detected_month_day < now.date():
+                detected_date_assumed_horizont = "past"
+            else:
+                detected_date_assumed_horizont = "future"
+        elif month_detected is not None:
+            if now.month == month_detected:
+                detected_date_assumed_horizont = "current"
+            elif has_month_already_pass(now, month_detected):
+                detected_date_assumed_horizont = "past"
+            else:
+                detected_date_assumed_horizont = "future"
+
+        if month_detected is None:
+            continue
+
+        if bool(group[0].strip(" ")):
+            if 'jovo' in remove_accent(group[0]):
+                group_res['date_parts'].append(Year(now.year + 1, 'named_month'))
+            elif 'tavaly' in remove_accent(group[0]):
+                group_res['date_parts'].append(Year(now.year - 1, 'named_month'))
+        else:
+            if search_scope == SearchScopes.FUTURE_DAY and detected_date_assumed_horizont == "past":
+                group_res['date_parts'].append(Year(now.year + 1, 'named_month'))
+            elif search_scope == SearchScopes.PAST_SEARCH and detected_date_assumed_horizont == "future":
+                group_res['date_parts'].append(Year(now.year - 1, 'named_month'))
+
+        res.append(group_res)
+
+    return res
+
+
+def match_relative_day(s: str, now: datetime) -> List[Dict[str, Any]]:
+    groups = [*re.findall(R_TODAY, s),
+              *re.findall(R_TOMORROW, s),
+              *re.findall(R_NTOMORROW, s),
+              *re.findall(R_YESTERDAY, s),
+              *re.findall(R_NYESTERDAY, s)]
+
+    res = []
+    for group in groups:
+
+        if type(group) != str:
+            group = [m for m in group if m][0]
+
+        if 'ma' in group or 'má' in group:
+            res.append({'match': group, 'date_parts': [Year(now.year, 'relative_day'), Month(now.month, 'relative_day'),
+                                                       Day(now.day, 'relative_day')]})
+        elif 'holnapu' in group:
+            tom2 = now + timedelta(days=2)
+            res.append({'match': group,
+                        'date_parts': [Year(tom2.year, 'relative_day'), Month(tom2.month, 'relative_day'),
+                                       Day(tom2.day, 'relative_day')]})
+        elif 'holnap' in group:
+            tom = now + timedelta(days=1)
+            res.append({'match': group, 'date_parts': [Year(tom.year, 'relative_day'), Month(tom.month, 'relative_day'),
+                                                       Day(tom.day, 'relative_day')]})
+        elif 'tegnapel' in group:
+            yes2 = now - timedelta(days=2)
+            res.append({'match': group,
+                        'date_parts': [Year(yes2.year, 'relative_day'), Month(yes2.month, 'relative_day'),
+                                       Day(yes2.day, 'relative_day')]})
+        elif 'tegnap' in group:
+            yes = now - timedelta(days=1)
+            res.append({'match': group, 'date_parts': [Year(yes.year, 'relative_day'), Month(yes.month, 'relative_day'),
+                                                       Day(yes.day, 'relative_day')]})
+
+    return res
+
+
+def match_weekday(s: str, now: datetime,
+                  search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, Any]]:
+    groups = re.findall(R_WEEKDAY, s)
+
+    res = []
+    for group in groups:
+        date_parts = {'match': group, 'date_parts': []}
+        week, day = group
+        n_weeks = 0
+
+        if 'jovo' in remove_accent(week):
+            n_weeks = 1
+        elif 'mult' in remove_accent(week) or 'elozo' in remove_accent(week):
+            n_weeks = -1
+
+        def to_next_week(dt):
+            if dt.date() < now.date():
+                return dt + timedelta(days=7)
+            return dt
+
+        def to_last_week(dt):
+            if dt.date() > now.date():
+                return dt - timedelta(days=7)
+            return dt
+
+        def get_day_of_week(w, d):
+            return ((now - timedelta(days=now.weekday())) + timedelta(days=w * 7)) + timedelta(days=d)
+
+        day_num = -1
+        if 'hetfo' in remove_accent(day):
+            day_num = 0
+        elif 'kedd' in remove_accent(day):
+            day_num = 1
+        elif 'szerda' in remove_accent(day):
+            day_num = 2
+        elif 'csut' in remove_accent(day):
+            day_num = 3
+        elif 'pent' in remove_accent(day):
+            day_num = 4
+        elif 'szom' in remove_accent(day):
+            day_num = 5
+        elif 'vas' in remove_accent(day):
+            day_num = 6
+
+        if day_num != -1:
+            if search_scope == SearchScopes.PAST_SEARCH:
+                if n_weeks == 0:
+                    day = to_last_week(get_day_of_week(n_weeks, day_num))
+                else:
+                    day = get_day_of_week(n_weeks, day_num)
+            elif search_scope == SearchScopes.FUTURE_DAY:
+                if n_weeks == 0:
+                    day = to_next_week(get_day_of_week(n_weeks, day_num))
+                else:
+                    day = get_day_of_week(n_weeks, day_num)
+            else:
+                day = get_day_of_week(n_weeks, day_num)
+
+            date_parts['date_parts'] = [Year(day.year, 'weekday'), Month(day.month, 'weekday'), Day(day.day, 'weekday')]
+
+        res.append(date_parts)
+
+    return res
+
+
+def match_week(s: str, now: datetime) -> List[Dict[str, Any]]:
+    groups = re.findall(R_WEEK, s)
+
+    res = []
+    for group in groups:
+        date_parts = {'match': group, 'date_parts': []}
+
+        if 'ez' in group:
+            y, w = now.isocalendar()[0:2]
+            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
+        elif 'jovo' in remove_accent(group):
+            y, w = (now + timedelta(days=7)).isocalendar()[0:2]
+            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
+        elif 'mult' in remove_accent(group) or 'elozo' in remove_accent(group):
+            y, w = (now - timedelta(days=7)).isocalendar()[0:2]
+            date_parts['date_parts'].extend([Year(y, 'week'), Week(w, 'week')])
+
+        res.append(date_parts)
+
+    return res
+
+
+def match_n_periods_compared_to_now(s: str, now: datetime) -> List[Dict[str, Any]]:
+    fn = 'n_date_periods_compared_to_now'
+
+    regexes = [
+        (R_NWEEKS_FROM_NOW, 'w', 'future'),
+        (R_NDAYS_FROM_NOW, 'd', 'future'),
+        (R_NHOURS_FROM_NOW, 'h', 'future'),
+        (R_NMINS_FROM_NOW, 'm', 'future'),
+        (R_NWEEKS_PRIOR_NOW, 'w', 'past'),
+        (R_NDAYS_PRIOR_NOW, 'd', 'past'),
+        (R_NHOURS_PRIOR_NOW, 'h', 'past'),
+        (R_NMINS_PRIOR_NOW, 'm', 'past'),
+    ]
+    res = []
+
+    for regex, freq, before_or_after in regexes:
+        multiplier = -1 if before_or_after == "past" else 1
+        groups = re.findall(regex, s)
+        for group in groups:
+            date_parts = {'match': group, 'date_parts': []}
+
+            n = group[1]
+            if n:
+                n = word_to_num(n)
+
+                if n == -1:
+                    continue
+
+                if freq == 'w':
+                    res_dt = (now + timedelta(days=multiplier * 7 * n))
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn)])
+                elif freq == 'd':
+                    res_dt = (now + timedelta(days=multiplier * n))
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn)])
+                elif freq == 'h':
+                    res_dt = (now + timedelta(hours=multiplier * n))
+                    y, m, d, h = res_dt.year, res_dt.month, res_dt.day, res_dt.hour
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn), Hour(h, fn)])
+                elif freq == 'm':
+                    res_dt = (now + timedelta(minutes=multiplier * n))
+                    y, mo, d, h, mi = res_dt.year, res_dt.month, res_dt.day, res_dt.hour, res_dt.minute
+                    date_parts['date_parts'].extend([Year(y, fn), Month(mo, fn),
+                                                     Day(d, fn), Hour(h, fn), Minute(mi, fn)])
+
+            res.append(date_parts)
+
+    return res
+
+
+def match_named_year(s: str, now: datetime) -> List[Dict[str, Any]]:
+    groups = re.findall(R_YEAR, s)
+
+    res = []
+    for group in groups:
+        date_parts = {'match': group, 'date_parts': []}
+
+        if 'tavalyelott' in remove_accent(group):
+            date_parts['date_parts'] = [Year(now.year - 2, 'named_year')]
+        elif 'tavaly' in remove_accent(group):
+            date_parts['date_parts'] = [Year(now.year - 1, 'named_year')]
+        elif 'iden' in remove_accent(group):
+            date_parts['date_parts'] = [Year(now.year, 'named_year')]
+        elif 'jovo' in remove_accent(group):
+            date_parts['date_parts'] = [Year(now.year + 1, 'named_year')]
+        elif 'mulva' in remove_accent(group):
+            num_after = word_to_num(group)
+
+            if num_after == -1:
+                continue
+
+            if num_after != -1:
+                date_parts['date_parts'] = [Year(now.year + num_after, 'named_year')]
+        elif 'ezelott' in remove_accent(group) or 'korabban' in remove_accent(group):
+            num_before = word_to_num(group)
+
+            if num_before == -1:
+                continue
+
+            if num_before != -1:
+                date_parts['date_parts'] = [Year(now.year - num_before, 'named_year')]
+
+        res.append(date_parts)
+
+    return res
+
+
+def match_relative_month(s: str, now: datetime) -> List[Dict[str, Any]]:
+    groups = re.findall(R_RELATIVE_MONTH, s)
+
+    res = []
+    for group in groups:
+        date_parts = {'match': group, 'date_parts': []}
+
+        if ('mult' in remove_accent(group)
+                or 'elozo' in remove_accent(group)
+                or 'utolso' in remove_accent(group)
+                or 'utobbi' in remove_accent(group)):
+            prev_month = now.date() + relativedelta(months=-1)
+            date_parts['date_parts'] = [Year(prev_month.year, 'relative_month'),
+                                        Month(prev_month.month, 'relative_month')]
+        elif (remove_accent(group).startswith("ezen")
+              or 'ebben' in remove_accent(group)
+              or 'aktualis' in remove_accent(group)):
+            date_parts['date_parts'] = [Year(now.year, 'relative_month'), Month(now.month, 'relative_month')]
+        elif ('jovo' in remove_accent(group)
+              or 'kovetkez' in remove_accent(group)):
+            next_month = now.date() + relativedelta(months=1)
+            date_parts['date_parts'] = [Year(next_month.year, 'relative_month'),
+                                        Month(next_month.month, 'relative_month')]
+
+        res.append(date_parts)
+
+    return res
+
+
+def match_in_past_n_periods(s: str, now: datetime) -> List[Dict[str, Any]]:
+    fn = 'in_past_n_periods'
+
+    regexes = [
+        (R_IN_PAST_PERIOD_YEARS, 'year', 'past'),
+        (R_IN_PAST_PERIOD_MONTHS, 'month', 'past'),
+        (R_IN_PAST_PERIOD_WEEKS, 'week', 'past'),
+        (R_IN_PAST_PERIOD_DAYS, 'day', 'past'),
+        (R_IN_PAST_PERIOD_HOURS, 'hour', 'past'),
+        (R_IN_PAST_PERIOD_MINS, 'minute', 'past'),
+    ]
+    res = []
+
+    for regex, freq, before_or_after in regexes:
+        multiplier = -1 if before_or_after == "past" else 1
+        groups = re.findall(regex, s)
+        for group in groups:
+            date_parts = {'match': group, 'date_parts': []}
+
+            n = group[1]
+            if n:
+                n = word_to_num(n) if n != " " else 1
+
+                if n == -1:
+                    continue
+
+                if freq == 'year':
+                    res_dt = (now + relativedelta(years=multiplier * n))
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
+                                                     OverrideTopWithNow(None, fn)])
+
+                elif freq == 'month':
+                    res_dt = now + relativedelta(months=multiplier * n)
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
+                                                     OverrideTopWithNow(None, fn)])
+
+                elif freq == 'week':
+                    res_dt = (now + timedelta(days=multiplier * 7 * n))
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
+                                                     OverrideTopWithNow(None, fn)])
+                elif freq == 'day':
+                    res_dt = (now + timedelta(days=multiplier * n))
+                    y, m, d = res_dt.year, res_dt.month, res_dt.day
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn),
+                                                     OverrideTopWithNow(None, fn)])
+                elif freq == 'hour':
+                    res_dt = (now + timedelta(hours=multiplier * n))
+                    y, m, d, h = res_dt.year, res_dt.month, res_dt.day, res_dt.hour
+                    date_parts['date_parts'].extend([Year(y, fn), Month(m, fn), Day(d, fn), Hour(h, fn),
+                                                     OverrideTopWithNow(None, fn)])
+                elif freq == 'minute':
+                    res_dt = (now + timedelta(minutes=multiplier * n))
+                    y, mo, d, h, mi = res_dt.year, res_dt.month, res_dt.day, res_dt.hour, res_dt.minute
+                    date_parts['date_parts'].extend([Year(y, fn), Month(mo, fn),
+                                                     Day(d, fn), Hour(h, fn), Minute(mi, fn),
+                                                     OverrideTopWithNow(None, fn)])
+
+            res.append(date_parts)
+
+    return res
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/datetime_extractor.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/datetime_extractor.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,327 +1,327 @@
-"""This module handles combined date and time parsing."""
-
-from datetime import datetime, timedelta, date, time
-from calendar import monthrange
-from itertools import chain
-
-from typing import Dict, List, Union
-from copy import copy
-
-from hun_date_parser.date_parser.structure_parsers import match_multi_match, match_interval
-from hun_date_parser.date_parser.date_parsers import (match_named_month, match_iso_date, match_weekday,
-                                                      match_relative_day,
-                                                      match_week, match_named_year, match_n_periods_compared_to_now,
-                                                      match_relative_month, match_in_past_n_periods)
-from hun_date_parser.date_parser.time_parsers import match_digi_clock, match_time_words, match_now, match_hwords
-from hun_date_parser.utils import (Year, Month, Week, Day, Daypart, Hour, Minute, OverrideTopWithNow, SearchScopes,
-                                   OverrideBottomWithNow, monday_of_calenderweek, DateTimePartConatiner,
-                                   return_on_value_error)
-
-datelike = Union[datetime, date, time, None]
-
-daypart_mapping = [
-    (3, 5),     # hajnal
-    (6, 10),    # reggel
-    (8, 11),    # délelőtt
-    (12, 18),   # délután
-    (18, 21),   # este
-    (22, 2)     # éjjel
-]
-
-
-def text2datetime(input_sentence: str, now: datetime = datetime.now(),
-                  search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
-    """
-    Returns the list of datetime intervals found in the input sentence.
-    :param input_sentence: Input sentence string.
-    :param now: Current timestamp to calculate relative dates.
-    :param search_scope: Defines whether the timeframe should be restricted to past or future.
-    :return: list of datetime interval dictionaries
-    """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='datetime', search_scope=search_scope)
-    return datetime_extractor.parse_datetime(sentence=input_sentence)
-
-
-def text2date(input_sentence: str, now: datetime = datetime.now(),
-              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
-    """
-    Returns the list of date intervals found in the input sentence.
-    :param input_sentence: Input sentence string.
-    :param now: Current timestamp to calculate relative dates.
-    :param search_scope: Defines whether the timeframe should be restricted to past or future.
-    :return: list of date interval dictionaries
-    """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='date', search_scope=search_scope)
-    return datetime_extractor.parse_datetime(sentence=input_sentence)
-
-
-def text2time(input_sentence: str, now: datetime = datetime.now(),
-              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
-    """
-    Returns the list of time intervals found in the input sentence.
-    :param input_sentence: Input sentence string.
-    :param now: Current timestamp to calculate relative dates.
-    :param search_scope: Defines whether the timeframe should be restricted to past or future.
-    :return: list of time interval dictionaries
-    """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='time', search_scope=search_scope)
-    return datetime_extractor.parse_datetime(sentence=input_sentence)
-
-
-def match_rules(now: datetime, sentence: str,
-                search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List:
-    """
-    Matches all rules against input text.
-    :param now: Current timestamp to calculate relative dates.
-    :param sentence: Input sentence.
-    :param search_scope: Defines whether the timeframe should be restricted to past or future.
-    :return: Parsed date and time classes.
-    """
-    matches = [*match_named_month(sentence, now, search_scope),
-               *match_iso_date(sentence),
-               *match_relative_day(sentence, now),
-               *match_weekday(sentence, now, search_scope),
-               *match_week(sentence, now),
-               *match_named_year(sentence, now),
-               *match_digi_clock(sentence),
-               *match_hwords(sentence),
-               *match_time_words(sentence),
-               *match_now(sentence, now),
-               *match_n_periods_compared_to_now(sentence, now),
-               *match_relative_month(sentence, now),
-               *match_in_past_n_periods(sentence, now)]
-
-    matches = list(chain(*[m['date_parts'] for m in matches]))
-
-    return matches
-
-
-def extend_start_end(interval: Dict) -> Dict:
-    """
-    Heuristic to add missing date and time classes in case of interval.
-    :param interval: Dictionary with start and end dateparts.
-    :return: Extended dictionary with start and end dateparts.
-    """
-    if interval['start_date'] == 'OPEN' or interval['end_date'] == 'OPEN':
-        return interval
-
-    interval_ = copy(interval)
-    for dp in interval['start_date']:
-        if type(dp) not in [type(d) for d in interval['end_date']]:
-            interval_['end_date'].append(dp)
-
-    return interval_
-
-
-def type_isin_list(date_type: type, lst: Union[List, str]) -> bool:
-    if type(lst) == str:
-        return False
-
-    matches = [pot_dp for pot_dp in lst if isinstance(pot_dp, date_type)]
-
-    return bool(matches)
-
-
-class DatetimeExtractor:
-    """
-    This class handles combined date and time parsing.
-    """
-
-    def __init__(self, now: datetime = datetime.now(), output_container: str = 'datetime',
-                 search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> None:
-        """
-        :param now: Current timestamp to calculate relative dates.
-        :param output_container: datetime object to populate with datetime parts
-        :param search_scope: Defines whether the timeframe should be restricted to past or future.
-        """
-        self.now = now
-        self.output_container = output_container
-        self.search_scope = search_scope
-
-    def _get_implicit_intervall(self, sentence_part: str):
-        matches = match_rules(self.now, sentence_part, self.search_scope)
-        return [{'start_date': matches, 'end_date': matches}]
-
-    @return_on_value_error(None)
-    def assemble_datetime(self, now: datetime,
-                          dateparts: Union[List[Union[Year, Month, Week, Day, Daypart, Hour, Minute]], str],
-                          bottom: bool = True) -> datelike:
-        """
-        Assambles parsed date and time classes into datetime instance.
-        :param now: Current timestamp to calculate relative dates.
-        :param dateparts: List of date and time classes.
-        :param bottom: True if the bottom of the interval should be returned, False otherwise
-        :param output_container: datetime object to populate with datetime parts
-        :return: datetime instance
-        """
-        res_dt: List[int] = []
-
-        if dateparts == 'OPEN':
-            return None
-        if not dateparts:
-            return None
-
-        has_date, has_time = False, False
-
-        # this functionality is used to override the bottom or the top of the interval with the current date
-        # rules indicate the necessity for this with returning either OverrideBottomWithNow or OverrideTopWithNow
-        override_bottom, override_top = type_isin_list(OverrideBottomWithNow, dateparts),\
-            type_isin_list(OverrideTopWithNow, dateparts)
-
-        pre_first = True
-        for date_type in [Year, Month, Week, Day, Daypart, Hour, Minute]:
-            dp_match = [pot_dp for pot_dp in dateparts if isinstance(pot_dp, date_type)]
-
-            _dp_match: Union[DateTimePartConatiner, None]
-            if dp_match:
-                _dp_match = dp_match[0]
-            else:
-                _dp_match = None
-
-            if date_type == Year:
-                if _dp_match and _dp_match.value is not None:
-                    has_date = True
-                    pre_first = False
-                    res_dt.append(_dp_match.value)
-                else:
-                    # TODO: this should take into account the search_scope parameter...
-                    res_dt.append(now.year)
-
-            if date_type == Month:
-                if _dp_match and _dp_match.value is not None:
-                    has_date = True
-                    pre_first = False
-                    res_dt.append(_dp_match.value)
-                elif pre_first:
-                    res_dt.append(now.month)
-                elif bottom:
-                    res_dt.append(1)
-                else:
-                    res_dt.append(12)
-
-            if date_type == Week and not type_isin_list(Day, dateparts):
-                if _dp_match and _dp_match.value is not None:
-                    has_date = True
-                    pre_first = False
-                    week2dt = monday_of_calenderweek(res_dt[0], _dp_match.value) + timedelta(days=(0 if bottom else 6))
-                    res_dt = [week2dt.year, week2dt.month, week2dt.day]
-
-            if date_type == Day and len(res_dt) == 2:
-                if _dp_match and _dp_match.value is not None:
-                    has_date = True
-                    pre_first = False
-                    res_dt.append(_dp_match.value)
-                elif pre_first:
-                    res_dt.append(now.day)
-                elif bottom:
-                    res_dt.append(1)
-                else:
-                    mr = monthrange(res_dt[0], res_dt[1])
-                    res_dt.append(mr[1])
-
-            if date_type == Daypart:
-                if _dp_match and _dp_match.value is not None:
-                    has_time = True
-                    pre_first = False
-                    dp = _dp_match.value
-                    if bottom:
-                        res_dt.append(daypart_mapping[dp][0])
-                    elif dp == 5:
-                        y, m, d = res_dt
-                        next_day = datetime(y, m, d) + timedelta(days=1)
-                        res_dt = [next_day.year, next_day.month, next_day.day, daypart_mapping[dp][1]]
-                    else:
-                        res_dt.append(daypart_mapping[dp][1])
-
-            if date_type == Hour and len(res_dt) == 3:
-                if _dp_match and _dp_match.value is not None:
-                    has_time = True
-                    pre_first = False
-                    res_dt.append(_dp_match.value)
-                elif pre_first:
-                    res_dt.append(now.hour)
-                elif bottom:
-                    res_dt.append(0)
-                elif not bottom:
-                    res_dt.append(23)
-
-            if date_type == Minute:
-                if _dp_match and _dp_match.value is not None:
-                    has_time = True
-                    pre_first = False
-                    res_dt.append(_dp_match.value)
-                elif pre_first:
-                    res_dt.append(now.minute)
-                elif bottom:
-                    res_dt.append(0)
-                elif not bottom:
-                    res_dt.append(59)
-
-        if bottom:
-            res_dt.append(0)
-        else:
-            res_dt.append(59)
-
-        y, m, d, h, mi, s = res_dt
-
-        if self.output_container == 'datetime':
-            if bottom and override_bottom:
-                return now
-            elif not bottom and override_top:
-                return now
-            elif has_date or has_time:
-                return datetime(y, m, d, h, mi, s)
-            else:
-                return None
-        elif self.output_container == 'date':
-            if bottom and override_bottom:
-                return now.date()
-            elif not bottom and override_top:
-                return now.date()
-            elif has_date:
-                return date(y, m, d)
-            else:
-                return None
-        elif self.output_container == 'time':
-            if bottom and override_bottom:
-                return now.time()
-            elif not bottom and override_top:
-                return now.time()
-            elif has_time:
-                return time(h, mi, s)
-            else:
-                return None
-        else:
-            return None
-
-    def parse_datetime(self, sentence: str) -> List[Dict[str, datelike]]:
-        """
-        Extracts list of datetime intervals from input sentence.
-        :param sentence: Input sentence string.
-        :return: list of datetime interval dictionaries
-        """
-        sentence = sentence.lower()
-        sentence_parts = match_multi_match(sentence)
-        parsed_dates = []
-
-        for sentence_part in sentence_parts:
-            interval = match_interval(sentence_part)
-
-            if interval:
-                interval['start_date'] = 'OPEN' if interval['start_date'] == 'OPEN' else match_rules(self.now, interval[
-                    'start_date'], self.search_scope)
-                interval['end_date'] = 'OPEN' if interval['end_date'] == 'OPEN' else match_rules(self.now, interval[
-                    'end_date'], self.search_scope)
-                parsed_dates.append(interval)
-            else:
-                parsed_dates += self._get_implicit_intervall(sentence_part)
-
-        parsed_dates = [extend_start_end(intv) for intv in parsed_dates]
-
-        parsed_dates = [{'start_date': self.assemble_datetime(self.now, parsed_date['start_date'], bottom=True),
-                         'end_date': self.assemble_datetime(self.now, parsed_date['end_date'], bottom=False)}
-                        for parsed_date in parsed_dates]
-
-        parsed_dates = [intv for intv in parsed_dates if intv['start_date'] or intv['end_date']]
-
-        return parsed_dates
+"""This module handles combined date and time parsing."""
+
+from datetime import datetime, timedelta, date, time
+from calendar import monthrange
+from itertools import chain
+
+from typing import Dict, List, Union
+from copy import copy
+
+from hun_date_parser.date_parser.structure_parsers import match_multi_match, match_interval
+from hun_date_parser.date_parser.date_parsers import (match_named_month, match_iso_date, match_weekday,
+                                                      match_relative_day,
+                                                      match_week, match_named_year, match_n_periods_compared_to_now,
+                                                      match_relative_month, match_in_past_n_periods)
+from hun_date_parser.date_parser.time_parsers import match_digi_clock, match_time_words, match_now, match_hwords
+from hun_date_parser.utils import (Year, Month, Week, Day, Daypart, Hour, Minute, OverrideTopWithNow, SearchScopes,
+                                   OverrideBottomWithNow, monday_of_calenderweek, DateTimePartConatiner,
+                                   return_on_value_error)
+
+datelike = Union[datetime, date, time, None]
+
+daypart_mapping = [
+    (3, 5),     # hajnal
+    (6, 10),    # reggel
+    (8, 11),    # délelőtt
+    (12, 18),   # délután
+    (18, 21),   # este
+    (22, 2)     # éjjel
+]
+
+
+def text2datetime(input_sentence: str, now: datetime = datetime.now(),
+                  search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
+    """
+    Returns the list of datetime intervals found in the input sentence.
+    :param input_sentence: Input sentence string.
+    :param now: Current timestamp to calculate relative dates.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
+    :return: list of datetime interval dictionaries
+    """
+    datetime_extractor = DatetimeExtractor(now=now, output_container='datetime', search_scope=search_scope)
+    return datetime_extractor.parse_datetime(sentence=input_sentence)
+
+
+def text2date(input_sentence: str, now: datetime = datetime.now(),
+              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
+    """
+    Returns the list of date intervals found in the input sentence.
+    :param input_sentence: Input sentence string.
+    :param now: Current timestamp to calculate relative dates.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
+    :return: list of date interval dictionaries
+    """
+    datetime_extractor = DatetimeExtractor(now=now, output_container='date', search_scope=search_scope)
+    return datetime_extractor.parse_datetime(sentence=input_sentence)
+
+
+def text2time(input_sentence: str, now: datetime = datetime.now(),
+              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
+    """
+    Returns the list of time intervals found in the input sentence.
+    :param input_sentence: Input sentence string.
+    :param now: Current timestamp to calculate relative dates.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
+    :return: list of time interval dictionaries
+    """
+    datetime_extractor = DatetimeExtractor(now=now, output_container='time', search_scope=search_scope)
+    return datetime_extractor.parse_datetime(sentence=input_sentence)
+
+
+def match_rules(now: datetime, sentence: str,
+                search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List:
+    """
+    Matches all rules against input text.
+    :param now: Current timestamp to calculate relative dates.
+    :param sentence: Input sentence.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
+    :return: Parsed date and time classes.
+    """
+    matches = [*match_named_month(sentence, now, search_scope),
+               *match_iso_date(sentence),
+               *match_relative_day(sentence, now),
+               *match_weekday(sentence, now, search_scope),
+               *match_week(sentence, now),
+               *match_named_year(sentence, now),
+               *match_digi_clock(sentence),
+               *match_hwords(sentence),
+               *match_time_words(sentence),
+               *match_now(sentence, now),
+               *match_n_periods_compared_to_now(sentence, now),
+               *match_relative_month(sentence, now),
+               *match_in_past_n_periods(sentence, now)]
+
+    matches = list(chain(*[m['date_parts'] for m in matches]))
+
+    return matches
+
+
+def extend_start_end(interval: Dict) -> Dict:
+    """
+    Heuristic to add missing date and time classes in case of interval.
+    :param interval: Dictionary with start and end dateparts.
+    :return: Extended dictionary with start and end dateparts.
+    """
+    if interval['start_date'] == 'OPEN' or interval['end_date'] == 'OPEN':
+        return interval
+
+    interval_ = copy(interval)
+    for dp in interval['start_date']:
+        if type(dp) not in [type(d) for d in interval['end_date']]:
+            interval_['end_date'].append(dp)
+
+    return interval_
+
+
+def type_isin_list(date_type: type, lst: Union[List, str]) -> bool:
+    if type(lst) == str:
+        return False
+
+    matches = [pot_dp for pot_dp in lst if isinstance(pot_dp, date_type)]
+
+    return bool(matches)
+
+
+class DatetimeExtractor:
+    """
+    This class handles combined date and time parsing.
+    """
+
+    def __init__(self, now: datetime = datetime.now(), output_container: str = 'datetime',
+                 search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> None:
+        """
+        :param now: Current timestamp to calculate relative dates.
+        :param output_container: datetime object to populate with datetime parts
+        :param search_scope: Defines whether the timeframe should be restricted to past or future.
+        """
+        self.now = now
+        self.output_container = output_container
+        self.search_scope = search_scope
+
+    def _get_implicit_intervall(self, sentence_part: str):
+        matches = match_rules(self.now, sentence_part, self.search_scope)
+        return [{'start_date': matches, 'end_date': matches}]
+
+    @return_on_value_error(None)
+    def assemble_datetime(self, now: datetime,
+                          dateparts: Union[List[Union[Year, Month, Week, Day, Daypart, Hour, Minute]], str],
+                          bottom: bool = True) -> datelike:
+        """
+        Assambles parsed date and time classes into datetime instance.
+        :param now: Current timestamp to calculate relative dates.
+        :param dateparts: List of date and time classes.
+        :param bottom: True if the bottom of the interval should be returned, False otherwise
+        :param output_container: datetime object to populate with datetime parts
+        :return: datetime instance
+        """
+        res_dt: List[int] = []
+
+        if dateparts == 'OPEN':
+            return None
+        if not dateparts:
+            return None
+
+        has_date, has_time = False, False
+
+        # this functionality is used to override the bottom or the top of the interval with the current date
+        # rules indicate the necessity for this with returning either OverrideBottomWithNow or OverrideTopWithNow
+        override_bottom, override_top = type_isin_list(OverrideBottomWithNow, dateparts),\
+            type_isin_list(OverrideTopWithNow, dateparts)
+
+        pre_first = True
+        for date_type in [Year, Month, Week, Day, Daypart, Hour, Minute]:
+            dp_match = [pot_dp for pot_dp in dateparts if isinstance(pot_dp, date_type)]
+
+            _dp_match: Union[DateTimePartConatiner, None]
+            if dp_match:
+                _dp_match = dp_match[0]
+            else:
+                _dp_match = None
+
+            if date_type == Year:
+                if _dp_match and _dp_match.value is not None:
+                    has_date = True
+                    pre_first = False
+                    res_dt.append(_dp_match.value)
+                else:
+                    # TODO: this should take into account the search_scope parameter...
+                    res_dt.append(now.year)
+
+            if date_type == Month:
+                if _dp_match and _dp_match.value is not None:
+                    has_date = True
+                    pre_first = False
+                    res_dt.append(_dp_match.value)
+                elif pre_first:
+                    res_dt.append(now.month)
+                elif bottom:
+                    res_dt.append(1)
+                else:
+                    res_dt.append(12)
+
+            if date_type == Week and not type_isin_list(Day, dateparts):
+                if _dp_match and _dp_match.value is not None:
+                    has_date = True
+                    pre_first = False
+                    week2dt = monday_of_calenderweek(res_dt[0], _dp_match.value) + timedelta(days=(0 if bottom else 6))
+                    res_dt = [week2dt.year, week2dt.month, week2dt.day]
+
+            if date_type == Day and len(res_dt) == 2:
+                if _dp_match and _dp_match.value is not None:
+                    has_date = True
+                    pre_first = False
+                    res_dt.append(_dp_match.value)
+                elif pre_first:
+                    res_dt.append(now.day)
+                elif bottom:
+                    res_dt.append(1)
+                else:
+                    mr = monthrange(res_dt[0], res_dt[1])
+                    res_dt.append(mr[1])
+
+            if date_type == Daypart:
+                if _dp_match and _dp_match.value is not None:
+                    has_time = True
+                    pre_first = False
+                    dp = _dp_match.value
+                    if bottom:
+                        res_dt.append(daypart_mapping[dp][0])
+                    elif dp == 5:
+                        y, m, d = res_dt
+                        next_day = datetime(y, m, d) + timedelta(days=1)
+                        res_dt = [next_day.year, next_day.month, next_day.day, daypart_mapping[dp][1]]
+                    else:
+                        res_dt.append(daypart_mapping[dp][1])
+
+            if date_type == Hour and len(res_dt) == 3:
+                if _dp_match and _dp_match.value is not None:
+                    has_time = True
+                    pre_first = False
+                    res_dt.append(_dp_match.value)
+                elif pre_first:
+                    res_dt.append(now.hour)
+                elif bottom:
+                    res_dt.append(0)
+                elif not bottom:
+                    res_dt.append(23)
+
+            if date_type == Minute:
+                if _dp_match and _dp_match.value is not None:
+                    has_time = True
+                    pre_first = False
+                    res_dt.append(_dp_match.value)
+                elif pre_first:
+                    res_dt.append(now.minute)
+                elif bottom:
+                    res_dt.append(0)
+                elif not bottom:
+                    res_dt.append(59)
+
+        if bottom:
+            res_dt.append(0)
+        else:
+            res_dt.append(59)
+
+        y, m, d, h, mi, s = res_dt
+
+        if self.output_container == 'datetime':
+            if bottom and override_bottom:
+                return now
+            elif not bottom and override_top:
+                return now
+            elif has_date or has_time:
+                return datetime(y, m, d, h, mi, s)
+            else:
+                return None
+        elif self.output_container == 'date':
+            if bottom and override_bottom:
+                return now.date()
+            elif not bottom and override_top:
+                return now.date()
+            elif has_date:
+                return date(y, m, d)
+            else:
+                return None
+        elif self.output_container == 'time':
+            if bottom and override_bottom:
+                return now.time()
+            elif not bottom and override_top:
+                return now.time()
+            elif has_time:
+                return time(h, mi, s)
+            else:
+                return None
+        else:
+            return None
+
+    def parse_datetime(self, sentence: str) -> List[Dict[str, datelike]]:
+        """
+        Extracts list of datetime intervals from input sentence.
+        :param sentence: Input sentence string.
+        :return: list of datetime interval dictionaries
+        """
+        sentence = sentence.lower()
+        sentence_parts = match_multi_match(sentence)
+        parsed_dates = []
+
+        for sentence_part in sentence_parts:
+            interval = match_interval(sentence_part)
+
+            if interval:
+                interval['start_date'] = 'OPEN' if interval['start_date'] == 'OPEN' else match_rules(self.now, interval[
+                    'start_date'], self.search_scope)
+                interval['end_date'] = 'OPEN' if interval['end_date'] == 'OPEN' else match_rules(self.now, interval[
+                    'end_date'], self.search_scope)
+                parsed_dates.append(interval)
+            else:
+                parsed_dates += self._get_implicit_intervall(sentence_part)
+
+        parsed_dates = [extend_start_end(intv) for intv in parsed_dates]
+
+        parsed_dates = [{'start_date': self.assemble_datetime(self.now, parsed_date['start_date'], bottom=True),
+                         'end_date': self.assemble_datetime(self.now, parsed_date['end_date'], bottom=False)}
+                        for parsed_date in parsed_dates]
+
+        parsed_dates = [intv for intv in parsed_dates if intv['start_date'] or intv['end_date']]
+
+        return parsed_dates
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-"""
-This module (still WIP) implements extracting datetime intervals from pre-determined datetime intervals.
-If extraction within the set interval is not successful, the extraction falls back to the text2datetime function
-"""
-
-from datetime import datetime, date, time, timedelta
-from enum import Enum
-from typing import Dict, List, Union, Tuple
-from copy import deepcopy
-
-from hun_date_parser import text2datetime
-from hun_date_parser.utils import remove_accent, SearchScopes
-from hun_date_parser.date_parser.time_parsers import _raw_match_time_words
-
-datelike = Union[datetime, date, time, None]
-
-
-def get_reversed_am_pm(dt: datetime):
-    dt_ = deepcopy(dt)
-    if 0 < dt.hour < 12:
-        dt_ = datetime(dt.year, dt.month, dt.day, dt.hour + 12, dt.minute, dt.second)
-    elif not (dt.hour == 23 and dt.minute == 59) and dt.hour > 12:
-        dt_ = datetime(dt.year, dt.month, dt.day, dt.hour - 12, dt.minute, dt.second)
-    elif dt.hour == 12:
-        dt_ = dt_ + timedelta(days=1)
-        dt_ = datetime(dt_.year, dt_.month, dt_.day, 0, dt_.minute, dt_.second)
-
-    return dt_
-
-
-class ExtractWithinRangeSuccess(Enum):
-    VALID_IN_RANGE = 'in_range'
-    OUT_OF_RANGE_FALLBACK = 'out_of_range'
-    RELATIVE_TIME_WORD_FALLBACK = 'relative_time_word'
-    OPEN_RANGE_FALLBACK = 'open_range'
-    NO_MATCH_FALLBACK = 'no_match'
-
-
-def is_relative_datetime(query: str):
-    """
-    Determines wheter the query text refers to a relative datetime, ie.: next monday
-    """
-    relative_time_words = ['ma', 'holnap', 'holnaput', 'tegnap', 'tegnapel', 'jovo', 'mult']
-    transformed_query = remove_accent(query)
-
-    for time_word in relative_time_words:
-        if time_word in transformed_query:
-            return True
-
-    return False
-
-
-def extract_datetime_within_interval(interval_start: datetime,
-                                     interval_end: datetime,
-                                     query_text: str,
-                                     search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED,
-                                     fallback_now=datetime.now()) -> Tuple[ExtractWithinRangeSuccess,
-                                                                           List[Dict[str, datelike]]]:
-    """
-    Extracts datetime intervals from pre-determined datetime intervals.
-    :param interval_start: Bounding interval start
-    :param interval_end: Bounding interval end
-    :param query_text: Text to extract datetime interval from
-    :param search_scope: Sets the desired time horizont of the search.
-    :param fallback_now: When interval restriction is unsuccessful (RELATIVE_TIME_WORD_FALLBACK, OUT_OF_RANGE_FALLBACK)
-    the text2datetime function's result is returned, which can be supplied with a pseudo-now datetime
-    :return: success flag, restricted time interval
-    """
-
-    res = text2datetime(query_text,
-                        search_scope=search_scope,
-                        now=interval_start)
-
-    possible_am_pm_missmatch = False
-    parts = _raw_match_time_words(query_text)
-    if parts:
-        group, daypart, hour_modifier, hour, minute = parts
-        if not daypart and hour:
-            possible_am_pm_missmatch = True
-
-    extend_res = []
-    if possible_am_pm_missmatch:
-        for match in res:
-            if isinstance(match["start_date"], datetime) and isinstance(match["end_date"], datetime):
-                extend_res.append({
-                        "start_date": get_reversed_am_pm(match["start_date"]),
-                        "end_date": get_reversed_am_pm(match["end_date"])
-                    })
-
-    res += extend_res
-
-    restricted_date: List[Dict[str, datelike]] = []
-    response_candidates = [(5, ExtractWithinRangeSuccess.NO_MATCH_FALLBACK, restricted_date)]
-    for r in res:
-        if not (isinstance(r['start_date'], datetime) and isinstance(r['end_date'], datetime)):
-            response_type = ExtractWithinRangeSuccess.OPEN_RANGE_FALLBACK
-            restricted_date = text2datetime(query_text,
-                                            search_scope=search_scope,
-                                            now=fallback_now)
-
-            response_candidates.append((4, response_type, restricted_date))
-            continue
-
-        assert type(interval_start) == datetime and type(r['start_date']) == datetime
-        assert type(interval_end) == datetime and type(r['end_date']) == datetime
-        if not (interval_start <= r['start_date'] and r['end_date'] <= interval_end):
-            # Extracted datetime is out of expected interval...
-            response_type = ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK
-            restricted_date = text2datetime(query_text,
-                                            search_scope=search_scope,
-                                            now=fallback_now)
-
-            response_candidates.append((2, response_type, restricted_date))
-            continue
-
-        if is_relative_datetime(query_text):
-            # Datetime ranges relative to the current timestamp doesn't really make sense in this scenario...
-            response_type = ExtractWithinRangeSuccess.RELATIVE_TIME_WORD_FALLBACK
-            restricted_date = text2datetime(query_text,
-                                            search_scope=search_scope,
-                                            now=fallback_now)
-
-            response_candidates.append((3, response_type, restricted_date))
-        else:
-            response_type = ExtractWithinRangeSuccess.VALID_IN_RANGE
-            restricted_date = [r]
-
-            response_candidates.append((1, response_type, restricted_date))
-
-    response_candidates_ranked = sorted(response_candidates, key=lambda x: x[0])
-    _, response_type, restricted_date = response_candidates_ranked[0]
-
-    return response_type, restricted_date
+"""
+This module (still WIP) implements extracting datetime intervals from pre-determined datetime intervals.
+If extraction within the set interval is not successful, the extraction falls back to the text2datetime function
+"""
+
+from datetime import datetime, date, time, timedelta
+from enum import Enum
+from typing import Dict, List, Union, Tuple
+from copy import deepcopy
+
+from hun_date_parser import text2datetime
+from hun_date_parser.utils import remove_accent, SearchScopes
+from hun_date_parser.date_parser.time_parsers import _raw_match_time_words
+
+datelike = Union[datetime, date, time, None]
+
+
+def get_reversed_am_pm(dt: datetime):
+    dt_ = deepcopy(dt)
+    if 0 < dt.hour < 12:
+        dt_ = datetime(dt.year, dt.month, dt.day, dt.hour + 12, dt.minute, dt.second)
+    elif not (dt.hour == 23 and dt.minute == 59) and dt.hour > 12:
+        dt_ = datetime(dt.year, dt.month, dt.day, dt.hour - 12, dt.minute, dt.second)
+    elif dt.hour == 12:
+        dt_ = dt_ + timedelta(days=1)
+        dt_ = datetime(dt_.year, dt_.month, dt_.day, 0, dt_.minute, dt_.second)
+
+    return dt_
+
+
+class ExtractWithinRangeSuccess(Enum):
+    VALID_IN_RANGE = 'in_range'
+    OUT_OF_RANGE_FALLBACK = 'out_of_range'
+    RELATIVE_TIME_WORD_FALLBACK = 'relative_time_word'
+    OPEN_RANGE_FALLBACK = 'open_range'
+    NO_MATCH_FALLBACK = 'no_match'
+
+
+def is_relative_datetime(query: str):
+    """
+    Determines wheter the query text refers to a relative datetime, ie.: next monday
+    """
+    relative_time_words = ['ma', 'holnap', 'holnaput', 'tegnap', 'tegnapel', 'jovo', 'mult']
+    transformed_query = remove_accent(query)
+
+    for time_word in relative_time_words:
+        if time_word in transformed_query:
+            return True
+
+    return False
+
+
+def extract_datetime_within_interval(interval_start: datetime,
+                                     interval_end: datetime,
+                                     query_text: str,
+                                     search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED,
+                                     fallback_now=datetime.now()) -> Tuple[ExtractWithinRangeSuccess,
+                                                                           List[Dict[str, datelike]]]:
+    """
+    Extracts datetime intervals from pre-determined datetime intervals.
+    :param interval_start: Bounding interval start
+    :param interval_end: Bounding interval end
+    :param query_text: Text to extract datetime interval from
+    :param search_scope: Sets the desired time horizont of the search.
+    :param fallback_now: When interval restriction is unsuccessful (RELATIVE_TIME_WORD_FALLBACK, OUT_OF_RANGE_FALLBACK)
+    the text2datetime function's result is returned, which can be supplied with a pseudo-now datetime
+    :return: success flag, restricted time interval
+    """
+
+    res = text2datetime(query_text,
+                        search_scope=search_scope,
+                        now=interval_start)
+
+    possible_am_pm_missmatch = False
+    parts = _raw_match_time_words(query_text)
+    if parts:
+        group, daypart, hour_modifier, hour, minute = parts
+        if not daypart and hour:
+            possible_am_pm_missmatch = True
+
+    extend_res = []
+    if possible_am_pm_missmatch:
+        for match in res:
+            if isinstance(match["start_date"], datetime) and isinstance(match["end_date"], datetime):
+                extend_res.append({
+                        "start_date": get_reversed_am_pm(match["start_date"]),
+                        "end_date": get_reversed_am_pm(match["end_date"])
+                    })
+
+    res += extend_res
+
+    restricted_date: List[Dict[str, datelike]] = []
+    response_candidates = [(5, ExtractWithinRangeSuccess.NO_MATCH_FALLBACK, restricted_date)]
+    for r in res:
+        if not (isinstance(r['start_date'], datetime) and isinstance(r['end_date'], datetime)):
+            response_type = ExtractWithinRangeSuccess.OPEN_RANGE_FALLBACK
+            restricted_date = text2datetime(query_text,
+                                            search_scope=search_scope,
+                                            now=fallback_now)
+
+            response_candidates.append((4, response_type, restricted_date))
+            continue
+
+        assert type(interval_start) == datetime and type(r['start_date']) == datetime
+        assert type(interval_end) == datetime and type(r['end_date']) == datetime
+        if not (interval_start <= r['start_date'] and r['end_date'] <= interval_end):
+            # Extracted datetime is out of expected interval...
+            response_type = ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK
+            restricted_date = text2datetime(query_text,
+                                            search_scope=search_scope,
+                                            now=fallback_now)
+
+            response_candidates.append((2, response_type, restricted_date))
+            continue
+
+        if is_relative_datetime(query_text):
+            # Datetime ranges relative to the current timestamp doesn't really make sense in this scenario...
+            response_type = ExtractWithinRangeSuccess.RELATIVE_TIME_WORD_FALLBACK
+            restricted_date = text2datetime(query_text,
+                                            search_scope=search_scope,
+                                            now=fallback_now)
+
+            response_candidates.append((3, response_type, restricted_date))
+        else:
+            response_type = ExtractWithinRangeSuccess.VALID_IN_RANGE
+            restricted_date = [r]
+
+            response_candidates.append((1, response_type, restricted_date))
+
+    response_candidates_ranked = sorted(response_candidates, key=lambda x: x[0])
+    _, response_type, restricted_date = response_candidates_ranked[0]
+
+    return response_type, restricted_date
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/patterns.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/patterns.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-# multi patters
-R_MULTI = r'(.*)\bvagy\b(.*)|(.*)\bés\b(.*)'
-
-# schemas
-R_TOLIG = r'(.*-?t[oóöő]l\b)(.*-?ig\b)'
-R_TOL = r'([:\w ]*-?t[oóöő]l\b).*'
-R_IG = r'([:\w ]*-?ig\b)'
-
-# hyper day level patterns
-R_ISO_DATE = r'(\b\d{4,4})(?:[-\\/\.](1[0-2]|0?[1-9]))?(?:[-\\/\.](1[0-9]|2[0-9]|3[01]|0?[1-9]))?'
-R_NAMED_MONTH = r'(j[oöő]v[oöő].*?|tavaly.*?)?(\bjan(?:\b|\.|u[aá]r){1}|\bfeb(?:\b|r\.|\.|ru[aá]r){1}|\bm[aá]r(?:\b|c\b|c\.|\.|cius){1}|\b[aá]pr(?:\b|\.|ilis){1}\b|m[aá]j(?:\b|\.|us){1}|\bj[uú]n(?:\b|\.|ius){1}|\bj[uú]l(?:\b|\.|ius){1}|\baug(?:\b|\.|usztus){1}|\bszep(?:t\b|t\.|\b|\.|tember){1}|\bokt(?:\b|\.|[oó]ber){1}|\bnov(?:\b|\.|ember){1}|\bdec(?:\b|\.|ember){1})(?: ([1-3][0-9]|[1-9]))?'
-R_RELATIVE_MONTH = r'(?:(\blegut[oó]bbi|\butols[oó]|\bmúlt|\but[oó]bbi|\bezen|\bebben|\baktu[aá]lis|\bj[oöő]v[oöő]|\bk[oö]vetkez[oőö]|\bk[oö]vetkezend[oőö]).*)? a?h[oó]nap'
-
-R_WEEKDAY = r'(?:(el[oő]z[oő]|m[uú]lt|ezen|j[oöő]v[oöő]).*)?(h[eé]tf[oő]|kedd|szerd[aá]|cs[uü]t[oö]rt[oö]k|p[eé]ntek|szombat|vas[aá]rnap)'
-R_WEEK = r'(el[oő]z[oő] h[eé]t|m[uú]lt h[eé]t|m[uú]lth[eé]t|ezen a? h[eé]t|j[oöő]v[oöő]h[eé]t|j[oöő]v[oöő] h[eé]t)'
-
-R_TODAY = r'\b(má(?:tól|ra))\b|\b(ma)\b|\b(mai nap)\b'
-R_TOMORROW = r'\b(holnap)(?!ut[aá]n)'
-R_NTOMORROW = r'\b(holnaput[aá]n)'
-R_YESTERDAY = r'\b(tegnap)'
-R_NYESTERDAY = r'\b(tegnapel[oő]tt)'
-
-R_NMINS_FROM_NOW = r'(([\w]*) perc m[úu]lva)'
-R_NHOURS_FROM_NOW = r'(([\w]*) [oó]ra m[úu]lva)'
-R_NDAYS_FROM_NOW = r'(([\w]*) nap m[úu]lva)'
-R_NWEEKS_FROM_NOW = r'(([\w]*) h[eé]t m[úu]lva)'
-
-R_NMINS_PRIOR_NOW = r'(([\w]*) percc?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
-R_NHOURS_PRIOR_NOW = r'(([\w]*) [oó]r[aá]val (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
-R_NDAYS_PRIOR_NOW = r'(([\w]*) napp?al (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
-R_NWEEKS_PRIOR_NOW = r'(([\w]*) h[eé]tt?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
-
-R_IN_PAST_PERIOD_MINS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(percben|perc)'
-R_IN_PAST_PERIOD_HOURS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([oó]r[aá]ban|[oó]rai|[oó]ra)'
-R_IN_PAST_PERIOD_DAYS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(napban|napi|nap)'
-R_IN_PAST_PERIOD_WEEKS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[eé]tben|heti|h[eé]t)'
-R_IN_PAST_PERIOD_MONTHS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[oó]napban|havi|h[oó]nap)'
-R_IN_PAST_PERIOD_YEARS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([eé]v|[eé]vben|[eé]vi)'
-
-R_YEAR = r'(tavalyel[oöő]tt|id[eé]n|j[oöő]v[oöő]re|tavaly|.*[eé]v m[uú]lva|.*[eé]vvel ezel[oő]tt|.*[eé]vvel kor[aá]bban)'
-
-# hour level
-R_AT = r'([:\w ]*-?kor)'
-
-# hour+minute parsers
-R_DIGI = r'\b([0-2]?[0-9]):([0-9][0-9])'
-R_HWORDS = r'([0-2][0-9])(?: ?óra|-?kor| ?h) ?(?:([0-9][0-9])(?:(?: ?perc| ?p)[\w]*))? ?(?:([0-9][0-9])(?:(?: ?m[áa]sodperc| ?mp)[\w]*))?'
-R_HWORDS_ = r'([1-2]?[0-9])?h\b'
-R_HOUR_MIN = r'(?:(.*hajnal[i]?|.*reggel|.*d[eé]lel[oőö]tt|.*d[eé]lut[aá]n|.*este|.*[eé]jjel))? ?(?:(.*negyed|.*f[eé]l|.*h[aá]romnegyed))? ?(?:(?:\b([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)?((?:el[oő]tt|ut[aá]n)?.*perc)?)?'
-R_HOUR_MIN_REV = r'(?:(.*)(?:perc.{0,4}))?? (?:(hajnal[i]?|reggel|d[eé]lel[oőö]tt|d[eé]lut[aá]n|este|[eé]jjel))? ?(negyed|f[eé]l|h[aá]romnegyed)? ?(?:([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)? ?(ut[aá]n|el[oöő]tt)?'
-
-# R_MIN = r'(.*)(?:perc)'
-# R_SEC = r'(.*)(?: ?m[áa]sodperc| ?mp)'
+# multi patters
+R_MULTI = r'(.*)\bvagy\b(.*)|(.*)\bés\b(.*)'
+
+# schemas
+R_TOLIG = r'(.*-?t[oóöő]l\b)(.*-?ig\b)'
+R_TOL = r'([:\w ]*-?t[oóöő]l\b).*'
+R_IG = r'([:\w ]*-?ig\b)'
+
+# hyper day level patterns
+R_ISO_DATE = r'(\b\d{4,4})(?:[-\\/\. ](1[0-2]|0?[1-9]))?(?:[-\\/\. ](1[0-9]|2[0-9]|3[01]|0?[1-9]))?'
+R_REV_ISO_DATE = r'\b(1[0-9]|2[0-9]|3[01]|0?[1-9])[-\\/\. ](1[0-2]|0?[1-9])[-\\/\. ](\b\d{4,4})'
+R_NAMED_MONTH = r'(j[oöő]v[oöő].*?|tavaly.*?)?(\bjan(?:\b|\.|u[aá]r){1}|\bfeb(?:\b|r\.|\.|ru[aá]r){1}|\bm[aá]r(?:\b|c\b|c\.|\.|cius){1}|\b[aá]pr(?:\b|\.|ilis){1}\b|m[aá]j(?:\b|\.|us){1}|\bj[uú]n(?:\b|\.|ius){1}|\bj[uú]l(?:\b|\.|ius){1}|\baug(?:\b|\.|usztus){1}|\bszep(?:t\b|t\.|\b|\.|tember){1}|\bokt(?:\b|\.|[oó]ber){1}|\bnov(?:\b|\.|ember){1}|\bdec(?:\b|\.|ember){1})(?: ([1-3][0-9]|[1-9]))?'
+R_RELATIVE_MONTH = r'(?:(\blegut[oó]bbi|\butols[oó]|\bmúlt|\but[oó]bbi|\bezen|\bebben|\baktu[aá]lis|\bj[oöő]v[oöő]|\bk[oö]vetkez[oőö]|\bk[oö]vetkezend[oőö]).*)? a?h[oó]nap'
+
+R_WEEKDAY = r'(?:(el[oő]z[oő]|m[uú]lt|ezen|j[oöő]v[oöő]).*)?(h[eé]tf[oő]|kedd|szerd[aá]|cs[uü]t[oö]rt[oö]k|p[eé]ntek|szombat|vas[aá]rnap)'
+R_WEEK = r'(el[oő]z[oő] h[eé]t|m[uú]lt h[eé]t|m[uú]lth[eé]t|ezen a? h[eé]t|j[oöő]v[oöő]h[eé]t|j[oöő]v[oöő] h[eé]t)'
+
+R_TODAY = r'\b(má(?:tól|ra))\b|\b(ma)\b|\b(mai nap)\b'
+R_TOMORROW = r'\b(holnap)(?!ut[aá]n)'
+R_NTOMORROW = r'\b(holnaput[aá]n)'
+R_YESTERDAY = r'\b(tegnap)'
+R_NYESTERDAY = r'\b(tegnapel[oő]tt)'
+
+R_NMINS_FROM_NOW = r'(([\w]*) perc m[úu]lva)'
+R_NHOURS_FROM_NOW = r'(([\w]*) [oó]ra m[úu]lva)'
+R_NDAYS_FROM_NOW = r'(([\w]*) nap m[úu]lva)'
+R_NWEEKS_FROM_NOW = r'(([\w]*) h[eé]t m[úu]lva)'
+
+R_NMINS_PRIOR_NOW = r'(([\w]*) percc?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NHOURS_PRIOR_NOW = r'(([\w]*) [oó]r[aá]val (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NDAYS_PRIOR_NOW = r'(([\w]*) napp?al (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NWEEKS_PRIOR_NOW = r'(([\w]*) h[eé]tt?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+
+R_IN_PAST_PERIOD_MINS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(percben|perc)'
+R_IN_PAST_PERIOD_HOURS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([oó]r[aá]ban|[oó]rai|[oó]ra)'
+R_IN_PAST_PERIOD_DAYS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(napban|napi|nap)'
+R_IN_PAST_PERIOD_WEEKS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[eé]tben|heti|h[eé]t)'
+R_IN_PAST_PERIOD_MONTHS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[oó]napban|havi|h[oó]nap)'
+R_IN_PAST_PERIOD_YEARS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([eé]v|[eé]vben|[eé]vi)'
+
+R_YEAR = r'(tavalyel[oöő]tt|id[eé]n|j[oöő]v[oöő]re|tavaly|.*[eé]v m[uú]lva|.*[eé]vvel ezel[oő]tt|.*[eé]vvel kor[aá]bban)'
+
+# hour level
+R_AT = r'([:\w ]*-?kor)'
+
+# hour+minute parsers
+R_DIGI = r'\b([0-2]?[0-9]):([0-9][0-9])'
+R_HWORDS = r'([0-2][0-9])(?: ?óra|-?kor| ?h) ?(?:([0-9][0-9])(?:(?: ?perc| ?p)[\w]*))? ?(?:([0-9][0-9])(?:(?: ?m[áa]sodperc| ?mp)[\w]*))?'
+R_HWORDS_ = r'([1-2]?[0-9])?h\b'
+R_HOUR_MIN = r'(?:(.*hajnal[i]?|.*reggel|.*d[eé]lel[oőö]tt|.*d[eé]lut[aá]n|.*este|.*[eé]jjel))? ?(?:(.*negyed|.*f[eé]l|.*h[aá]romnegyed))? ?(?:(?:\b([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)?((?:el[oő]tt|ut[aá]n)?.*perc)?)?'
+R_HOUR_MIN_REV = r'(?:(.*)(?:perc.{0,4}))?? (?:(hajnal[i]?|reggel|d[eé]lel[oőö]tt|d[eé]lut[aá]n|este|[eé]jjel))? ?(negyed|f[eé]l|h[aá]romnegyed)? ?(?:([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)? ?(ut[aá]n|el[oöő]tt)?'
+
+# R_MIN = r'(.*)(?:perc)'
+# R_SEC = r'(.*)(?: ?m[áa]sodperc| ?mp)'
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/structure_parsers.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_parser/time_parsers.py` & `hun-date-parser-0.2.1/hun_date_parser/date_parser/time_parsers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-import re
-
-from typing import Dict, List, Any, Tuple, Optional
-from datetime import datetime
-
-from hun_date_parser.date_parser.patterns import R_DIGI, R_HOUR_MIN, R_HOUR_MIN_REV, R_HWORDS_
-from hun_date_parser.utils import remove_accent, word_to_num, Year, Month, Day, Hour, Minute, Daypart
-from hun_date_parser.date_parser.date_parsers import match_weekday
-
-NAN = -1
-
-
-def match_digi_clock(s: str) -> List[Dict[str, Any]]:
-    """
-    Match digi clock format.
-    :param s: textual input
-    :return: tuple of date parts
-    """
-    match = re.findall(R_DIGI, s)
-
-    res = []
-    for group in match:
-        group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
-
-        if len(group) == 2:
-            h, m = group
-            res.append({'match': group, 'date_parts': [Hour(h, 'digi_clock'), Minute(m, 'digi_clock')]})
-        elif len(group) == 1:
-            res.append({'match': group, 'date_parts': [Hour(group[0], 'digi_clock')]})
-
-    return res
-
-
-def match_hwords(s: str) -> List[Dict[str, Any]]:
-    group = re.findall(R_HWORDS_, s)
-    group = [m for m in group if ''.join(m)]
-
-    res = []
-    for match in group:
-        match = int(match)
-        res.append({'match': match, 'date_parts': [Hour(match, 'hwords')]})
-
-    return res
-
-
-def is_indeed_hour(s: str):
-    s_uac = remove_accent(s)
-
-    words_indicating_hour = [
-        "ora",
-        "-kor",
-        "egykor",
-        "kettokor",
-        "haromkor",
-        "negykor",
-        "otkor",
-        "hatkor",
-        "hetkor",
-        "nyolckor",
-        "kilenckor",
-        "tizkor",
-        "tizenegykor",
-        "tizenkettokor"
-    ]
-
-    for w in words_indicating_hour:
-        if w in s_uac:
-            return True
-
-    return False
-
-
-def _raw_match_time_words(s: str) -> Optional[Tuple[Any, Any, Any, Any, Any]]:
-    """
-    Extracts date and time particles from text
-    :param s: input text
-    :return:
-    """
-    group = re.findall(R_HOUR_MIN, s)
-    group = [m for m in group if ''.join(m)]
-
-    group_rev = re.findall(R_HOUR_MIN_REV, s)
-    group_rev = [m for m in group_rev if ''.join(m)]
-
-    if not (group or group_rev):
-        return None
-    elif group and not group_rev:
-        daypart, hour_modifier, hour, minute = group[0]
-    elif not group and group_rev:
-        minute, daypart, hour_modifier, hour, is_before = group_rev[0]
-        minute += (' ' + is_before)
-    elif group_rev[0].count('') < group[0].count(''):
-        minute, daypart, hour_modifier, hour, is_before = group_rev[0]
-        minute += (' ' + is_before)
-    else:
-        daypart, hour_modifier, hour, minute = group[0]
-
-    # when a single number is matched, the pattern currently interprets it as an hour value
-    # i.e.: "1" --> 1 hour or "egy" --> 1 hour
-    # this check is designed to address this issue (R_HOUR_MIN pattern needs to be rewritten for a proper solution)
-    if not (daypart or minute or hour_modifier) and hour and not is_indeed_hour(s):
-        return [('', '', '', '')], '', '', '', ''
-
-    return group, daypart, hour_modifier, hour, minute
-
-
-def match_time_words(s: str) -> List[Dict[str, Any]]:
-    """
-    :param s: textual input
-    :return: tuple of date parts
-    """
-    parts = _raw_match_time_words(s)
-    if not parts:
-        return []
-    else:
-        group, daypart, hour_modifier, hour, minute = parts
-
-    # Only numbers can match dates as well, this is an attempt to remove false matches
-    hour_index = s.index(f'{hour}')
-    before_hour = s[:hour_index].split()
-    if before_hour:
-        months = ['jan', 'feb', 'mar', 'apr', 'maj', 'jun', 'jul', 'aug', 'szep', 'okt', 'nov', 'dec']
-        for month in months:
-            if month in remove_accent(before_hour[-1]):
-                return []
-
-    # Fix false time match for input 'jövő hét'
-    if remove_accent(hour) == 'het':
-        hour_indeces = [m.start() for m in re.finditer('het(?!fo)', remove_accent(s))]
-        if hour_indeces:
-            before_hour = s[:hour_indeces[-1]].split()
-            if before_hour:
-                if 'jovo' in remove_accent(before_hour[-1]):
-                    return []
-
-    res = []
-    am = True
-    date_parts = []
-
-    if daypart and hour:
-        if 'reggel' in daypart or 'delelott' in remove_accent(daypart) or 'hajnal' in daypart:
-            am = True
-        elif 'delutan' in remove_accent(daypart) or 'este' in daypart or 'ejjel' in remove_accent(daypart):
-            am = False
-
-    if hour:
-
-        # SKIP the whole matching rule when any of these apply
-        # TODO: come up with a more elegant solution for this
-        # TODO: i.e: by implementing the possibility of one rule exclude another
-        # this is made redundant by the change in the patterns
-        non_hours = ['ev', 'perc']
-        for nh in non_hours:
-            if f' {nh}' in remove_accent(hour) or remove_accent(hour).startswith(nh):
-                return []
-
-        if 'mulva' in remove_accent(s):
-            return []
-
-        hour_num = word_to_num(hour)
-        minute_num = word_to_num(minute)
-
-        if not daypart:
-            # default to business hour if daypart is not specified
-            if hour_num < 8:
-                hour_num += 12
-
-        if hour_modifier:
-            if 'haromnegyed' in remove_accent(hour_modifier):
-                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
-                minute_num = 45
-            elif 'fel' in remove_accent(hour_modifier):
-                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
-                minute_num = 30
-            elif 'negyed' in remove_accent(hour_modifier):
-                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
-                minute_num = 15
-
-        if hour_num == NAN:
-            return []
-        else:
-            if hour_num < 12 and not am:
-                hour_num += 12
-
-        if minute or hour_modifier:
-            # this is made redundant by the change in the patterns
-            non_minutes = ['ev', 'ora']
-            for nm in non_minutes:
-                if f' {nm}' in remove_accent(minute) or remove_accent(minute).startswith(nm):
-                    return []
-
-            if 'elott' in remove_accent(minute) and not hour_modifier:
-                hour_num -= (minute_num // 60) + 1
-                hour_num = hour_num if hour_num >= 0 else 23
-                date_parts.extend([Hour(hour_num, 'time_words'), Minute(60 - (minute_num % 60), 'time_words')])
-            elif 'elott' in remove_accent(minute) and hour_modifier:
-                n_minutes_before = word_to_num(minute)
-                if n_minutes_before != NAN:
-                    minute_num -= n_minutes_before
-                if minute_num < 0:
-                    hour_num += (minute_num // 60)
-                    hour_num = hour_num if hour_num >= 0 else 23
-                    minute_num = minute_num % 60
-                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
-            elif hour_modifier:
-                n_minutes_after = word_to_num(minute)
-                if n_minutes_after != NAN:
-                    minute_num += n_minutes_after
-                if minute_num > 59:
-                    hour_num += (minute_num // 60)
-                    hour_num = hour_num if hour_num <= 23 else 0
-                    minute_num = minute_num % 60
-                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
-            else:
-                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
-
-        else:
-            date_parts.append(Hour(hour_num, 'time_words'))
-
-        res.append({'match': group, 'date_parts': date_parts})
-
-    elif daypart:
-        if 'hajnal' in daypart:
-            res.append({'match': group, 'date_parts': [Daypart(0, 'time_words')]})
-        elif 'reggel' in daypart:
-            res.append({'match': group, 'date_parts': [Daypart(1, 'time_words')]})
-        elif 'delelott' in remove_accent(daypart):
-            res.append({'match': group, 'date_parts': [Daypart(2, 'time_words')]})
-        elif 'delutan' in remove_accent(daypart):
-            res.append({'match': group, 'date_parts': [Daypart(3, 'time_words')]})
-        elif 'este' in daypart:
-            res.append({'match': group, 'date_parts': [Daypart(4, 'time_words')]})
-        elif 'ejjel' in remove_accent(daypart):
-            res.append({'match': group, 'date_parts': [Daypart(5, 'time_words')]})
-
-    return res
-
-
-def match_now(s: str, now: datetime) -> List[Dict[str, Any]]:
-    if match_weekday(s, now):
-        return []
-
-    match = re.match(r'.*\bmost\b.*', s.lower())
-    if match:
-        date_parts = [Year(now.year, 'now'), Month(now.month, 'now'), Day(now.day, 'now'), Hour(now.hour, 'now'),
-                      Minute(now.minute, 'now')]
-        return [{'match': 'most', 'date_parts': date_parts}]
-
-    return []
+import re
+
+from typing import Dict, List, Any, Tuple, Optional
+from datetime import datetime
+
+from hun_date_parser.date_parser.patterns import R_DIGI, R_HOUR_MIN, R_HOUR_MIN_REV, R_HWORDS_
+from hun_date_parser.utils import remove_accent, word_to_num, Year, Month, Day, Hour, Minute, Daypart
+from hun_date_parser.date_parser.date_parsers import match_weekday
+
+NAN = -1
+
+
+def match_digi_clock(s: str) -> List[Dict[str, Any]]:
+    """
+    Match digi clock format.
+    :param s: textual input
+    :return: tuple of date parts
+    """
+    match = re.findall(R_DIGI, s)
+
+    res = []
+    for group in match:
+        group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
+
+        if len(group) == 2:
+            h, m = group
+            res.append({'match': group, 'date_parts': [Hour(h, 'digi_clock'), Minute(m, 'digi_clock')]})
+        elif len(group) == 1:
+            res.append({'match': group, 'date_parts': [Hour(group[0], 'digi_clock')]})
+
+    return res
+
+
+def match_hwords(s: str) -> List[Dict[str, Any]]:
+    group = re.findall(R_HWORDS_, s)
+    group = [m for m in group if ''.join(m)]
+
+    res = []
+    for match in group:
+        match = int(match)
+        res.append({'match': match, 'date_parts': [Hour(match, 'hwords')]})
+
+    return res
+
+
+def is_indeed_hour(s: str):
+    s_uac = remove_accent(s)
+
+    words_indicating_hour = [
+        "ora",
+        "-kor",
+        "egykor",
+        "kettokor",
+        "haromkor",
+        "negykor",
+        "otkor",
+        "hatkor",
+        "hetkor",
+        "nyolckor",
+        "kilenckor",
+        "tizkor",
+        "tizenegykor",
+        "tizenkettokor"
+    ]
+
+    for w in words_indicating_hour:
+        if w in s_uac:
+            return True
+
+    return False
+
+
+def _raw_match_time_words(s: str) -> Optional[Tuple[Any, Any, Any, Any, Any]]:
+    """
+    Extracts date and time particles from text
+    :param s: input text
+    :return:
+    """
+    group = re.findall(R_HOUR_MIN, s)
+    group = [m for m in group if ''.join(m)]
+
+    group_rev = re.findall(R_HOUR_MIN_REV, s)
+    group_rev = [m for m in group_rev if ''.join(m)]
+
+    if not (group or group_rev):
+        return None
+    elif group and not group_rev:
+        daypart, hour_modifier, hour, minute = group[0]
+    elif not group and group_rev:
+        minute, daypart, hour_modifier, hour, is_before = group_rev[0]
+        minute += (' ' + is_before)
+    elif group_rev[0].count('') < group[0].count(''):
+        minute, daypart, hour_modifier, hour, is_before = group_rev[0]
+        minute += (' ' + is_before)
+    else:
+        daypart, hour_modifier, hour, minute = group[0]
+
+    # when a single number is matched, the pattern currently interprets it as an hour value
+    # i.e.: "1" --> 1 hour or "egy" --> 1 hour
+    # this check is designed to address this issue (R_HOUR_MIN pattern needs to be rewritten for a proper solution)
+    if not (daypart or minute or hour_modifier) and hour and not is_indeed_hour(s):
+        return [('', '', '', '')], '', '', '', ''
+
+    return group, daypart, hour_modifier, hour, minute
+
+
+def match_time_words(s: str) -> List[Dict[str, Any]]:
+    """
+    :param s: textual input
+    :return: tuple of date parts
+    """
+    parts = _raw_match_time_words(s)
+    if not parts:
+        return []
+    else:
+        group, daypart, hour_modifier, hour, minute = parts
+
+    # Only numbers can match dates as well, this is an attempt to remove false matches
+    hour_index = s.index(f'{hour}')
+    before_hour = s[:hour_index].split()
+    if before_hour:
+        months = ['jan', 'feb', 'mar', 'apr', 'maj', 'jun', 'jul', 'aug', 'szep', 'okt', 'nov', 'dec']
+        for month in months:
+            if month in remove_accent(before_hour[-1]):
+                return []
+
+    # Fix false time match for input 'jövő hét'
+    if remove_accent(hour) == 'het':
+        hour_indeces = [m.start() for m in re.finditer('het(?!fo)', remove_accent(s))]
+        if hour_indeces:
+            before_hour = s[:hour_indeces[-1]].split()
+            if before_hour:
+                if 'jovo' in remove_accent(before_hour[-1]):
+                    return []
+
+    res = []
+    am = True
+    date_parts = []
+
+    if daypart and hour:
+        if 'reggel' in daypart or 'delelott' in remove_accent(daypart) or 'hajnal' in daypart:
+            am = True
+        elif 'delutan' in remove_accent(daypart) or 'este' in daypart or 'ejjel' in remove_accent(daypart):
+            am = False
+
+    if hour:
+
+        # SKIP the whole matching rule when any of these apply
+        # TODO: come up with a more elegant solution for this
+        # TODO: i.e: by implementing the possibility of one rule exclude another
+        # this is made redundant by the change in the patterns
+        non_hours = ['ev', 'perc']
+        for nh in non_hours:
+            if f' {nh}' in remove_accent(hour) or remove_accent(hour).startswith(nh):
+                return []
+
+        if 'mulva' in remove_accent(s):
+            return []
+
+        hour_num = word_to_num(hour)
+        minute_num = word_to_num(minute)
+
+        if not daypart:
+            # default to business hour if daypart is not specified
+            if hour_num < 8:
+                hour_num += 12
+
+        if hour_modifier:
+            if 'haromnegyed' in remove_accent(hour_modifier):
+                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
+                minute_num = 45
+            elif 'fel' in remove_accent(hour_modifier):
+                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
+                minute_num = 30
+            elif 'negyed' in remove_accent(hour_modifier):
+                hour_num = hour_num - 1 if hour_num - 1 >= 0 else 23
+                minute_num = 15
+
+        if hour_num == NAN:
+            return []
+        else:
+            if hour_num < 12 and not am:
+                hour_num += 12
+
+        if minute or hour_modifier:
+            # this is made redundant by the change in the patterns
+            non_minutes = ['ev', 'ora']
+            for nm in non_minutes:
+                if f' {nm}' in remove_accent(minute) or remove_accent(minute).startswith(nm):
+                    return []
+
+            if 'elott' in remove_accent(minute) and not hour_modifier:
+                hour_num -= (minute_num // 60) + 1
+                hour_num = hour_num if hour_num >= 0 else 23
+                date_parts.extend([Hour(hour_num, 'time_words'), Minute(60 - (minute_num % 60), 'time_words')])
+            elif 'elott' in remove_accent(minute) and hour_modifier:
+                n_minutes_before = word_to_num(minute)
+                if n_minutes_before != NAN:
+                    minute_num -= n_minutes_before
+                if minute_num < 0:
+                    hour_num += (minute_num // 60)
+                    hour_num = hour_num if hour_num >= 0 else 23
+                    minute_num = minute_num % 60
+                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
+            elif hour_modifier:
+                n_minutes_after = word_to_num(minute)
+                if n_minutes_after != NAN:
+                    minute_num += n_minutes_after
+                if minute_num > 59:
+                    hour_num += (minute_num // 60)
+                    hour_num = hour_num if hour_num <= 23 else 0
+                    minute_num = minute_num % 60
+                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
+            else:
+                date_parts.extend([Hour(hour_num, 'time_words'), Minute(minute_num, 'time_words')])
+
+        else:
+            date_parts.append(Hour(hour_num, 'time_words'))
+
+        res.append({'match': group, 'date_parts': date_parts})
+
+    elif daypart:
+        if 'hajnal' in daypart:
+            res.append({'match': group, 'date_parts': [Daypart(0, 'time_words')]})
+        elif 'reggel' in daypart:
+            res.append({'match': group, 'date_parts': [Daypart(1, 'time_words')]})
+        elif 'delelott' in remove_accent(daypart):
+            res.append({'match': group, 'date_parts': [Daypart(2, 'time_words')]})
+        elif 'delutan' in remove_accent(daypart):
+            res.append({'match': group, 'date_parts': [Daypart(3, 'time_words')]})
+        elif 'este' in daypart:
+            res.append({'match': group, 'date_parts': [Daypart(4, 'time_words')]})
+        elif 'ejjel' in remove_accent(daypart):
+            res.append({'match': group, 'date_parts': [Daypart(5, 'time_words')]})
+
+    return res
+
+
+def match_now(s: str, now: datetime) -> List[Dict[str, Any]]:
+    if match_weekday(s, now):
+        return []
+
+    match = re.match(r'.*\bmost\b.*', s.lower())
+    if match:
+        date_parts = [Year(now.year, 'now'), Month(now.month, 'now'), Day(now.day, 'now'), Hour(now.hour, 'now'),
+                      Minute(now.minute, 'now')]
+        return [{'match': 'most', 'date_parts': date_parts}]
+
+    return []
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/date2text.py` & `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/date2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/datetime_textualizer.py` & `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/datetime_textualizer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""This module handles turning datetime instances into Hungarian text."""
-
-from datetime import datetime
-from typing import Dict
-
-from hun_date_parser.date_textualizer.date2text import date2text, date2full_text
-from hun_date_parser.date_textualizer.time2text import time2absolutetexttime, time2digi, time2relitivetexttime, \
-    time2lifelike
-
-
-def datetime2text(input_datetime: datetime, time_precision: int = 3, now: datetime = datetime.now()):
-    """
-    Returns date and time textual representation candidates for input datetime object.
-    :param input_datetime: Input datetime object.
-    :param time_precision: Display only hours, minutes, seconds (corresponding to 1, 2, 3)
-    :param now: Current timestamp to calculate relative dates.
-    :return: Dictionary with the results
-    """
-    datetime_textualizer = DatetimeTextualizer(now=now)
-    return datetime_textualizer.generate_candidates(input_datetime=input_datetime, time_precision=time_precision)
-
-
-class DatetimeTextualizer:
-    """
-    This class handles turning datetime instances into Hungarian text.
-    """
-
-    def __init__(self, now: datetime = datetime.now()):
-        """
-        :param now: Current timestamp to calculate relative dates.
-        """
-        self.now = now
-
-    def generate_candidates(self, input_datetime: datetime, time_precision: int = 3) -> Dict:
-        """
-        Generates date and time textual representation candidates for input datetime object.
-        :param input_datetime: Input datetime object.
-        :param time_precision: Display only hours, minutes, seconds (corresponding to 1, 2, 3)
-        :return: Dictionary with the results
-        """
-        dates = [date2text(input_datetime.date(), self.now.date()),
-                 date2full_text(input_datetime.date())]
-        times = [time2absolutetexttime(input_datetime.time(), time_precision),
-                 time2digi(input_datetime.time(), time_precision),
-                 time2relitivetexttime(input_datetime.time(), time_precision),
-                 time2lifelike(input_datetime.time(), time_precision)]
-
-        return {
-            "dates": dates,
-            "times": times
-        }
+"""This module handles turning datetime instances into Hungarian text."""
+
+from datetime import datetime
+from typing import Dict
+
+from hun_date_parser.date_textualizer.date2text import date2text, date2full_text
+from hun_date_parser.date_textualizer.time2text import time2absolutetexttime, time2digi, time2relitivetexttime, \
+    time2lifelike
+
+
+def datetime2text(input_datetime: datetime, time_precision: int = 3, now: datetime = datetime.now()):
+    """
+    Returns date and time textual representation candidates for input datetime object.
+    :param input_datetime: Input datetime object.
+    :param time_precision: Display only hours, minutes, seconds (corresponding to 1, 2, 3)
+    :param now: Current timestamp to calculate relative dates.
+    :return: Dictionary with the results
+    """
+    datetime_textualizer = DatetimeTextualizer(now=now)
+    return datetime_textualizer.generate_candidates(input_datetime=input_datetime, time_precision=time_precision)
+
+
+class DatetimeTextualizer:
+    """
+    This class handles turning datetime instances into Hungarian text.
+    """
+
+    def __init__(self, now: datetime = datetime.now()):
+        """
+        :param now: Current timestamp to calculate relative dates.
+        """
+        self.now = now
+
+    def generate_candidates(self, input_datetime: datetime, time_precision: int = 3) -> Dict:
+        """
+        Generates date and time textual representation candidates for input datetime object.
+        :param input_datetime: Input datetime object.
+        :param time_precision: Display only hours, minutes, seconds (corresponding to 1, 2, 3)
+        :return: Dictionary with the results
+        """
+        dates = [date2text(input_datetime.date(), self.now.date()),
+                 date2full_text(input_datetime.date())]
+        times = [time2absolutetexttime(input_datetime.time(), time_precision),
+                 time2digi(input_datetime.time(), time_precision),
+                 time2relitivetexttime(input_datetime.time(), time_precision),
+                 time2lifelike(input_datetime.time(), time_precision)]
+
+        return {
+            "dates": dates,
+            "times": times
+        }
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/time2text.py` & `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/time2text.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from datetime import time
-
-from hun_date_parser.utils import num_to_word
-
-hours_word = {
-    0: 'nulla',
-    1: 'hajnali egy',
-    2: 'hajnali kettő',
-    3: 'hajnali három',
-    4: 'hajnali négy',
-    5: 'hajnali öt',
-    6: 'reggel hat',
-    7: 'reggel hét',
-    8: 'reggel nyolc',
-    9: 'reggel kilenc',
-    10: 'délelőtt tíz',
-    11: 'délelőtt tizenegy',
-    12: 'tizenkét',
-    13: 'délután egy',
-    14: 'délután kettő',
-    15: 'délután három',
-    16: 'délután négy',
-    17: 'délután öt',
-    18: 'este hat',
-    19: 'este hét',
-    20: 'este nyolc',
-    21: 'este kilenc',
-    22: 'este tíz',
-    23: 'este tizenegy',
-}
-
-dayparts = {
-    0: 'éjjel',
-    3: 'hajnal',
-    6: 'reggel',
-    10: 'délelőtt',
-    12: 'délután',
-    18: 'este',
-    22: 'éjjel',
-    24: 'éjjel'
-}
-
-
-def get_daypart(h: int):
-    if h == 12:
-        return ''
-    for i, (k, v) in enumerate(dayparts.items()):
-        if k <= h <= list(dayparts)[i+1]:
-            return v
-
-
-def time2relitivetexttime(t: time, resolution: int):
-    assert 1 <= resolution <= 3
-
-    if resolution >= 1:
-        hour = t.hour
-        hour_rep = hours_word[hour]
-
-    if resolution >= 2:
-        minute = t.minute
-        minute_res = num_to_word(minute)
-
-    if resolution >= 3:
-        second = t.second
-        second_res = num_to_word(second)
-
-    if resolution == 1:
-        if hour == 0:
-            return 'éjfél'
-        elif hour == 12:
-            return 'dél'
-        else:
-            return f"{hour_rep} óra"
-    elif resolution == 2:
-        return f"{hour_rep} óra {minute_res} perc"
-    elif resolution == 3:
-        return f"{hour_rep} óra {minute_res} perc {second_res} másodperc"
-
-
-def time2absolutetexttime(t: time, resolution: int):
-    assert 1 <= resolution <= 3
-
-    if resolution >= 1:
-        hour = t.hour
-        hour_rep = num_to_word(hour)
-
-    if resolution >= 2:
-        minute = t.minute
-        minute_res = num_to_word(minute)
-
-    if resolution >= 3:
-        second = t.second
-        second_res = num_to_word(second)
-
-    if resolution == 1:
-        return f"{hour_rep} óra"
-    elif resolution == 2:
-        return f"{hour_rep} óra {minute_res} perc"
-    elif resolution == 3:
-        return f"{hour_rep} óra {minute_res} perc {second_res} másodperc"
-
-
-def time2digi(t: time, resolution: int):
-    assert 1 <= resolution <= 3
-
-    if resolution == 1:
-        return f'{t.hour}'
-    if resolution == 2:
-        return f'{str(t.hour).zfill(2)}:{str(t.minute).zfill(2)}'
-    if resolution == 3:
-        return f'{str(t.hour).zfill(2)}:{str(t.minute).zfill(2)}:{str(t.second).zfill(2)}'
-
-
-def time2lifelike(t: time, resolution: int = 2):
-
-    if resolution == 1:
-        t = time(t.hour, 0)
-
-    def get_h_rep(h):
-        if h % 12 != 0:
-            return h % 12
-        else:
-            return 12
-
-    h, m = t.hour, t.minute
-
-    h_ = h + 1 if h <= 23 else 0
-
-    if m == 0:
-        return f'{get_daypart(h)} {get_h_rep(h)} óra'.lstrip()
-    elif 0 < m < 10:
-        return f'{get_daypart(h)} {get_h_rep(h)} óra után {m} perccel'.lstrip()
-    elif 10 <= m < 15:
-        return f'{get_daypart(h_)} negyed {get_h_rep(h_)} előtt {15 - m} perccel'.lstrip()
-    elif m == 15:
-        return f'{get_daypart(h_)} negyed {get_h_rep(h_)}'.lstrip()
-    elif 15 < m <= 20:
-        return f'{get_daypart(h_)} negyed {get_h_rep(h_)} után {m - 15} perccel'.lstrip()
-    elif 20 < m < 30:
-        return f'{get_daypart(h_)} fél {get_h_rep(h_)} előtt {30 - m} perccel'.lstrip()
-    elif m == 30:
-        return f'{get_daypart(h_)} fél {get_h_rep(h_)}'.lstrip()
-    elif 30 < m <= 40:
-        return f'{get_daypart(h_)} fél {get_h_rep(h_)} után {m - 30} perccel'.lstrip()
-    elif 40 < m < 45:
-        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)} előtt {45 - m} perccel'.lstrip()
-    elif m == 45:
-        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)}'.lstrip()
-    elif 45 < m <= 50:
-        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)} után {m - 45} perccel'.lstrip()
-    elif 50 < m:
-        return f'{get_daypart(h_)} {get_h_rep(h_)} óra előtt {60 - m} perccel'.lstrip()
-    else:
-        return ''
+from datetime import time
+
+from hun_date_parser.utils import num_to_word
+
+hours_word = {
+    0: 'nulla',
+    1: 'hajnali egy',
+    2: 'hajnali kettő',
+    3: 'hajnali három',
+    4: 'hajnali négy',
+    5: 'hajnali öt',
+    6: 'reggel hat',
+    7: 'reggel hét',
+    8: 'reggel nyolc',
+    9: 'reggel kilenc',
+    10: 'délelőtt tíz',
+    11: 'délelőtt tizenegy',
+    12: 'tizenkét',
+    13: 'délután egy',
+    14: 'délután kettő',
+    15: 'délután három',
+    16: 'délután négy',
+    17: 'délután öt',
+    18: 'este hat',
+    19: 'este hét',
+    20: 'este nyolc',
+    21: 'este kilenc',
+    22: 'este tíz',
+    23: 'este tizenegy',
+}
+
+dayparts = {
+    0: 'éjjel',
+    3: 'hajnal',
+    6: 'reggel',
+    10: 'délelőtt',
+    12: 'délután',
+    18: 'este',
+    22: 'éjjel',
+    24: 'éjjel'
+}
+
+
+def get_daypart(h: int):
+    if h == 12:
+        return ''
+    for i, (k, v) in enumerate(dayparts.items()):
+        if k <= h <= list(dayparts)[i+1]:
+            return v
+
+
+def time2relitivetexttime(t: time, resolution: int):
+    assert 1 <= resolution <= 3
+
+    if resolution >= 1:
+        hour = t.hour
+        hour_rep = hours_word[hour]
+
+    if resolution >= 2:
+        minute = t.minute
+        minute_res = num_to_word(minute)
+
+    if resolution >= 3:
+        second = t.second
+        second_res = num_to_word(second)
+
+    if resolution == 1:
+        if hour == 0:
+            return 'éjfél'
+        elif hour == 12:
+            return 'dél'
+        else:
+            return f"{hour_rep} óra"
+    elif resolution == 2:
+        return f"{hour_rep} óra {minute_res} perc"
+    elif resolution == 3:
+        return f"{hour_rep} óra {minute_res} perc {second_res} másodperc"
+
+
+def time2absolutetexttime(t: time, resolution: int):
+    assert 1 <= resolution <= 3
+
+    if resolution >= 1:
+        hour = t.hour
+        hour_rep = num_to_word(hour)
+
+    if resolution >= 2:
+        minute = t.minute
+        minute_res = num_to_word(minute)
+
+    if resolution >= 3:
+        second = t.second
+        second_res = num_to_word(second)
+
+    if resolution == 1:
+        return f"{hour_rep} óra"
+    elif resolution == 2:
+        return f"{hour_rep} óra {minute_res} perc"
+    elif resolution == 3:
+        return f"{hour_rep} óra {minute_res} perc {second_res} másodperc"
+
+
+def time2digi(t: time, resolution: int):
+    assert 1 <= resolution <= 3
+
+    if resolution == 1:
+        return f'{t.hour}'
+    if resolution == 2:
+        return f'{str(t.hour).zfill(2)}:{str(t.minute).zfill(2)}'
+    if resolution == 3:
+        return f'{str(t.hour).zfill(2)}:{str(t.minute).zfill(2)}:{str(t.second).zfill(2)}'
+
+
+def time2lifelike(t: time, resolution: int = 2):
+
+    if resolution == 1:
+        t = time(t.hour, 0)
+
+    def get_h_rep(h):
+        if h % 12 != 0:
+            return h % 12
+        else:
+            return 12
+
+    h, m = t.hour, t.minute
+
+    h_ = h + 1 if h <= 23 else 0
+
+    if m == 0:
+        return f'{get_daypart(h)} {get_h_rep(h)} óra'.lstrip()
+    elif 0 < m < 10:
+        return f'{get_daypart(h)} {get_h_rep(h)} óra után {m} perccel'.lstrip()
+    elif 10 <= m < 15:
+        return f'{get_daypart(h_)} negyed {get_h_rep(h_)} előtt {15 - m} perccel'.lstrip()
+    elif m == 15:
+        return f'{get_daypart(h_)} negyed {get_h_rep(h_)}'.lstrip()
+    elif 15 < m <= 20:
+        return f'{get_daypart(h_)} negyed {get_h_rep(h_)} után {m - 15} perccel'.lstrip()
+    elif 20 < m < 30:
+        return f'{get_daypart(h_)} fél {get_h_rep(h_)} előtt {30 - m} perccel'.lstrip()
+    elif m == 30:
+        return f'{get_daypart(h_)} fél {get_h_rep(h_)}'.lstrip()
+    elif 30 < m <= 40:
+        return f'{get_daypart(h_)} fél {get_h_rep(h_)} után {m - 30} perccel'.lstrip()
+    elif 40 < m < 45:
+        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)} előtt {45 - m} perccel'.lstrip()
+    elif m == 45:
+        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)}'.lstrip()
+    elif 45 < m <= 50:
+        return f'{get_daypart(h_)} háromnegyed {get_h_rep(h_)} után {m - 45} perccel'.lstrip()
+    elif 50 < m:
+        return f'{get_daypart(h_)} {get_h_rep(h_)} óra előtt {60 - m} perccel'.lstrip()
+    else:
+        return ''
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser.egg-info/PKG-INFO` & `hun-date-parser-0.2.1/hun_date_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">Hungarian Date Parser</h1>
         
@@ -69,16 +69,16 @@
         An example:
         ```python
         from hun_date_parser import text2datetime
         from datetime import datetime
         from hun_date_parser.utils import SearchScopes
         
         text2datetime('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-        # [{'start_date': datetime.datetime(2023, 8, 1, 0, 0),
-        #   'end_date': datetime.datetime(2023, 8, 31, 23, 59, 59)}]
+        # [{'start_date': datetime.datetime(2022, 8, 1, 0, 0),
+        #   'end_date': datetime.datetime(2022, 8, 31, 23, 59, 59)}]
         
         text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
         # [{'start_date': datetime.datetime(2023, 6, 2, 0, 0),
         #   'end_date': datetime.datetime(2023, 6, 2, 23, 59, 59)}]
         
         text2datetime('péntek', now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED)
         # [{'start_date': datetime.datetime(2023, 6, 9, 0, 0),
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.0 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.1 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com License:
 UNKNOWN Description:
                       ****** Hungarian Date Parser ******
  A tool for extracting datetime intervals from Hungarian sentences and turning
                      datetime objects into Hungarian text.
@@ -40,16 +40,16 @@
 instance, given a scenario when May is parsed by the function, with this
 setting, if this year's May is still in the future, last year's May will be
 returned. - Please note, when there's no ambiguity, the function can still
 return future/past dates, even when a different preference is specified. An
 example: ```python from hun_date_parser import text2datetime from datetime
 import datetime from hun_date_parser.utils import SearchScopes text2datetime
 ('augusztus', now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH)
-# [{'start_date': datetime.datetime(2023, 8, 1, 0, 0), # 'end_date':
-datetime.datetime(2023, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
+# [{'start_date': datetime.datetime(2022, 8, 1, 0, 0), # 'end_date':
+datetime.datetime(2022, 8, 31, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.PAST_SEARCH) # [
 {'start_date': datetime.datetime(2023, 6, 2, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 2, 23, 59, 59)}] text2datetime('pÃ©ntek',
 now=datetime(2023, 6, 7), search_scope=SearchScopes.NOT_RESTRICTED) # [
 {'start_date': datetime.datetime(2023, 6, 9, 0, 0), # 'end_date':
 datetime.datetime(2023, 6, 9, 23, 59, 59)}] ``` The library is also capable of
 turning datetime objects into their Hungarian text representation. ```python
```

### Comparing `hun-date-parser-0.2.0/hun_date_parser.egg-info/SOURCES.txt` & `hun-date-parser-0.2.1/hun_date_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.0/setup.py` & `hun-date-parser-0.2.1/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import pathlib
-
-import pkg_resources
-import setuptools
-import re
-import hun_date_parser
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-    long_description = re.sub(r':.*:', '', long_description)  # remove Github emojis
-
-with pathlib.Path('requirements.txt').open() as requirements_txt:
-    install_requires = [
-        str(requirement)
-        for requirement
-        in pkg_resources.parse_requirements(requirements_txt)
-    ]
-
-setuptools.setup(
-    name="hun-date-parser",
-    version=hun_date_parser.__version__,
-    author="Soma Nagy",
-    author_email="nagysomabalint@gmail.com",
-    description="A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/szegedai/hun-date-parser",
-    install_requires=install_requires,
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-)
+import pathlib
+
+import pkg_resources
+import setuptools
+import re
+import hun_date_parser
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+    long_description = re.sub(r':.*:', '', long_description)  # remove Github emojis
+
+with pathlib.Path('requirements.txt').open() as requirements_txt:
+    install_requires = [
+        str(requirement)
+        for requirement
+        in pkg_resources.parse_requirements(requirements_txt)
+    ]
+
+setuptools.setup(
+    name="hun-date-parser",
+    version=hun_date_parser.__version__,
+    author="Soma Nagy",
+    author_email="nagysomabalint@gmail.com",
+    description="A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/szegedai/hun-date-parser",
+    install_requires=install_requires,
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+)
```

### Comparing `hun-date-parser-0.2.0/test/test_date_parsers.py` & `hun-date-parser-0.2.1/test/test_date_parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,244 +1,255 @@
-import pytest
-from datetime import datetime
-
-from hun_date_parser.date_parser.date_parsers import Year, Month, Week, Day, OverrideTopWithNow
-from hun_date_parser.date_parser.date_parsers import (match_iso_date, match_named_month, match_relative_day,
-                                                      match_weekday,
-                                                      match_week, match_named_year, match_relative_month,
-                                                      match_n_periods_compared_to_now, match_in_past_n_periods)
-from hun_date_parser.utils import SearchScopes
-
-
-tf_named_month = [
-    ('jan 20-án', [[Month(1, 'named_month'), Day(20, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('2020 febr. 4', [[Month(2, 'named_month'), Day(4, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('január', [[Month(1, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    (' február ', [[Month(2, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('janos', [], SearchScopes.NOT_RESTRICTED),
-    ('', [], SearchScopes.NOT_RESTRICTED),
-    ('2020 július', [[Month(7, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('2020 június - augusztus 30', [[Month(6, 'named_month')], [Month(8, 'named_month'), Day(30, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('június 20 - július 30',
-     [[Month(6, 'named_month'), Day(20, 'named_month')], [Month(7, 'named_month'), Day(30, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('tavaly február ', [[Month(2, 'named_month'), Year(2019, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('legyen jövő február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('legyen jövő év február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('ápr 15', [[Month(4, 'named_month'), Day(15, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('április 1', [[Month(4, 'named_month'), Day(1, 'named_month')]], SearchScopes.NOT_RESTRICTED),
-    ('legyen jövőre február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month'), Year(2021, 'named_month')]],
-     SearchScopes.FUTURE_DAY),
-    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-    ('november 15', [[Month(11, 'named_month'), Day(15, 'named_month'), Year(2019, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month')]],
-     SearchScopes.FUTURE_DAY),
-    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month'), Year(2019, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-    ('október 3', [[Month(10, 'named_month'), Day(3, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('október 10', [[Month(10, 'named_month'), Day(10, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('október 10', [[Month(10, 'named_month'), Day(10, 'named_month')]],
-     SearchScopes.FUTURE_DAY),
-    ('október 9', [[Month(10, 'named_month'), Day(9, 'named_month'), Year(2021, 'named_month')]],
-     SearchScopes.FUTURE_DAY),
-    ('október 11', [[Month(10, 'named_month'), Day(11, 'named_month'), Year(2019, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-    ('október', [[Month(10, 'named_month')]],
-     SearchScopes.NOT_RESTRICTED),
-    ('október', [[Month(10, 'named_month')]],
-     SearchScopes.FUTURE_DAY),
-    ('október', [[Month(10, 'named_month')]],
-     SearchScopes.PAST_SEARCH),
-]
-
-tf_match_relative_day = [
-    ('ma', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')]]),
-    ('ma-holnap', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')],
-                   [Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(2, 'relative_day')]]),
-    ('holnapután reggel nyolc', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(3, 'relative_day')]]),
-    ('legyen ma reggel', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')]]),
-    ('miért nem jöttél tegnap? na majd ma',
-     [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')],
-      [Year(2020, 'relative_day'), Month(9, 'relative_day'), Day(30, 'relative_day')]])
-]
-
-tf_iso_date = [
-    ('2020-01-15', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
-    ('legyen 2020-01 elején', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date')]]),
-    ('2001-ben történt', [[Year(2001, 'match_iso_date')]]),
-    ('2020-12-30-án', [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')]]),
-    ('2020-12-30-án 2020.12.29',
-     [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')],
-      [Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(29, 'match_iso_date')]])]
-
-tf_weekday = [
-    ('múlt vasárnap', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(6, 'weekday')]], SearchScopes.NOT_RESTRICTED),
-    ('ezen a heten hetfon', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(7, 'weekday')]], SearchScopes.NOT_RESTRICTED),
-    ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
-    ('előző szombaton ', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(5, 'weekday')]], SearchScopes.NOT_RESTRICTED),
-    ('miért nem jöttél tegnap? na majd ma', [], SearchScopes.NOT_RESTRICTED),
-    ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
-    ('szombaton ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(12, 'weekday')]], SearchScopes.FUTURE_DAY),
-    ('mit szólnál hétfőhöz?', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(14, 'weekday')]], SearchScopes.FUTURE_DAY),
-    ('pénteken ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(11, 'weekday')]], SearchScopes.FUTURE_DAY),
-    ('múlt hét kedden beszéltünk', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(1, 'weekday')]], SearchScopes.FUTURE_DAY),
-    ('szerdán ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(16, 'weekday')]], SearchScopes.FUTURE_DAY),
-    ('jövő héten szerdán ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(16, 'weekday')]], SearchScopes.FUTURE_DAY)]
-
-tf_week = [('múlthéten', [[Year(2020, "week"), Week(49, "week")]]),
-           ('múlt hét kedden', [[Year(2020, "week"), Week(49, "week")]]),
-           ('ezen a heten hetfon', [[Year(2020, "week"), Week(50, "week")]]),
-           ('jövőhéten', [[Year(2020, "week"), Week(51, "week")]]),
-           ('legyen ma', [])]
-
-tf_named_year = [('tavaly', [[Year(2019, 'named_year')]]),
-                 ('múlt hét kedden', []),
-                 ('legyen meg még idén légyszi', [[Year(2020, 'named_year')]]),
-                 ('kb két év múlva', [[Year(2022, 'named_year')]]),
-                 ('tavalyelőtt történt', [[Year(2018, 'named_year')]]),
-                 ('40 év múlva', [[Year(2060, 'named_year')]]),
-                 ('kb három évvel ezelőtt', [[Year(2017, 'named_year')]]),
-                 ('találkozzunk jövő héten szombaton', [])]
-
-tf_relative_month = [
-    ('az utolsó hónapom.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
-    ('a legutóbbi hónapom.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
-    ('a legutobbi honapom', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
-    ('mi történt a múlt hónapban?', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
-    ('Mik az elmúlt hónapban történtek', [[]]),
-    ('a múlt hónapban időrendi sorrendben.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
-    (' az elmúlt hónapban a?', [[]]),
-    (' az elmult honapban a?', [[]]),
-    ('ebben a hónapban', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
-    ('ezen hónapban', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
-    ('az aktuális hónap', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
-    ('jövő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
-    ('következő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
-    ('következendő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
-]
-
-tf_n_periods_from_now = [
-    ('egy hét múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(27, 'n_date_periods_compared_to_now')]]),
-    ('egy héttel korábban', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(13, 'n_date_periods_compared_to_now')]]),
-    ('két héttel korábbi időpont', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(6, 'n_date_periods_compared_to_now')]]),
-    ('1 hét múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(27, 'n_date_periods_compared_to_now')]]),
-    ('1 héttel ezelőtt', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(13, 'n_date_periods_compared_to_now')]]),
-    ('6 nappal ezelőtt', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(14, 'n_date_periods_compared_to_now')]]),
-    ('5 nap múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(25, 'n_date_periods_compared_to_now')]]),
-]
-
-tf_in_past_n_periods = [
-    ("elmúlt egy hét", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
-                         Day(13, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
-    ("az előző egy hétben", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
-                              Day(13, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
-    ("az előző két hétben", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
-                              Day(6, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
-    ("az előző két évi adatok", [[Year(2021, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
-                                  Day(20, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
-    ("az előző 10 nap tranzakciói", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
-                                      Day(10, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
-    ("az előző sport nap teljesítménye", []),
-]
-
-
-@pytest.mark.parametrize("inp,exp", tf_iso_date)
-def test_match_iso_date(inp, exp):
-    out = match_iso_date(inp)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp,search_scope", tf_named_month)
-def test_named_month(inp, exp, search_scope):
-    now = datetime(2020, 10, 10)
-
-    out = match_named_month(inp, now, search_scope)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_match_relative_day)
-def test_match_relative_day(inp, exp):
-    now = datetime(2020, 10, 1)
-
-    out = match_relative_day(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp,search_scope", tf_weekday)
-def test_match_weekday(inp, exp, search_scope):
-    now = datetime(2020, 12, 11)  # friday
-    out = match_weekday(inp, now, search_scope)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_week)
-def test_match_match_week(inp, exp):
-    now = datetime(2020, 12, 7)
-    out = match_week(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_named_year)
-def test_match_named_year(inp, exp):
-    now = datetime(2020, 12, 7)
-    out = match_named_year(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_relative_month)
-def test_match_relative_month(inp, exp):
-    now = datetime(2023, 5, 20)
-    out = match_relative_month(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_n_periods_from_now)
-def test_match_n_periods_compared_to_now(inp, exp):
-    now = datetime(2023, 5, 20)
-    out = match_n_periods_compared_to_now(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-@pytest.mark.parametrize("inp,exp", tf_in_past_n_periods)
-def test_match_in_past_n_periods(inp, exp):
-    now = datetime(2023, 5, 20)
-    out = match_in_past_n_periods(inp, now)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
+import pytest
+from datetime import datetime
+
+from hun_date_parser.date_parser.date_parsers import Year, Month, Week, Day, OverrideTopWithNow
+from hun_date_parser.date_parser.date_parsers import (match_iso_date, match_named_month, match_relative_day,
+                                                      match_weekday,
+                                                      match_week, match_named_year, match_relative_month,
+                                                      match_n_periods_compared_to_now, match_in_past_n_periods)
+from hun_date_parser.utils import SearchScopes
+
+
+tf_named_month = [
+    ('jan 20-án', [[Month(1, 'named_month'), Day(20, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('2020 febr. 4', [[Month(2, 'named_month'), Day(4, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('január', [[Month(1, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    (' február ', [[Month(2, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('janos', [], SearchScopes.NOT_RESTRICTED),
+    ('', [], SearchScopes.NOT_RESTRICTED),
+    ('2020 július', [[Month(7, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('2020 június - augusztus 30', [[Month(6, 'named_month')], [Month(8, 'named_month'), Day(30, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('június 20 - július 30',
+     [[Month(6, 'named_month'), Day(20, 'named_month')], [Month(7, 'named_month'), Day(30, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('tavaly február ', [[Month(2, 'named_month'), Year(2019, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('legyen jövő február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('legyen jövő év február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('ápr 15', [[Month(4, 'named_month'), Day(15, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('április 1', [[Month(4, 'named_month'), Day(1, 'named_month')]], SearchScopes.NOT_RESTRICTED),
+    ('legyen jövőre február 12-én', [[Month(2, 'named_month'), Day(12, 'named_month'), Year(2021, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month'), Year(2021, 'named_month')]],
+     SearchScopes.FUTURE_DAY),
+    ('május 15', [[Month(5, 'named_month'), Day(15, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+    ('november 15', [[Month(11, 'named_month'), Day(15, 'named_month'), Year(2019, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month')]],
+     SearchScopes.FUTURE_DAY),
+    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month'), Year(2019, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+    ('október 3', [[Month(10, 'named_month'), Day(3, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+    ('október 15', [[Month(10, 'named_month'), Day(15, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('október 10', [[Month(10, 'named_month'), Day(10, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('október 10', [[Month(10, 'named_month'), Day(10, 'named_month')]],
+     SearchScopes.FUTURE_DAY),
+    ('október 9', [[Month(10, 'named_month'), Day(9, 'named_month'), Year(2021, 'named_month')]],
+     SearchScopes.FUTURE_DAY),
+    ('október 11', [[Month(10, 'named_month'), Day(11, 'named_month'), Year(2019, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+    ('október', [[Month(10, 'named_month')]],
+     SearchScopes.NOT_RESTRICTED),
+    ('október', [[Month(10, 'named_month')]],
+     SearchScopes.FUTURE_DAY),
+    ('október', [[Month(10, 'named_month')]],
+     SearchScopes.PAST_SEARCH),
+]
+
+tf_match_relative_day = [
+    ('ma', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')]]),
+    ('ma-holnap', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')],
+                   [Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(2, 'relative_day')]]),
+    ('holnapután reggel nyolc', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(3, 'relative_day')]]),
+    ('legyen ma reggel', [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')]]),
+    ('miért nem jöttél tegnap? na majd ma',
+     [[Year(2020, 'relative_day'), Month(10, 'relative_day'), Day(1, 'relative_day')],
+      [Year(2020, 'relative_day'), Month(9, 'relative_day'), Day(30, 'relative_day')]])
+]
+
+tf_iso_date = [
+    ('2020-01-15', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('legyen 2020-01 elején', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date')]]),
+    ('2001-ben történt', [[Year(2001, 'match_iso_date')]]),
+    ('2020-12-30-án', [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')]]),
+    ('2020-12-30-án 2020.12.29',
+     [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')],
+      [Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(29, 'match_iso_date')]]),
+    ('2020 12 30-án', [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')]]),
+    ('a 1 1 1 b', []),
+    ('abcd 2020 1 15 abd', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('abcd 2020 01 15 abd', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('2020 01 15', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('15 01 2020', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('abcd 2020 01 15 10', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('ekkor: 15-01-2020', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('ekkor 08 08 2023', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
+    ('ekkor 36 08 2023', [[Year(2023, 'match_iso_date')]]),
+]
+
+tf_weekday = [
+    ('múlt vasárnap', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(6, 'weekday')]], SearchScopes.NOT_RESTRICTED),
+    ('ezen a heten hetfon', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(7, 'weekday')]], SearchScopes.NOT_RESTRICTED),
+    ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
+    ('előző szombaton ', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(5, 'weekday')]], SearchScopes.NOT_RESTRICTED),
+    ('miért nem jöttél tegnap? na majd ma', [], SearchScopes.NOT_RESTRICTED),
+    ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
+    ('szombaton ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(12, 'weekday')]], SearchScopes.FUTURE_DAY),
+    ('mit szólnál hétfőhöz?', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(14, 'weekday')]], SearchScopes.FUTURE_DAY),
+    ('pénteken ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(11, 'weekday')]], SearchScopes.FUTURE_DAY),
+    ('múlt hét kedden beszéltünk', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(1, 'weekday')]], SearchScopes.FUTURE_DAY),
+    ('szerdán ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(16, 'weekday')]], SearchScopes.FUTURE_DAY),
+    ('jövő héten szerdán ráérek', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(16, 'weekday')]], SearchScopes.FUTURE_DAY)]
+
+tf_week = [('múlthéten', [[Year(2020, "week"), Week(49, "week")]]),
+           ('múlt hét kedden', [[Year(2020, "week"), Week(49, "week")]]),
+           ('ezen a heten hetfon', [[Year(2020, "week"), Week(50, "week")]]),
+           ('jövőhéten', [[Year(2020, "week"), Week(51, "week")]]),
+           ('legyen ma', [])]
+
+tf_named_year = [('tavaly', [[Year(2019, 'named_year')]]),
+                 ('múlt hét kedden', []),
+                 ('legyen meg még idén légyszi', [[Year(2020, 'named_year')]]),
+                 ('kb két év múlva', [[Year(2022, 'named_year')]]),
+                 ('tavalyelőtt történt', [[Year(2018, 'named_year')]]),
+                 ('40 év múlva', [[Year(2060, 'named_year')]]),
+                 ('kb három évvel ezelőtt', [[Year(2017, 'named_year')]]),
+                 ('találkozzunk jövő héten szombaton', [])]
+
+tf_relative_month = [
+    ('az utolsó hónapom.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
+    ('a legutóbbi hónapom.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
+    ('a legutobbi honapom', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
+    ('mi történt a múlt hónapban?', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
+    ('Mik az elmúlt hónapban történtek', [[]]),
+    ('a múlt hónapban időrendi sorrendben.', [[Year(2023, 'relative_month'), Month(4, 'relative_month')]]),
+    (' az elmúlt hónapban a?', [[]]),
+    (' az elmult honapban a?', [[]]),
+    ('ebben a hónapban', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
+    ('ezen hónapban', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
+    ('az aktuális hónap', [[Year(2023, 'relative_month'), Month(5, 'relative_month')]]),
+    ('jövő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
+    ('következő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
+    ('következendő hónap', [[Year(2023, 'relative_month'), Month(6, 'relative_month')]]),
+]
+
+tf_n_periods_from_now = [
+    ('egy hét múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(27, 'n_date_periods_compared_to_now')]]),
+    ('egy héttel korábban', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(13, 'n_date_periods_compared_to_now')]]),
+    ('két héttel korábbi időpont', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(6, 'n_date_periods_compared_to_now')]]),
+    ('1 hét múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(27, 'n_date_periods_compared_to_now')]]),
+    ('1 héttel ezelőtt', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(13, 'n_date_periods_compared_to_now')]]),
+    ('6 nappal ezelőtt', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(14, 'n_date_periods_compared_to_now')]]),
+    ('5 nap múlva', [[Year(2023, 'n_date_periods_compared_to_now'), Month(5, 'n_date_periods_compared_to_now'), Day(25, 'n_date_periods_compared_to_now')]]),
+]
+
+tf_in_past_n_periods = [
+    ("elmúlt egy hét", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
+                         Day(13, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
+    ("az előző egy hétben", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
+                              Day(13, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
+    ("az előző két hétben", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
+                              Day(6, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
+    ("az előző két évi adatok", [[Year(2021, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
+                                  Day(20, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
+    ("az előző 10 nap tranzakciói", [[Year(2023, 'in_past_n_periods'), Month(5, 'in_past_n_periods'),
+                                      Day(10, 'in_past_n_periods'), OverrideTopWithNow(None, 'in_past_n_periods')]]),
+    ("az előző sport nap teljesítménye", []),
+]
+
+
+@pytest.mark.parametrize("inp,exp", tf_iso_date)
+def test_match_iso_date(inp, exp):
+    out = match_iso_date(inp)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp,search_scope", tf_named_month)
+def test_named_month(inp, exp, search_scope):
+    now = datetime(2020, 10, 10)
+
+    out = match_named_month(inp, now, search_scope)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_match_relative_day)
+def test_match_relative_day(inp, exp):
+    now = datetime(2020, 10, 1)
+
+    out = match_relative_day(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp,search_scope", tf_weekday)
+def test_match_weekday(inp, exp, search_scope):
+    now = datetime(2020, 12, 11)  # friday
+    out = match_weekday(inp, now, search_scope)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_week)
+def test_match_match_week(inp, exp):
+    now = datetime(2020, 12, 7)
+    out = match_week(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_named_year)
+def test_match_named_year(inp, exp):
+    now = datetime(2020, 12, 7)
+    out = match_named_year(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_relative_month)
+def test_match_relative_month(inp, exp):
+    now = datetime(2023, 5, 20)
+    out = match_relative_month(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_n_periods_from_now)
+def test_match_n_periods_compared_to_now(inp, exp):
+    now = datetime(2023, 5, 20)
+    out = match_n_periods_compared_to_now(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+@pytest.mark.parametrize("inp,exp", tf_in_past_n_periods)
+def test_match_in_past_n_periods(inp, exp):
+    now = datetime(2023, 5, 20)
+    out = match_in_past_n_periods(inp, now)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
```

### Comparing `hun-date-parser-0.2.0/test/test_datetime_extractor.py` & `hun-date-parser-0.2.1/test/test_datetime_extractor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-import pytest
-from datetime import datetime
-
-from hun_date_parser.utils import *
-from hun_date_parser.date_parser.datetime_extractor import DatetimeExtractor, extend_start_end
-
-scenarios = [
-    ('ezen a héten', [datetime(2020, 12, 14, 0, 0, 0), datetime(2020, 12, 20, 23, 59, 59)]),
-    ('legyen ma reggel nyolckor', [datetime(2020, 12, 18, 8, 0, 0), datetime(2020, 12, 18, 8, 59, 59)]),
-    ('legyen ma', [datetime(2020, 12, 18, 0, 0, 0), datetime(2020, 12, 18, 23, 59, 59)]),
-    ('találkozzunk szombaton reggel háromnegyed nyolckor', [datetime(2020, 12, 19, 7, 45, 0),
-                                                            datetime(2020, 12, 19, 7, 45, 59)]),
-    ('találkozzunk szombaton háromnegyed nyolckor', [datetime(2020, 12, 19, 7, 45, 0),
-                                                     datetime(2020, 12, 19, 7, 45, 59)]),
-    ('találkozzunk december 27-én', [datetime(2020, 12, 27), datetime(2020, 12, 27, 23, 59, 59)]),
-    ('találkozzunk december 10-én', [datetime(2020, 12, 10), datetime(2020, 12, 10, 23, 59, 59)]),
-    ('találkozzunk jövő héten kedden', [datetime(2020, 12, 22), datetime(2020, 12, 22, 23, 59, 59)]),
-    ('találkozzunk jövő héten kedden reggel nyolckor', [datetime(2020, 12, 22, 8), datetime(2020, 12, 22, 8, 59, 59)]),
-    ('ráérek jövő hét hétfőn', [datetime(2020, 12, 21), datetime(2020, 12, 21, 23, 59, 59)]),
-    ('ráérek jövő hét hétfőn reggel 7-kor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
-    ('ráérek jövő hét hétfőn reggel hétkor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
-    ('ráérek jövő hétfőn reggel hétkor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
-    ('ráérek reggel hétkor', [datetime(2020, 12, 18, 7), datetime(2020, 12, 18, 7, 59, 59)]),
-    ('hétfőn reggel hétkor', [datetime(2020, 12, 14, 7), datetime(2020, 12, 14, 7, 59, 59)]),
-    ('reggel hétkor', [datetime(2020, 12, 18, 7), datetime(2020, 12, 18, 7, 59, 59)]),
-    ('hétkor', [datetime(2020, 12, 18, 19), datetime(2020, 12, 18, 19, 59, 59)]),
-    ('2021 január 5', [datetime(2021, 1, 5), datetime(2021, 1, 5, 23, 59, 59)]),
-    ('2021 január 5 reggel 7', [datetime(2021, 1, 5, 7), datetime(2021, 1, 5, 7, 59, 59)]),
-    ('január 5 reggel 7', [datetime(2020, 1, 5, 7), datetime(2020, 1, 5, 7, 59, 59)]),
-    ('január 5-én', [datetime(2020, 1, 5), datetime(2020, 1, 5, 23, 59, 59)]),
-    ('legyen most mondjuk', [datetime(2020, 12, 18), datetime(2020, 12, 18, 0, 0, 59)]),  # TODO: Come up with better
-    ('egy óra múlva', [datetime(2020, 12, 18, 1), datetime(2020, 12, 18, 1, 59, 59)]),
-    ('két óra múlva', [datetime(2020, 12, 18, 2), datetime(2020, 12, 18, 2, 59, 59)]),
-    ('egy hét múlva', [datetime(2020, 12, 25), datetime(2020, 12, 25, 23, 59, 59)]),
-    ('5 perc múlva', [datetime(2020, 12, 18, 0, 5), datetime(2020, 12, 18, 0, 5, 59)]),
-    ('három nap múlva', [datetime(2020, 12, 21), datetime(2020, 12, 21, 23, 59, 59)]),
-    ('csütörtök', [datetime(2020, 12, 17), datetime(2020, 12, 17, 23, 59, 59)]),
-    ('jövő csütörtökön', [datetime(2020, 12, 24), datetime(2020, 12, 24, 23, 59, 59)]),
-    ('jövő csütörtökön 16h', [datetime(2020, 12, 24, 16), datetime(2020, 12, 24, 16, 59, 59)]),
-    ('igen 10-kor', [datetime(2020, 12, 18, 10), datetime(2020, 12, 18, 10, 59, 59)]),
-    ('csütörtök vagy péntek', [datetime(2020, 12, 17), datetime(2020, 12, 17, 23, 59, 59),
-                               datetime(2020, 12, 18), datetime(2020, 12, 18, 23, 59, 59)]),
-    ('előző két napban', [datetime(2020, 12, 16), datetime(2020, 12, 18)]),
-    ('előző 14 napban', [datetime(2020, 12, 4), datetime(2020, 12, 18)]),
-    ('előző tizennégy napban', [datetime(2020, 12, 4), datetime(2020, 12, 18)]),
-    ('előző 1 havi', [datetime(2020, 11, 18), datetime(2020, 12, 18)]),
-    ('előző 2 havi', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('előző két havi', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('előző két hónapban', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('megelőző két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('az elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('az elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
-    ('az elmúlt hónap', [datetime(2020, 11, 18), datetime(2020, 12, 18)]),
-    ('az elmúlt nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
-    ('az elmúlt 1 nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
-    ('az elmúlt egy nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
-    ('az elmúlt hét', [datetime(2020, 12, 11), datetime(2020, 12, 18)]),
-    ('az elmúlt 1 hét', [datetime(2020, 12, 11), datetime(2020, 12, 18)]),
-]
-
-
-@pytest.mark.parametrize("inp_txt, resp", scenarios)
-def test_datetime_extractor(inp_txt, resp):
-    now = datetime(2020, 12, 18)
-    de = DatetimeExtractor(now)
-    parsed_date = de.parse_datetime(inp_txt)
-
-    if len(resp) == 2:
-        st, end = resp
-
-        assert len(parsed_date) == 1
-        assert parsed_date[0]['start_date'] == st
-        assert parsed_date[0]['end_date'] == end
-
-    elif len(resp) == 4:
-        st1, end1, st2, end2 = resp
-
-        assert len(parsed_date) == 2
-        assert parsed_date[0]['start_date'] == st1
-        assert parsed_date[0]['end_date'] == end1
-        assert parsed_date[1]['start_date'] == st2
-        assert parsed_date[1]['end_date'] == end2
-
-
-def test_extend_start_end():
-    inp_1 = {'start_date': [], 'end_date': [Hour(1, '')]}
-    assert extend_start_end(inp_1) == inp_1
-
-    inp_2 = {'start_date': [Month(1, ''), Hour(1, '')], 'end_date': []}
-    assert extend_start_end(inp_2) == {'start_date': [Month(1, ''), Hour(1, '')],
-                                       'end_date': [Month(1, ''), Hour(1, '')]}
-
-
-assemble_scenarios = [
-    ([Year(2024, "rule_name"), Month(2, "rule_name")], datetime(2024, 2, 1, 0, 0, 0), True),
-    ([Year(2024, "rule_name"), Month(2, "rule_name")], datetime(2024, 2, 29, 23, 59, 59), False),
-
-    ([Year(2024, "rule_name"), Month(2, "rule_name"), Day(2, "rule_name")], datetime(2024, 2, 2, 0, 0, 0), True),
-    ([Year(2024, "rule_name"), Month(2, "rule_name"), Day(2, "rule_name")], datetime(2024, 2, 2, 23, 59, 59), False),
-
-    ([Month(7, "rule_name"), Day(2, "rule_name")], datetime(2023, 7, 2, 0, 0, 0), True),
-    ([Month(7, "rule_name"), Day(2, "rule_name")], datetime(2023, 7, 2, 23, 59, 59), False),
-
-    ([Day(29, "rule_name"), Hour(10, "rule_name")], datetime(2023, 5, 29, 10, 0, 0), True),
-    ([Day(29, "rule_name"), Hour(10, "rule_name")], datetime(2023, 5, 29, 10, 59, 59), False),
-
-    ([Hour(10, "rule_name")], datetime(2023, 5, 23, 10, 0, 0), True),
-
-    ([Hour(12, "rule_name"), OverrideBottomWithNow(None, "rule_name")], datetime(2023, 5, 23, 12, 59, 59), False),
-    ([Hour(12, "rule_name"), OverrideBottomWithNow(None, "rule_name")], datetime(2023, 5, 23, 0, 0, 0), True),
-    ([Year(2023, "rule_name"), Month(5, "rule_name"), Day(22, "rule_name"), Hour(12, "rule_name"),
-      OverrideTopWithNow(None, "rule_name")], datetime(2023, 5, 22, 12, 0, 0), True),
-    ([Year(2023, "rule_name"), Month(5, "rule_name"), Day(22, "rule_name"), Hour(12, "rule_name"),
-      OverrideTopWithNow(None, "rule_name")], datetime(2023, 5, 23, 0, 0, 0), False),
-]
-
-
-@pytest.mark.parametrize("inp_lst, resp, is_bottom", assemble_scenarios)
-def test_assemble_datetime(inp_lst, resp, is_bottom):
-    now = datetime(2023, 5, 23)
-    dt_extractor = DatetimeExtractor()
-    result = dt_extractor.assemble_datetime(now=now,
-                                            dateparts=inp_lst,
-                                            bottom=is_bottom)
-
-    assert result == resp
-
-
-tf_past_search_scenarios = [
-    ('ezen a héten', [datetime(2023, 5, 29, 0, 0, 0), datetime(2023, 6, 4, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ('ezen a héten', [datetime(2023, 5, 29, 0, 0, 0), datetime(2023, 6, 4, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ('legyen ma reggel nyolckor', [datetime(2023, 6, 1, 8, 0, 0), datetime(2023, 6, 1, 8, 59, 59)],
-     SearchScopes.PAST_SEARCH),
-    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("szombat", [datetime(2023, 5, 27, 0, 0, 0), datetime(2023, 5, 27, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("szombat", [datetime(2023, 6, 3, 0, 0, 0), datetime(2023, 6, 3, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ("szombat", [datetime(2023, 6, 3, 0, 0, 0), datetime(2023, 6, 3, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("múlt szombat", [datetime(2023, 5, 27, 0, 0, 0), datetime(2023, 5, 27, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ("szerda", [datetime(2023, 5, 31, 0, 0, 0), datetime(2023, 5, 31, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("kedd", [datetime(2023, 5, 30, 0, 0, 0), datetime(2023, 5, 30, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("kedd", [datetime(2023, 5, 30, 0, 0, 0), datetime(2023, 5, 30, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ("kedd", [datetime(2023, 6, 6, 0, 0, 0), datetime(2023, 6, 6, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("jövő hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-    ("jövő hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("augusztus", [datetime(2022, 8, 1, 0, 0, 0), datetime(2022, 8, 31, 23, 59, 59)], SearchScopes.PAST_SEARCH),
-    ("augusztus", [datetime(2023, 8, 1, 0, 0, 0), datetime(2023, 8, 31, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
-    ("augusztus", [datetime(2023, 8, 1, 0, 0, 0), datetime(2023, 8, 31, 23, 59, 59)], SearchScopes.FUTURE_DAY),
-]
-
-
-@pytest.mark.parametrize("inp_txt, resp, search_scope", tf_past_search_scenarios)
-def test_past_search(inp_txt, resp, search_scope):
-    now = datetime(2023, 6, 1)
-    de = DatetimeExtractor(now, search_scope=search_scope)
-    parsed_date = de.parse_datetime(inp_txt)
-    st, end = resp
-
-    assert len(parsed_date) == 1
-    assert parsed_date[0]['start_date'] == st
-    assert parsed_date[0]['end_date'] == end
-
-
-tf_bad_dates = [
-    "január 32",
-    "június 31"
-]
-
-
-@pytest.mark.parametrize("inp_txt", tf_bad_dates)
-def test_bad_dates(inp_txt):
-    now = datetime(2023, 6, 1)
-    de = DatetimeExtractor(now)
-    parsed_date = de.parse_datetime(inp_txt)
-    assert parsed_date == []
-
+import pytest
+from datetime import datetime
+
+from hun_date_parser.utils import *
+from hun_date_parser.date_parser.datetime_extractor import DatetimeExtractor, extend_start_end
+
+scenarios = [
+    ('ezen a héten', [datetime(2020, 12, 14, 0, 0, 0), datetime(2020, 12, 20, 23, 59, 59)]),
+    ('legyen ma reggel nyolckor', [datetime(2020, 12, 18, 8, 0, 0), datetime(2020, 12, 18, 8, 59, 59)]),
+    ('legyen ma', [datetime(2020, 12, 18, 0, 0, 0), datetime(2020, 12, 18, 23, 59, 59)]),
+    ('találkozzunk szombaton reggel háromnegyed nyolckor', [datetime(2020, 12, 19, 7, 45, 0),
+                                                            datetime(2020, 12, 19, 7, 45, 59)]),
+    ('találkozzunk szombaton háromnegyed nyolckor', [datetime(2020, 12, 19, 7, 45, 0),
+                                                     datetime(2020, 12, 19, 7, 45, 59)]),
+    ('találkozzunk december 27-én', [datetime(2020, 12, 27), datetime(2020, 12, 27, 23, 59, 59)]),
+    ('találkozzunk december 10-én', [datetime(2020, 12, 10), datetime(2020, 12, 10, 23, 59, 59)]),
+    ('találkozzunk jövő héten kedden', [datetime(2020, 12, 22), datetime(2020, 12, 22, 23, 59, 59)]),
+    ('találkozzunk jövő héten kedden reggel nyolckor', [datetime(2020, 12, 22, 8), datetime(2020, 12, 22, 8, 59, 59)]),
+    ('ráérek jövő hét hétfőn', [datetime(2020, 12, 21), datetime(2020, 12, 21, 23, 59, 59)]),
+    ('ráérek jövő hét hétfőn reggel 7-kor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
+    ('ráérek jövő hét hétfőn reggel hétkor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
+    ('ráérek jövő hétfőn reggel hétkor', [datetime(2020, 12, 21, 7), datetime(2020, 12, 21, 7, 59, 59)]),
+    ('ráérek reggel hétkor', [datetime(2020, 12, 18, 7), datetime(2020, 12, 18, 7, 59, 59)]),
+    ('hétfőn reggel hétkor', [datetime(2020, 12, 14, 7), datetime(2020, 12, 14, 7, 59, 59)]),
+    ('reggel hétkor', [datetime(2020, 12, 18, 7), datetime(2020, 12, 18, 7, 59, 59)]),
+    ('hétkor', [datetime(2020, 12, 18, 19), datetime(2020, 12, 18, 19, 59, 59)]),
+    ('2021 január 5', [datetime(2021, 1, 5), datetime(2021, 1, 5, 23, 59, 59)]),
+    ('2021 január 5 reggel 7', [datetime(2021, 1, 5, 7), datetime(2021, 1, 5, 7, 59, 59)]),
+    ('január 5 reggel 7', [datetime(2020, 1, 5, 7), datetime(2020, 1, 5, 7, 59, 59)]),
+    ('január 5-én', [datetime(2020, 1, 5), datetime(2020, 1, 5, 23, 59, 59)]),
+    ('legyen most mondjuk', [datetime(2020, 12, 18), datetime(2020, 12, 18, 0, 0, 59)]),  # TODO: Come up with better
+    ('egy óra múlva', [datetime(2020, 12, 18, 1), datetime(2020, 12, 18, 1, 59, 59)]),
+    ('két óra múlva', [datetime(2020, 12, 18, 2), datetime(2020, 12, 18, 2, 59, 59)]),
+    ('egy hét múlva', [datetime(2020, 12, 25), datetime(2020, 12, 25, 23, 59, 59)]),
+    ('5 perc múlva', [datetime(2020, 12, 18, 0, 5), datetime(2020, 12, 18, 0, 5, 59)]),
+    ('három nap múlva', [datetime(2020, 12, 21), datetime(2020, 12, 21, 23, 59, 59)]),
+    ('csütörtök', [datetime(2020, 12, 17), datetime(2020, 12, 17, 23, 59, 59)]),
+    ('jövő csütörtökön', [datetime(2020, 12, 24), datetime(2020, 12, 24, 23, 59, 59)]),
+    ('jövő csütörtökön 16h', [datetime(2020, 12, 24, 16), datetime(2020, 12, 24, 16, 59, 59)]),
+    ('igen 10-kor', [datetime(2020, 12, 18, 10), datetime(2020, 12, 18, 10, 59, 59)]),
+    ('csütörtök vagy péntek', [datetime(2020, 12, 17), datetime(2020, 12, 17, 23, 59, 59),
+                               datetime(2020, 12, 18), datetime(2020, 12, 18, 23, 59, 59)]),
+    ('előző két napban', [datetime(2020, 12, 16), datetime(2020, 12, 18)]),
+    ('előző 14 napban', [datetime(2020, 12, 4), datetime(2020, 12, 18)]),
+    ('előző tizennégy napban', [datetime(2020, 12, 4), datetime(2020, 12, 18)]),
+    ('előző 1 havi', [datetime(2020, 11, 18), datetime(2020, 12, 18)]),
+    ('előző 2 havi', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('előző két havi', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('előző két hónapban', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('megelőző két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('az elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('az elmúlt két hónap', [datetime(2020, 10, 18), datetime(2020, 12, 18)]),
+    ('az elmúlt hónap', [datetime(2020, 11, 18), datetime(2020, 12, 18)]),
+    ('az elmúlt nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
+    ('az elmúlt 1 nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
+    ('az elmúlt egy nap', [datetime(2020, 12, 17), datetime(2020, 12, 18)]),
+    ('az elmúlt hét', [datetime(2020, 12, 11), datetime(2020, 12, 18)]),
+    ('az elmúlt 1 hét', [datetime(2020, 12, 11), datetime(2020, 12, 18)]),
+]
+
+
+@pytest.mark.parametrize("inp_txt, resp", scenarios)
+def test_datetime_extractor(inp_txt, resp):
+    now = datetime(2020, 12, 18)
+    de = DatetimeExtractor(now)
+    parsed_date = de.parse_datetime(inp_txt)
+
+    if len(resp) == 2:
+        st, end = resp
+
+        assert len(parsed_date) == 1
+        assert parsed_date[0]['start_date'] == st
+        assert parsed_date[0]['end_date'] == end
+
+    elif len(resp) == 4:
+        st1, end1, st2, end2 = resp
+
+        assert len(parsed_date) == 2
+        assert parsed_date[0]['start_date'] == st1
+        assert parsed_date[0]['end_date'] == end1
+        assert parsed_date[1]['start_date'] == st2
+        assert parsed_date[1]['end_date'] == end2
+
+
+def test_extend_start_end():
+    inp_1 = {'start_date': [], 'end_date': [Hour(1, '')]}
+    assert extend_start_end(inp_1) == inp_1
+
+    inp_2 = {'start_date': [Month(1, ''), Hour(1, '')], 'end_date': []}
+    assert extend_start_end(inp_2) == {'start_date': [Month(1, ''), Hour(1, '')],
+                                       'end_date': [Month(1, ''), Hour(1, '')]}
+
+
+assemble_scenarios = [
+    ([Year(2024, "rule_name"), Month(2, "rule_name")], datetime(2024, 2, 1, 0, 0, 0), True),
+    ([Year(2024, "rule_name"), Month(2, "rule_name")], datetime(2024, 2, 29, 23, 59, 59), False),
+
+    ([Year(2024, "rule_name"), Month(2, "rule_name"), Day(2, "rule_name")], datetime(2024, 2, 2, 0, 0, 0), True),
+    ([Year(2024, "rule_name"), Month(2, "rule_name"), Day(2, "rule_name")], datetime(2024, 2, 2, 23, 59, 59), False),
+
+    ([Month(7, "rule_name"), Day(2, "rule_name")], datetime(2023, 7, 2, 0, 0, 0), True),
+    ([Month(7, "rule_name"), Day(2, "rule_name")], datetime(2023, 7, 2, 23, 59, 59), False),
+
+    ([Day(29, "rule_name"), Hour(10, "rule_name")], datetime(2023, 5, 29, 10, 0, 0), True),
+    ([Day(29, "rule_name"), Hour(10, "rule_name")], datetime(2023, 5, 29, 10, 59, 59), False),
+
+    ([Hour(10, "rule_name")], datetime(2023, 5, 23, 10, 0, 0), True),
+
+    ([Hour(12, "rule_name"), OverrideBottomWithNow(None, "rule_name")], datetime(2023, 5, 23, 12, 59, 59), False),
+    ([Hour(12, "rule_name"), OverrideBottomWithNow(None, "rule_name")], datetime(2023, 5, 23, 0, 0, 0), True),
+    ([Year(2023, "rule_name"), Month(5, "rule_name"), Day(22, "rule_name"), Hour(12, "rule_name"),
+      OverrideTopWithNow(None, "rule_name")], datetime(2023, 5, 22, 12, 0, 0), True),
+    ([Year(2023, "rule_name"), Month(5, "rule_name"), Day(22, "rule_name"), Hour(12, "rule_name"),
+      OverrideTopWithNow(None, "rule_name")], datetime(2023, 5, 23, 0, 0, 0), False),
+]
+
+
+@pytest.mark.parametrize("inp_lst, resp, is_bottom", assemble_scenarios)
+def test_assemble_datetime(inp_lst, resp, is_bottom):
+    now = datetime(2023, 5, 23)
+    dt_extractor = DatetimeExtractor()
+    result = dt_extractor.assemble_datetime(now=now,
+                                            dateparts=inp_lst,
+                                            bottom=is_bottom)
+
+    assert result == resp
+
+
+tf_past_search_scenarios = [
+    ('ezen a héten', [datetime(2023, 5, 29, 0, 0, 0), datetime(2023, 6, 4, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ('ezen a héten', [datetime(2023, 5, 29, 0, 0, 0), datetime(2023, 6, 4, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ('legyen ma reggel nyolckor', [datetime(2023, 6, 1, 8, 0, 0), datetime(2023, 6, 1, 8, 59, 59)],
+     SearchScopes.PAST_SEARCH),
+    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ('legyen ma', [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("szombat", [datetime(2023, 5, 27, 0, 0, 0), datetime(2023, 5, 27, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("szombat", [datetime(2023, 6, 3, 0, 0, 0), datetime(2023, 6, 3, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ("szombat", [datetime(2023, 6, 3, 0, 0, 0), datetime(2023, 6, 3, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("múlt szombat", [datetime(2023, 5, 27, 0, 0, 0), datetime(2023, 5, 27, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("csütörtök", [datetime(2023, 6, 1, 0, 0, 0), datetime(2023, 6, 1, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ("szerda", [datetime(2023, 5, 31, 0, 0, 0), datetime(2023, 5, 31, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ("múlt szerda", [datetime(2023, 5, 24, 0, 0, 0), datetime(2023, 5, 24, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("kedd", [datetime(2023, 5, 30, 0, 0, 0), datetime(2023, 5, 30, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("kedd", [datetime(2023, 5, 30, 0, 0, 0), datetime(2023, 5, 30, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ("kedd", [datetime(2023, 6, 6, 0, 0, 0), datetime(2023, 6, 6, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("jövő hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+    ("jövő hétfő", [datetime(2023, 6, 5, 0, 0, 0), datetime(2023, 6, 5, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("augusztus", [datetime(2022, 8, 1, 0, 0, 0), datetime(2022, 8, 31, 23, 59, 59)], SearchScopes.PAST_SEARCH),
+    ("augusztus", [datetime(2023, 8, 1, 0, 0, 0), datetime(2023, 8, 31, 23, 59, 59)], SearchScopes.NOT_RESTRICTED),
+    ("augusztus", [datetime(2023, 8, 1, 0, 0, 0), datetime(2023, 8, 31, 23, 59, 59)], SearchScopes.FUTURE_DAY),
+]
+
+
+@pytest.mark.parametrize("inp_txt, resp, search_scope", tf_past_search_scenarios)
+def test_past_search(inp_txt, resp, search_scope):
+    now = datetime(2023, 6, 1)
+    de = DatetimeExtractor(now, search_scope=search_scope)
+    parsed_date = de.parse_datetime(inp_txt)
+    st, end = resp
+
+    assert len(parsed_date) == 1
+    assert parsed_date[0]['start_date'] == st
+    assert parsed_date[0]['end_date'] == end
+
+
+tf_bad_dates = [
+    "január 32",
+    "június 31"
+]
+
+
+@pytest.mark.parametrize("inp_txt", tf_bad_dates)
+def test_bad_dates(inp_txt):
+    now = datetime(2023, 6, 1)
+    de = DatetimeExtractor(now)
+    parsed_date = de.parse_datetime(inp_txt)
+    assert parsed_date == []
+
```

### Comparing `hun-date-parser-0.2.0/test/test_exposed.py` & `hun-date-parser-0.2.1/test/test_exposed.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from datetime import datetime, date, time
-
-from hun_date_parser import datetime2text, text2datetime, text2date, text2time
-
-
-def test_datetime2text():
-    candidates = datetime2text(datetime(2020, 12, 21))
-
-    assert set(candidates) == {'dates', 'times'}
-    assert len([c for c in candidates['dates'] if c]) == 2
-    assert len([c for c in candidates['times'] if c]) == 4
-
-
-def test_text2datetime():
-    now = datetime(2020, 12, 27)
-    tf = [('ma', [{'start_date': datetime(2020, 12, 27), 'end_date': datetime(2020, 12, 27, 23, 59, 59)}]),
-          ('ma reggel', [{'start_date': datetime(2020, 12, 27, 6), 'end_date': datetime(2020, 12, 27, 10, 59, 59)}])]
-
-    for inp, out in tf:
-        assert text2datetime(inp, now=now) == out
-
-
-def test_text2date():
-    now = datetime(2020, 12, 27)
-    tf = [('ma', [{'start_date': date(2020, 12, 27), 'end_date': date(2020, 12, 27)}]),
-          ('ma reggel', [{'start_date': date(2020, 12, 27), 'end_date': date(2020, 12, 27)}]),
-          ('reggel nyolc óra', [])]
-
-    for inp, out in tf:
-        assert text2date(inp, now=now) == out
-
-
-def test_text2time():
-    now = datetime(2020, 12, 27)
-    tf = [('ma', []),
-          ('ma reggel', [{'start_date': time(6), 'end_date': time(10, 59, 59)}]),
-          ('ma délelőtt', [{'start_date': time(8), 'end_date': time(11, 59, 59)}]),
-          ('reggel nyolc óra', [{'start_date': time(8), 'end_date': time(8, 59, 59)}])]
-
-    for inp, out in tf:
-        assert text2time(inp, now=now) == out
+from datetime import datetime, date, time
+
+from hun_date_parser import datetime2text, text2datetime, text2date, text2time
+
+
+def test_datetime2text():
+    candidates = datetime2text(datetime(2020, 12, 21))
+
+    assert set(candidates) == {'dates', 'times'}
+    assert len([c for c in candidates['dates'] if c]) == 2
+    assert len([c for c in candidates['times'] if c]) == 4
+
+
+def test_text2datetime():
+    now = datetime(2020, 12, 27)
+    tf = [('ma', [{'start_date': datetime(2020, 12, 27), 'end_date': datetime(2020, 12, 27, 23, 59, 59)}]),
+          ('ma reggel', [{'start_date': datetime(2020, 12, 27, 6), 'end_date': datetime(2020, 12, 27, 10, 59, 59)}])]
+
+    for inp, out in tf:
+        assert text2datetime(inp, now=now) == out
+
+
+def test_text2date():
+    now = datetime(2020, 12, 27)
+    tf = [('ma', [{'start_date': date(2020, 12, 27), 'end_date': date(2020, 12, 27)}]),
+          ('ma reggel', [{'start_date': date(2020, 12, 27), 'end_date': date(2020, 12, 27)}]),
+          ('reggel nyolc óra', [])]
+
+    for inp, out in tf:
+        assert text2date(inp, now=now) == out
+
+
+def test_text2time():
+    now = datetime(2020, 12, 27)
+    tf = [('ma', []),
+          ('ma reggel', [{'start_date': time(6), 'end_date': time(10, 59, 59)}]),
+          ('ma délelőtt', [{'start_date': time(8), 'end_date': time(11, 59, 59)}]),
+          ('reggel nyolc óra', [{'start_date': time(8), 'end_date': time(8, 59, 59)}])]
+
+    for inp, out in tf:
+        assert text2time(inp, now=now) == out
```

### Comparing `hun-date-parser-0.2.0/test/test_restricted_parsing.py` & `hun-date-parser-0.2.1/test/test_restricted_parsing.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import pytest
-from datetime import datetime
-
-from hun_date_parser.date_parser.interval_restriction import extract_datetime_within_interval, ExtractWithinRangeSuccess
-
-
-scenarios = [
-        ({'start_date': datetime(2021, 10, 11), 'end_date': datetime(2021, 10, 18, 23, 59, 59)},
-         'kedden',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2021, 10, 12), 'end_date': datetime(2021, 10, 12, 23, 59, 59)}])),
-
-        ({'start_date': datetime(2021, 10, 11), 'end_date': datetime(2021, 10, 18, 23, 59, 59)},
-         'kedden vagy szerdán',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2021, 10, 12), 'end_date': datetime(2021, 10, 12, 23, 59, 59)}])),
-
-        ({'start_date': datetime(2022, 1, 1), 'end_date': datetime(2022, 12, 31, 23, 59, 59)},
-         'februárban',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2022, 2, 1), 'end_date': datetime(2022, 2, 28, 23, 59, 59)}])),
-
-        ({'start_date': datetime(2020, 1, 1), 'end_date': datetime(2020, 12, 31, 23, 59, 59)},
-         'februárban',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2020, 2, 1), 'end_date': datetime(2020, 2, 29, 23, 59, 59)}])),
-
-        # Test AM/PM mismatch resolution
-        ({'start_date': datetime(2021, 1, 1, 12), 'end_date': datetime(2021, 1, 1, 16, 59, 59)},
-         'három órakor',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2021, 1, 1, 15), 'end_date': datetime(2021, 1, 1, 15, 59, 59)}])),
-
-        # Test AM/PM mismatch resolution
-        ({'start_date': datetime(2021, 1, 1, 18), 'end_date': datetime(2021, 1, 1, 21, 59, 59)},
-         'nyolc órakor',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2021, 1, 1, 20), 'end_date': datetime(2021, 1, 1, 20, 59, 59)}])),
-
-        # Test AM/PM mismatch resolution
-        ({'start_date': datetime(2021, 1, 1, 18), 'end_date': datetime(2021, 1, 1, 21, 59, 59)},
-         'reggel nyolckor',
-         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
-          [{'start_date': datetime(2021, 10, 11, 8), 'end_date': datetime(2021, 10, 11, 8, 59, 59)}])),
-
-        # Test AM/PM mismatch resolution
-        ({'start_date': datetime(2021, 1, 1, 20), 'end_date': datetime(2021, 1, 2, 2, 59, 59)},
-         '12-kor',
-         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
-          [{'start_date': datetime(2021, 1, 2, 0), 'end_date': datetime(2021, 1, 2, 0, 59, 59)}])),
-
-        ({'start_date': datetime(2020, 1, 1), 'end_date': datetime(2020, 12, 31, 23, 59, 59)},
-         'jövő februárban',
-         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
-          [{'start_date': datetime(2022, 2, 1), 'end_date': datetime(2022, 2, 28, 23, 59, 59)}])),
-
-        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
-         'augusztusban',
-         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
-          [{'start_date': datetime(2021, 8, 1), 'end_date': datetime(2021, 8, 31, 23, 59, 59)}])),
-
-        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
-         'augusztustól',
-         (ExtractWithinRangeSuccess.OPEN_RANGE_FALLBACK,
-          [{'start_date': datetime(2021, 8, 1), 'end_date': None}])),
-
-        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
-         'jövő kedd',
-         (ExtractWithinRangeSuccess.RELATIVE_TIME_WORD_FALLBACK,
-          [{'start_date': datetime(2021, 10, 19), 'end_date': datetime(2021, 10, 19, 23, 59, 59)}])),
-    ]
-
-
-@pytest.mark.parametrize("interval_restriction, query_sentence, expected", scenarios)
-def test_extract_within_interval(interval_restriction, query_sentence, expected):
-    result = extract_datetime_within_interval(interval_restriction['start_date'],
-                                              interval_restriction['end_date'],
-                                              query_sentence,
-                                              fallback_now=datetime(2021, 10, 11))
-
-    assert result == expected
+import pytest
+from datetime import datetime
+
+from hun_date_parser.date_parser.interval_restriction import extract_datetime_within_interval, ExtractWithinRangeSuccess
+
+
+scenarios = [
+        ({'start_date': datetime(2021, 10, 11), 'end_date': datetime(2021, 10, 18, 23, 59, 59)},
+         'kedden',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2021, 10, 12), 'end_date': datetime(2021, 10, 12, 23, 59, 59)}])),
+
+        ({'start_date': datetime(2021, 10, 11), 'end_date': datetime(2021, 10, 18, 23, 59, 59)},
+         'kedden vagy szerdán',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2021, 10, 12), 'end_date': datetime(2021, 10, 12, 23, 59, 59)}])),
+
+        ({'start_date': datetime(2022, 1, 1), 'end_date': datetime(2022, 12, 31, 23, 59, 59)},
+         'februárban',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2022, 2, 1), 'end_date': datetime(2022, 2, 28, 23, 59, 59)}])),
+
+        ({'start_date': datetime(2020, 1, 1), 'end_date': datetime(2020, 12, 31, 23, 59, 59)},
+         'februárban',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2020, 2, 1), 'end_date': datetime(2020, 2, 29, 23, 59, 59)}])),
+
+        # Test AM/PM mismatch resolution
+        ({'start_date': datetime(2021, 1, 1, 12), 'end_date': datetime(2021, 1, 1, 16, 59, 59)},
+         'három órakor',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2021, 1, 1, 15), 'end_date': datetime(2021, 1, 1, 15, 59, 59)}])),
+
+        # Test AM/PM mismatch resolution
+        ({'start_date': datetime(2021, 1, 1, 18), 'end_date': datetime(2021, 1, 1, 21, 59, 59)},
+         'nyolc órakor',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2021, 1, 1, 20), 'end_date': datetime(2021, 1, 1, 20, 59, 59)}])),
+
+        # Test AM/PM mismatch resolution
+        ({'start_date': datetime(2021, 1, 1, 18), 'end_date': datetime(2021, 1, 1, 21, 59, 59)},
+         'reggel nyolckor',
+         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
+          [{'start_date': datetime(2021, 10, 11, 8), 'end_date': datetime(2021, 10, 11, 8, 59, 59)}])),
+
+        # Test AM/PM mismatch resolution
+        ({'start_date': datetime(2021, 1, 1, 20), 'end_date': datetime(2021, 1, 2, 2, 59, 59)},
+         '12-kor',
+         (ExtractWithinRangeSuccess.VALID_IN_RANGE,
+          [{'start_date': datetime(2021, 1, 2, 0), 'end_date': datetime(2021, 1, 2, 0, 59, 59)}])),
+
+        ({'start_date': datetime(2020, 1, 1), 'end_date': datetime(2020, 12, 31, 23, 59, 59)},
+         'jövő februárban',
+         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
+          [{'start_date': datetime(2022, 2, 1), 'end_date': datetime(2022, 2, 28, 23, 59, 59)}])),
+
+        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
+         'augusztusban',
+         (ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK,
+          [{'start_date': datetime(2021, 8, 1), 'end_date': datetime(2021, 8, 31, 23, 59, 59)}])),
+
+        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
+         'augusztustól',
+         (ExtractWithinRangeSuccess.OPEN_RANGE_FALLBACK,
+          [{'start_date': datetime(2021, 8, 1), 'end_date': None}])),
+
+        ({'start_date': datetime(2021, 1, 1), 'end_date': datetime(2021, 3, 31, 23, 59, 59)},
+         'jövő kedd',
+         (ExtractWithinRangeSuccess.RELATIVE_TIME_WORD_FALLBACK,
+          [{'start_date': datetime(2021, 10, 19), 'end_date': datetime(2021, 10, 19, 23, 59, 59)}])),
+    ]
+
+
+@pytest.mark.parametrize("interval_restriction, query_sentence, expected", scenarios)
+def test_extract_within_interval(interval_restriction, query_sentence, expected):
+    result = extract_datetime_within_interval(interval_restriction['start_date'],
+                                              interval_restriction['end_date'],
+                                              query_sentence,
+                                              fallback_now=datetime(2021, 10, 11))
+
+    assert result == expected
```

### Comparing `hun-date-parser-0.2.0/test/test_structure_parsers.py` & `hun-date-parser-0.2.1/test/test_structure_parsers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from hun_date_parser.date_parser.structure_parsers import match_interval, match_multi_match
-
-
-def test_match_interval():
-    w = [('keddtől egészen péntekig', {'start_date': 'keddtől', 'end_date': 'egészen péntekig'}),
-         ('reggeltől estig', {'start_date': 'reggeltől', 'end_date': 'estig'}),
-         ('kedden', {}),
-         ('2020 január másodikától jövő év közepéig', {'start_date': '2020 január másodikától', 'end_date': 'jövő év közepéig'}),
-         ('2020 decemberétől', {'start_date': '2020 decemberétől', 'end_date': 'OPEN'}),
-         ('ma reggeltől bármikor', {'start_date': 'ma reggeltől', 'end_date': 'OPEN'}),
-         ('egészen péntekig jó lesz', {'start_date': 'OPEN', 'end_date': 'egészen péntekig'}),
-         ('2020-10-12-től 2020-11-01-ig', {'start_date': '2020-10-12-től', 'end_date': '2020-11-01-ig'})]
-
-    for inp, out in w:
-        assert match_interval(inp) == out
-
-
-def test_match_multi_match():
-    w = [('kedden és szerdán', ['kedden', 'szerdán']),
-         # ('kedden, szerdán és pénteken', ['kedden', 'szerdán', 'pénteken']),
-         # ('kedden, szerdán', ['kedden', 'szerdán']),
-         # These could cause significant unintended consequences,
-         # deeper rethinking is required than simply splitting among commas as well
-         ('2020 január vagy februárjában', ['2020 január', 'februárjában'])]
-
-    for inp, out in w:
-        assert match_multi_match(inp) == out
+from hun_date_parser.date_parser.structure_parsers import match_interval, match_multi_match
+
+
+def test_match_interval():
+    w = [('keddtől egészen péntekig', {'start_date': 'keddtől', 'end_date': 'egészen péntekig'}),
+         ('reggeltől estig', {'start_date': 'reggeltől', 'end_date': 'estig'}),
+         ('kedden', {}),
+         ('2020 január másodikától jövő év közepéig', {'start_date': '2020 január másodikától', 'end_date': 'jövő év közepéig'}),
+         ('2020 decemberétől', {'start_date': '2020 decemberétől', 'end_date': 'OPEN'}),
+         ('ma reggeltől bármikor', {'start_date': 'ma reggeltől', 'end_date': 'OPEN'}),
+         ('egészen péntekig jó lesz', {'start_date': 'OPEN', 'end_date': 'egészen péntekig'}),
+         ('2020-10-12-től 2020-11-01-ig', {'start_date': '2020-10-12-től', 'end_date': '2020-11-01-ig'})]
+
+    for inp, out in w:
+        assert match_interval(inp) == out
+
+
+def test_match_multi_match():
+    w = [('kedden és szerdán', ['kedden', 'szerdán']),
+         # ('kedden, szerdán és pénteken', ['kedden', 'szerdán', 'pénteken']),
+         # ('kedden, szerdán', ['kedden', 'szerdán']),
+         # These could cause significant unintended consequences,
+         # deeper rethinking is required than simply splitting among commas as well
+         ('2020 január vagy februárjában', ['2020 január', 'februárjában'])]
+
+    for inp, out in w:
+        assert match_multi_match(inp) == out
```

### Comparing `hun-date-parser-0.2.0/test/test_time_parsers.py` & `hun-date-parser-0.2.1/test/test_time_parsers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import pytest
-from datetime import datetime
-
-from hun_date_parser.utils import Year, Month, Day, Daypart, Hour, Minute
-from hun_date_parser.date_parser.time_parsers import match_digi_clock, match_time_words, match_now, match_hwords
-
-
-def test_match_digi_clock():
-    fn = 'digi_clock'
-    tf = [('kedden 8:45', [[Hour(8, fn), Minute(45, fn)]]),
-          ('kedden 08:45', [[Hour(8, fn), Minute(45, fn)]]),
-          ('ma este 18:12-kor', [[Hour(18, fn), Minute(12, fn)]])]
-
-    for inp, exp in tf:
-        out = match_digi_clock(inp)
-        date_parts = []
-        for e in out:
-            date_parts.append(e['date_parts'])
-        assert date_parts == exp
-
-
-time_word_fn = 'time_words'
-time_word_scenarios = [
-    ('reggel nyolc előtt hat perccel', [[Hour(7, time_word_fn), Minute(54, time_word_fn)]]),
-    ('reggel nyolc előtt nyolcvan perccel', [[Hour(6, time_word_fn), Minute(40, time_word_fn)]]),
-    ('este 8 előtt 12 perccel', [[Hour(19, time_word_fn), Minute(48, time_word_fn)]]),
-    ('nyolc óra nyolc perckor', [[Hour(8, time_word_fn), Minute(8, time_word_fn)]]),
-    ('ma reggel hat óra', [[Hour(6, time_word_fn)]]),
-    ('ma reggel', [[Daypart(1, time_word_fn)]]),
-    ('ma délután háromkor', [[Hour(15, time_word_fn)]]),
-    ('ma délután három után negyvenhat perckor', [[Hour(15, time_word_fn), Minute(46, time_word_fn)]]),
-    ('ma délután haemdknc után negyvenhat perckor', [[Daypart(3, time_word_fn)]]),
-    ('ma', []),
-    ('ötvenöt perckor', []),
-    ('húsz óra negyvenkilenc perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
-    ('20 óra negyvenkilenc perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
-    ('20 óra 49 perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
-    ('este 8-kor', [[Hour(20, time_word_fn)]]),
-    ('este háromnegyed 8-kor', [[Hour(19, time_word_fn), Minute(45, time_word_fn)]]),
-    ('este negyed 8-kor', [[Hour(19, time_word_fn), Minute(15, time_word_fn)]]),
-    ('háromnegyed nyolckor', [[Hour(7, time_word_fn), Minute(45, time_word_fn)]]),
-    ('este negyed 8 előtt 6 perccel', [[Hour(19, time_word_fn), Minute(9, time_word_fn)]]),
-    ('este háromnegyed 8 előtt két perccel', [[Hour(19, time_word_fn), Minute(43, time_word_fn)]]),
-    ('este fél 8 előtt harminckilenc perccel', [[Hour(18, time_word_fn), Minute(51, time_word_fn)]]),
-    ('este fél 8 előtt', [[Hour(19, time_word_fn), Minute(30, time_word_fn)]]),
-    ('harminckilenc perccel este fél 8 előtt', [[Hour(18, time_word_fn), Minute(51, time_word_fn)]]),
-    ('mondjuk két perccel 6 után', [[Hour(18, time_word_fn), Minute(2, time_word_fn)]]),
-    ('mondjuk tíz perccel 8 óra előtt', [[Hour(7, time_word_fn), Minute(50, time_word_fn)]]),
-    ('délután fél négy után hat perccel', [[Hour(15, time_word_fn), Minute(36, time_word_fn)]]),
-    ('6 óra után 3 perccel', [[Hour(18, time_word_fn), Minute(3, time_word_fn)]]),
-    ('igen, 10-kor', [[Hour(10, time_word_fn)]]),
-    ('igen 10-kor', [[Hour(10, time_word_fn)]]),
-    ('ezen a héten', []),
-    ('2020 december', []),
-    ('kb húsz év múlva', []),
-    ('kb húsz évvel ezelőtt', [])
-]
-
-
-@pytest.mark.parametrize("inp, exp", time_word_scenarios)
-def test_match_time_words(inp, exp):
-    out = match_time_words(inp)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
-
-
-def test_match_now():
-    now = datetime(2020, 12, 30, 12, 1)
-    fn = 'now'
-    tf = [('kedden 8:45', []),
-          ('most kedden', []),
-          ('legyen most',
-           [[Year(now.year, fn), Month(now.month, fn), Day(now.day, fn), Hour(now.hour, fn), Minute(now.minute, fn)]])]
-
-    for inp, exp in tf:
-        out = match_now(inp, now)
-        date_parts = []
-        for e in out:
-            date_parts.append(e['date_parts'])
-        assert date_parts == exp
-
-
-hword_fn = 'hwords'
-hword_scenarios = [
-    ('16h', [[Hour(16, hword_fn)]]),
-    ('16 h', []),
-    ('16h-kor', [[Hour(16, hword_fn)]]),
-    ('h', []),
-    ('1 hely', []),
-    ('jövő csütörtökön 16h', [[Hour(16, hword_fn)]])
-]
-
-
-@pytest.mark.parametrize("inp, exp", hword_scenarios)
-def test_match_hwords(inp, exp):
-    out = match_hwords(inp)
-    date_parts = []
-    for e in out:
-        date_parts.append(e['date_parts'])
-    assert date_parts == exp
+import pytest
+from datetime import datetime
+
+from hun_date_parser.utils import Year, Month, Day, Daypart, Hour, Minute
+from hun_date_parser.date_parser.time_parsers import match_digi_clock, match_time_words, match_now, match_hwords
+
+
+def test_match_digi_clock():
+    fn = 'digi_clock'
+    tf = [('kedden 8:45', [[Hour(8, fn), Minute(45, fn)]]),
+          ('kedden 08:45', [[Hour(8, fn), Minute(45, fn)]]),
+          ('ma este 18:12-kor', [[Hour(18, fn), Minute(12, fn)]])]
+
+    for inp, exp in tf:
+        out = match_digi_clock(inp)
+        date_parts = []
+        for e in out:
+            date_parts.append(e['date_parts'])
+        assert date_parts == exp
+
+
+time_word_fn = 'time_words'
+time_word_scenarios = [
+    ('reggel nyolc előtt hat perccel', [[Hour(7, time_word_fn), Minute(54, time_word_fn)]]),
+    ('reggel nyolc előtt nyolcvan perccel', [[Hour(6, time_word_fn), Minute(40, time_word_fn)]]),
+    ('este 8 előtt 12 perccel', [[Hour(19, time_word_fn), Minute(48, time_word_fn)]]),
+    ('nyolc óra nyolc perckor', [[Hour(8, time_word_fn), Minute(8, time_word_fn)]]),
+    ('ma reggel hat óra', [[Hour(6, time_word_fn)]]),
+    ('ma reggel', [[Daypart(1, time_word_fn)]]),
+    ('ma délután háromkor', [[Hour(15, time_word_fn)]]),
+    ('ma délután három után negyvenhat perckor', [[Hour(15, time_word_fn), Minute(46, time_word_fn)]]),
+    ('ma délután haemdknc után negyvenhat perckor', [[Daypart(3, time_word_fn)]]),
+    ('ma', []),
+    ('ötvenöt perckor', []),
+    ('húsz óra negyvenkilenc perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
+    ('20 óra negyvenkilenc perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
+    ('20 óra 49 perckor', [[Hour(20, time_word_fn), Minute(49, time_word_fn)]]),
+    ('este 8-kor', [[Hour(20, time_word_fn)]]),
+    ('este háromnegyed 8-kor', [[Hour(19, time_word_fn), Minute(45, time_word_fn)]]),
+    ('este negyed 8-kor', [[Hour(19, time_word_fn), Minute(15, time_word_fn)]]),
+    ('háromnegyed nyolckor', [[Hour(7, time_word_fn), Minute(45, time_word_fn)]]),
+    ('este negyed 8 előtt 6 perccel', [[Hour(19, time_word_fn), Minute(9, time_word_fn)]]),
+    ('este háromnegyed 8 előtt két perccel', [[Hour(19, time_word_fn), Minute(43, time_word_fn)]]),
+    ('este fél 8 előtt harminckilenc perccel', [[Hour(18, time_word_fn), Minute(51, time_word_fn)]]),
+    ('este fél 8 előtt', [[Hour(19, time_word_fn), Minute(30, time_word_fn)]]),
+    ('harminckilenc perccel este fél 8 előtt', [[Hour(18, time_word_fn), Minute(51, time_word_fn)]]),
+    ('mondjuk két perccel 6 után', [[Hour(18, time_word_fn), Minute(2, time_word_fn)]]),
+    ('mondjuk tíz perccel 8 óra előtt', [[Hour(7, time_word_fn), Minute(50, time_word_fn)]]),
+    ('délután fél négy után hat perccel', [[Hour(15, time_word_fn), Minute(36, time_word_fn)]]),
+    ('6 óra után 3 perccel', [[Hour(18, time_word_fn), Minute(3, time_word_fn)]]),
+    ('igen, 10-kor', [[Hour(10, time_word_fn)]]),
+    ('igen 10-kor', [[Hour(10, time_word_fn)]]),
+    ('ezen a héten', []),
+    ('2020 december', []),
+    ('kb húsz év múlva', []),
+    ('kb húsz évvel ezelőtt', [])
+]
+
+
+@pytest.mark.parametrize("inp, exp", time_word_scenarios)
+def test_match_time_words(inp, exp):
+    out = match_time_words(inp)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
+
+
+def test_match_now():
+    now = datetime(2020, 12, 30, 12, 1)
+    fn = 'now'
+    tf = [('kedden 8:45', []),
+          ('most kedden', []),
+          ('legyen most',
+           [[Year(now.year, fn), Month(now.month, fn), Day(now.day, fn), Hour(now.hour, fn), Minute(now.minute, fn)]])]
+
+    for inp, exp in tf:
+        out = match_now(inp, now)
+        date_parts = []
+        for e in out:
+            date_parts.append(e['date_parts'])
+        assert date_parts == exp
+
+
+hword_fn = 'hwords'
+hword_scenarios = [
+    ('16h', [[Hour(16, hword_fn)]]),
+    ('16 h', []),
+    ('16h-kor', [[Hour(16, hword_fn)]]),
+    ('h', []),
+    ('1 hely', []),
+    ('jövő csütörtökön 16h', [[Hour(16, hword_fn)]])
+]
+
+
+@pytest.mark.parametrize("inp, exp", hword_scenarios)
+def test_match_hwords(inp, exp):
+    out = match_hwords(inp)
+    date_parts = []
+    for e in out:
+        date_parts.append(e['date_parts'])
+    assert date_parts == exp
```

### Comparing `hun-date-parser-0.2.0/test/test_utils.py` & `hun-date-parser-0.2.1/test/test_utils.py`

 * *Files identical despite different names*

