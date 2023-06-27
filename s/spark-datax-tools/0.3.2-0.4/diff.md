# Comparing `tmp/spark_datax_tools-0.3.2.tar.gz` & `tmp/spark_datax_tools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_datax_tools-0.3.2.tar", last modified: Sun Jun 25 06:15:11 2023, max compression
+gzip compressed data, was "spark_datax_tools-0.4.tar", last modified: Tue Jun 27 12:07:24 2023, max compression
```

## Comparing `spark_datax_tools-0.3.2.tar` & `spark_datax_tools-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.868221 spark_datax_tools-0.3.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4266 2023-06-25 06:15:11.868221 spark_datax_tools-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.3.2/README.md
--rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-25 06:15:11.869223 spark_datax_tools-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-25 06:08:46.000000 spark_datax_tools-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.826899 spark_datax_tools-0.3.2/spark_datax_tools/
--rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.3.2/spark_datax_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.857803 spark_datax_tools-0.3.2/spark_datax_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/spark_datax_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    50486 2023-06-17 22:17:00.000000 spark_datax_tools-0.3.2/spark_datax_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.866805 spark_datax_tools-0.3.2/spark_datax_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.866805 spark_datax_tools-0.3.2/spark_datax_tools/utils/files/
--rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/files/ns.csv
--rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.3.2/spark_datax_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 06:15:11.849801 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/
--rw-rw-rw-   0        0        0     4266 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-25 06:15:11.000000 spark_datax_tools-0.3.2/spark_datax_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4264 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.4/README.md
+-rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-06-27 12:07:00.000000 spark_datax_tools-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.744099 spark_datax_tools-0.4/spark_datax_tools/
+-rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.4/spark_datax_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.759726 spark_datax_tools-0.4/spark_datax_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/spark_datax_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    43876 2023-06-27 12:06:38.000000 spark_datax_tools-0.4/spark_datax_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.775353 spark_datax_tools-0.4/spark_datax_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/spark_datax_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.4/spark_datax_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/spark_datax_tools/utils/files/
+-rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_datax_tools-0.4/spark_datax_tools/utils/files/ns.csv
+-rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.4/spark_datax_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.759726 spark_datax_tools-0.4/spark_datax_tools.egg-info/
+-rw-rw-rw-   0        0        0     4264 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/top_level.txt
```

### Comparing `spark_datax_tools-0.3.2/LICENSE` & `spark_datax_tools-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/PKG-INFO` & `spark_datax_tools-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_datax_tools
-Version: 0.3.2
+Version: 0.4
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.2/README.md` & `spark_datax_tools-0.4/README.md`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/pyproject.toml` & `spark_datax_tools-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/setup.py` & `spark_datax_tools-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_datax_tools',
     packages=find_packages(),
-    version='0.3.2',
+    version='0.4',
     description='spark_datax_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_datax_tools/',
     download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
```

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools/__init__.py` & `spark_datax_tools-0.4/spark_datax_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools/functions/generator.py` & `spark_datax_tools-0.4/spark_datax_tools/functions/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -953,160 +953,18 @@
                 service = ""
                 user = ""
                 password = ""
 
                 if name_adapter.upper() == "PERU":
                     host = "118.180.35.45" if is_dev else "118.180.61.137"
                     port = "1521"
-                    service = "tst12c"
+                    service = "tst12c" if is_dev else "ora12c"
                     user = "Credencial lo agrega el aplicativo"
                     password = "Credencial lo agrega el aplicativo"
 
                 parameters = dict(uuaa=uuaa, ns=ns, adapter_id=adapter_id,
                                   connection_id=connection_id,
                                   adapter_description=adapter_description,
                                   host=host, port=port, service=service,
                                   user=user, password=password)
                 generated_structure_ticket(origen="ORACLE", params=parameters, is_dev=is_dev)
 
