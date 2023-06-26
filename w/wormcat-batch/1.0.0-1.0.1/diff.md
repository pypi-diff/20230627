# Comparing `tmp/wormcat_batch-1.0.0.tar.gz` & `tmp/wormcat_batch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wormcat_batch-1.0.0.tar", last modified: Mon Feb 17 15:03:45 2020, max compression
+gzip compressed data, was "wormcat_batch-1.0.1.tar", last modified: Mon Jun 26 22:58:41 2023, max compression
```

## Comparing `wormcat_batch-1.0.0.tar` & `wormcat_batch-1.0.1.tar`

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
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-26 22:58:41.275292 wormcat_batch-1.0.1/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-26 22:58:41.275179 wormcat_batch-1.0.1/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     1817 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-26 22:58:41.275328 wormcat_batch-1.0.1/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      640 2023-06-26 22:57:17.000000 wormcat_batch-1.0.1/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-26 22:58:41.274318 wormcat_batch-1.0.1/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2434 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     7031 2023-06-26 21:26:30.000000 wormcat_batch-1.0.1/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.1/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-26 22:58:41.275041 wormcat_batch-1.0.1/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       23 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-06-26 22:58:41.000000 wormcat_batch-1.0.1/wormcat_batch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wormcat_batch-1.0.0/wormcat_batch/execute_r.py` & `wormcat_batch-1.0.1/wormcat_batch/execute_r.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.0/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.0.1/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.0/wormcat_batch/worm_cat.R` & `wormcat_batch-1.0.1/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.0/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.0.1/wormcat_batch/run_wormcat_batch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import argparse
 import pandas as pd
 from wormcat_batch.execute_r import ExecuteR
 from wormcat_batch.create_wormcat_xlsx import process_category_files
 
 def get_wormcat_lib():
     executeR = ExecuteR()
     path = executeR.wormcat_library_path_fun()
@@ -15,24 +16,24 @@
         path = path[first_quote+1:last_quote]
 
     return path
 
 def get_category_files(path):
     category_files=[]
     index=1
-    path = "{}{}extdata".format(path,os.path.sep)
+    path = "{}{}extdata".format(path, os.path.sep)
     for root, dirs, files in os.walk(path):
         for filename in files:
             category_files.append(filename)
-            print("[{}]  {}".format(index, filename))
+            #print("[{}]  {}".format(index, filename))
             index +=1
 
-    i = int(input("Select File Name: "))
-    category_file = category_files[i-1]
-    return category_file, path
+    #i = int(input("Select File Name: "))
+    #category_file = category_files[i-1]
+    return category_files, path
 
 def get_output_dir():
     done = False
     output_dir = ""
     while not done:
         output_dir = input("Please provide an Empty Output Directory (or enter to quit): ")
         if output_dir == "":
@@ -122,24 +123,63 @@
         for cat_num in [1,2,3]:
             rgs_fisher = "{}{}{}{}rgs_fisher_cat{}.csv".format(output_dir,os.path.sep,dir_nm,os.path.sep,cat_num)
             cat_nm = "Cat{}".format(cat_num)
             row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
             df_process = df_process.append(row, ignore_index=True)
     return df_process
 
+def is_directory_empty(directory):
+    if not directory:
+        return False
+    if not os.path.exists(directory):
+        return False  # Directory does not exist
+    if not os.path.isdir(directory):
+        return False  # Path exists but is not a directory
+    return not os.listdir(directory)  # Return True if directory is empty, False otherwise
+
 def main():
     print("Wormcat Batch")
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-i', '--input-excel', help='Inputfile in Excel format')
+    parser.add_argument('-o', '--output-path', help='Output path')
+    parser.add_argument('-a', '--annotation-file-nm', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name')
+    args = parser.parse_args()
+
+    if not args.input_excel:
+        print("wormcat_cli --input-excel <full_path_to_excel> --output-path <full_path_to_out_dir> --annotation-file-nm 'whole_genome_v2_nov-11-2021.csv' ")
+        print("Inputfile in Excel format is missing.")
+        return
+
+    if not is_directory_empty(args.output_path):
+        print("wormcat_cli --input-excel <full_path_to_excel> --output-path <full_path_to_out_dir> --annotation-file-nm 'whole_genome_v2_nov-11-2021.csv' ")
+        print("Output path is either non-existent, not a directory, or not empty.")
+        return
+
+
     wormcat_path = get_wormcat_lib()
-    annotation_file, path = get_category_files(wormcat_path)
-    output_dir = get_output_dir()
-    xsl_file_nm = get_spreadsheet_to_process()
-    process_spreadsheet(xsl_file_nm, output_dir, annotation_file)
-    start=xsl_file_nm.rfind(os.path.sep)
-    out_xsl_file_nm="{}{}Out_{}".format(output_dir,os.path.sep,xsl_file_nm[start+1:])
-    annotation_file ="{}{}{}".format(path,os.path.sep,annotation_file)
-    df_process = files_to_process(output_dir)
+    annotation_files, path = get_category_files(wormcat_path)
+
+    if not args.annotation_file_nm or not args.annotation_file_nm in annotation_files:
+        print("wormcat_cli --input-excel <full_path_to_excel> --output-path <full_path_to_out_dir> --annotation-file-nm 'whole_genome_v2_nov-11-2021.csv' ")
+        print("Missing or incorrect annotation-file-nm.")
+        print("Available names: {}".format(annotation_files))
+        return
+
+    # Rest of your program logic goes here
+    print("Input Excel:", args.input_excel)
+    print("Output Path:", args.output_path)
+    print("Annotation File Nm:", args.annotation_file_nm)
+
+    #output_dir = get_output_dir()
+    #xsl_file_nm = get_spreadsheet_to_process()
+
+    process_spreadsheet(args.input_excel, args.output_path, args.annotation_file_nm)
+    start=args.input_excel.rfind(os.path.sep)
+    out_xsl_file_nm="{}{}Out_{}".format(args.output_path, os.path.sep, args.input_excel[start+1:])
+    annotation_file ="{}{}{}".format(path, os.path.sep, args.annotation_file_nm)
+    df_process = files_to_process(args.output_path)
     process_category_files(df_process,annotation_file,out_xsl_file_nm)
 
 #C:\Users\dan\Downloads\Murphy_TS.xlsx
 #https://cran.r-project.org/bin/windows/Rtools/
 if __name__ == '__main__':
     main()
```

### Comparing `wormcat_batch-1.0.0/README.md` & `wormcat_batch-1.0.1/README.md`

 * *Files identical despite different names*

