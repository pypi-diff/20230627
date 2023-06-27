# Comparing `tmp/google-csv-helper-1.0.5.tar.gz` & `tmp/google-csv-helper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.0.5.tar", last modified: Tue Jun  6 18:33:15 2023, max compression
+gzip compressed data, was "google-csv-helper-1.1.0.tar", last modified: Tue Jun 27 17:17:12 2023, max compression
```

## Comparing `google-csv-helper-1.0.5.tar` & `google-csv-helper-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.888971 google-csv-helper-1.0.5/google_csv_helper/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/csv_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/csv_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/google_csv_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/google_csv_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/csv_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/ga3_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/ga4_csv_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/google_csv_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/setup.py
```

### Comparing `google-csv-helper-1.0.5/LICENSE` & `google-csv-helper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.5/PKG-INFO` & `google-csv-helper-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.0.5
+Version: 1.1.0
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # google-csv-helper
 
-[![Upload Python Package](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml)
-
 A simple tool for parsing google csv files.
 
 # Installation
 
 ```
 % pip install google-csv-helper
 ```
```

### Comparing `google-csv-helper-1.0.5/README.md` & `google-csv-helper-1.1.0/google_csv_helper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,23 @@
-# google-csv-helper
+Metadata-Version: 2.1
+Name: google-csv-helper
+Version: 1.1.0
+Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
+Home-page: https://github.com/changyy/google-csv-helper
+Download-URL: https://pypi.org/project/google-csv-helper/
+Author: Yuan-Yi Chang
+Author-email: <changyy.csie@gmail.com>
+Keywords: python,google,csv,adsense,admob,report
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-[![Upload Python Package](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml)
+# google-csv-helper
 
 A simple tool for parsing google csv files.
 
 # Installation
 
 ```
 % pip install google-csv-helper
```

### Comparing `google-csv-helper-1.0.5/google_csv_helper/adsense_csv_helper.py` & `google-csv-helper-1.1.0/google_csv_helper/adsense_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.5/google_csv_helper/cmd.py` & `google-csv-helper-1.1.0/google_csv_helper/cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 # -*- encoding: utf-8 -*-
 import sys
 import argparse
 import datetime
 
 from google_csv_helper import __version__
 from google_csv_helper import adsense_csv_helper
+from google_csv_helper import ga3_csv_helper
+from google_csv_helper import ga4_csv_helper
 
 def main():
     def valid_date(data: str):
         output = datetime.date.today()
         if data != "today":
             try:
                 return datetime.datetime.strptime(data, "%Y-%m-%d")
             except ValueError:
                 raise argparse.ArgumentTypeError(f"not a valid date: {data}")
         return output
     parser = argparse.ArgumentParser()
     parser.add_argument("csv_dir", nargs="*", type=str, help="the directory where the csv file is located")
     parser.add_argument("--output", choices=['json', 'markdown'], default='json', help="results format")
+    parser.add_argument("--output-type", choices=['adsense', 'ga3', 'ga4'], default="adsense", help="the report")
     parser.add_argument("--report", choices=['date', 'week', 'month'], default='date', help="the report type")
     parser.add_argument("--debug", action="store_true", default=False, help="output the debug messages")
     parser.add_argument("--version", action="store_true", default=False, help="show the version")
-    parser.add_argument("--enddate", default="today", type=valid_date, help="date for csv key field filter")
+    parser.add_argument("--enddate", default="today", type=valid_date, help="date for csv key field filter, date format = 'YYYY-mm-dd'")
     parser.add_argument("--adsense-filename-keyword", type=str, default="adsense", help="the keyword on csv filename of adsense")
     parser.add_argument("--admob-filename-keyword", type=str, default="admob", help="the keyword on csv filename of admob")
-    parser.add_argument("--ga-csv-filename-keyword", type=str, default="ga", help="the keyword on csv filename of gogle anayltics")
+    parser.add_argument("--ga-filename-keyword", type=str, default="ga", help="the keyword on csv filename of gogle anayltics")
 
     csv_filename_pattern = []
     args = parser.parse_args()
 
-    for p in args.adsense_filename_keyword.split(','):
-        csv_filename_pattern.append( str(p).strip() )
-    for p in args.admob_filename_keyword.split(','):
-        csv_filename_pattern.append( str(p).strip() )
 
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if len(args.csv_dir) == 0:
         parser.print_help()
         sys.exit(0)
 
-    obj = adsense_csv_helper.AdsenseCSVHelper(args.csv_dir)
+    obj = None
+    if args.output_type == 'adsense':
+        for p in args.adsense_filename_keyword.split(','):
+            csv_filename_pattern.append( str(p).strip() )
+        for p in args.admob_filename_keyword.split(','):
+            csv_filename_pattern.append( str(p).strip() )
+        obj = adsense_csv_helper.AdsenseCSVHelper(args.csv_dir, csv_filename_pattern)
+    elif args.output_type == 'ga3':
+        for p in args.ga_filename_keyword.split(','):
+            csv_filename_pattern.append( str(p).strip() )
+        obj = ga3_csv_helper.GA3CSVHelper(args.csv_dir, csv_filename_pattern)
+    elif args.output_type == 'ga4':
+        for p in args.ga_filename_keyword.split(','):
+            csv_filename_pattern.append( str(p).strip() )
+        obj = ga4_csv_helper.GA4CSVHelper(args.csv_dir, csv_filename_pattern)
 
     if args.debug:
         obj.enableDebug()
     obj.readAllCSVRawFile()
 
     if args.output == 'markdown':
         if args.report == 'date':
-            print("## Current:")
-            print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
-            print("## Previuos:")
-            print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern))
+            if args.output_type == 'adsense':
+                print("## Current:")
+                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
+                print("## Previuos:")
+                print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern))
+            else:
+                print("## Current:")
+                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
+                print("## Previuos:")
+                print(obj.getDailyMarkDownReport(args.enddate - datetime.timedelta(days=7), csv_filename_pattern))
     else:
         if args.report == 'date':
             print(obj.getAllJSONResult())
 
 if __name__ == '__main__':
     main()
