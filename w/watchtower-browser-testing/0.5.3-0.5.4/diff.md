# Comparing `tmp/watchtower_browser_testing-0.5.3.tar.gz` & `tmp/watchtower_browser_testing-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.5.3.tar", last modified: Tue Jun 27 08:55:18 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.5.4.tar", last modified: Tue Jun 27 08:57:29 2023, max compression
```

## Comparing `watchtower_browser_testing-0.5.3.tar` & `watchtower_browser_testing-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/
--rw-rw-rw-   0        0        0      310 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.612280 watchtower_browser_testing-0.5.3/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     4813 2023-06-23 14:01:53.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    20929 2023-06-27 08:54:31.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     9381 2023-06-23 13:59:03.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/utils.py
--rw-rw-rw-   0        0        0       21 2023-06-27 08:54:31.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.612280 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:57:29.550774 watchtower_browser_testing-0.5.4/
+-rw-rw-rw-   0        0        0      310 2023-06-27 08:57:29.550774 watchtower_browser_testing-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:57:29.551775 watchtower_browser_testing-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:57:29.542817 watchtower_browser_testing-0.5.4/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     4813 2023-06-23 14:01:53.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:57:29.548774 watchtower_browser_testing-0.5.4/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    20929 2023-06-27 08:57:22.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     9381 2023-06-23 13:59:03.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/utils.py
+-rw-rw-rw-   0        0        0       21 2023-06-27 08:57:22.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:57:29.547774 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-27 08:57:29.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-27 08:57:29.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:57:29.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-27 08:57:29.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 08:57:29.000000 watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.5.3/setup.py` & `watchtower_browser_testing-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing/testsuite.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -317,16 +317,16 @@
 
             for event_name, obj in val.items():
 
                 event_id = scenario_id + '_' + event_name
                 body_validator = obj['validators'].get('body')
                 body_is_dict_list = False
                 if body_validator and isinstance(body_validator, Validator):
-                    body_validator = body_validator.schema
                     body_is_dict_list = body_validator.is_dict_list
+                    body_validator = body_validator.schema
                 json_string_body = json.dumps(dict(body_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
 
                 query_validator = obj['validators'].get('query_string')
                 if query_validator and isinstance(query_validator, Validator):
                     query_validator = query_validator.schema
                 json_string_query = json.dumps(dict(query_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
```

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.5.4/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

