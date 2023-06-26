# Comparing `tmp/c_custom_code_checker-1.0.2.tar.gz` & `tmp/c_custom_code_checker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c_custom_code_checker-1.0.2.tar", last modified: Sun Jun 25 20:56:02 2023, max compression
+gzip compressed data, was "c_custom_code_checker-1.0.3.tar", last modified: Mon Jun 26 22:33:35 2023, max compression
```

## Comparing `c_custom_code_checker-1.0.2.tar` & `c_custom_code_checker-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.522935 c_custom_code_checker-1.0.2/
--rw-rw-rw-   0        0        0     5096 2023-06-25 20:56:02.521929 c_custom_code_checker-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4577 2023-06-25 20:41:57.000000 c_custom_code_checker-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.431930 c_custom_code_checker-1.0.2/c_custom_code_checker/
--rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.453940 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/
--rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/__init__.py
--rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/criterion_keys.py
--rw-rw-rw-   0        0        0      767 2023-06-24 23:57:10.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/rules_reserved_keys.py
--rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/strings.py
--rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/constants/target_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.483930 c_custom_code_checker-1.0.2/c_custom_code_checker/enums/
--rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/enums/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/enums/criterion_enum.py
--rw-rw-rw-   0        0        0     1728 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/enums/target_enum.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.500938 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/
--rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
--rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
--rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/invalid_criterion_exception.py
--rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/invalid_target_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
--rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/exceptions/rule_missing_target_exception.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.503932 c_custom_code_checker-1.0.2/c_custom_code_checker/handlers/
--rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/handlers/__init__.py
--rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/handlers/criterion_handlers.py
--rw-rw-rw-   0        0        0     3721 2023-06-25 18:09:20.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.507935 c_custom_code_checker-1.0.2/c_custom_code_checker/models/
--rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/models/__init__.py
--rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/models/rule_model.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.513932 c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/
--rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-06-25 18:05:46.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/code_parser.py
--rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/rule_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.520932 c_custom_code_checker-1.0.2/c_custom_code_checker/utlis/
--rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/utlis/__init__.py
--rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/utlis/console_utils.py
--rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c_custom_code_checker-1.0.2/c_custom_code_checker/utlis/files_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:56:02.441929 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/
--rw-rw-rw-   0        0        0     5096 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1688 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-25 20:56:02.000000 c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-06-25 20:55:51.000000 c_custom_code_checker-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 20:56:02.522935 c_custom_code_checker-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-06-25 20:55:30.000000 c_custom_code_checker-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.904306 c_custom_code_checker-1.0.3/
+-rw-rw-rw-   0        0        0     5096 2023-06-26 22:33:35.903305 c_custom_code_checker-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4577 2023-06-25 20:41:57.000000 c_custom_code_checker-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.837355 c_custom_code_checker-1.0.3/c_custom_code_checker/
+-rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.858338 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/
+-rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/criterion_keys.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 22:04:39.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/rules_reserved_keys.py
+-rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/strings.py
+-rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/target_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.866311 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/
+-rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/criterion_enum.py
+-rw-rw-rw-   0        0        0     1949 2023-06-26 22:09:23.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/target_enum.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.883319 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/
+-rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
+-rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
+-rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/invalid_criterion_exception.py
+-rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/invalid_target_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
+-rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/rule_missing_target_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.887305 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/
+-rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/criterion_handlers.py
+-rw-rw-rw-   0        0        0     3723 2023-06-26 22:20:21.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/main.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.890305 c_custom_code_checker-1.0.3/c_custom_code_checker/models/
+-rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/models/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/models/rule_model.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.897316 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/
+-rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/__init__.py
+-rw-rw-rw-   0        0        0     4044 2023-06-26 22:23:27.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/code_parser.py
+-rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/rule_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.902307 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/
+-rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/__init__.py
+-rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/console_utils.py
+-rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/files_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.850336 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/
+-rw-rw-rw-   0        0        0     5096 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1688 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-06-26 22:32:58.000000 c_custom_code_checker-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 22:33:35.904306 c_custom_code_checker-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-06-26 22:33:12.000000 c_custom_code_checker-1.0.3/setup.py
```

### Comparing `c_custom_code_checker-1.0.2/PKG-INFO` & `c_custom_code_checker-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c_custom_code_checker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed
 Author-email: Yago Caetano <yago_caetano@outlook.com>
 Project-URL: Homepage, https://github.com/Yago-Caetano/c-custom-code-checker
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `c_custom_code_checker-1.0.2/README.md` & `c_custom_code_checker-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/constants/rules_reserved_keys.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/constants/rules_reserved_keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TARGET_NAME = "target"
 
     TARGET_TYPE_NONE = "none"
     TARGET_TYPE_METHODS = "functions"
     TARGET_TYPE_GLOBALS = "globals"
     TARGET_TYPE_VARIABLES = "variables"
     TARGET_TYPE_DEFINES = "macros"
+    TARGET_TYPE_ENUMS = "enums"
 
 
     '''
         Criterions
     '''
     CRITERION_OBJ_KEY = "criterion"
     CRITERION_TARGET = "target"
```

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/enums/criterion_enum.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/enums/criterion_enum.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/enums/target_enum.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/enums/target_enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 from c_custom_code_checker.constants.target_keys import TargetKeys
 
 class TargetEnum(Enum):
     TARGET_NONE = {TargetKeys.VALUE_IN_RULE: RulesReservedKeys.TARGET_TYPE_NONE,TargetKeys.CLANG_KINDS:[],TargetKeys.CLANG_LINKAGE_KIND:None,TargetKeys.CLANG_ACCESS_KIND:None}
     TARGET_FUNCTION = {TargetKeys.VALUE_IN_RULE: RulesReservedKeys.TARGET_TYPE_METHODS, TargetKeys.CLANG_KINDS:[CursorKind.FUNCTION_DECL,CursorKind.FUNCTION_TEMPLATE], TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[{TargetKeys.CLANG_LINKAGE_KIND:[LinkageKind.INTERNAL]}],TargetKeys.REQUIREMENTS_OR:[]}}
     TARGET_GLOBAL_VARIABLE = {TargetKeys.VALUE_IN_RULE:RulesReservedKeys.TARGET_TYPE_GLOBALS, TargetKeys.CLANG_KINDS:[CursorKind.VAR_DECL],TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[{TargetKeys.CLANG_LINKAGE_KIND:[LinkageKind.INTERNAL]},{TargetKeys.CLANG_PARENT_KIND:[CursorKind.TRANSLATION_UNIT]}],TargetKeys.REQUIREMENTS_OR:[{TargetKeys.CLANG_ACCESS_KIND:AccessSpecifier.PUBLIC},{TargetKeys.CLANG_PARENT_KIND:None}]}}
     TARGET_LOCAL_VARIABLE = {TargetKeys.VALUE_IN_RULE: RulesReservedKeys.TARGET_TYPE_VARIABLES,TargetKeys.CLANG_KINDS:[CursorKind.VAR_DECL],TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[{TargetKeys.CLANG_LINKAGE_KIND:[LinkageKind.INTERNAL]}],TargetKeys.REQUIREMENTS_OR:[]}}
