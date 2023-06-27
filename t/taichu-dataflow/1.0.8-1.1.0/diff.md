# Comparing `tmp/taichu-dataflow-1.0.8.tar.gz` & `tmp/taichu-dataflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-dataflow-1.0.8.tar", last modified: Mon Jun 12 09:26:13 2023, max compression
+gzip compressed data, was "taichu-dataflow-1.1.0.tar", last modified: Tue Jun 27 01:51:43 2023, max compression
```

## Comparing `taichu-dataflow-1.0.8.tar` & `taichu-dataflow-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/PKG-INFO
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 shenli     (501) staff       (20)      401 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 shenli     (501) staff       (20)       13 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 shenli     (501) staff       (20)       16 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/top_level.txt
--rw-r--r--   0 shenli     (501) staff       (20)        1 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 shenli     (501) staff       (20)      194 2023-06-12 03:14:29.000000 taichu-dataflow-1.0.8/README.md
--rw-r--r--   0 shenli     (501) staff       (20)      699 2023-06-12 09:25:57.000000 taichu-dataflow-1.0.8/setup.py
--rw-r--r--   0 shenli     (501) staff       (20)       38 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/setup.cfg
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/
--rwxrwxrwx   0 shenli     (501) staff       (20)     1151 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/filebeat.sh
--rw-r--r--   0 shenli     (501) staff       (20)      534 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/__init__.py
--rw-r--r--   0 shenli     (501) staff       (20)     1928 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/export_back.py
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/
--rw-r--r--   0 shenli     (501) staff       (20)      437 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/env.py
--rw-r--r--   0 shenli     (501) staff       (20)     1340 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py
--rw-r--r--   0 shenli     (501) staff       (20)      475 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/__init__.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-27 01:51:43.910223 taichu-dataflow-1.1.0/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-27 01:51:43.909976 taichu-dataflow-1.1.0/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.1.0/README.md
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-27 01:51:43.910305 taichu-dataflow-1.1.0/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      888 2023-06-27 01:51:41.000000 taichu-dataflow-1.1.0/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-27 01:51:43.906698 taichu-dataflow-1.1.0/taichu_dataflow/
+-rw-r--r--   0 wangkun    (501) staff       (20)      618 2023-06-27 01:48:41.000000 taichu-dataflow-1.1.0/taichu_dataflow/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1805 2023-06-27 01:48:41.000000 taichu-dataflow-1.1.0/taichu_dataflow/command.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     3551 2023-06-27 01:48:41.000000 taichu-dataflow-1.1.0/taichu_dataflow/export_back.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-27 01:51:43.909619 taichu-dataflow-1.1.0/taichu_dataflow/storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     1280 2023-06-14 03:15:36.000000 taichu-dataflow-1.1.0/taichu_dataflow/storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2169 2023-06-27 01:48:41.000000 taichu-dataflow-1.1.0/taichu_dataflow/storage/alluxio.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-dataflow-1.1.0/taichu_dataflow/storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1034 2023-06-14 03:08:02.000000 taichu-dataflow-1.1.0/taichu_dataflow/storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-27 01:51:43.908528 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      473 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       64 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/entry_points.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       50 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-27 01:51:43.000000 taichu-dataflow-1.1.0/taichu_dataflow.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-dataflow-1.0.8/setup.py` & `taichu-dataflow-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from setuptools import setup, find_packages
 
 if __name__ == '__main__':
     name = 'taichu-dataflow'
 
-    requirements = ['boto==2.49.0']
+    requirements = ['boto==2.49.0', 'esdk-obs-python==3.22.2', 'click==8.1.3']
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.8',
+        version='1.1.0',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
         install_requires=requirements,
         include_package_data=True,
         package_data={
             '': ['*.sh'],
+        },
+        entry_points={
+            'console_scripts': [
+                'taichudataflow = taichu_dataflow.command:cli',
+            ],
         }
     )
```

### Comparing `taichu-dataflow-1.0.8/taichu_dataflow/__init__.py` & `taichu-dataflow-1.1.0/taichu_dataflow/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import logging
 import os
+import sys
 import threading
 
 
 def init_filebeat():
     script_dir = os.path.dirname(os.path.abspath(__file__))
     script_path = os.path.join(script_dir, 'filebeat.sh')
     os.system(f"/bin/bash {script_path} >/dev/null 2>&1")
 
 
 def init_logger():
-    logging.basicConfig(level=logging.DEBUG,
-                        format='%(asctime)s %(levelname)s %(message)s',
-                        filename='/tmp/dataflow.log',
-                        filemode='w')
+    logging.basicConfig(
+        handlers=[
+            logging.StreamHandler(sys.stdout),
+            logging.FileHandler("/tmp/dataflow.log", mode="a")
+        ],
+        level=logging.INFO,
+        format='%(asctime)s [%(levelname)s] [%(module)s:%(lineno)d] %(message)s'
+    )
 
 
-threading.Thread(target=init_filebeat).start()
+# threading.Thread(target=init_filebeat).start()
 init_logger()
```

### Comparing `taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py` & `taichu-dataflow-1.1.0/taichu_dataflow/storage/alluxio.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,35 @@
 import boto.exception
 
 
 class StorageAlluxio(StorageInterface):
     _client = None
     _bucket = None
 
-    def __init__(self, storage_type):
+    def __init__(self):
         self._client = boto.connect_s3(
             aws_access_key_id=S3_ACCESS_KEY_ID,
             aws_secret_access_key=S3_SECRET_ACCESS_KEY,
             host=ALLUXIO_HOST,
             port=ALLUXIO_PORT,
             path=ALLUXIO_PATH,
             is_secure=False,
             calling_format=boto.s3.connection.OrdinaryCallingFormat(),
         )
         self._bucket = self._client.get_bucket(STORAGE_BUCKET)
 
     def write_bytes(self, content_bytes, key):
-        pass
+        try:
+            s3_key = self._bucket.new_key(key)
+            s3_key.set_contents_from_file(content_bytes)
+        except boto.exception.BotoClientError:
+            pass
+        except Exception as e:
+            logging.info("key: " + key)
+            logging.error("TaichuStorageError", e)
 
     def write_string(self, content_string, key):
         try:
             s3_key = self._bucket.new_key(key)
             s3_key.set_contents_from_string(content_string)
         except boto.exception.BotoClientError:
             pass
@@ -37,8 +44,23 @@
 
     def write_file(self, file_path, key):
         s3_key = self._bucket.new_key(key)
         with open(file_path, "rb") as f:
             try:
                 s3_key.set_contents_from_file(f)
             except:
-                return
+                return
+
+    def download_dir(self, src, dest):
+        rps = self._bucket.list(prefix=src)
+        for r in rps:
+            os.makedirs(dest, exist_ok=True)
+            local_file = f'{dest}{r.name.replace(src, "")}'
+            try:
+                key = self._bucket.get_key(r.name)
+                with open(local_file, 'wb') as f:
+                    key.get_contents_to_file(f)
+            except Exception as e:
+                if 'SAXParseException' in str(type(e)):
+                    pass
+                else:
+                    logging.error(e)
```

