# Comparing `tmp/wormcat_batch-1.0.0.tar.gz` & `tmp/wormcat_batch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wormcat_batch-1.0.0.tar", last modified: Mon Feb 17 15:03:45 2020, max compression
+gzip compressed data, was "wormcat_batch-1.0.2.tar", last modified: Tue Jun 27 18:15:48 2023, max compression
```

## Comparing `wormcat_batch-1.0.0.tar` & `wormcat_batch-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 danhiggins   (501) staff       (20)        0 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/
--rw-r--r--   0 danhiggins   (501) staff       (20)      299 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/PKG-INFO
-drwxr-xr-x   0 danhiggins   (501) staff       (20)        0 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/
--rw-r--r--   0 danhiggins   (501) staff       (20)      299 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 danhiggins   (501) staff       (20)        1 2020-02-17 00:19:48.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 danhiggins   (501) staff       (20)      451 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 danhiggins   (501) staff       (20)       70 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 danhiggins   (501) staff       (20)       23 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 danhiggins   (501) staff       (20)       14 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/top_level.txt
--rw-r--r--   0 danhiggins   (501) staff       (20)        1 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch.egg-info/dependency_links.txt
-drwxr-xr-x   0 danhiggins   (501) staff       (20)        0 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/wormcat_batch/
--rw-r--r--   0 danhiggins   (501) staff       (20)     2434 2020-02-17 14:26:35.000000 wormcat_batch-1.0.0/wormcat_batch/execute_r.py
--rwxr-xr-x   0 danhiggins   (501) staff       (20)       46 2020-02-17 00:07:33.000000 wormcat_batch-1.0.0/wormcat_batch/is_wormcat_installed.R
--rw-r--r--   0 danhiggins   (501) staff       (20)     2024 2020-02-17 00:07:33.000000 wormcat_batch-1.0.0/wormcat_batch/create_wormcat_xlsx.py
--rwxr-xr-x   0 danhiggins   (501) staff       (20)     1446 2020-02-17 00:07:33.000000 wormcat_batch-1.0.0/wormcat_batch/worm_cat.R
--rwxr-xr-x   0 danhiggins   (501) staff       (20)     5120 2020-02-17 14:28:17.000000 wormcat_batch-1.0.0/wormcat_batch/run_wormcat_batch.py
--rw-r--r--   0 danhiggins   (501) staff       (20)       95 2020-02-17 00:07:33.000000 wormcat_batch-1.0.0/MANIFEST.in
--rw-r--r--   0 danhiggins   (501) staff       (20)     1817 2020-02-17 12:56:22.000000 wormcat_batch-1.0.0/README.md
--rw-r--r--   0 danhiggins   (501) staff       (20)      575 2020-02-17 15:03:41.000000 wormcat_batch-1.0.0/setup.py
--rw-r--r--   0 danhiggins   (501) staff       (20)       38 2020-02-17 15:03:45.000000 wormcat_batch-1.0.0/setup.cfg
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-27 18:15:48.825627 wormcat_batch-1.0.2/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.2/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-27 18:15:48.825518 wormcat_batch-1.0.2/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2178 2023-06-27 18:10:22.000000 wormcat_batch-1.0.2/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-27 18:15:48.825663 wormcat_batch-1.0.2/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      685 2023-06-27 18:14:07.000000 wormcat_batch-1.0.2/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-27 18:15:48.824625 wormcat_batch-1.0.2/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.2/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.2/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.2/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     7128 2023-06-27 17:51:03.000000 wormcat_batch-1.0.2/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.2/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-27 18:15:48.825374 wormcat_batch-1.0.2/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-27 15:34:55.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       23 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-06-27 18:15:48.000000 wormcat_batch-1.0.2/wormcat_batch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wormcat_batch-1.0.0/wormcat_batch/execute_r.py` & `wormcat_batch-1.0.2/wormcat_batch/execute_r.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     def worm_cat_fun(self, file_name, out_dir, title="rgs", annotation_file="straight", input_type="Sequence ID"):
         ret_val = self.run(self.worm_cat_function, file_name, title, out_dir, "False", annotation_file, input_type)
         return ret_val
 
     def run(self, arg_list, *args):
         try:
             processed_args = self.process_args(arg_list, *args)
+            #print(f"R function: {processed_args}")
             process = Popen(processed_args, stdout=PIPE)
             out, err = process.communicate()
             out = str(out, 'utf-8')
             if not out:
                 out = None
             #sys.stderr.write("run: out={} err={}\n".format(out,err))
             return out
```

### Comparing `wormcat_batch-1.0.0/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.0.2/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.0/wormcat_batch/worm_cat.R` & `wormcat_batch-1.0.2/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.0/README.md` & `wormcat_batch-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -55,12 +55,28 @@
 After execution the Output Directory will contain all the Wormcat run data and a
 summary Excel spreadsheet.
 
 
 
 ### Sample Output
 
+
 <img src="./Images/Sample_Output.png"  height="415" width="800"/>
 
+### Local development /test hints
+
+#### Setup to test
+conda activate <appropriate_env>
+pip install .
+
+#### Test
+cd /Users/dan/delme #some working directory
+wormcat_cli --input-excel /Users/dan/Code/Python/Wormcat_batch/Example/Murphy_TS.xlsx --output-path ./output  
+
+#### Deploy
+python setup.py sdist
+twine check dist/*
+twine upload --repository pypi dist/*
+
```

### Comparing `wormcat_batch-1.0.0/setup.py` & `wormcat_batch-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import os
 from setuptools import setup
-#python setup.py sdist upload
+#python setup.py sdist
+#pip install dist/wormcat_batch-1.0.1.tar.gz
+# twine check dist/*
+# twine upload --repository pypi dist/*
+
 setup(name='wormcat_batch',
-      version='1.0.0',
+      version='1.0.2',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
```

