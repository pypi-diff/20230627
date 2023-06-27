# Comparing `tmp/openai-image-1.0.3.tar.gz` & `tmp/openai-image-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-image-1.0.3.tar", last modified: Tue Jun 27 07:16:39 2023, max compression
+gzip compressed data, was "openai-image-1.0.4.tar", last modified: Tue Jun 27 07:22:13 2023, max compression
```

## Comparing `openai-image-1.0.3.tar` & `openai-image-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:16:39.554251 openai-image-1.0.3/
--rw-rw-rw-   0        0        0     1100 2023-06-23 06:27:04.000000 openai-image-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1974 2023-06-27 07:16:39.555256 openai-image-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2023-06-27 07:14:12.000000 openai-image-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:16:39.426259 openai-image-1.0.3/openai_image/
--rw-rw-rw-   0        0        0       96 2023-06-26 17:52:32.000000 openai-image-1.0.3/openai_image/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-06-26 17:54:42.000000 openai-image-1.0.3/openai_image/main.py
--rw-rw-rw-   0        0        0      187 2023-06-26 16:28:03.000000 openai-image-1.0.3/openai_image/settings.py
--rw-rw-rw-   0        0        0      162 2023-06-26 16:28:11.000000 openai-image-1.0.3/openai_image/settings_sample.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:16:39.540260 openai-image-1.0.3/openai_image.egg-info/
--rw-rw-rw-   0        0        0     1974 2023-06-27 07:16:38.000000 openai-image-1.0.3/openai_image.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-27 07:16:38.000000 openai-image-1.0.3/openai_image.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:16:38.000000 openai-image-1.0.3/openai_image.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 07:16:38.000000 openai-image-1.0.3/openai_image.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 07:16:38.000000 openai-image-1.0.3/openai_image.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 07:16:39.567257 openai-image-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-06-27 07:15:44.000000 openai-image-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.348175 openai-image-1.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-06-23 06:27:04.000000 openai-image-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1974 2023-06-27 07:22:13.349177 openai-image-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2023-06-27 07:22:07.000000 openai-image-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.285177 openai-image-1.0.4/openai_image/
+-rw-rw-rw-   0        0        0       96 2023-06-26 17:52:32.000000 openai-image-1.0.4/openai_image/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-06-26 17:54:42.000000 openai-image-1.0.4/openai_image/main.py
+-rw-rw-rw-   0        0        0      187 2023-06-26 16:28:03.000000 openai-image-1.0.4/openai_image/settings.py
+-rw-rw-rw-   0        0        0      162 2023-06-26 16:28:11.000000 openai-image-1.0.4/openai_image/settings_sample.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.346180 openai-image-1.0.4/openai_image.egg-info/
+-rw-rw-rw-   0        0        0     1974 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:22:13.352175 openai-image-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-06-27 07:21:19.000000 openai-image-1.0.4/setup.py
```

### Comparing `openai-image-1.0.3/LICENSE` & `openai-image-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-image-1.0.3/PKG-INFO` & `openai-image-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: openai-image
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python script for generating image from text by Open AI
 Home-page: https://github.com/IgorMan2005/openai_image/
 Author: IgorMan
 Author-email: igorman2005@gmail.com
-Project-URL: Documentation, https://best-itpro.ru/openai_image
+Project-URL: Documentation, https://best-itpro.ru/news/openai_image/
 Keywords: openai image api open ai python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai_image
 Python script for generating image from text by Open AI
 
 
-<image src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
+<img src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
 
 
 **1. Install openai & openai-image**
 
 
 ```
 pip install openai
@@ -71,30 +71,30 @@
 import openai_image
 
 openai_image.get_image()
 
 ```
 Prompt target text: **blue bird**
 
-<image src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
+<img src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
 
 Your image file ready: **/images/blue_bird.jpg**
 
 
 
 *Example2:*
 
 ```
 import openai_image
 
 openai_image.get_image('Alice in Wonderland')
 
 ```
 
-<image src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
+<img src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
 
 Your image file ready: **/images/Alice_in_Wonderland.jpg**
 
 
 ### Documentation
 
 https://best-itpro.ru/news/openai_image/
```

### Comparing `openai-image-1.0.3/README.md` & `openai-image-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # openai_image
 Python script for generating image from text by Open AI
 
 
-<image src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
+<img src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
 
 
 **1. Install openai & openai-image**
 
 
 ```
 pip install openai
@@ -55,30 +55,30 @@
 import openai_image
 
 openai_image.get_image()
 
 ```
 Prompt target text: **blue bird**
 
-<image src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
+<img src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
 
 Your image file ready: **/images/blue_bird.jpg**
 
 
 
 *Example2:*
 
 ```
 import openai_image
 
 openai_image.get_image('Alice in Wonderland')
 
 ```
 
-<image src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
+<img src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
 
 Your image file ready: **/images/Alice_in_Wonderland.jpg**
 
 
 ### Documentation
 
 https://best-itpro.ru/news/openai_image/
```

### Comparing `openai-image-1.0.3/openai_image/main.py` & `openai-image-1.0.4/openai_image/main.py`

 * *Files identical despite different names*

### Comparing `openai-image-1.0.3/openai_image.egg-info/PKG-INFO` & `openai-image-1.0.4/openai_image.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: openai-image
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python script for generating image from text by Open AI
 Home-page: https://github.com/IgorMan2005/openai_image/
 Author: IgorMan
 Author-email: igorman2005@gmail.com
-Project-URL: Documentation, https://best-itpro.ru/openai_image
+Project-URL: Documentation, https://best-itpro.ru/news/openai_image/
 Keywords: openai image api open ai python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai_image
 Python script for generating image from text by Open AI
 
 
-<image src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
+<img src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
 
 
 **1. Install openai & openai-image**
 
 
 ```
 pip install openai
@@ -71,30 +71,30 @@
 import openai_image
 
 openai_image.get_image()
 
 ```
 Prompt target text: **blue bird**
 
-<image src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
+<img src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
 
 Your image file ready: **/images/blue_bird.jpg**
 
 
 
 *Example2:*
 
 ```
 import openai_image
 
 openai_image.get_image('Alice in Wonderland')
 
 ```
 
-<image src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
+<img src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
 
 Your image file ready: **/images/Alice_in_Wonderland.jpg**
 
 
 ### Documentation
 
 https://best-itpro.ru/news/openai_image/
```

### Comparing `openai-image-1.0.3/setup.py` & `openai-image-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='openai-image',
-  version='1.0.3',
+  version='1.0.4',
   author='IgorMan',
   author_email='igorman2005@gmail.com',
   description='Python script for generating image from text by Open AI',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/IgorMan2005/openai_image/',
   packages=['openai_image'],
@@ -18,11 +18,11 @@
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='openai image api open ai python',
   project_urls={
-    'Documentation': 'https://best-itpro.ru/openai_image',
+    'Documentation': 'https://best-itpro.ru/news/openai_image/',
   },
   python_requires='>=3.6'
 )
```

