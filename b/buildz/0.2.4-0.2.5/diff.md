# Comparing `tmp/buildz-0.2.4.tar.gz` & `tmp/buildz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.2.4.tar", last modified: Mon Jun 19 18:25:20 2023, max compression
+gzip compressed data, was "buildz-0.2.5.tar", last modified: Tue Jun 27 16:03:57 2023, max compression
```

## Comparing `buildz-0.2.4.tar` & `buildz-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)    11357 2023-05-10 08:15:22.000000 buildz-0.2.4/LICENSE
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       49 2023-05-10 08:15:22.000000 buildz-0.2.4/MANIFEST.in
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-19 18:25:20.901150 buildz-0.2.4/PKG-INFO
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5193 2023-06-19 17:20:46.000000 buildz-0.2.4/README.md
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1039 2023-06-02 05:54:37.000000 buildz-0.2.4/buildz/__init__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      336 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/__main__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      413 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/base.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     7595 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/build.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)    10421 2023-05-10 08:21:53.000000 buildz-0.2.4/buildz/confz.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/demo/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      514 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/demo.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      502 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/demo.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      451 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/run.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      203 2023-06-19 17:24:31.000000 buildz-0.2.4/buildz/demo/test.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1026 2023-06-19 17:27:16.000000 buildz-0.2.4/buildz/demo/testz.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      357 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/value.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5173 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/keys.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      804 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/tools.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/xconfz/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       45 2023-06-19 17:22:29.000000 buildz-0.2.4/buildz/xconfz/__init__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2886 2023-06-19 17:22:25.000000 buildz-0.2.4/buildz/xconfz/base.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1631 2023-06-19 17:22:23.000000 buildz-0.2.4/buildz/xconfz/buff.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      227 2023-06-19 17:21:53.000000 buildz-0.2.4/buildz/xconfz/fc.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1951 2023-06-19 17:22:20.000000 buildz-0.2.4/buildz/xconfz/fc_item.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1846 2023-06-19 17:22:16.000000 buildz-0.2.4/buildz/xconfz/fc_list.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2116 2023-06-19 17:22:13.000000 buildz-0.2.4/buildz/xconfz/fc_map.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1732 2023-06-19 17:22:08.000000 buildz-0.2.4/buildz/xconfz/fc_set.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2821 2023-06-19 17:22:05.000000 buildz-0.2.4/buildz/xconfz/fc_str.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2762 2023-06-19 17:21:59.000000 buildz-0.2.4/buildz/xconfz/fc_type.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     4020 2023-06-19 17:21:39.000000 buildz-0.2.4/buildz/xconfz/mg.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz.egg-info/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/PKG-INFO
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      661 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/SOURCES.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)        1 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/dependency_links.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)        7 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/top_level.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       38 2023-06-19 18:25:20.901150 buildz-0.2.4/setup.cfg
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      746 2023-06-19 17:13:51.000000 buildz-0.2.4/setup.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    11357 2023-05-10 08:15:22.000000 buildz-0.2.5/LICENSE
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       49 2023-05-10 08:15:22.000000 buildz-0.2.5/MANIFEST.in
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-27 16:03:57.203179 buildz-0.2.5/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5193 2023-06-19 17:20:46.000000 buildz-0.2.5/README.md
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1039 2023-06-02 05:54:37.000000 buildz-0.2.5/buildz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      336 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/__main__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      413 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     7595 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/build.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    10421 2023-05-10 08:21:53.000000 buildz-0.2.5/buildz/confz.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/demo/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      514 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/demo.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      502 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/demo.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      451 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/run.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      203 2023-06-19 17:24:31.000000 buildz-0.2.5/buildz/demo/test.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1107 2023-06-20 16:06:31.000000 buildz-0.2.5/buildz/demo/testz.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      357 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/value.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5173 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/keys.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      804 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/tools.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/xconfz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       45 2023-06-19 17:22:29.000000 buildz-0.2.5/buildz/xconfz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     3397 2023-06-27 15:49:52.000000 buildz-0.2.5/buildz/xconfz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1631 2023-06-19 17:22:23.000000 buildz-0.2.5/buildz/xconfz/buff.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      227 2023-06-19 17:21:53.000000 buildz-0.2.5/buildz/xconfz/fc.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1951 2023-06-19 17:22:20.000000 buildz-0.2.5/buildz/xconfz/fc_item.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1846 2023-06-19 17:22:16.000000 buildz-0.2.5/buildz/xconfz/fc_list.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2116 2023-06-19 17:22:13.000000 buildz-0.2.5/buildz/xconfz/fc_map.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1732 2023-06-19 17:22:08.000000 buildz-0.2.5/buildz/xconfz/fc_set.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2821 2023-06-19 17:22:05.000000 buildz-0.2.5/buildz/xconfz/fc_str.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2762 2023-06-19 17:21:59.000000 buildz-0.2.5/buildz/xconfz/fc_type.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     4067 2023-06-27 15:31:44.000000 buildz-0.2.5/buildz/xconfz/mg.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz.egg-info/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      661 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        1 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        7 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/top_level.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       38 2023-06-27 16:03:57.203179 buildz-0.2.5/setup.cfg
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      746 2023-06-27 15:32:44.000000 buildz-0.2.5/setup.py
```

### Comparing `buildz-0.2.4/LICENSE` & `buildz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/PKG-INFO` & `buildz-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.2.4
+Version: 0.2.5
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.2.4/README.md` & `buildz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/__init__.py` & `buildz-0.2.5/buildz/__init__.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/build.py` & `buildz-0.2.5/buildz/build.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/confz.py` & `buildz-0.2.5/buildz/confz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/demo/demo.confz` & `buildz-0.2.5/buildz/demo/demo.confz`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/demo/testz.py` & `buildz-0.2.5/buildz/demo/testz.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,18 +41,40 @@
     x:"\""
     a=0, #note 1
     b= 1;
     c= x;
     d= [a,b,c]y=0,
     y = 1,
     val = <1, i>
+
+
+
+
     bl = 1|b
     x = 0|nil
+    lst = [
+    a,b,c,
+
+1
+2
+3
+
+
+    x,y,z,,,
+    ]
 }
 """
+s=r"""
+[1,2,
+
+
+3
+4
+5]
+"""
 try:
     from buildz import build
 except:
     import sys
     import os
     sys.path.append(os.path.abspath("./../.."))
     from buildz import build
```