-    TARGET_DEFINE = {TargetKeys.VALUE_IN_RULE:RulesReservedKeys.TARGET_TYPE_DEFINES,TargetKeys.CLANG_KINDS:[CursorKind.MACRO_DEFINITION,CursorKind.MACRO_INSTANTIATION],TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[],TargetKeys.REQUIREMENTS_OR:[]}}
+    TARGET_DEFINE = {TargetKeys.VALUE_IN_RULE:RulesReservedKeys.TARGET_TYPE_DEFINES,TargetKeys.CLANG_KINDS:[CursorKind.MACRO_DEFINITION,CursorKind.MACRO_INSTANTIATION],TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[],TargetKeys.REQUIREMENTS_OR:[]}}
+    TARGET_TYPE_ENUMS = {TargetKeys.VALUE_IN_RULE:RulesReservedKeys.TARGET_TYPE_ENUMS,TargetKeys.CLANG_KINDS:[CursorKind.ENUM_DECL],TargetKeys.REQUIREMENTS:{TargetKeys.REQUIREMENTS_AND:[],TargetKeys.REQUIREMENTS_OR:[]}}
```

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/handlers/criterion_handlers.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/criterion_handlers.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/main.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import argparse
 import glob
 import platform
 
 from tqdm import tqdm
+
 from c_custom_code_checker.constants.strings import StringsConstants
 from c_custom_code_checker.exceptions.lib_clang_not_found_exception import LibClangNotFoundException
 
 from c_custom_code_checker.parsers.code_parser import CodeParser
 from c_custom_code_checker.parsers.rule_parser import RuleParser
 from c_custom_code_checker.utlis.console_utils import  print_exception, print_failure, print_header, print_process, print_success
 from c_custom_code_checker.utlis.files_utils import search_files_by_keyword
```

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/models/rule_model.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/models/rule_model.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/code_parser.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/code_parser.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/parsers/rule_parser.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/rule_parser.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker/utlis/console_utils.py` & `c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/console_utils.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/PKG-INFO` & `c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c-custom-code-checker
-Version: 1.0.2
+Version: 1.0.3
 Summary: Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed
 Author-email: Yago Caetano <yago_caetano@outlook.com>
 Project-URL: Homepage, https://github.com/Yago-Caetano/c-custom-code-checker
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `c_custom_code_checker-1.0.2/c_custom_code_checker.egg-info/SOURCES.txt` & `c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.2/pyproject.toml` & `c_custom_code_checker-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","art>=6.0","clang>=16.0.1.1","colorama>=0.4.4","libclang>=16.0.0","tqdm>=4.65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c_custom_code_checker"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Yago Caetano", email="yago_caetano@outlook.com" },
 ]
 description = "Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

