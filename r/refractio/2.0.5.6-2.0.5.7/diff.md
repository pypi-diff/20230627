# Comparing `tmp/refractio-2.0.5.6.tar.gz` & `tmp/refractio-2.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.6.tar", last modified: Wed Jun 21 14:06:26 2023, max compression
+gzip compressed data, was "refractio-2.0.5.7.tar", last modified: Tue Jun 27 10:35:40 2023, max compression
```

## Comparing `refractio-2.0.5.6.tar` & `refractio-2.0.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.134051 refractio-2.0.5.6/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-21 14:06:26.133051 refractio-2.0.5.6/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-21 14:05:47.000000 refractio-2.0.5.6/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.132051 refractio-2.0.5.6/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16632 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.133051 refractio-2.0.5.6/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-21 14:06:26.134051 refractio-2.0.5.6/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-21 14:05:47.000000 refractio-2.0.5.6/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.766329 refractio-2.0.5.7/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-27 10:35:40.766329 refractio-2.0.5.7/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-27 10:34:00.000000 refractio-2.0.5.7/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.764329 refractio-2.0.5.7/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16508 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.765329 refractio-2.0.5.7/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-27 10:35:40.766329 refractio-2.0.5.7/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-27 10:34:00.000000 refractio-2.0.5.7/setup.py
```

### Comparing `refractio-2.0.5.6/PKG-INFO` & `refractio-2.0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.6
+Version: 2.0.5.7
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.6/README.md` & `refractio-2.0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/amazons3.py` & `refractio-2.0.5.7/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/azure.py` & `refractio-2.0.5.7/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/hive.py` & `refractio-2.0.5.7/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/manager.py` & `refractio-2.0.5.7/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/mysql.py` & `refractio-2.0.5.7/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/postgres.py` & `refractio-2.0.5.7/refractio/postgres.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/refractio.py` & `refractio-2.0.5.7/refractio/refractio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! -*- coding: utf-8 -*-
 """Library to read and write dataframes"""
 
 import os
 import requests
 import pandas as pd
 
-from .manager import validate_project_id
+from .manager import validate_project_id, get_dataframe_query
 
 
-def get_dataframe(ds_name, project_id=os.getenv("project_id"), row_count=-1, strategy="top", user_id="1001"):
+def get_dataframe(ds_name, project_id=os.getenv("project_id"), row_count=-1, strategy="top", user_id="1001",
+                  filter_condition=None):
     """
     Param:
         ds_name,
         project_id=os.getenv("project_id"),
         row_count=-1,
         strategy="top"
         user_id="1001"
@@ -24,23 +25,23 @@
         project_id = validate_project_id(project_id)
         url = f"http://connection-manager:80/connections/api/External/v1/external/getConnConfig/" \
               f"{ds_name}/refract_user/{project_id}"    # user id hard coded, as it's not being used in API code.
         connection_details = requests.get(url, verify=False).json()
 
         if connection_details["params"]["READER"]["type"] == "RDBMS":
             if connection_details["params"]["READER"]["sub_type"] == "SNOWFLAKE":
-                data_frame = get_snowflake_df(connection_details, row_count, strategy)
+                data_frame = get_snowflake_df(connection_details, row_count, strategy, filter_condition)
             elif connection_details["params"]["READER"]["sub_type"] == "MYSQL":
-                data_frame = get_mysql_df(connection_details, row_count, strategy)
+                data_frame = get_mysql_df(connection_details, row_count, strategy, filter_condition)
             elif connection_details["params"]["READER"]["sub_type"] == "HIVE":
-                data_frame = get_hive_df(connection_details, row_count, strategy, user_id)
+                data_frame = get_hive_df(connection_details, row_count, strategy, user_id, filter_condition)
             elif connection_details["params"]["READER"]["sub_type"] == "SQLSERVER":
-                data_frame = get_sqlserver_df(connection_details, row_count, strategy)
+                data_frame = get_sqlserver_df(connection_details, row_count, strategy, filter_condition)
             elif connection_details["params"]["READER"]["sub_type"] == "POSTGRES":
-                data_frame = get_postgres_df(connection_details, row_count, strategy)
+                data_frame = get_postgres_df(connection_details, row_count, strategy, filter_condition)
             else:
                 print("Reading dataframe using connector backend")
                 # Need to install, git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
                 from connector.mosaicio import MosaicioConnector
                 connector = MosaicioConnector()
                 data_frame = connector.getPandasDataFrame(
                     param=connection_details["params"],
@@ -88,15 +89,15 @@
             return pd.read_excel(io=local_file_path,
                                  nrows=nrows,
                                  parse_dates=False)
     except Exception as ex:
         print(f"Exception occurred in get_local_dataframe: {ex}")
 
 
-def get_snowflake_df(connection_details, row_count, strategy):
+def get_snowflake_df(connection_details, row_count, strategy, filter_condition):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form snowflake connection
     """
