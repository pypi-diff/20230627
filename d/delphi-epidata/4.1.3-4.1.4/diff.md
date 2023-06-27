# Comparing `tmp/delphi_epidata-4.1.3.tar.gz` & `tmp/delphi_epidata-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-4.1.3.tar", last modified: Tue Jun 13 14:54:48 2023, max compression
+gzip compressed data, was "delphi_epidata-4.1.4.tar", last modified: Tue Jun 27 18:28:15 2023, max compression
```

## Comparing `delphi_epidata-4.1.3.tar` & `delphi_epidata-4.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:54:48.315045 delphi_epidata-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-13 14:54:36.000000 delphi_epidata-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 14:54:48.315045 delphi_epidata-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 14:54:36.000000 delphi_epidata-4.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:54:48.315045 delphi_epidata-4.1.3/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-13 14:54:36.000000 delphi_epidata-4.1.3/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25286 2023-06-13 14:54:47.000000 delphi_epidata-4.1.3/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:54:48.315045 delphi_epidata-4.1.3/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 14:54:48.000000 delphi_epidata-4.1.3/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 14:54:48.000000 delphi_epidata-4.1.3/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:54:48.000000 delphi_epidata-4.1.3/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 14:54:48.000000 delphi_epidata-4.1.3/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 14:54:48.000000 delphi_epidata-4.1.3/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:54:48.315045 delphi_epidata-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-13 14:54:36.000000 delphi_epidata-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.218568 delphi_epidata-4.1.4/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-06-27 18:28:14.000000 delphi_epidata-4.1.4/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/setup.py
```

### Comparing `delphi_epidata-4.1.3/LICENSE` & `delphi_epidata-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.3/PKG-INFO` & `delphi_epidata-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi_epidata
-Version: 4.1.3
+Version: 4.1.4
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.3/delphi_epidata/delphi_epidata.py` & `delphi_epidata-4.1.4/delphi_epidata/delphi_epidata.py`

 * *Files 5% similar despite different names*

```diff
@@ -390,70 +390,14 @@
     params = {
       'endpoint': 'meta_norostat',
       'auth': auth,
     }
     # Make the API call
     return Epidata._request(params)
 
-  # Fetch AFHSB data
-  @staticmethod
-  def afhsb(auth, locations, epiweeks, flu_types):
-    """Fetch AFHSB data (point data, no min/max)."""
-    # Check parameters
-    if auth is None or locations is None or epiweeks is None or flu_types is None:
-      raise Exception('`auth`, `locations`, `epiweeks` and `flu_types` are all required')
-
-    loc_exception = 'Location parameter  `{}` is invalid. Valid `location` parameters are: '\
-      '`hhs[1-10]`, `cen[1-9]`, 2-letter state code or 3-letter country code.'
-    for location in locations:
-      location = location.lower()
-      if (location.startswith('hhs') or location.startswith('cen')):
-        prefix, postfix = location[:3], location[3:]
-        if (postfix.isnumeric()):
-          region_num = int(postfix)
-          if (region_num < 1 or region_num > 10 or (region_num == 10 and prefix == 'cen')):
-            raise Exception(loc_exception.format(location))
-        else:
-          raise Exception(loc_exception.format(location))
-      elif (len(location) < 2 or len(location) > 3):
-        raise Exception(loc_exception.format(location))
-
-    flu_exception = 'Flu-type parameters `{}` is invalid. Valid flu-type parameters are: '\
-      '`flu1`, `flu2`, `flu3`, `ili`, `flu2-flu1`, `flu3-flu2`, `ili-flu3`.'
-    valid_flu_types = ['flu1', 'flu2', 'flu3', 'ili', 'flu2-flu1', 'flu3-flu2', 'ili-flu3']
-    for flu_type in flu_types:
-      if (not flu_type in valid_flu_types):
-        raise Exception(flu_exception.format(flu_type))
-
-    # Set up request
-    params = {
-      'endpoint': 'afhsb',
-      'auth': auth,
-      'locations': Epidata._list(locations),
-      'epiweeks': Epidata._list(epiweeks),
-      'flu_types': Epidata._list(flu_types)
-    }
-    # Make the API call
-    return Epidata._request(params)
-
-  # Fetch AFHSB metadata
-  @staticmethod
-  def meta_afhsb(auth):
-    """Fetch AFHSB metadata."""
-    # Check parameters
-    if auth is None:
-      raise Exception('`auth` is required')
-    # Set up request
-    params = {
-      'endpoint': 'meta_afhsb',
-      'auth': auth,
-    }
-    # Make the API call
-    return Epidata._request(params)
-
   # Fetch NIDSS flu data
   @staticmethod
   def nidss_flu(regions, epiweeks, issues=None, lag=None):
     """Fetch NIDSS flu data."""
     # Check parameters
     if regions is None or epiweeks is None:
       raise Exception('`regions` and `epiweeks` are both required')
```

### Comparing `delphi_epidata-4.1.3/delphi_epidata.egg-info/PKG-INFO` & `delphi_epidata-4.1.4/delphi_epidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi-epidata
-Version: 4.1.3
+Version: 4.1.4
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.3/setup.py` & `delphi_epidata-4.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="4.1.3",
+    version="4.1.4",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```

