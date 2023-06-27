# Comparing `tmp/ddb_single-0.3.6.tar.gz` & `tmp/ddb_single-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddb_single-0.3.6.tar", last modified: Wed May  3 02:46:54 2023, max compression
+gzip compressed data, was "ddb_single-0.3.7.tar", last modified: Wed May  3 09:10:10 2023, max compression
```

## Comparing `ddb_single-0.3.6.tar` & `ddb_single-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 02:46:54.450151 ddb_single-0.3.6/
--rw-rw-rw-   0        0        0     9190 2023-05-03 02:46:54.450151 ddb_single-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 02:46:54.436620 ddb_single-0.3.6/ddb_single/
--rw-rw-rw-   0        0        0      144 2023-05-03 02:46:35.000000 ddb_single-0.3.6/ddb_single/__init__.py
--rw-rw-rw-   0        0        0    13297 2023-02-15 12:06:42.000000 ddb_single-0.3.6/ddb_single/model.py
--rw-rw-rw-   0        0        0     8975 2023-04-30 12:08:38.000000 ddb_single-0.3.6/ddb_single/query.py
--rw-rw-rw-   0        0        0    21669 2023-05-03 02:45:55.000000 ddb_single-0.3.6/ddb_single/table.py
--rw-rw-rw-   0        0        0     5899 2022-10-02 09:32:13.000000 ddb_single-0.3.6/ddb_single/utils_botos.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:46:54.449147 ddb_single-0.3.6/ddb_single.egg-info/
--rw-rw-rw-   0        0        0     9190 2023-05-03 02:46:54.000000 ddb_single-0.3.6/ddb_single.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-03 02:46:54.000000 ddb_single-0.3.6/ddb_single.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 02:46:54.000000 ddb_single-0.3.6/ddb_single.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 02:46:54.000000 ddb_single-0.3.6/ddb_single.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 02:46:54.000000 ddb_single-0.3.6/ddb_single.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 02:46:54.450151 ddb_single-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      671 2022-10-02 11:49:36.000000 ddb_single-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:10:10.968000 ddb_single-0.3.7/
+-rw-rw-rw-   0        0        0     9190 2023-05-03 09:10:10.968000 ddb_single-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 09:10:10.933411 ddb_single-0.3.7/ddb_single/
+-rw-rw-rw-   0        0        0      144 2023-05-03 09:09:50.000000 ddb_single-0.3.7/ddb_single/__init__.py
+-rw-rw-rw-   0        0        0    13297 2023-02-15 12:06:42.000000 ddb_single-0.3.7/ddb_single/model.py
+-rw-rw-rw-   0        0        0     8975 2023-04-30 12:08:38.000000 ddb_single-0.3.7/ddb_single/query.py
+-rw-rw-rw-   0        0        0    21790 2023-05-03 09:09:32.000000 ddb_single-0.3.7/ddb_single/table.py
+-rw-rw-rw-   0        0        0     5899 2022-10-02 09:32:13.000000 ddb_single-0.3.7/ddb_single/utils_botos.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:10:10.966990 ddb_single-0.3.7/ddb_single.egg-info/
+-rw-rw-rw-   0        0        0     9190 2023-05-03 09:10:10.000000 ddb_single-0.3.7/ddb_single.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-03 09:10:10.000000 ddb_single-0.3.7/ddb_single.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:10:10.000000 ddb_single-0.3.7/ddb_single.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 09:10:10.000000 ddb_single-0.3.7/ddb_single.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 09:10:10.000000 ddb_single-0.3.7/ddb_single.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:10:10.968000 ddb_single-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      671 2022-10-02 11:49:36.000000 ddb_single-0.3.7/setup.py
```

### Comparing `ddb_single-0.3.6/PKG-INFO` & `ddb_single-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb_single
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ddb_single-0.3.6/ddb_single/model.py` & `ddb_single-0.3.7/ddb_single/model.py`

 * *Files identical despite different names*

### Comparing `ddb_single-0.3.6/ddb_single/query.py` & `ddb_single-0.3.7/ddb_single/query.py`

 * *Files identical despite different names*

### Comparing `ddb_single-0.3.6/ddb_single/table.py` & `ddb_single-0.3.7/ddb_single/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,21 +195,24 @@
                 return util_b.json_export(res_data)
             else:
                 return []
 
     # アイテムの取得
     def get_item(self, pk, sk=None):
         sk = sk if sk else self.pk2sk(pk)
-        res = self.__client__.get_item(
+        res: dict = self.__client__.get_item(
             TableName=self.__table_name__,
             Key={
                 self.__primary_key__: {self.__primary_key_type__: pk},
                 self.__secondary_key__: {self.__secondary_key_type__: sk}
             }
         )
+        if 'Item' not in res:
+            # アイテムがない場合はNoneを返す
+            return None
         res = util_b.deserialize(res.get('Item'))
         res = util_b.json_export(res)
         return res
 
     # アイテムをバッチで取得
     def _batch_get_item(self, key_list:list, sleep_time=0.5, max_tries=5) -> list:
         # リストが空なら空リストを返す
```

### Comparing `ddb_single-0.3.6/ddb_single/utils_botos.py` & `ddb_single-0.3.7/ddb_single/utils_botos.py`

 * *Files identical despite different names*

### Comparing `ddb_single-0.3.6/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.3.7/ddb_single.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb-single
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ddb_single-0.3.6/setup.py` & `ddb_single-0.3.7/setup.py`

 * *Files identical despite different names*

