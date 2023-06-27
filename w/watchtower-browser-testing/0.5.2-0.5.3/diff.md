# Comparing `tmp/watchtower_browser_testing-0.5.2.tar.gz` & `tmp/watchtower_browser_testing-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.5.2.tar", last modified: Fri Jun 23 14:05:44 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.5.3.tar", last modified: Tue Jun 27 08:55:18 2023, max compression
```

## Comparing `watchtower_browser_testing-0.5.2.tar` & `watchtower_browser_testing-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/
--rw-rw-rw-   0        0        0      310 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.180038 watchtower_browser_testing-0.5.2/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     4813 2023-06-23 14:01:53.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    18953 2023-06-13 13:52:56.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     9381 2023-06-23 13:59:03.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/utils.py
--rw-rw-rw-   0        0        0       21 2023-06-23 14:05:31.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/
+-rw-rw-rw-   0        0        0      310 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.612280 watchtower_browser_testing-0.5.3/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     4813 2023-06-23 14:01:53.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.628138 watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    20929 2023-06-27 08:54:31.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     9381 2023-06-23 13:59:03.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/utils.py
+-rw-rw-rw-   0        0        0       21 2023-06-27 08:54:31.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:55:18.612280 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 08:55:18.000000 watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.5.2/setup.py` & `watchtower_browser_testing-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing/testsuite.py`

 * *Files 9% similar despite different names*

```diff
@@ -315,42 +315,88 @@
                 val = val_func()
 
 
             for event_name, obj in val.items():
 
                 event_id = scenario_id + '_' + event_name
                 body_validator = obj['validators'].get('body')
+                body_is_dict_list = False
                 if body_validator and isinstance(body_validator, Validator):
                     body_validator = body_validator.schema
+                    body_is_dict_list = body_validator.is_dict_list
                 json_string_body = json.dumps(dict(body_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
 
                 query_validator = obj['validators'].get('query_string')
                 if query_validator and isinstance(query_validator, Validator):
                     query_validator = query_validator.schema
                 json_string_query = json.dumps(dict(query_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
 
                 check_user_id = not 'check_user_id' in obj['validators'] or obj['validators']['check_user_id']
                 allow_multiple = obj.get('allow_multiple', False)
+                n_matches = obj.get('n_matches')
+                n_matches_lt = obj.get('n_matches_lt')
+                n_matches_gt = obj.get('n_matches_gt')
+
+                mdstring = cls.create_validation_string(event_name=event_name,
+                                                        allow_multiple=allow_multiple,
+                                                        check_user_id=check_user_id,
+                                                        json_string_query=json_string_query,
+                                                        json_string_body=json_string_body,
+                                                        body_is_dict_list=body_is_dict_list,
+                                                        n_matches=n_matches,
+                                                        n_matches_lt=n_matches_lt,
+                                                        n_matches_gt=n_matches_gt)
 
-                mdstring = config.VALIDATION_MD_STRING.format(event_name=event_name,
-                                                              allow_multiple=allow_multiple,
-                                                              check_user_id=check_user_id,
-                                                              json_string_query=json_string_query,
-                                                              json_string_body=json_string_body)
                 event_struct = {'name': event_name,
                                 'id': 'e_' + event_id,
                                 'type': 'event',
                                 'description': markdown.convert(mdstring)}
 
                 scenario_struct['children'].append(event_struct)
 
             structure['children'].append(scenario_struct)
 
         return structure
 
+    @staticmethod
+    def create_validation_string(event_name,
+                                 allow_multiple,
+                                 check_user_id,
+                                 json_string_query,
+                                 json_string_body,
+                                 body_is_dict_list,
+                                 n_matches,
+                                 n_matches_lt,
+                                 n_matches_gt):
+
+        if not n_matches is None:
+            n_requests_string = f'n_matches: {n_matches}'
+        elif (not n_matches_gt is None) and (not n_matches_lt is None):
+            n_requests_string = f'n_matches in range: [{n_matches_gt}, {n_matches_lt}]'
+        elif not n_matches_gt is None:
+            n_requests_string = f'n_matches greater than: {n_matches_gt}'
+        elif not n_matches_lt is None:
+            n_requests_string = f'n_matches less than: {n_matches_lt}'
+        else:
+            n_requests_string = f'allow_multiple: {"yes" if allow_multiple else "no"}'
+
+        return f'''
+<details>
+<summary>{event_name} validation (click to see details)</summary>
+
+```
+{n_requests_string}
+
+check_user_id: {"yes" if check_user_id else "no"}
+
+query_params_validator: {json_string_query}
+
+body_validator{" (list of objects)" if body_is_dict_list else ""}: {json_string_body}
+```
+</details>'''
 
 class MeasurementPlan(object):
 
     test_modules = None
     test_directory = None
     display_name = None
     slug = None
```

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.5.3/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