-# def generate_parquet_spark(spark=None,
-#                            df=None,
-#                            table_name=None,
-#                            spark_schema=None,
-#                            spark_schema_string=None,
-#                            directory_output=None,
-#                            sample_parquet=None,
-#                            columns_string_default={},
-#                            columns_date_default={},
-#                            columns_decimal_default={},
-#                            columns_integer_default={}
-#                            ):
-#     if not spark:
-#         raise Exception(f'require object spark: {spark} ')
-#
-#     if not isinstance(df, pd.DataFrame):
-#         raise Exception('require var df: {df} ')
-#
-#     if not table_name:
-#         raise Exception(f'require var table_name: {table_name} ')
-#
-#     if not spark_schema:
-#         raise Exception(f'require var spark_schema: {spark_schema} ')
-#
-#     import random
-#     import string
-#     from datetime import datetime
-#     from dateutil.relativedelta import relativedelta
-#     from faker import Faker
-#     from pyspark.sql import functions as func
-#
-#     fake = Faker()
-#
-#     df = df[df["table"] == f'{table_name}']
-#
-#     output2 = list()
-#     for _ in range(sample_parquet):
-#         columns_dict = dict()
-#
-#         for index, row in df.iterrows():
-#             naming = str(row['naming']).lower().strip()
-#             _format = row['format']
-#             if str(_format).upper() == "TIME":
-#                 _format = "ALPHANUMERIC(8)"
-#             _spark_format = spark_transform_dtype(format=_format)
-#             _parentheses = extract_only_parentesis(format=_format)
-#
-#             _fake = None
-#             if _spark_format in ("INTEGER",):
-#                 _fake = fake.pyint(min_value=0, max_value=9999)
-#                 if naming in list(columns_integer_default.keys()):
-#                     new_int = int(columns_integer_default[naming])
-#                     _fake = fake.pyint(min_value=new_int, max_value=new_int)
-#
-#             elif _spark_format in ("TIMESTAMP",):
-#                 d2 = datetime.now()
-#                 d1 = d2 - relativedelta(months=6)
-#                 _fake = fake.date_time_between(start_date=d1, end_date=d2)
-#             elif _spark_format in ("DECIMAL",):
-#                 _parentheses_split = str(_parentheses).split(",")
-#                 if len(_parentheses_split) <= 1:
-#                     _decimal_left = int(_parentheses_split[0])
-#                     _decimal_right = 0
-#                 else:
-#                     _decimal_left = int(_parentheses_split[0])
-#                     _decimal_right = int(_parentheses_split[1])
-#
-#                 min_value_left = int("1" * (_decimal_left - _decimal_right))
-#                 max_value_left = int("9" * (_decimal_left - _decimal_right))
-#
-#                 if _decimal_right == 0:
-#                     _decimal_right2 = 1
-#                     min_value_right = int("0" * _decimal_right2)
-#                     max_value_right = int("0" * _decimal_right2)
-#                 else:
-#                     _decimal_right2 = _decimal_right
-#                     min_value_right = int("1" * _decimal_right2)
-#                     max_value_right = int("9" * _decimal_right2)
-#
-#                 _fake = str(fake.pydecimal(left_digits=_decimal_left,
-#                                            right_digits=_decimal_right,
-#                                            positive=True,
-#                                            min_value=min_value_left,
-#                                            max_value=max_value_left))
-#
-#                 if naming in list(columns_decimal_default.keys()):
-#                     new_decimal = float(columns_decimal_default[naming])
-#                     _fake = fake.bothify(text=f'{new_decimal}')
-#
-#             elif _spark_format in ("TIME",):
-#                 _fake = fake.time()
-#             elif _spark_format in ("DATE",):
-#                 if naming in list(columns_date_default.keys()):
-#                     new_text = columns_date_default[naming]
-#                     _fake = datetime.strptime(new_text, '%Y-%m-%d')
-#                 else:
-#                     d2 = datetime.today()
-#                     d1 = d2 - relativedelta(months=6)
-#                     _fake = fake.date_between(start_date=d1, end_date=d2)
-#             elif _spark_format in ("STRING", "DATE"):
-#                 if naming in ("g_entific_id",):
-#                     _fake = fake.bothify(text='PE')
-#                 elif naming in ("gf_frequency_type", "frequency_type"):
-#                     _fake = fake.bothify(text='?', letters='DM')
-#                 elif naming in list(columns_string_default.keys()):
-#                     new_text = columns_string_default[naming]
-#                     _fake = fake.bothify(text=new_text)
-#                 else:
-#                     _fake = ''.join(random.choices(string.ascii_letters + string.digits, k=int(_parentheses)))
-#             columns_dict[naming] = _fake
-#         output2.append(columns_dict)
-#     df2 = pd.DataFrame(output2)
-#
-#     df3 = spark.createDataFrame(df2, schema=spark_schema_string)
-#
-#     for i in spark_schema.jsonValue()["fields"]:
-#         column_name = str(i["name"])
-#         column_type = str(i["type"])
-#         if column_type.startswith("decimal"):
-#             df3 = df3.withColumn(f"{column_name}", func.col(f"{column_name}").cast(f"{column_type}"))
-#         elif column_type.startswith("date"):
-#             df3 = df3.withColumn(f"{column_name}", func.col(f"{column_name}").cast("date"))
-#         elif column_type.startswith("timestamp"):
-#             df3 = df3.withColumn(f"{column_name}", func.col(f"{column_name}").cast("timestamp"))
-#
-#     df3.coalesce(1).write.mode("overwrite").parquet(f'{directory_output}/{table_name}/dummy_{table_name}.parquet')
-#
-#     return df3
-#
-#
-# def generate_components(spark=None,
-#                         path_excel=None,
-#                         uuaa_name=None,
-#                         table_name=None,
-#                         schema_datax_version="0",
-#                         directory_output="schema_dev_summary",
-#                         sample_parquet=500,
-#                         columns_string_default={},
-#                         columns_date_default={},
-#                         columns_decimal_default={},
-#                         columns_integer_default={}):
-#     pass
```

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools/utils/files/ns.csv` & `spark_datax_tools-0.4/spark_datax_tools/utils/files/ns.csv`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools/utils/utils.py` & `spark_datax_tools-0.4/spark_datax_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools.egg-info/PKG-INFO` & `spark_datax_tools-0.4/spark_datax_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-datax-tools
-Version: 0.3.2
+Version: 0.4
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.2/spark_datax_tools.egg-info/SOURCES.txt` & `spark_datax_tools-0.4/spark_datax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