### Comparing `buildz-0.2.4/buildz/keys.py` & `buildz-0.2.5/buildz/keys.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/tools.py` & `buildz-0.2.5/buildz/tools.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/base.py` & `buildz-0.2.5/buildz/xconfz/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,20 +105,48 @@
 pass
 
 class BaseDeal:
     def check_curr(self, buff,  s):
         return buff.curr(len(s))==s
     def init(self, reg):
         pass
+    def make(self, data, fc, format = False, simple = True):
+        return None
     def prev(self, buff, queue):
         return False
     def deal(self, queue, stack):
         return False
 
 pass
 
-class BaseOutput:
+class BaseFormat:
     def deal(self, data, fc):
-        return ""
+        return None
 
 pass
 
+
+class FormatNode:
+    def init(self):
+        self.childs = []
+        self.value = None
+        self.up = None
+        return self
+    def val(self, value):
+        self.value = value
+    def add(self, node):
+        self.childs.append(node)
+        node.up = self
+    def is_leaf(self):
+        return len(self.childs)==0
+
+pass
+
+class KVFormatNode(FormatNode):
+    pass
+
+pass
+
+class SptFormatNode(FormatNode):
+    pass
+
+pass
```

### Comparing `buildz-0.2.4/buildz/xconfz/buff.py` & `buildz-0.2.5/buildz/xconfz/buff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_item.py` & `buildz-0.2.5/buildz/xconfz/fc_item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_list.py` & `buildz-0.2.5/buildz/xconfz/fc_list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_map.py` & `buildz-0.2.5/buildz/xconfz/fc_map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_set.py` & `buildz-0.2.5/buildz/xconfz/fc_set.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_str.py` & `buildz-0.2.5/buildz/xconfz/fc_str.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/fc_type.py` & `buildz-0.2.5/buildz/xconfz/fc_type.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/buildz/xconfz/mg.py` & `buildz-0.2.5/buildz/xconfz/mg.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     types.add_type("null", get_none)
     types.add_type("nil", get_none)
     types.add_type("~", get_none)
 
     cfz.add(types)
 
 
+    cfz.add_fc(StrDeal,"/*","*/", note = True)
     cfz.add_fc(StrDeal,*["###"]*2, note = True)
     cfz.add_fc(StrDeal,"#", "\n", single_line = True, note = True)
     cfz.add_fc(StrDeal,"//", "\n", single_line = True, note = True)
     #cfz.add_fc(StrDeal,*["'''"]*2)
     #cfz.add_fc(StrDeal,*['"""']*2)
     #cfz.add_fc(StrDeal,*["'"]*2, single_line = True)
     #cfz.add_fc(StrDeal,*['"']*2, single_line = True)
```

### Comparing `buildz-0.2.4/buildz.egg-info/PKG-INFO` & `buildz-0.2.5/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.2.4
+Version: 0.2.5
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.2.4/buildz.egg-info/SOURCES.txt` & `buildz-0.2.5/buildz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildz-0.2.4/setup.py` & `buildz-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.2.4',
+    version = '0.2.5',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

