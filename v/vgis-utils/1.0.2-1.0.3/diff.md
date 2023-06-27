# Comparing `tmp/vgis_utils-1.0.2.tar.gz` & `tmp/vgis_utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.2.tar", last modified: Tue Jun 27 08:33:22 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.3.tar", last modified: Tue Jun 27 08:48:40 2023, max compression
```

## Comparing `vgis_utils-1.0.2.tar` & `vgis_utils-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:33:22.655262 vgis_utils-1.0.2/
--rw-rw-rw-   0        0        0     1034 2023-06-27 08:33:22.655262 vgis_utils-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:33:22.656294 vgis_utils-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2163 2023-06-27 08:29:35.000000 vgis_utils-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:33:22.653264 vgis_utils-1.0.2/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-06-27 08:33:22.000000 vgis_utils-1.0.2/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-06-27 08:33:22.000000 vgis_utils-1.0.2/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:33:22.000000 vgis_utils-1.0.2/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 08:33:22.000000 vgis_utils-1.0.2/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:33:22.000000 vgis_utils-1.0.2/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:40.005745 vgis_utils-1.0.3/
+-rw-rw-rw-   0        0        0     1034 2023-06-27 08:48:40.004746 vgis_utils-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:48:40.005745 vgis_utils-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2174 2023-06-27 08:42:14.000000 vgis_utils-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.964749 vgis_utils-1.0.3/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.3/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.3/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.977748 vgis_utils-1.0.3/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     7416 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.980747 vgis_utils-1.0.3/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8353 2023-06-27 08:29:36.000000 vgis_utils-1.0.3/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.983747 vgis_utils-1.0.3/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.3/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.986746 vgis_utils-1.0.3/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.3/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.991748 vgis_utils-1.0.3/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.3/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.995772 vgis_utils-1.0.3/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13669 2023-06-27 08:26:45.000000 vgis_utils-1.0.3/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.998772 vgis_utils-1.0.3/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     1436 2023-06-27 06:19:39.000000 vgis_utils-1.0.3/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:40.002767 vgis_utils-1.0.3/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.3/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.973749 vgis_utils-1.0.3/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.2/PKG-INFO` & `vgis_utils-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.2/setup.py` & `vgis_utils-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3.9
 # -*- coding: utf-8 -*-
 # @Time    :  2023/6/27 14:35
 # @Author  : chenxw
 # @Email   : gisfanmachel@gmail.com
 # @File    : setup.py
-# @Descr   : 
+# @Descr   : 安装文档
 # @Software: PyCharm
 
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.2",  # Required 发布版本号
+    version="1.0.3",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -42,15 +42,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 
-    keywords="utils,setuptools, development",  # Optional 搜索关键字
+    keywords="utils,setuptools,development",  # Optional 搜索关键字
 
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
     install_requires=["opencv-python","Pillow","numpy"],  # Optional 第三方依赖库
```

### Comparing `vgis_utils-1.0.2/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.3/vgis_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

