# Comparing `tmp/aws-s3-cli-0.0.3.tar.gz` & `tmp/aws-s3-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-s3-cli-0.0.3.tar", last modified: Mon Jun 26 17:47:20 2023, max compression
+gzip compressed data, was "aws-s3-cli-0.0.4.tar", last modified: Tue Jun 27 15:11:29 2023, max compression
```

## Comparing `aws-s3-cli-0.0.3.tar` & `aws-s3-cli-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 17:47:20.454187 aws-s3-cli-0.0.3/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.3/LICENSE
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.3/MANIFEST.in
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2778 2023-06-26 17:47:20.454187 aws-s3-cli-0.0.3/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1987 2023-06-26 17:45:55.000000 aws-s3-cli-0.0.3/README.md
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 17:47:20.454187 aws-s3-cli-0.0.3/aws_s3_cli/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     4694 2023-06-26 16:11:13.000000 aws-s3-cli-0.0.3/aws_s3_cli/aws_s3_cli.py
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 17:47:20.454187 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2778 2023-06-26 17:47:20.000000 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-06-26 17:47:20.000000 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-06-26 17:47:20.000000 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-06-26 17:47:20.000000 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/requires.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-06-26 17:47:20.000000 aws-s3-cli-0.0.3/aws_s3_cli.egg-info/top_level.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-06-26 17:47:20.454187 aws-s3-cli-0.0.3/setup.cfg
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-06-26 17:47:11.000000 aws-s3-cli-0.0.3/setup.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.4/LICENSE
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.4/MANIFEST.in
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2885 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2095 2023-06-27 15:11:08.000000 aws-s3-cli-0.0.4/README.md
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/aws_s3_cli/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     4694 2023-06-26 16:11:13.000000 aws-s3-cli-0.0.4/aws_s3_cli/aws_s3_cli.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2885 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/requires.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/top_level.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/setup.cfg
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-06-27 15:11:00.000000 aws-s3-cli-0.0.4/setup.py
```

### Comparing `aws-s3-cli-0.0.3/LICENSE` & `aws-s3-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.3/PKG-INFO` & `aws-s3-cli-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## aws-s3-cli :
-[![Downloads](https://static.pepy.tech/badge/aws-s3-cli)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-s3-cli?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
 
 
 ```
 aws s3 bucket cli
 
 upload, download, check file availability, and get all available list from AWS s3 bucket.
 ```
```

### Comparing `aws-s3-cli-0.0.3/README.md` & `aws-s3-cli-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## aws-s3-cli :
-[![Downloads](https://static.pepy.tech/badge/aws-s3-cli)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-s3-cli?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
 
 
 ```
 aws s3 bucket cli
 
 upload, download, check file availability, and get all available list from AWS s3 bucket.
 ```
@@ -72,8 +72,8 @@
 ## Author:
 Sujit Mandal
 
 [GitHub](https://github.com/sujitmandal)
 
 [PyPi](https://pypi.org/user/sujitmandal/)
 
-[LinkedIn](https://www.linkedin.com/in/sujit-mandal-91215013a/)
+[LinkedIn](https://www.linkedin.com/in/sujit-mandal-91215013a/)
```

### Comparing `aws-s3-cli-0.0.3/aws_s3_cli/aws_s3_cli.py` & `aws-s3-cli-0.0.4/aws_s3_cli/aws_s3_cli.py`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.3/aws_s3_cli.egg-info/PKG-INFO` & `aws-s3-cli-0.0.4/aws_s3_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## aws-s3-cli :
-[![Downloads](https://static.pepy.tech/badge/aws-s3-cli)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-s3-cli?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
 
 
 ```
 aws s3 bucket cli
 
 upload, download, check file availability, and get all available list from AWS s3 bucket.
 ```
```

### Comparing `aws-s3-cli-0.0.3/setup.py` & `aws-s3-cli-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md') as files:
         README = files.read()
 
     return(README)
 
 setup(
     name = 'aws-s3-cli',
-    version = '0.0.3',
+    version = '0.0.4',
     description = "upload, download, check file availability, and get all available list from AWS s3 bucket.",
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/sujitmandal/aws-s3-cli',
     author = 'Sujit Mandal',
     author_email = 'mandals974@gmail.com',
     license = 'MIT',
```

