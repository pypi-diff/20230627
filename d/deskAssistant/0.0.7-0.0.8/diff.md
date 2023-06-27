# Comparing `tmp/deskAssistant-0.0.7.tar.gz` & `tmp/deskAssistant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deskAssistant-0.0.7.tar", last modified: Fri Apr 21 19:49:40 2023, max compression
+gzip compressed data, was "dist\deskAssistant-0.0.8.tar", last modified: Tue Jun 27 08:12:04 2023, max compression
```

## Comparing `deskAssistant-0.0.7.tar` & `deskAssistant-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.764917 deskAssistant-0.0.7/
--rw-rw-rw-   0        0        0      539 2023-04-21 19:49:40.759930 deskAssistant-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.738475 deskAssistant-0.0.7/deskAssistant/
--rw-rw-rw-   0        0        0       49 2023-04-21 18:44:38.000000 deskAssistant-0.0.7/deskAssistant/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-04-21 18:03:48.000000 deskAssistant-0.0.7/deskAssistant/deskAssistant.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:49:40.758934 deskAssistant-0.0.7/deskAssistant.egg-info/
--rw-rw-rw-   0        0        0      539 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 19:49:40.000000 deskAssistant-0.0.7/deskAssistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 19:49:40.767908 deskAssistant-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-21 18:05:00.000000 deskAssistant-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:12:04.293618 deskAssistant-0.0.8/
+-rw-rw-rw-   0        0        0      539 2023-06-27 08:12:04.289628 deskAssistant-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 08:12:04.221809 deskAssistant-0.0.8/deskAssistant/
+-rw-rw-rw-   0        0        0       49 2023-04-21 18:44:38.000000 deskAssistant-0.0.8/deskAssistant/__init__.py
+-rw-rw-rw-   0        0        0     2160 2023-06-27 07:58:39.000000 deskAssistant-0.0.8/deskAssistant/deskAssistant.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:12:04.287633 deskAssistant-0.0.8/deskAssistant.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-27 08:12:03.000000 deskAssistant-0.0.8/deskAssistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-27 08:12:04.000000 deskAssistant-0.0.8/deskAssistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:12:03.000000 deskAssistant-0.0.8/deskAssistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-27 08:12:03.000000 deskAssistant-0.0.8/deskAssistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 08:12:03.000000 deskAssistant-0.0.8/deskAssistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:12:04.294613 deskAssistant-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-06-27 08:04:25.000000 deskAssistant-0.0.8/setup.py
```

### Comparing `deskAssistant-0.0.7/PKG-INFO` & `deskAssistant-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskAssistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to help with making a virtual assistant
 Author: Blinken77YT
 Author-email: theonilsson2012@icloud.com
 Keywords: python,virtual,assistant,assistant virtual,virtual assistant
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deskAssistant-0.0.7/deskAssistant/deskAssistant.py` & `deskAssistant-0.0.8/deskAssistant/deskAssistant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import speech_recognition as sr
 import pyttsx3 as tts
 import datetime as dt
 import webbrowser
 
 class Assistant:
-    def __init__(self):
+    def __init__(self, voiceid=0, rate=100):
         self.engine = tts.init()
         self.r = sr.Recognizer()
+        self.voices = self.engine.getProperty('voices')
+        self.engine.setProperty('voice', self.voices[voiceid].id)
+        self.engine.setProperty('rate', rate)
 
     def takeCommand(self):
         with sr.Microphone() as source:
             print("Listening...")
             self.r.pause_threshold = 0.7
             audio = self.r.listen(source)
             try:
```

### Comparing `deskAssistant-0.0.7/deskAssistant.egg-info/PKG-INFO` & `deskAssistant-0.0.8/deskAssistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskAssistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to help with making a virtual assistant
 Author: Blinken77YT
 Author-email: theonilsson2012@icloud.com
 Keywords: python,virtual,assistant,assistant virtual,virtual assistant
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deskAssistant-0.0.7/setup.py` & `deskAssistant-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A package to help with making a virtual assistant'
 
 # Setting up
 setup(
     name="deskAssistant",
     version=VERSION,
     author="Blinken77YT",
```