```

### Comparing `google-csv-helper-1.0.5/google_csv_helper/csv_common.py` & `google-csv-helper-1.1.0/google_csv_helper/csv_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,33 @@
     "觀察到的有效千次曝光出價 (USD)": "Impression RPM (USD)",
     "點擊次數": "Clicks",
     "點閱率 (%) (%)" : "CTR%",
 
     # GA3 zh-TW
     "日索引": "Date",
     "使用者": "User",
+    "新使用者": "NewUser",
+
+    # Firebase zh-CN
+    "第 N 天" : "",
+    "30 天" : "",
+    "7 天"  : "",
+    "1 天" : "",
+}
+
+CSV_FIREBASE_KEYWORD = {
+    "活跃用户随时间的变化趋势如何？" : "DAU",
+    "开始日期" : "Begin",
+    "结束日期" : "End",
+}
+
+CSV_KEYWORD_USAGE = {
+    "活跃用户随时间的变化趋势如何？" : "",
+    "开始日期" : "",
+    "结束日期" : "",
 }
 
 CSV_FIELD_VALUE_TRANSFORM = {
     "CTR%" : {
         "handlerType": "function",
         "handler": lambda x: str(float(x.replace('%',''))*0.01),
         "newFieldName": "CTR",
@@ -76,15 +95,15 @@
 }
 
 CSV_OUTPUT_ADSENSE_FIELDS = [
     'Estimated earnings (USD)', 'Impressions', 'Impression RPM (USD)', 'Clicks', 'CTR', 'CPC (USD)',
 ]
 
 CSV_OUTPUT_GA_FIELDS = [
-    'User',
+    'User', 'NewUser', 'PageView',
 ]
 
 CSV_INPUT_CHECK_MAIN_FIELD = [
     'Date', 'Week', 'Month',
 ]
 
 CSV_OUTPUT_REPORT_COMPARISON_INFO = [
```

### Comparing `google-csv-helper-1.0.5/google_csv_helper/csv_helper.py` & `google-csv-helper-1.1.0/google_csv_helper/csv_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,48 +8,58 @@
 import csv
 import pandas
 import datetime
 
 class CSVHelper:
     raw_csv_files_output = {}
     pandas_dataframe_output = {}
+    input_field_checking = csv_common.CSV_INPUT_CHECK_MAIN_FIELD
+    input_field_transform = csv_common.CSV_FIELD_NAME_TRANSFORM
     debugMode = False
-    def __init__(self, input_path: str|list[str]):
+    def __init__(self, input_path: str|list[str], filename_pattern: list[str]):
         self.input_path = []
         if isinstance(input_path, str):
             #self.input_path.append(input_path)
-            self.findAllCSV(input_path)
+            self.findAllCSV(input_path, filename_pattern)
         elif isinstance(input_path, list):
             for item in input_path:
                 if isinstance(item, str):
                     #self.input_path.append(item)
-                    self.findAllCSV(item)
+                    self.findAllCSV(item, filename_pattern)
         self.src_file = []
         self.src_dir = []
 
     def enableDebug(self):
         self.debugMode = True
 
     def disableDebug(self):
         self.debugMode = False
 
-    def findAllCSV(self, input_path:str):
+    def findAllCSV(self, input_path:str, filename_pattern:list[str]):
         output = {}
         lookup = {}
         if os.path.isfile(input_path):
             output[ os.path.dirname(input_path) ] = [input_path]
         else:
             for (dirpath, dirnames, filenames) in os.walk(input_path):
                 for f in filenames:
                     exname = os.path.splitext(f)[1].lower()
                     if exname != '.csv' and exname != '.tsv' :
                         continue
                     if dirpath not in output:
                         output[dirpath] = []
                     full_path = os.path.join(dirpath,f)
+                    if len(filename_pattern) != 0:
+                        pick = False
+                        for pattern in filename_pattern:
+                            if pattern in full_path:
+                                pick = True
+                                break
+                        if pick == False:
+                            continue
                     if full_path not in lookup:
                         output[dirpath].append(full_path)
                         lookup[full_path] = dirpath
         self.raw_csv_files_output = output
 
     def readAllCSVRawFile(self):
         output = {}
@@ -76,15 +86,15 @@
                                 df = pandas.read_table(item, comment='#', engine='python', encoding=try_encoding)
                         if df.empty != True and len(df.index) > 1:
                             if self.debugMode:
                                 print(f"Use Encoding: '{try_encoding}' and '{exname}' mode")
                             break
                     except Exception as e:
                         pass
-                if df.empty != True:
+                if df is not None and df.empty != True:
                     try:
                         df = df.dropna(subset=[df.columns[0]]).reset_index(drop=True)
                     except Exception as e:
                         if self.debugMode:
                             print(f"remove NaN row failed: {e}")
                         pass
                     if self.debugMode:
@@ -152,35 +162,35 @@
             return
         if self.debugMode:
             print(f"handlePandasDataFrame: {key}: {filename}")
 
         fieldRename = {}
         # field name transform
         for field in dataFrame.columns:
-            if field in csv_common.CSV_FIELD_NAME_TRANSFORM:
-                fieldRename[field] = csv_common.CSV_FIELD_NAME_TRANSFORM[field]
+            if field in self.input_field_transform:
+                fieldRename[field] = self.input_field_transform[field]
         if len(fieldRename) > 0:
             dataFrame.rename(columns=fieldRename, inplace = True)
             if self.debugMode:
                 print(f"fieldRename: {fieldRename}, result: {dataFrame.columns}")
 
         if key not in self.pandas_dataframe_output:
             self.pandas_dataframe_output[key] = {}
 
         #keyField = dataFrame.columns[0]
         keyField = None
         for field in dataFrame.columns:
-            if field in csv_common.CSV_INPUT_CHECK_MAIN_FIELD:
+            if field in self.input_field_checking:
                 keyField = field
                 break
 
         # Skip
         if keyField == None:
             if self.debugMode:
-                print(f"[WARNING] keyField({csv_common.CSV_INPUT_CHECK_MAIN_FIELD}) not found, skip this data: {filename}, fields: {dataFrame.columns}")
+                print(f"[WARNING] keyField({self.input_field_checking}) not found, skip this data: {filename}, fields: {dataFrame.columns}")
             return
 
         for field, info in csv_common.CSV_FIELD_VALUE_TRANSFORM.items():
             if field in dataFrame.columns and info['newFieldName'] not in dataFrame.columns:
                 #print(dataFrame.columns)
                 if self.debugMode:
                     print(f"[INFO] create '{info['newFieldName']}' field from '{field}' dataframe via '{info['handlerType']}'")
@@ -194,34 +204,33 @@
         for field in csv_common.CSV_OUTPUT_ADSENSE_FIELDS:
             if field not in dataFrame.columns:
                 isAdsenseData = False
                 if self.debugMode:
                     print(f"[INFO] dataField({csv_common.CSV_OUTPUT_ADSENSE_FIELDS}) not found, skip this data: {filename}, field: {dataFrame.columns}")
                 break
 
-        isGAData = True
+        isGAData = False
+        inputGADataFields = []
         for field in csv_common.CSV_OUTPUT_GA_FIELDS:
-            if field not in dataFrame.columns:
-                isGAData = False
-                if self.debugMode:
-                    print(f"[INFO] dataField({csv_common.CSV_OUTPUT_GA_FIELDS}) not found, skip this data: {filename}, field: {dataFrame.columns}")
-                break
+            if field in dataFrame.columns:
+                inputGADataFields.append(field)
+                isGAData = True
 
         if isGAData == False and isAdsenseData == False:
             print(f"[WARNING] skip the data: {dataFrame.columns}")
             return
             
         if self.debugMode:
             print(f"[INFO] import file: {filename}")
 
         currentData = None
         if isAdsenseData:
             currentData = dataFrame[ [keyField] + csv_common.CSV_OUTPUT_ADSENSE_FIELDS ]
         if isGAData:
-            currentData = dataFrame[ [keyField] + csv_common.CSV_OUTPUT_GA_FIELDS ]
+            currentData = dataFrame[ [keyField] + inputGADataFields ]
         currentDataLength = len(currentData)
         currentDateBegin = currentData[keyField][0] if currentDataLength > 0 else None
         currentDateEnd = currentData[keyField][currentDataLength - 1] if currentDataLength > 0 else None
 
         # set output
         if keyField not in self.pandas_dataframe_output[key]:
             self.pandas_dataframe_output[key][keyField] = currentData
```

### Comparing `google-csv-helper-1.0.5/setup.py` & `google-csv-helper-1.1.0/setup.py`

 * *Files identical despite different names*

