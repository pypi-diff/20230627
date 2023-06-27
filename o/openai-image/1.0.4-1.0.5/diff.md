# Comparing `tmp/openai-image-1.0.4.tar.gz` & `tmp/openai-image-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-image-1.0.4.tar", last modified: Tue Jun 27 07:22:13 2023, max compression
+gzip compressed data, was "openai-image-1.0.5.tar", last modified: Tue Jun 27 17:57:22 2023, max compression
```

## Comparing `openai-image-1.0.4.tar` & `openai-image-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.348175 openai-image-1.0.4/
--rw-rw-rw-   0        0        0     1100 2023-06-23 06:27:04.000000 openai-image-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1974 2023-06-27 07:22:13.349177 openai-image-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-06-27 07:22:07.000000 openai-image-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.285177 openai-image-1.0.4/openai_image/
--rw-rw-rw-   0        0        0       96 2023-06-26 17:52:32.000000 openai-image-1.0.4/openai_image/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-06-26 17:54:42.000000 openai-image-1.0.4/openai_image/main.py
--rw-rw-rw-   0        0        0      187 2023-06-26 16:28:03.000000 openai-image-1.0.4/openai_image/settings.py
--rw-rw-rw-   0        0        0      162 2023-06-26 16:28:11.000000 openai-image-1.0.4/openai_image/settings_sample.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:22:13.346180 openai-image-1.0.4/openai_image.egg-info/
--rw-rw-rw-   0        0        0     1974 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 07:22:12.000000 openai-image-1.0.4/openai_image.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 07:22:13.352175 openai-image-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-06-27 07:21:19.000000 openai-image-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:57:22.457295 openai-image-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-06-23 06:27:04.000000 openai-image-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2411 2023-06-27 17:57:22.457295 openai-image-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1818 2023-06-27 17:11:09.000000 openai-image-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:57:22.339294 openai-image-1.0.5/openai_image/
+-rw-rw-rw-   0        0        0       66 2023-06-27 17:51:06.000000 openai-image-1.0.5/openai_image/__init__.py
+-rw-rw-rw-   0        0        0     2507 2023-06-27 17:54:13.000000 openai-image-1.0.5/openai_image/main.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:57:22.454290 openai-image-1.0.5/openai_image.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-06-27 17:57:21.000000 openai-image-1.0.5/openai_image.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-27 17:57:22.000000 openai-image-1.0.5/openai_image.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:57:21.000000 openai-image-1.0.5/openai_image.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 17:57:21.000000 openai-image-1.0.5/openai_image.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 17:57:21.000000 openai-image-1.0.5/openai_image.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:57:22.471292 openai-image-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-06-27 17:55:32.000000 openai-image-1.0.5/setup.py
```

### Comparing `openai-image-1.0.4/LICENSE` & `openai-image-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-image-1.0.4/PKG-INFO` & `openai-image-1.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: openai-image
-Version: 1.0.4
-Summary: Python script for generating image from text by Open AI
-Home-page: https://github.com/IgorMan2005/openai_image/
-Author: IgorMan
-Author-email: igorman2005@gmail.com
-Project-URL: Documentation, https://best-itpro.ru/news/openai_image/
-Keywords: openai image api open ai python
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # openai_image
 Python script for generating image from text by Open AI
 
 
 <img src="https://igorman2005.github.io/images/openai-image.jpg" alt="openai_image">
 
 
@@ -32,73 +16,87 @@
 ```
 
 
 **2. Recieve your OpenAI API KEY**
 
 https://platform.openai.com/account/api-keys
 
-create file settings.py in your folder/
 
-put this key to settings.py file
+
+**3. Settings**
 
 ```
 API_KEY = 'your-secret-openai-api-key'
-```
 
-**3. Set image size**
+PIC_SIZE = '256x256'
 
-settings.py:
+IMAGES = ''
 
-```
-PIC_SIZE = '256x256'
+TARGET_TEXT = ''
 ```
 
-(options :'256x256', '512x512', '1024x1024')
+PIC_SIZE options :'256x256', '512x512', '1024x1024'
 
+IMAGES options: if IMAGES = '', script will use current folder. But you can set your own dir, for example: IMAGES = 'D:\Pictures'
 
-**4. Mkdir images**
+TARGET_TEXT options: TARGET_TEXT = '', you will input your target text from keyboard. And you can set it in code, for example TARGET_TEXT = 'Alice in Wonderland'
 
-Create folder 'images' (foder for ready images)
-
-**5. Use openai_image**
+**4. Use openai_image**
 
 ```
 import openai_image
 ```
 
 *Example1:*
 
 ```
 import openai_image
 
-openai_image.get_image()
+API_KEY = 'your-secret-openai-api-key'
+
+PIC_SIZE = '256x256'
+
+IMAGES = ''
+
+TARGET_TEXT = ''
+
+openai_image.get_image(API_KEY, PIC_SIZE, IMAGES, TARGET_TEXT)
 
 ```
 Prompt target text: **blue bird**
 
 <img src="https://igorman2005.github.io/images/blue_bird.jpg" alt="openai_image blue bird">
 
-Your image file ready: **/images/blue_bird.jpg**
+Your image file ready: **blue_bird.png**
 
 
 
 *Example2:*
 
 ```
-import openai_image
+from openai_image import *
+
+API_KEY = 'your-secret-openai-api-key'
+
+PIC_SIZE = '256x256'
+
+IMAGES = 'D:\Pictures\'
+
+TARGET_TEXT = 'Alice in Wonderland'
+
+get_image(API_KEY, PIC_SIZE, IMAGES, TARGET_TEXT)
 
-openai_image.get_image('Alice in Wonderland')
 
 ```
 
 <img src="https://igorman2005.github.io/images/Alice_in_Wonderland.jpg" alt="openai image Alice in Wonderland">
 
-Your image file ready: **/images/Alice_in_Wonderland.jpg**
+Your image file ready: **D:\Pictures\Alice_in_Wonderland.png**
 
 
 ### Documentation
 
 https://best-itpro.ru/news/openai_image/
 
 
 That's All, Folks! 
-;)
+;)
```

### Comparing `openai-image-1.0.4/setup.py` & `openai-image-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='openai-image',
-  version='1.0.4',
+  version='1.0.5',
   author='IgorMan',
   author_email='igorman2005@gmail.com',
   description='Python script for generating image from text by Open AI',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/IgorMan2005/openai_image/',
   packages=['openai_image'],
```

