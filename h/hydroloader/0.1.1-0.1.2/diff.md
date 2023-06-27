# Comparing `tmp/hydroloader-0.1.1.tar.gz` & `tmp/hydroloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroloader-0.1.1.tar", last modified: Fri Jun 23 01:34:46 2023, max compression
+gzip compressed data, was "hydroloader-0.1.2.tar", last modified: Tue Jun 27 20:39:38 2023, max compression
```

## Comparing `hydroloader-0.1.1.tar` & `hydroloader-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.515020 hydroloader-0.1.1/
--rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.1/LICENSE.txt
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-23 01:34:46.515088 hydroloader-0.1.1/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.1/README.md
--rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.1/pyproject.toml
--rw-r--r--   0 klippold   (501) staff       (20)      352 2023-06-23 01:34:46.515375 hydroloader-0.1.1/setup.cfg
--rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.1/setup.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.512218 hydroloader-0.1.1/src/
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.513905 hydroloader-0.1.1/src/hydroloader/
--rw-r--r--   0 klippold   (501) staff       (20)      337 2023-06-13 00:42:46.000000 hydroloader-0.1.1/src/hydroloader/__init__.py
--rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.1/src/hydroloader/exceptions.py
--rw-r--r--   0 klippold   (501) staff       (20)    15287 2023-06-23 00:32:44.000000 hydroloader-0.1.1/src/hydroloader/main.py
--rw-r--r--   0 klippold   (501) staff       (20)     7793 2023-06-22 20:13:42.000000 hydroloader-0.1.1/src/hydroloader/models.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.514757 hydroloader-0.1.1/src/hydroloader.egg-info/
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/SOURCES.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/dependency_links.txt
--rw-r--r--   0 klippold   (501) staff       (20)      101 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/requires.txt
--rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/top_level.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.1/src/hydroloader.egg-info/zip-safe
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-27 20:39:38.193527 hydroloader-0.1.2/
+-rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.2/LICENSE.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-27 20:39:38.193591 hydroloader-0.1.2/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.2/README.md
+-rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.2/pyproject.toml
+-rw-r--r--   0 klippold   (501) staff       (20)      352 2023-06-27 20:39:38.193873 hydroloader-0.1.2/setup.cfg
+-rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.2/setup.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-27 20:39:38.190281 hydroloader-0.1.2/src/
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-27 20:39:38.192391 hydroloader-0.1.2/src/hydroloader/
+-rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.2/src/hydroloader/__init__.py
+-rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.2/src/hydroloader/exceptions.py
+-rw-r--r--   0 klippold   (501) staff       (20)    15287 2023-06-23 00:32:44.000000 hydroloader-0.1.2/src/hydroloader/main.py
+-rw-r--r--   0 klippold   (501) staff       (20)     7934 2023-06-27 18:07:45.000000 hydroloader-0.1.2/src/hydroloader/models.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-27 20:39:38.193266 hydroloader-0.1.2/src/hydroloader.egg-info/
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-27 20:39:38.000000 hydroloader-0.1.2/src/hydroloader.egg-info/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-27 20:39:38.000000 hydroloader-0.1.2/src/hydroloader.egg-info/SOURCES.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-27 20:39:38.000000 hydroloader-0.1.2/src/hydroloader.egg-info/dependency_links.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      101 2023-06-27 20:39:38.000000 hydroloader-0.1.2/src/hydroloader.egg-info/requires.txt
+-rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-27 20:39:38.000000 hydroloader-0.1.2/src/hydroloader.egg-info/top_level.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.2/src/hydroloader.egg-info/zip-safe
```

### Comparing `hydroloader-0.1.1/LICENSE.txt` & `hydroloader-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.1/src/hydroloader/main.py` & `hydroloader-0.1.2/src/hydroloader/main.py`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.1/src/hydroloader/models.py` & `hydroloader-0.1.2/src/hydroloader/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         crontab string is valid. If it's not, an exception will be raised.
 
         :param cls: Pass the class to the function
         :param v: Pass the value of the field to be validated
         :return: The crontab string
         """
 
-        CronTab(v)
+        if v is not None:
+            CronTab(v)
 
         return v
 
 
 class HydroLoaderConfFileAccess(BaseModel):
     path: Optional[str]
     url: Optional[AnyHttpUrl]
@@ -157,18 +158,18 @@
 
         :param cls: Pass in the class of the object being created
         :param v: Pass the timezone offset
         :return: A tzinfo object
         """
 
         tzinfo_pattern = r'^[+-](0[0-9]|1[0-4])[0-5][0-9]$'
-        if re.match(tzinfo_pattern, v) is None:
+        if v is not None and re.match(tzinfo_pattern, v) is None:
             raise ValueError('The offset must be a valid UTC timezone offset formatted such as "+0000".')
 
-        return datetime.strptime(v, '%z').tzinfo
+        return datetime.strptime(v, '%z').tzinfo if v is not None else None
 
 
 class HydroLoaderConfFileDatastream(BaseModel):
     column: Union[conint(gt=0), str]
     datastream_id: UUID
 
 
@@ -178,16 +179,16 @@
     file_timestamp: HydroLoaderConfFileTimestamp
     datastreams: List[HydroLoaderConfFileDatastream]
 
     @root_validator()
     def check_header_and_fields(cls, values):
         """"""
 
-        if not values['file_access'].header_row:
-            if not isinstance(values['file_timestamp'].column, int):
+        if not values.get('file_access') or not values['file_access'].header_row:
+            if values.get('file_timestamp') and not isinstance(values['file_timestamp'].column, int):
                 raise ValueError('If no header row is defined, all column identifiers must be integers.')
             for datastream in values['datastreams']:
                 if not isinstance(datastream.column, int):
                     raise ValueError('If no header row is defined, all column identifiers must be integers.')
 
         return values
```

