# Comparing `tmp/mystring-0.0.95.tar.gz` & `tmp/mystring-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.95.tar", last modified: Tue Jun 20 04:30:36 2023, max compression
+gzip compressed data, was "mystring-0.0.96.tar", last modified: Tue Jun 27 14:18:18 2023, max compression
```

## Comparing `mystring-0.0.95.tar` & `mystring-0.0.96.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 04:30:32.000000 mystring-0.0.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-20 04:30:36.077448 mystring-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 04:30:32.000000 mystring-0.0.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-20 04:30:32.000000 mystring-0.0.95/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 04:30:36.077448 mystring-0.0.95/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-20 04:30:32.000000 mystring-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:18:18.338687 mystring-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 14:18:14.000000 mystring-0.0.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 14:18:18.338687 mystring-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 14:18:14.000000 mystring-0.0.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:18:18.338687 mystring-0.0.96/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-06-27 14:18:14.000000 mystring-0.0.96/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:18:18.338687 mystring-0.0.96/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 14:18:18.000000 mystring-0.0.96/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-27 14:18:18.000000 mystring-0.0.96/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:18:18.000000 mystring-0.0.96/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 14:18:18.000000 mystring-0.0.96/mystring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 14:18:18.000000 mystring-0.0.96/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:18:18.338687 mystring-0.0.96/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-27 14:18:14.000000 mystring-0.0.96/setup.py
```

### Comparing `mystring-0.0.95/LICENSE` & `mystring-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.95/mystring/__init__.py` & `mystring-0.0.96/mystring/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,25 @@
 		return mystring(base64.b64encode(self.encode(encoding)).decode(encoding))
 
 	@staticmethod
 	def frombase64(string, encoding='utf-8'):
 		import base64
 		return base64.b64decode(string.encode(encoding)).decode(encoding)
 
+	def matches(regex:str, at_most:int=-1) -> bool:
+		try:
+			regex = re.compile(regex)
+			grps = [
+				match.group() for idx,match in enumerate(regex.finditer(str(self)))
+			]
+			return (at_most > -1 and len(grps) <= at_most) or (at_most == -1 and len(grps) > 0)
+		except Exception as e:
+			print("Error grabbing regex: {0}".format(e))
+			return False
+
 import pandas as pd
 class frame(pd.DataFrame):
 	def __init__(self,*args,**kwargs):
 		super(frame,self).__init__(*args,**kwargs)
 
 	def col_exists(self,column):
 		return column in self.columns
```

### Comparing `mystring-0.0.95/setup.py` & `mystring-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.95"
+VERSION = "0.0.96"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

