# Comparing `tmp/diself-1.0.tar.gz` & `tmp/diself-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diself-1.0.tar", last modified: Mon Jun 26 23:48:48 2023, max compression
+gzip compressed data, was "diself-1.0.1.tar", last modified: Mon Jun 26 23:51:43 2023, max compression
```

## Comparing `diself-1.0.tar` & `diself-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 23:48:48.300634 diself-1.0/
--rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-1.0/LICENSE
--rw-rw-rw-   0        0        0     3201 2023-06-26 23:48:48.300634 diself-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2826 2023-06-26 23:10:20.000000 diself-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 23:48:48.294634 diself-1.0/diself/
--rw-rw-rw-   0        0        0       21 2023-06-26 23:28:11.000000 diself-1.0/diself/__init__.py
--rw-rw-rw-   0        0        0     4175 2023-06-26 23:47:17.000000 diself-1.0/diself/diself.py
-drwxrwxrwx   0        0        0        0 2023-06-26 23:48:48.299637 diself-1.0/diself.egg-info/
--rw-rw-rw-   0        0        0     3201 2023-06-26 23:48:48.000000 diself-1.0/diself.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-26 23:48:48.000000 diself-1.0/diself.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 23:48:48.000000 diself-1.0/diself.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 23:48:48.000000 diself-1.0/diself.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 23:48:48.000000 diself-1.0/diself.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 23:48:48.300634 diself-1.0/setup.cfg
--rw-rw-rw-   0        0        0      451 2023-06-26 23:48:42.000000 diself-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.206737 diself-1.0.1/
+-rw-rw-rw-   0        0        0     1065 2023-06-26 22:08:08.000000 diself-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3203 2023-06-26 23:51:43.206737 diself-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2826 2023-06-26 23:10:20.000000 diself-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.201738 diself-1.0.1/diself/
+-rw-rw-rw-   0        0        0       21 2023-06-26 23:28:11.000000 diself-1.0.1/diself/__init__.py
+-rw-rw-rw-   0        0        0     4201 2023-06-26 23:51:21.000000 diself-1.0.1/diself/diself.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:51:43.205740 diself-1.0.1/diself.egg-info/
+-rw-rw-rw-   0        0        0     3203 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 23:51:43.000000 diself-1.0.1/diself.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 23:51:43.207738 diself-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-06-26 23:51:38.000000 diself-1.0.1/setup.py
```

### Comparing `diself-1.0/LICENSE` & `diself-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diself-1.0/PKG-INFO` & `diself-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 1.0
+Version: 1.0.1
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diself-1.0/README.md` & `diself-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `diself-1.0/diself/diself.py` & `diself-1.0.1/diself/diself.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,20 +54,21 @@
     """
     def __init__(self, token) -> None:
         global tk
         self.token=token
         tk=token
         self.client=requests.get(f"https://discord.com/api/v10/users/@me", headers={'Authorization': self.token})
         if self.client.status_code != 200:raise TypeError("Invalid or expired token")
-        for i in self.client.json():
+        self.client=self.client.json()
+        for i in self.client:
             exec(f"self.{i}=self.client['{i}']")
         t1=threading.Thread(target=wsf, args=(token,)).start()
 
     def __str__(self):
-        return json.dumps(self.client.json())
+        return json.dumps(self.client)
 
     class TextChannel:
         def __init__(self, id) -> None:
             self.id=id
             self.channel=requests.get(f"https://discord.com/api/v10/channels/{self.id}", headers={'Authorization': tk}).json()
             for i in self.channel:
                 exec(f"self.{i}=self.channel['{i}']")
```

### Comparing `diself-1.0/diself.egg-info/PKG-INFO` & `diself-1.0.1/diself.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diself
-Version: 1.0
+Version: 1.0.1
 Summary: A python module like discord.py but for selfbot
 Home-page: https://github.com/lululepu/diself
 Author: Lululepu
 Author-email: a.no.qsdf@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

