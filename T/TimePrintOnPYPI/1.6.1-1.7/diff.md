# Comparing `tmp/TimePrintOnPYPI-1.6.1.tar.gz` & `tmp/TimePrintOnPYPI-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.6.1.tar", last modified: Tue Jun 27 09:10:15 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.7.tar", last modified: Tue Jun 27 09:12:21 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.6.1.tar` & `TimePrintOnPYPI-1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:10:15.956883 TimePrintOnPYPI-1.6.1/
--rw-rw-rw-   0        0        0     8031 2023-06-27 09:10:15.955883 TimePrintOnPYPI-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7541 2023-06-27 09:09:45.000000 TimePrintOnPYPI-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 09:10:15.931313 TimePrintOnPYPI-1.6.1/TimePrint/
--rw-rw-rw-   0        0        0     2601 2023-06-27 09:10:04.000000 TimePrintOnPYPI-1.6.1/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:10:15.953882 TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     8031 2023-06-27 09:10:15.000000 TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-27 09:10:15.000000 TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:10:15.000000 TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 09:10:15.000000 TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:10:15.956883 TimePrintOnPYPI-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-06-27 09:09:58.000000 TimePrintOnPYPI-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:12:21.776267 TimePrintOnPYPI-1.7/
+-rw-rw-rw-   0        0        0     8027 2023-06-27 09:12:21.775252 TimePrintOnPYPI-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7539 2023-06-27 09:12:12.000000 TimePrintOnPYPI-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:12:21.757128 TimePrintOnPYPI-1.7/TimePrint/
+-rw-rw-rw-   0        0        0     2599 2023-06-27 09:12:17.000000 TimePrintOnPYPI-1.7/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:12:21.772249 TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-06-27 09:12:21.000000 TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-27 09:12:21.000000 TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:12:21.000000 TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 09:12:21.000000 TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:12:21.776267 TimePrintOnPYPI-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-27 09:12:08.000000 TimePrintOnPYPI-1.7/setup.py
```

### Comparing `TimePrintOnPYPI-1.6.1/PKG-INFO` & `TimePrintOnPYPI-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.6.1
+Version: 1.7
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# <span style="color: #FF0000;">**TIME PRINT V1.6.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.7**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
@@ -24,15 +24,15 @@
 ## <span style="color: #007FFF;">**P("text")**</span>
 <span style="color: #E6A8D7;">You don't want to wait until it writes bla bla seconds ?<br>
 it just goes write effect and its fast (very fast)<br>
 Example;<br>
 <span style="color: #87CEEB">**P("TEXT")**<br>
 <span style="color: #0F52BA">format: "text":str<br>
 
-## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETRUNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
+## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETURNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
 <span style="color: #E6A8D7;">Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
 <span style="color: #E6A8D7;">Example format usages;<br>
 
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M")<span style="color: #E6A8D7;">" Returns --> 12:56 = <span style="color: #87CEEB;">(Hours:Minutes)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M:%S")<span style="color: #E6A8D7;">" Returns --> 12:56:24 = <span style="color: #87CEEB;">(Hours:Minutes:Seconds)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%d.%m.%y")<span style="color: #E6A8D7;">" Returns --> 10.02.2023 = <span style="color: #87CEEB;">(Day.Month.Year)
```

### Comparing `TimePrintOnPYPI-1.6.1/README.md` & `TimePrintOnPYPI-1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <span style="color: #FF0000;">**TIME PRINT V1.6.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.7**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
@@ -10,15 +10,15 @@
 ## <span style="color: #007FFF;">**P("text")**</span>
 <span style="color: #E6A8D7;">You don't want to wait until it writes bla bla seconds ?<br>
 it just goes write effect and its fast (very fast)<br>
 Example;<br>
 <span style="color: #87CEEB">**P("TEXT")**<br>
 <span style="color: #0F52BA">format: "text":str<br>
 
-## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETRUNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
+## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETURNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
 <span style="color: #E6A8D7;">Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
 <span style="color: #E6A8D7;">Example format usages;<br>
 
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M")<span style="color: #E6A8D7;">" Returns --> 12:56 = <span style="color: #87CEEB;">(Hours:Minutes)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M:%S")<span style="color: #E6A8D7;">" Returns --> 12:56:24 = <span style="color: #87CEEB;">(Hours:Minutes:Seconds)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%d.%m.%y")<span style="color: #E6A8D7;">" Returns --> 10.02.2023 = <span style="color: #87CEEB;">(Day.Month.Year)
```

### Comparing `TimePrintOnPYPI-1.6.1/TimePrint/__init__.py` & `TimePrintOnPYPI-1.7/TimePrint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.6.1")
+    print("Version: 1.7")
 def Timetag(format: str) -> str:
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
 
     "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
```

### Comparing `TimePrintOnPYPI-1.6.1/TimePrintOnPYPI.egg-info/PKG-INFO` & `TimePrintOnPYPI-1.7/TimePrintOnPYPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.6.1
+Version: 1.7
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# <span style="color: #FF0000;">**TIME PRINT V1.6.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.7**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
@@ -24,15 +24,15 @@
 ## <span style="color: #007FFF;">**P("text")**</span>
 <span style="color: #E6A8D7;">You don't want to wait until it writes bla bla seconds ?<br>
 it just goes write effect and its fast (very fast)<br>
 Example;<br>
 <span style="color: #87CEEB">**P("TEXT")**<br>
 <span style="color: #0F52BA">format: "text":str<br>
 
-## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETRUNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
+## <span style="color: #007FFF;">**Timetag(format:str)<br>TIME TAG ONLY SUPPORTS (TR) LANGUAGE. ALL RETURNS WILL BE TURKISH ALL THIS STUFF IS EXAMPLE**</span>
 <span style="color: #E6A8D7;">Its not very cool thing but i added,Don't have to much talk just look ex.<br>
 
 <span style="color: #E6A8D7;">Example format usages;<br>
 
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M")<span style="color: #E6A8D7;">" Returns --> 12:56 = <span style="color: #87CEEB;">(Hours:Minutes)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%H:%M:%S")<span style="color: #E6A8D7;">" Returns --> 12:56:24 = <span style="color: #87CEEB;">(Hours:Minutes:Seconds)<br>
 <span style="color: #E6A8D7;">"<span style="color: #87CEEB;">Timetag("%d.%m.%y")<span style="color: #E6A8D7;">" Returns --> 10.02.2023 = <span style="color: #87CEEB;">(Day.Month.Year)
```

### Comparing `TimePrintOnPYPI-1.6.1/setup.py` & `TimePrintOnPYPI-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         print("Need Help ? Contact Me From e-mail: osmntn08@gmail.com")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.6.1',
+    version='1.7',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

