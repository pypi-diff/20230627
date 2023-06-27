# Comparing `tmp/abenity-0.0.8.tar.gz` & `tmp/abenity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abenity-0.0.8.tar", last modified: Wed Jan 25 01:12:43 2023, max compression
+gzip compressed data, was "abenity-1.1.0.tar", last modified: Tue Jun 27 17:07:35 2023, max compression
```

## Comparing `abenity-0.0.8.tar` & `abenity-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-01-25 01:12:43.932417 abenity-0.0.8/
--rw-r--r--   0 mark       (501) staff       (20)     1109 2023-01-25 00:47:55.000000 abenity-0.0.8/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)      629 2023-01-25 01:12:43.932071 abenity-0.0.8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      241 2023-01-25 01:10:12.000000 abenity-0.0.8/README.md
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-01-25 01:12:43.929236 abenity-0.0.8/abenity/
--rw-r--r--   0 mark       (501) staff       (20)     1147 2017-11-07 06:46:28.000000 abenity-0.0.8/abenity/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     6472 2022-09-16 19:25:34.000000 abenity-0.0.8/abenity/client.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-01-25 01:12:43.931650 abenity-0.0.8/abenity.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)      629 2023-01-25 01:12:43.000000 abenity-0.0.8/abenity.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      218 2023-01-25 01:12:43.000000 abenity-0.0.8/abenity.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-01-25 01:12:43.000000 abenity-0.0.8/abenity.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       68 2023-01-25 01:12:43.000000 abenity-0.0.8/abenity.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)        8 2023-01-25 01:12:43.000000 abenity-0.0.8/abenity.egg-info/top_level.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-01-25 01:12:43.932529 abenity-0.0.8/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1394 2023-01-25 01:12:15.000000 abenity-0.0.8/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-27 17:07:35.807900 abenity-1.1.0/
+-rw-r--r--   0 mark       (501) staff       (20)     1109 2023-01-25 00:47:55.000000 abenity-1.1.0/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)      629 2023-06-27 17:07:35.807791 abenity-1.1.0/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      241 2023-01-25 01:10:12.000000 abenity-1.1.0/README.md
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-27 17:07:35.806603 abenity-1.1.0/abenity/
+-rw-r--r--   0 mark       (501) staff       (20)     1147 2017-11-07 06:46:28.000000 abenity-1.1.0/abenity/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     6662 2023-06-23 18:03:50.000000 abenity-1.1.0/abenity/client.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-27 17:07:35.807371 abenity-1.1.0/abenity.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)      629 2023-06-27 17:07:35.000000 abenity-1.1.0/abenity.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      236 2023-06-27 17:07:35.000000 abenity-1.1.0/abenity.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-27 17:07:35.000000 abenity-1.1.0/abenity.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       68 2023-06-27 17:07:35.000000 abenity-1.1.0/abenity.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)        8 2023-06-27 17:07:35.000000 abenity-1.1.0/abenity.egg-info/top_level.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-27 17:07:35.807939 abenity-1.1.0/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1394 2023-06-27 17:01:53.000000 abenity-1.1.0/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-27 17:07:35.807494 abenity-1.1.0/tests/
+-rw-r--r--   0 mark       (501) staff       (20)     4373 2022-09-16 19:25:34.000000 abenity-1.1.0/tests/test_sso.py
```

### Comparing `abenity-0.0.8/LICENSE` & `abenity-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abenity-0.0.8/PKG-INFO` & `abenity-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abenity
-Version: 0.0.8
+Version: 1.1.0
 Summary: Abenity API client
 Home-page: https://github.com/abenity/abenity-python
 Author: Abenity
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `abenity-0.0.8/abenity/__init__.py` & `abenity-1.1.0/abenity/__init__.py`

 * *Files identical despite different names*

### Comparing `abenity-0.0.8/abenity/client.py` & `abenity-1.1.0/abenity/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
         if http_method == 'GET':
             response = requests.get(api_url, verify=False, headers=headers,
                                     params=params, timeout=self._timeout)
         elif http_method == 'POST':
             response = requests.post(api_url, verify=False, headers=headers,
                                      data=params, timeout=self._timeout)
+        elif http_method == 'DELETE':
+            response = requests.delete(api_url, verify=False, headers=headers,
+                                     data=params, timeout=self._timeout)
 
         return json.loads(response.text)
 
     def _encrypt_payload(self, payload, iv):
         cipher = DES3.new(six.b(self._triple_des_key),
                           DES3.MODE_CBC,
                           IV=iv)
```

### Comparing `abenity-0.0.8/abenity.egg-info/PKG-INFO` & `abenity-1.1.0/abenity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abenity
-Version: 0.0.8
+Version: 1.1.0
 Summary: Abenity API client
 Home-page: https://github.com/abenity/abenity-python
 Author: Abenity
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `abenity-0.0.8/setup.py` & `abenity-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 setup(
     name='abenity',
     packages=['abenity'],
-    version='0.0.8',
+    version='1.1.0',
 
     description='Abenity API client',
     long_description='A Python library for using the Abenity API.',
     url='https://github.com/abenity/abenity-python',
     author='Abenity',
     license='MIT',
     cmdclass={'test': PyTest},
```

