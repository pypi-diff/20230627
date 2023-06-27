# Comparing `tmp/pythclient-0.1.7.tar.gz` & `tmp/pythclient-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythclient-0.1.7.tar", last modified: Thu Jun 22 09:41:13 2023, max compression
+gzip compressed data, was "pythclient-0.1.8.tar", last modified: Tue Jun 27 08:20:45 2023, max compression
```

## Comparing `pythclient-0.1.7.tar` & `pythclient-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-22 09:40:59.000000 pythclient-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-22 09:41:13.429975 pythclient-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-22 09:40:59.000000 pythclient-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-22 09:40:59.000000 pythclient-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/pythclient/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/pythaccounts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/pythclient.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/pythclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 09:41:13.429975 pythclient-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-22 09:40:59.000000 pythclient-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    11068 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_mapping_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_account_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_product_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_pyth_account.py
--rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_pyth_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_solana_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.933852 pythclient-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-27 08:20:27.000000 pythclient-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-27 08:20:45.933852 pythclient-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-27 08:20:27.000000 pythclient-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 08:20:27.000000 pythclient-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.929852 pythclient-0.1.8/pythclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/pythaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/pythclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.929852 pythclient-0.1.8/pythclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 08:20:45.933852 pythclient-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-27 08:20:27.000000 pythclient-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.933852 pythclient-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8432 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_mapping_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_account_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_product_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_pyth_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_pyth_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_solana_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_utils.py
```

### Comparing `pythclient-0.1.7/LICENSE` & `pythclient-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/PKG-INFO` & `pythclient-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.7/README.md` & `pythclient-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/calendar.py` & `pythclient-0.1.8/pythclient/calendar.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/exceptions.py` & `pythclient-0.1.8/pythclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/pythaccounts.py` & `pythclient-0.1.8/pythclient/pythaccounts.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/pythclient.py` & `pythclient-0.1.8/pythclient/pythclient.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/ratelimit.py` & `pythclient-0.1.8/pythclient/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/solana.py` & `pythclient-0.1.8/pythclient/solana.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient/utils.py` & `pythclient-0.1.8/pythclient/utils.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/pythclient.egg-info/PKG-INFO` & `pythclient-0.1.8/pythclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.7/pythclient.egg-info/SOURCES.txt` & `pythclient-0.1.8/pythclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/setup.py` & `pythclient-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiodns', 'aiohttp>=3.7.4', 'backoff', 'base58', 'dnspython', 'flake8', 'loguru', 'typing-extensions', 'pytz']
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pythclient',
-    version='0.1.7',
+    version='0.1.8',
     packages=['pythclient'],
     author='Pyth Developers',
     author_email='contact@pyth.network',
     description='A library to retrieve Pyth account structures off the Solana blockchain.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pyth-network/pyth-client-py',
```

### Comparing `pythclient-0.1.7/tests/test_mapping_account.py` & `pythclient-0.1.8/tests/test_mapping_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_price_account.py` & `pythclient-0.1.8/tests/test_price_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_price_account_header.py` & `pythclient-0.1.8/tests/test_price_account_header.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_price_component.py` & `pythclient-0.1.8/tests/test_price_component.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_price_info.py` & `pythclient-0.1.8/tests/test_price_info.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_product_account.py` & `pythclient-0.1.8/tests/test_product_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_pyth_account.py` & `pythclient-0.1.8/tests/test_pyth_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_pyth_client.py` & `pythclient-0.1.8/tests/test_pyth_client.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_solana_account.py` & `pythclient-0.1.8/tests/test_solana_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.7/tests/test_utils.py` & `pythclient-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