@@ -114,30 +115,29 @@
         cloudPlatform=connection_details["params"]["READER"]["cloudPlatform"],
         schema=connection_details["params"]["READER"]["schema"],
         wareHouse=connection_details["params"]["READER"]["wareHouse"],
         region=connection_details["params"]["READER"]["region"]
     )
     # Create cursor
     cur = con.cursor()
-    if int(row_count) > 0:
-        # Execute query
-        cur.execute(f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}")
-    else:
-        cur.execute(f"SELECT * FROM {connection_details['params']['READER']['tables']}")
+    query = get_dataframe_query(connection_details['params']['READER']['tables'],
+                                row_count, filter_condition)  # Get query to fetch details
+
+    cur.execute(query)  # Execute query
 
     # Read results into a pandas DataFrame
     data_frame = cur.fetch_pandas_all()
 
     # Close cursor and connection
     cur.close()
     con.close()
     return data_frame
 
 
-def get_hive_df(connection_details, row_count, strategy, user_id):
+def get_hive_df(connection_details, row_count, strategy, user_id, filter_condition):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
         user_id: template image user id
     To read data frame form hive connection
@@ -150,29 +150,26 @@
     conn = connect(host=connection_details["params"]["READER"]["host"],
                    port=int(connection_details["params"]["READER"]["port"]),
                    auth_mechanism='PLAIN',
                    user=connection_details["params"]["READER"]["user"],
                    password=connection_details["params"]["READER"]["password"],
                    database=connection_details["params"]["READER"]["database"])
 
-    if int(row_count) > 0:
-        # Generate query
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
-    else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
+    query = get_dataframe_query(connection_details['params']['READER']['tables'],
+                                row_count, filter_condition)  # Get query to fetch details
 
     # Read data from Hive
     data_frame = pd.read_sql(query, conn)
 
     # Close the connection
     conn.close()
     return data_frame
 
 
-def get_mysql_df(connection_details, row_count, strategy):
+def get_mysql_df(connection_details, row_count, strategy, filter_condition):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form mysql connection
     """
@@ -181,27 +178,24 @@
 
     conn = pymysql.connect(host=connection_details["params"]["READER"]["host"],
                            port=int(connection_details["params"]["READER"]["port"]),
                            user=connection_details["params"]["READER"]["user"],
                            passwd=connection_details["params"]["READER"]["password"],
                            db=connection_details["params"]["READER"]["database"])
 
-    if int(row_count) > 0:
-        # Generate query
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
-    else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
+    query = get_dataframe_query(connection_details['params']['READER']['tables'],
+                                row_count, filter_condition)  # Get query to fetch details
     # Read data fromm mysql
     data_frame = pd.read_sql(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
 
 
-def get_sqlserver_df(connection_details, row_count, strategy):
+def get_sqlserver_df(connection_details, row_count, strategy, filter_condition):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame from sql server connection
     """
@@ -215,27 +209,24 @@
     conn = pyodbc.connect(f'DRIVER={driver_lib};'
                           f'SERVER={connection_details["params"]["READER"]["host"]};'
                           f'DATABASE={connection_details["params"]["READER"]["database"]};'
                           f'UID={connection_details["params"]["READER"]["user"]};'
                           f'PWD={connection_details["params"]["READER"]["password"]};'
                           f'TrustServerCertificate=yes;')
 
-    if int(row_count) > 0:
-        # Generate query
-        query = f"SELECT TOP {int(row_count)} * FROM {connection_details['params']['READER']['tables']}"
-    else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
+    query = get_dataframe_query(connection_details['params']['READER']['tables'],
+                                row_count, filter_condition, top=True)  # Get query to fetch details
     # Read data from sqlserver
     data_frame = pd.read_sql(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
 
 
-def get_postgres_df(connection_details, row_count, strategy):
+def get_postgres_df(connection_details, row_count, strategy, filter_condition):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form postgres connection
     """
@@ -245,19 +236,17 @@
 
     conn = psycopg2.connect(host=connection_details["params"]["READER"]["host"],
                             port=int(connection_details["params"]["READER"]["port"]),
                             user=connection_details["params"]["READER"]["user"],
                             password=connection_details["params"]["READER"]["password"],
                             database=connection_details["params"]["READER"]["database"])
 
-    if int(row_count) > 0:
-        # Generate query
-        query = f"SELECT * FROM {connection_details['params']['READER']['schema']}.{connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
-    else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['schema']}.{connection_details['params']['READER']['tables']}"
+    query = get_dataframe_query(f"{connection_details['params']['READER']['schema']}."
+                                f"{connection_details['params']['READER']['tables']}",
+                                row_count, filter_condition)  # Get query to fetch details
     # Read data fromm postgres
     data_frame = sqlio.read_sql_query(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
```

### Comparing `refractio-2.0.5.6/refractio/sftp.py` & `refractio-2.0.5.7/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/snowflake.py` & `refractio-2.0.5.7/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio/sqlserver.py` & `refractio-2.0.5.7/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.7/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.6
+Version: 2.0.5.7
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.6/refractio.egg-info/requires.txt` & `refractio-2.0.5.7/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.6/setup.py` & `refractio-2.0.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.6'
+VERSION = '2.0.5.7'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

