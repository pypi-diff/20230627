# Comparing `tmp/aws-ssm-copy-0.5.1.tar.gz` & `tmp/aws-ssm-copy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ssm-copy-0.5.1.tar", last modified: Tue May 30 09:58:51 2023, max compression
+gzip compressed data, was "aws-ssm-copy-0.5.2.tar", last modified: Tue Jun 27 14:16:58 2023, max compression
```

## Comparing `aws-ssm-copy-0.5.1.tar` & `aws-ssm-copy-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:58:51.180272 aws-ssm-copy-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-30 09:58:51.180272 aws-ssm-copy-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:58:51.180272 aws-ssm-copy-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:58:51.176272 aws-ssm-copy-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:58:51.176272 aws-ssm-copy-0.5.1/src/aws_ssm_copy/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12050 2023-05-30 09:58:48.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy/ssm_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:58:51.180272 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:58:50.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 09:58:51.000000 aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/src/aws_ssm_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12173 2023-06-27 14:16:56.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy/ssm_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:16:58.694179 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 14:16:58.000000 aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/top_level.txt
```

### Comparing `aws-ssm-copy-0.5.1/LICENSE` & `aws-ssm-copy-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ssm-copy-0.5.1/PKG-INFO` & `aws-ssm-copy-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-copy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Copy AWS Parameter Store parameters
 Home-page: https://github.com/binxio/aws-ssm-copy
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: UNKNOWN
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `aws-ssm-copy-0.5.1/README.md` & `aws-ssm-copy-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `aws-ssm-copy-0.5.1/setup.py` & `aws-ssm-copy-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
-version = "0.5.1"
+version = "0.5.2"
 
 setup(
     name='aws-ssm-copy',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     entry_points={
         'console_scripts': ['aws-ssm-copy = aws_ssm_copy:main']
```

### Comparing `aws-ssm-copy-0.5.1/src/aws_ssm_copy/ssm_copy.py` & `aws-ssm-copy-0.5.2/src/aws_ssm_copy/ssm_copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,19 +114,22 @@
         """
         source_tag_list = self.source_ssm.list_tags_for_resource(
             ResourceType='Parameter',
             ResourceId=name
         )['TagList']
         source_tags = {tag['Key']: tag['Value'] for tag in source_tag_list}
 
-        existing_tags_list = self.target_ssm.list_tags_for_resource(
-            ResourceType='Parameter',
-            ResourceId=new_name
-        )['TagList']
-        target_tags = {tag['Key']: tag['Value'] for tag in existing_tags_list}
+        try:
+            existing_tags_list = self.target_ssm.list_tags_for_resource(
+                ResourceType='Parameter',
+                ResourceId=new_name
+            )['TagList']
+            target_tags = {tag['Key']: tag['Value'] for tag in existing_tags_list}
+        except self.target_ssm.exceptions.InvalidResourceId:
+            target_tags = {}
 
         to_remove = list(filter(lambda key: key not in source_tags, target_tags.keys()))
         to_add = list(filter(lambda key: key not in target_tags or source_tags[key] != target_tags[key], source_tags.keys()))
         if to_remove:
 
             if self.dry_run:
                 sys.stdout.write(f"DRY-RUN: remove tags {','.join(to_remove)} from {new_name}\n")
```

### Comparing `aws-ssm-copy-0.5.1/src/aws_ssm_copy.egg-info/PKG-INFO` & `aws-ssm-copy-0.5.2/src/aws_ssm_copy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-copy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Copy AWS Parameter Store parameters
 Home-page: https://github.com/binxio/aws-ssm-copy
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: UNKNOWN
 Platform: any
 Description-Content-Type: text/markdown
```

