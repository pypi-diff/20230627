# Comparing `tmp/yellowdog-python-examples-6.0.3.tar.gz` & `tmp/yellowdog-python-examples-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.3.tar", last modified: Wed Jun 21 15:21:00 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.4.tar", last modified: Tue Jun 27 08:14:40 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.3.tar` & `yellowdog-python-examples-6.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.795598 yellowdog-python-examples-6.0.3/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.3/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-21 15:21:00.795687 yellowdog-python-examples-6.0.3/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.3/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   110945 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.3/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-21 15:21:00.795998 yellowdog-python-examples-6.0.3/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.3/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.794636 yellowdog-python-examples-6.0.3/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.3/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.3/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.3/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.3/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.3/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.3/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.3/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.3/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.3/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-06-20 14:36:54.000000 yellowdog-python-examples-6.0.3/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.3/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2995 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.795471 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543909 yellowdog-python-examples-6.0.4/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.4/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 08:14:40.543984 yellowdog-python-examples-6.0.4/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.4/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   111863 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.4/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-27 08:14:40.544294 yellowdog-python-examples-6.0.4/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.4/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543080 yellowdog-python-examples-6.0.4/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.4/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.4/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.4/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.4/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.4/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.4/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    41866 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     7748 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.4/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2545 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.4/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.4/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2995 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.4/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543811 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.3/LICENSE` & `yellowdog-python-examples-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/PKG-INFO` & `yellowdog-python-examples-6.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.3
+Version: 6.0.4
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.3/PYPI_README.md` & `yellowdog-python-examples-6.0.4/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/README.md` & `yellowdog-python-examples-6.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -182,6754 +182,6811 @@
 00000b50: 6e20 7468 6520 696e 7075 7473 204c 6973  n the inputs Lis
 00000b60: 745d 2823 6669 6c65 732d 696e 2d74 6865  t](#files-in-the
 00000b70: 2d69 6e70 7574 732d 6c69 7374 290a 2020  -inputs-list).  
 00000b80: 2020 2020 2020 202a 205b 4669 6c65 7320         * [Files 
 00000b90: 696e 2074 6865 2075 706c 6f61 6446 696c  in the uploadFil
 00000ba0: 6573 204c 6973 745d 2823 6669 6c65 732d  es List](#files-
 00000bb0: 696e 2d74 6865 2d75 706c 6f61 6466 696c  in-the-uploadfil
-00000bc0: 6573 2d6c 6973 7429 0a20 2020 2020 202a  es-list).      *
-00000bd0: 205b 4669 6c65 2044 6570 656e 6465 6e63   [File Dependenc
-00000be0: 6965 7320 5573 696e 6720 7665 7269 6679  ies Using verify
-00000bf0: 4174 5374 6172 7420 616e 6420 7665 7269  AtStart and veri
-00000c00: 6679 5761 6974 5d28 2366 696c 652d 6465  fyWait](#file-de
-00000c10: 7065 6e64 656e 6369 6573 2d75 7369 6e67  pendencies-using
-00000c20: 2d76 6572 6966 7961 7473 7461 7274 2d61  -verifyatstart-a
-00000c30: 6e64 2d76 6572 6966 7977 6169 7429 0a20  nd-verifywait). 
-00000c40: 2020 2020 202a 205b 4669 6c65 7320 446f       * [Files Do
-00000c50: 776e 6c6f 6164 6564 2055 7369 6e67 2069  wnloaded Using i
-00000c60: 6e70 7574 734f 7074 696f 6e61 6c5d 2823  nputsOptional](#
-00000c70: 6669 6c65 732d 646f 776e 6c6f 6164 6564  files-downloaded
-00000c80: 2d75 7369 6e67 2d69 6e70 7574 736f 7074  -using-inputsopt
-00000c90: 696f 6e61 6c29 0a20 2020 2020 202a 205b  ional).      * [
-00000ca0: 4669 6c65 7320 446f 776e 6c6f 6164 6564  Files Downloaded
-00000cb0: 2074 6f20 6120 4e6f 6465 2066 6f72 2075   to a Node for u
-00000cc0: 7365 2069 6e20 5461 736b 2045 7865 6375  se in Task Execu
-00000cd0: 7469 6f6e 5d28 2366 696c 6573 2d64 6f77  tion](#files-dow
-00000ce0: 6e6c 6f61 6465 642d 746f 2d61 2d6e 6f64  nloaded-to-a-nod
-00000cf0: 652d 666f 722d 7573 652d 696e 2d74 6173  e-for-use-in-tas
-00000d00: 6b2d 6578 6563 7574 696f 6e29 0a20 2020  k-execution).   
-00000d10: 2020 202a 205b 4669 6c65 7320 5570 6c6f     * [Files Uplo
-00000d20: 6164 6564 2066 726f 6d20 6120 4e6f 6465  aded from a Node
-00000d30: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
-00000d40: 746f 7265 2061 6674 6572 2054 6173 6b20  tore after Task 
-00000d50: 4578 6563 7574 696f 6e5d 2823 6669 6c65  Execution](#file
-00000d60: 732d 7570 6c6f 6164 6564 2d66 726f 6d2d  s-uploaded-from-
-00000d70: 612d 6e6f 6465 2d74 6f2d 7468 652d 6f62  a-node-to-the-ob
-00000d80: 6a65 6374 2d73 746f 7265 2d61 6674 6572  ject-store-after
-00000d90: 2d74 6173 6b2d 6578 6563 7574 696f 6e29  -task-execution)
-00000da0: 0a20 2020 2020 202a 205b 4669 6c65 7320  .      * [Files 
-00000db0: 446f 776e 6c6f 6164 6564 2066 726f 6d20  Downloaded from 
-00000dc0: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
-00000dd0: 2074 6f20 4c6f 6361 6c20 5374 6f72 6167   to Local Storag
-00000de0: 655d 2823 6669 6c65 732d 646f 776e 6c6f  e](#files-downlo
-00000df0: 6164 6564 2d66 726f 6d2d 7468 652d 6f62  aded-from-the-ob
-00000e00: 6a65 6374 2d73 746f 7265 2d74 6f2d 6c6f  ject-store-to-lo
-00000e10: 6361 6c2d 7374 6f72 6167 6529 0a20 2020  cal-storage).   
-00000e20: 2a20 5b54 6173 6b20 4578 6563 7574 696f  * [Task Executio
-00000e30: 6e20 436f 6e74 6578 745d 2823 7461 736b  n Context](#task
-00000e40: 2d65 7865 6375 7469 6f6e 2d63 6f6e 7465  -execution-conte
-00000e50: 7874 290a 2020 2020 2020 2a20 5b54 6173  xt).      * [Tas
-00000e60: 6b20 4578 6563 7574 696f 6e20 5374 6570  k Execution Step
-00000e70: 735d 2823 7461 736b 2d65 7865 6375 7469  s](#task-executi
-00000e80: 6f6e 2d73 7465 7073 290a 2020 2020 2020  on-steps).      
-00000e90: 2a20 5b54 6865 2055 7365 7220 616e 6420  * [The User and 
-00000ea0: 4772 6f75 7020 7573 6564 2066 6f72 2054  Group used for T
-00000eb0: 6173 6b73 5d28 2374 6865 2d75 7365 722d  asks](#the-user-
-00000ec0: 616e 642d 6772 6f75 702d 7573 6564 2d66  and-group-used-f
-00000ed0: 6f72 2d74 6173 6b73 290a 2020 2020 2020  or-tasks).      
-00000ee0: 2a20 5b48 6f6d 6520 4469 7265 6374 6f72  * [Home Director
-00000ef0: 7920 666f 7220 7964 2d61 6765 6e74 5d28  y for yd-agent](
-00000f00: 2368 6f6d 652d 6469 7265 6374 6f72 792d  #home-directory-
-00000f10: 666f 722d 7964 2d61 6765 6e74 290a 2020  for-yd-agent).  
-00000f20: 2020 2020 2a20 5b54 6173 6b20 4578 6563      * [Task Exec
-00000f30: 7574 696f 6e20 4469 7265 6374 6f72 795d  ution Directory]
-00000f40: 2823 7461 736b 2d65 7865 6375 7469 6f6e  (#task-execution
-00000f50: 2d64 6972 6563 746f 7279 290a 2020 202a  -directory).   *
-00000f60: 205b 5370 6563 6966 7969 6e67 2057 6f72   [Specifying Wor
-00000f70: 6b20 5265 7175 6972 656d 656e 7473 2075  k Requirements u
-00000f80: 7369 6e67 2043 5356 2044 6174 615d 2823  sing CSV Data](#
-00000f90: 7370 6563 6966 7969 6e67 2d77 6f72 6b2d  specifying-work-
-00000fa0: 7265 7175 6972 656d 656e 7473 2d75 7369  requirements-usi
-00000fb0: 6e67 2d63 7376 2d64 6174 6129 0a20 2020  ng-csv-data).   
-00000fc0: 2020 202a 205b 576f 726b 2052 6571 7569     * [Work Requi
-00000fd0: 7265 6d65 6e74 2043 5356 2044 6174 6120  rement CSV Data 
-00000fe0: 4578 616d 706c 655d 2823 776f 726b 2d72  Example](#work-r
-00000ff0: 6571 7569 7265 6d65 6e74 2d63 7376 2d64  equirement-csv-d
-00001000: 6174 612d 6578 616d 706c 6529 0a20 2020  ata-example).   
-00001010: 2020 202a 205b 4353 5620 5661 7269 6162     * [CSV Variab
-00001020: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
-00001030: 5d28 2363 7376 2d76 6172 6961 626c 652d  ](#csv-variable-
-00001040: 7375 6273 7469 7475 7469 6f6e 7329 0a20  substitutions). 
-00001050: 2020 2020 202a 205b 5072 6f70 6572 7479       * [Property
-00001060: 2049 6e68 6572 6974 616e 6365 5d28 2370   Inheritance](#p
-00001070: 726f 7065 7274 792d 696e 6865 7269 7461  roperty-inherita
-00001080: 6e63 652d 3129 0a20 2020 2020 202a 205b  nce-1).      * [
-00001090: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
-000010a0: 6f75 7073 2075 7369 6e67 204d 756c 7469  oups using Multi
-000010b0: 706c 6520 4353 5620 4669 6c65 735d 2823  ple CSV Files](#
-000010c0: 6d75 6c74 6970 6c65 2d74 6173 6b2d 6772  multiple-task-gr
-000010d0: 6f75 7073 2d75 7369 6e67 2d6d 756c 7469  oups-using-multi
-000010e0: 706c 652d 6373 762d 6669 6c65 7329 0a20  ple-csv-files). 
-000010f0: 2020 2020 202a 205b 5573 696e 6720 4353       * [Using CS
-00001100: 5620 4461 7461 2077 6974 6820 5369 6d70  V Data with Simp
-00001110: 6c65 2c20 544f 4d4c 2d4f 6e6c 7920 576f  le, TOML-Only Wo
-00001120: 726b 2052 6571 7569 7265 6d65 6e74 2053  rk Requirement S
-00001130: 7065 6369 6669 6361 7469 6f6e 735d 2823  pecifications](#
-00001140: 7573 696e 672d 6373 762d 6461 7461 2d77  using-csv-data-w
-00001150: 6974 682d 7369 6d70 6c65 2d74 6f6d 6c2d  ith-simple-toml-
-00001160: 6f6e 6c79 2d77 6f72 6b2d 7265 7175 6972  only-work-requir
-00001170: 656d 656e 742d 7370 6563 6966 6963 6174  ement-specificat
-00001180: 696f 6e73 290a 2020 2020 2020 2a20 5b49  ions).      * [I
-00001190: 6e73 7065 6374 696e 6720 7468 6520 5265  nspecting the Re
-000011a0: 7375 6c74 7320 6f66 2043 5356 2056 6172  sults of CSV Var
-000011b0: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
-000011c0: 6f6e 5d28 2369 6e73 7065 6374 696e 672d  on](#inspecting-
-000011d0: 7468 652d 7265 7375 6c74 732d 6f66 2d63  the-results-of-c
-000011e0: 7376 2d76 6172 6961 626c 652d 7375 6273  sv-variable-subs
-000011f0: 7469 7475 7469 6f6e 290a 2a20 5b57 6f72  titution).* [Wor
-00001200: 6b65 7220 506f 6f6c 2050 726f 7065 7274  ker Pool Propert
-00001210: 6965 735d 2823 776f 726b 6572 2d70 6f6f  ies](#worker-poo
-00001220: 6c2d 7072 6f70 6572 7469 6573 290a 2020  l-properties).  
-00001230: 202a 205b 4175 746f 6d61 7469 6320 5072   * [Automatic Pr
-00001240: 6f70 6572 7469 6573 5d28 2361 7574 6f6d  operties](#autom
-00001250: 6174 6963 2d70 726f 7065 7274 6965 732d  atic-properties-
-00001260: 3129 0a20 2020 2a20 5b54 4f4d 4c20 5072  1).   * [TOML Pr
-00001270: 6f70 6572 7469 6573 2069 6e20 7468 6520  operties in the 
-00001280: 776f 726b 6572 506f 6f6c 2053 6563 7469  workerPool Secti
-00001290: 6f6e 5d28 2374 6f6d 6c2d 7072 6f70 6572  on](#toml-proper
-000012a0: 7469 6573 2d69 6e2d 7468 652d 776f 726b  ties-in-the-work
-000012b0: 6572 706f 6f6c 2d73 6563 7469 6f6e 290a  erpool-section).
-000012c0: 2020 202a 205b 576f 726b 6572 2050 6f6f     * [Worker Poo
-000012d0: 6c20 5370 6563 6966 6963 6174 696f 6e20  l Specification 
-000012e0: 5573 696e 6720 4a53 4f4e 2044 6f63 756d  Using JSON Docum
-000012f0: 656e 7473 5d28 2377 6f72 6b65 722d 706f  ents](#worker-po
-00001300: 6f6c 2d73 7065 6369 6669 6361 7469 6f6e  ol-specification
-00001310: 2d75 7369 6e67 2d6a 736f 6e2d 646f 6375  -using-json-docu
-00001320: 6d65 6e74 7329 0a20 2020 2020 202a 205b  ments).      * [
-00001330: 576f 726b 6572 2050 6f6f 6c20 4a53 4f4e  Worker Pool JSON
-00001340: 2045 7861 6d70 6c65 735d 2823 776f 726b   Examples](#work
-00001350: 6572 2d70 6f6f 6c2d 6a73 6f6e 2d65 7861  er-pool-json-exa
-00001360: 6d70 6c65 7329 0a20 2020 2020 202a 205b  mples).      * [
-00001370: 544f 4d4c 2050 726f 7065 7274 6965 7320  TOML Properties 
-00001380: 496e 6865 7269 7465 6420 6279 2057 6f72  Inherited by Wor
-00001390: 6b65 7220 506f 6f6c 204a 534f 4e20 5370  ker Pool JSON Sp
-000013a0: 6563 6966 6963 6174 696f 6e73 5d28 2374  ecifications](#t
-000013b0: 6f6d 6c2d 7072 6f70 6572 7469 6573 2d69  oml-properties-i
-000013c0: 6e68 6572 6974 6564 2d62 792d 776f 726b  nherited-by-work
-000013d0: 6572 2d70 6f6f 6c2d 6a73 6f6e 2d73 7065  er-pool-json-spe
-000013e0: 6369 6669 6361 7469 6f6e 7329 0a20 2020  cifications).   
-000013f0: 2a20 5b56 6172 6961 626c 6520 5375 6273  * [Variable Subs
-00001400: 7469 7475 7469 6f6e 7320 696e 2057 6f72  titutions in Wor
-00001410: 6b65 7220 506f 6f6c 2050 726f 7065 7274  ker Pool Propert
-00001420: 6965 735d 2823 7661 7269 6162 6c65 2d73  ies](#variable-s
-00001430: 7562 7374 6974 7574 696f 6e73 2d69 6e2d  ubstitutions-in-
-00001440: 776f 726b 6572 2d70 6f6f 6c2d 7072 6f70  worker-pool-prop
-00001450: 6572 7469 6573 290a 2020 202a 205b 4472  erties).   * [Dr
-00001460: 792d 5275 6e6e 696e 6720 576f 726b 6572  y-Running Worker
-00001470: 2050 6f6f 6c20 5072 6f76 6973 696f 6e69   Pool Provisioni
-00001480: 6e67 5d28 2364 7279 2d72 756e 6e69 6e67  ng](#dry-running
-00001490: 2d77 6f72 6b65 722d 706f 6f6c 2d70 726f  -worker-pool-pro
-000014a0: 7669 7369 6f6e 696e 6729 0a2a 205b 4a73  visioning).* [Js
-000014b0: 6f6e 6e65 7420 5375 7070 6f72 745d 2823  onnet Support](#
-000014c0: 6a73 6f6e 6e65 742d 7375 7070 6f72 7429  jsonnet-support)
-000014d0: 0a20 2020 2a20 5b4a 736f 6e6e 6574 2049  .   * [Jsonnet I
-000014e0: 6e73 7461 6c6c 6174 696f 6e5d 2823 6a73  nstallation](#js
-000014f0: 6f6e 6e65 742d 696e 7374 616c 6c61 7469  onnet-installati
-00001500: 6f6e 290a 2020 202a 205b 5661 7269 6162  on).   * [Variab
-00001510: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
-00001520: 2069 6e20 4a73 6f6e 6e65 7420 4669 6c65   in Jsonnet File
-00001530: 735d 2823 7661 7269 6162 6c65 2d73 7562  s](#variable-sub
-00001540: 7374 6974 7574 696f 6e73 2d69 6e2d 6a73  stitutions-in-js
-00001550: 6f6e 6e65 742d 6669 6c65 7329 0a20 2020  onnet-files).   
-00001560: 2a20 5b43 6865 636b 696e 6720 4a73 6f6e  * [Checking Json
-00001570: 6e65 7420 5072 6f63 6573 7369 6e67 5d28  net Processing](
-00001580: 2363 6865 636b 696e 672d 6a73 6f6e 6e65  #checking-jsonne
-00001590: 742d 7072 6f63 6573 7369 6e67 290a 2020  t-processing).  
-000015a0: 202a 205b 4a73 6f6e 6e65 7420 4578 616d   * [Jsonnet Exam
-000015b0: 706c 655d 2823 6a73 6f6e 6e65 742d 6578  ple](#jsonnet-ex
-000015c0: 616d 706c 6529 0a2a 205b 436f 6d6d 616e  ample).* [Comman
-000015d0: 6420 4c69 7374 5d28 2363 6f6d 6d61 6e64  d List](#command
-000015e0: 2d6c 6973 7429 0a20 2020 2a20 5b79 642d  -list).   * [yd-
-000015f0: 7375 626d 6974 5d28 2379 642d 7375 626d  submit](#yd-subm
-00001600: 6974 290a 2020 202a 205b 7964 2d70 726f  it).   * [yd-pro
-00001610: 7669 7369 6f6e 5d28 2379 642d 7072 6f76  vision](#yd-prov
-00001620: 6973 696f 6e29 0a20 2020 2a20 5b79 642d  ision).   * [yd-
-00001630: 6361 6e63 656c 5d28 2379 642d 6361 6e63  cancel](#yd-canc
-00001640: 656c 290a 2020 202a 205b 7964 2d61 626f  el).   * [yd-abo
-00001650: 7274 5d28 2379 642d 6162 6f72 7429 0a20  rt](#yd-abort). 
-00001660: 2020 2a20 5b79 642d 646f 776e 6c6f 6164    * [yd-download
-00001670: 5d28 2379 642d 646f 776e 6c6f 6164 290a  ](#yd-download).
-00001680: 2020 202a 205b 7964 2d64 656c 6574 655d     * [yd-delete]
-00001690: 2823 7964 2d64 656c 6574 6529 0a20 2020  (#yd-delete).   
-000016a0: 2a20 5b79 642d 7570 6c6f 6164 5d28 2379  * [yd-upload](#y
-000016b0: 642d 7570 6c6f 6164 290a 2020 202a 205b  d-upload).   * [
-000016c0: 7964 2d73 6875 7464 6f77 6e5d 2823 7964  yd-shutdown](#yd
-000016d0: 2d73 6875 7464 6f77 6e29 0a20 2020 2a20  -shutdown).   * 
-000016e0: 5b79 642d 696e 7374 616e 7469 6174 655d  [yd-instantiate]
-000016f0: 2823 7964 2d69 6e73 7461 6e74 6961 7465  (#yd-instantiate
-00001700: 290a 2020 2020 2020 2a20 5b54 6573 742d  ).      * [Test-
-00001710: 5275 6e6e 696e 6720 6120 4479 6e61 6d69  Running a Dynami
-00001720: 6320 5465 6d70 6c61 7465 5d28 2374 6573  c Template](#tes
-00001730: 742d 7275 6e6e 696e 672d 612d 6479 6e61  t-running-a-dyna
-00001740: 6d69 632d 7465 6d70 6c61 7465 290a 2020  mic-template).  
-00001750: 202a 205b 7964 2d74 6572 6d69 6e61 7465   * [yd-terminate
-00001760: 5d28 2379 642d 7465 726d 696e 6174 6529  ](#yd-terminate)
-00001770: 0a0a 3c21 2d2d 2041 6464 6564 2062 793a  ..<!-- Added by:
-00001780: 2070 7774 2c20 6174 3a20 5475 6520 4a75   pwt, at: Tue Ju
-00001790: 6e20 3230 2031 363a 3139 3a35 3120 4253  n 20 16:19:51 BS
-000017a0: 5420 3230 3233 202d 2d3e 0a0a 3c21 2d2d  T 2023 -->..<!--
-000017b0: 7465 2d2d 3e0a 0a23 204f 7665 7276 6965  te-->..# Overvie
-000017c0: 770a 0a54 6869 7320 7265 706f 7369 746f  w..This reposito
-000017d0: 7279 2063 6f6e 7461 696e 7320 6120 7365  ry contains a se
-000017e0: 7420 6f66 2065 7861 6d70 6c65 2050 7974  t of example Pyt
-000017f0: 686f 6e20 7363 7269 7074 7320 666f 7220  hon scripts for 
-00001800: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
-00001810: 2074 6865 2059 656c 6c6f 7744 6f67 2050   the YellowDog P
-00001820: 6c61 7466 6f72 6d2e 2054 6865 2073 6372  latform. The scr
-00001830: 6970 7473 2075 7365 2074 6865 202a 2a5b  ipts use the **[
-00001840: 5965 6c6c 6f77 446f 6720 5079 7468 6f6e  YellowDog Python
-00001850: 2053 444b 5d28 6874 7470 733a 2f2f 646f   SDK](https://do
-00001860: 6373 2e79 656c 6c6f 7764 6f67 2e63 6f2f  cs.yellowdog.co/
-00001870: 6170 692f 7079 7468 6f6e 2f69 6e64 6578  api/python/index
-00001880: 2e68 746d 6c29 2a2a 2c20 7468 6520 636f  .html)**, the co
-00001890: 6465 2066 6f72 2077 6869 6368 2063 616e  de for which can
-000018a0: 2062 6520 666f 756e 6420 5b6f 6e20 4769   be found [on Gi
-000018b0: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
-000018c0: 7468 7562 2e63 6f6d 2f79 656c 6c6f 7764  thub.com/yellowd
-000018d0: 6f67 2f79 656c 6c6f 7764 6f67 2d73 646b  og/yellowdog-sdk
-000018e0: 2d70 7974 686f 6e2d 7075 626c 6963 292e  -python-public).
-000018f0: 0a0a 0a2a 284e 6f74 653a 2074 6865 7365  ...*(Note: these
-00001900: 2073 6372 6970 7473 2061 7265 2069 6e74   scripts are int
-00001910: 656e 6465 6420 746f 2062 6520 6120 6865  ended to be a he
-00001920: 6c70 6675 6c20 7374 6172 7469 6e67 2070  lpful starting p
-00001930: 6f69 6e74 2066 6f72 2065 7870 6572 696d  oint for experim
-00001940: 656e 7469 6e67 2077 6974 6820 7468 6520  enting with the 
-00001950: 5965 6c6c 6f77 446f 6720 506c 6174 666f  YellowDog Platfo
-00001960: 726d 2e20 5468 6579 2061 7265 206e 6f74  rm. They are not
-00001970: 2061 7373 7572 6564 2074 6f20 6265 206f   assured to be o
-00001980: 6620 7072 6f64 7563 7469 6f6e 2071 7561  f production qua
-00001990: 6c69 7479 206e 6f72 2064 6f20 7468 6579  lity nor do they
-000019a0: 2072 6570 7265 7365 6e74 2061 2073 7461   represent a sta
-000019b0: 6e64 6172 6420 6f72 2072 6563 6f6d 6d65  ndard or recomme
-000019c0: 6e64 6564 206d 6574 686f 6420 666f 7220  nded method for 
-000019d0: 7573 696e 6720 5965 6c6c 6f77 446f 672e  using YellowDog.
-000019e0: 292a 0a0a 5468 6973 2064 6f63 756d 656e  )*..This documen
-000019f0: 7461 7469 6f6e 2073 686f 756c 6420 6265  tation should be
-00001a00: 2072 6561 6420 696e 2063 6f6e 6a75 6e63   read in conjunc
-00001a10: 7469 6f6e 2077 6974 6820 7468 6520 6d61  tion with the ma
-00001a20: 696e 202a 2a5b 5965 6c6c 6f77 446f 6720  in **[YellowDog 
-00001a30: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00001a40: 7474 7073 3a2f 2f64 6f63 732e 7965 6c6c  ttps://docs.yell
-00001a50: 6f77 646f 672e 636f 292a 2a2c 2077 6869  owdog.co)**, whi
-00001a60: 6368 2070 726f 7669 6465 7320 6120 636f  ch provides a co
-00001a70: 6d70 7265 6865 6e73 6976 6520 6465 7363  mprehensive desc
-00001a80: 7269 7074 696f 6e20 6f66 2074 6865 2063  ription of the c
-00001a90: 6f6e 6365 7074 7320 616e 6420 6f70 6572  oncepts and oper
-00001aa0: 6174 696f 6e20 6f66 2074 6865 2059 656c  ation of the Yel
-00001ab0: 6c6f 7744 6f67 2050 6c61 7466 6f72 6d2e  lowDog Platform.
-00001ac0: 0a0a 5465 6d70 6c61 7465 2073 6f6c 7574  ..Template solut
-00001ad0: 696f 6e73 2066 6f72 2065 7870 6572 696d  ions for experim
-00001ae0: 656e 7469 6e67 2077 6974 6820 7468 6573  enting with thes
-00001af0: 6520 7363 7269 7074 7320 6361 6e20 6265  e scripts can be
-00001b00: 2066 6f75 6e64 2069 6e20 7468 6520 2a2a   found in the **
-00001b10: 5b70 7974 686f 6e2d 6578 616d 706c 6573  [python-examples
-00001b20: 2d74 656d 706c 6174 6573 5d28 6874 7470  -templates](http
-00001b30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-00001b40: 656c 6c6f 7764 6f67 2f70 7974 686f 6e2d  ellowdog/python-
-00001b50: 6578 616d 706c 6573 2d74 656d 706c 6174  examples-templat
-00001b60: 6573 292a 2a20 7265 706f 7369 746f 7279  es)** repository
-00001b70: 2e0a 0a54 6865 2073 6372 6970 7473 2070  ...The scripts p
-00001b80: 726f 7669 6465 2074 6865 2066 6f6c 6c6f  rovide the follo
-00001b90: 7769 6e67 2063 6170 6162 696c 6974 6965  wing capabilitie
-00001ba0: 733a 0a0a 2d20 2a2a 5072 6f76 6973 696f  s:..- **Provisio
-00001bb0: 6e69 6e67 2a2a 2057 6f72 6b65 7220 506f  ning** Worker Po
-00001bc0: 6f6c 7320 7769 7468 2074 6865 202a 2a60  ols with the **`
-00001bd0: 7964 2d70 726f 7669 7369 6f6e 602a 2a20  yd-provision`** 
-00001be0: 636f 6d6d 616e 640a 2d20 2a2a 5375 626d  command.- **Subm
-00001bf0: 6974 7469 6e67 2a2a 2057 6f72 6b20 5265  itting** Work Re
-00001c00: 7175 6972 656d 656e 7473 2077 6974 6820  quirements with 
-00001c10: 7468 6520 2a2a 6079 642d 7375 626d 6974  the **`yd-submit
-00001c20: 602a 2a20 636f 6d6d 616e 640a 2d20 2a2a  `** command.- **
-00001c30: 5570 6c6f 6164 696e 672a 2a20 6669 6c65  Uploading** file
-00001c40: 7320 746f 2074 6865 2059 656c 6c6f 7744  s to the YellowD
-00001c50: 6f67 204f 626a 6563 7420 5374 6f72 6520  og Object Store 
-00001c60: 7769 7468 2074 6865 202a 2a60 7964 2d75  with the **`yd-u
-00001c70: 706c 6f61 6460 2a2a 2063 6f6d 6d61 6e64  pload`** command
-00001c80: 0a2d 202a 2a49 6e73 7461 6e74 6961 7469  .- **Instantiati
-00001c90: 6e67 2a2a 2043 6f6d 7075 7465 2052 6571  ng** Compute Req
-00001ca0: 7569 7265 6d65 6e74 7320 7769 7468 2074  uirements with t
-00001cb0: 6865 202a 2a60 7964 2d69 6e73 7461 6e74  he **`yd-instant
-00001cc0: 6961 7465 602a 2a20 636f 6d6d 616e 640a  iate`** command.
-00001cd0: 2d20 2a2a 446f 776e 6c6f 6164 696e 672a  - **Downloading*
-00001ce0: 2a20 5265 7375 6c74 7320 6672 6f6d 2074  * Results from t
-00001cf0: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
-00001d00: 6563 7420 5374 6f72 6520 7769 7468 2074  ect Store with t
-00001d10: 6865 202a 2a60 7964 2d64 6f77 6e6c 6f61  he **`yd-downloa
-00001d20: 6460 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  d`** command.- *
-00001d30: 2a41 626f 7274 696e 672a 2a20 7275 6e6e  *Aborting** runn
-00001d40: 696e 6720 5461 736b 7320 7769 7468 2074  ing Tasks with t
-00001d50: 6865 202a 2a60 7964 2d61 626f 7274 602a  he **`yd-abort`*
-00001d60: 2a20 636f 6d6d 616e 640a 2d20 2a2a 4361  * command.- **Ca
-00001d70: 6e63 656c 6c69 6e67 2a2a 2057 6f72 6b20  ncelling** Work 
-00001d80: 5265 7175 6972 656d 656e 7473 2077 6974  Requirements wit
-00001d90: 6820 7468 6520 2a2a 6079 642d 6361 6e63  h the **`yd-canc
-00001da0: 656c 602a 2a20 636f 6d6d 616e 640a 2d20  el`** command.- 
-00001db0: 2a2a 5368 7574 7469 6e67 2044 6f77 6e2a  **Shutting Down*
-00001dc0: 2a20 576f 726b 6572 2050 6f6f 6c73 2077  * Worker Pools w
-00001dd0: 6974 6820 7468 6520 2a2a 6079 642d 7368  ith the **`yd-sh
-00001de0: 7574 646f 776e 602a 2a20 636f 6d6d 616e  utdown`** comman
-00001df0: 640a 2d20 2a2a 5465 726d 696e 6174 696e  d.- **Terminatin
-00001e00: 672a 2a20 436f 6d70 7574 6520 5265 7175  g** Compute Requ
-00001e10: 6972 656d 656e 7473 2077 6974 6820 7468  irements with th
-00001e20: 6520 2a2a 6079 642d 7465 726d 696e 6174  e **`yd-terminat
-00001e30: 6560 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  e`** command.- *
-00001e40: 2a44 656c 6574 696e 672a 2a20 6f62 6a65  *Deleting** obje
-00001e50: 6374 7320 696e 2074 6865 2059 656c 6c6f  cts in the Yello
-00001e60: 7744 6f67 204f 626a 6563 7420 5374 6f72  wDog Object Stor
-00001e70: 6520 7769 7468 2074 6865 202a 2a60 7964  e with the **`yd
-00001e80: 2d64 656c 6574 6560 2a2a 2063 6f6d 6d61  -delete`** comma
-00001e90: 6e64 0a0a 5468 6520 6f70 6572 6174 696f  nd..The operatio
-00001ea0: 6e20 6f66 2074 6865 2063 6f6d 6d61 6e64  n of the command
-00001eb0: 7320 6973 2063 6f6e 7472 6f6c 6c65 6420  s is controlled 
-00001ec0: 7573 696e 6720 544f 4d4c 2063 6f6e 6669  using TOML confi
-00001ed0: 6775 7261 7469 6f6e 2066 696c 6573 2e20  guration files. 
-00001ee0: 496e 2061 6464 6974 696f 6e2c 2057 6f72  In addition, Wor
-00001ef0: 6b20 5265 7175 6972 656d 656e 7473 2061  k Requirements a
-00001f00: 6e64 2057 6f72 6b65 7220 506f 6f6c 7320  nd Worker Pools 
-00001f10: 6361 6e20 6265 2064 6566 696e 6564 2075  can be defined u
-00001f20: 7369 6e67 204a 534f 4e20 6669 6c65 7320  sing JSON files 
-00001f30: 7072 6f76 6964 696e 6720 6578 7465 6e73  providing extens
-00001f40: 6976 6520 636f 6e66 6967 7572 6162 696c  ive configurabil
-00001f50: 6974 792e 0a0a 2320 5965 6c6c 6f77 446f  ity...# YellowDo
-00001f60: 6720 5072 6572 6571 7569 7369 7465 730a  g Prerequisites.
-00001f70: 0a54 6f20 7375 626d 6974 202a 2a57 6f72  .To submit **Wor
-00001f80: 6b20 5265 7175 6972 656d 656e 7473 2a2a  k Requirements**
-00001f90: 2074 6f20 5965 6c6c 6f77 446f 6720 666f   to YellowDog fo
-00001fa0: 7220 7072 6f63 6573 7369 6e67 2062 7920  r processing by 
-00001fb0: 436f 6e66 6967 7572 6564 2057 6f72 6b65  Configured Worke
-00001fc0: 7220 506f 6f6c 7320 286f 6e2d 7072 656d  r Pools (on-prem
-00001fd0: 6973 6529 2061 6e64 2f6f 7220 5072 6f76  ise) and/or Prov
-00001fe0: 6973 696f 6e65 6420 576f 726b 6572 2050  isioned Worker P
-00001ff0: 6f6f 6c73 2028 636c 6f75 642d 7072 6f76  ools (cloud-prov
-00002000: 6973 696f 6e65 6420 7265 736f 7572 6365  isioned resource
-00002010: 7329 2c20 796f 7527 6c6c 206e 6565 643a  s), you'll need:
-00002020: 0a0a 312e 2041 2059 656c 6c6f 7744 6f67  ..1. A YellowDog
-00002030: 2050 6c61 7466 6f72 6d20 4163 636f 756e   Platform Accoun
-00002040: 742e 0a0a 0a32 2e20 416e 2041 7070 6c69  t....2. An Appli
-00002050: 6361 7469 6f6e 204b 6579 2026 2053 6563  cation Key & Sec
-00002060: 7265 743a 2069 6e20 7468 6520 2a2a 4163  ret: in the **Ac
-00002070: 636f 756e 7473 2a2a 2073 6563 7469 6f6e  counts** section
-00002080: 2075 6e64 6572 2074 6865 202a 2a41 7070   under the **App
-00002090: 6c69 6361 7469 6f6e 732a 2a20 7461 6220  lications** tab 
-000020a0: 696e 2074 6865 205b 5965 6c6c 6f77 446f  in the [YellowDo
-000020b0: 6720 506f 7274 616c 5d28 6874 7470 733a  g Portal](https:
-000020c0: 2f2f 706f 7274 616c 2e79 656c 6c6f 7764  //portal.yellowd
-000020d0: 6f67 2e63 6f2f 232f 6163 636f 756e 742f  og.co/#/account/
-000020e0: 6170 706c 6963 6174 696f 6e73 292c 2075  applications), u
-000020f0: 7365 2074 6865 202a 2a41 6464 2041 7070  se the **Add App
-00002100: 6c69 6361 7469 6f6e 2a2a 2062 7574 746f  lication** butto
-00002110: 6e20 746f 2063 7265 6174 6520 6120 6e65  n to create a ne
-00002120: 7720 4170 706c 6963 6174 696f 6e2c 2061  w Application, a
-00002130: 6e64 206d 616b 6520 6120 6e6f 7465 206f  nd make a note o
-00002140: 6620 6974 7320 2a2a 4b65 792a 2a20 616e  f its **Key** an
-00002150: 6420 2a2a 5365 6372 6574 2a2a 2028 7468  d **Secret** (th
-00002160: 6573 6520 7769 6c6c 206f 6e6c 7920 6265  ese will only be
-00002170: 2064 6973 706c 6179 6564 206f 6e63 6529   displayed once)
-00002180: 2e0a 0a0a 546f 2063 7265 6174 6520 2a2a  ....To create **
-00002190: 5072 6f76 6973 696f 6e65 6420 576f 726b  Provisioned Work
-000021a0: 6572 2050 6f6f 6c73 2a2a 2c20 796f 7527  er Pools**, you'
-000021b0: 6c6c 206e 6565 643a 0a0a 332e 2041 202a  ll need:..3. A *
-000021c0: 2a4b 6579 7269 6e67 2a2a 2063 7265 6174  *Keyring** creat
-000021d0: 6564 2076 6961 2074 6865 2059 656c 6c6f  ed via the Yello
-000021e0: 7744 6f67 2050 6f72 7461 6c2c 2077 6974  wDog Portal, wit
-000021f0: 6820 6163 6365 7373 2074 6f20 436c 6f75  h access to Clou
-00002200: 6420 5072 6f76 6964 6572 2063 7265 6465  d Provider crede
-00002210: 6e74 6961 6c73 2061 7320 7265 7175 6972  ntials as requir
-00002220: 6564 2e20 5468 6520 4170 706c 6963 6174  ed. The Applicat
-00002230: 696f 6e20 6d75 7374 2062 6520 6772 616e  ion must be gran
-00002240: 7465 6420 6163 6365 7373 2074 6f20 7468  ted access to th
-00002250: 6520 4b65 7972 696e 672e 0a0a 0a34 2e20  e Keyring....4. 
-00002260: 4f6e 6520 6f72 206d 6f72 6520 2a2a 436f  One or more **Co
-00002270: 6d70 7574 6520 536f 7572 6365 732a 2a20  mpute Sources** 
-00002280: 6465 6669 6e65 642c 2061 6e64 2061 202a  defined, and a *
-00002290: 2a43 6f6d 7075 7465 2052 6571 7569 7265  *Compute Require
-000022a0: 6d65 6e74 2054 656d 706c 6174 652a 2a20  ment Template** 
-000022b0: 6372 6561 7465 642e 2054 6865 2069 6d61  created. The ima
-000022c0: 6765 7320 7573 6564 2062 7920 696e 7374  ges used by inst
-000022d0: 616e 6365 7320 6d75 7374 2069 6e63 6c75  ances must inclu
-000022e0: 6465 2074 6865 2059 656c 6c6f 7744 6f67  de the YellowDog
-000022f0: 2061 6765 6e74 2c20 636f 6e66 6967 7572   agent, configur
-00002300: 6564 2077 6974 6820 7468 6520 5461 736b  ed with the Task
-00002310: 2054 7970 6528 7329 2074 6f20 6d61 7463   Type(s) to matc
-00002320: 6820 7468 6520 576f 726b 2052 6571 7569  h the Work Requi
-00002330: 7265 6d65 6e74 7320 746f 2062 6520 7375  rements to be su
-00002340: 626d 6974 7465 642e 0a0a 546f 2073 6574  bmitted...To set
-00002350: 2075 7020 2a2a 436f 6e66 6967 7572 6564   up **Configured
-00002360: 2057 6f72 6b65 7220 506f 6f6c 732a 2a2c   Worker Pools**,
-00002370: 2079 6f75 276c 6c20 6e65 6564 3a0a 0a35   you'll need:..5
-00002380: 2e20 4120 436f 6e66 6967 7572 6564 2057  . A Configured W
-00002390: 6f72 6b65 7220 506f 6f6c 2054 6f6b 656e  orker Pool Token
-000023a0: 3a20 6672 6f6d 2074 6865 202a 2a57 6f72  : from the **Wor
-000023b0: 6b65 7273 2a2a 2074 6162 2069 6e20 7468  kers** tab in th
-000023c0: 6520 5b59 656c 6c6f 7744 6f67 2050 6f72  e [YellowDog Por
-000023d0: 7461 6c5d 2868 7474 7073 3a2f 2f70 6f72  tal](https://por
-000023e0: 7461 6c2e 7965 6c6c 6f77 646f 672e 636f  tal.yellowdog.co
-000023f0: 2f23 2f77 6f72 6b65 7273 292c 2075 7365  /#/workers), use
-00002400: 2074 6865 202a 2a2b 4164 6420 436f 6e66   the **+Add Conf
-00002410: 6967 7572 6564 2057 6f72 6b65 7220 506f  igured Worker Po
-00002420: 6f6c 2a2a 2062 7574 746f 6e20 746f 2063  ol** button to c
-00002430: 7265 6174 6520 6120 6e65 7720 576f 726b  reate a new Work
-00002440: 6572 2050 6f6f 6c20 616e 6420 6765 6e65  er Pool and gene
-00002450: 7261 7465 2061 2074 6f6b 656e 2e0a 0a0a  rate a token....
-00002460: 362e 204f 6274 6169 6e20 7468 6520 5965  6. Obtain the Ye
-00002470: 6c6c 6f77 446f 6720 4167 656e 7420 616e  llowDog Agent an
-00002480: 6420 696e 7374 616c 6c2f 636f 6e66 6967  d install/config
-00002490: 7572 6520 6974 206f 6e20 796f 7572 206f  ure it on your o
-000024a0: 6e2d 7072 656d 6973 6520 7379 7374 656d  n-premise system
-000024b0: 7320 7573 696e 6720 7468 6520 546f 6b65  s using the Toke
-000024c0: 6e20 6162 6f76 652e 0a0a 2320 5363 7269  n above...# Scri
-000024d0: 7074 2049 6e73 7461 6c6c 6174 696f 6e20  pt Installation 
-000024e0: 7769 7468 2050 6970 0a0a 5079 7468 6f6e  with Pip..Python
-000024f0: 2076 6572 7369 6f6e 2033 2e37 206f 7220   version 3.7 or 
-00002500: 6c61 7465 7220 6973 2072 6571 7569 7265  later is require
-00002510: 642e 2049 7427 7320 7265 636f 6d6d 656e  d. It's recommen
-00002520: 6465 6420 7468 6174 2069 6e73 7461 6c6c  ded that install
-00002530: 6174 696f 6e20 6973 2070 6572 666f 726d  ation is perform
-00002540: 6564 2069 6e20 6120 5079 7468 6f6e 2076  ed in a Python v
-00002550: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00002560: 6e74 2028 6f72 2073 696d 696c 6172 2920  nt (or similar) 
-00002570: 746f 2069 736f 6c61 7465 2074 6865 2069  to isolate the i
-00002580: 6e73 7461 6c6c 6174 696f 6e20 6672 6f6d  nstallation from
-00002590: 206f 7468 6572 2050 7974 686f 6e20 656e   other Python en
-000025a0: 7669 726f 6e6d 656e 7473 206f 6e20 796f  vironments on yo
-000025b0: 7572 2073 7973 7465 6d2e 0a0a 496e 7374  ur system...Inst
-000025c0: 616c 6c61 7469 6f6e 2061 6e64 2073 7562  allation and sub
-000025d0: 7365 7175 656e 7420 7570 6461 7465 2061  sequent update a
-000025e0: 7265 2076 6961 2060 7069 7060 2061 6e64  re via `pip` and
-000025f0: 2050 7950 4920 7573 696e 673a 200a 0a60   PyPI using: ..`
-00002600: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
-00002610: 616c 6c20 2d55 2079 656c 6c6f 7764 6f67  all -U yellowdog
-00002620: 2d70 7974 686f 6e2d 6578 616d 706c 6573  -python-examples
-00002630: 0a60 6060 0a0a 4966 2079 6f75 2772 6520  .```..If you're 
-00002640: 696e 7465 7265 7374 6564 2069 6e20 696e  interested in in
-00002650: 636c 7564 696e 6720 2a2a 4a73 6f6e 6e65  cluding **Jsonne
-00002660: 742a 2a20 7375 7070 6f72 742c 2070 6c65  t** support, ple
-00002670: 6173 6520 7365 6520 7468 6520 5b4a 736f  ase see the [Jso
-00002680: 6e6e 6574 2053 7570 706f 7274 5d28 236a  nnet Support](#j
-00002690: 736f 6e6e 6574 2d73 7570 706f 7274 2920  sonnet-support) 
-000026a0: 7365 6374 696f 6e20 6265 6c6f 772e 0a0a  section below...
-000026b0: 2320 5363 7269 7074 2049 6e73 7461 6c6c  # Script Install
-000026c0: 6174 696f 6e20 7769 7468 2050 6970 780a  ation with Pipx.
-000026d0: 0a54 6865 2063 6f6d 6d61 6e64 7320 6361  .The commands ca
-000026e0: 6e20 616c 736f 2062 6520 696e 7374 616c  n also be instal
-000026f0: 6c65 6420 7573 696e 6720 2a2a 5b70 6970  led using **[pip
-00002700: 785d 2868 7474 7073 3a2f 2f70 7970 612e  x](https://pypa.
-00002710: 6769 7468 7562 2e69 6f2f 7069 7078 2f29  github.io/pipx/)
-00002720: 2a2a 2e0a 0a54 6869 7320 6d65 7468 6f64  **...This method
-00002730: 2072 6571 7569 7265 7320 5079 7468 6f6e   requires Python
-00002740: 2033 2e37 2b20 616e 6420 7069 7078 2074   3.7+ and pipx t
-00002750: 6f20 6265 2069 6e73 7461 6c6c 6564 2e20  o be installed. 
-00002760: 546f 2069 6e73 7461 6c6c 3a0a 6060 6073  To install:.```s
-00002770: 6865 6c6c 0a70 6970 7820 696e 7374 616c  hell.pipx instal
-00002780: 6c20 7965 6c6c 6f77 646f 672d 7079 7468  l yellowdog-pyth
-00002790: 6f6e 2d65 7861 6d70 6c65 730a 6060 600a  on-examples.```.
-000027a0: 0a54 6f20 7570 6461 7465 3a0a 6060 6073  .To update:.```s
-000027b0: 6865 6c6c 0a70 6970 7820 7570 6772 6164  hell.pipx upgrad
-000027c0: 6520 7965 6c6c 6f77 646f 672d 7079 7468  e yellowdog-pyth
-000027d0: 6f6e 2d65 7861 6d70 6c65 730a 6060 600a  on-examples.```.
-000027e0: 0a23 2055 7361 6765 0a0a 426f 7468 206f  .# Usage..Both o
-000027f0: 6620 7468 6520 696e 7374 616c 6c61 7469  f the installati
-00002800: 6f6e 206d 6574 686f 6473 2061 626f 7665  on methods above
-00002810: 2077 696c 6c20 696e 7374 616c 6c20 6120   will install a 
-00002820: 6e75 6d62 6572 206f 6620 2a2a 6079 642d  number of **`yd-
-00002830: 602a 2a20 636f 6d6d 616e 6473 206f 6e20  `** commands on 
-00002840: 796f 7572 2050 4154 482e 0a0a 436f 6d6d  your PATH...Comm
-00002850: 616e 6473 2061 7265 2072 756e 2066 726f  ands are run fro
-00002860: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
-00002870: 6e65 2e20 496e 766f 6b69 6e67 2074 6865  ne. Invoking the
-00002880: 2063 6f6d 6d61 6e64 2077 6974 6820 7468   command with th
-00002890: 6520 602d 2d68 656c 7060 206f 7220 602d  e `--help` or `-
-000028a0: 6860 206f 7074 696f 6e20 7769 6c6c 2064  h` option will d
-000028b0: 6973 706c 6179 2074 6865 2063 6f6d 6d61  isplay the comma
-000028c0: 6e64 206c 696e 6520 6f70 7469 6f6e 7320  nd line options 
-000028d0: 6170 706c 6963 6162 6c65 2074 6f20 6120  applicable to a 
-000028e0: 6769 7665 6e20 636f 6d6d 616e 642c 2065  given command, e
-000028f0: 2e67 2e3a 0a0a 6060 6074 6578 740a 2025  .g.:..```text. %
-00002900: 2079 642d 6361 6e63 656c 202d 2d68 656c   yd-cancel --hel
-00002910: 700a 7573 6167 653a 2079 642d 6361 6e63  p.usage: yd-canc
-00002920: 656c 205b 2d68 5d20 5b2d 2d64 6f63 735d  el [-h] [--docs]
-00002930: 205b 2d2d 636f 6e66 6967 203c 636f 6e66   [--config <conf
-00002940: 6967 5f66 696c 652e 746f 6d6c 3e5d 205b  ig_file.toml>] [
-00002950: 2d2d 6b65 7920 3c61 7070 2d6b 6579 3e5d  --key <app-key>]
-00002960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002970: 2020 5b2d 2d73 6563 7265 7420 3c61 7070    [--secret <app
-00002980: 2d73 6563 7265 743e 5d20 5b2d 2d6e 616d  -secret>] [--nam
-00002990: 6573 7061 6365 203c 6e61 6d65 7370 6163  espace <namespac
-000029a0: 653e 5d20 5b2d 2d74 6167 203c 7461 673e  e>] [--tag <tag>
-000029b0: 5d20 5b2d 2d75 726c 203c 7572 6c3e 5d0a  ] [--url <url>].
+00000bc0: 6573 2d6c 6973 7429 0a20 2020 2020 2020  es-list).       
+00000bd0: 2020 2a20 5b55 7369 6e67 2057 696c 6463    * [Using Wildc
+00000be0: 6172 6473 2069 6e20 7468 6520 7570 6c6f  ards in the uplo
+00000bf0: 6164 4669 6c65 7320 4c69 7374 5d28 2375  adFiles List](#u
+00000c00: 7369 6e67 2d77 696c 6463 6172 6473 2d69  sing-wildcards-i
+00000c10: 6e2d 7468 652d 7570 6c6f 6164 6669 6c65  n-the-uploadfile
+00000c20: 732d 6c69 7374 290a 2020 2020 2020 2a20  s-list).      * 
+00000c30: 5b46 696c 6520 4465 7065 6e64 656e 6369  [File Dependenci
+00000c40: 6573 2055 7369 6e67 2076 6572 6966 7941  es Using verifyA
+00000c50: 7453 7461 7274 2061 6e64 2076 6572 6966  tStart and verif
+00000c60: 7957 6169 745d 2823 6669 6c65 2d64 6570  yWait](#file-dep
+00000c70: 656e 6465 6e63 6965 732d 7573 696e 672d  endencies-using-
+00000c80: 7665 7269 6679 6174 7374 6172 742d 616e  verifyatstart-an
+00000c90: 642d 7665 7269 6679 7761 6974 290a 2020  d-verifywait).  
+00000ca0: 2020 2020 2a20 5b46 696c 6573 2044 6f77      * [Files Dow
+00000cb0: 6e6c 6f61 6465 6420 5573 696e 6720 696e  nloaded Using in
+00000cc0: 7075 7473 4f70 7469 6f6e 616c 5d28 2366  putsOptional](#f
+00000cd0: 696c 6573 2d64 6f77 6e6c 6f61 6465 642d  iles-downloaded-
+00000ce0: 7573 696e 672d 696e 7075 7473 6f70 7469  using-inputsopti
+00000cf0: 6f6e 616c 290a 2020 2020 2020 2a20 5b46  onal).      * [F
+00000d00: 696c 6573 2044 6f77 6e6c 6f61 6465 6420  iles Downloaded 
+00000d10: 746f 2061 204e 6f64 6520 666f 7220 7573  to a Node for us
+00000d20: 6520 696e 2054 6173 6b20 4578 6563 7574  e in Task Execut
+00000d30: 696f 6e5d 2823 6669 6c65 732d 646f 776e  ion](#files-down
+00000d40: 6c6f 6164 6564 2d74 6f2d 612d 6e6f 6465  loaded-to-a-node
+00000d50: 2d66 6f72 2d75 7365 2d69 6e2d 7461 736b  -for-use-in-task
+00000d60: 2d65 7865 6375 7469 6f6e 290a 2020 2020  -execution).    
+00000d70: 2020 2a20 5b46 696c 6573 2055 706c 6f61    * [Files Uploa
+00000d80: 6465 6420 6672 6f6d 2061 204e 6f64 6520  ded from a Node 
+00000d90: 746f 2074 6865 204f 626a 6563 7420 5374  to the Object St
+00000da0: 6f72 6520 6166 7465 7220 5461 736b 2045  ore after Task E
+00000db0: 7865 6375 7469 6f6e 5d28 2366 696c 6573  xecution](#files
+00000dc0: 2d75 706c 6f61 6465 642d 6672 6f6d 2d61  -uploaded-from-a
+00000dd0: 2d6e 6f64 652d 746f 2d74 6865 2d6f 626a  -node-to-the-obj
+00000de0: 6563 742d 7374 6f72 652d 6166 7465 722d  ect-store-after-
+00000df0: 7461 736b 2d65 7865 6375 7469 6f6e 290a  task-execution).
+00000e00: 2020 2020 2020 2a20 5b46 696c 6573 2044        * [Files D
+00000e10: 6f77 6e6c 6f61 6465 6420 6672 6f6d 2074  ownloaded from t
+00000e20: 6865 204f 626a 6563 7420 5374 6f72 6520  he Object Store 
+00000e30: 746f 204c 6f63 616c 2053 746f 7261 6765  to Local Storage
+00000e40: 5d28 2366 696c 6573 2d64 6f77 6e6c 6f61  ](#files-downloa
+00000e50: 6465 642d 6672 6f6d 2d74 6865 2d6f 626a  ded-from-the-obj
+00000e60: 6563 742d 7374 6f72 652d 746f 2d6c 6f63  ect-store-to-loc
+00000e70: 616c 2d73 746f 7261 6765 290a 2020 202a  al-storage).   *
+00000e80: 205b 5461 736b 2045 7865 6375 7469 6f6e   [Task Execution
+00000e90: 2043 6f6e 7465 7874 5d28 2374 6173 6b2d   Context](#task-
+00000ea0: 6578 6563 7574 696f 6e2d 636f 6e74 6578  execution-contex
+00000eb0: 7429 0a20 2020 2020 202a 205b 5461 736b  t).      * [Task
+00000ec0: 2045 7865 6375 7469 6f6e 2053 7465 7073   Execution Steps
+00000ed0: 5d28 2374 6173 6b2d 6578 6563 7574 696f  ](#task-executio
+00000ee0: 6e2d 7374 6570 7329 0a20 2020 2020 202a  n-steps).      *
+00000ef0: 205b 5468 6520 5573 6572 2061 6e64 2047   [The User and G
+00000f00: 726f 7570 2075 7365 6420 666f 7220 5461  roup used for Ta
+00000f10: 736b 735d 2823 7468 652d 7573 6572 2d61  sks](#the-user-a
+00000f20: 6e64 2d67 726f 7570 2d75 7365 642d 666f  nd-group-used-fo
+00000f30: 722d 7461 736b 7329 0a20 2020 2020 202a  r-tasks).      *
+00000f40: 205b 486f 6d65 2044 6972 6563 746f 7279   [Home Directory
+00000f50: 2066 6f72 2079 642d 6167 656e 745d 2823   for yd-agent](#
+00000f60: 686f 6d65 2d64 6972 6563 746f 7279 2d66  home-directory-f
+00000f70: 6f72 2d79 642d 6167 656e 7429 0a20 2020  or-yd-agent).   
+00000f80: 2020 202a 205b 5461 736b 2045 7865 6375     * [Task Execu
+00000f90: 7469 6f6e 2044 6972 6563 746f 7279 5d28  tion Directory](
+00000fa0: 2374 6173 6b2d 6578 6563 7574 696f 6e2d  #task-execution-
+00000fb0: 6469 7265 6374 6f72 7929 0a20 2020 2a20  directory).   * 
+00000fc0: 5b53 7065 6369 6679 696e 6720 576f 726b  [Specifying Work
+00000fd0: 2052 6571 7569 7265 6d65 6e74 7320 7573   Requirements us
+00000fe0: 696e 6720 4353 5620 4461 7461 5d28 2373  ing CSV Data](#s
+00000ff0: 7065 6369 6679 696e 672d 776f 726b 2d72  pecifying-work-r
+00001000: 6571 7569 7265 6d65 6e74 732d 7573 696e  equirements-usin
+00001010: 672d 6373 762d 6461 7461 290a 2020 2020  g-csv-data).    
+00001020: 2020 2a20 5b57 6f72 6b20 5265 7175 6972    * [Work Requir
+00001030: 656d 656e 7420 4353 5620 4461 7461 2045  ement CSV Data E
+00001040: 7861 6d70 6c65 5d28 2377 6f72 6b2d 7265  xample](#work-re
+00001050: 7175 6972 656d 656e 742d 6373 762d 6461  quirement-csv-da
+00001060: 7461 2d65 7861 6d70 6c65 290a 2020 2020  ta-example).    
+00001070: 2020 2a20 5b43 5356 2056 6172 6961 626c    * [CSV Variabl
+00001080: 6520 5375 6273 7469 7475 7469 6f6e 735d  e Substitutions]
+00001090: 2823 6373 762d 7661 7269 6162 6c65 2d73  (#csv-variable-s
+000010a0: 7562 7374 6974 7574 696f 6e73 290a 2020  ubstitutions).  
+000010b0: 2020 2020 2a20 5b50 726f 7065 7274 7920      * [Property 
+000010c0: 496e 6865 7269 7461 6e63 655d 2823 7072  Inheritance](#pr
+000010d0: 6f70 6572 7479 2d69 6e68 6572 6974 616e  operty-inheritan
+000010e0: 6365 2d31 290a 2020 2020 2020 2a20 5b4d  ce-1).      * [M
+000010f0: 756c 7469 706c 6520 5461 736b 2047 726f  ultiple Task Gro
+00001100: 7570 7320 7573 696e 6720 4d75 6c74 6970  ups using Multip
+00001110: 6c65 2043 5356 2046 696c 6573 5d28 236d  le CSV Files](#m
+00001120: 756c 7469 706c 652d 7461 736b 2d67 726f  ultiple-task-gro
+00001130: 7570 732d 7573 696e 672d 6d75 6c74 6970  ups-using-multip
+00001140: 6c65 2d63 7376 2d66 696c 6573 290a 2020  le-csv-files).  
+00001150: 2020 2020 2a20 5b55 7369 6e67 2043 5356      * [Using CSV
+00001160: 2044 6174 6120 7769 7468 2053 696d 706c   Data with Simpl
+00001170: 652c 2054 4f4d 4c2d 4f6e 6c79 2057 6f72  e, TOML-Only Wor
+00001180: 6b20 5265 7175 6972 656d 656e 7420 5370  k Requirement Sp
+00001190: 6563 6966 6963 6174 696f 6e73 5d28 2375  ecifications](#u
+000011a0: 7369 6e67 2d63 7376 2d64 6174 612d 7769  sing-csv-data-wi
+000011b0: 7468 2d73 696d 706c 652d 746f 6d6c 2d6f  th-simple-toml-o
+000011c0: 6e6c 792d 776f 726b 2d72 6571 7569 7265  nly-work-require
+000011d0: 6d65 6e74 2d73 7065 6369 6669 6361 7469  ment-specificati
+000011e0: 6f6e 7329 0a20 2020 2020 202a 205b 496e  ons).      * [In
+000011f0: 7370 6563 7469 6e67 2074 6865 2052 6573  specting the Res
+00001200: 756c 7473 206f 6620 4353 5620 5661 7269  ults of CSV Vari
+00001210: 6162 6c65 2053 7562 7374 6974 7574 696f  able Substitutio
+00001220: 6e5d 2823 696e 7370 6563 7469 6e67 2d74  n](#inspecting-t
+00001230: 6865 2d72 6573 756c 7473 2d6f 662d 6373  he-results-of-cs
+00001240: 762d 7661 7269 6162 6c65 2d73 7562 7374  v-variable-subst
+00001250: 6974 7574 696f 6e29 0a2a 205b 576f 726b  itution).* [Work
+00001260: 6572 2050 6f6f 6c20 5072 6f70 6572 7469  er Pool Properti
+00001270: 6573 5d28 2377 6f72 6b65 722d 706f 6f6c  es](#worker-pool
+00001280: 2d70 726f 7065 7274 6965 7329 0a20 2020  -properties).   
+00001290: 2a20 5b41 7574 6f6d 6174 6963 2050 726f  * [Automatic Pro
+000012a0: 7065 7274 6965 735d 2823 6175 746f 6d61  perties](#automa
+000012b0: 7469 632d 7072 6f70 6572 7469 6573 2d31  tic-properties-1
+000012c0: 290a 2020 202a 205b 544f 4d4c 2050 726f  ).   * [TOML Pro
+000012d0: 7065 7274 6965 7320 696e 2074 6865 2077  perties in the w
+000012e0: 6f72 6b65 7250 6f6f 6c20 5365 6374 696f  orkerPool Sectio
+000012f0: 6e5d 2823 746f 6d6c 2d70 726f 7065 7274  n](#toml-propert
+00001300: 6965 732d 696e 2d74 6865 2d77 6f72 6b65  ies-in-the-worke
+00001310: 7270 6f6f 6c2d 7365 6374 696f 6e29 0a20  rpool-section). 
+00001320: 2020 2a20 5b57 6f72 6b65 7220 506f 6f6c    * [Worker Pool
+00001330: 2053 7065 6369 6669 6361 7469 6f6e 2055   Specification U
+00001340: 7369 6e67 204a 534f 4e20 446f 6375 6d65  sing JSON Docume
+00001350: 6e74 735d 2823 776f 726b 6572 2d70 6f6f  nts](#worker-poo
+00001360: 6c2d 7370 6563 6966 6963 6174 696f 6e2d  l-specification-
+00001370: 7573 696e 672d 6a73 6f6e 2d64 6f63 756d  using-json-docum
+00001380: 656e 7473 290a 2020 2020 2020 2a20 5b57  ents).      * [W
+00001390: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
+000013a0: 4578 616d 706c 6573 5d28 2377 6f72 6b65  Examples](#worke
+000013b0: 722d 706f 6f6c 2d6a 736f 6e2d 6578 616d  r-pool-json-exam
+000013c0: 706c 6573 290a 2020 2020 2020 2a20 5b54  ples).      * [T
+000013d0: 4f4d 4c20 5072 6f70 6572 7469 6573 2049  OML Properties I
+000013e0: 6e68 6572 6974 6564 2062 7920 576f 726b  nherited by Work
+000013f0: 6572 2050 6f6f 6c20 4a53 4f4e 2053 7065  er Pool JSON Spe
+00001400: 6369 6669 6361 7469 6f6e 735d 2823 746f  cifications](#to
+00001410: 6d6c 2d70 726f 7065 7274 6965 732d 696e  ml-properties-in
+00001420: 6865 7269 7465 642d 6279 2d77 6f72 6b65  herited-by-worke
+00001430: 722d 706f 6f6c 2d6a 736f 6e2d 7370 6563  r-pool-json-spec
+00001440: 6966 6963 6174 696f 6e73 290a 2020 202a  ifications).   *
+00001450: 205b 5661 7269 6162 6c65 2053 7562 7374   [Variable Subst
+00001460: 6974 7574 696f 6e73 2069 6e20 576f 726b  itutions in Work
+00001470: 6572 2050 6f6f 6c20 5072 6f70 6572 7469  er Pool Properti
+00001480: 6573 5d28 2376 6172 6961 626c 652d 7375  es](#variable-su
+00001490: 6273 7469 7475 7469 6f6e 732d 696e 2d77  bstitutions-in-w
+000014a0: 6f72 6b65 722d 706f 6f6c 2d70 726f 7065  orker-pool-prope
+000014b0: 7274 6965 7329 0a20 2020 2a20 5b44 7279  rties).   * [Dry
+000014c0: 2d52 756e 6e69 6e67 2057 6f72 6b65 7220  -Running Worker 
+000014d0: 506f 6f6c 2050 726f 7669 7369 6f6e 696e  Pool Provisionin
+000014e0: 675d 2823 6472 792d 7275 6e6e 696e 672d  g](#dry-running-
+000014f0: 776f 726b 6572 2d70 6f6f 6c2d 7072 6f76  worker-pool-prov
+00001500: 6973 696f 6e69 6e67 290a 2a20 5b4a 736f  isioning).* [Jso
+00001510: 6e6e 6574 2053 7570 706f 7274 5d28 236a  nnet Support](#j
+00001520: 736f 6e6e 6574 2d73 7570 706f 7274 290a  sonnet-support).
+00001530: 2020 202a 205b 4a73 6f6e 6e65 7420 496e     * [Jsonnet In
+00001540: 7374 616c 6c61 7469 6f6e 5d28 236a 736f  stallation](#jso
+00001550: 6e6e 6574 2d69 6e73 7461 6c6c 6174 696f  nnet-installatio
+00001560: 6e29 0a20 2020 2a20 5b56 6172 6961 626c  n).   * [Variabl
+00001570: 6520 5375 6273 7469 7475 7469 6f6e 7320  e Substitutions 
+00001580: 696e 204a 736f 6e6e 6574 2046 696c 6573  in Jsonnet Files
+00001590: 5d28 2376 6172 6961 626c 652d 7375 6273  ](#variable-subs
+000015a0: 7469 7475 7469 6f6e 732d 696e 2d6a 736f  titutions-in-jso
+000015b0: 6e6e 6574 2d66 696c 6573 290a 2020 202a  nnet-files).   *
+000015c0: 205b 4368 6563 6b69 6e67 204a 736f 6e6e   [Checking Jsonn
+000015d0: 6574 2050 726f 6365 7373 696e 675d 2823  et Processing](#
+000015e0: 6368 6563 6b69 6e67 2d6a 736f 6e6e 6574  checking-jsonnet
+000015f0: 2d70 726f 6365 7373 696e 6729 0a20 2020  -processing).   
+00001600: 2a20 5b4a 736f 6e6e 6574 2045 7861 6d70  * [Jsonnet Examp
+00001610: 6c65 5d28 236a 736f 6e6e 6574 2d65 7861  le](#jsonnet-exa
+00001620: 6d70 6c65 290a 2a20 5b43 6f6d 6d61 6e64  mple).* [Command
+00001630: 204c 6973 745d 2823 636f 6d6d 616e 642d   List](#command-
+00001640: 6c69 7374 290a 2020 202a 205b 7964 2d73  list).   * [yd-s
+00001650: 7562 6d69 745d 2823 7964 2d73 7562 6d69  ubmit](#yd-submi
+00001660: 7429 0a20 2020 2a20 5b79 642d 7072 6f76  t).   * [yd-prov
+00001670: 6973 696f 6e5d 2823 7964 2d70 726f 7669  ision](#yd-provi
+00001680: 7369 6f6e 290a 2020 202a 205b 7964 2d63  sion).   * [yd-c
+00001690: 616e 6365 6c5d 2823 7964 2d63 616e 6365  ancel](#yd-cance
+000016a0: 6c29 0a20 2020 2a20 5b79 642d 6162 6f72  l).   * [yd-abor
+000016b0: 745d 2823 7964 2d61 626f 7274 290a 2020  t](#yd-abort).  
+000016c0: 202a 205b 7964 2d64 6f77 6e6c 6f61 645d   * [yd-download]
+000016d0: 2823 7964 2d64 6f77 6e6c 6f61 6429 0a20  (#yd-download). 
+000016e0: 2020 2a20 5b79 642d 6465 6c65 7465 5d28    * [yd-delete](
+000016f0: 2379 642d 6465 6c65 7465 290a 2020 202a  #yd-delete).   *
+00001700: 205b 7964 2d75 706c 6f61 645d 2823 7964   [yd-upload](#yd
+00001710: 2d75 706c 6f61 6429 0a20 2020 2a20 5b79  -upload).   * [y
+00001720: 642d 7368 7574 646f 776e 5d28 2379 642d  d-shutdown](#yd-
+00001730: 7368 7574 646f 776e 290a 2020 202a 205b  shutdown).   * [
+00001740: 7964 2d69 6e73 7461 6e74 6961 7465 5d28  yd-instantiate](
+00001750: 2379 642d 696e 7374 616e 7469 6174 6529  #yd-instantiate)
+00001760: 0a20 2020 2020 202a 205b 5465 7374 2d52  .      * [Test-R
+00001770: 756e 6e69 6e67 2061 2044 796e 616d 6963  unning a Dynamic
+00001780: 2054 656d 706c 6174 655d 2823 7465 7374   Template](#test
+00001790: 2d72 756e 6e69 6e67 2d61 2d64 796e 616d  -running-a-dynam
+000017a0: 6963 2d74 656d 706c 6174 6529 0a20 2020  ic-template).   
+000017b0: 2a20 5b79 642d 7465 726d 696e 6174 655d  * [yd-terminate]
+000017c0: 2823 7964 2d74 6572 6d69 6e61 7465 290a  (#yd-terminate).
+000017d0: 0a3c 212d 2d20 4164 6465 6420 6279 3a20  .<!-- Added by: 
+000017e0: 7077 742c 2061 743a 204d 6f6e 204a 756e  pwt, at: Mon Jun
+000017f0: 2032 3620 3135 3a33 393a 3436 2042 5354   26 15:39:46 BST
+00001800: 2032 3032 3320 2d2d 3e0a 0a3c 212d 2d74   2023 -->..<!--t
+00001810: 652d 2d3e 0a0a 2320 4f76 6572 7669 6577  e-->..# Overview
+00001820: 0a0a 5468 6973 2072 6570 6f73 6974 6f72  ..This repositor
+00001830: 7920 636f 6e74 6169 6e73 2061 2073 6574  y contains a set
+00001840: 206f 6620 6578 616d 706c 6520 5079 7468   of example Pyth
+00001850: 6f6e 2073 6372 6970 7473 2066 6f72 2069  on scripts for i
+00001860: 6e74 6572 6163 7469 6e67 2077 6974 6820  nteracting with 
+00001870: 7468 6520 5965 6c6c 6f77 446f 6720 506c  the YellowDog Pl
+00001880: 6174 666f 726d 2e20 5468 6520 7363 7269  atform. The scri
+00001890: 7074 7320 7573 6520 7468 6520 2a2a 5b59  pts use the **[Y
+000018a0: 656c 6c6f 7744 6f67 2050 7974 686f 6e20  ellowDog Python 
+000018b0: 5344 4b5d 2868 7474 7073 3a2f 2f64 6f63  SDK](https://doc
+000018c0: 732e 7965 6c6c 6f77 646f 672e 636f 2f61  s.yellowdog.co/a
+000018d0: 7069 2f70 7974 686f 6e2f 696e 6465 782e  pi/python/index.
+000018e0: 6874 6d6c 292a 2a2c 2074 6865 2063 6f64  html)**, the cod
+000018f0: 6520 666f 7220 7768 6963 6820 6361 6e20  e for which can 
+00001900: 6265 2066 6f75 6e64 205b 6f6e 2047 6974  be found [on Git
+00001910: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00001920: 6875 622e 636f 6d2f 7965 6c6c 6f77 646f  hub.com/yellowdo
+00001930: 672f 7965 6c6c 6f77 646f 672d 7364 6b2d  g/yellowdog-sdk-
+00001940: 7079 7468 6f6e 2d70 7562 6c69 6329 2e0a  python-public)..
+00001950: 0a0a 2a28 4e6f 7465 3a20 7468 6573 6520  ..*(Note: these 
+00001960: 7363 7269 7074 7320 6172 6520 696e 7465  scripts are inte
+00001970: 6e64 6564 2074 6f20 6265 2061 2068 656c  nded to be a hel
+00001980: 7066 756c 2073 7461 7274 696e 6720 706f  pful starting po
+00001990: 696e 7420 666f 7220 6578 7065 7269 6d65  int for experime
+000019a0: 6e74 696e 6720 7769 7468 2074 6865 2059  nting with the Y
+000019b0: 656c 6c6f 7744 6f67 2050 6c61 7466 6f72  ellowDog Platfor
+000019c0: 6d2e 2054 6865 7920 6172 6520 6e6f 7420  m. They are not 
+000019d0: 6173 7375 7265 6420 746f 2062 6520 6f66  assured to be of
+000019e0: 2070 726f 6475 6374 696f 6e20 7175 616c   production qual
+000019f0: 6974 7920 6e6f 7220 646f 2074 6865 7920  ity nor do they 
+00001a00: 7265 7072 6573 656e 7420 6120 7374 616e  represent a stan
+00001a10: 6461 7264 206f 7220 7265 636f 6d6d 656e  dard or recommen
+00001a20: 6465 6420 6d65 7468 6f64 2066 6f72 2075  ded method for u
+00001a30: 7369 6e67 2059 656c 6c6f 7744 6f67 2e29  sing YellowDog.)
+00001a40: 2a0a 0a54 6869 7320 646f 6375 6d65 6e74  *..This document
+00001a50: 6174 696f 6e20 7368 6f75 6c64 2062 6520  ation should be 
+00001a60: 7265 6164 2069 6e20 636f 6e6a 756e 6374  read in conjunct
+00001a70: 696f 6e20 7769 7468 2074 6865 206d 6169  ion with the mai
+00001a80: 6e20 2a2a 5b59 656c 6c6f 7744 6f67 2044  n **[YellowDog D
+00001a90: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00001aa0: 7470 733a 2f2f 646f 6373 2e79 656c 6c6f  tps://docs.yello
+00001ab0: 7764 6f67 2e63 6f29 2a2a 2c20 7768 6963  wdog.co)**, whic
+00001ac0: 6820 7072 6f76 6964 6573 2061 2063 6f6d  h provides a com
+00001ad0: 7072 6568 656e 7369 7665 2064 6573 6372  prehensive descr
+00001ae0: 6970 7469 6f6e 206f 6620 7468 6520 636f  iption of the co
+00001af0: 6e63 6570 7473 2061 6e64 206f 7065 7261  ncepts and opera
+00001b00: 7469 6f6e 206f 6620 7468 6520 5965 6c6c  tion of the Yell
+00001b10: 6f77 446f 6720 506c 6174 666f 726d 2e0a  owDog Platform..
+00001b20: 0a54 656d 706c 6174 6520 736f 6c75 7469  .Template soluti
+00001b30: 6f6e 7320 666f 7220 6578 7065 7269 6d65  ons for experime
+00001b40: 6e74 696e 6720 7769 7468 2074 6865 7365  nting with these
+00001b50: 2073 6372 6970 7473 2063 616e 2062 6520   scripts can be 
+00001b60: 666f 756e 6420 696e 2074 6865 202a 2a5b  found in the **[
+00001b70: 7079 7468 6f6e 2d65 7861 6d70 6c65 732d  python-examples-
+00001b80: 7465 6d70 6c61 7465 735d 2868 7474 7073  templates](https
+00001b90: 3a2f 2f67 6974 6875 622e 636f 6d2f 7965  ://github.com/ye
+00001ba0: 6c6c 6f77 646f 672f 7079 7468 6f6e 2d65  llowdog/python-e
+00001bb0: 7861 6d70 6c65 732d 7465 6d70 6c61 7465  xamples-template
+00001bc0: 7329 2a2a 2072 6570 6f73 6974 6f72 792e  s)** repository.
+00001bd0: 0a0a 5468 6520 7363 7269 7074 7320 7072  ..The scripts pr
+00001be0: 6f76 6964 6520 7468 6520 666f 6c6c 6f77  ovide the follow
+00001bf0: 696e 6720 6361 7061 6269 6c69 7469 6573  ing capabilities
+00001c00: 3a0a 0a2d 202a 2a50 726f 7669 7369 6f6e  :..- **Provision
+00001c10: 696e 672a 2a20 576f 726b 6572 2050 6f6f  ing** Worker Poo
+00001c20: 6c73 2077 6974 6820 7468 6520 2a2a 6079  ls with the **`y
+00001c30: 642d 7072 6f76 6973 696f 6e60 2a2a 2063  d-provision`** c
+00001c40: 6f6d 6d61 6e64 0a2d 202a 2a53 7562 6d69  ommand.- **Submi
+00001c50: 7474 696e 672a 2a20 576f 726b 2052 6571  tting** Work Req
+00001c60: 7569 7265 6d65 6e74 7320 7769 7468 2074  uirements with t
+00001c70: 6865 202a 2a60 7964 2d73 7562 6d69 7460  he **`yd-submit`
+00001c80: 2a2a 2063 6f6d 6d61 6e64 0a2d 202a 2a55  ** command.- **U
+00001c90: 706c 6f61 6469 6e67 2a2a 2066 696c 6573  ploading** files
+00001ca0: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
+00001cb0: 6720 4f62 6a65 6374 2053 746f 7265 2077  g Object Store w
+00001cc0: 6974 6820 7468 6520 2a2a 6079 642d 7570  ith the **`yd-up
+00001cd0: 6c6f 6164 602a 2a20 636f 6d6d 616e 640a  load`** command.
+00001ce0: 2d20 2a2a 496e 7374 616e 7469 6174 696e  - **Instantiatin
+00001cf0: 672a 2a20 436f 6d70 7574 6520 5265 7175  g** Compute Requ
+00001d00: 6972 656d 656e 7473 2077 6974 6820 7468  irements with th
+00001d10: 6520 2a2a 6079 642d 696e 7374 616e 7469  e **`yd-instanti
+00001d20: 6174 6560 2a2a 2063 6f6d 6d61 6e64 0a2d  ate`** command.-
+00001d30: 202a 2a44 6f77 6e6c 6f61 6469 6e67 2a2a   **Downloading**
+00001d40: 2052 6573 756c 7473 2066 726f 6d20 7468   Results from th
+00001d50: 6520 5965 6c6c 6f77 446f 6720 4f62 6a65  e YellowDog Obje
+00001d60: 6374 2053 746f 7265 2077 6974 6820 7468  ct Store with th
+00001d70: 6520 2a2a 6079 642d 646f 776e 6c6f 6164  e **`yd-download
+00001d80: 602a 2a20 636f 6d6d 616e 640a 2d20 2a2a  `** command.- **
+00001d90: 4162 6f72 7469 6e67 2a2a 2072 756e 6e69  Aborting** runni
+00001da0: 6e67 2054 6173 6b73 2077 6974 6820 7468  ng Tasks with th
+00001db0: 6520 2a2a 6079 642d 6162 6f72 7460 2a2a  e **`yd-abort`**
+00001dc0: 2063 6f6d 6d61 6e64 0a2d 202a 2a43 616e   command.- **Can
+00001dd0: 6365 6c6c 696e 672a 2a20 576f 726b 2052  celling** Work R
+00001de0: 6571 7569 7265 6d65 6e74 7320 7769 7468  equirements with
+00001df0: 2074 6865 202a 2a60 7964 2d63 616e 6365   the **`yd-cance
+00001e00: 6c60 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  l`** command.- *
+00001e10: 2a53 6875 7474 696e 6720 446f 776e 2a2a  *Shutting Down**
+00001e20: 2057 6f72 6b65 7220 506f 6f6c 7320 7769   Worker Pools wi
+00001e30: 7468 2074 6865 202a 2a60 7964 2d73 6875  th the **`yd-shu
+00001e40: 7464 6f77 6e60 2a2a 2063 6f6d 6d61 6e64  tdown`** command
+00001e50: 0a2d 202a 2a54 6572 6d69 6e61 7469 6e67  .- **Terminating
+00001e60: 2a2a 2043 6f6d 7075 7465 2052 6571 7569  ** Compute Requi
+00001e70: 7265 6d65 6e74 7320 7769 7468 2074 6865  rements with the
+00001e80: 202a 2a60 7964 2d74 6572 6d69 6e61 7465   **`yd-terminate
+00001e90: 602a 2a20 636f 6d6d 616e 640a 2d20 2a2a  `** command.- **
+00001ea0: 4465 6c65 7469 6e67 2a2a 206f 626a 6563  Deleting** objec
+00001eb0: 7473 2069 6e20 7468 6520 5965 6c6c 6f77  ts in the Yellow
+00001ec0: 446f 6720 4f62 6a65 6374 2053 746f 7265  Dog Object Store
+00001ed0: 2077 6974 6820 7468 6520 2a2a 6079 642d   with the **`yd-
+00001ee0: 6465 6c65 7465 602a 2a20 636f 6d6d 616e  delete`** comman
+00001ef0: 640a 0a54 6865 206f 7065 7261 7469 6f6e  d..The operation
+00001f00: 206f 6620 7468 6520 636f 6d6d 616e 6473   of the commands
+00001f10: 2069 7320 636f 6e74 726f 6c6c 6564 2075   is controlled u
+00001f20: 7369 6e67 2054 4f4d 4c20 636f 6e66 6967  sing TOML config
+00001f30: 7572 6174 696f 6e20 6669 6c65 732e 2049  uration files. I
+00001f40: 6e20 6164 6469 7469 6f6e 2c20 576f 726b  n addition, Work
+00001f50: 2052 6571 7569 7265 6d65 6e74 7320 616e   Requirements an
+00001f60: 6420 576f 726b 6572 2050 6f6f 6c73 2063  d Worker Pools c
+00001f70: 616e 2062 6520 6465 6669 6e65 6420 7573  an be defined us
+00001f80: 696e 6720 4a53 4f4e 2066 696c 6573 2070  ing JSON files p
+00001f90: 726f 7669 6469 6e67 2065 7874 656e 7369  roviding extensi
+00001fa0: 7665 2063 6f6e 6669 6775 7261 6269 6c69  ve configurabili
+00001fb0: 7479 2e0a 0a23 2059 656c 6c6f 7744 6f67  ty...# YellowDog
+00001fc0: 2050 7265 7265 7175 6973 6974 6573 0a0a   Prerequisites..
+00001fd0: 546f 2073 7562 6d69 7420 2a2a 576f 726b  To submit **Work
+00001fe0: 2052 6571 7569 7265 6d65 6e74 732a 2a20   Requirements** 
+00001ff0: 746f 2059 656c 6c6f 7744 6f67 2066 6f72  to YellowDog for
+00002000: 2070 726f 6365 7373 696e 6720 6279 2043   processing by C
+00002010: 6f6e 6669 6775 7265 6420 576f 726b 6572  onfigured Worker
+00002020: 2050 6f6f 6c73 2028 6f6e 2d70 7265 6d69   Pools (on-premi
+00002030: 7365 2920 616e 642f 6f72 2050 726f 7669  se) and/or Provi
+00002040: 7369 6f6e 6564 2057 6f72 6b65 7220 506f  sioned Worker Po
+00002050: 6f6c 7320 2863 6c6f 7564 2d70 726f 7669  ols (cloud-provi
+00002060: 7369 6f6e 6564 2072 6573 6f75 7263 6573  sioned resources
+00002070: 292c 2079 6f75 276c 6c20 6e65 6564 3a0a  ), you'll need:.
+00002080: 0a31 2e20 4120 5965 6c6c 6f77 446f 6720  .1. A YellowDog 
+00002090: 506c 6174 666f 726d 2041 6363 6f75 6e74  Platform Account
+000020a0: 2e0a 0a0a 322e 2041 6e20 4170 706c 6963  ....2. An Applic
+000020b0: 6174 696f 6e20 4b65 7920 2620 5365 6372  ation Key & Secr
+000020c0: 6574 3a20 696e 2074 6865 202a 2a41 6363  et: in the **Acc
+000020d0: 6f75 6e74 732a 2a20 7365 6374 696f 6e20  ounts** section 
+000020e0: 756e 6465 7220 7468 6520 2a2a 4170 706c  under the **Appl
+000020f0: 6963 6174 696f 6e73 2a2a 2074 6162 2069  ications** tab i
+00002100: 6e20 7468 6520 5b59 656c 6c6f 7744 6f67  n the [YellowDog
+00002110: 2050 6f72 7461 6c5d 2868 7474 7073 3a2f   Portal](https:/
+00002120: 2f70 6f72 7461 6c2e 7965 6c6c 6f77 646f  /portal.yellowdo
+00002130: 672e 636f 2f23 2f61 6363 6f75 6e74 2f61  g.co/#/account/a
+00002140: 7070 6c69 6361 7469 6f6e 7329 2c20 7573  pplications), us
+00002150: 6520 7468 6520 2a2a 4164 6420 4170 706c  e the **Add Appl
+00002160: 6963 6174 696f 6e2a 2a20 6275 7474 6f6e  ication** button
+00002170: 2074 6f20 6372 6561 7465 2061 206e 6577   to create a new
+00002180: 2041 7070 6c69 6361 7469 6f6e 2c20 616e   Application, an
+00002190: 6420 6d61 6b65 2061 206e 6f74 6520 6f66  d make a note of
+000021a0: 2069 7473 202a 2a4b 6579 2a2a 2061 6e64   its **Key** and
+000021b0: 202a 2a53 6563 7265 742a 2a20 2874 6865   **Secret** (the
+000021c0: 7365 2077 696c 6c20 6f6e 6c79 2062 6520  se will only be 
+000021d0: 6469 7370 6c61 7965 6420 6f6e 6365 292e  displayed once).
+000021e0: 0a0a 0a54 6f20 6372 6561 7465 202a 2a50  ...To create **P
+000021f0: 726f 7669 7369 6f6e 6564 2057 6f72 6b65  rovisioned Worke
+00002200: 7220 506f 6f6c 732a 2a2c 2079 6f75 276c  r Pools**, you'l
+00002210: 6c20 6e65 6564 3a0a 0a33 2e20 4120 2a2a  l need:..3. A **
+00002220: 4b65 7972 696e 672a 2a20 6372 6561 7465  Keyring** create
+00002230: 6420 7669 6120 7468 6520 5965 6c6c 6f77  d via the Yellow
+00002240: 446f 6720 506f 7274 616c 2c20 7769 7468  Dog Portal, with
+00002250: 2061 6363 6573 7320 746f 2043 6c6f 7564   access to Cloud
+00002260: 2050 726f 7669 6465 7220 6372 6564 656e   Provider creden
+00002270: 7469 616c 7320 6173 2072 6571 7569 7265  tials as require
+00002280: 642e 2054 6865 2041 7070 6c69 6361 7469  d. The Applicati
+00002290: 6f6e 206d 7573 7420 6265 2067 7261 6e74  on must be grant
+000022a0: 6564 2061 6363 6573 7320 746f 2074 6865  ed access to the
+000022b0: 204b 6579 7269 6e67 2e0a 0a0a 342e 204f   Keyring....4. O
+000022c0: 6e65 206f 7220 6d6f 7265 202a 2a43 6f6d  ne or more **Com
+000022d0: 7075 7465 2053 6f75 7263 6573 2a2a 2064  pute Sources** d
+000022e0: 6566 696e 6564 2c20 616e 6420 6120 2a2a  efined, and a **
+000022f0: 436f 6d70 7574 6520 5265 7175 6972 656d  Compute Requirem
+00002300: 656e 7420 5465 6d70 6c61 7465 2a2a 2063  ent Template** c
+00002310: 7265 6174 6564 2e20 5468 6520 696d 6167  reated. The imag
+00002320: 6573 2075 7365 6420 6279 2069 6e73 7461  es used by insta
+00002330: 6e63 6573 206d 7573 7420 696e 636c 7564  nces must includ
+00002340: 6520 7468 6520 5965 6c6c 6f77 446f 6720  e the YellowDog 
+00002350: 6167 656e 742c 2063 6f6e 6669 6775 7265  agent, configure
+00002360: 6420 7769 7468 2074 6865 2054 6173 6b20  d with the Task 
+00002370: 5479 7065 2873 2920 746f 206d 6174 6368  Type(s) to match
+00002380: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+00002390: 656d 656e 7473 2074 6f20 6265 2073 7562  ements to be sub
+000023a0: 6d69 7474 6564 2e0a 0a54 6f20 7365 7420  mitted...To set 
+000023b0: 7570 202a 2a43 6f6e 6669 6775 7265 6420  up **Configured 
+000023c0: 576f 726b 6572 2050 6f6f 6c73 2a2a 2c20  Worker Pools**, 
+000023d0: 796f 7527 6c6c 206e 6565 643a 0a0a 352e  you'll need:..5.
+000023e0: 2041 2043 6f6e 6669 6775 7265 6420 576f   A Configured Wo
+000023f0: 726b 6572 2050 6f6f 6c20 546f 6b65 6e3a  rker Pool Token:
+00002400: 2066 726f 6d20 7468 6520 2a2a 576f 726b   from the **Work
+00002410: 6572 732a 2a20 7461 6220 696e 2074 6865  ers** tab in the
+00002420: 205b 5965 6c6c 6f77 446f 6720 506f 7274   [YellowDog Port
+00002430: 616c 5d28 6874 7470 733a 2f2f 706f 7274  al](https://port
+00002440: 616c 2e79 656c 6c6f 7764 6f67 2e63 6f2f  al.yellowdog.co/
+00002450: 232f 776f 726b 6572 7329 2c20 7573 6520  #/workers), use 
+00002460: 7468 6520 2a2a 2b41 6464 2043 6f6e 6669  the **+Add Confi
+00002470: 6775 7265 6420 576f 726b 6572 2050 6f6f  gured Worker Poo
+00002480: 6c2a 2a20 6275 7474 6f6e 2074 6f20 6372  l** button to cr
+00002490: 6561 7465 2061 206e 6577 2057 6f72 6b65  eate a new Worke
+000024a0: 7220 506f 6f6c 2061 6e64 2067 656e 6572  r Pool and gener
+000024b0: 6174 6520 6120 746f 6b65 6e2e 0a0a 0a36  ate a token....6
+000024c0: 2e20 4f62 7461 696e 2074 6865 2059 656c  . Obtain the Yel
+000024d0: 6c6f 7744 6f67 2041 6765 6e74 2061 6e64  lowDog Agent and
+000024e0: 2069 6e73 7461 6c6c 2f63 6f6e 6669 6775   install/configu
+000024f0: 7265 2069 7420 6f6e 2079 6f75 7220 6f6e  re it on your on
+00002500: 2d70 7265 6d69 7365 2073 7973 7465 6d73  -premise systems
+00002510: 2075 7369 6e67 2074 6865 2054 6f6b 656e   using the Token
+00002520: 2061 626f 7665 2e0a 0a23 2053 6372 6970   above...# Scrip
+00002530: 7420 496e 7374 616c 6c61 7469 6f6e 2077  t Installation w
+00002540: 6974 6820 5069 700a 0a50 7974 686f 6e20  ith Pip..Python 
+00002550: 7665 7273 696f 6e20 332e 3720 6f72 206c  version 3.7 or l
+00002560: 6174 6572 2069 7320 7265 7175 6972 6564  ater is required
+00002570: 2e20 4974 2773 2072 6563 6f6d 6d65 6e64  . It's recommend
+00002580: 6564 2074 6861 7420 696e 7374 616c 6c61  ed that installa
+00002590: 7469 6f6e 2069 7320 7065 7266 6f72 6d65  tion is performe
+000025a0: 6420 696e 2061 2050 7974 686f 6e20 7669  d in a Python vi
+000025b0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+000025c0: 7420 286f 7220 7369 6d69 6c61 7229 2074  t (or similar) t
+000025d0: 6f20 6973 6f6c 6174 6520 7468 6520 696e  o isolate the in
+000025e0: 7374 616c 6c61 7469 6f6e 2066 726f 6d20  stallation from 
+000025f0: 6f74 6865 7220 5079 7468 6f6e 2065 6e76  other Python env
+00002600: 6972 6f6e 6d65 6e74 7320 6f6e 2079 6f75  ironments on you
+00002610: 7220 7379 7374 656d 2e0a 0a49 6e73 7461  r system...Insta
+00002620: 6c6c 6174 696f 6e20 616e 6420 7375 6273  llation and subs
+00002630: 6571 7565 6e74 2075 7064 6174 6520 6172  equent update ar
+00002640: 6520 7669 6120 6070 6970 6020 616e 6420  e via `pip` and 
+00002650: 5079 5049 2075 7369 6e67 3a20 0a0a 6060  PyPI using: ..``
+00002660: 6073 6865 6c6c 0a70 6970 2069 6e73 7461  `shell.pip insta
+00002670: 6c6c 202d 5520 7965 6c6c 6f77 646f 672d  ll -U yellowdog-
+00002680: 7079 7468 6f6e 2d65 7861 6d70 6c65 730a  python-examples.
+00002690: 6060 600a 0a49 6620 796f 7527 7265 2069  ```..If you're i
+000026a0: 6e74 6572 6573 7465 6420 696e 2069 6e63  nterested in inc
+000026b0: 6c75 6469 6e67 202a 2a4a 736f 6e6e 6574  luding **Jsonnet
+000026c0: 2a2a 2073 7570 706f 7274 2c20 706c 6561  ** support, plea
+000026d0: 7365 2073 6565 2074 6865 205b 4a73 6f6e  se see the [Json
+000026e0: 6e65 7420 5375 7070 6f72 745d 2823 6a73  net Support](#js
+000026f0: 6f6e 6e65 742d 7375 7070 6f72 7429 2073  onnet-support) s
+00002700: 6563 7469 6f6e 2062 656c 6f77 2e0a 0a23  ection below...#
+00002710: 2053 6372 6970 7420 496e 7374 616c 6c61   Script Installa
+00002720: 7469 6f6e 2077 6974 6820 5069 7078 0a0a  tion with Pipx..
+00002730: 5468 6520 636f 6d6d 616e 6473 2063 616e  The commands can
+00002740: 2061 6c73 6f20 6265 2069 6e73 7461 6c6c   also be install
+00002750: 6564 2075 7369 6e67 202a 2a5b 7069 7078  ed using **[pipx
+00002760: 5d28 6874 7470 733a 2f2f 7079 7061 2e67  ](https://pypa.g
+00002770: 6974 6875 622e 696f 2f70 6970 782f 292a  ithub.io/pipx/)*
+00002780: 2a2e 0a0a 5468 6973 206d 6574 686f 6420  *...This method 
+00002790: 7265 7175 6972 6573 2050 7974 686f 6e20  requires Python 
+000027a0: 332e 372b 2061 6e64 2070 6970 7820 746f  3.7+ and pipx to
+000027b0: 2062 6520 696e 7374 616c 6c65 642e 2054   be installed. T
+000027c0: 6f20 696e 7374 616c 6c3a 0a60 6060 7368  o install:.```sh
+000027d0: 656c 6c0a 7069 7078 2069 6e73 7461 6c6c  ell.pipx install
+000027e0: 2079 656c 6c6f 7764 6f67 2d70 7974 686f   yellowdog-pytho
+000027f0: 6e2d 6578 616d 706c 6573 0a60 6060 0a0a  n-examples.```..
+00002800: 546f 2075 7064 6174 653a 0a60 6060 7368  To update:.```sh
+00002810: 656c 6c0a 7069 7078 2075 7067 7261 6465  ell.pipx upgrade
+00002820: 2079 656c 6c6f 7764 6f67 2d70 7974 686f   yellowdog-pytho
+00002830: 6e2d 6578 616d 706c 6573 0a60 6060 0a0a  n-examples.```..
+00002840: 2320 5573 6167 650a 0a42 6f74 6820 6f66  # Usage..Both of
+00002850: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
+00002860: 6e20 6d65 7468 6f64 7320 6162 6f76 6520  n methods above 
+00002870: 7769 6c6c 2069 6e73 7461 6c6c 2061 206e  will install a n
+00002880: 756d 6265 7220 6f66 202a 2a60 7964 2d60  umber of **`yd-`
+00002890: 2a2a 2063 6f6d 6d61 6e64 7320 6f6e 2079  ** commands on y
+000028a0: 6f75 7220 5041 5448 2e0a 0a43 6f6d 6d61  our PATH...Comma
+000028b0: 6e64 7320 6172 6520 7275 6e20 6672 6f6d  nds are run from
+000028c0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+000028d0: 652e 2049 6e76 6f6b 696e 6720 7468 6520  e. Invoking the 
+000028e0: 636f 6d6d 616e 6420 7769 7468 2074 6865  command with the
+000028f0: 2060 2d2d 6865 6c70 6020 6f72 2060 2d68   `--help` or `-h
+00002900: 6020 6f70 7469 6f6e 2077 696c 6c20 6469  ` option will di
+00002910: 7370 6c61 7920 7468 6520 636f 6d6d 616e  splay the comman
+00002920: 6420 6c69 6e65 206f 7074 696f 6e73 2061  d line options a
+00002930: 7070 6c69 6361 626c 6520 746f 2061 2067  pplicable to a g
+00002940: 6976 656e 2063 6f6d 6d61 6e64 2c20 652e  iven command, e.
+00002950: 672e 3a0a 0a60 6060 7465 7874 0a20 2520  g.:..```text. % 
+00002960: 7964 2d63 616e 6365 6c20 2d2d 6865 6c70  yd-cancel --help
+00002970: 0a75 7361 6765 3a20 7964 2d63 616e 6365  .usage: yd-cance
+00002980: 6c20 5b2d 685d 205b 2d2d 646f 6373 5d20  l [-h] [--docs] 
+00002990: 5b2d 2d63 6f6e 6669 6720 3c63 6f6e 6669  [--config <confi
+000029a0: 675f 6669 6c65 2e74 6f6d 6c3e 5d20 5b2d  g_file.toml>] [-
+000029b0: 2d6b 6579 203c 6170 702d 6b65 793e 5d0a  -key <app-key>].
 000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 205b 2d2d 7661 7269 6162 6c65 203c 7661   [--variable <va
-000029e0: 7231 3d76 313e 5d20 5b2d 2d71 7569 6574  r1=v1>] [--quiet
-000029f0: 5d20 5b2d 2d64 6562 7567 5d20 5b2d 2d70  ] [--debug] [--p
-00002a00: 6163 5d20 5b2d 2d61 626f 7274 5d20 5b2d  ac] [--abort] [-
-00002a10: 2d66 6f6c 6c6f 775d 0a20 2020 2020 2020  -follow].       
-00002a20: 2020 2020 2020 2020 2020 5b2d 2d69 6e74            [--int
-00002a30: 6572 6163 7469 7665 5d20 5b2d 2d79 6573  eractive] [--yes
-00002a40: 5d0a 0a59 656c 6c6f 7744 6f67 2065 7861  ]..YellowDog exa
-00002a50: 6d70 6c65 2075 7469 6c69 7479 2066 6f72  mple utility for
-00002a60: 2063 616e 6365 6c6c 696e 6720 576f 726b   cancelling Work
-00002a70: 2052 6571 7569 7265 6d65 6e74 730a 0a6f   Requirements..o
-00002a80: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
-00002a90: 733a 0a20 202d 682c 202d 2d68 656c 7020  s:.  -h, --help 
-00002aa0: 2020 2020 2020 2020 2020 2073 686f 7720             show 
-00002ab0: 7468 6973 2068 656c 7020 6d65 7373 6167  this help messag
-00002ac0: 6520 616e 6420 6578 6974 0a20 202d 2d64  e and exit.  --d
-00002ad0: 6f63 7320 2020 2020 2020 2020 2020 2020  ocs             
-00002ae0: 2020 2070 726f 7669 6465 2061 206c 696e     provide a lin
-00002af0: 6b20 746f 2074 6865 2064 6f63 756d 656e  k to the documen
-00002b00: 7461 7469 6f6e 2066 6f72 2074 6869 7320  tation for this 
-00002b10: 7665 7273 696f 6e0a 2020 2d2d 636f 6e66  version.  --conf
-00002b20: 6967 203c 636f 6e66 6967 5f66 696c 652e  ig <config_file.
-00002b30: 746f 6d6c 3e2c 202d 6320 3c63 6f6e 6669  toml>, -c <confi
-00002b40: 675f 6669 6c65 2e74 6f6d 6c3e 0a20 2020  g_file.toml>.   
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-00002b70: 6f6e 2066 696c 6520 696e 2054 4f4d 4c20  on file in TOML 
-00002b80: 666f 726d 6174 3b20 6465 6661 756c 7420  format; default 
-00002b90: 6973 2027 636f 6e66 6967 2e74 6f6d 6c27  is 'config.toml'
-00002ba0: 2069 6e20 7468 6520 6375 7272 656e 740a   in the current.
+000029d0: 205b 2d2d 7365 6372 6574 203c 6170 702d   [--secret <app-
+000029e0: 7365 6372 6574 3e5d 205b 2d2d 6e61 6d65  secret>] [--name
+000029f0: 7370 6163 6520 3c6e 616d 6573 7061 6365  space <namespace
+00002a00: 3e5d 205b 2d2d 7461 6720 3c74 6167 3e5d  >] [--tag <tag>]
+00002a10: 205b 2d2d 7572 6c20 3c75 726c 3e5d 0a20   [--url <url>]. 
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 5b2d 2d76 6172 6961 626c 6520 3c76 6172  [--variable <var
+00002a40: 313d 7631 3e5d 205b 2d2d 7175 6965 745d  1=v1>] [--quiet]
+00002a50: 205b 2d2d 6465 6275 675d 205b 2d2d 7061   [--debug] [--pa
+00002a60: 635d 205b 2d2d 6162 6f72 745d 205b 2d2d  c] [--abort] [--
+00002a70: 666f 6c6c 6f77 5d0a 2020 2020 2020 2020  follow].        
+00002a80: 2020 2020 2020 2020 205b 2d2d 696e 7465           [--inte
+00002a90: 7261 6374 6976 655d 205b 2d2d 7965 735d  ractive] [--yes]
+00002aa0: 0a0a 5965 6c6c 6f77 446f 6720 6578 616d  ..YellowDog exam
+00002ab0: 706c 6520 7574 696c 6974 7920 666f 7220  ple utility for 
+00002ac0: 6361 6e63 656c 6c69 6e67 2057 6f72 6b20  cancelling Work 
+00002ad0: 5265 7175 6972 656d 656e 7473 0a0a 6f70  Requirements..op
+00002ae0: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+00002af0: 3a0a 2020 2d68 2c20 2d2d 6865 6c70 2020  :.  -h, --help  
+00002b00: 2020 2020 2020 2020 2020 7368 6f77 2074            show t
+00002b10: 6869 7320 6865 6c70 206d 6573 7361 6765  his help message
+00002b20: 2061 6e64 2065 7869 740a 2020 2d2d 646f   and exit.  --do
+00002b30: 6373 2020 2020 2020 2020 2020 2020 2020  cs              
+00002b40: 2020 7072 6f76 6964 6520 6120 6c69 6e6b    provide a link
+00002b50: 2074 6f20 7468 6520 646f 6375 6d65 6e74   to the document
+00002b60: 6174 696f 6e20 666f 7220 7468 6973 2076  ation for this v
+00002b70: 6572 7369 6f6e 0a20 202d 2d63 6f6e 6669  ersion.  --confi
+00002b80: 6720 3c63 6f6e 6669 675f 6669 6c65 2e74  g <config_file.t
+00002b90: 6f6d 6c3e 2c20 2d63 203c 636f 6e66 6967  oml>, -c <config
+00002ba0: 5f66 696c 652e 746f 6d6c 3e0a 2020 2020  _file.toml>.    
 00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2020 2020 2020 6469 7265 6374 6f72          director
-00002bd0: 790a 2020 2d2d 6b65 7920 3c61 7070 2d6b  y.  --key <app-k
-00002be0: 6579 3e2c 202d 6b20 3c61 7070 2d6b 6579  ey>, -k <app-key
-00002bf0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002c00: 2020 2020 2020 2020 2020 7468 6520 5965            the Ye
-00002c10: 6c6c 6f77 446f 6720 4170 706c 6963 6174  llowDog Applicat
-00002c20: 696f 6e20 6b65 790a 2020 2d2d 7365 6372  ion key.  --secr
-00002c30: 6574 203c 6170 702d 7365 6372 6574 3e2c  et <app-secret>,
-00002c40: 202d 7320 3c61 7070 2d73 6563 7265 743e   -s <app-secret>
+00002bc0: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
+00002bd0: 6e20 6669 6c65 2069 6e20 544f 4d4c 2066  n file in TOML f
+00002be0: 6f72 6d61 743b 2064 6566 6175 6c74 2069  ormat; default i
+00002bf0: 7320 2763 6f6e 6669 672e 746f 6d6c 2720  s 'config.toml' 
+00002c00: 696e 2074 6865 2063 7572 7265 6e74 0a20  in the current. 
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 2020 2020 2064 6972 6563 746f 7279         directory
+00002c30: 0a20 202d 2d6b 6579 203c 6170 702d 6b65  .  --key <app-ke
+00002c40: 793e 2c20 2d6b 203c 6170 702d 6b65 793e  y>, -k <app-key>
 00002c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002c60: 2020 2020 2020 2020 2074 6865 2059 656c           the Yel
 00002c70: 6c6f 7744 6f67 2041 7070 6c69 6361 7469  lowDog Applicati
-00002c80: 6f6e 2073 6563 7265 740a 2020 2d2d 6e61  on secret.  --na
-00002c90: 6d65 7370 6163 6520 3c6e 616d 6573 7061  mespace <namespa
-00002ca0: 6365 3e2c 202d 6e20 3c6e 616d 6573 7061  ce>, -n <namespa
-00002cb0: 6365 3e0a 2020 2020 2020 2020 2020 2020  ce>.            
-00002cc0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00002cd0: 6e61 6d65 7370 6163 6520 746f 2075 7365  namespace to use
-00002ce0: 2077 6865 6e20 6372 6561 7469 6e67 2061   when creating a
-00002cf0: 6e64 2069 6465 6e74 6966 7969 6e67 2065  nd identifying e
-00002d00: 6e74 6974 6965 730a 2020 2d2d 7461 6720  ntities.  --tag 
-00002d10: 3c74 6167 3e2c 202d 7420 3c74 6167 3e0a  <tag>, -t <tag>.
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2020 7468 6520 7461 6720          the tag 
-00002d40: 746f 2075 7365 2066 6f72 2074 6167 6769  to use for taggi
-00002d50: 6e67 2061 6e64 206e 616d 696e 6720 656e  ng and naming en
-00002d60: 7469 7469 6573 0a20 202d 2d75 726c 203c  tities.  --url <
-00002d70: 7572 6c3e 2c20 2d75 203c 7572 6c3e 0a20  url>, -u <url>. 
+00002c80: 6f6e 206b 6579 0a20 202d 2d73 6563 7265  on key.  --secre
+00002c90: 7420 3c61 7070 2d73 6563 7265 743e 2c20  t <app-secret>, 
+00002ca0: 2d73 203c 6170 702d 7365 6372 6574 3e0a  -s <app-secret>.
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 7468 6520 5965 6c6c          the Yell
+00002cd0: 6f77 446f 6720 4170 706c 6963 6174 696f  owDog Applicatio
+00002ce0: 6e20 7365 6372 6574 0a20 202d 2d6e 616d  n secret.  --nam
+00002cf0: 6573 7061 6365 203c 6e61 6d65 7370 6163  espace <namespac
+00002d00: 653e 2c20 2d6e 203c 6e61 6d65 7370 6163  e>, -n <namespac
+00002d10: 653e 0a20 2020 2020 2020 2020 2020 2020  e>.             
+00002d20: 2020 2020 2020 2020 2020 2074 6865 206e             the n
+00002d30: 616d 6573 7061 6365 2074 6f20 7573 6520  amespace to use 
+00002d40: 7768 656e 2063 7265 6174 696e 6720 616e  when creating an
+00002d50: 6420 6964 656e 7469 6679 696e 6720 656e  d identifying en
+00002d60: 7469 7469 6573 0a20 202d 2d74 6167 203c  tities.  --tag <
+00002d70: 7461 673e 2c20 2d74 203c 7461 673e 0a20  tag>, -t <tag>. 
 00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2020 2020 2020 2074 6865 2055 524c 206f         the URL o
-00002da0: 6620 7468 6520 5965 6c6c 6f77 446f 6720  f the YellowDog 
-00002db0: 506c 6174 666f 726d 2041 5049 0a20 202d  Platform API.  -
-00002dc0: 2d76 6172 6961 626c 6520 3c76 6172 313d  -variable <var1=
-00002dd0: 7631 3e2c 202d 7620 3c76 6172 313d 7631  v1>, -v <var1=v1
-00002de0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002df0: 2020 2020 2020 2020 2020 7573 6572 2d64            user-d
-00002e00: 6566 696e 6564 2076 6172 6961 626c 6520  efined variable 
-00002e10: 7375 6273 7469 7475 7469 6f6e 733b 2063  substitutions; c
-00002e20: 616e 2062 6520 7375 7070 6c69 6564 206d  an be supplied m
-00002e30: 756c 7469 706c 6520 7469 6d65 730a 2020  ultiple times.  
-00002e40: 2d2d 7175 6965 742c 202d 7120 2020 2020  --quiet, -q     
-00002e50: 2020 2020 2020 7375 7070 7265 7373 2028        suppress (
-00002e60: 6e6f 6e2d 6572 726f 722c 206e 6f6e 2d69  non-error, non-i
-00002e70: 6e74 6572 6163 7469 7665 2920 7374 6174  nteractive) stat
-00002e80: 7573 2061 6e64 2070 726f 6772 6573 7320  us and progress 
-00002e90: 6d65 7373 6167 6573 0a20 202d 2d64 6562  messages.  --deb
-00002ea0: 7567 2020 2020 2020 2020 2020 2020 2020  ug              
-00002eb0: 2070 7269 6e74 2061 2073 7461 636b 2074   print a stack t
-00002ec0: 7261 6365 2028 6574 632e 2920 6f6e 2065  race (etc.) on e
-00002ed0: 7272 6f72 0a20 202d 2d70 6163 2020 2020  rror.  --pac    
-00002ee0: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
-00002ef0: 626c 6520 5041 4320 2870 726f 7879 2061  ble PAC (proxy a
-00002f00: 7574 6f2d 636f 6e66 6967 7572 6174 696f  uto-configuratio
-00002f10: 6e29 2073 7570 706f 7274 0a20 202d 2d61  n) support.  --a
-00002f20: 626f 7274 2c20 2d61 2020 2020 2020 2020  bort, -a        
-00002f30: 2020 2061 626f 7274 2061 6c6c 2072 756e     abort all run
-00002f40: 6e69 6e67 2074 6173 6b73 2077 6974 6820  ning tasks with 
-00002f50: 696d 6d65 6469 6174 6520 6566 6665 6374  immediate effect
-00002f60: 0a20 202d 2d66 6f6c 6c6f 772c 202d 6620  .  --follow, -f 
-00002f70: 2020 2020 2020 2020 2077 6865 6e20 7573           when us
-00002f80: 696e 6720 2d2d 6162 6f72 742c 2070 6f6c  ing --abort, pol
-00002f90: 6c20 756e 7469 6c20 616c 6c20 5461 736b  l until all Task
-00002fa0: 7320 6861 7665 2062 6565 6e20 6162 6f72  s have been abor
-00002fb0: 7465 640a 2020 2d2d 696e 7465 7261 6374  ted.  --interact
-00002fc0: 6976 652c 202d 6920 2020 2020 6c69 7374  ive, -i     list
-00002fd0: 2c20 616e 6420 696e 7465 7261 6374 6976  , and interactiv
-00002fe0: 656c 7920 7365 6c65 6374 2c20 6974 656d  ely select, item
-00002ff0: 7320 746f 2061 6374 206f 6e0a 2020 2d2d  s to act on.  --
-00003000: 7965 732c 202d 7920 2020 2020 2020 2020  yes, -y         
-00003010: 2020 2020 7065 7266 6f72 6d20 6465 7374      perform dest
-00003020: 7275 6374 6976 6520 6163 7469 6f6e 7320  ructive actions 
-00003030: 7769 7468 6f75 7420 7265 7175 6972 696e  without requirin
-00003040: 6720 7573 6572 2063 6f6e 6669 726d 6174  g user confirmat
-00003050: 696f 6e0a 6060 600a 0a23 2043 6f6e 6669  ion.```..# Confi
-00003060: 6775 7261 7469 6f6e 0a0a 4279 2064 6566  guration..By def
-00003070: 6175 6c74 2c20 7468 6520 6f70 6572 6174  ault, the operat
-00003080: 696f 6e20 6f66 2061 6c6c 2063 6f6d 6d61  ion of all comma
-00003090: 6e64 7320 6973 2063 6f6e 6669 6775 7265  nds is configure
-000030a0: 6420 7573 696e 6720 6120 544f 4d4c 2063  d using a TOML c
-000030b0: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-000030c0: 652e 0a0a 5468 6520 636f 6e66 6967 7572  e...The configur
-000030d0: 6174 696f 6e20 6669 6c65 2068 6173 2074  ation file has t
-000030e0: 6872 6565 2070 6f73 7369 626c 6520 7365  hree possible se
-000030f0: 6374 696f 6e73 3a0a 0a31 2e20 4120 6063  ctions:..1. A `c
-00003100: 6f6d 6d6f 6e60 2073 6563 7469 6f6e 2074  ommon` section t
-00003110: 6861 7420 636f 6e74 6169 6e73 2072 6571  hat contains req
-00003120: 7569 7265 6420 7365 6375 7269 7479 2070  uired security p
-00003130: 726f 7065 7274 6965 7320 666f 7220 696e  roperties for in
-00003140: 7465 7261 6374 696e 6720 7769 7468 2074  teracting with t
-00003150: 6865 2059 656c 6c6f 7744 6f67 2070 6c61  he YellowDog pla
-00003160: 7466 6f72 6d2c 2073 6574 7320 7468 6520  tform, sets the 
-00003170: 4e61 6d65 7370 6163 6520 696e 2077 6869  Namespace in whi
-00003180: 6368 2059 656c 6c6f 7744 6f67 2061 7373  ch YellowDog ass
-00003190: 6574 7320 616e 6420 6f62 6a65 6374 7320  ets and objects 
-000031a0: 6172 6520 6372 6561 7465 642c 2061 6e64  are created, and
-000031b0: 2061 2054 6167 2074 6861 7420 6973 2075   a Tag that is u
-000031c0: 7365 6420 666f 7220 7461 6767 696e 6720  sed for tagging 
-000031d0: 616e 6420 6e61 6d69 6e67 2061 7373 6574  and naming asset
-000031e0: 7320 616e 6420 6f62 6a65 6374 732e 0a32  s and objects..2
-000031f0: 2e20 4120 6077 6f72 6b52 6571 7569 7265  . A `workRequire
-00003200: 6d65 6e74 6020 7365 6374 696f 6e20 7468  ment` section th
-00003210: 6174 2064 6566 696e 6573 2074 6865 2070  at defines the p
-00003220: 726f 7065 7274 6965 7320 6f66 2057 6f72  roperties of Wor
-00003230: 6b20 5265 7175 6972 656d 656e 7473 2074  k Requirements t
-00003240: 6f20 6265 2073 7562 6d69 7474 6564 2074  o be submitted t
-00003250: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
-00003260: 706c 6174 666f 726d 2e0a 332e 2041 2060  platform..3. A `
-00003270: 776f 726b 6572 506f 6f6c 6020 7365 6374  workerPool` sect
-00003280: 696f 6e20 7468 6174 2064 6566 696e 6573  ion that defines
-00003290: 2074 6865 2070 726f 7065 7274 6965 7320   the properties 
-000032a0: 6f66 2050 726f 7669 736f 6e65 6420 576f  of Provisoned Wo
-000032b0: 726b 6572 2050 6f6f 6c73 2074 6f20 6265  rker Pools to be
-000032c0: 2063 7265 6174 6564 2075 7369 6e67 2074   created using t
-000032d0: 6865 2059 656c 6c6f 7744 6f67 2070 6c61  he YellowDog pla
-000032e0: 7466 6f72 6d2e 200a 0a54 6865 7265 2069  tform. ..There i
-000032f0: 7320 6120 646f 6375 6d65 6e74 6564 2074  s a documented t
-00003300: 656d 706c 6174 6520 544f 4d4c 2066 696c  emplate TOML fil
-00003310: 6520 7072 6f76 6964 6564 2069 6e20 5b63  e provided in [c
-00003320: 6f6e 6669 672e 746f 6d6c 2e74 656d 706c  onfig.toml.templ
-00003330: 6174 655d 2863 6f6e 6669 672e 746f 6d6c  ate](config.toml
-00003340: 2e74 656d 706c 6174 6529 2c20 636f 6e74  .template), cont
-00003350: 6169 6e69 6e67 2074 6865 206d 6169 6e20  aining the main 
-00003360: 7072 6f70 6572 7469 6573 2074 6861 7420  properties that 
-00003370: 6361 6e20 6265 2063 6f6e 6669 6775 7265  can be configure
-00003380: 642e 0a0a 5468 6520 636f 6e66 6967 7572  d...The configur
-00003390: 6174 696f 6e20 6669 6c65 6e61 6d65 2063  ation filename c
-000033a0: 616e 2062 6520 7375 7070 6c69 6564 2069  an be supplied i
-000033b0: 6e20 7468 7265 6520 6469 6666 6572 656e  n three differen
-000033c0: 7420 7761 7973 3a0a 0a31 2e20 4f6e 2074  t ways:..1. On t
-000033d0: 6865 2063 6f6d 6d61 6e64 206c 696e 652c  he command line,
-000033e0: 2075 7369 6e67 2074 6865 2060 2d2d 636f   using the `--co
-000033f0: 6e66 6967 6020 6f72 2060 2d63 6020 6f70  nfig` or `-c` op
-00003400: 7469 6f6e 732c 2065 2e67 2e3a 3c62 723e  tions, e.g.:<br>
-00003410: 6079 642d 7375 626d 6974 202d 6320 6a6f  `yd-submit -c jo
-00003420: 6273 2f63 6f6e 6669 675f 312e 746f 6d6c  bs/config_1.toml
-00003430: 600a 322e 2055 7369 6e67 2074 6865 2060  `.2. Using the `
-00003440: 5944 5f43 4f4e 4660 2065 6e76 6972 6f6e  YD_CONF` environ
-00003450: 6d65 6e74 2076 6172 6961 626c 652c 2065  ment variable, e
-00003460: 2e67 2e3a 203c 6272 3e60 6578 706f 7274  .g.: <br>`export
-00003470: 2059 445f 434f 4e46 3d22 6a6f 6273 2f63   YD_CONF="jobs/c
-00003480: 6f6e 6669 675f 312e 746f 6d6c 2260 0a33  onfig_1.toml"`.3
-00003490: 2e20 4966 206e 6569 7468 6572 206f 6620  . If neither of 
-000034a0: 7468 6520 6162 6f76 6520 6973 2073 7570  the above is sup
-000034b0: 706c 6965 642c 2074 6865 2063 6f6d 6d61  plied, the comma
-000034c0: 6e64 7320 6c6f 6f6b 2066 6f72 2061 2060  nds look for a `
-000034d0: 636f 6e66 6967 2e74 6f6d 6c60 2066 696c  config.toml` fil
-000034e0: 6520 696e 2074 6865 2063 7572 7265 6e74  e in the current
-000034f0: 2064 6972 6563 746f 7279 0a0a 5468 6520   directory..The 
-00003500: 6f70 7469 6f6e 7320 6162 6f76 6520 6172  options above ar
-00003510: 6520 7368 6f77 6e20 696e 206f 7264 6572  e shown in order
-00003520: 206f 6620 7072 6563 6564 656e 6365 2c20   of precedence, 
-00003530: 692e 652e 2c20 6120 6669 6c65 6e61 6d65  i.e., a filename
-00003540: 2073 7570 706c 6965 6420 6f6e 2074 6865   supplied on the
-00003550: 2063 6f6d 6d61 6e64 206c 696e 6520 7375   command line su
-00003560: 7065 7273 6564 6573 206f 6e65 2073 6574  persedes one set
-00003570: 2069 6e20 6059 445f 434f 4e46 602c 2077   in `YD_CONF`, w
-00003580: 6869 6368 2073 7570 6572 7365 6465 7320  hich supersedes 
-00003590: 7468 6520 6465 6661 756c 742e 0a0a 2320  the default...# 
-000035a0: 4e61 6d69 6e67 2052 756c 6573 0a0a 416c  Naming Rules..Al
-000035b0: 6c20 656e 7469 7479 206e 616d 6573 2075  l entity names u
-000035c0: 7365 6420 7769 7468 696e 2074 6865 2059  sed within the Y
-000035d0: 656c 6c6f 7744 6f67 2050 6c61 7466 6f72  ellowDog Platfor
-000035e0: 6d20 6d75 7374 2063 6f6d 706c 7920 7769  m must comply wi
-000035f0: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
-00003600: 2072 6573 7472 6963 7469 6f6e 733a 0a0a   restrictions:..
-00003610: 2d20 4e61 6d65 7320 6361 6e20 6f6e 6c79  - Names can only
-00003620: 2063 6f6e 7461 696e 2074 6865 2066 6f6c   contain the fol
-00003630: 6c6f 7769 6e67 3a20 6c6f 7765 7263 6173  lowing: lowercas
-00003640: 6520 6c65 7474 6572 732c 2064 6967 6974  e letters, digit
-00003650: 732c 2068 7970 6865 6e73 2061 6e64 2075  s, hyphens and u
-00003660: 6e64 6572 7363 6f72 6573 2028 6e6f 7465  nderscores (note
-00003670: 2074 6861 7420 7370 6163 6573 2061 7265   that spaces are
-00003680: 206e 6f74 2070 6572 6d69 7474 6564 290a   not permitted).
-00003690: 2d20 4e61 6d65 7320 6d75 7374 2073 7461  - Names must sta
-000036a0: 7274 2077 6974 6820 6120 6c65 7474 6572  rt with a letter
-000036b0: 0a2d 204e 616d 6573 206d 7573 7420 656e  .- Names must en
-000036c0: 6420 7769 7468 2061 206c 6574 7465 7220  d with a letter 
-000036d0: 6f72 2064 6967 6974 0a2d 204e 616d 6520  or digit.- Name 
-000036e0: 6c65 6e67 7468 206d 7573 7420 6265 203c  length must be <
-000036f0: 3d20 3630 2063 6861 7261 6374 6572 730a  = 60 characters.
-00003700: 0a54 6865 7365 2072 6573 7472 6963 7469  .These restricti
-00003710: 6f6e 7320 6170 706c 7920 746f 2065 6e74  ons apply to ent
-00003720: 6974 6965 7320 696e 636c 7564 696e 6720  ities including 
-00003730: 4e61 6d65 7370 6163 6573 2c20 5461 6773  Namespaces, Tags
-00003740: 2c20 576f 726b 2052 6571 7569 7265 6d65  , Work Requireme
-00003750: 6e74 732c 2054 6173 6b20 4772 6f75 7073  nts, Task Groups
-00003760: 2c20 5461 736b 732c 2057 6f72 6b65 7220  , Tasks, Worker 
-00003770: 506f 6f6c 732c 2061 6e64 2043 6f6d 7075  Pools, and Compu
-00003780: 7465 2052 6571 7569 7265 6d65 6e74 732c  te Requirements,
-00003790: 2061 6e64 2061 6c73 6f20 6170 706c 7920   and also apply 
-000037a0: 746f 2065 6e74 6974 6965 7320 7468 6174  to entities that
-000037b0: 2061 7265 2063 7572 7265 6e74 6c79 2075   are currently u
-000037c0: 7365 6420 696e 6469 7265 6374 6c79 2062  sed indirectly b
-000037d0: 7920 7468 6573 6520 7363 7269 7074 732c  y these scripts,
-000037e0: 2069 6e63 6c75 6469 6e67 2055 7365 726e   including Usern
-000037f0: 616d 6573 2c20 4372 6564 656e 7469 616c  ames, Credential
-00003800: 732c 204b 6579 7269 6e67 732c 2043 6f6d  s, Keyrings, Com
-00003810: 7075 7465 2053 6f75 7263 6573 2061 6e64  pute Sources and
-00003820: 2043 6f6d 7075 7465 2054 656d 706c 6174   Compute Templat
-00003830: 6573 2e0a 0a23 2043 6f6d 6d6f 6e20 5072  es...# Common Pr
-00003840: 6f70 6572 7469 6573 0a0a 5468 6520 605b  operties..The `[
-00003850: 636f 6d6d 6f6e 5d60 2073 6563 7469 6f6e  common]` section
-00003860: 206f 6620 7468 6520 636f 6e66 6967 7572   of the configur
-00003870: 6174 696f 6e20 6669 6c65 2063 616e 2063  ation file can c
-00003880: 6f6e 7461 696e 2074 6865 2066 6f6c 6c6f  ontain the follo
-00003890: 7769 6e67 2070 726f 7065 7274 6965 733a  wing properties:
-000038a0: 0a0a 7c20 5072 6f70 6572 7479 2020 2020  ..| Property    
-000038b0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003900: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
-00003910: 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d  ------|:--------
-00003920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-00003970: 606b 6579 6020 2020 2020 2020 7c20 5468  `key`       | Th
-00003980: 6520 2a2a 6b65 792a 2a20 6f66 2074 6865  e **key** of the
-00003990: 2059 656c 6c6f 7744 6f67 2041 7070 6c69   YellowDog Appli
-000039a0: 6361 7469 6f6e 2075 6e64 6572 2077 6869  cation under whi
-000039b0: 6368 2074 6865 2063 6f6d 6d61 6e64 7320  ch the commands 
-000039c0: 7769 6c6c 2072 756e 2020 2020 2020 2020  will run        
-000039d0: 2020 7c0a 7c20 6073 6563 7265 7460 2020    |.| `secret`  
-000039e0: 2020 7c20 5468 6520 2a2a 7365 6372 6574    | The **secret
-000039f0: 2a2a 206f 6620 7468 6520 5965 6c6c 6f77  ** of the Yellow
-00003a00: 446f 6720 4170 706c 6963 6174 696f 6e20  Dog Application 
-00003a10: 756e 6465 7220 7768 6963 6820 7468 6520  under which the 
-00003a20: 636f 6d6d 616e 6473 2077 696c 6c20 7275  commands will ru
-00003a30: 6e20 2020 2020 2020 7c0a 7c20 606e 616d  n       |.| `nam
-00003a40: 6573 7061 6365 6020 7c20 5468 6520 2a2a  espace` | The **
-00003a50: 6e61 6d65 7370 6163 652a 2a20 746f 2062  namespace** to b
-00003a60: 6520 7573 6564 2066 6f72 2067 726f 7570  e used for group
-00003a70: 696e 6720 7265 736f 7572 6365 7320 2020  ing resources   
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00003aa0: 7c20 6074 6167 6020 2020 2020 2020 7c20  | `tag`       | 
-00003ab0: 5468 6520 2a2a 7461 672a 2a20 746f 2062  The **tag** to b
-00003ac0: 6520 7573 6564 2066 6f72 2074 6167 6769  e used for taggi
-00003ad0: 6e67 2072 6573 6f75 7263 6573 2061 6e64  ng resources and
-00003ae0: 206e 616d 696e 6720 6f62 6a65 6374 7320   naming objects 
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 7c0a 7c20 6075 726c 6020 2020      |.| `url`   
-00003b10: 2020 2020 7c20 5468 6520 2a2a 5552 4c2a      | The **URL*
-00003b20: 2a20 6f66 2074 6865 2059 656c 6c6f 7744  * of the YellowD
-00003b30: 6f67 2050 6c61 7466 6f72 6d20 4150 4920  og Platform API 
-00003b40: 656e 6470 6f69 6e74 2c20 6966 2074 6865  endpoint, if the
-00003b50: 2064 6566 6175 6c74 2069 736e 2774 2074   default isn't t
-00003b60: 6f20 6265 2075 7365 6420 7c0a 7c20 6075  o be used |.| `u
-00003b70: 7365 5041 4360 2020 2020 7c20 5573 6520  sePAC`    | Use 
-00003b80: 5041 4320 2870 726f 7879 2061 7574 6f63  PAC (proxy autoc
-00003b90: 6f6e 6669 6775 7261 7469 6f6e 2920 6966  onfiguration) if
-00003ba0: 2073 6574 2074 6f20 6074 7275 6560 2020   set to `true`  
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 7c0a 7c20 6076 6172 6961 626c 6573 6020  |.| `variables` 
-00003be0: 7c20 4120 7461 626c 6520 636f 6e74 6169  | A table contai
-00003bf0: 6e69 6e67 202a 2a76 6172 6961 626c 6520  ning **variable 
-00003c00: 7375 6273 7469 7475 7469 6f6e 732a 2a20  substitutions** 
-00003c10: 2873 6565 2074 6865 2056 6172 6961 626c  (see the Variabl
-00003c20: 6573 2073 6563 7469 6f6e 2062 656c 6f77  es section below
-00003c30: 2920 2020 2020 7c0a 0a41 6e20 6578 616d  )     |..An exam
-00003c40: 706c 6520 6063 6f6d 6d6f 6e60 2073 6563  ple `common` sec
-00003c50: 7469 6f6e 2069 7320 7368 6f77 6e20 6265  tion is shown be
-00003c60: 6c6f 773a 0a0a 6060 6074 6f6d 6c0a 5b63  low:..```toml.[c
-00003c70: 6f6d 6d6f 6e5d 0a20 2020 206b 6579 203d  ommon].    key =
-00003c80: 2022 6173 6466 6768 6a6b 6c7a 7863 7662   "asdfghjklzxcvb
-00003c90: 2d31 3233 3435 3637 220a 2020 2020 7365  -1234567".    se
-00003ca0: 6372 6574 203d 2022 7177 6572 7479 7569  cret = "qwertyui
-00003cb0: 6f70 6173 6466 6768 6a6b 6c7a 7863 7662  opasdfghjklzxcvb
-00003cc0: 6e6d 3132 3334 3536 3738 3930 7177 6572  nm1234567890qwer
-00003cd0: 7479 7522 0a20 2020 206e 616d 6573 7061  tyu".    namespa
-00003ce0: 6365 203d 2022 7072 6f6a 6563 742d 7822  ce = "project-x"
-00003cf0: 0a20 2020 2074 6167 203d 2022 7465 7374  .    tag = "test
-00003d00: 696e 672d 7b7b 7573 6572 6e61 6d65 7d7d  ing-{{username}}
-00003d10: 220a 6060 600a 0a49 6e64 656e 7461 7469  ".```..Indentati
-00003d20: 6f6e 2069 7320 6f70 7469 6f6e 616c 2069  on is optional i
-00003d30: 6e20 544f 4d4c 2066 696c 6573 2061 6e64  n TOML files and
-00003d40: 2069 7320 666f 7220 7265 6164 6162 696c   is for readabil
-00003d50: 6974 7920 6f6e 6c79 2e0a 0a23 2320 4854  ity only...## HT
-00003d60: 5450 5320 5072 6f78 7920 5375 7070 6f72  TPS Proxy Suppor
-00003d70: 740a 0a54 6865 2063 6f6d 6d61 6e64 7320  t..The commands 
-00003d80: 7769 6c6c 2075 7365 2074 6865 2076 616c  will use the val
-00003d90: 7565 206f 6620 7468 6520 656e 7669 726f  ue of the enviro
-00003da0: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
-00003db0: 4854 5450 535f 5052 4f58 5960 2069 6620  HTTPS_PROXY` if 
-00003dc0: 726f 7574 696e 6720 7468 726f 7567 6820  routing through 
-00003dd0: 6120 7072 6f78 7920 6973 2072 6571 7569  a proxy is requi
-00003de0: 7265 642e 0a0a 496e 2061 6464 6974 696f  red...In additio
-00003df0: 6e2c 2074 6865 2063 6f6d 6d61 6e64 7320  n, the commands 
-00003e00: 6361 6e20 7573 6520 7072 6f78 7920 6175  can use proxy au
-00003e10: 746f 636f 6e66 6967 7572 6174 696f 6e20  toconfiguration 
-00003e20: 2850 4143 2920 6966 2074 6865 2060 2d2d  (PAC) if the `--
-00003e30: 7061 6360 2063 6f6d 6d61 6e64 206c 696e  pac` command lin
-00003e40: 6520 6f70 7469 6f6e 2069 7320 7370 6563  e option is spec
-00003e50: 6966 6965 642c 206f 7220 6966 2074 6865  ified, or if the
-00003e60: 2060 7573 6550 4143 6020 7072 6f70 6572   `usePAC` proper
-00003e70: 7479 2069 7320 7365 7420 746f 2060 7472  ty is set to `tr
-00003e80: 7565 6020 696e 2074 6865 2060 5b63 6f6d  ue` in the `[com
-00003e90: 6d6f 6e5d 6020 7365 6374 696f 6e20 6f66  mon]` section of
-00003ea0: 2074 6865 2060 636f 6e66 6967 2e74 6f6d   the `config.tom
-00003eb0: 6c60 2066 696c 652e 0a0a 2323 2053 7065  l` file...## Spe
-00003ec0: 6369 6679 696e 6720 436f 6d6d 6f6e 2050  cifying Common P
-00003ed0: 726f 7065 7274 6965 7320 7573 696e 6720  roperties using 
-00003ee0: 7468 6520 436f 6d6d 616e 6420 4c69 6e65  the Command Line
-00003ef0: 206f 7220 456e 7669 726f 6e6d 656e 7420   or Environment 
-00003f00: 5661 7269 6162 6c65 730a 0a41 6c6c 2074  Variables..All t
-00003f10: 6865 2063 6f6d 6d6f 6e20 7072 6f70 6572  he common proper
-00003f20: 7469 6573 2063 616e 2062 6520 7365 7420  ties can be set 
-00003f30: 7573 696e 6720 636f 6d6d 616e 6420 6c69  using command li
-00003f40: 6e65 206f 7074 696f 6e73 2c20 6f72 2069  ne options, or i
-00003f50: 6e20 656e 7669 726f 6e6d 656e 7420 7661  n environment va
-00003f60: 7269 6162 6c65 732e 0a0a 5468 6520 2a2a  riables...The **
-00003f70: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-00003f80: 696f 6e73 2a2a 2061 7265 2061 7320 666f  ions** are as fo
-00003f90: 6c6c 6f77 733a 0a0a 2d20 602d 2d6b 6579  llows:..- `--key
-00003fa0: 6020 6f72 2060 2d6b 600a 2d20 602d 2d73  ` or `-k`.- `--s
-00003fb0: 6563 7265 7460 206f 7220 602d 7360 0a2d  ecret` or `-s`.-
-00003fc0: 2060 2d2d 6e61 6d65 7370 6163 6560 206f   `--namespace` o
-00003fd0: 7220 602d 6e60 0a2d 2060 2d2d 7461 6760  r `-n`.- `--tag`
-00003fe0: 206f 7220 602d 7460 0a2d 2060 2d2d 7572   or `-t`.- `--ur
-00003ff0: 6c60 206f 7220 602d 7560 0a2d 2060 2d2d  l` or `-u`.- `--
-00004000: 7061 6360 0a0a 5468 6573 6520 6f70 7469  pac`..These opti
-00004010: 6f6e 7320 6361 6e20 616c 736f 2062 6520  ons can also be 
-00004020: 6c69 7374 6564 2062 7920 7275 6e6e 696e  listed by runnin
-00004030: 6720 6120 636f 6d6d 616e 6420 7769 7468  g a command with
-00004040: 2074 6865 2060 2d2d 6865 6c70 6020 6f72   the `--help` or
-00004050: 2060 2d68 6020 6f70 7469 6f6e 2e0a 0a54   `-h` option...T
-00004060: 6865 202a 2a65 6e76 6972 6f6e 6d65 6e74  he **environment
-00004070: 2076 6172 6961 626c 6573 2a2a 2061 7265   variables** are
-00004080: 2061 7320 666f 6c6c 6f77 733a 0a0a 2d20   as follows:..- 
-00004090: 6059 445f 4b45 5960 0a2d 2060 5944 5f53  `YD_KEY`.- `YD_S
-000040a0: 4543 5245 5460 0a2d 2060 5944 5f4e 414d  ECRET`.- `YD_NAM
-000040b0: 4553 5041 4345 600a 2d20 6059 445f 5441  ESPACE`.- `YD_TA
-000040c0: 4760 0a2d 2060 5944 5f55 524c 600a 0a57  G`.- `YD_URL`..W
-000040d0: 6865 6e20 7365 7474 696e 6720 7468 6520  hen setting the 
-000040e0: 7661 6c75 6520 6f66 2074 6865 2061 626f  value of the abo
-000040f0: 7665 2070 726f 7065 7274 6965 732c 2061  ve properties, a
-00004100: 2070 726f 7065 7274 7920 7365 7420 6f6e   property set on
-00004110: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00004120: 6520 7461 6b65 7320 7072 6563 6564 656e  e takes preceden
-00004130: 6365 206f 7665 7220 6f6e 6520 7365 7420  ce over one set 
-00004140: 7669 6120 616e 2065 6e76 6972 6f6e 6d65  via an environme
-00004150: 6e74 2076 6172 6961 626c 652c 2061 6e64  nt variable, and
-00004160: 2062 6f74 6820 7461 6b65 2070 7265 6365   both take prece
-00004170: 6465 6e63 6520 6f76 6572 2061 2076 616c  dence over a val
-00004180: 7565 2073 6574 2069 6e20 6120 636f 6e66  ue set in a conf
-00004190: 6967 7572 6174 696f 6e20 6669 6c65 2e0a  iguration file..
-000041a0: 0a49 6620 616c 6c20 7468 6520 7265 7175  .If all the requ
-000041b0: 6972 6564 2063 6f6d 6d6f 6e20 7072 6f70  ired common prop
-000041c0: 6572 7469 6573 2061 7265 2073 6574 2075  erties are set u
-000041d0: 7369 6e67 2074 6865 2063 6f6d 6d61 6e64  sing the command
-000041e0: 206c 696e 6520 6f72 2065 6e76 6972 6f6e   line or environ
-000041f0: 6d65 6e74 2076 6172 6961 626c 6573 2c20  ment variables, 
-00004200: 7468 656e 2074 6865 2065 6e74 6972 6520  then the entire 
-00004210: 6063 6f6d 6d6f 6e60 2073 6563 7469 6f6e  `common` section
-00004220: 206f 6620 7468 6520 544f 4d4c 2066 696c   of the TOML fil
-00004230: 6520 6361 6e20 6265 206f 6d69 7474 6564  e can be omitted
-00004240: 2e0a 0a23 2320 5661 7269 6162 6c65 2053  ...## Variable S
-00004250: 7562 7374 6974 7574 696f 6e73 2069 6e20  ubstitutions in 
-00004260: 436f 6d6d 6f6e 2050 726f 7065 7274 6965  Common Propertie
-00004270: 730a 0a4e 6f74 6520 7468 6520 7573 6520  s..Note the use 
-00004280: 6f66 2060 7b7b 7573 6572 6e61 6d65 7d7d  of `{{username}}
-00004290: 6020 696e 2074 6865 2076 616c 7565 206f  ` in the value o
-000042a0: 6620 7468 6520 6074 6167 6020 7072 6f70  f the `tag` prop
-000042b0: 6572 7479 3a20 7468 6973 2069 7320 6120  erty: this is a 
-000042c0: 2a2a 7661 7269 6162 6c65 2073 7562 7374  **variable subst
-000042d0: 6974 7574 696f 6e2a 2a20 7468 6174 2063  itution** that c
-000042e0: 616e 206f 7074 696f 6e61 6c6c 7920 6265  an optionally be
-000042f0: 2075 7365 6420 746f 2069 6e73 6572 7420   used to insert 
-00004300: 7468 6520 6c6f 6769 6e20 7573 6572 6e61  the login userna
-00004310: 6d65 206f 6620 7468 6520 7573 6572 2072  me of the user r
-00004320: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
-00004330: 6e64 732e 2053 6f2c 2066 6f72 2075 7365  nds. So, for use
-00004340: 726e 616d 6520 6061 6263 602c 2074 6865  rname `abc`, the
-00004350: 2060 7461 6760 2077 6f75 6c64 2062 6520   `tag` would be 
-00004360: 7365 7420 746f 2060 7465 7374 696e 672d  set to `testing-
-00004370: 6162 6360 2e20 5468 6973 2063 616e 2062  abc`. This can b
-00004380: 6520 6865 6c70 6675 6c20 746f 2064 6973  e helpful to dis
-00004390: 616d 6269 6775 6174 6520 6d75 6c74 6970  ambiguate multip
-000043a0: 6c65 2075 7365 7273 2072 756e 6e69 6e67  le users running
-000043b0: 2077 6974 6820 7468 6520 7361 6d65 2063   with the same c
-000043c0: 6f6e 6669 6775 7261 7469 6f6e 2064 6174  onfiguration dat
-000043d0: 612e 0a0a 5661 7269 6162 6c65 2073 7562  a...Variable sub
-000043e0: 7374 6974 7574 696f 6e73 2061 7265 2064  stitutions are d
-000043f0: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
-00004400: 0a23 2056 6172 6961 626c 6520 5375 6273  .# Variable Subs
-00004410: 7469 7475 7469 6f6e 730a 0a56 6172 6961  titutions..Varia
-00004420: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
-00004430: 7320 7072 6f76 6964 6520 6120 706f 7765  s provide a powe
-00004440: 7266 756c 2077 6179 206f 6620 696e 7472  rful way of intr
-00004450: 6f64 7563 696e 6720 7661 7269 6162 6c65  oducing variable
-00004460: 2076 616c 7565 7320 696e 746f 2054 4f4d   values into TOM
-00004470: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
-00004480: 6669 6c65 732c 2057 6f72 6b20 5265 7175  files, Work Requ
-00004490: 6972 656d 656e 7420 4a53 4f4e 2064 6566  irement JSON def
-000044a0: 696e 6974 696f 6e73 2c20 616e 6420 576f  initions, and Wo
-000044b0: 726b 6572 2050 6f6f 6c20 4a53 4f4e 2064  rker Pool JSON d
-000044c0: 6566 696e 6974 696f 6e73 2e20 5468 6579  efinitions. They
-000044d0: 2063 616e 2062 6520 696e 636c 7564 6564   can be included
-000044e0: 2069 6e20 7468 6520 7661 6c75 6520 6f66   in the value of
-000044f0: 2061 6e79 2070 726f 7065 7274 7920 696e   any property in
-00004500: 2065 6163 6820 6f66 2074 6865 7365 206f   each of these o
-00004510: 626a 6563 7473 2c20 696e 636c 7564 696e  bjects, includin
-00004520: 6720 696e 2076 616c 7565 7320 7769 7468  g in values with
-00004530: 696e 206c 6973 7473 2028 652e 672e 2c20  in lists (e.g., 
-00004540: 666f 7220 7468 6520 6061 7267 756d 656e  for the `argumen
-00004550: 7473 6020 7072 6f70 6572 7479 2920 616e  ts` property) an
-00004560: 6420 6172 7261 7973 2028 652e 672e 2c20  d arrays (e.g., 
-00004570: 7468 6520 6065 6e76 6972 6f6e 6d65 6e74  the `environment
-00004580: 6020 7072 6f70 6572 7479 292e 0a0a 5661  ` property)...Va
-00004590: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-000045a0: 696f 6e73 2061 7265 2065 7870 7265 7373  ions are express
-000045b0: 6564 2075 7369 6e67 2060 7b7b 7661 7269  ed using `{{vari
-000045c0: 6162 6c65 7d7d 6020 6e6f 7461 7469 6f6e  able}}` notation
-000045d0: 2c20 7768 6572 6520 7468 6520 6578 7072  , where the expr
-000045e0: 6573 7369 6f6e 2069 7320 7265 706c 6163  ession is replac
-000045f0: 6564 2062 7920 7468 6520 7661 6c75 6520  ed by the value 
-00004600: 6f66 2060 7661 7269 6162 6c65 602e 0a0a  of `variable`...
-00004610: 5375 6273 7469 7475 7469 6f6e 7320 6361  Substitutions ca
-00004620: 6e20 616c 736f 2062 6520 7065 7266 6f72  n also be perfor
-00004630: 6d65 6420 666f 7220 6e6f 6e2d 7374 7269  med for non-stri
-00004640: 6e67 2028 6e75 6d62 6572 2061 6e64 2062  ng (number and b
-00004650: 6f6f 6c65 616e 2920 7661 6c75 6573 2075  oolean) values u
-00004660: 7369 6e67 2074 6865 2060 6e75 6d3a 6020  sing the `num:` 
-00004670: 616e 6420 6062 6f6f 6c3a 6020 7072 6566  and `bool:` pref
-00004680: 6978 6573 2077 6974 6869 6e20 7468 6520  ixes within the 
-00004690: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
-000046a0: 7574 696f 6e3a 0a0a 2d20 4465 6669 6e65  ution:..- Define
-000046b0: 2074 6865 2076 6172 6961 626c 6520 7375   the variable su
-000046c0: 6273 7469 7475 7469 6f6e 2075 7369 6e67  bstitution using
-000046d0: 206f 6e65 206f 6620 7468 6520 666f 6c6c   one of the foll
-000046e0: 6f77 696e 6720 7061 7474 6572 6e73 3a20  owing patterns: 
-000046f0: 6022 7b7b 6e75 6d3a 6d79 5f69 6e74 7d7d  `"{{num:my_int}}
-00004700: 2260 2c20 6022 7b7b 6e75 6d3a 6d79 5f66  "`, `"{{num:my_f
-00004710: 6c6f 6174 7d7d 2260 2c20 6022 7b7b 626f  loat}}"`, `"{{bo
-00004720: 6f6c 3a6d 795f 626f 6f6c 7d7d 2260 0a2d  ol:my_bool}}"`.-
-00004730: 2056 6172 6961 626c 6520 6465 6669 6e69   Variable defini
-00004740: 7469 6f6e 7320 7375 7070 6c69 6564 206f  tions supplied o
-00004750: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
-00004760: 6e65 2077 6f75 6c64 2074 6865 6e20 6265  ne would then be
-00004770: 206f 6620 7468 6520 666f 726d 3a20 602d   of the form: `-
-00004780: 6d20 6d79 5f69 6e74 3d35 202d 6d20 6d79  m my_int=5 -m my
-00004790: 5f66 6c6f 6174 3d32 2e35 202d 6d20 6d79  _float=2.5 -m my
-000047a0: 5f62 6f6f 6c3d 7472 7565 600a 2d20 496e  _bool=true`.- In
-000047b0: 2074 6865 2070 726f 6365 7373 6564 204a   the processed J
-000047c0: 534f 4e20 6f72 2054 4f4d 4c2c 2074 6865  SON or TOML, the
-000047d0: 7365 2076 616c 7565 7320 776f 756c 6420  se values would 
-000047e0: 6265 636f 6d65 2060 3560 2c20 6032 2e35  become `5`, `2.5
-000047f0: 6020 616e 6420 6074 7275 6560 2c20 7265  ` and `true`, re
-00004800: 7370 6563 7469 7665 6c79 2c20 636f 6e76  spectively, conv
-00004810: 6572 7465 6420 6672 6f6d 2073 7472 696e  erted from strin
-00004820: 6773 2074 6f20 7468 6569 7220 636f 7272  gs to their corr
-00004830: 6563 7420 4a53 4f4e 2074 7970 6573 0a0a  ect JSON types..
-00004840: 2323 2044 6566 6175 6c74 2056 6172 6961  ## Default Varia
-00004850: 626c 6573 0a0a 5468 6520 666f 6c6c 6f77  bles..The follow
-00004860: 696e 6720 7375 6273 7469 7475 7469 6f6e  ing substitution
-00004870: 7320 6172 6520 6175 746f 6d61 7469 6361  s are automatica
-00004880: 6c6c 7920 6372 6561 7465 6420 616e 6420  lly created and 
-00004890: 6361 6e20 6265 2075 7365 6420 696e 2061  can be used in a
-000048a0: 6e79 2073 6563 7469 6f6e 206f 6620 7468  ny section of th
-000048b0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-000048c0: 6669 6c65 2c20 6f72 2069 6e20 616e 7920  file, or in any 
-000048d0: 4a53 4f4e 2073 7065 6369 6669 6361 7469  JSON specificati
-000048e0: 6f6e 3a0a 0a7c 2044 6972 6563 7469 7665  on:..| Directive
-000048f0: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
-00004900: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 7c20 4578 616d 706c 6520 6f66 2053    | Example of S
-00004950: 7562 7374 6974 7574 696f 6e20 7c0a 7c3a  ubstitution |.|:
-00004960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004970: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000049a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000049b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
-000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000049d0: 2d2d 2d2d 2d7c 0a7c 2060 7b7b 7573 6572  -----|.| `{{user
-000049e0: 6e61 6d65 7d7d 6020 207c 2054 6865 2063  name}}`  | The c
-000049f0: 7572 7265 6e74 2075 7365 7227 7320 6c6f  urrent user's lo
-00004a00: 6769 6e20 7573 6572 6e61 6d65 2c20 6c6f  gin username, lo
-00004a10: 7765 7220 6361 7365 2c20 7370 6163 6573  wer case, spaces
-00004a20: 2072 6570 6c61 6365 6420 2020 2020 2020   replaced       
-00004a30: 2020 2020 7c20 6a61 6e65 5f73 6d69 7468      | jane_smith
-00004a40: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00004a50: 7c20 607b 7b64 6174 657d 7d60 2020 2020  | `{{date}}`    
-00004a60: 2020 7c20 5468 6520 6375 7272 656e 7420    | The current 
-00004a70: 6461 7465 2028 5554 4329 3a20 5959 5959  date (UTC): YYYY
-00004a80: 4d4d 4444 2020 2020 2020 2020 2020 2020  MMDD            
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2020 2020 2020 207c 2032               | 2
-00004ab0: 3032 3231 3032 3720 2020 2020 2020 2020  0221027         
-00004ac0: 2020 2020 2020 207c 0a7c 2060 7b7b 7469         |.| `{{ti
-00004ad0: 6d65 7d7d 6020 2020 2020 207c 2054 6865  me}}`      | The
-00004ae0: 2063 7572 7265 6e74 2074 696d 6520 2855   current time (U
-00004af0: 5443 293a 2048 484d 4d53 5320 2020 2020  TC): HHMMSS     
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 7c20 3136 3330 3236 2020        | 163026  
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 7c0a 7c20 607b 7b64 6174 6574 696d 657d  |.| `{{datetime}
-00004b50: 7d60 2020 7c20 436f 6e63 6174 656e 6174  }`  | Concatenat
-00004b60: 696f 6e20 6f66 2074 6865 2064 6174 6520  ion of the date 
-00004b70: 616e 6420 7469 6d65 2061 626f 7665 2c20  and time above, 
-00004b80: 7769 7468 2061 2027 2d27 2073 6570 6172  with a '-' separ
-00004b90: 6174 6f72 2020 2020 2020 2020 2020 207c  ator           |
-00004ba0: 2032 3032 3231 3032 372d 3136 3330 3236   20221027-163026
-00004bb0: 2020 2020 2020 2020 207c 0a7c 2060 7b7b           |.| `{{
-00004bc0: 7261 6e64 6f6d 7d7d 6020 2020 207c 2041  random}}`    | A
-00004bd0: 2072 616e 646f 6d2c 2074 6872 6565 2064   random, three d
-00004be0: 6967 6974 2068 6578 6164 6563 696d 616c  igit hexadecimal
-00004bf0: 206e 756d 6265 7220 286c 6f77 6572 2063   number (lower c
-00004c00: 6173 6529 2020 2020 2020 2020 2020 2020  ase)            
-00004c10: 2020 2020 2020 2020 7c20 6131 6320 2020          | a1c   
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 7c0a 7c20 607b 7b6e 616d 6573 7061    |.| `{{namespa
-00004c40: 6365 7d7d 6020 7c20 5468 6520 606e 616d  ce}}` | The `nam
-00004c50: 6573 7061 6365 6020 7072 6f70 6572 7479  espace` property
-00004c60: 2e20 4e6f 7465 2074 6861 7420 606e 616d  . Note that `nam
-00004c70: 6573 7061 6365 6020 6d75 7374 2c20 6f66  espace` must, of
-00004c80: 2063 6f75 7273 652c 2062 6520 7365 742e   course, be set.
-00004c90: 207c 206d 795f 6e61 6d65 7370 6163 6520   | my_namespace 
-00004ca0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-00004cb0: 7b7b 7461 677d 7d60 2020 2020 2020 207c  {{tag}}`       |
-00004cc0: 2054 6865 2060 7461 6760 2070 726f 7065   The `tag` prope
-00004cd0: 7274 792e 204e 6f74 6520 7468 6174 2060  rty. Note that `
-00004ce0: 7461 6760 206d 7573 7420 6265 2073 6574  tag` must be set
-00004cf0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 2020 2020 2020 2020 2020 7c20 6d79 5f74            | my_t
-00004d10: 6167 2020 2020 2020 2020 2020 2020 2020  ag              
-00004d20: 2020 2020 7c0a 7c20 607b 7b6b 6579 7d7d      |.| `{{key}}
-00004d30: 6020 2020 2020 2020 7c20 5468 6520 6170  `       | The ap
-00004d40: 706c 6963 6174 696f 6e20 606b 6579 6020  plication `key` 
-00004d50: 7072 6f70 6572 7479 2e20 2020 2020 2020  property.       
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00004d90: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00004da0: 2060 7b7b 7365 6372 6574 7d7d 6020 2020   `{{secret}}`   
-00004db0: 207c 2054 6865 2061 7070 6c69 6361 7469   | The applicati
-00004dc0: 6f6e 2060 7365 6372 6574 6020 7072 6f70  on `secret` prop
-00004dd0: 6572 7479 2e20 2020 2020 2020 2020 2020  erty.           
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 7c0a 7c20 607b 7b75 726c        |.| `{{url
-00004e20: 7d7d 6020 2020 2020 2020 7c20 5468 6520  }}`       | The 
-00004e30: 506c 6174 666f 726d 2060 7572 6c60 2070  Platform `url` p
-00004e40: 726f 7065 7274 792e 2020 2020 2020 2020  roperty.        
-00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2074 6865 2074 6167 2074         the tag t
+00002da0: 6f20 7573 6520 666f 7220 7461 6767 696e  o use for taggin
+00002db0: 6720 616e 6420 6e61 6d69 6e67 2065 6e74  g and naming ent
+00002dc0: 6974 6965 730a 2020 2d2d 7572 6c20 3c75  ities.  --url <u
+00002dd0: 726c 3e2c 202d 7520 3c75 726c 3e0a 2020  rl>, -u <url>.  
+00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002df0: 2020 2020 2020 7468 6520 5552 4c20 6f66        the URL of
+00002e00: 2074 6865 2059 656c 6c6f 7744 6f67 2050   the YellowDog P
+00002e10: 6c61 7466 6f72 6d20 4150 490a 2020 2d2d  latform API.  --
+00002e20: 7661 7269 6162 6c65 203c 7661 7231 3d76  variable <var1=v
+00002e30: 313e 2c20 2d76 203c 7661 7231 3d76 313e  1>, -v <var1=v1>
+00002e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002e50: 2020 2020 2020 2020 2075 7365 722d 6465           user-de
+00002e60: 6669 6e65 6420 7661 7269 6162 6c65 2073  fined variable s
+00002e70: 7562 7374 6974 7574 696f 6e73 3b20 6361  ubstitutions; ca
+00002e80: 6e20 6265 2073 7570 706c 6965 6420 6d75  n be supplied mu
+00002e90: 6c74 6970 6c65 2074 696d 6573 0a20 202d  ltiple times.  -
+00002ea0: 2d71 7569 6574 2c20 2d71 2020 2020 2020  -quiet, -q      
+00002eb0: 2020 2020 2073 7570 7072 6573 7320 286e       suppress (n
+00002ec0: 6f6e 2d65 7272 6f72 2c20 6e6f 6e2d 696e  on-error, non-in
+00002ed0: 7465 7261 6374 6976 6529 2073 7461 7475  teractive) statu
+00002ee0: 7320 616e 6420 7072 6f67 7265 7373 206d  s and progress m
+00002ef0: 6573 7361 6765 730a 2020 2d2d 6465 6275  essages.  --debu
+00002f00: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+00002f10: 7072 696e 7420 6120 7374 6163 6b20 7472  print a stack tr
+00002f20: 6163 6520 2865 7463 2e29 206f 6e20 6572  ace (etc.) on er
+00002f30: 726f 720a 2020 2d2d 7061 6320 2020 2020  ror.  --pac     
+00002f40: 2020 2020 2020 2020 2020 2020 656e 6162              enab
+00002f50: 6c65 2050 4143 2028 7072 6f78 7920 6175  le PAC (proxy au
+00002f60: 746f 2d63 6f6e 6669 6775 7261 7469 6f6e  to-configuration
+00002f70: 2920 7375 7070 6f72 740a 2020 2d2d 6162  ) support.  --ab
+00002f80: 6f72 742c 202d 6120 2020 2020 2020 2020  ort, -a         
+00002f90: 2020 6162 6f72 7420 616c 6c20 7275 6e6e    abort all runn
+00002fa0: 696e 6720 7461 736b 7320 7769 7468 2069  ing tasks with i
+00002fb0: 6d6d 6564 6961 7465 2065 6666 6563 740a  mmediate effect.
+00002fc0: 2020 2d2d 666f 6c6c 6f77 2c20 2d66 2020    --follow, -f  
+00002fd0: 2020 2020 2020 2020 7768 656e 2075 7369          when usi
+00002fe0: 6e67 202d 2d61 626f 7274 2c20 706f 6c6c  ng --abort, poll
+00002ff0: 2075 6e74 696c 2061 6c6c 2054 6173 6b73   until all Tasks
+00003000: 2068 6176 6520 6265 656e 2061 626f 7274   have been abort
+00003010: 6564 0a20 202d 2d69 6e74 6572 6163 7469  ed.  --interacti
+00003020: 7665 2c20 2d69 2020 2020 206c 6973 742c  ve, -i     list,
+00003030: 2061 6e64 2069 6e74 6572 6163 7469 7665   and interactive
+00003040: 6c79 2073 656c 6563 742c 2069 7465 6d73  ly select, items
+00003050: 2074 6f20 6163 7420 6f6e 0a20 202d 2d79   to act on.  --y
+00003060: 6573 2c20 2d79 2020 2020 2020 2020 2020  es, -y          
+00003070: 2020 2070 6572 666f 726d 2064 6573 7472     perform destr
+00003080: 7563 7469 7665 2061 6374 696f 6e73 2077  uctive actions w
+00003090: 6974 686f 7574 2072 6571 7569 7269 6e67  ithout requiring
+000030a0: 2075 7365 7220 636f 6e66 6972 6d61 7469   user confirmati
+000030b0: 6f6e 0a60 6060 0a0a 2320 436f 6e66 6967  on.```..# Config
+000030c0: 7572 6174 696f 6e0a 0a42 7920 6465 6661  uration..By defa
+000030d0: 756c 742c 2074 6865 206f 7065 7261 7469  ult, the operati
+000030e0: 6f6e 206f 6620 616c 6c20 636f 6d6d 616e  on of all comman
+000030f0: 6473 2069 7320 636f 6e66 6967 7572 6564  ds is configured
+00003100: 2075 7369 6e67 2061 2054 4f4d 4c20 636f   using a TOML co
+00003110: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00003120: 2e0a 0a54 6865 2063 6f6e 6669 6775 7261  ...The configura
+00003130: 7469 6f6e 2066 696c 6520 6861 7320 7468  tion file has th
+00003140: 7265 6520 706f 7373 6962 6c65 2073 6563  ree possible sec
+00003150: 7469 6f6e 733a 0a0a 312e 2041 2060 636f  tions:..1. A `co
+00003160: 6d6d 6f6e 6020 7365 6374 696f 6e20 7468  mmon` section th
+00003170: 6174 2063 6f6e 7461 696e 7320 7265 7175  at contains requ
+00003180: 6972 6564 2073 6563 7572 6974 7920 7072  ired security pr
+00003190: 6f70 6572 7469 6573 2066 6f72 2069 6e74  operties for int
+000031a0: 6572 6163 7469 6e67 2077 6974 6820 7468  eracting with th
+000031b0: 6520 5965 6c6c 6f77 446f 6720 706c 6174  e YellowDog plat
+000031c0: 666f 726d 2c20 7365 7473 2074 6865 204e  form, sets the N
+000031d0: 616d 6573 7061 6365 2069 6e20 7768 6963  amespace in whic
+000031e0: 6820 5965 6c6c 6f77 446f 6720 6173 7365  h YellowDog asse
+000031f0: 7473 2061 6e64 206f 626a 6563 7473 2061  ts and objects a
+00003200: 7265 2063 7265 6174 6564 2c20 616e 6420  re created, and 
+00003210: 6120 5461 6720 7468 6174 2069 7320 7573  a Tag that is us
+00003220: 6564 2066 6f72 2074 6167 6769 6e67 2061  ed for tagging a
+00003230: 6e64 206e 616d 696e 6720 6173 7365 7473  nd naming assets
+00003240: 2061 6e64 206f 626a 6563 7473 2e0a 322e   and objects..2.
+00003250: 2041 2060 776f 726b 5265 7175 6972 656d   A `workRequirem
+00003260: 656e 7460 2073 6563 7469 6f6e 2074 6861  ent` section tha
+00003270: 7420 6465 6669 6e65 7320 7468 6520 7072  t defines the pr
+00003280: 6f70 6572 7469 6573 206f 6620 576f 726b  operties of Work
+00003290: 2052 6571 7569 7265 6d65 6e74 7320 746f   Requirements to
+000032a0: 2062 6520 7375 626d 6974 7465 6420 746f   be submitted to
+000032b0: 2074 6865 2059 656c 6c6f 7744 6f67 2070   the YellowDog p
+000032c0: 6c61 7466 6f72 6d2e 0a33 2e20 4120 6077  latform..3. A `w
+000032d0: 6f72 6b65 7250 6f6f 6c60 2073 6563 7469  orkerPool` secti
+000032e0: 6f6e 2074 6861 7420 6465 6669 6e65 7320  on that defines 
+000032f0: 7468 6520 7072 6f70 6572 7469 6573 206f  the properties o
+00003300: 6620 5072 6f76 6973 6f6e 6564 2057 6f72  f Provisoned Wor
+00003310: 6b65 7220 506f 6f6c 7320 746f 2062 6520  ker Pools to be 
+00003320: 6372 6561 7465 6420 7573 696e 6720 7468  created using th
+00003330: 6520 5965 6c6c 6f77 446f 6720 706c 6174  e YellowDog plat
+00003340: 666f 726d 2e20 0a0a 5468 6572 6520 6973  form. ..There is
+00003350: 2061 2064 6f63 756d 656e 7465 6420 7465   a documented te
+00003360: 6d70 6c61 7465 2054 4f4d 4c20 6669 6c65  mplate TOML file
+00003370: 2070 726f 7669 6465 6420 696e 205b 636f   provided in [co
+00003380: 6e66 6967 2e74 6f6d 6c2e 7465 6d70 6c61  nfig.toml.templa
+00003390: 7465 5d28 636f 6e66 6967 2e74 6f6d 6c2e  te](config.toml.
+000033a0: 7465 6d70 6c61 7465 292c 2063 6f6e 7461  template), conta
+000033b0: 696e 696e 6720 7468 6520 6d61 696e 2070  ining the main p
+000033c0: 726f 7065 7274 6965 7320 7468 6174 2063  roperties that c
+000033d0: 616e 2062 6520 636f 6e66 6967 7572 6564  an be configured
+000033e0: 2e0a 0a54 6865 2063 6f6e 6669 6775 7261  ...The configura
+000033f0: 7469 6f6e 2066 696c 656e 616d 6520 6361  tion filename ca
+00003400: 6e20 6265 2073 7570 706c 6965 6420 696e  n be supplied in
+00003410: 2074 6872 6565 2064 6966 6665 7265 6e74   three different
+00003420: 2077 6179 733a 0a0a 312e 204f 6e20 7468   ways:..1. On th
+00003430: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
+00003440: 7573 696e 6720 7468 6520 602d 2d63 6f6e  using the `--con
+00003450: 6669 6760 206f 7220 602d 6360 206f 7074  fig` or `-c` opt
+00003460: 696f 6e73 2c20 652e 672e 3a3c 6272 3e60  ions, e.g.:<br>`
+00003470: 7964 2d73 7562 6d69 7420 2d63 206a 6f62  yd-submit -c job
+00003480: 732f 636f 6e66 6967 5f31 2e74 6f6d 6c60  s/config_1.toml`
+00003490: 0a32 2e20 5573 696e 6720 7468 6520 6059  .2. Using the `Y
+000034a0: 445f 434f 4e46 6020 656e 7669 726f 6e6d  D_CONF` environm
+000034b0: 656e 7420 7661 7269 6162 6c65 2c20 652e  ent variable, e.
+000034c0: 672e 3a20 3c62 723e 6065 7870 6f72 7420  g.: <br>`export 
+000034d0: 5944 5f43 4f4e 463d 226a 6f62 732f 636f  YD_CONF="jobs/co
+000034e0: 6e66 6967 5f31 2e74 6f6d 6c22 600a 332e  nfig_1.toml"`.3.
+000034f0: 2049 6620 6e65 6974 6865 7220 6f66 2074   If neither of t
+00003500: 6865 2061 626f 7665 2069 7320 7375 7070  he above is supp
+00003510: 6c69 6564 2c20 7468 6520 636f 6d6d 616e  lied, the comman
+00003520: 6473 206c 6f6f 6b20 666f 7220 6120 6063  ds look for a `c
+00003530: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00003540: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00003550: 6469 7265 6374 6f72 790a 0a54 6865 206f  directory..The o
+00003560: 7074 696f 6e73 2061 626f 7665 2061 7265  ptions above are
+00003570: 2073 686f 776e 2069 6e20 6f72 6465 7220   shown in order 
+00003580: 6f66 2070 7265 6365 6465 6e63 652c 2069  of precedence, i
+00003590: 2e65 2e2c 2061 2066 696c 656e 616d 6520  .e., a filename 
+000035a0: 7375 7070 6c69 6564 206f 6e20 7468 6520  supplied on the 
+000035b0: 636f 6d6d 616e 6420 6c69 6e65 2073 7570  command line sup
+000035c0: 6572 7365 6465 7320 6f6e 6520 7365 7420  ersedes one set 
+000035d0: 696e 2060 5944 5f43 4f4e 4660 2c20 7768  in `YD_CONF`, wh
+000035e0: 6963 6820 7375 7065 7273 6564 6573 2074  ich supersedes t
+000035f0: 6865 2064 6566 6175 6c74 2e0a 0a23 204e  he default...# N
+00003600: 616d 696e 6720 5275 6c65 730a 0a41 6c6c  aming Rules..All
+00003610: 2065 6e74 6974 7920 6e61 6d65 7320 7573   entity names us
+00003620: 6564 2077 6974 6869 6e20 7468 6520 5965  ed within the Ye
+00003630: 6c6c 6f77 446f 6720 506c 6174 666f 726d  llowDog Platform
+00003640: 206d 7573 7420 636f 6d70 6c79 2077 6974   must comply wit
+00003650: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
+00003660: 7265 7374 7269 6374 696f 6e73 3a0a 0a2d  restrictions:..-
+00003670: 204e 616d 6573 2063 616e 206f 6e6c 7920   Names can only 
+00003680: 636f 6e74 6169 6e20 7468 6520 666f 6c6c  contain the foll
+00003690: 6f77 696e 673a 206c 6f77 6572 6361 7365  owing: lowercase
+000036a0: 206c 6574 7465 7273 2c20 6469 6769 7473   letters, digits
+000036b0: 2c20 6879 7068 656e 7320 616e 6420 756e  , hyphens and un
+000036c0: 6465 7273 636f 7265 7320 286e 6f74 6520  derscores (note 
+000036d0: 7468 6174 2073 7061 6365 7320 6172 6520  that spaces are 
+000036e0: 6e6f 7420 7065 726d 6974 7465 6429 0a2d  not permitted).-
+000036f0: 204e 616d 6573 206d 7573 7420 7374 6172   Names must star
+00003700: 7420 7769 7468 2061 206c 6574 7465 720a  t with a letter.
+00003710: 2d20 4e61 6d65 7320 6d75 7374 2065 6e64  - Names must end
+00003720: 2077 6974 6820 6120 6c65 7474 6572 206f   with a letter o
+00003730: 7220 6469 6769 740a 2d20 4e61 6d65 206c  r digit.- Name l
+00003740: 656e 6774 6820 6d75 7374 2062 6520 3c3d  ength must be <=
+00003750: 2036 3020 6368 6172 6163 7465 7273 0a0a   60 characters..
+00003760: 5468 6573 6520 7265 7374 7269 6374 696f  These restrictio
+00003770: 6e73 2061 7070 6c79 2074 6f20 656e 7469  ns apply to enti
+00003780: 7469 6573 2069 6e63 6c75 6469 6e67 204e  ties including N
+00003790: 616d 6573 7061 6365 732c 2054 6167 732c  amespaces, Tags,
+000037a0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000037b0: 7473 2c20 5461 736b 2047 726f 7570 732c  ts, Task Groups,
+000037c0: 2054 6173 6b73 2c20 576f 726b 6572 2050   Tasks, Worker P
+000037d0: 6f6f 6c73 2c20 616e 6420 436f 6d70 7574  ools, and Comput
+000037e0: 6520 5265 7175 6972 656d 656e 7473 2c20  e Requirements, 
+000037f0: 616e 6420 616c 736f 2061 7070 6c79 2074  and also apply t
+00003800: 6f20 656e 7469 7469 6573 2074 6861 7420  o entities that 
+00003810: 6172 6520 6375 7272 656e 746c 7920 7573  are currently us
+00003820: 6564 2069 6e64 6972 6563 746c 7920 6279  ed indirectly by
+00003830: 2074 6865 7365 2073 6372 6970 7473 2c20   these scripts, 
+00003840: 696e 636c 7564 696e 6720 5573 6572 6e61  including Userna
+00003850: 6d65 732c 2043 7265 6465 6e74 6961 6c73  mes, Credentials
+00003860: 2c20 4b65 7972 696e 6773 2c20 436f 6d70  , Keyrings, Comp
+00003870: 7574 6520 536f 7572 6365 7320 616e 6420  ute Sources and 
+00003880: 436f 6d70 7574 6520 5465 6d70 6c61 7465  Compute Template
+00003890: 732e 0a0a 2320 436f 6d6d 6f6e 2050 726f  s...# Common Pro
+000038a0: 7065 7274 6965 730a 0a54 6865 2060 5b63  perties..The `[c
+000038b0: 6f6d 6d6f 6e5d 6020 7365 6374 696f 6e20  ommon]` section 
+000038c0: 6f66 2074 6865 2063 6f6e 6669 6775 7261  of the configura
+000038d0: 7469 6f6e 2066 696c 6520 6361 6e20 636f  tion file can co
+000038e0: 6e74 6169 6e20 7468 6520 666f 6c6c 6f77  ntain the follow
+000038f0: 696e 6720 7072 6f70 6572 7469 6573 3a0a  ing properties:.
+00003900: 0a7c 2050 726f 7065 7274 7920 2020 207c  .| Property    |
+00003910: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003960: 2020 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d       |.|:-------
+00003970: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d  -----|:---------
+00003980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000039a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000039b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000039c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2060  -----------|.| `
+000039d0: 6b65 7960 2020 2020 2020 207c 2054 6865  key`       | The
+000039e0: 202a 2a6b 6579 2a2a 206f 6620 7468 6520   **key** of the 
+000039f0: 5965 6c6c 6f77 446f 6720 4170 706c 6963  YellowDog Applic
+00003a00: 6174 696f 6e20 756e 6465 7220 7768 6963  ation under whic
+00003a10: 6820 7468 6520 636f 6d6d 616e 6473 2077  h the commands w
+00003a20: 696c 6c20 7275 6e20 2020 2020 2020 2020  ill run         
+00003a30: 207c 0a7c 2060 7365 6372 6574 6020 2020   |.| `secret`   
+00003a40: 207c 2054 6865 202a 2a73 6563 7265 742a   | The **secret*
+00003a50: 2a20 6f66 2074 6865 2059 656c 6c6f 7744  * of the YellowD
+00003a60: 6f67 2041 7070 6c69 6361 7469 6f6e 2075  og Application u
+00003a70: 6e64 6572 2077 6869 6368 2074 6865 2063  nder which the c
+00003a80: 6f6d 6d61 6e64 7320 7769 6c6c 2072 756e  ommands will run
+00003a90: 2020 2020 2020 207c 0a7c 2060 6e61 6d65         |.| `name
+00003aa0: 7370 6163 6560 207c 2054 6865 202a 2a6e  space` | The **n
+00003ab0: 616d 6573 7061 6365 2a2a 2074 6f20 6265  amespace** to be
+00003ac0: 2075 7365 6420 666f 7220 6772 6f75 7069   used for groupi
+00003ad0: 6e67 2072 6573 6f75 7263 6573 2020 2020  ng resources    
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00003b00: 2060 7461 6760 2020 2020 2020 207c 2054   `tag`       | T
+00003b10: 6865 202a 2a74 6167 2a2a 2074 6f20 6265  he **tag** to be
+00003b20: 2075 7365 6420 666f 7220 7461 6767 696e   used for taggin
+00003b30: 6720 7265 736f 7572 6365 7320 616e 6420  g resources and 
+00003b40: 6e61 6d69 6e67 206f 626a 6563 7473 2020  naming objects  
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 2020 207c 0a7c 2060 7572 6c60 2020 2020     |.| `url`    
+00003b70: 2020 207c 2054 6865 202a 2a55 524c 2a2a     | The **URL**
+00003b80: 206f 6620 7468 6520 5965 6c6c 6f77 446f   of the YellowDo
+00003b90: 6720 506c 6174 666f 726d 2041 5049 2065  g Platform API e
+00003ba0: 6e64 706f 696e 742c 2069 6620 7468 6520  ndpoint, if the 
+00003bb0: 6465 6661 756c 7420 6973 6e27 7420 746f  default isn't to
+00003bc0: 2062 6520 7573 6564 207c 0a7c 2060 7573   be used |.| `us
+00003bd0: 6550 4143 6020 2020 207c 2055 7365 2050  ePAC`    | Use P
+00003be0: 4143 2028 7072 6f78 7920 6175 746f 636f  AC (proxy autoco
+00003bf0: 6e66 6967 7572 6174 696f 6e29 2069 6620  nfiguration) if 
+00003c00: 7365 7420 746f 2060 7472 7565 6020 2020  set to `true`   
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00003c30: 0a7c 2060 7661 7269 6162 6c65 7360 207c  .| `variables` |
+00003c40: 2041 2074 6162 6c65 2063 6f6e 7461 696e   A table contain
+00003c50: 696e 6720 2a2a 7661 7269 6162 6c65 2073  ing **variable s
+00003c60: 7562 7374 6974 7574 696f 6e73 2a2a 2028  ubstitutions** (
+00003c70: 7365 6520 7468 6520 5661 7269 6162 6c65  see the Variable
+00003c80: 7320 7365 6374 696f 6e20 6265 6c6f 7729  s section below)
+00003c90: 2020 2020 207c 0a0a 416e 2065 7861 6d70       |..An examp
+00003ca0: 6c65 2060 636f 6d6d 6f6e 6020 7365 6374  le `common` sect
+00003cb0: 696f 6e20 6973 2073 686f 776e 2062 656c  ion is shown bel
+00003cc0: 6f77 3a0a 0a60 6060 746f 6d6c 0a5b 636f  ow:..```toml.[co
+00003cd0: 6d6d 6f6e 5d0a 2020 2020 6b65 7920 3d20  mmon].    key = 
+00003ce0: 2261 7364 6667 686a 6b6c 7a78 6376 622d  "asdfghjklzxcvb-
+00003cf0: 3132 3334 3536 3722 0a20 2020 2073 6563  1234567".    sec
+00003d00: 7265 7420 3d20 2271 7765 7274 7975 696f  ret = "qwertyuio
+00003d10: 7061 7364 6667 686a 6b6c 7a78 6376 626e  pasdfghjklzxcvbn
+00003d20: 6d31 3233 3435 3637 3839 3071 7765 7274  m1234567890qwert
+00003d30: 7975 220a 2020 2020 6e61 6d65 7370 6163  yu".    namespac
+00003d40: 6520 3d20 2270 726f 6a65 6374 2d78 220a  e = "project-x".
+00003d50: 2020 2020 7461 6720 3d20 2274 6573 7469      tag = "testi
+00003d60: 6e67 2d7b 7b75 7365 726e 616d 657d 7d22  ng-{{username}}"
+00003d70: 0a60 6060 0a0a 496e 6465 6e74 6174 696f  .```..Indentatio
+00003d80: 6e20 6973 206f 7074 696f 6e61 6c20 696e  n is optional in
+00003d90: 2054 4f4d 4c20 6669 6c65 7320 616e 6420   TOML files and 
+00003da0: 6973 2066 6f72 2072 6561 6461 6269 6c69  is for readabili
+00003db0: 7479 206f 6e6c 792e 0a0a 2323 2048 5454  ty only...## HTT
+00003dc0: 5053 2050 726f 7879 2053 7570 706f 7274  PS Proxy Support
+00003dd0: 0a0a 5468 6520 636f 6d6d 616e 6473 2077  ..The commands w
+00003de0: 696c 6c20 7573 6520 7468 6520 7661 6c75  ill use the valu
+00003df0: 6520 6f66 2074 6865 2065 6e76 6972 6f6e  e of the environ
+00003e00: 6d65 6e74 2076 6172 6961 626c 6520 6048  ment variable `H
+00003e10: 5454 5053 5f50 524f 5859 6020 6966 2072  TTPS_PROXY` if r
+00003e20: 6f75 7469 6e67 2074 6872 6f75 6768 2061  outing through a
+00003e30: 2070 726f 7879 2069 7320 7265 7175 6972   proxy is requir
+00003e40: 6564 2e0a 0a49 6e20 6164 6469 7469 6f6e  ed...In addition
+00003e50: 2c20 7468 6520 636f 6d6d 616e 6473 2063  , the commands c
+00003e60: 616e 2075 7365 2070 726f 7879 2061 7574  an use proxy aut
+00003e70: 6f63 6f6e 6669 6775 7261 7469 6f6e 2028  oconfiguration (
+00003e80: 5041 4329 2069 6620 7468 6520 602d 2d70  PAC) if the `--p
+00003e90: 6163 6020 636f 6d6d 616e 6420 6c69 6e65  ac` command line
+00003ea0: 206f 7074 696f 6e20 6973 2073 7065 6369   option is speci
+00003eb0: 6669 6564 2c20 6f72 2069 6620 7468 6520  fied, or if the 
+00003ec0: 6075 7365 5041 4360 2070 726f 7065 7274  `usePAC` propert
+00003ed0: 7920 6973 2073 6574 2074 6f20 6074 7275  y is set to `tru
+00003ee0: 6560 2069 6e20 7468 6520 605b 636f 6d6d  e` in the `[comm
+00003ef0: 6f6e 5d60 2073 6563 7469 6f6e 206f 6620  on]` section of 
+00003f00: 7468 6520 6063 6f6e 6669 672e 746f 6d6c  the `config.toml
+00003f10: 6020 6669 6c65 2e0a 0a23 2320 5370 6563  ` file...## Spec
+00003f20: 6966 7969 6e67 2043 6f6d 6d6f 6e20 5072  ifying Common Pr
+00003f30: 6f70 6572 7469 6573 2075 7369 6e67 2074  operties using t
+00003f40: 6865 2043 6f6d 6d61 6e64 204c 696e 6520  he Command Line 
+00003f50: 6f72 2045 6e76 6972 6f6e 6d65 6e74 2056  or Environment V
+00003f60: 6172 6961 626c 6573 0a0a 416c 6c20 7468  ariables..All th
+00003f70: 6520 636f 6d6d 6f6e 2070 726f 7065 7274  e common propert
+00003f80: 6965 7320 6361 6e20 6265 2073 6574 2075  ies can be set u
+00003f90: 7369 6e67 2063 6f6d 6d61 6e64 206c 696e  sing command lin
+00003fa0: 6520 6f70 7469 6f6e 732c 206f 7220 696e  e options, or in
+00003fb0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00003fc0: 6961 626c 6573 2e0a 0a54 6865 202a 2a63  iables...The **c
+00003fd0: 6f6d 6d61 6e64 206c 696e 6520 6f70 7469  ommand line opti
+00003fe0: 6f6e 732a 2a20 6172 6520 6173 2066 6f6c  ons** are as fol
+00003ff0: 6c6f 7773 3a0a 0a2d 2060 2d2d 6b65 7960  lows:..- `--key`
+00004000: 206f 7220 602d 6b60 0a2d 2060 2d2d 7365   or `-k`.- `--se
+00004010: 6372 6574 6020 6f72 2060 2d73 600a 2d20  cret` or `-s`.- 
+00004020: 602d 2d6e 616d 6573 7061 6365 6020 6f72  `--namespace` or
+00004030: 2060 2d6e 600a 2d20 602d 2d74 6167 6020   `-n`.- `--tag` 
+00004040: 6f72 2060 2d74 600a 2d20 602d 2d75 726c  or `-t`.- `--url
+00004050: 6020 6f72 2060 2d75 600a 2d20 602d 2d70  ` or `-u`.- `--p
+00004060: 6163 600a 0a54 6865 7365 206f 7074 696f  ac`..These optio
+00004070: 6e73 2063 616e 2061 6c73 6f20 6265 206c  ns can also be l
+00004080: 6973 7465 6420 6279 2072 756e 6e69 6e67  isted by running
+00004090: 2061 2063 6f6d 6d61 6e64 2077 6974 6820   a command with 
+000040a0: 7468 6520 602d 2d68 656c 7060 206f 7220  the `--help` or 
+000040b0: 602d 6860 206f 7074 696f 6e2e 0a0a 5468  `-h` option...Th
+000040c0: 6520 2a2a 656e 7669 726f 6e6d 656e 7420  e **environment 
+000040d0: 7661 7269 6162 6c65 732a 2a20 6172 6520  variables** are 
+000040e0: 6173 2066 6f6c 6c6f 7773 3a0a 0a2d 2060  as follows:..- `
+000040f0: 5944 5f4b 4559 600a 2d20 6059 445f 5345  YD_KEY`.- `YD_SE
+00004100: 4352 4554 600a 2d20 6059 445f 4e41 4d45  CRET`.- `YD_NAME
+00004110: 5350 4143 4560 0a2d 2060 5944 5f54 4147  SPACE`.- `YD_TAG
+00004120: 600a 2d20 6059 445f 5552 4c60 0a0a 5768  `.- `YD_URL`..Wh
+00004130: 656e 2073 6574 7469 6e67 2074 6865 2076  en setting the v
+00004140: 616c 7565 206f 6620 7468 6520 6162 6f76  alue of the abov
+00004150: 6520 7072 6f70 6572 7469 6573 2c20 6120  e properties, a 
+00004160: 7072 6f70 6572 7479 2073 6574 206f 6e20  property set on 
+00004170: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+00004180: 2074 616b 6573 2070 7265 6365 6465 6e63   takes precedenc
+00004190: 6520 6f76 6572 206f 6e65 2073 6574 2076  e over one set v
+000041a0: 6961 2061 6e20 656e 7669 726f 6e6d 656e  ia an environmen
+000041b0: 7420 7661 7269 6162 6c65 2c20 616e 6420  t variable, and 
+000041c0: 626f 7468 2074 616b 6520 7072 6563 6564  both take preced
+000041d0: 656e 6365 206f 7665 7220 6120 7661 6c75  ence over a valu
+000041e0: 6520 7365 7420 696e 2061 2063 6f6e 6669  e set in a confi
+000041f0: 6775 7261 7469 6f6e 2066 696c 652e 0a0a  guration file...
+00004200: 4966 2061 6c6c 2074 6865 2072 6571 7569  If all the requi
+00004210: 7265 6420 636f 6d6d 6f6e 2070 726f 7065  red common prope
+00004220: 7274 6965 7320 6172 6520 7365 7420 7573  rties are set us
+00004230: 696e 6720 7468 6520 636f 6d6d 616e 6420  ing the command 
+00004240: 6c69 6e65 206f 7220 656e 7669 726f 6e6d  line or environm
+00004250: 656e 7420 7661 7269 6162 6c65 732c 2074  ent variables, t
+00004260: 6865 6e20 7468 6520 656e 7469 7265 2060  hen the entire `
+00004270: 636f 6d6d 6f6e 6020 7365 6374 696f 6e20  common` section 
+00004280: 6f66 2074 6865 2054 4f4d 4c20 6669 6c65  of the TOML file
+00004290: 2063 616e 2062 6520 6f6d 6974 7465 642e   can be omitted.
+000042a0: 0a0a 2323 2056 6172 6961 626c 6520 5375  ..## Variable Su
+000042b0: 6273 7469 7475 7469 6f6e 7320 696e 2043  bstitutions in C
+000042c0: 6f6d 6d6f 6e20 5072 6f70 6572 7469 6573  ommon Properties
+000042d0: 0a0a 4e6f 7465 2074 6865 2075 7365 206f  ..Note the use o
+000042e0: 6620 607b 7b75 7365 726e 616d 657d 7d60  f `{{username}}`
+000042f0: 2069 6e20 7468 6520 7661 6c75 6520 6f66   in the value of
+00004300: 2074 6865 2060 7461 6760 2070 726f 7065   the `tag` prope
+00004310: 7274 793a 2074 6869 7320 6973 2061 202a  rty: this is a *
+00004320: 2a76 6172 6961 626c 6520 7375 6273 7469  *variable substi
+00004330: 7475 7469 6f6e 2a2a 2074 6861 7420 6361  tution** that ca
+00004340: 6e20 6f70 7469 6f6e 616c 6c79 2062 6520  n optionally be 
+00004350: 7573 6564 2074 6f20 696e 7365 7274 2074  used to insert t
+00004360: 6865 206c 6f67 696e 2075 7365 726e 616d  he login usernam
+00004370: 6520 6f66 2074 6865 2075 7365 7220 7275  e of the user ru
+00004380: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
+00004390: 6473 2e20 536f 2c20 666f 7220 7573 6572  ds. So, for user
+000043a0: 6e61 6d65 2060 6162 6360 2c20 7468 6520  name `abc`, the 
+000043b0: 6074 6167 6020 776f 756c 6420 6265 2073  `tag` would be s
+000043c0: 6574 2074 6f20 6074 6573 7469 6e67 2d61  et to `testing-a
+000043d0: 6263 602e 2054 6869 7320 6361 6e20 6265  bc`. This can be
+000043e0: 2068 656c 7066 756c 2074 6f20 6469 7361   helpful to disa
+000043f0: 6d62 6967 7561 7465 206d 756c 7469 706c  mbiguate multipl
+00004400: 6520 7573 6572 7320 7275 6e6e 696e 6720  e users running 
+00004410: 7769 7468 2074 6865 2073 616d 6520 636f  with the same co
+00004420: 6e66 6967 7572 6174 696f 6e20 6461 7461  nfiguration data
+00004430: 2e0a 0a56 6172 6961 626c 6520 7375 6273  ...Variable subs
+00004440: 7469 7475 7469 6f6e 7320 6172 6520 6469  titutions are di
+00004450: 7363 7573 7365 6420 6265 6c6f 772e 0a0a  scussed below...
+00004460: 2320 5661 7269 6162 6c65 2053 7562 7374  # Variable Subst
+00004470: 6974 7574 696f 6e73 0a0a 5661 7269 6162  itutions..Variab
+00004480: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
+00004490: 2070 726f 7669 6465 2061 2070 6f77 6572   provide a power
+000044a0: 6675 6c20 7761 7920 6f66 2069 6e74 726f  ful way of intro
+000044b0: 6475 6369 6e67 2076 6172 6961 626c 6520  ducing variable 
+000044c0: 7661 6c75 6573 2069 6e74 6f20 544f 4d4c  values into TOML
+000044d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+000044e0: 696c 6573 2c20 576f 726b 2052 6571 7569  iles, Work Requi
+000044f0: 7265 6d65 6e74 204a 534f 4e20 6465 6669  rement JSON defi
+00004500: 6e69 7469 6f6e 732c 2061 6e64 2057 6f72  nitions, and Wor
+00004510: 6b65 7220 506f 6f6c 204a 534f 4e20 6465  ker Pool JSON de
+00004520: 6669 6e69 7469 6f6e 732e 2054 6865 7920  finitions. They 
+00004530: 6361 6e20 6265 2069 6e63 6c75 6465 6420  can be included 
+00004540: 696e 2074 6865 2076 616c 7565 206f 6620  in the value of 
+00004550: 616e 7920 7072 6f70 6572 7479 2069 6e20  any property in 
+00004560: 6561 6368 206f 6620 7468 6573 6520 6f62  each of these ob
+00004570: 6a65 6374 732c 2069 6e63 6c75 6469 6e67  jects, including
+00004580: 2069 6e20 7661 6c75 6573 2077 6974 6869   in values withi
+00004590: 6e20 6c69 7374 7320 2865 2e67 2e2c 2066  n lists (e.g., f
+000045a0: 6f72 2074 6865 2060 6172 6775 6d65 6e74  or the `argument
+000045b0: 7360 2070 726f 7065 7274 7929 2061 6e64  s` property) and
+000045c0: 2061 7272 6179 7320 2865 2e67 2e2c 2074   arrays (e.g., t
+000045d0: 6865 2060 656e 7669 726f 6e6d 656e 7460  he `environment`
+000045e0: 2070 726f 7065 7274 7929 2e0a 0a56 6172   property)...Var
+000045f0: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00004600: 6f6e 7320 6172 6520 6578 7072 6573 7365  ons are expresse
+00004610: 6420 7573 696e 6720 607b 7b76 6172 6961  d using `{{varia
+00004620: 626c 657d 7d60 206e 6f74 6174 696f 6e2c  ble}}` notation,
+00004630: 2077 6865 7265 2074 6865 2065 7870 7265   where the expre
+00004640: 7373 696f 6e20 6973 2072 6570 6c61 6365  ssion is replace
+00004650: 6420 6279 2074 6865 2076 616c 7565 206f  d by the value o
+00004660: 6620 6076 6172 6961 626c 6560 2e0a 0a53  f `variable`...S
+00004670: 7562 7374 6974 7574 696f 6e73 2063 616e  ubstitutions can
+00004680: 2061 6c73 6f20 6265 2070 6572 666f 726d   also be perform
+00004690: 6564 2066 6f72 206e 6f6e 2d73 7472 696e  ed for non-strin
+000046a0: 6720 286e 756d 6265 7220 616e 6420 626f  g (number and bo
+000046b0: 6f6c 6561 6e29 2076 616c 7565 7320 7573  olean) values us
+000046c0: 696e 6720 7468 6520 606e 756d 3a60 2061  ing the `num:` a
+000046d0: 6e64 2060 626f 6f6c 3a60 2070 7265 6669  nd `bool:` prefi
+000046e0: 7865 7320 7769 7468 696e 2074 6865 2076  xes within the v
+000046f0: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
+00004700: 7469 6f6e 3a0a 0a2d 2044 6566 696e 6520  tion:..- Define 
+00004710: 7468 6520 7661 7269 6162 6c65 2073 7562  the variable sub
+00004720: 7374 6974 7574 696f 6e20 7573 696e 6720  stitution using 
+00004730: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
+00004740: 7769 6e67 2070 6174 7465 726e 733a 2060  wing patterns: `
+00004750: 227b 7b6e 756d 3a6d 795f 696e 747d 7d22  "{{num:my_int}}"
+00004760: 602c 2060 227b 7b6e 756d 3a6d 795f 666c  `, `"{{num:my_fl
+00004770: 6f61 747d 7d22 602c 2060 227b 7b62 6f6f  oat}}"`, `"{{boo
+00004780: 6c3a 6d79 5f62 6f6f 6c7d 7d22 600a 2d20  l:my_bool}}"`.- 
+00004790: 5661 7269 6162 6c65 2064 6566 696e 6974  Variable definit
+000047a0: 696f 6e73 2073 7570 706c 6965 6420 6f6e  ions supplied on
+000047b0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+000047c0: 6520 776f 756c 6420 7468 656e 2062 6520  e would then be 
+000047d0: 6f66 2074 6865 2066 6f72 6d3a 2060 2d6d  of the form: `-m
+000047e0: 206d 795f 696e 743d 3520 2d6d 206d 795f   my_int=5 -m my_
+000047f0: 666c 6f61 743d 322e 3520 2d6d 206d 795f  float=2.5 -m my_
+00004800: 626f 6f6c 3d74 7275 6560 0a2d 2049 6e20  bool=true`.- In 
+00004810: 7468 6520 7072 6f63 6573 7365 6420 4a53  the processed JS
+00004820: 4f4e 206f 7220 544f 4d4c 2c20 7468 6573  ON or TOML, thes
+00004830: 6520 7661 6c75 6573 2077 6f75 6c64 2062  e values would b
+00004840: 6563 6f6d 6520 6035 602c 2060 322e 3560  ecome `5`, `2.5`
+00004850: 2061 6e64 2060 7472 7565 602c 2072 6573   and `true`, res
+00004860: 7065 6374 6976 656c 792c 2063 6f6e 7665  pectively, conve
+00004870: 7274 6564 2066 726f 6d20 7374 7269 6e67  rted from string
+00004880: 7320 746f 2074 6865 6972 2063 6f72 7265  s to their corre
+00004890: 6374 204a 534f 4e20 7479 7065 730a 0a23  ct JSON types..#
+000048a0: 2320 4465 6661 756c 7420 5661 7269 6162  # Default Variab
+000048b0: 6c65 730a 0a54 6865 2066 6f6c 6c6f 7769  les..The followi
+000048c0: 6e67 2073 7562 7374 6974 7574 696f 6e73  ng substitutions
+000048d0: 2061 7265 2061 7574 6f6d 6174 6963 616c   are automatical
+000048e0: 6c79 2063 7265 6174 6564 2061 6e64 2063  ly created and c
+000048f0: 616e 2062 6520 7573 6564 2069 6e20 616e  an be used in an
+00004900: 7920 7365 6374 696f 6e20 6f66 2074 6865  y section of the
+00004910: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00004920: 696c 652c 206f 7220 696e 2061 6e79 204a  ile, or in any J
+00004930: 534f 4e20 7370 6563 6966 6963 6174 696f  SON specificatio
+00004940: 6e3a 0a0a 7c20 4469 7265 6374 6976 6520  n:..| Directive 
+00004950: 2020 2020 2020 7c20 4465 7363 7269 7074        | Descript
+00004960: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
+00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049a0: 207c 2045 7861 6d70 6c65 206f 6620 5375   | Example of Su
+000049b0: 6273 7469 7475 7469 6f6e 207c 0a7c 3a2d  bstitution |.|:-
+000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+000049d0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+000049e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a10: 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d  ----------|:----
+00004a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a30: 2d2d 2d2d 7c0a 7c20 607b 7b75 7365 726e  ----|.| `{{usern
+00004a40: 616d 657d 7d60 2020 7c20 5468 6520 6375  ame}}`  | The cu
+00004a50: 7272 656e 7420 7573 6572 2773 206c 6f67  rrent user's log
+00004a60: 696e 2075 7365 726e 616d 652c 206c 6f77  in username, low
+00004a70: 6572 2063 6173 652c 2073 7061 6365 7320  er case, spaces 
+00004a80: 7265 706c 6163 6564 2020 2020 2020 2020  replaced        
+00004a90: 2020 207c 206a 616e 655f 736d 6974 6820     | jane_smith 
+00004aa0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00004ab0: 2060 7b7b 6461 7465 7d7d 6020 2020 2020   `{{date}}`     
+00004ac0: 207c 2054 6865 2063 7572 7265 6e74 2064   | The current d
+00004ad0: 6174 6520 2855 5443 293a 2059 5959 594d  ate (UTC): YYYYM
+00004ae0: 4d44 4420 2020 2020 2020 2020 2020 2020  MDD             
+00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b00: 2020 2020 2020 2020 2020 2020 7c20 3230              | 20
+00004b10: 3232 3130 3237 2020 2020 2020 2020 2020  221027          
+00004b20: 2020 2020 2020 7c0a 7c20 607b 7b74 696d        |.| `{{tim
+00004b30: 657d 7d60 2020 2020 2020 7c20 5468 6520  e}}`      | The 
+00004b40: 6375 7272 656e 7420 7469 6d65 2028 5554  current time (UT
+00004b50: 4329 3a20 4848 4d4d 5353 2020 2020 2020  C): HHMMSS      
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b80: 2020 2020 207c 2031 3633 3032 3620 2020       | 163026   
+00004b90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004ba0: 0a7c 2060 7b7b 6461 7465 7469 6d65 7d7d  .| `{{datetime}}
+00004bb0: 6020 207c 2043 6f6e 6361 7465 6e61 7469  `  | Concatenati
+00004bc0: 6f6e 206f 6620 7468 6520 6461 7465 2061  on of the date a
+00004bd0: 6e64 2074 696d 6520 6162 6f76 652c 2077  nd time above, w
+00004be0: 6974 6820 6120 272d 2720 7365 7061 7261  ith a '-' separa
+00004bf0: 746f 7220 2020 2020 2020 2020 2020 7c20  tor           | 
+00004c00: 3230 3232 3130 3237 2d31 3633 3032 3620  20221027-163026 
+00004c10: 2020 2020 2020 2020 7c0a 7c20 607b 7b72          |.| `{{r
+00004c20: 616e 646f 6d7d 7d60 2020 2020 7c20 4120  andom}}`    | A 
+00004c30: 7261 6e64 6f6d 2c20 7468 7265 6520 6469  random, three di
+00004c40: 6769 7420 6865 7861 6465 6369 6d61 6c20  git hexadecimal 
+00004c50: 6e75 6d62 6572 2028 6c6f 7765 7220 6361  number (lower ca
+00004c60: 7365 2920 2020 2020 2020 2020 2020 2020  se)             
+00004c70: 2020 2020 2020 207c 2061 3163 2020 2020         | a1c    
+00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c90: 207c 0a7c 2060 7b7b 6e61 6d65 7370 6163   |.| `{{namespac
+00004ca0: 657d 7d60 207c 2054 6865 2060 6e61 6d65  e}}` | The `name
+00004cb0: 7370 6163 6560 2070 726f 7065 7274 792e  space` property.
+00004cc0: 204e 6f74 6520 7468 6174 2060 6e61 6d65   Note that `name
+00004cd0: 7370 6163 6560 206d 7573 742c 206f 6620  space` must, of 
+00004ce0: 636f 7572 7365 2c20 6265 2073 6574 2e20  course, be set. 
+00004cf0: 7c20 6d79 5f6e 616d 6573 7061 6365 2020  | my_namespace  
+00004d00: 2020 2020 2020 2020 2020 7c0a 7c20 607b            |.| `{
+00004d10: 7b74 6167 7d7d 6020 2020 2020 2020 7c20  {tag}}`       | 
+00004d20: 5468 6520 6074 6167 6020 7072 6f70 6572  The `tag` proper
+00004d30: 7479 2e20 4e6f 7465 2074 6861 7420 6074  ty. Note that `t
+00004d40: 6167 6020 6d75 7374 2062 6520 7365 742e  ag` must be set.
+00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d60: 2020 2020 2020 2020 207c 206d 795f 7461           | my_ta
+00004d70: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+00004d80: 2020 207c 0a7c 2060 7b7b 6b65 797d 7d60     |.| `{{key}}`
+00004d90: 2020 2020 2020 207c 2054 6865 2061 7070         | The app
+00004da0: 6c69 6361 7469 6f6e 2060 6b65 7960 2070  lication `key` p
+00004db0: 726f 7065 7274 792e 2020 2020 2020 2020  roperty.        
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00004df0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00004e00: 607b 7b73 6563 7265 747d 7d60 2020 2020  `{{secret}}`    
+00004e10: 7c20 5468 6520 6170 706c 6963 6174 696f  | The applicatio
+00004e20: 6e20 6073 6563 7265 7460 2070 726f 7065  n `secret` prope
+00004e30: 7274 792e 2020 2020 2020 2020 2020 2020  rty.            
+00004e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e50: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00004e80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00004e90: 0a0a 466f 7220 7468 6520 6064 6174 6560  ..For the `date`
-00004ea0: 2c20 6074 696d 6560 2c20 6064 6174 6574  , `time`, `datet
-00004eb0: 696d 6560 2061 6e64 2060 7261 6e64 6f6d  ime` and `random
-00004ec0: 6020 6469 7265 6374 6976 6573 2c20 7468  ` directives, th
-00004ed0: 6520 7361 6d65 2076 616c 7565 7320 7769  e same values wi
-00004ee0: 6c6c 2062 6520 7573 6564 2066 6f72 2074  ll be used for t
-00004ef0: 6865 2064 7572 6174 696f 6e20 6f66 2061  he duration of a
-00004f00: 2063 6f6d 6d61 6e64 202d 2d20 692e 652e   command -- i.e.
-00004f10: 2c20 6966 2060 7b7b 7469 6d65 7d7d 6020  , if `{{time}}` 
-00004f20: 6973 2075 7365 6420 7769 7468 696e 206d  is used within m
-00004f30: 756c 7469 706c 6520 7072 6f70 6572 7469  ultiple properti
-00004f40: 6573 2c20 7468 6520 7361 6d65 2076 616c  es, the same val
-00004f50: 7565 2077 696c 6c20 6265 2075 7365 6420  ue will be used 
-00004f60: 666f 7220 6561 6368 2073 7562 7374 6974  for each substit
-00004f70: 7574 696f 6e2e 0a0a 2323 2055 7365 722d  ution...## User-
-00004f80: 4465 6669 6e65 6420 5661 7269 6162 6c65  Defined Variable
-00004f90: 730a 0a41 7262 6974 7261 7279 2076 6172  s..Arbitrary var
-00004fa0: 6961 626c 6573 2063 616e 2062 6520 7375  iables can be su
-00004fb0: 7070 6c69 6564 2075 7369 6e67 2063 6f6d  pplied using com
-00004fc0: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
-00004fd0: 732c 2062 7920 7365 7474 696e 6720 656e  s, by setting en
-00004fe0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00004ff0: 6c65 7320 7072 6566 6978 6564 2077 6974  les prefixed wit
-00005000: 6820 6059 445f 5641 525f 602c 206f 7220  h `YD_VAR_`, or 
-00005010: 6279 2069 6e63 6c75 6469 6e67 2074 6865  by including the
-00005020: 2064 6972 6563 7469 7665 7320 696e 2074   directives in t
-00005030: 6865 2060 5b63 6f6d 6d6f 6e5d 6020 7365  he `[common]` se
-00005040: 6374 696f 6e20 6f66 2074 6865 2054 4f4d  ction of the TOM
-00005050: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
-00005060: 6669 6c65 2e0a 0a31 2e20 5468 6520 2a2a  file...1. The **
-00005070: 636f 6d6d 616e 6420 6c69 6e65 2a2a 206f  command line** o
-00005080: 7074 696f 6e20 6973 2060 2d2d 7661 7269  ption is `--vari
-00005090: 6162 6c65 6020 286f 7220 602d 7660 292e  able` (or `-v`).
-000050a0: 2046 6f72 2065 7861 6d70 6c65 2c20 6079   For example, `y
-000050b0: 642d 7375 626d 6974 202d 7620 7072 6f6a  d-submit -v proj
-000050c0: 6563 745f 636f 6465 3d70 722d 3231 332d  ect_code=pr-213-
-000050d0: 6120 2d76 2072 756e 5f69 643d 3132 3334  a -v run_id=1234
-000050e0: 6020 7769 6c6c 2065 7374 6162 6c69 7368  ` will establish
-000050f0: 2074 776f 206e 6577 2076 6172 6961 626c   two new variabl
-00005100: 6573 2074 6861 7420 6361 6e20 6265 2075  es that can be u
-00005110: 7365 6420 6173 2060 7b7b 7072 6f6a 6563  sed as `{{projec
-00005120: 745f 636f 6465 7d7d 6020 616e 6420 607b  t_code}}` and `{
-00005130: 7b72 756e 5f69 647d 7d60 2c20 7768 6963  {run_id}}`, whic
-00005140: 6820 7769 6c6c 2062 6520 7375 6273 7469  h will be substi
-00005150: 7475 7465 6420 6279 2060 7072 2d32 3133  tuted by `pr-213
-00005160: 2d61 6020 616e 6420 6031 3233 3460 2072  -a` and `1234` r
-00005170: 6573 7065 6374 6976 656c 792e 0a0a 0a32  espectively....2
-00005180: 2e20 466f 7220 2a2a 656e 7669 726f 6e6d  . For **environm
-00005190: 656e 7420 7661 7269 6162 6c65 732a 2a2c  ent variables**,
-000051a0: 2073 6574 7469 6e67 2074 6865 2076 6172   setting the var
-000051b0: 6961 626c 6520 6059 445f 5641 525f 7072  iable `YD_VAR_pr
-000051c0: 6f6a 6563 745f 636f 6465 3d22 7072 2d32  oject_code="pr-2
-000051d0: 3133 2d61 2260 2077 696c 6c20 6372 6561  13-a"` will crea
-000051e0: 7465 2061 206e 6577 2076 6172 6961 626c  te a new variabl
-000051f0: 6520 7468 6174 2063 616e 2062 6520 7573  e that can be us
-00005200: 6564 2061 7320 607b 7b70 726f 6a65 6374  ed as `{{project
-00005210: 5f63 6f64 657d 7d60 2c20 7768 6963 6820  _code}}`, which 
-00005220: 7769 6c6c 2062 6520 7375 6273 7469 7475  will be substitu
-00005230: 7465 6420 6279 2060 7072 2d32 3133 2d61  ted by `pr-213-a
-00005240: 602e 0a0a 0a33 2e20 466f 7220 2a2a 7365  `....3. For **se
-00005250: 7474 696e 6720 7769 7468 696e 2074 6865  tting within the
-00005260: 2054 4f4d 4c20 6669 6c65 2a2a 2c20 696e   TOML file**, in
-00005270: 636c 7564 6520 6120 2a2a 6076 6172 6961  clude a **`varia
-00005280: 626c 6573 602a 2a20 7461 626c 6520 696e  bles`** table in
-00005290: 2074 6865 2060 5b63 6f6d 6d6f 6e5d 6020   the `[common]` 
-000052a0: 7365 6374 696f 6e20 6f66 2074 6865 2066  section of the f
-000052b0: 696c 652e 2045 2e67 2e2c 2060 7661 7269  ile. E.g., `vari
-000052c0: 6162 6c65 7320 3d20 7b70 726f 6a65 6374  ables = {project
-000052d0: 5f63 6f64 6520 3d20 2270 722d 3231 3361  _code = "pr-213a
-000052e0: 222c 2072 756e 5f69 6420 3d20 2231 3233  ", run_id = "123
-000052f0: 3422 7d60 2e20 4e6f 7465 2074 6861 7420  4"}`. Note that 
-00005300: 7468 6973 2063 616e 2061 6c73 6f20 7573  this can also us
-00005310: 6520 7468 6520 666f 726d 3a0a 0a60 6060  e the form:..```
-00005320: 746f 6d6c 0a5b 636f 6d6d 6f6e 2e76 6172  toml.[common.var
-00005330: 6961 626c 6573 5d0a 7072 6f6a 6563 745f  iables].project_
-00005340: 636f 6465 203d 2022 7072 2d32 3133 6122  code = "pr-213a"
-00005350: 0a72 756e 5f69 6420 3d20 2231 3233 3422  .run_id = "1234"
-00005360: 0a60 6060 0a0a 4469 7265 6374 6976 6573  .```..Directives
-00005370: 2073 6574 206f 6e20 7468 6520 636f 6d6d   set on the comm
-00005380: 616e 6420 6c69 6e65 2074 616b 6520 7072  and line take pr
-00005390: 6563 6564 656e 6365 206f 7665 7220 6469  ecedence over di
-000053a0: 7265 6374 6976 6573 2073 6574 2069 6e20  rectives set in 
-000053b0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-000053c0: 6162 6c65 732c 2061 6e64 2062 6f74 6820  ables, and both 
-000053d0: 6f66 2074 6865 6d20 7461 6b65 2070 7265  of them take pre
-000053e0: 6365 6465 6e63 6520 6f76 6572 2064 6972  cedence over dir
-000053f0: 6563 7469 7665 7320 7365 7420 696e 2061  ectives set in a
-00005400: 2054 4f4d 4c20 6669 6c65 2e0a 0a54 6869   TOML file...Thi
-00005410: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
-00005420: 7573 6564 2074 6f20 6f76 6572 7269 6465  used to override
-00005430: 2074 6865 2064 6566 6175 6c74 2064 6972   the default dir
-00005440: 6563 7469 7665 732c 2065 2e67 2e2c 2073  ectives, e.g., s
-00005450: 6574 7469 6e67 2060 2d76 2075 7365 726e  etting `-v usern
-00005460: 616d 653d 226f 7468 6572 2d75 7365 7222  ame="other-user"
-00005470: 6020 7769 6c6c 206f 7665 7272 6964 6520  ` will override 
-00005480: 7468 6520 6465 6661 756c 7420 607b 7b75  the default `{{u
-00005490: 7365 726e 616d 657d 7d60 2064 6972 6563  sername}}` direc
-000054a0: 7469 7665 2e0a 0a23 2320 4e65 7374 6564  tive...## Nested
-000054b0: 2056 6172 6961 626c 6573 0a0a 496e 2074   Variables..In t
-000054c0: 6865 2063 6173 6520 6f66 202a 2a54 4f4d  he case of **TOM
-000054d0: 4c20 7072 6f70 6572 7469 6573 206f 6e6c  L properties onl
-000054e0: 792a 2a2c 2076 6172 6961 626c 6520 7375  y**, variable su
-000054f0: 6273 7469 7475 7469 6f6e 7320 6361 6e20  bstitutions can 
-00005500: 6265 206e 6573 7465 642e 0a0a 466f 7220  be nested...For 
-00005510: 6578 616d 706c 652c 2069 6620 6f6e 6520  example, if one 
-00005520: 7761 6e74 6564 2074 6f20 7365 6c65 6374  wanted to select
-00005530: 2061 2064 6966 6665 7265 6e74 2060 7465   a different `te
-00005540: 6d70 6c61 7465 4964 6020 666f 7220 6120  mplateId` for a 
-00005550: 576f 726b 6572 2050 6f6f 6c20 6465 7065  Worker Pool depe
-00005560: 6e64 696e 6720 6f6e 2074 6865 2076 616c  nding on the val
-00005570: 7565 206f 6620 6120 6072 6567 696f 6e60  ue of a `region`
-00005580: 2076 6172 6961 626c 652c 206f 6e65 2063   variable, one c
-00005590: 6f75 6c64 2075 7365 2074 6865 2066 6f6c  ould use the fol
-000055a0: 6c6f 7769 6e67 3a0a 0a60 6060 746f 6d6c  lowing:..```toml
-000055b0: 0a5b 636f 6d6d 6f6e 2e76 6172 6961 626c  .[common.variabl
-000055c0: 6573 5d0a 2020 2020 7465 6d70 6c61 7465  es].    template
-000055d0: 5f6c 6f6e 646f 6e20 3d20 2279 6469 643a  _london = "ydid:
-000055e0: 6372 743a 3635 4546 3446 3a61 3464 3735  crt:65EF4F:a4d75
-000055f0: 3763 662d 6236 3761 2d34 6562 362d 6264  7cf-b67a-4eb6-bd
-00005600: 3339 2d38 6136 6666 6434 3663 3866 3422  39-8a6ffd46c8f4"
-00005610: 0a20 2020 2074 656d 706c 6174 655f 7068  .    template_ph
-00005620: 6f65 6e69 7820 3d20 2279 6469 643a 6372  oenix = "ydid:cr
-00005630: 743a 3635 4546 3446 3a65 3432 3339 6465  t:65EF4F:e4239de
-00005640: 632d 3738 6332 2d34 3231 632d 6137 6633  c-78c2-421c-a7f3
-00005650: 2d37 3165 3631 6237 3239 3436 6622 0a20  -71e61b72946f". 
-00005660: 2020 2074 656d 706c 6174 655f 6672 616e     template_fran
-00005670: 6b66 7572 7420 3d20 2279 6469 643a 6372  kfurt = "ydid:cr
-00005680: 743a 3635 4546 3446 3a33 3239 3630 3263  t:65EF4F:329602c
-00005690: 662d 3539 3435 2d34 6161 642d 6132 3838  f-5945-4aad-a288
-000056a0: 2d65 6134 3234 6436 3464 3535 6522 0a0a  -ea424d64d55e"..
-000056b0: 5b63 6f6d 6d6f 6e2e 776f 726b 6572 506f  [common.workerPo
-000056c0: 6f6c 5d0a 2020 2020 7465 6d70 6c61 7465  ol].    template
-000056d0: 4964 203d 2022 7b7b 7465 6d70 6c61 7465  Id = "{{template
-000056e0: 5f7b 7b72 6567 696f 6e7d 7d7d 7d22 0a60  _{{region}}}}".`
-000056f0: 6060 0a0a 5468 656e 2c20 6966 206f 6e65  ``..Then, if one
-00005700: 2075 7365 6420 6079 642d 7072 6f76 6973   used `yd-provis
-00005710: 696f 6e20 2d76 2072 6567 696f 6e3d 7068  ion -v region=ph
-00005720: 6f65 6e69 7860 2c20 7468 6520 6074 656d  oenix`, the `tem
-00005730: 706c 6174 6549 6460 2070 726f 7065 7274  plateId` propert
-00005740: 7920 776f 756c 6420 6669 7273 7420 7265  y would first re
-00005750: 736f 6c76 6520 746f 2060 227b 7b74 656d  solve to `"{{tem
-00005760: 706c 6174 655f 7068 656f 6e69 787d 7d22  plate_pheonix}}"
-00005770: 602c 2061 6e64 2074 6865 6e20 746f 2060  `, and then to `
-00005780: 2279 6469 643a 6372 743a 3635 4546 3446  "ydid:crt:65EF4F
-00005790: 3a65 3432 3339 6465 632d 3738 6332 2d34  :e4239dec-78c2-4
-000057a0: 3231 632d 6137 6633 2d37 3165 3631 6237  21c-a7f3-71e61b7
-000057b0: 3239 3436 6622 602e 0a0a 4e65 7374 696e  2946f"`...Nestin
-000057c0: 6720 6361 6e20 6265 2075 7020 746f 2074  g can be up to t
-000057d0: 6872 6565 206c 6576 656c 7320 6465 6570  hree levels deep
-000057e0: 2069 6e63 6c75 6469 6e67 2074 6865 2074   including the t
-000057f0: 6f70 206c 6576 656c 2e0a 0a23 2057 6f72  op level...# Wor
-00005800: 6b20 5265 7175 6972 656d 656e 7420 5072  k Requirement Pr
-00005810: 6f70 6572 7469 6573 0a0a 5468 6520 6077  operties..The `w
-00005820: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
-00005830: 7365 6374 696f 6e20 6f66 2074 6865 2063  section of the c
-00005840: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00005850: 6520 6973 206f 7074 696f 6e61 6c2e 2049  e is optional. I
-00005860: 7427 7320 7573 6564 206f 6e6c 7920 6279  t's used only by
-00005870: 2074 6865 2060 7964 2d73 7562 6d69 7460   the `yd-submit`
-00005880: 2063 6f6d 6d61 6e64 2c20 616e 6420 636f   command, and co
-00005890: 6e74 726f 6c73 2074 6865 2057 6f72 6b20  ntrols the Work 
-000058a0: 5265 7175 6972 656d 656e 7420 7468 6174  Requirement that
-000058b0: 2069 7320 7375 626d 6974 7465 6420 746f   is submitted to
-000058c0: 2074 6865 2050 6c61 7466 6f72 6d2e 0a0a   the Platform...
-000058d0: 5468 6520 6465 7461 696c 7320 6f66 2061  The details of a
-000058e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-000058f0: 7420 746f 2062 6520 7375 626d 6974 7465  t to be submitte
-00005900: 6420 6361 6e20 6265 2063 6170 7475 7265  d can be capture
-00005910: 6420 656e 7469 7265 6c79 2077 6974 6869  d entirely withi
-00005920: 6e20 7468 6520 544f 4d4c 2063 6f6e 6669  n the TOML confi
-00005930: 6775 7261 7469 6f6e 2066 696c 6520 666f  guration file fo
-00005940: 7220 7369 6d70 6c65 2065 7861 6d70 6c65  r simple example
-00005950: 732e 204d 6f72 6520 636f 6d70 6c65 7820  s. More complex 
-00005960: 6578 616d 706c 6573 2063 6170 7475 7265  examples capture
-00005970: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-00005980: 656d 656e 7420 696e 2061 2063 6f6d 6269  ement in a combi
-00005990: 6e61 7469 6f6e 206f 6620 7468 6520 544f  nation of the TO
-000059a0: 4d4c 2066 696c 6520 706c 7573 2061 204a  ML file plus a J
-000059b0: 534f 4e20 646f 6375 6d65 6e74 2c20 6f72  SON document, or
-000059c0: 2069 6e20 6120 4a53 4f4e 2064 6f63 756d   in a JSON docum
-000059d0: 656e 7420 6f6e 6c79 2e0a 0a23 2320 576f  ent only...## Wo
-000059e0: 726b 2052 6571 7569 7265 6d65 6e74 204a  rk Requirement J
-000059f0: 534f 4e20 4669 6c65 2053 7472 7563 7475  SON File Structu
-00005a00: 7265 0a0a 576f 726b 2052 6571 7569 7265  re..Work Require
-00005a10: 6d65 6e74 7320 6172 6520 7265 7072 6573  ments are repres
-00005a20: 656e 7465 6420 696e 204a 534f 4e20 646f  ented in JSON do
-00005a30: 6375 6d65 6e74 7320 7573 696e 6720 6120  cuments using a 
-00005a40: 636f 6e74 6169 6e6d 656e 7420 6869 6572  containment hier
-00005a50: 6172 6368 7920 6f66 2061 202a 2a57 6f72  archy of a **Wor
-00005a60: 6b20 5265 7175 6972 656d 656e 742a 2a20  k Requirement** 
-00005a70: 636f 6e74 6169 6e69 6e67 2061 202a 2a6c  containing a **l
-00005a80: 6973 7420 6f66 2054 6173 6b20 4772 6f75  ist of Task Grou
-00005a90: 7073 2a2a 2c20 636f 6e74 6169 6e69 6e67  ps**, containing
-00005aa0: 2061 202a 2a6c 6973 7420 6f66 2054 6173   a **list of Tas
-00005ab0: 6b73 2a2a 2e0a 0a41 2076 6572 7920 7369  ks**...A very si
-00005ac0: 6d70 6c65 2065 7861 6d70 6c65 2064 6f63  mple example doc
-00005ad0: 756d 656e 7420 6973 2073 686f 776e 2062  ument is shown b
-00005ae0: 656c 6f77 2077 6974 6820 6120 746f 702d  elow with a top-
-00005af0: 6c65 7665 6c20 576f 726b 2052 6571 7569  level Work Requi
-00005b00: 7265 6d65 6e74 2063 6f6e 7461 696e 696e  rement containin
-00005b10: 6720 7477 6f20 5461 736b 2047 726f 7570  g two Task Group
-00005b20: 7320 6561 6368 2063 6f6e 7461 696e 696e  s each containin
-00005b30: 6720 7477 6f20 5461 736b 732c 2065 6163  g two Tasks, eac
-00005b40: 6820 7769 7468 2061 2064 6966 6665 7265  h with a differe
-00005b50: 6e74 2073 6574 206f 6620 6172 6775 6d65  nt set of argume
-00005b60: 6e74 7320 746f 2062 6520 7061 7373 6564  nts to be passed
-00005b70: 2074 6f20 7468 6520 5461 736b 2e0a 0a60   to the Task...`
-00005b80: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
-00005b90: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
-00005ba0: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-00005bb0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-00005bc0: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
-00005bd0: 223a 205b 312c 2032 2c20 335d 0a20 2020  ": [1, 2, 3].   
-00005be0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00005bf0: 7b0a 2020 2020 2020 2020 2020 2261 7267  {.          "arg
-00005c00: 756d 656e 7473 223a 205b 342c 2035 2c20  uments": [4, 5, 
-00005c10: 365d 0a20 2020 2020 2020 207d 0a20 2020  6].        }.   
-00005c20: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
-00005c30: 7b0a 2020 2020 2020 2274 6173 6b73 223a  {.      "tasks":
-00005c40: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
-00005c50: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
-00005c60: 7322 3a20 5b37 2c20 382c 2039 5d0a 2020  s": [7, 8, 9].  
-00005c70: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00005c80: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-00005c90: 6775 6d65 6e74 7322 3a20 5b31 302c 2031  guments": [10, 1
-00005ca0: 312c 2031 325d 0a20 2020 2020 2020 207d  1, 12].        }
-00005cb0: 0a20 2020 2020 205d 0a20 2020 207d 0a20  .      ].    }. 
-00005cc0: 205d 0a7d 0a0a 6060 600a 0a54 6f20 7370   ].}..```..To sp
-00005cd0: 6563 6966 7920 7468 6520 6669 6c65 2063  ecify the file c
-00005ce0: 6f6e 7461 696e 696e 6720 7468 6520 4a53  ontaining the JS
-00005cf0: 4f4e 2064 6f63 756d 656e 742c 2065 6974  ON document, eit
-00005d00: 6865 7220 706f 7075 6c61 7465 2074 6865  her populate the
-00005d10: 2060 776f 726b 5265 7175 6972 656d 656e   `workRequiremen
-00005d20: 7444 6174 6160 2070 726f 7065 7274 7920  tData` property 
-00005d30: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
-00005d40: 6972 656d 656e 7460 2073 6563 7469 6f6e  irement` section
-00005d50: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
-00005d60: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00005d70: 7769 7468 2074 6865 204a 534f 4e20 6669  with the JSON fi
-00005d80: 6c65 6e61 6d65 2c20 6f72 2073 7065 6369  lename, or speci
-00005d90: 6679 2069 7420 6f6e 2074 6865 2063 6f6d  fy it on the com
-00005da0: 6d61 6e64 206c 696e 6520 7573 696e 6720  mand line using 
-00005db0: 7468 6520 602d 2d77 6f72 6b2d 7265 7175  the `--work-requ
-00005dc0: 6972 656d 656e 7460 206f 7220 602d 7260  irement` or `-r`
-00005dd0: 206f 7074 696f 6e73 2028 7768 6963 6820   options (which 
-00005de0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
-00005df0: 6520 7072 6f70 6572 7479 2069 6e20 7468  e property in th
-00005e00: 6520 544f 4d4c 2066 696c 6529 2c20 652e  e TOML file), e.
-00005e10: 672e 0a0a 6079 642d 7375 626d 6974 202d  g...`yd-submit -
-00005e20: 2d63 6f6e 6669 6720 6d79 636f 6e66 6967  -config myconfig
-00005e30: 2e74 6f6d 6c20 2d2d 776f 726b 2d72 6571  .toml --work-req
-00005e40: 7569 7265 6d65 6e74 206d 795f 776f 726b  uirement my_work
-00005e50: 7265 712e 6a73 6f6e 600a 0a23 2320 5072  req.json`..## Pr
-00005e60: 6f70 6572 7479 2049 6e68 6572 6974 616e  operty Inheritan
-00005e70: 6365 0a0a 546f 2073 696d 706c 6966 7920  ce..To simplify 
-00005e80: 7468 6520 6465 6669 6e69 7469 6f6e 206f  the definition o
-00005e90: 6620 576f 726b 2052 6571 7569 7265 6d65  f Work Requireme
-00005ea0: 6e74 732c 2074 6865 7265 2069 7320 6120  nts, there is a 
-00005eb0: 7072 6f70 6572 7479 2069 6e68 6572 6974  property inherit
-00005ec0: 616e 6365 206d 6563 6861 6e69 736d 2e20  ance mechanism. 
-00005ed0: 5072 6f70 6572 7469 6573 2074 6861 7420  Properties that 
-00005ee0: 6172 6520 7365 7420 6174 2061 2068 6967  are set at a hig
-00005ef0: 6865 7220 6c65 7665 6c20 696e 2074 6865  her level in the
-00005f00: 2068 6965 7261 7263 6879 2061 7265 2069   hierarchy are i
-00005f10: 6e68 6572 6974 6564 2061 7420 6c6f 7765  nherited at lowe
-00005f20: 7220 6c65 7665 6c73 2c20 756e 6c65 7373  r levels, unless
-00005f30: 2065 7870 6c69 6369 746c 7920 6f76 6572   explicitly over
-00005f40: 7269 6464 656e 2e0a 0a54 6869 7320 6d65  ridden...This me
-00005f50: 616e 7320 7468 6174 2061 2070 726f 7065  ans that a prope
-00005f60: 7274 7920 7365 7420 696e 2074 6865 2060  rty set in the `
-00005f70: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
-00005f80: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-00005f90: 544f 4d4c 2066 696c 6520 6361 6e20 6265  TOML file can be
-00005fa0: 2069 6e68 6572 6974 6564 2073 7563 6365   inherited succe
-00005fb0: 7373 6976 656c 7920 6279 2074 6865 2057  ssively by the W
-00005fc0: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
-00005fd0: 2054 6173 6b20 4772 6f75 7073 2061 6e64   Task Groups and
-00005fe0: 2054 6173 6b73 2069 6e20 7468 6520 4a53   Tasks in the JS
-00005ff0: 4f4e 2064 6f63 756d 656e 7420 2861 7373  ON document (ass
-00006000: 756d 696e 6720 7468 6520 7072 6f70 6572  uming the proper
-00006010: 7479 2069 7320 7661 6c69 6420 6174 2065  ty is valid at e
-00006020: 6163 6820 6c65 7665 6c29 2e20 2048 656e  ach level).  Hen
-00006030: 6365 2c20 5461 736b 7320 696e 6865 7269  ce, Tasks inheri
-00006040: 7420 6672 6f6d 2054 6173 6b20 4772 6f75  t from Task Grou
-00006050: 7073 2c20 7768 6963 6820 696e 6865 7269  ps, which inheri
-00006060: 7420 6672 6f6d 2074 6865 2057 6f72 6b20  t from the Work 
-00006070: 5265 7175 6972 656d 656e 7420 696e 2074  Requirement in t
-00006080: 6865 204a 534f 4e20 646f 6375 6d65 6e74  he JSON document
-00006090: 2c20 7768 6963 6820 696e 6865 7269 7473  , which inherits
-000060a0: 2066 726f 6d20 7468 6520 6077 6f72 6b52   from the `workR
-000060b0: 6571 7569 7265 6d65 6e74 6020 7072 6f70  equirement` prop
-000060c0: 6572 7469 6573 2069 6e20 7468 6520 544f  erties in the TO
-000060d0: 4d4c 2066 696c 652e 0a0a 4f76 6572 7269  ML file...Overri
-000060e0: 6464 656e 2070 726f 7065 7274 6965 7320  dden properties 
-000060f0: 6172 6520 616c 736f 2069 6e68 6572 6974  are also inherit
-00006100: 6564 2e20 452e 672e 2c20 6966 2061 2070  ed. E.g., if a p
-00006110: 726f 7065 7274 7920 6973 2073 6574 2061  roperty is set a
-00006120: 7420 7468 6520 5461 736b 2047 726f 7570  t the Task Group
-00006130: 206c 6576 656c 2c20 6974 2077 696c 6c20   level, it will 
-00006140: 6265 2069 6e68 6572 6974 6564 2062 7920  be inherited by 
-00006150: 7468 6520 5461 736b 7320 696e 2074 6861  the Tasks in tha
-00006160: 7420 5461 736b 2047 726f 7570 2075 6e6c  t Task Group unl
-00006170: 6573 7320 6578 706c 6963 6974 6c79 206f  ess explicitly o
-00006180: 7665 7272 6964 6465 6e2e 0a0a 2323 2057  verridden...## W
-00006190: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-000061a0: 5072 6f70 6572 7479 2044 6963 7469 6f6e  Property Diction
-000061b0: 6172 790a 0a54 6865 2066 6f6c 6c6f 7769  ary..The followi
-000061c0: 6e67 2074 6162 6c65 206f 7574 6c69 6e65  ng table outline
-000061d0: 7320 616c 6c20 7468 6520 7072 6f70 6572  s all the proper
-000061e0: 7469 6573 2061 7661 696c 6162 6c65 2066  ties available f
-000061f0: 6f72 2064 6566 696e 696e 6720 576f 726b  or defining Work
-00006200: 2052 6571 7569 7265 6d65 6e74 732c 2061   Requirements, a
-00006210: 6e64 2074 6865 206c 6576 656c 7320 6174  nd the levels at
-00006220: 2077 6869 6368 2074 6865 7920 6172 6520   which they are 
-00006230: 616c 6c6f 7765 6420 746f 2062 6520 7573  allowed to be us
-00006240: 6564 2e20 536f 2c20 666f 7220 6578 616d  ed. So, for exam
-00006250: 706c 652c 2074 6865 2060 7072 6f76 6964  ple, the `provid
-00006260: 6572 6020 7072 6f70 6572 7479 2063 616e  er` property can
-00006270: 2062 6520 7365 7420 696e 2074 6865 2054   be set in the T
-00006280: 4f4d 4c20 6669 6c65 2c20 6174 2074 6865  OML file, at the
-00006290: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-000062a0: 7420 4c65 7665 6c20 6f72 2061 7420 7468  t Level or at th
-000062b0: 6520 5461 736b 2047 726f 7570 204c 6576  e Task Group Lev
-000062c0: 656c 2c20 6275 7420 6e6f 7420 6174 2074  el, but not at t
-000062d0: 6865 2054 6173 6b20 6c65 7665 6c2c 2061  he Task level, a
-000062e0: 6e64 2070 726f 7065 7274 7920 6064 6570  nd property `dep
-000062f0: 656e 6465 6e74 4f6e 6020 6361 6e20 6f6e  endentOn` can on
-00006300: 6c79 2062 6520 7365 7420 6174 2074 6865  ly be set at the
-00006310: 2054 6173 6b20 4772 6f75 7020 6c65 7665   Task Group leve
-00006320: 6c2e 0a0a 416c 6c20 7072 6f70 6572 7469  l...All properti
-00006330: 6573 2061 7265 206f 7074 696f 6e61 6c20  es are optional 
-00006340: 6578 6365 7074 2066 6f72 202a 2a60 7461  except for **`ta
-00006350: 736b 5479 7065 602a 2a20 286f 7220 2a2a  skType`** (or **
-00006360: 6074 6173 6b54 7970 6573 602a 2a29 2e0a  `taskTypes`**)..
-00006370: 0a7c 2050 726f 7065 7274 7920 4e61 6d65  .| Property Name
-00006380: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00006390: 4465 7363 7269 7074 696f 6e20 2020 2020  Description     
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 207c 0a7c 2060 7b7b 7572 6c7d       |.| `{{url}
+00004e80: 7d60 2020 2020 2020 207c 2054 6865 2050  }`       | The P
+00004e90: 6c61 7466 6f72 6d20 6075 726c 6020 7072  latform `url` pr
+00004ea0: 6f70 6572 7479 2e20 2020 2020 2020 2020  operty.         
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ed0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00004ef0: 0a46 6f72 2074 6865 2060 6461 7465 602c  .For the `date`,
+00004f00: 2060 7469 6d65 602c 2060 6461 7465 7469   `time`, `dateti
+00004f10: 6d65 6020 616e 6420 6072 616e 646f 6d60  me` and `random`
+00004f20: 2064 6972 6563 7469 7665 732c 2074 6865   directives, the
+00004f30: 2073 616d 6520 7661 6c75 6573 2077 696c   same values wil
+00004f40: 6c20 6265 2075 7365 6420 666f 7220 7468  l be used for th
+00004f50: 6520 6475 7261 7469 6f6e 206f 6620 6120  e duration of a 
+00004f60: 636f 6d6d 616e 6420 2d2d 2069 2e65 2e2c  command -- i.e.,
+00004f70: 2069 6620 607b 7b74 696d 657d 7d60 2069   if `{{time}}` i
+00004f80: 7320 7573 6564 2077 6974 6869 6e20 6d75  s used within mu
+00004f90: 6c74 6970 6c65 2070 726f 7065 7274 6965  ltiple propertie
+00004fa0: 732c 2074 6865 2073 616d 6520 7661 6c75  s, the same valu
+00004fb0: 6520 7769 6c6c 2062 6520 7573 6564 2066  e will be used f
+00004fc0: 6f72 2065 6163 6820 7375 6273 7469 7475  or each substitu
+00004fd0: 7469 6f6e 2e0a 0a23 2320 5573 6572 2d44  tion...## User-D
+00004fe0: 6566 696e 6564 2056 6172 6961 626c 6573  efined Variables
+00004ff0: 0a0a 4172 6269 7472 6172 7920 7661 7269  ..Arbitrary vari
+00005000: 6162 6c65 7320 6361 6e20 6265 2073 7570  ables can be sup
+00005010: 706c 6965 6420 7573 696e 6720 636f 6d6d  plied using comm
+00005020: 616e 6420 6c69 6e65 206f 7074 696f 6e73  and line options
+00005030: 2c20 6279 2073 6574 7469 6e67 2065 6e76  , by setting env
+00005040: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00005050: 6573 2070 7265 6669 7865 6420 7769 7468  es prefixed with
+00005060: 2060 5944 5f56 4152 5f60 2c20 6f72 2062   `YD_VAR_`, or b
+00005070: 7920 696e 636c 7564 696e 6720 7468 6520  y including the 
+00005080: 6469 7265 6374 6976 6573 2069 6e20 7468  directives in th
+00005090: 6520 605b 636f 6d6d 6f6e 5d60 2073 6563  e `[common]` sec
+000050a0: 7469 6f6e 206f 6620 7468 6520 544f 4d4c  tion of the TOML
+000050b0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+000050c0: 696c 652e 0a0a 312e 2054 6865 202a 2a63  ile...1. The **c
+000050d0: 6f6d 6d61 6e64 206c 696e 652a 2a20 6f70  ommand line** op
+000050e0: 7469 6f6e 2069 7320 602d 2d76 6172 6961  tion is `--varia
+000050f0: 626c 6560 2028 6f72 2060 2d76 6029 2e20  ble` (or `-v`). 
+00005100: 466f 7220 6578 616d 706c 652c 2060 7964  For example, `yd
+00005110: 2d73 7562 6d69 7420 2d76 2070 726f 6a65  -submit -v proje
+00005120: 6374 5f63 6f64 653d 7072 2d32 3133 2d61  ct_code=pr-213-a
+00005130: 202d 7620 7275 6e5f 6964 3d31 3233 3460   -v run_id=1234`
+00005140: 2077 696c 6c20 6573 7461 626c 6973 6820   will establish 
+00005150: 7477 6f20 6e65 7720 7661 7269 6162 6c65  two new variable
+00005160: 7320 7468 6174 2063 616e 2062 6520 7573  s that can be us
+00005170: 6564 2061 7320 607b 7b70 726f 6a65 6374  ed as `{{project
+00005180: 5f63 6f64 657d 7d60 2061 6e64 2060 7b7b  _code}}` and `{{
+00005190: 7275 6e5f 6964 7d7d 602c 2077 6869 6368  run_id}}`, which
+000051a0: 2077 696c 6c20 6265 2073 7562 7374 6974   will be substit
+000051b0: 7574 6564 2062 7920 6070 722d 3231 332d  uted by `pr-213-
+000051c0: 6160 2061 6e64 2060 3132 3334 6020 7265  a` and `1234` re
+000051d0: 7370 6563 7469 7665 6c79 2e0a 0a0a 322e  spectively....2.
+000051e0: 2046 6f72 202a 2a65 6e76 6972 6f6e 6d65   For **environme
+000051f0: 6e74 2076 6172 6961 626c 6573 2a2a 2c20  nt variables**, 
+00005200: 7365 7474 696e 6720 7468 6520 7661 7269  setting the vari
+00005210: 6162 6c65 2060 5944 5f56 4152 5f70 726f  able `YD_VAR_pro
+00005220: 6a65 6374 5f63 6f64 653d 2270 722d 3231  ject_code="pr-21
+00005230: 332d 6122 6020 7769 6c6c 2063 7265 6174  3-a"` will creat
+00005240: 6520 6120 6e65 7720 7661 7269 6162 6c65  e a new variable
+00005250: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+00005260: 6420 6173 2060 7b7b 7072 6f6a 6563 745f  d as `{{project_
+00005270: 636f 6465 7d7d 602c 2077 6869 6368 2077  code}}`, which w
+00005280: 696c 6c20 6265 2073 7562 7374 6974 7574  ill be substitut
+00005290: 6564 2062 7920 6070 722d 3231 332d 6160  ed by `pr-213-a`
+000052a0: 2e0a 0a0a 332e 2046 6f72 202a 2a73 6574  ....3. For **set
+000052b0: 7469 6e67 2077 6974 6869 6e20 7468 6520  ting within the 
+000052c0: 544f 4d4c 2066 696c 652a 2a2c 2069 6e63  TOML file**, inc
+000052d0: 6c75 6465 2061 202a 2a60 7661 7269 6162  lude a **`variab
+000052e0: 6c65 7360 2a2a 2074 6162 6c65 2069 6e20  les`** table in 
+000052f0: 7468 6520 605b 636f 6d6d 6f6e 5d60 2073  the `[common]` s
+00005300: 6563 7469 6f6e 206f 6620 7468 6520 6669  ection of the fi
+00005310: 6c65 2e20 452e 672e 2c20 6076 6172 6961  le. E.g., `varia
+00005320: 626c 6573 203d 207b 7072 6f6a 6563 745f  bles = {project_
+00005330: 636f 6465 203d 2022 7072 2d32 3133 6122  code = "pr-213a"
+00005340: 2c20 7275 6e5f 6964 203d 2022 3132 3334  , run_id = "1234
+00005350: 227d 602e 204e 6f74 6520 7468 6174 2074  "}`. Note that t
+00005360: 6869 7320 6361 6e20 616c 736f 2075 7365  his can also use
+00005370: 2074 6865 2066 6f72 6d3a 0a0a 6060 6074   the form:..```t
+00005380: 6f6d 6c0a 5b63 6f6d 6d6f 6e2e 7661 7269  oml.[common.vari
+00005390: 6162 6c65 735d 0a70 726f 6a65 6374 5f63  ables].project_c
+000053a0: 6f64 6520 3d20 2270 722d 3231 3361 220a  ode = "pr-213a".
+000053b0: 7275 6e5f 6964 203d 2022 3132 3334 220a  run_id = "1234".
+000053c0: 6060 600a 0a44 6972 6563 7469 7665 7320  ```..Directives 
+000053d0: 7365 7420 6f6e 2074 6865 2063 6f6d 6d61  set on the comma
+000053e0: 6e64 206c 696e 6520 7461 6b65 2070 7265  nd line take pre
+000053f0: 6365 6465 6e63 6520 6f76 6572 2064 6972  cedence over dir
+00005400: 6563 7469 7665 7320 7365 7420 696e 2065  ectives set in e
+00005410: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00005420: 626c 6573 2c20 616e 6420 626f 7468 206f  bles, and both o
+00005430: 6620 7468 656d 2074 616b 6520 7072 6563  f them take prec
+00005440: 6564 656e 6365 206f 7665 7220 6469 7265  edence over dire
+00005450: 6374 6976 6573 2073 6574 2069 6e20 6120  ctives set in a 
+00005460: 544f 4d4c 2066 696c 652e 0a0a 5468 6973  TOML file...This
+00005470: 206d 6574 686f 6420 6361 6e20 6265 2075   method can be u
+00005480: 7365 6420 746f 206f 7665 7272 6964 6520  sed to override 
+00005490: 7468 6520 6465 6661 756c 7420 6469 7265  the default dire
+000054a0: 6374 6976 6573 2c20 652e 672e 2c20 7365  ctives, e.g., se
+000054b0: 7474 696e 6720 602d 7620 7573 6572 6e61  tting `-v userna
+000054c0: 6d65 3d22 6f74 6865 722d 7573 6572 2260  me="other-user"`
+000054d0: 2077 696c 6c20 6f76 6572 7269 6465 2074   will override t
+000054e0: 6865 2064 6566 6175 6c74 2060 7b7b 7573  he default `{{us
+000054f0: 6572 6e61 6d65 7d7d 6020 6469 7265 6374  ername}}` direct
+00005500: 6976 652e 0a0a 2323 204e 6573 7465 6420  ive...## Nested 
+00005510: 5661 7269 6162 6c65 730a 0a49 6e20 7468  Variables..In th
+00005520: 6520 6361 7365 206f 6620 2a2a 544f 4d4c  e case of **TOML
+00005530: 2070 726f 7065 7274 6965 7320 6f6e 6c79   properties only
+00005540: 2a2a 2c20 7661 7269 6162 6c65 2073 7562  **, variable sub
+00005550: 7374 6974 7574 696f 6e73 2063 616e 2062  stitutions can b
+00005560: 6520 6e65 7374 6564 2e0a 0a46 6f72 2065  e nested...For e
+00005570: 7861 6d70 6c65 2c20 6966 206f 6e65 2077  xample, if one w
+00005580: 616e 7465 6420 746f 2073 656c 6563 7420  anted to select 
+00005590: 6120 6469 6666 6572 656e 7420 6074 656d  a different `tem
+000055a0: 706c 6174 6549 6460 2066 6f72 2061 2057  plateId` for a W
+000055b0: 6f72 6b65 7220 506f 6f6c 2064 6570 656e  orker Pool depen
+000055c0: 6469 6e67 206f 6e20 7468 6520 7661 6c75  ding on the valu
+000055d0: 6520 6f66 2061 2060 7265 6769 6f6e 6020  e of a `region` 
+000055e0: 7661 7269 6162 6c65 2c20 6f6e 6520 636f  variable, one co
+000055f0: 756c 6420 7573 6520 7468 6520 666f 6c6c  uld use the foll
+00005600: 6f77 696e 673a 0a0a 6060 6074 6f6d 6c0a  owing:..```toml.
+00005610: 5b63 6f6d 6d6f 6e2e 7661 7269 6162 6c65  [common.variable
+00005620: 735d 0a20 2020 2074 656d 706c 6174 655f  s].    template_
+00005630: 6c6f 6e64 6f6e 203d 2022 7964 6964 3a63  london = "ydid:c
+00005640: 7274 3a36 3545 4634 463a 6134 6437 3537  rt:65EF4F:a4d757
+00005650: 6366 2d62 3637 612d 3465 6236 2d62 6433  cf-b67a-4eb6-bd3
+00005660: 392d 3861 3666 6664 3436 6338 6634 220a  9-8a6ffd46c8f4".
+00005670: 2020 2020 7465 6d70 6c61 7465 5f70 686f      template_pho
+00005680: 656e 6978 203d 2022 7964 6964 3a63 7274  enix = "ydid:crt
+00005690: 3a36 3545 4634 463a 6534 3233 3964 6563  :65EF4F:e4239dec
+000056a0: 2d37 3863 322d 3432 3163 2d61 3766 332d  -78c2-421c-a7f3-
+000056b0: 3731 6536 3162 3732 3934 3666 220a 2020  71e61b72946f".  
+000056c0: 2020 7465 6d70 6c61 7465 5f66 7261 6e6b    template_frank
+000056d0: 6675 7274 203d 2022 7964 6964 3a63 7274  furt = "ydid:crt
+000056e0: 3a36 3545 4634 463a 3332 3936 3032 6366  :65EF4F:329602cf
+000056f0: 2d35 3934 352d 3461 6164 2d61 3238 382d  -5945-4aad-a288-
+00005700: 6561 3432 3464 3634 6435 3565 220a 0a5b  ea424d64d55e"..[
+00005710: 776f 726b 6572 506f 6f6c 5d0a 2020 2020  workerPool].    
+00005720: 7465 6d70 6c61 7465 4964 203d 2022 7b7b  templateId = "{{
+00005730: 7465 6d70 6c61 7465 5f7b 7b72 6567 696f  template_{{regio
+00005740: 6e7d 7d7d 7d22 0a60 6060 0a0a 5468 656e  n}}}}".```..Then
+00005750: 2c20 6966 206f 6e65 2075 7365 6420 6079  , if one used `y
+00005760: 642d 7072 6f76 6973 696f 6e20 2d76 2072  d-provision -v r
+00005770: 6567 696f 6e3d 7068 6f65 6e69 7860 2c20  egion=phoenix`, 
+00005780: 7468 6520 6074 656d 706c 6174 6549 6460  the `templateId`
+00005790: 2070 726f 7065 7274 7920 776f 756c 6420   property would 
+000057a0: 6669 7273 7420 7265 736f 6c76 6520 746f  first resolve to
+000057b0: 2060 227b 7b74 656d 706c 6174 655f 7068   `"{{template_ph
+000057c0: 656f 6e69 787d 7d22 602c 2061 6e64 2074  eonix}}"`, and t
+000057d0: 6865 6e20 746f 2060 2279 6469 643a 6372  hen to `"ydid:cr
+000057e0: 743a 3635 4546 3446 3a65 3432 3339 6465  t:65EF4F:e4239de
+000057f0: 632d 3738 6332 2d34 3231 632d 6137 6633  c-78c2-421c-a7f3
+00005800: 2d37 3165 3631 6237 3239 3436 6622 602e  -71e61b72946f"`.
+00005810: 0a0a 4e65 7374 696e 6720 6361 6e20 6265  ..Nesting can be
+00005820: 2075 7020 746f 2074 6872 6565 206c 6576   up to three lev
+00005830: 656c 7320 6465 6570 2069 6e63 6c75 6469  els deep includi
+00005840: 6e67 2074 6865 2074 6f70 206c 6576 656c  ng the top level
+00005850: 2e0a 0a23 2057 6f72 6b20 5265 7175 6972  ...# Work Requir
+00005860: 656d 656e 7420 5072 6f70 6572 7469 6573  ement Properties
+00005870: 0a0a 5468 6520 6077 6f72 6b52 6571 7569  ..The `workRequi
+00005880: 7265 6d65 6e74 6020 7365 6374 696f 6e20  rement` section 
+00005890: 6f66 2074 6865 2063 6f6e 6669 6775 7261  of the configura
+000058a0: 7469 6f6e 2066 696c 6520 6973 206f 7074  tion file is opt
+000058b0: 696f 6e61 6c2e 2049 7427 7320 7573 6564  ional. It's used
+000058c0: 206f 6e6c 7920 6279 2074 6865 2060 7964   only by the `yd
+000058d0: 2d73 7562 6d69 7460 2063 6f6d 6d61 6e64  -submit` command
+000058e0: 2c20 616e 6420 636f 6e74 726f 6c73 2074  , and controls t
+000058f0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+00005900: 656e 7420 7468 6174 2069 7320 7375 626d  ent that is subm
+00005910: 6974 7465 6420 746f 2074 6865 2050 6c61  itted to the Pla
+00005920: 7466 6f72 6d2e 0a0a 5468 6520 6465 7461  tform...The deta
+00005930: 696c 7320 6f66 2061 2057 6f72 6b20 5265  ils of a Work Re
+00005940: 7175 6972 656d 656e 7420 746f 2062 6520  quirement to be 
+00005950: 7375 626d 6974 7465 6420 6361 6e20 6265  submitted can be
+00005960: 2063 6170 7475 7265 6420 656e 7469 7265   captured entire
+00005970: 6c79 2077 6974 6869 6e20 7468 6520 544f  ly within the TO
+00005980: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+00005990: 2066 696c 6520 666f 7220 7369 6d70 6c65   file for simple
+000059a0: 2065 7861 6d70 6c65 732e 204d 6f72 6520   examples. More 
+000059b0: 636f 6d70 6c65 7820 6578 616d 706c 6573  complex examples
+000059c0: 2063 6170 7475 7265 2074 6865 2057 6f72   capture the Wor
+000059d0: 6b20 5265 7175 6972 656d 656e 7420 696e  k Requirement in
+000059e0: 2061 2063 6f6d 6269 6e61 7469 6f6e 206f   a combination o
+000059f0: 6620 7468 6520 544f 4d4c 2066 696c 6520  f the TOML file 
+00005a00: 706c 7573 2061 204a 534f 4e20 646f 6375  plus a JSON docu
+00005a10: 6d65 6e74 2c20 6f72 2069 6e20 6120 4a53  ment, or in a JS
+00005a20: 4f4e 2064 6f63 756d 656e 7420 6f6e 6c79  ON document only
+00005a30: 2e0a 0a23 2320 576f 726b 2052 6571 7569  ...## Work Requi
+00005a40: 7265 6d65 6e74 204a 534f 4e20 4669 6c65  rement JSON File
+00005a50: 2053 7472 7563 7475 7265 0a0a 576f 726b   Structure..Work
+00005a60: 2052 6571 7569 7265 6d65 6e74 7320 6172   Requirements ar
+00005a70: 6520 7265 7072 6573 656e 7465 6420 696e  e represented in
+00005a80: 204a 534f 4e20 646f 6375 6d65 6e74 7320   JSON documents 
+00005a90: 7573 696e 6720 6120 636f 6e74 6169 6e6d  using a containm
+00005aa0: 656e 7420 6869 6572 6172 6368 7920 6f66  ent hierarchy of
+00005ab0: 2061 202a 2a57 6f72 6b20 5265 7175 6972   a **Work Requir
+00005ac0: 656d 656e 742a 2a20 636f 6e74 6169 6e69  ement** containi
+00005ad0: 6e67 2061 202a 2a6c 6973 7420 6f66 2054  ng a **list of T
+00005ae0: 6173 6b20 4772 6f75 7073 2a2a 2c20 636f  ask Groups**, co
+00005af0: 6e74 6169 6e69 6e67 2061 202a 2a6c 6973  ntaining a **lis
+00005b00: 7420 6f66 2054 6173 6b73 2a2a 2e0a 0a41  t of Tasks**...A
+00005b10: 2076 6572 7920 7369 6d70 6c65 2065 7861   very simple exa
+00005b20: 6d70 6c65 2064 6f63 756d 656e 7420 6973  mple document is
+00005b30: 2073 686f 776e 2062 656c 6f77 2077 6974   shown below wit
+00005b40: 6820 6120 746f 702d 6c65 7665 6c20 576f  h a top-level Wo
+00005b50: 726b 2052 6571 7569 7265 6d65 6e74 2063  rk Requirement c
+00005b60: 6f6e 7461 696e 696e 6720 7477 6f20 5461  ontaining two Ta
+00005b70: 736b 2047 726f 7570 7320 6561 6368 2063  sk Groups each c
+00005b80: 6f6e 7461 696e 696e 6720 7477 6f20 5461  ontaining two Ta
+00005b90: 736b 732c 2065 6163 6820 7769 7468 2061  sks, each with a
+00005ba0: 2064 6966 6665 7265 6e74 2073 6574 206f   different set o
+00005bb0: 6620 6172 6775 6d65 6e74 7320 746f 2062  f arguments to b
+00005bc0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
+00005bd0: 5461 736b 2e0a 0a60 6060 6a73 6f6e 0a7b  Task...```json.{
+00005be0: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+00005bf0: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+00005c00: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
+00005c10: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00005c20: 7267 756d 656e 7473 223a 205b 312c 2032  rguments": [1, 2
+00005c30: 2c20 335d 0a20 2020 2020 2020 207d 2c0a  , 3].        },.
+00005c40: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00005c50: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
+00005c60: 205b 342c 2035 2c20 365d 0a20 2020 2020   [4, 5, 6].     
+00005c70: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+00005c80: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00005c90: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
+00005ca0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00005cb0: 6172 6775 6d65 6e74 7322 3a20 5b37 2c20  arguments": [7, 
+00005cc0: 382c 2039 5d0a 2020 2020 2020 2020 7d2c  8, 9].        },
+00005cd0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00005ce0: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+00005cf0: 3a20 5b31 302c 2031 312c 2031 325d 0a20  : [10, 11, 12]. 
+00005d00: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00005d10: 0a20 2020 207d 0a20 205d 0a7d 0a0a 6060  .    }.  ].}..``
+00005d20: 600a 0a54 6f20 7370 6563 6966 7920 7468  `..To specify th
+00005d30: 6520 6669 6c65 2063 6f6e 7461 696e 696e  e file containin
+00005d40: 6720 7468 6520 4a53 4f4e 2064 6f63 756d  g the JSON docum
+00005d50: 656e 742c 2065 6974 6865 7220 706f 7075  ent, either popu
+00005d60: 6c61 7465 2074 6865 2060 776f 726b 5265  late the `workRe
+00005d70: 7175 6972 656d 656e 7444 6174 6160 2070  quirementData` p
+00005d80: 726f 7065 7274 7920 696e 2074 6865 2060  roperty in the `
+00005d90: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+00005da0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+00005db0: 544f 4d4c 2063 6f6e 6669 6775 7261 7469  TOML configurati
+00005dc0: 6f6e 2066 696c 6520 7769 7468 2074 6865  on file with the
+00005dd0: 204a 534f 4e20 6669 6c65 6e61 6d65 2c20   JSON filename, 
+00005de0: 6f72 2073 7065 6369 6679 2069 7420 6f6e  or specify it on
+00005df0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00005e00: 6520 7573 696e 6720 7468 6520 602d 2d77  e using the `--w
+00005e10: 6f72 6b2d 7265 7175 6972 656d 656e 7460  ork-requirement`
+00005e20: 206f 7220 602d 7260 206f 7074 696f 6e73   or `-r` options
+00005e30: 2028 7768 6963 6820 7769 6c6c 206f 7665   (which will ove
+00005e40: 7272 6964 6520 7468 6520 7072 6f70 6572  rride the proper
+00005e50: 7479 2069 6e20 7468 6520 544f 4d4c 2066  ty in the TOML f
+00005e60: 696c 6529 2c20 652e 672e 0a0a 6079 642d  ile), e.g...`yd-
+00005e70: 7375 626d 6974 202d 2d63 6f6e 6669 6720  submit --config 
+00005e80: 6d79 636f 6e66 6967 2e74 6f6d 6c20 2d2d  myconfig.toml --
+00005e90: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
+00005ea0: 206d 795f 776f 726b 7265 712e 6a73 6f6e   my_workreq.json
+00005eb0: 600a 0a23 2320 5072 6f70 6572 7479 2049  `..## Property I
+00005ec0: 6e68 6572 6974 616e 6365 0a0a 546f 2073  nheritance..To s
+00005ed0: 696d 706c 6966 7920 7468 6520 6465 6669  implify the defi
+00005ee0: 6e69 7469 6f6e 206f 6620 576f 726b 2052  nition of Work R
+00005ef0: 6571 7569 7265 6d65 6e74 732c 2074 6865  equirements, the
+00005f00: 7265 2069 7320 6120 7072 6f70 6572 7479  re is a property
+00005f10: 2069 6e68 6572 6974 616e 6365 206d 6563   inheritance mec
+00005f20: 6861 6e69 736d 2e20 5072 6f70 6572 7469  hanism. Properti
+00005f30: 6573 2074 6861 7420 6172 6520 7365 7420  es that are set 
+00005f40: 6174 2061 2068 6967 6865 7220 6c65 7665  at a higher leve
+00005f50: 6c20 696e 2074 6865 2068 6965 7261 7263  l in the hierarc
+00005f60: 6879 2061 7265 2069 6e68 6572 6974 6564  hy are inherited
+00005f70: 2061 7420 6c6f 7765 7220 6c65 7665 6c73   at lower levels
+00005f80: 2c20 756e 6c65 7373 2065 7870 6c69 6369  , unless explici
+00005f90: 746c 7920 6f76 6572 7269 6464 656e 2e0a  tly overridden..
+00005fa0: 0a54 6869 7320 6d65 616e 7320 7468 6174  .This means that
+00005fb0: 2061 2070 726f 7065 7274 7920 7365 7420   a property set 
+00005fc0: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
+00005fd0: 6972 656d 656e 7460 2073 6563 7469 6f6e  irement` section
+00005fe0: 206f 6620 7468 6520 544f 4d4c 2066 696c   of the TOML fil
+00005ff0: 6520 6361 6e20 6265 2069 6e68 6572 6974  e can be inherit
+00006000: 6564 2073 7563 6365 7373 6976 656c 7920  ed successively 
+00006010: 6279 2074 6865 2057 6f72 6b20 5265 7175  by the Work Requ
+00006020: 6972 656d 656e 742c 2054 6173 6b20 4772  irement, Task Gr
+00006030: 6f75 7073 2061 6e64 2054 6173 6b73 2069  oups and Tasks i
+00006040: 6e20 7468 6520 4a53 4f4e 2064 6f63 756d  n the JSON docum
+00006050: 656e 7420 2861 7373 756d 696e 6720 7468  ent (assuming th
+00006060: 6520 7072 6f70 6572 7479 2069 7320 7661  e property is va
+00006070: 6c69 6420 6174 2065 6163 6820 6c65 7665  lid at each leve
+00006080: 6c29 2e20 2048 656e 6365 2c20 5461 736b  l).  Hence, Task
+00006090: 7320 696e 6865 7269 7420 6672 6f6d 2054  s inherit from T
+000060a0: 6173 6b20 4772 6f75 7073 2c20 7768 6963  ask Groups, whic
+000060b0: 6820 696e 6865 7269 7420 6672 6f6d 2074  h inherit from t
+000060c0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+000060d0: 656e 7420 696e 2074 6865 204a 534f 4e20  ent in the JSON 
+000060e0: 646f 6375 6d65 6e74 2c20 7768 6963 6820  document, which 
+000060f0: 696e 6865 7269 7473 2066 726f 6d20 7468  inherits from th
+00006100: 6520 6077 6f72 6b52 6571 7569 7265 6d65  e `workRequireme
+00006110: 6e74 6020 7072 6f70 6572 7469 6573 2069  nt` properties i
+00006120: 6e20 7468 6520 544f 4d4c 2066 696c 652e  n the TOML file.
+00006130: 0a0a 4f76 6572 7269 6464 656e 2070 726f  ..Overridden pro
+00006140: 7065 7274 6965 7320 6172 6520 616c 736f  perties are also
+00006150: 2069 6e68 6572 6974 6564 2e20 452e 672e   inherited. E.g.
+00006160: 2c20 6966 2061 2070 726f 7065 7274 7920  , if a property 
+00006170: 6973 2073 6574 2061 7420 7468 6520 5461  is set at the Ta
+00006180: 736b 2047 726f 7570 206c 6576 656c 2c20  sk Group level, 
+00006190: 6974 2077 696c 6c20 6265 2069 6e68 6572  it will be inher
+000061a0: 6974 6564 2062 7920 7468 6520 5461 736b  ited by the Task
+000061b0: 7320 696e 2074 6861 7420 5461 736b 2047  s in that Task G
+000061c0: 726f 7570 2075 6e6c 6573 7320 6578 706c  roup unless expl
+000061d0: 6963 6974 6c79 206f 7665 7272 6964 6465  icitly overridde
+000061e0: 6e2e 0a0a 2323 2057 6f72 6b20 5265 7175  n...## Work Requ
+000061f0: 6972 656d 656e 7420 5072 6f70 6572 7479  irement Property
+00006200: 2044 6963 7469 6f6e 6172 790a 0a54 6865   Dictionary..The
+00006210: 2066 6f6c 6c6f 7769 6e67 2074 6162 6c65   following table
+00006220: 206f 7574 6c69 6e65 7320 616c 6c20 7468   outlines all th
+00006230: 6520 7072 6f70 6572 7469 6573 2061 7661  e properties ava
+00006240: 696c 6162 6c65 2066 6f72 2064 6566 696e  ilable for defin
+00006250: 696e 6720 576f 726b 2052 6571 7569 7265  ing Work Require
+00006260: 6d65 6e74 732c 2061 6e64 2074 6865 206c  ments, and the l
+00006270: 6576 656c 7320 6174 2077 6869 6368 2074  evels at which t
+00006280: 6865 7920 6172 6520 616c 6c6f 7765 6420  hey are allowed 
+00006290: 746f 2062 6520 7573 6564 2e20 536f 2c20  to be used. So, 
+000062a0: 666f 7220 6578 616d 706c 652c 2074 6865  for example, the
+000062b0: 2060 7072 6f76 6964 6572 6020 7072 6f70   `provider` prop
+000062c0: 6572 7479 2063 616e 2062 6520 7365 7420  erty can be set 
+000062d0: 696e 2074 6865 2054 4f4d 4c20 6669 6c65  in the TOML file
+000062e0: 2c20 6174 2074 6865 2057 6f72 6b20 5265  , at the Work Re
+000062f0: 7175 6972 656d 656e 7420 4c65 7665 6c20  quirement Level 
+00006300: 6f72 2061 7420 7468 6520 5461 736b 2047  or at the Task G
+00006310: 726f 7570 204c 6576 656c 2c20 6275 7420  roup Level, but 
+00006320: 6e6f 7420 6174 2074 6865 2054 6173 6b20  not at the Task 
+00006330: 6c65 7665 6c2c 2061 6e64 2070 726f 7065  level, and prope
+00006340: 7274 7920 6064 6570 656e 6465 6e74 4f6e  rty `dependentOn
+00006350: 6020 6361 6e20 6f6e 6c79 2062 6520 7365  ` can only be se
+00006360: 7420 6174 2074 6865 2054 6173 6b20 4772  t at the Task Gr
+00006370: 6f75 7020 6c65 7665 6c2e 0a0a 416c 6c20  oup level...All 
+00006380: 7072 6f70 6572 7469 6573 2061 7265 206f  properties are o
+00006390: 7074 696f 6e61 6c20 6578 6365 7074 2066  ptional except f
+000063a0: 6f72 202a 2a60 7461 736b 5479 7065 602a  or **`taskType`*
+000063b0: 2a20 286f 7220 2a2a 6074 6173 6b54 7970  * (or **`taskTyp
+000063c0: 6573 602a 2a29 2e0a 0a7c 2050 726f 7065  es`**)...| Prope
+000063d0: 7274 7920 4e61 6d65 2020 2020 2020 2020  rty Name        
+000063e0: 2020 2020 2020 7c20 4465 7363 7269 7074        | Descript
+000063f0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
 00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2020 2020 2020 2020 207c 2054 4f4d 4c20           | TOML 
-00006440: 7c20 5752 2020 7c20 5447 7270 207c 2054  | WR  | TGrp | T
-00006450: 6173 6b20 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d  ask |.|:--------
-00006460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006470: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
-00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006490: 207c 2054 4f4d 4c20 7c20 5752 2020 7c20   | TOML | WR  | 
+000064a0: 5447 7270 207c 2054 6173 6b20 7c0a 7c3a  TGrp | Task |.|:
 000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
 000064d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00006500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a  --------------|:
-00006520: 2d2d 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d  -----|:----|:---
-00006530: 2d2d 7c3a 2d2d 2d2d 2d7c 0a7c 2060 6172  --|:-----|.| `ar
-00006540: 6775 6d65 6e74 7360 2020 2020 2020 2020  guments`        
-00006550: 2020 2020 2020 2020 7c20 5468 6520 6c69          | The li
-00006560: 7374 206f 6620 6172 6775 6d65 6e74 7320  st of arguments 
-00006570: 746f 2062 6520 7061 7373 6564 2074 6f20  to be passed to 
-00006580: 7468 6520 5461 736b 2077 6865 6e20 6974  the Task when it
-00006590: 2069 7320 6578 6563 7574 6564 2e20 452e   is executed. E.
-000065a0: 672e 3a20 605b 312c 2022 5477 6f22 5d60  g.: `[1, "Two"]`
-000065b0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-00006610: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
-00006620: 7c20 6063 6170 7475 7265 5461 736b 4f75  | `captureTaskOu
-00006630: 7470 7574 6020 2020 2020 2020 207c 2057  tput`        | W
-00006640: 6865 7468 6572 2074 6865 2063 6f6e 736f  hether the conso
-00006650: 6c65 206f 7574 7075 7420 6f66 2061 2054  le output of a T
-00006660: 6173 6b27 7320 7072 6f63 6573 7320 7368  ask's process sh
-00006670: 6f75 6c64 2062 6520 7570 6c6f 6164 6564  ould be uploaded
-00006680: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
-00006690: 6720 4f62 6a65 6374 2053 746f 7265 206f  g Object Store o
-000066a0: 6e20 5461 736b 2063 6f6d 706c 6574 696f  n Task completio
-000066b0: 6e2e 2044 6566 6175 6c74 3a20 6074 7275  n. Default: `tru
-000066c0: 6560 2e20 2020 2020 2020 2020 2020 2020  e`.             
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-000066f0: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
-00006700: 7320 207c 0a7c 2060 636f 6d70 6c65 7465  s  |.| `complete
-00006710: 6454 6173 6b54 746c 6020 2020 2020 2020  dTaskTtl`       
-00006720: 2020 7c20 5468 6520 7469 6d65 2028 696e    | The time (in
-00006730: 206d 696e 7574 6573 2920 746f 206c 6976   minutes) to liv
-00006740: 6520 666f 7220 636f 6d70 6c65 7465 6420  e for completed 
-00006750: 5461 736b 732e 2049 6620 7365 742c 2054  Tasks. If set, T
-00006760: 6173 6b73 2074 6861 7420 6861 7665 2062  asks that have b
-00006770: 6565 6e20 636f 6d70 6c65 7465 6420 666f  een completed fo
-00006780: 7220 6c6f 6e67 6572 2074 6861 6e20 7468  r longer than th
-00006790: 6973 2070 6572 696f 6420 7769 6c6c 2062  is period will b
-000067a0: 6520 6465 6c65 7465 642e 2045 2e67 2e3a  e deleted. E.g.:
-000067b0: 2060 3130 2e30 602e 2020 2020 2020 2020   `10.0`.        
-000067c0: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-000067d0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-000067e0: 207c 2020 2020 2020 7c0a 7c20 6063 7376   |      |.| `csv
-000067f0: 4669 6c65 6020 2020 2020 2020 2020 2020  File`           
-00006800: 2020 2020 2020 207c 2054 6865 206e 616d         | The nam
-00006810: 6520 6f66 2074 6865 2043 5356 2066 696c  e of the CSV fil
-00006820: 6520 7573 6564 2074 6f20 6465 7269 7665  e used to derive
-00006830: 2054 6173 6b20 6461 7461 2e20 416e 2061   Task data. An a
-00006840: 6c74 6572 6e61 7469 7665 2074 6f20 6063  lternative to `c
-00006850: 7376 4669 6c65 7360 2074 6861 7420 6361  svFiles` that ca
-00006860: 6e20 6265 2075 7365 6420 7768 656e 2074  n be used when t
-00006870: 6865 7265 2773 206f 6e6c 7920 6120 7369  here's only a si
-00006880: 6e67 6c65 2043 5356 2066 696c 652e 2045  ngle CSV file. E
-00006890: 2e67 2e20 6022 6669 6c65 2e63 7376 2260  .g. `"file.csv"`
-000068a0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-000068b0: 2020 7c20 5965 7320 207c 2020 2020 207c    | Yes  |     |
-000068c0: 2020 2020 2020 7c20 2020 2020 207c 0a7c        |      |.|
-000068d0: 2060 6373 7646 696c 6573 6020 2020 2020   `csvFiles`     
-000068e0: 2020 2020 2020 2020 2020 2020 7c20 4120              | A 
-000068f0: 6c69 7374 206f 6620 4353 5620 6669 6c65  list of CSV file
-00006900: 7320 7573 6564 2074 6f20 6465 7269 7665  s used to derive
-00006910: 2054 6173 6b20 6461 7461 2e20 452e 672e   Task data. E.g.
-00006920: 2060 5b22 6669 6c65 2e63 7376 222c 2022   `["file.csv", "
-00006930: 6669 6c65 5f32 2e63 7376 3a32 5d60 2e20  file_2.csv:2]`. 
-00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-000069a0: 2020 2020 7c20 2020 2020 207c 2020 2020      |      |    
-000069b0: 2020 7c0a 7c20 6064 6570 656e 6465 6e74    |.| `dependent
-000069c0: 4f6e 6020 2020 2020 2020 2020 2020 2020  On`             
-000069d0: 207c 2054 6865 206e 616d 6520 6f66 2061   | The name of a
-000069e0: 6e6f 7468 6572 2054 6173 6b20 4772 6f75  nother Task Grou
-000069f0: 7020 7769 7468 696e 2074 6865 2073 616d  p within the sam
-00006a00: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-00006a10: 6e74 2074 6861 7420 6d75 7374 2062 6520  nt that must be 
-00006a20: 7375 6363 6573 7366 756c 6c79 2063 6f6d  successfully com
-00006a30: 706c 6574 6564 2062 6566 6f72 6520 7468  pleted before th
-00006a40: 6520 5461 736b 2047 726f 7570 2069 7320  e Task Group is 
-00006a50: 7374 6172 7465 642e 2045 2e67 2e20 6022  started. E.g. `"
-00006a60: 7461 736b 5f67 726f 7570 5f31 2260 2e20  task_group_1"`. 
-00006a70: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00006a80: 2020 207c 2020 2020 207c 2059 6573 2020     |     | Yes  
-00006a90: 7c20 2020 2020 207c 0a7c 2060 646f 636b  |      |.| `dock
-00006aa0: 6572 456e 7669 726f 6e6d 656e 7460 2020  erEnvironment`  
-00006ab0: 2020 2020 2020 7c20 5468 6520 656e 7669        | The envi
-00006ac0: 726f 6e6d 656e 7420 746f 2062 6520 7061  ronment to be pa
-00006ad0: 7373 6564 2074 6f20 6120 446f 636b 6572  ssed to a Docker
-00006ae0: 2063 6f6e 7461 696e 6572 2e20 4f6e 6c79   container. Only
-00006af0: 2075 7365 6420 6279 2074 6865 2060 646f   used by the `do
-00006b00: 636b 6572 6020 5461 736b 2054 7970 652e  cker` Task Type.
-00006b10: 2045 2e67 2e2c 204a 534f 4e3a 2060 7b22   E.g., JSON: `{"
-00006b20: 5641 525f 3122 3a20 2261 6263 227d 602c  VAR_1": "abc"}`,
-00006b30: 2054 4f4d 4c3a 2060 7b56 4152 5f31 203d   TOML: `{VAR_1 =
-00006b40: 2022 6162 6322 2c20 5641 525f 3220 3d20   "abc", VAR_2 = 
-00006b50: 2264 6566 227d 602e 2020 2020 2020 2020  "def"}`.        
-00006b60: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00006b70: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
-00006b80: 6064 6f63 6b65 7250 6173 7377 6f72 6460  `dockerPassword`
-00006b90: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00006ba0: 2070 6173 7377 6f72 6420 666f 7220 446f   password for Do
-00006bb0: 636b 6572 4875 622c 206f 6e6c 7920 7573  ckerHub, only us
-00006bc0: 6564 2062 7920 7468 6520 6064 6f63 6b65  ed by the `docke
-00006bd0: 7260 2054 6173 6b20 5479 7065 2e20 452c  r` Task Type. E,
-00006be0: 672e 2c20 6022 6d79 5f70 6173 7377 6f72  g., `"my_passwor
-00006bf0: 6422 602e 2020 2020 2020 2020 2020 2020  d"`.            
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00006c50: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
-00006c60: 207c 0a7c 2060 646f 636b 6572 5573 6572   |.| `dockerUser
-00006c70: 6e61 6d65 6020 2020 2020 2020 2020 2020  name`           
-00006c80: 7c20 5468 6520 7573 6572 6e61 6d65 2066  | The username f
-00006c90: 6f72 2044 6f63 6b65 7248 7562 2c20 6f6e  or DockerHub, on
-00006ca0: 6c79 2075 7365 6420 6279 2074 6865 2060  ly used by the `
-00006cb0: 646f 636b 6572 6020 5461 736b 2054 7970  docker` Task Typ
-00006cc0: 652e 2045 2c67 2e2c 2060 226d 795f 7573  e. E,g., `"my_us
-00006cd0: 6572 6e61 6d65 2260 2e20 2020 2020 2020  ername"`.       
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00006d30: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00006d40: 2059 6573 2020 7c0a 7c20 6065 6e76 6972   Yes  |.| `envir
-00006d50: 6f6e 6d65 6e74 6020 2020 2020 2020 2020  onment`         
-00006d60: 2020 2020 207c 2054 6865 2065 6e76 6972       | The envir
-00006d70: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00006d80: 2074 6f20 7365 7420 666f 7220 6120 5461   to set for a Ta
-00006d90: 736b 2077 6865 6e20 6974 2773 2065 7865  sk when it's exe
-00006da0: 6375 7465 642e 2045 2e67 2e2c 204a 534f  cuted. E.g., JSO
-00006db0: 4e3a 2060 7b22 5641 525f 3122 3a20 2261  N: `{"VAR_1": "a
-00006dc0: 6263 222c 2022 5641 525f 3222 3a20 2264  bc", "VAR_2": "d
-00006dd0: 6566 227d 602c 2054 4f4d 4c3a 2060 7b56  ef"}`, TOML: `{V
-00006de0: 4152 5f31 203d 2022 6162 6322 2c20 5641  AR_1 = "abc", VA
-00006df0: 525f 3220 3d20 2264 6566 227d 602e 2020  R_2 = "def"}`.  
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00006e20: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
-00006e30: 6578 636c 7573 6976 6557 6f72 6b65 7273  exclusiveWorkers
-00006e40: 6020 2020 2020 2020 2020 7c20 4966 2074  `         | If t
-00006e50: 7275 652c 2074 6865 6e20 646f 206e 6f74  rue, then do not
-00006e60: 2061 6c6c 6f77 2063 6c61 696d 6564 2057   allow claimed W
-00006e70: 6f72 6b65 7273 2074 6f20 6265 2073 6861  orkers to be sha
-00006e80: 7265 6420 7769 7468 206f 7468 6572 2054  red with other T
-00006e90: 6173 6b20 4772 6f75 7073 3b20 6f74 6865  ask Groups; othe
-00006ea0: 7277 6973 652c 2057 6f72 6b65 7273 2063  rwise, Workers c
-00006eb0: 616e 2062 6520 7368 6172 6564 2e20 4465  an be shared. De
-00006ec0: 6661 756c 743a 6066 616c 7365 602e 2020  fault:`false`.  
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-00006f00: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
-00006f10: 7c0a 7c20 6065 7865 6375 7461 626c 6560  |.| `executable`
-00006f20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006f30: 2054 6865 2027 6578 6563 7574 6162 6c65   The 'executable
-00006f40: 2720 746f 2072 756e 2077 6865 6e20 6120  ' to run when a 
-00006f50: 4261 7368 206f 7220 446f 636b 6572 2054  Bash or Docker T
-00006f60: 6173 6b20 6973 2065 7865 6375 7465 642e  ask is executed.
-00006f70: 2042 6173 6820 7363 7269 7074 2066 6f72   Bash script for
-00006f80: 2042 6173 682c 2063 6f6e 7461 696e 6572   Bash, container
-00006f90: 2069 6d61 6765 2066 6f72 2044 6f63 6b65   image for Docke
-00006fa0: 722e 204f 7074 696f 6e61 6c3a 206f 6d69  r. Optional: omi
-00006fb0: 7420 746f 2073 7570 7072 6573 7320 6175  t to suppress au
-00006fc0: 746f 6d61 7469 6320 7072 6f63 6573 7369  tomatic processi
-00006fd0: 6e67 2e20 2020 2020 2020 7c20 5965 7320  ng.       | Yes 
-00006fe0: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
-00006ff0: 5965 7320 207c 0a7c 2060 6669 6e69 7368  Yes  |.| `finish
-00007000: 4966 416c 6c54 6173 6b73 4669 6e69 7368  IfAllTasksFinish
-00007010: 6564 6020 7c20 4966 2074 7275 652c 2074  ed` | If true, t
-00007020: 6865 2054 6173 6b20 4772 6f75 7020 7769  he Task Group wi
-00007030: 6c6c 2066 696e 6973 6820 6175 746f 6d61  ll finish automa
-00007040: 7469 6361 6c6c 7920 6966 2061 6c6c 2063  tically if all c
-00007050: 6f6e 7461 696e 6564 2074 6173 6b73 2066  ontained tasks f
-00007060: 696e 6973 682e 2044 6566 6175 6c74 3a60  inish. Default:`
-00007070: 7472 7565 602e 2020 2020 2020 2020 2020  true`.          
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000070c0: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
-000070d0: 7320 207c 2020 2020 2020 7c0a 7c20 6066  s  |      |.| `f
-000070e0: 696e 6973 6849 6641 6e79 5461 736b 4661  inishIfAnyTaskFa
-000070f0: 696c 6564 6020 2020 207c 2049 6620 7472  iled`    | If tr
-00007100: 7565 2c20 7468 6520 5461 736b 2047 726f  ue, the Task Gro
-00007110: 7570 2077 696c 6c20 6265 2066 6169 6c65  up will be faile
-00007120: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
-00007130: 6966 2061 6e79 2063 6f6e 7461 696e 6564  if any contained
-00007140: 2074 6173 6b73 2066 6169 6c2e 2044 6566   tasks fail. Def
-00007150: 6175 6c74 3a60 6661 6c73 6560 2e20 2020  ault:`false`.   
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-000071b0: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
-000071c0: 0a7c 2060 666c 6174 7465 6e49 6e70 7574  .| `flattenInput
-000071d0: 5061 7468 7360 2020 2020 2020 2020 7c20  Paths`        | 
-000071e0: 4465 7465 726d 696e 6573 2077 6865 7468  Determines wheth
-000071f0: 6572 2069 6e70 7574 206f 626a 6563 7420  er input object 
-00007200: 7061 7468 7320 7368 6f75 6c64 2062 6520  paths should be 
-00007210: 666c 6174 7465 6e65 6420 2869 2e65 2e2c  flattened (i.e.,
-00007220: 2064 6972 6563 746f 7279 2073 7472 7563   directory struc
-00007230: 7475 7265 2072 656d 6f76 6564 2920 7768  ture removed) wh
-00007240: 656e 2064 6f77 6e6c 6f61 6465 6420 746f  en downloaded to
-00007250: 2061 206e 6f64 652e 2044 6566 6175 6c74   a node. Default
-00007260: 3a20 6066 616c 7365 602e 2020 2020 2020  : `false`.      
-00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-00007290: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
-000072a0: 6573 2020 7c0a 7c20 6066 6c61 7474 656e  es  |.| `flatten
-000072b0: 5570 6c6f 6164 5061 7468 7360 2020 2020  UploadPaths`    
-000072c0: 2020 207c 2049 676e 6f72 6520 6c6f 6361     | Ignore loca
-000072d0: 6c20 6469 7265 6374 6f72 7920 7061 7468  l directory path
-000072e0: 7320 7768 656e 2075 706c 6f61 6469 6e67  s when uploading
-000072f0: 2066 696c 6573 2074 6f20 7468 6520 4f62   files to the Ob
-00007300: 6a65 6374 2053 746f 7265 3b20 706c 6163  ject Store; plac
-00007310: 6520 696e 2060 3c6e 616d 6573 7061 6365  e in `<namespace
-00007320: 3e3a 3c77 6f72 6b2d 7265 712d 6e61 6d65  >:<work-req-name
-00007330: 3e2f 602e 2044 6566 6175 6c74 3a20 6066  >/`. Default: `f
-00007340: 616c 7365 602e 2020 2020 2020 2020 2020  alse`.          
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007370: 5965 7320 207c 2059 6573 207c 2020 2020  Yes  | Yes |    
-00007380: 2020 7c20 2020 2020 207c 0a7c 2060 6675    |      |.| `fu
-00007390: 6c66 696c 4f6e 5375 626d 6974 6020 2020  lfilOnSubmit`   
-000073a0: 2020 2020 2020 2020 7c20 496e 6469 6361          | Indica
-000073b0: 7465 7320 6966 2074 6865 2057 6f72 6b20  tes if the Work 
-000073c0: 5265 7175 6972 656d 656e 7420 7368 6f75  Requirement shou
-000073d0: 6c64 2062 6520 6675 6c66 696c 6c65 6420  ld be fulfilled 
-000073e0: 7768 656e 2069 7420 6973 2073 7562 6d69  when it is submi
-000073f0: 7474 6564 2c20 7261 7468 6572 2074 6861  tted, rather tha
-00007400: 6e20 6265 696e 6720 616c 6c6f 7765 6420  n being allowed 
-00007410: 746f 2077 6169 7420 696e 2050 454e 4449  to wait in PENDI
-00007420: 4e47 2073 7461 7475 732e 2044 6566 6175  NG status. Defau
-00007430: 6c74 3a60 6661 6c73 6560 2e20 2020 2020  lt:`false`.     
-00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007450: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-00007460: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
-00007470: 7c20 6069 6e70 7574 7360 2020 2020 2020  | `inputs`      
-00007480: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-00007490: 6865 206c 6973 7420 6f66 2069 6e70 7574  he list of input
-000074a0: 2066 696c 6573 2074 6f20 6265 2075 706c   files to be upl
-000074b0: 6f61 6465 6420 746f 2074 6865 2059 656c  oaded to the Yel
-000074c0: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
-000074d0: 6f72 652c 2061 6e64 2072 6571 7569 7265  ore, and require
-000074e0: 6420 6279 2074 6865 2054 6173 6b20 2869  d by the Task (i
-000074f0: 6d70 6c69 6573 2060 7665 7269 6679 4174  mplies `verifyAt
-00007500: 5374 6172 7460 292e 2045 2e67 2e20 605b  Start`). E.g. `[
-00007510: 2261 2e73 6822 2c20 2262 2e73 6822 5d60  "a.sh", "b.sh"]`
-00007520: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00007530: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-00007540: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
-00007550: 7320 207c 0a7c 2060 696e 7075 7473 4f70  s  |.| `inputsOp
-00007560: 7469 6f6e 616c 6020 2020 2020 2020 2020  tional`         
-00007570: 2020 7c20 4120 6c69 7374 206f 6620 696e    | A list of in
-00007580: 7075 7420 6669 6c65 7320 7265 7175 6972  put files requir
-00007590: 6564 2062 7920 6120 5461 736b 2c20 6275  ed by a Task, bu
-000075a0: 7420 7768 6963 6820 6172 6520 6e6f 7420  t which are not 
-000075b0: 7375 626a 6563 7420 746f 2076 6572 6966  subject to verif
-000075c0: 6963 6174 696f 6e2e 2043 616e 2063 6f6e  ication. Can con
-000075d0: 7461 696e 2077 696c 6463 6172 6473 2e20  tain wildcards. 
-000075e0: 452e 672e 3a20 605b 2274 6173 6b5f 6772  E.g.: `["task_gr
-000075f0: 6f75 705f 312f 2a2a 2f72 6573 756c 7473  oup_1/**/results
-00007600: 2e74 7874 225d 602e 2020 2020 2020 2020  .txt"]`.        
-00007610: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-00007620: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-00007630: 207c 2059 6573 2020 7c0a 7c20 6069 6e73   | Yes  |.| `ins
-00007640: 7461 6e63 6554 7970 6573 6020 2020 2020  tanceTypes`     
-00007650: 2020 2020 2020 207c 2054 6865 206d 6163         | The mac
-00007660: 6869 6e65 2069 6e73 7461 6e63 6520 7479  hine instance ty
-00007670: 7065 7320 7468 6174 2063 616e 2062 6520  pes that can be 
-00007680: 7573 6564 2074 6f20 6578 6563 7574 6520  used to execute 
-00007690: 5461 736b 732e 2045 2e67 2e2c 2060 5b22  Tasks. E.g., `["
-000076a0: 7433 2e6d 6963 726f 222c 2022 7433 612e  t3.micro", "t3a.
-000076b0: 6d69 6372 6f22 5d60 2e20 2020 2020 2020  micro"]`.       
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-00007710: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
-00007720: 2060 6d61 7869 6d75 6d54 6173 6b52 6574   `maximumTaskRet
-00007730: 7269 6573 6020 2020 2020 2020 7c20 5468  ries`       | Th
-00007740: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
-00007750: 206f 6620 7469 6d65 7320 6120 5461 736b   of times a Task
-00007760: 2063 616e 2062 6520 7265 7472 6965 6420   can be retried 
-00007770: 6166 7465 7220 6974 2068 6173 2066 6169  after it has fai
-00007780: 6c65 642e 2045 2e67 2e3a 2060 3560 2e20  led. E.g.: `5`. 
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-000077f0: 5965 7320 7c20 5965 7320 207c 2020 2020  Yes | Yes  |    
-00007800: 2020 7c0a 7c20 606d 6178 576f 726b 6572    |.| `maxWorker
-00007810: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
-00007820: 207c 2054 6865 206d 6178 696d 756d 206e   | The maximum n
-00007830: 756d 6265 7220 6f66 2057 6f72 6b65 7273  umber of Workers
-00007840: 2074 6861 7420 6361 6e20 6265 2063 6c61   that can be cla
-00007850: 696d 6564 2066 6f72 2074 6865 2061 7373  imed for the ass
-00007860: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
-00007870: 7570 2e20 452e 672e 2c20 6031 3060 2e20  up. E.g., `10`. 
-00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-000078d0: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-000078e0: 7c20 2020 2020 207c 0a7c 2060 6d69 6e57  |      |.| `minW
-000078f0: 6f72 6b65 7273 6020 2020 2020 2020 2020  orkers`         
-00007900: 2020 2020 2020 7c20 5468 6520 6d69 6e69        | The mini
-00007910: 6d75 6d20 6e75 6d62 6572 206f 6620 576f  mum number of Wo
-00007920: 726b 6572 7320 7468 6174 2074 6865 2061  rkers that the a
-00007930: 7373 6f63 6961 7465 6420 5461 736b 2047  ssociated Task G
-00007940: 726f 7570 2072 6571 7569 7265 732e 2054  roup requires. T
-00007950: 6869 7320 6d61 6e79 2077 6f72 6b65 7273  his many workers
-00007960: 206d 7573 7420 6265 2063 6c61 696d 6564   must be claimed
-00007970: 2062 6566 6f72 6520 7468 6520 6173 736f   before the asso
-00007980: 6369 6174 6564 2054 6173 6b20 4772 6f75  ciated Task Grou
-00007990: 7020 7769 6c6c 2073 7461 7274 2077 6f72  p will start wor
-000079a0: 6b69 6e67 2e20 452e 672e 2c20 6031 602e  king. E.g., `1`.
-000079b0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-000079c0: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
-000079d0: 606e 616d 6560 2020 2020 2020 2020 2020  `name`          
-000079e0: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-000079f0: 206e 616d 6520 6f66 2074 6865 2057 6f72   name of the Wor
-00007a00: 6b20 5265 7175 6972 656d 656e 742c 2054  k Requirement, T
-00007a10: 6173 6b20 4772 6f75 7020 6f72 2054 6173  ask Group or Tas
-00007a20: 6b2e 2045 2e67 2e2c 2060 2277 725f 6e61  k. E.g., `"wr_na
-00007a30: 6d65 2260 2e20 4e6f 7465 2074 6861 7420  me"`. Note that 
-00007a40: 7468 6520 606e 616d 6560 2070 726f 7065  the `name` prope
-00007a50: 7274 7920 6973 206e 6f74 2069 6e68 6572  rty is not inher
-00007a60: 6974 6564 2e20 2020 2020 2020 2020 2020  ited.           
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00007aa0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
-00007ab0: 207c 0a7c 2060 6f75 7470 7574 7360 2020   |.| `outputs`  
+00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006570: 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d7c 3a2d  ------|:-----|:-
+00006580: 2d2d 2d7c 3a2d 2d2d 2d2d 7c3a 2d2d 2d2d  ---|:-----|:----
+00006590: 2d7c 0a7c 2060 6172 6775 6d65 6e74 7360  -|.| `arguments`
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 7c20 5468 6520 6c69 7374 206f 6620 6172  | The list of ar
+000065c0: 6775 6d65 6e74 7320 746f 2062 6520 7061  guments to be pa
+000065d0: 7373 6564 2074 6f20 7468 6520 5461 736b  ssed to the Task
+000065e0: 2077 6865 6e20 6974 2069 7320 6578 6563   when it is exec
+000065f0: 7574 6564 2e20 452e 672e 3a20 605b 312c  uted. E.g.: `[1,
+00006600: 2022 5477 6f22 5d60 2e20 2020 2020 2020   "Two"]`.       
+00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006650: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+00006660: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00006670: 2059 6573 2020 7c0a 7c20 6063 6170 7475   Yes  |.| `captu
+00006680: 7265 5461 736b 4f75 7470 7574 6020 2020  reTaskOutput`   
+00006690: 2020 2020 207c 2057 6865 7468 6572 2074       | Whether t
+000066a0: 6865 2063 6f6e 736f 6c65 206f 7574 7075  he console outpu
+000066b0: 7420 6f66 2061 2054 6173 6b27 7320 7072  t of a Task's pr
+000066c0: 6f63 6573 7320 7368 6f75 6c64 2062 6520  ocess should be 
+000066d0: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
+000066e0: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
+000066f0: 2053 746f 7265 206f 6e20 5461 736b 2063   Store on Task c
+00006700: 6f6d 706c 6574 696f 6e2e 2044 6566 6175  ompletion. Defau
+00006710: 6c74 3a20 6074 7275 6560 2e20 2020 2020  lt: `true`.     
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006740: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+00006750: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+00006760: 636f 6d70 6c65 7465 6454 6173 6b54 746c  completedTaskTtl
+00006770: 6020 2020 2020 2020 2020 7c20 5468 6520  `         | The 
+00006780: 7469 6d65 2028 696e 206d 696e 7574 6573  time (in minutes
+00006790: 2920 746f 206c 6976 6520 666f 7220 636f  ) to live for co
+000067a0: 6d70 6c65 7465 6420 5461 736b 732e 2049  mpleted Tasks. I
+000067b0: 6620 7365 742c 2054 6173 6b73 2074 6861  f set, Tasks tha
+000067c0: 7420 6861 7665 2062 6565 6e20 636f 6d70  t have been comp
+000067d0: 6c65 7465 6420 666f 7220 6c6f 6e67 6572  leted for longer
+000067e0: 2074 6861 6e20 7468 6973 2070 6572 696f   than this perio
+000067f0: 6420 7769 6c6c 2062 6520 6465 6c65 7465  d will be delete
+00006800: 642e 2045 2e67 2e3a 2060 3130 2e30 602e  d. E.g.: `10.0`.
+00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006820: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00006830: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
+00006840: 7c0a 7c20 6063 7376 4669 6c65 6020 2020  |.| `csvFile`   
+00006850: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006860: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00006870: 2043 5356 2066 696c 6520 7573 6564 2074   CSV file used t
+00006880: 6f20 6465 7269 7665 2054 6173 6b20 6461  o derive Task da
+00006890: 7461 2e20 416e 2061 6c74 6572 6e61 7469  ta. An alternati
+000068a0: 7665 2074 6f20 6063 7376 4669 6c65 7360  ve to `csvFiles`
+000068b0: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+000068c0: 6420 7768 656e 2074 6865 7265 2773 206f  d when there's o
+000068d0: 6e6c 7920 6120 7369 6e67 6c65 2043 5356  nly a single CSV
+000068e0: 2066 696c 652e 2045 2e67 2e20 6022 6669   file. E.g. `"fi
+000068f0: 6c65 2e63 7376 2260 2e20 2020 2020 2020  le.csv"`.       
+00006900: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+00006910: 207c 2020 2020 207c 2020 2020 2020 7c20   |     |      | 
+00006920: 2020 2020 207c 0a7c 2060 6373 7646 696c       |.| `csvFil
+00006930: 6573 6020 2020 2020 2020 2020 2020 2020  es`             
+00006940: 2020 2020 7c20 4120 6c69 7374 206f 6620      | A list of 
+00006950: 4353 5620 6669 6c65 7320 7573 6564 2074  CSV files used t
+00006960: 6f20 6465 7269 7665 2054 6173 6b20 6461  o derive Task da
+00006970: 7461 2e20 452e 672e 2060 5b22 6669 6c65  ta. E.g. `["file
+00006980: 2e63 7376 222c 2022 6669 6c65 5f32 2e63  .csv", "file_2.c
+00006990: 7376 3a32 5d60 2e20 2020 2020 2020 2020  sv:2]`.         
+000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000069f0: 2059 6573 2020 7c20 2020 2020 7c20 2020   Yes  |     |   
+00006a00: 2020 207c 2020 2020 2020 7c0a 7c20 6064     |      |.| `d
+00006a10: 6570 656e 6465 6e74 4f6e 6020 2020 2020  ependentOn`     
+00006a20: 2020 2020 2020 2020 207c 2054 6865 206e           | The n
+00006a30: 616d 6520 6f66 2061 6e6f 7468 6572 2054  ame of another T
+00006a40: 6173 6b20 4772 6f75 7020 7769 7468 696e  ask Group within
+00006a50: 2074 6865 2073 616d 6520 576f 726b 2052   the same Work R
+00006a60: 6571 7569 7265 6d65 6e74 2074 6861 7420  equirement that 
+00006a70: 6d75 7374 2062 6520 7375 6363 6573 7366  must be successf
+00006a80: 756c 6c79 2063 6f6d 706c 6574 6564 2062  ully completed b
+00006a90: 6566 6f72 6520 7468 6520 5461 736b 2047  efore the Task G
+00006aa0: 726f 7570 2069 7320 7374 6172 7465 642e  roup is started.
+00006ab0: 2045 2e67 2e20 6022 7461 736b 5f67 726f   E.g. `"task_gro
+00006ac0: 7570 5f31 2260 2e20 2020 2020 2020 2020  up_1"`.         
+00006ad0: 2020 2020 7c20 2020 2020 207c 2020 2020      |      |    
+00006ae0: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
+00006af0: 0a7c 2060 646f 636b 6572 456e 7669 726f  .| `dockerEnviro
+00006b00: 6e6d 656e 7460 2020 2020 2020 2020 7c20  nment`        | 
+00006b10: 5468 6520 656e 7669 726f 6e6d 656e 7420  The environment 
+00006b20: 746f 2062 6520 7061 7373 6564 2074 6f20  to be passed to 
+00006b30: 6120 446f 636b 6572 2063 6f6e 7461 696e  a Docker contain
+00006b40: 6572 2e20 4f6e 6c79 2075 7365 6420 6279  er. Only used by
+00006b50: 2074 6865 2060 646f 636b 6572 6020 5461   the `docker` Ta
+00006b60: 736b 2054 7970 652e 2045 2e67 2e2c 204a  sk Type. E.g., J
+00006b70: 534f 4e3a 2060 7b22 5641 525f 3122 3a20  SON: `{"VAR_1": 
+00006b80: 2261 6263 227d 602c 2054 4f4d 4c3a 2060  "abc"}`, TOML: `
+00006b90: 7b56 4152 5f31 203d 2022 6162 6322 2c20  {VAR_1 = "abc", 
+00006ba0: 5641 525f 3220 3d20 2264 6566 227d 602e  VAR_2 = "def"}`.
+00006bb0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+00006bc0: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
+00006bd0: 6573 2020 7c0a 7c20 6064 6f63 6b65 7250  es  |.| `dockerP
+00006be0: 6173 7377 6f72 6460 2020 2020 2020 2020  assword`        
+00006bf0: 2020 207c 2054 6865 2070 6173 7377 6f72     | The passwor
+00006c00: 6420 666f 7220 446f 636b 6572 4875 622c  d for DockerHub,
+00006c10: 206f 6e6c 7920 7573 6564 2062 7920 7468   only used by th
+00006c20: 6520 6064 6f63 6b65 7260 2054 6173 6b20  e `docker` Task 
+00006c30: 5479 7065 2e20 452c 672e 2c20 6022 6d79  Type. E,g., `"my
+00006c40: 5f70 6173 7377 6f72 6422 602e 2020 2020  _password"`.    
+00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006ca0: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
+00006cb0: 2020 7c20 5965 7320 207c 0a7c 2060 646f    | Yes  |.| `do
+00006cc0: 636b 6572 5573 6572 6e61 6d65 6020 2020  ckerUsername`   
+00006cd0: 2020 2020 2020 2020 7c20 5468 6520 7573          | The us
+00006ce0: 6572 6e61 6d65 2066 6f72 2044 6f63 6b65  ername for Docke
+00006cf0: 7248 7562 2c20 6f6e 6c79 2075 7365 6420  rHub, only used 
+00006d00: 6279 2074 6865 2060 646f 636b 6572 6020  by the `docker` 
+00006d10: 5461 736b 2054 7970 652e 2045 2c67 2e2c  Task Type. E,g.,
+00006d20: 2060 226d 795f 7573 6572 6e61 6d65 2260   `"my_username"`
+00006d30: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00006d90: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
+00006da0: 7c20 6065 6e76 6972 6f6e 6d65 6e74 6020  | `environment` 
+00006db0: 2020 2020 2020 2020 2020 2020 207c 2054               | T
+00006dc0: 6865 2065 6e76 6972 6f6e 6d65 6e74 2076  he environment v
+00006dd0: 6172 6961 626c 6573 2074 6f20 7365 7420  ariables to set 
+00006de0: 666f 7220 6120 5461 736b 2077 6865 6e20  for a Task when 
+00006df0: 6974 2773 2065 7865 6375 7465 642e 2045  it's executed. E
+00006e00: 2e67 2e2c 204a 534f 4e3a 2060 7b22 5641  .g., JSON: `{"VA
+00006e10: 525f 3122 3a20 2261 6263 222c 2022 5641  R_1": "abc", "VA
+00006e20: 525f 3222 3a20 2264 6566 227d 602c 2054  R_2": "def"}`, T
+00006e30: 4f4d 4c3a 2060 7b56 4152 5f31 203d 2022  OML: `{VAR_1 = "
+00006e40: 6162 6322 2c20 5641 525f 3220 3d20 2264  abc", VAR_2 = "d
+00006e50: 6566 227d 602e 2020 2020 2020 2020 2020  ef"}`.          
+00006e60: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00006e70: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+00006e80: 7320 207c 0a7c 2060 6578 636c 7573 6976  s  |.| `exclusiv
+00006e90: 6557 6f72 6b65 7273 6020 2020 2020 2020  eWorkers`       
+00006ea0: 2020 7c20 4966 2074 7275 652c 2074 6865    | If true, the
+00006eb0: 6e20 646f 206e 6f74 2061 6c6c 6f77 2063  n do not allow c
+00006ec0: 6c61 696d 6564 2057 6f72 6b65 7273 2074  laimed Workers t
+00006ed0: 6f20 6265 2073 6861 7265 6420 7769 7468  o be shared with
+00006ee0: 206f 7468 6572 2054 6173 6b20 4772 6f75   other Task Grou
+00006ef0: 7073 3b20 6f74 6865 7277 6973 652c 2057  ps; otherwise, W
+00006f00: 6f72 6b65 7273 2063 616e 2062 6520 7368  orkers can be sh
+00006f10: 6172 6564 2e20 4465 6661 756c 743a 6066  ared. Default:`f
+00006f20: 616c 7365 602e 2020 2020 2020 2020 2020  alse`.          
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f40: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+00006f50: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+00006f60: 207c 2020 2020 2020 7c0a 7c20 6065 7865   |      |.| `exe
+00006f70: 6375 7461 626c 6560 2020 2020 2020 2020  cutable`        
+00006f80: 2020 2020 2020 207c 2054 6865 2027 6578         | The 'ex
+00006f90: 6563 7574 6162 6c65 2720 746f 2072 756e  ecutable' to run
+00006fa0: 2077 6865 6e20 6120 4261 7368 206f 7220   when a Bash or 
+00006fb0: 446f 636b 6572 2054 6173 6b20 6973 2065  Docker Task is e
+00006fc0: 7865 6375 7465 642e 2042 6173 6820 7363  xecuted. Bash sc
+00006fd0: 7269 7074 2066 6f72 2042 6173 682c 2063  ript for Bash, c
+00006fe0: 6f6e 7461 696e 6572 2069 6d61 6765 2066  ontainer image f
+00006ff0: 6f72 2044 6f63 6b65 722e 204f 7074 696f  or Docker. Optio
+00007000: 6e61 6c3a 206f 6d69 7420 746f 2073 7570  nal: omit to sup
+00007010: 7072 6573 7320 6175 746f 6d61 7469 6320  press automatic 
+00007020: 7072 6f63 6573 7369 6e67 2e20 2020 2020  processing.     
+00007030: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00007040: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
+00007050: 2060 6669 6e69 7368 4966 416c 6c54 6173   `finishIfAllTas
+00007060: 6b73 4669 6e69 7368 6564 6020 7c20 4966  ksFinished` | If
+00007070: 2074 7275 652c 2074 6865 2054 6173 6b20   true, the Task 
+00007080: 4772 6f75 7020 7769 6c6c 2066 696e 6973  Group will finis
+00007090: 6820 6175 746f 6d61 7469 6361 6c6c 7920  h automatically 
+000070a0: 6966 2061 6c6c 2063 6f6e 7461 696e 6564  if all contained
+000070b0: 2074 6173 6b73 2066 696e 6973 682e 2044   tasks finish. D
+000070c0: 6566 6175 6c74 3a60 7472 7565 602e 2020  efault:`true`.  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007110: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00007120: 5965 7320 7c20 5965 7320 207c 2020 2020  Yes | Yes  |    
+00007130: 2020 7c0a 7c20 6066 696e 6973 6849 6641    |.| `finishIfA
+00007140: 6e79 5461 736b 4661 696c 6564 6020 2020  nyTaskFailed`   
+00007150: 207c 2049 6620 7472 7565 2c20 7468 6520   | If true, the 
+00007160: 5461 736b 2047 726f 7570 2077 696c 6c20  Task Group will 
+00007170: 6265 2066 6169 6c65 6420 6175 746f 6d61  be failed automa
+00007180: 7469 6361 6c6c 7920 6966 2061 6e79 2063  tically if any c
+00007190: 6f6e 7461 696e 6564 2074 6173 6b73 2066  ontained tasks f
+000071a0: 6169 6c2e 2044 6566 6175 6c74 3a60 6661  ail. Default:`fa
+000071b0: 6c73 6560 2e20 2020 2020 2020 2020 2020  lse`.           
+000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+00007200: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+00007210: 7c20 2020 2020 207c 0a7c 2060 666c 6174  |      |.| `flat
+00007220: 7465 6e49 6e70 7574 5061 7468 7360 2020  tenInputPaths`  
+00007230: 2020 2020 2020 7c20 4465 7465 726d 696e        | Determin
+00007240: 6573 2077 6865 7468 6572 2069 6e70 7574  es whether input
+00007250: 206f 626a 6563 7420 7061 7468 7320 7368   object paths sh
+00007260: 6f75 6c64 2062 6520 666c 6174 7465 6e65  ould be flattene
+00007270: 6420 2869 2e65 2e2c 2064 6972 6563 746f  d (i.e., directo
+00007280: 7279 2073 7472 7563 7475 7265 2072 656d  ry structure rem
+00007290: 6f76 6564 2920 7768 656e 2064 6f77 6e6c  oved) when downl
+000072a0: 6f61 6465 6420 746f 2061 206e 6f64 652e  oaded to a node.
+000072b0: 2044 6566 6175 6c74 3a20 6066 616c 7365   Default: `false
+000072c0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+000072f0: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
+00007300: 6066 6c61 7474 656e 5570 6c6f 6164 5061  `flattenUploadPa
+00007310: 7468 7360 2020 2020 2020 207c 2049 676e  ths`       | Ign
+00007320: 6f72 6520 6c6f 6361 6c20 6469 7265 6374  ore local direct
+00007330: 6f72 7920 7061 7468 7320 7768 656e 2075  ory paths when u
+00007340: 706c 6f61 6469 6e67 2066 696c 6573 2074  ploading files t
+00007350: 6f20 7468 6520 4f62 6a65 6374 2053 746f  o the Object Sto
+00007360: 7265 3b20 706c 6163 6520 696e 2060 3c6e  re; place in `<n
+00007370: 616d 6573 7061 6365 3e3a 3c77 6f72 6b2d  amespace>:<work-
+00007380: 7265 712d 6e61 6d65 3e2f 602e 2044 6566  req-name>/`. Def
+00007390: 6175 6c74 3a20 6066 616c 7365 602e 2020  ault: `false`.  
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+000073d0: 6573 207c 2020 2020 2020 7c20 2020 2020  es |      |     
+000073e0: 207c 0a7c 2060 6675 6c66 696c 4f6e 5375   |.| `fulfilOnSu
+000073f0: 626d 6974 6020 2020 2020 2020 2020 2020  bmit`           
+00007400: 7c20 496e 6469 6361 7465 7320 6966 2074  | Indicates if t
+00007410: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+00007420: 656e 7420 7368 6f75 6c64 2062 6520 6675  ent should be fu
+00007430: 6c66 696c 6c65 6420 7768 656e 2069 7420  lfilled when it 
+00007440: 6973 2073 7562 6d69 7474 6564 2c20 7261  is submitted, ra
+00007450: 7468 6572 2074 6861 6e20 6265 696e 6720  ther than being 
+00007460: 616c 6c6f 7765 6420 746f 2077 6169 7420  allowed to wait 
+00007470: 696e 2050 454e 4449 4e47 2073 7461 7475  in PENDING statu
+00007480: 732e 2044 6566 6175 6c74 3a60 6661 6c73  s. Default:`fals
+00007490: 6560 2e20 2020 2020 2020 2020 2020 2020  e`.             
+000074a0: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+000074b0: 2020 7c20 5965 7320 7c20 2020 2020 207c    | Yes |      |
+000074c0: 2020 2020 2020 7c0a 7c20 6069 6e70 7574        |.| `input
+000074d0: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
+000074e0: 2020 2020 207c 2054 6865 206c 6973 7420       | The list 
+000074f0: 6f66 2069 6e70 7574 2066 696c 6573 2074  of input files t
+00007500: 6f20 6265 2075 706c 6f61 6465 6420 746f  o be uploaded to
+00007510: 2074 6865 2059 656c 6c6f 7744 6f67 204f   the YellowDog O
+00007520: 626a 6563 7420 5374 6f72 652c 2061 6e64  bject Store, and
+00007530: 2072 6571 7569 7265 6420 6279 2074 6865   required by the
+00007540: 2054 6173 6b20 2869 6d70 6c69 6573 2060   Task (implies `
+00007550: 7665 7269 6679 4174 5374 6172 7460 292e  verifyAtStart`).
+00007560: 2045 2e67 2e20 605b 2261 2e73 6822 2c20   E.g. `["a.sh", 
+00007570: 2262 2e73 6822 5d60 206f 7220 605b 222a  "b.sh"]` or `["*
+00007580: 2e73 6822 5d60 2e20 2020 2020 2020 2020  .sh"]`.         
+00007590: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+000075a0: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+000075b0: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
+000075c0: 2020 2020 2020 2020 2020 7c20 4120 6c69            | A li
+000075d0: 7374 206f 6620 696e 7075 7420 6669 6c65  st of input file
+000075e0: 7320 7265 7175 6972 6564 2062 7920 6120  s required by a 
+000075f0: 5461 736b 2c20 6275 7420 7768 6963 6820  Task, but which 
+00007600: 6172 6520 6e6f 7420 7375 626a 6563 7420  are not subject 
+00007610: 746f 2076 6572 6966 6963 6174 696f 6e2e  to verification.
+00007620: 2043 616e 2063 6f6e 7461 696e 2077 696c   Can contain wil
+00007630: 6463 6172 6473 2e20 452e 672e 3a20 605b  dcards. E.g.: `[
+00007640: 2274 6173 6b5f 6772 6f75 705f 312f 2a2a  "task_group_1/**
+00007650: 2f72 6573 756c 7473 2e74 7874 225d 602e  /results.txt"]`.
+00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007670: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00007680: 7320 7c20 5965 7320 207c 2059 6573 2020  s | Yes  | Yes  
+00007690: 7c0a 7c20 6069 6e73 7461 6e63 6554 7970  |.| `instanceTyp
+000076a0: 6573 6020 2020 2020 2020 2020 2020 207c  es`            |
+000076b0: 2054 6865 206d 6163 6869 6e65 2069 6e73   The machine ins
+000076c0: 7461 6e63 6520 7479 7065 7320 7468 6174  tance types that
+000076d0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+000076e0: 6578 6563 7574 6520 5461 736b 732e 2045  execute Tasks. E
+000076f0: 2e67 2e2c 2060 5b22 7433 2e6d 6963 726f  .g., `["t3.micro
+00007700: 222c 2022 7433 612e 6d69 6372 6f22 5d60  ", "t3a.micro"]`
+00007710: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+00007760: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
+00007770: 2020 2020 207c 0a7c 2060 6d61 7869 6d75       |.| `maximu
+00007780: 6d54 6173 6b52 6574 7269 6573 6020 2020  mTaskRetries`   
+00007790: 2020 2020 7c20 5468 6520 6d61 7869 6d75      | The maximu
+000077a0: 6d20 6e75 6d62 6572 206f 6620 7469 6d65  m number of time
+000077b0: 7320 6120 5461 736b 2063 616e 2062 6520  s a Task can be 
+000077c0: 7265 7472 6965 6420 6166 7465 7220 6974  retried after it
+000077d0: 2068 6173 2066 6169 6c65 642e 2045 2e67   has failed. E.g
+000077e0: 2e3a 2060 3560 2e20 2020 2020 2020 2020  .: `5`.         
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007830: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007840: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
+00007850: 7320 207c 2020 2020 2020 7c0a 7c20 606d  s  |      |.| `m
+00007860: 6178 576f 726b 6572 7360 2020 2020 2020  axWorkers`      
+00007870: 2020 2020 2020 2020 207c 2054 6865 206d           | The m
+00007880: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00007890: 2057 6f72 6b65 7273 2074 6861 7420 6361   Workers that ca
+000078a0: 6e20 6265 2063 6c61 696d 6564 2066 6f72  n be claimed for
+000078b0: 2074 6865 2061 7373 6f63 6961 7465 6420   the associated 
+000078c0: 5461 736b 2047 726f 7570 2e20 452e 672e  Task Group. E.g.
+000078d0: 2c20 6031 3060 2e20 2020 2020 2020 2020  , `10`.         
+000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+00007930: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
+00007940: 0a7c 2060 6d69 6e57 6f72 6b65 7273 6020  .| `minWorkers` 
+00007950: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007960: 5468 6520 6d69 6e69 6d75 6d20 6e75 6d62  The minimum numb
+00007970: 6572 206f 6620 576f 726b 6572 7320 7468  er of Workers th
+00007980: 6174 2074 6865 2061 7373 6f63 6961 7465  at the associate
+00007990: 6420 5461 736b 2047 726f 7570 2072 6571  d Task Group req
+000079a0: 7569 7265 732e 2054 6869 7320 6d61 6e79  uires. This many
+000079b0: 2077 6f72 6b65 7273 206d 7573 7420 6265   workers must be
+000079c0: 2063 6c61 696d 6564 2062 6566 6f72 6520   claimed before 
+000079d0: 7468 6520 6173 736f 6369 6174 6564 2054  the associated T
+000079e0: 6173 6b20 4772 6f75 7020 7769 6c6c 2073  ask Group will s
+000079f0: 7461 7274 2077 6f72 6b69 6e67 2e20 452e  tart working. E.
+00007a00: 672e 2c20 6031 602e 207c 2059 6573 2020  g., `1`. | Yes  
+00007a10: 7c20 5965 7320 7c20 5965 7320 207c 2020  | Yes | Yes  |  
+00007a20: 2020 2020 7c0a 7c20 606e 616d 6560 2020      |.| `name`  
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 207c 2054 6865 206e 616d 6520 6f66     | The name of
+00007a50: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+00007a60: 656d 656e 742c 2054 6173 6b20 4772 6f75  ement, Task Grou
+00007a70: 7020 6f72 2054 6173 6b2e 2045 2e67 2e2c  p or Task. E.g.,
+00007a80: 2060 2277 725f 6e61 6d65 2260 2e20 4e6f   `"wr_name"`. No
+00007a90: 7465 2074 6861 7420 7468 6520 606e 616d  te that the `nam
+00007aa0: 6560 2070 726f 7065 7274 7920 6973 206e  e` property is n
+00007ab0: 6f74 2069 6e68 6572 6974 6564 2e20 2020  ot inherited.   
 00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 7c20 5468 6520 6669 6c65 7320 746f 2062  | The files to b
-00007ae0: 6520 7570 6c6f 6164 6564 2074 6f20 7468  e uploaded to th
-00007af0: 6520 5965 6c6c 6f77 446f 6720 4f62 6a65  e YellowDog Obje
-00007b00: 6374 2053 746f 7265 2062 7920 6120 576f  ct Store by a Wo
-00007b10: 726b 6572 206e 6f64 6520 6f6e 2063 6f6d  rker node on com
-00007b20: 706c 6574 696f 6e20 6f66 2074 6865 2054  pletion of the T
-00007b30: 6173 6b2e 2045 2e67 2e2c 2060 5b22 7265  ask. E.g., `["re
-00007b40: 7375 6c74 735f 312e 7478 7422 2c20 2272  sults_1.txt", "r
-00007b50: 6573 756c 7473 5f32 2e74 7874 225d 602e  esults_2.txt"]`.
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00007b80: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00007b90: 2059 6573 2020 7c0a 7c20 606f 7574 7075   Yes  |.| `outpu
-00007ba0: 7473 5265 7175 6972 6564 6020 2020 2020  tsRequired`     
-00007bb0: 2020 2020 207c 2054 6865 2066 696c 6573       | The files
-00007bc0: 2074 6861 7420 2a6d 7573 742a 2062 6520   that *must* be 
-00007bd0: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
-00007be0: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
-00007bf0: 2053 746f 7265 2062 7920 6120 576f 726b   Store by a Work
-00007c00: 6572 206e 6f64 6520 6f6e 2063 6f6d 706c  er node on compl
-00007c10: 6574 696f 6e20 6f66 2074 6865 2054 6173  etion of the Tas
-00007c20: 6b2e 2054 6865 2054 6173 6b20 7769 6c6c  k. The Task will
-00007c30: 2066 6169 6c20 6966 2061 6e79 206f 7574   fail if any out
-00007c40: 7075 7473 2061 7265 2075 6e61 7661 696c  puts are unavail
-00007c50: 6162 6c65 2e20 2020 2020 2020 2020 2020  able.           
-00007c60: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00007c70: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
-00007c80: 7072 696f 7269 7479 6020 2020 2020 2020  priority`       
-00007c90: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
-00007ca0: 7072 696f 7269 7479 206f 6620 576f 726b  priority of Work
-00007cb0: 2052 6571 7569 7265 6d65 6e74 7320 616e   Requirements an
-00007cc0: 6420 5461 736b 2047 726f 7570 732e 2048  d Task Groups. H
-00007cd0: 6967 6865 7220 7072 696f 7269 7479 2061  igher priority a
-00007ce0: 6371 7569 7265 7320 576f 726b 6572 7320  cquires Workers 
-00007cf0: 6168 6561 6420 6f66 206c 6f77 6572 2070  ahead of lower p
-00007d00: 7269 6f72 6974 792e 2045 2e67 2e2c 2060  riority. E.g., `
-00007d10: 302e 3060 2e20 2020 2020 2020 2020 2020  0.0`.           
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-00007d50: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
-00007d60: 7c0a 7c20 6070 726f 7669 6465 7273 6020  |.| `providers` 
-00007d70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007d80: 2043 6f6e 7374 7261 696e 7320 7468 6520   Constrains the 
-00007d90: 5965 6c6c 6f77 446f 6720 5363 6865 6475  YellowDog Schedu
-00007da0: 6c65 7220 6f6e 6c79 2074 6f20 6578 6563  ler only to exec
-00007db0: 7574 6520 7461 736b 7320 6672 6f6d 2074  ute tasks from t
-00007dc0: 6865 2061 7373 6f63 6961 7465 6420 5461  he associated Ta
-00007dd0: 736b 2047 726f 7570 206f 6e20 7468 6520  sk Group on the 
-00007de0: 7370 6563 6966 6965 6420 7072 6f76 6964  specified provid
-00007df0: 6572 732e 2045 2e67 2e2c 2060 5b22 4157  ers. E.g., `["AW
-00007e00: 5322 2c20 2247 4f4f 474c 4522 5d60 2e20  S", "GOOGLE"]`. 
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-00007e30: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
-00007e40: 2020 2020 207c 0a7c 2060 7261 6d60 2020       |.| `ram`  
-00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 7c20 5261 6e67 6520 636f 6e73      | Range cons
-00007e70: 7472 6169 6e74 206f 6e20 4742 206f 6620  traint on GB of 
-00007e80: 5241 4d20 7468 6174 2061 7265 2072 6571  RAM that are req
-00007e90: 7569 7265 6420 746f 2065 7865 6375 7465  uired to execute
-00007ea0: 2054 6173 6b73 2e20 452e 672e 2c20 605b   Tasks. E.g., `[
-00007eb0: 322e 352c 2034 2e30 5d60 2e20 2020 2020  2.5, 4.0]`.     
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007f10: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
-00007f20: 7320 207c 2020 2020 2020 7c0a 7c20 6072  s  |      |.| `r
-00007f30: 6567 696f 6e73 6020 2020 2020 2020 2020  egions`         
-00007f40: 2020 2020 2020 2020 207c 2043 6f6e 7374           | Const
-00007f50: 7261 696e 7320 7468 6520 5965 6c6c 6f77  rains the Yellow
-00007f60: 446f 6720 5363 6865 6475 6c65 7220 6f6e  Dog Scheduler on
-00007f70: 6c79 2074 6f20 6578 6563 7574 6520 5461  ly to execute Ta
-00007f80: 736b 7320 6672 6f6d 2074 6865 2061 7373  sks from the ass
-00007f90: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
-00007fa0: 7570 2069 6e20 7468 6520 7370 6563 6966  up in the specif
-00007fb0: 6965 6420 7265 6769 6f6e 732e 2045 2e67  ied regions. E.g
-00007fc0: 2e2c 2060 5b22 6575 2d77 6573 742d 325d  ., `["eu-west-2]
-00007fd0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
-00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-00008000: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
-00008010: 0a7c 2060 7461 736b 4261 7463 6853 697a  .| `taskBatchSiz
-00008020: 6560 2020 2020 2020 2020 2020 2020 7c20  e`            | 
-00008030: 4465 7465 726d 696e 6573 2074 6865 2062  Determines the b
-00008040: 6174 6368 2073 697a 6520 7573 6564 2074  atch size used t
-00008050: 6f20 6164 6420 5461 736b 7320 746f 2054  o add Tasks to T
-00008060: 6173 6b20 4772 6f75 7073 2e20 4465 6661  ask Groups. Defa
-00008070: 756c 7420 6973 2032 2c30 3030 2e20 2020  ult is 2,000.   
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-000080e0: 7c20 2020 2020 7c20 2020 2020 207c 2020  |     |      |  
-000080f0: 2020 2020 7c0a 7c20 6074 6173 6b43 6f75      |.| `taskCou
-00008100: 6e74 6020 2020 2020 2020 2020 2020 2020  nt`             
-00008110: 2020 207c 2054 6865 206e 756d 6265 7220     | The number 
-00008120: 6f66 2074 696d 6573 2074 6f20 6578 6563  of times to exec
-00008130: 7574 6520 7468 6520 5461 736b 2e20 4361  ute the Task. Ca
-00008140: 6e20 6265 2073 6574 2069 6e20 7468 6520  n be set in the 
-00008150: 544f 4d4c 2066 696c 6520 6f72 2069 6e20  TOML file or in 
-00008160: 616e 7920 4a53 4f4e 2054 6173 6b20 4772  any JSON Task Gr
-00008170: 6f75 7020 6465 6669 6e69 7469 6f6e 2e20  oup definition. 
-00008180: 4e6f 7465 3a20 6e6f 2069 6e68 6572 6974  Note: no inherit
-00008190: 616e 6365 2066 726f 6d20 544f 4d4c 2074  ance from TOML t
-000081a0: 6f20 4a53 4f4e 2e20 2020 2020 2020 2020  o JSON.         
-000081b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000081c0: 5965 7320 207c 2020 2020 207c 2059 6573  Yes  |     | Yes
-000081d0: 2020 7c20 2020 2020 207c 0a7c 2060 7461    |      |.| `ta
-000081e0: 736b 4461 7461 6020 2020 2020 2020 2020  skData`         
-000081f0: 2020 2020 2020 2020 7c20 5468 6520 6461          | The da
-00008200: 7461 2074 6f20 6265 2070 6173 7365 6420  ta to be passed 
-00008210: 746f 2074 6865 2057 6f72 6b65 7220 7768  to the Worker wh
-00008220: 656e 2074 6865 2054 6173 6b20 6973 2073  en the Task is s
-00008230: 7461 7274 6564 2e20 452e 672e 2c20 6022  tarted. E.g., `"
-00008240: 6d79 6461 7461 2260 2e20 4265 636f 6d65  mydata"`. Become
-00008250: 7320 6669 6c65 2060 7461 736b 6461 7461  s file `taskdata
-00008260: 2e74 7874 6020 696e 2074 6865 2054 6173  .txt` in the Tas
-00008270: 6b27 7320 776f 726b 696e 6720 6469 7265  k's working dire
-00008280: 6374 6f72 7920 7768 656e 2054 6865 2054  ctory when The T
-00008290: 6173 6b20 6578 6563 7574 6573 2e20 2020  ask executes.   
-000082a0: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-000082b0: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
-000082c0: 7c20 6074 6173 6b44 6174 6146 696c 6560  | `taskDataFile`
-000082d0: 2020 2020 2020 2020 2020 2020 207c 2050               | P
-000082e0: 6f70 756c 6174 6520 7468 6520 6074 6173  opulate the `tas
-000082f0: 6b44 6174 6160 2070 726f 7065 7274 7920  kData` property 
-00008300: 6162 6f76 6520 7769 7468 2074 6865 2063  above with the c
-00008310: 6f6e 7465 6e74 7320 6f66 2074 6865 2073  ontents of the s
-00008320: 7065 6369 6669 6564 2066 696c 652e 2045  pecified file. E
-00008330: 2e67 2e2c 2060 226d 795f 7461 736b 5f64  .g., `"my_task_d
-00008340: 6174 615f 6669 6c65 2e74 7874 2260 2e20  ata_file.txt"`. 
-00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-00008390: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
-000083a0: 7320 207c 0a7c 2060 7461 736b 4e61 6d65  s  |.| `taskName
-000083b0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-000083c0: 2020 7c20 5468 6520 6e61 6d65 2074 6f20    | The name to 
-000083d0: 7573 6520 666f 7220 7468 6520 5461 736b  use for the Task
-000083e0: 2e20 4f6e 6c79 2075 7361 626c 6520 696e  . Only usable in
-000083f0: 2074 6865 2054 4f4d 4c20 6669 6c65 2e20   the TOML file. 
-00008400: 4d6f 7374 6c79 2075 7365 6675 6c20 696e  Mostly useful in
-00008410: 2063 6f6e 6a75 6e63 7469 6f6e 2077 6974   conjunction wit
-00008420: 6820 4353 5620 5461 736b 2064 6174 612e  h CSV Task data.
-00008430: 2045 2e67 2e2c 2060 226d 795f 7461 736b   E.g., `"my_task
-00008440: 5f6e 756d 6265 725f 7b7b 7461 736b 5f6e  _number_{{task_n
-00008450: 756d 6265 727d 7d22 602e 2020 2020 2020  umber}}"`.      
-00008460: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-00008470: 6573 2020 7c20 2020 2020 7c20 2020 2020  es  |     |     
-00008480: 207c 2020 2020 2020 7c0a 7c20 6074 6173   |      |.| `tas
-00008490: 6b47 726f 7570 4e61 6d65 6020 2020 2020  kGroupName`     
-000084a0: 2020 2020 2020 207c 2054 6865 206e 616d         | The nam
-000084b0: 6520 746f 2075 7365 2066 6f72 2074 6865  e to use for the
-000084c0: 2054 6173 6b20 4772 6f75 702e 204f 6e6c   Task Group. Onl
-000084d0: 7920 7573 6162 6c65 2069 6e20 7468 6520  y usable in the 
-000084e0: 544f 4d4c 2066 696c 652e 2045 2e67 2e2c  TOML file. E.g.,
-000084f0: 2060 226d 795f 7467 5f6e 756d 6265 725f   `"my_tg_number_
-00008500: 7b7b 7461 736b 5f67 726f 7570 5f6e 756d  {{task_group_num
-00008510: 6265 727d 7d22 602e 2020 2020 2020 2020  ber}}"`.        
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 7c20 5965 7320 207c 2020 2020 207c    | Yes  |     |
-00008560: 2020 2020 2020 7c20 2020 2020 207c 0a7c        |      |.|
-00008570: 2060 7461 736b 5479 7065 6020 2020 2020   `taskType`     
-00008580: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-00008590: 6520 5461 736b 2054 7970 6520 6f66 2061  e Task Type of a
-000085a0: 2054 6173 6b2e 2045 2e67 2e2c 2060 2264   Task. E.g., `"d
-000085b0: 6f63 6b65 7222 602e 2020 2020 2020 2020  ocker"`.        
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007af0: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
+00007b00: 2020 7c20 5965 7320 207c 0a7c 2060 6f75    | Yes  |.| `ou
+00007b10: 7470 7574 7360 2020 2020 2020 2020 2020  tputs`          
+00007b20: 2020 2020 2020 2020 7c20 5468 6520 6669          | The fi
+00007b30: 6c65 7320 746f 2062 6520 7570 6c6f 6164  les to be upload
+00007b40: 6564 2074 6f20 7468 6520 5965 6c6c 6f77  ed to the Yellow
+00007b50: 446f 6720 4f62 6a65 6374 2053 746f 7265  Dog Object Store
+00007b60: 2062 7920 6120 576f 726b 6572 206e 6f64   by a Worker nod
+00007b70: 6520 6f6e 2063 6f6d 706c 6574 696f 6e20  e on completion 
+00007b80: 6f66 2074 6865 2054 6173 6b2e 2045 2e67  of the Task. E.g
+00007b90: 2e2c 2060 5b22 7265 7375 6c74 735f 312e  ., `["results_1.
+00007ba0: 7478 7422 2c20 2272 6573 756c 7473 5f32  txt", "results_2
+00007bb0: 2e74 7874 225d 602e 2020 2020 2020 2020  .txt"]`.        
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00007be0: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
+00007bf0: 7c20 606f 7574 7075 7473 5265 7175 6972  | `outputsRequir
+00007c00: 6564 6020 2020 2020 2020 2020 207c 2054  ed`          | T
+00007c10: 6865 2066 696c 6573 2074 6861 7420 2a6d  he files that *m
+00007c20: 7573 742a 2062 6520 7570 6c6f 6164 6564  ust* be uploaded
+00007c30: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
+00007c40: 6720 4f62 6a65 6374 2053 746f 7265 2062  g Object Store b
+00007c50: 7920 6120 576f 726b 6572 206e 6f64 6520  y a Worker node 
+00007c60: 6f6e 2063 6f6d 706c 6574 696f 6e20 6f66  on completion of
+00007c70: 2074 6865 2054 6173 6b2e 2054 6865 2054   the Task. The T
+00007c80: 6173 6b20 7769 6c6c 2066 6169 6c20 6966  ask will fail if
+00007c90: 2061 6e79 206f 7574 7075 7473 2061 7265   any outputs are
+00007ca0: 2075 6e61 7661 696c 6162 6c65 2e20 2020   unavailable.   
+00007cb0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00007cc0: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+00007cd0: 7320 207c 0a7c 2060 7072 696f 7269 7479  s  |.| `priority
+00007ce0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00007cf0: 2020 7c20 5468 6520 7072 696f 7269 7479    | The priority
+00007d00: 206f 6620 576f 726b 2052 6571 7569 7265   of Work Require
+00007d10: 6d65 6e74 7320 616e 6420 5461 736b 2047  ments and Task G
+00007d20: 726f 7570 732e 2048 6967 6865 7220 7072  roups. Higher pr
+00007d30: 696f 7269 7479 2061 6371 7569 7265 7320  iority acquires 
+00007d40: 576f 726b 6572 7320 6168 6561 6420 6f66  Workers ahead of
+00007d50: 206c 6f77 6572 2070 7269 6f72 6974 792e   lower priority.
+00007d60: 2045 2e67 2e2c 2060 302e 3060 2e20 2020   E.g., `0.0`.   
+00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d90: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+00007da0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+00007db0: 207c 2020 2020 2020 7c0a 7c20 6070 726f   |      |.| `pro
+00007dc0: 7669 6465 7273 6020 2020 2020 2020 2020  viders`         
+00007dd0: 2020 2020 2020 207c 2043 6f6e 7374 7261         | Constra
+00007de0: 696e 7320 7468 6520 5965 6c6c 6f77 446f  ins the YellowDo
+00007df0: 6720 5363 6865 6475 6c65 7220 6f6e 6c79  g Scheduler only
+00007e00: 2074 6f20 6578 6563 7574 6520 7461 736b   to execute task
+00007e10: 7320 6672 6f6d 2074 6865 2061 7373 6f63  s from the assoc
+00007e20: 6961 7465 6420 5461 736b 2047 726f 7570  iated Task Group
+00007e30: 206f 6e20 7468 6520 7370 6563 6966 6965   on the specifie
+00007e40: 6420 7072 6f76 6964 6572 732e 2045 2e67  d providers. E.g
+00007e50: 2e2c 2060 5b22 4157 5322 2c20 2247 4f4f  ., `["AWS", "GOO
+00007e60: 474c 4522 5d60 2e20 2020 2020 2020 2020  GLE"]`.         
+00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e80: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00007e90: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
+00007ea0: 2060 7261 6d60 2020 2020 2020 2020 2020   `ram`          
+00007eb0: 2020 2020 2020 2020 2020 2020 7c20 5261              | Ra
+00007ec0: 6e67 6520 636f 6e73 7472 6169 6e74 206f  nge constraint o
+00007ed0: 6e20 4742 206f 6620 5241 4d20 7468 6174  n GB of RAM that
+00007ee0: 2061 7265 2072 6571 7569 7265 6420 746f   are required to
+00007ef0: 2065 7865 6375 7465 2054 6173 6b73 2e20   execute Tasks. 
+00007f00: 452e 672e 2c20 605b 322e 352c 2034 2e30  E.g., `[2.5, 4.0
+00007f10: 5d60 2e20 2020 2020 2020 2020 2020 2020  ]`.             
+00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00007f70: 5965 7320 7c20 5965 7320 207c 2020 2020  Yes | Yes  |    
+00007f80: 2020 7c0a 7c20 6072 6567 696f 6e73 6020    |.| `regions` 
+00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 207c 2043 6f6e 7374 7261 696e 7320 7468   | Constrains th
+00007fb0: 6520 5965 6c6c 6f77 446f 6720 5363 6865  e YellowDog Sche
+00007fc0: 6475 6c65 7220 6f6e 6c79 2074 6f20 6578  duler only to ex
+00007fd0: 6563 7574 6520 5461 736b 7320 6672 6f6d  ecute Tasks from
+00007fe0: 2074 6865 2061 7373 6f63 6961 7465 6420   the associated 
+00007ff0: 5461 736b 2047 726f 7570 2069 6e20 7468  Task Group in th
+00008000: 6520 7370 6563 6966 6965 6420 7265 6769  e specified regi
+00008010: 6f6e 732e 2045 2e67 2e2c 2060 5b22 6575  ons. E.g., `["eu
+00008020: 2d77 6573 742d 325d 602e 2020 2020 2020  -west-2]`.      
+00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+00008050: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+00008060: 7c20 2020 2020 207c 0a7c 2060 7461 736b  |      |.| `task
+00008070: 4261 7463 6853 697a 6560 2020 2020 2020  BatchSize`      
+00008080: 2020 2020 2020 7c20 4465 7465 726d 696e        | Determin
+00008090: 6573 2074 6865 2062 6174 6368 2073 697a  es the batch siz
+000080a0: 6520 7573 6564 2074 6f20 6164 6420 5461  e used to add Ta
+000080b0: 736b 7320 746f 2054 6173 6b20 4772 6f75  sks to Task Grou
+000080c0: 7073 2e20 4465 6661 756c 7420 6973 2032  ps. Default is 2
+000080d0: 2c30 3030 2e20 2020 2020 2020 2020 2020  ,000.           
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 207c 2059 6573 2020 7c20 2020 2020 7c20   | Yes  |     | 
+00008140: 2020 2020 207c 2020 2020 2020 7c0a 7c20       |      |.| 
+00008150: 6074 6173 6b43 6f75 6e74 6020 2020 2020  `taskCount`     
+00008160: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+00008170: 206e 756d 6265 7220 6f66 2074 696d 6573   number of times
+00008180: 2074 6f20 6578 6563 7574 6520 7468 6520   to execute the 
+00008190: 5461 736b 2e20 4361 6e20 6265 2073 6574  Task. Can be set
+000081a0: 2069 6e20 7468 6520 544f 4d4c 2066 696c   in the TOML fil
+000081b0: 6520 6f72 2069 6e20 616e 7920 4a53 4f4e  e or in any JSON
+000081c0: 2054 6173 6b20 4772 6f75 7020 6465 6669   Task Group defi
+000081d0: 6e69 7469 6f6e 2e20 4e6f 7465 3a20 6e6f  nition. Note: no
+000081e0: 2069 6e68 6572 6974 616e 6365 2066 726f   inheritance fro
+000081f0: 6d20 544f 4d4c 2074 6f20 4a53 4f4e 2e20  m TOML to JSON. 
+00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008210: 2020 2020 2020 7c20 5965 7320 207c 2020        | Yes  |  
+00008220: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
+00008230: 207c 0a7c 2060 7461 736b 4461 7461 6020   |.| `taskData` 
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 7c20 5468 6520 6461 7461 2074 6f20 6265  | The data to be
+00008260: 2070 6173 7365 6420 746f 2074 6865 2057   passed to the W
+00008270: 6f72 6b65 7220 7768 656e 2074 6865 2054  orker when the T
+00008280: 6173 6b20 6973 2073 7461 7274 6564 2e20  ask is started. 
+00008290: 452e 672e 2c20 6022 6d79 6461 7461 2260  E.g., `"mydata"`
+000082a0: 2e20 4265 636f 6d65 7320 6669 6c65 2060  . Becomes file `
+000082b0: 7461 736b 6461 7461 2e74 7874 6020 696e  taskdata.txt` in
+000082c0: 2074 6865 2054 6173 6b27 7320 776f 726b   the Task's work
+000082d0: 696e 6720 6469 7265 6374 6f72 7920 7768  ing directory wh
+000082e0: 656e 2054 6865 2054 6173 6b20 6578 6563  en The Task exec
+000082f0: 7574 6573 2e20 2020 2020 207c 2059 6573  utes.      | Yes
+00008300: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00008310: 2059 6573 2020 7c0a 7c20 6074 6173 6b44   Yes  |.| `taskD
+00008320: 6174 6146 696c 6560 2020 2020 2020 2020  ataFile`        
+00008330: 2020 2020 207c 2050 6f70 756c 6174 6520       | Populate 
+00008340: 7468 6520 6074 6173 6b44 6174 6160 2070  the `taskData` p
+00008350: 726f 7065 7274 7920 6162 6f76 6520 7769  roperty above wi
+00008360: 7468 2074 6865 2063 6f6e 7465 6e74 7320  th the contents 
+00008370: 6f66 2074 6865 2073 7065 6369 6669 6564  of the specified
+00008380: 2066 696c 652e 2045 2e67 2e2c 2060 226d   file. E.g., `"m
+00008390: 795f 7461 736b 5f64 6174 615f 6669 6c65  y_task_data_file
+000083a0: 2e74 7874 2260 2e20 2020 2020 2020 2020  .txt"`.         
+000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+000083f0: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+00008400: 7461 736b 4e61 6d65 6020 2020 2020 2020  taskName`       
+00008410: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
+00008420: 6e61 6d65 2074 6f20 7573 6520 666f 7220  name to use for 
+00008430: 7468 6520 5461 736b 2e20 4f6e 6c79 2075  the Task. Only u
+00008440: 7361 626c 6520 696e 2074 6865 2054 4f4d  sable in the TOM
+00008450: 4c20 6669 6c65 2e20 4d6f 7374 6c79 2075  L file. Mostly u
+00008460: 7365 6675 6c20 696e 2063 6f6e 6a75 6e63  seful in conjunc
+00008470: 7469 6f6e 2077 6974 6820 4353 5620 5461  tion with CSV Ta
+00008480: 736b 2064 6174 612e 2045 2e67 2e2c 2060  sk data. E.g., `
+00008490: 226d 795f 7461 736b 5f6e 756d 6265 725f  "my_task_number_
+000084a0: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
+000084b0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+000084c0: 2020 2020 207c 2059 6573 2020 7c20 2020       | Yes  |   
+000084d0: 2020 7c20 2020 2020 207c 2020 2020 2020    |      |      
+000084e0: 7c0a 7c20 6074 6173 6b47 726f 7570 4e61  |.| `taskGroupNa
+000084f0: 6d65 6020 2020 2020 2020 2020 2020 207c  me`            |
+00008500: 2054 6865 206e 616d 6520 746f 2075 7365   The name to use
+00008510: 2066 6f72 2074 6865 2054 6173 6b20 4772   for the Task Gr
+00008520: 6f75 702e 204f 6e6c 7920 7573 6162 6c65  oup. Only usable
+00008530: 2069 6e20 7468 6520 544f 4d4c 2066 696c   in the TOML fil
+00008540: 652e 2045 2e67 2e2c 2060 226d 795f 7467  e. E.g., `"my_tg
+00008550: 5f6e 756d 6265 725f 7b7b 7461 736b 5f67  _number_{{task_g
+00008560: 726f 7570 5f6e 756d 6265 727d 7d22 602e  roup_number}}"`.
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085a0: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+000085b0: 207c 2020 2020 207c 2020 2020 2020 7c20   |     |      | 
+000085c0: 2020 2020 207c 0a7c 2060 7461 736b 5479       |.| `taskTy
+000085d0: 7065 6020 2020 2020 2020 2020 2020 2020  pe`             
+000085e0: 2020 2020 7c20 5468 6520 5461 736b 2054      | The Task T
+000085f0: 7970 6520 6f66 2061 2054 6173 6b2e 2045  ype of a Task. E
+00008600: 2e67 2e2c 2060 2264 6f63 6b65 7222 602e  .g., `"docker"`.
 00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00008640: 2020 2020 7c20 2020 2020 207c 2059 6573      |      | Yes
-00008650: 2020 7c0a 7c20 6074 6173 6b54 7970 6573    |.| `taskTypes
-00008660: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00008670: 207c 2054 6865 206c 6973 7420 6f66 2054   | The list of T
-00008680: 6173 6b20 5479 7065 7320 7265 7175 6972  ask Types requir
-00008690: 6564 2062 7920 7468 6520 7261 6e67 6520  ed by the range 
-000086a0: 6f66 2054 6173 6b73 2069 6e20 6120 5461  of Tasks in a Ta
-000086b0: 736b 2047 726f 7570 2e20 452e 672e 2c20  sk Group. E.g., 
-000086c0: 605b 2264 6f63 6b65 7222 2c20 6261 7368  `["docker", bash
-000086d0: 225d 602e 2020 2020 2020 2020 2020 2020  "]`.            
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00008720: 2020 207c 2059 6573 207c 2059 6573 2020     | Yes | Yes  
-00008730: 7c20 2020 2020 207c 0a7c 2060 7461 736b  |      |.| `task
-00008740: 7350 6572 576f 726b 6572 6020 2020 2020  sPerWorker`     
-00008750: 2020 2020 2020 7c20 4465 7465 726d 696e        | Determin
-00008760: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-00008770: 2057 6f72 6b65 7220 636c 6169 6d73 2062   Worker claims b
-00008780: 6173 6564 206f 6e20 7370 6c69 7474 696e  ased on splittin
-00008790: 6720 7468 6520 6e75 6d62 6572 206f 6620  g the number of 
-000087a0: 756e 6669 6e69 7368 6564 2054 6173 6b73  unfinished Tasks
-000087b0: 2061 6372 6f73 7320 576f 726b 6572 732e   across Workers.
-000087c0: 2045 2e67 2e2c 2060 3160 2e20 2020 2020   E.g., `1`.     
-000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00008810: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
-00008820: 6075 706c 6f61 6446 696c 6573 6020 2020  `uploadFiles`   
-00008830: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00008840: 206c 6973 7420 6f66 2066 696c 6573 2074   list of files t
-00008850: 6f20 6265 2075 706c 6f61 6465 6420 746f  o be uploaded to
-00008860: 2074 6865 2059 656c 6c6f 7744 6f67 204f   the YellowDog O
-00008870: 626a 6563 7420 5374 6f72 652e 2045 2e67  bject Store. E.g
-00008880: 2e2c 2028 4a53 4f4e 293a 2060 5b7b 226c  ., (JSON): `[{"l
-00008890: 6f63 616c 5061 7468 223a 2066 696c 655f  ocalPath": file_
-000088a0: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
-000088b0: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
-000088c0: 7422 7d5d 602e 2020 2020 2020 2020 2020  t"}]`.          
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-000088f0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
-00008900: 207c 0a7c 2060 7663 7075 7360 2020 2020   |.| `vcpus`    
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 7c20 5261 6e67 6520 636f 6e73 7472 6169  | Range constrai
-00008930: 6e74 206f 6e20 6e75 6d62 6572 206f 6620  nt on number of 
-00008940: 7643 5055 7320 7468 6174 2061 7265 2072  vCPUs that are r
-00008950: 6571 7569 7265 6420 746f 2065 7865 6375  equired to execu
-00008960: 7465 2054 6173 6b73 2045 2e67 2e2c 2060  te Tasks E.g., `
-00008970: 5b32 2e30 2c20 342e 305d 602e 2020 2020  [2.0, 4.0]`.    
-00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-000089d0: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-000089e0: 2020 2020 2020 7c0a 7c20 6076 6572 6966        |.| `verif
-000089f0: 7941 7453 7461 7274 6020 2020 2020 2020  yAtStart`       
-00008a00: 2020 2020 207c 2041 206c 6973 7420 6f66       | A list of
-00008a10: 2066 696c 6573 2072 6571 7569 7265 6420   files required 
-00008a20: 6279 2061 2054 6173 6b2e 204d 7573 7420  by a Task. Must 
-00008a30: 6265 2070 7265 7365 6e74 2077 6865 6e20  be present when 
-00008a40: 7468 6520 5461 736b 2069 7320 7265 6164  the Task is read
-00008a50: 7920 746f 2073 7461 7274 206f 7220 7468  y to start or th
-00008a60: 6520 5461 736b 2077 696c 6c20 6661 696c  e Task will fail
-00008a70: 2e20 452e 672e 3a20 605b 2274 6173 6b5f  . E.g.: `["task_
-00008a80: 6772 6f75 705f 312f 7461 736b 5f31 2f72  group_1/task_1/r
-00008a90: 6573 756c 7473 2e74 7874 225d 602e 2020  esults.txt"]`.  
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00008ac0: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
-00008ad0: 7665 7269 6679 5761 6974 6020 2020 2020  verifyWait`     
-00008ae0: 2020 2020 2020 2020 2020 7c20 4120 6c69            | A li
-00008af0: 7374 206f 6620 6669 6c65 7320 7265 7175  st of files requ
-00008b00: 6972 6564 2062 7920 6120 5461 736b 2e20  ired by a Task. 
-00008b10: 5468 6520 5461 736b 2077 696c 6c20 7761  The Task will wa
-00008b20: 6974 2075 6e74 696c 2074 6865 2066 696c  it until the fil
-00008b30: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
-00008b40: 2062 6566 6f72 6520 7374 6172 7469 6e67   before starting
-00008b50: 2e20 452e 672e 3a20 605b 2274 6173 6b5f  . E.g.: `["task_
-00008b60: 6772 6f75 705f 312f 7461 736b 5f31 2f72  group_1/task_1/r
-00008b70: 6573 756c 7473 2e74 7874 225d 602e 2020  esults.txt"]`.  
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-00008ba0: 7320 7c20 5965 7320 207c 2059 6573 2020  s | Yes  | Yes  
-00008bb0: 7c0a 7c20 6077 6f72 6b65 7254 6167 7360  |.| `workerTags`
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00008bd0: 2054 6865 206c 6973 7420 6f66 2057 6f72   The list of Wor
-00008be0: 6b65 7220 5461 6773 2074 6861 7420 7769  ker Tags that wi
-00008bf0: 6c6c 2062 6520 7573 6564 2074 6f20 6d61  ll be used to ma
-00008c00: 7463 6820 6167 6169 6e73 7420 7468 6520  tch against the 
-00008c10: 576f 726b 6572 2054 6167 206f 6620 6120  Worker Tag of a 
-00008c20: 6361 6e64 6964 6174 6520 576f 726b 6572  candidate Worker
-00008c30: 2e20 452e 672e 2c20 605b 2274 6167 5f78  . E.g., `["tag_x
-00008c40: 222c 2022 7461 675f 7922 5d60 2e20 2020  ", "tag_y"]`.   
-00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-00008c80: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
-00008c90: 2020 2020 207c 0a7c 2060 776f 726b 5265       |.| `workRe
-00008ca0: 7175 6972 656d 656e 7444 6174 6160 2020  quirementData`  
-00008cb0: 2020 2020 7c20 5468 6520 6e61 6d65 206f      | The name o
-00008cc0: 6620 7468 6520 6669 6c65 2063 6f6e 7461  f the file conta
-00008cd0: 696e 696e 6720 7468 6520 4a53 4f4e 2064  ining the JSON d
-00008ce0: 6f63 756d 656e 7420 696e 2077 6869 6368  ocument in which
-00008cf0: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-00008d00: 656d 656e 7420 6973 2064 6566 696e 6564  ement is defined
-00008d10: 2e20 452e 672e 2c20 6022 7465 7374 5f77  . E.g., `"test_w
-00008d20: 6f72 6b72 6571 2e6a 736f 6e22 602e 2020  orkreq.json"`.  
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00008d60: 2059 6573 2020 7c20 2020 2020 7c20 2020   Yes  |     |   
-00008d70: 2020 207c 2020 2020 2020 7c0a 0a23 2320     |      |..## 
-00008d80: 4175 746f 6d61 7469 6320 5072 6f70 6572  Automatic Proper
-00008d90: 7469 6573 0a0a 496e 2061 6464 6974 696f  ties..In additio
-00008da0: 6e20 746f 2074 6865 2069 6e68 6572 6974  n to the inherit
-00008db0: 616e 6365 206d 6563 6861 6e69 736d 2c20  ance mechanism, 
-00008dc0: 736f 6d65 2070 726f 7065 7274 6965 7320  some properties 
-00008dd0: 6172 6520 7365 7420 6175 746f 6d61 7469  are set automati
-00008de0: 6361 6c6c 7920 6279 2074 6865 2060 7964  cally by the `yd
-00008df0: 2d73 7562 6d69 7460 2063 6f6d 6d61 6e64  -submit` command
-00008e00: 2c20 6173 2061 2075 7361 6765 2063 6f6e  , as a usage con
-00008e10: 7665 6e69 656e 6365 2069 6620 7468 6579  venience if they
-00008e20: 2772 6520 6e6f 7420 6578 706c 6963 6974  're not explicit
-00008e30: 6c79 2070 726f 7669 6465 642e 0a0a 2323  ly provided...##
-00008e40: 2320 576f 726b 2052 6571 7569 7265 6d65  # Work Requireme
-00008e50: 6e74 2c20 5461 736b 2047 726f 7570 2061  nt, Task Group a
-00008e60: 6e64 2054 6173 6b20 4e61 6d69 6e67 0a0a  nd Task Naming..
-00008e70: 2d20 5468 6520 2a2a 576f 726b 2052 6571  - The **Work Req
-00008e80: 7569 7265 6d65 6e74 2a2a 206e 616d 6520  uirement** name 
-00008e90: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-00008ea0: 2073 6574 2075 7369 6e67 2061 2063 6f6e   set using a con
-00008eb0: 6361 7465 6e61 7469 6f6e 206f 6620 7468  catenation of th
-00008ec0: 6520 6074 6167 6020 7072 6f70 6572 7479  e `tag` property
-00008ed0: 2c20 6120 5554 4320 7469 6d65 7374 616d  , a UTC timestam
-00008ee0: 702c 2061 6e64 2074 6872 6565 2072 616e  p, and three ran
-00008ef0: 646f 6d20 6865 7820 6368 6172 6163 7465  dom hex characte
-00008f00: 7273 3a20 652c 672c 2e20 606d 7974 6167  rs: e,g,. `mytag
-00008f10: 5f32 3231 3032 342d 3135 3535 3234 2d34  _221024-155524-4
-00008f20: 3061 602e 0a2d 202a 2a54 6173 6b20 4772  0a`..- **Task Gr
-00008f30: 6f75 702a 2a20 6e61 6d65 7320 6172 6520  oup** names are 
-00008f40: 6175 746f 6d61 7469 6361 6c6c 7920 6372  automatically cr
-00008f50: 6561 7465 6420 666f 7220 616e 7920 5461  eated for any Ta
-00008f60: 736b 2047 726f 7570 2074 6861 7420 6973  sk Group that is
-00008f70: 206e 6f74 2065 7870 6c69 6369 746c 7920   not explicitly 
-00008f80: 6e61 6d65 642c 2075 7369 6e67 206e 616d  named, using nam
-00008f90: 6573 206f 6620 7468 6520 666f 726d 2060  es of the form `
-00008fa0: 7461 736b 5f67 726f 7570 5f31 6020 286f  task_group_1` (o
-00008fb0: 7220 6074 6173 6b5f 6772 6f75 705f 3031  r `task_group_01
-00008fc0: 602c 2065 7463 2e2c 2066 6f72 206c 6172  `, etc., for lar
-00008fd0: 6765 7220 6e75 6d62 6572 7320 6f66 2054  ger numbers of T
-00008fe0: 6173 6b20 4772 6f75 7073 292e 2054 6173  ask Groups). Tas
-00008ff0: 6b20 4772 6f75 7020 6e75 6d62 6572 7320  k Group numbers 
-00009000: 6361 6e20 616c 736f 2062 6520 696e 636c  can also be incl
-00009010: 7564 6564 2069 6e20 7573 6572 2d64 6566  uded in user-def
-00009020: 696e 6564 2054 6173 6b20 4772 6f75 7020  ined Task Group 
-00009030: 6e61 6d65 7320 7573 696e 6720 7468 6520  names using the 
-00009040: 607b 7b74 6173 6b5f 6772 6f75 705f 6e75  `{{task_group_nu
-00009050: 6d62 6572 7d7d 6020 7661 7269 6162 6c65  mber}}` variable
-00009060: 2073 7562 7374 6974 7574 696f 6e20 6469   substitution di
-00009070: 7363 7573 7365 6420 6265 6c6f 772e 0a2d  scussed below..-
-00009080: 202a 2a54 6173 6b2a 2a20 6e61 6d65 7320   **Task** names 
-00009090: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
-000090a0: 7920 6372 6561 7465 6420 666f 7220 616e  y created for an
-000090b0: 7920 5461 736b 2074 6861 7420 6973 206e  y Task that is n
-000090c0: 6f74 2065 7870 6c69 6369 746c 7920 6e61  ot explicitly na
-000090d0: 6d65 642c 2075 7369 6e67 206e 616d 6573  med, using names
-000090e0: 206f 6620 7468 6520 666f 726d 2060 7461   of the form `ta
-000090f0: 736b 5f31 6020 286f 7220 6074 6173 6b5f  sk_1` (or `task_
-00009100: 3031 602c 2065 7463 2e2c 2066 6f72 206c  01`, etc., for l
-00009110: 6172 6765 7220 6e75 6d62 6572 7320 6f66  arger numbers of
-00009120: 2054 6173 6b73 292e 2054 6865 2054 6173   Tasks). The Tas
-00009130: 6b20 636f 756e 7465 7220 7265 7365 7473  k counter resets
-00009140: 2066 6f72 2065 6163 6820 6469 6666 6572   for each differ
-00009150: 656e 7420 5461 736b 2047 726f 7570 2e20  ent Task Group. 
-00009160: 5461 736b 206e 756d 6265 7273 2063 616e  Task numbers can
-00009170: 2061 6c73 6f20 6265 2069 6e63 6c75 6465   also be include
-00009180: 6420 696e 2075 7365 722d 6465 6669 6e65  d in user-define
-00009190: 6420 5461 736b 206e 616d 6573 2075 7369  d Task names usi
-000091a0: 6e67 2074 6865 2060 7b7b 7461 736b 5f6e  ng the `{{task_n
-000091b0: 756d 6265 727d 7d60 2076 6172 6961 626c  umber}}` variabl
-000091c0: 6520 7375 6273 7469 7475 7469 6f6e 2064  e substitution d
-000091d0: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
-000091e0: 0a23 2323 2054 6173 6b20 5479 7065 730a  .### Task Types.
-000091f0: 0a2d 2049 6620 6074 6173 6b54 7970 6560  .- If `taskType`
-00009200: 2069 7320 7365 7420 6f6e 6c79 2061 7420   is set only at 
-00009210: 7468 6520 544f 4d4c 2066 696c 6520 6c65  the TOML file le
-00009220: 7665 6c2c 2074 6865 6e20 6074 6173 6b54  vel, then `taskT
-00009230: 7970 6573 6020 6973 2061 7574 6f6d 6174  ypes` is automat
-00009240: 6963 616c 6c79 2070 6f70 756c 6174 6564  ically populated
-00009250: 2066 6f72 2054 6173 6b20 4772 6f75 7073   for Task Groups
-00009260: 2c20 756e 6c65 7373 206f 7665 7272 6964  , unless overrid
-00009270: 6465 6e2e 0a2d 2049 6620 6074 6173 6b54  den..- If `taskT
-00009280: 7970 6560 2069 7320 7365 7420 6174 2074  ype` is set at t
-00009290: 6865 2054 6173 6b20 6c65 7665 6c2c 2074  he Task level, t
-000092a0: 6865 6e20 6074 6173 6b54 7970 6573 6020  hen `taskTypes` 
-000092b0: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-000092c0: 2070 6f70 756c 6174 6564 2066 6f72 2074   populated for t
-000092d0: 6865 2054 6173 6b20 4772 6f75 7073 206c  he Task Groups l
-000092e0: 6576 656c 2075 7369 6e67 2074 6865 2061  evel using the a
-000092f0: 6363 756d 756c 6174 6564 2054 6173 6b20  ccumulated Task 
-00009300: 5479 7065 7320 6672 6f6d 2074 6865 2054  Types from the T
-00009310: 6173 6b73 2069 6e63 6c75 6465 6420 696e  asks included in
-00009320: 2065 6163 6820 5461 736b 2047 726f 7570   each Task Group
-00009330: 2c20 756e 6c65 7373 206f 7665 7272 6964  , unless overrid
-00009340: 6465 6e2e 0a2d 2049 6620 6074 6173 6b54  den..- If `taskT
-00009350: 7970 6573 6020 6973 2073 6574 2061 7420  ypes` is set at 
-00009360: 7468 6520 5461 736b 2047 726f 7570 204c  the Task Group L
-00009370: 6576 656c 2c20 616e 6420 6861 7320 6f6e  evel, and has on
-00009380: 6c79 206f 6e65 2054 6173 6b20 5479 7065  ly one Task Type
-00009390: 2065 6e74 7279 2c20 7468 656e 2060 7461   entry, then `ta
-000093a0: 736b 5479 7065 6020 6973 2061 7574 6f6d  skType` is autom
-000093b0: 6174 6963 616c 6c79 2073 6574 2061 7420  atically set at 
-000093c0: 7468 6520 5461 736b 204c 6576 656c 2075  the Task Level u
-000093d0: 7369 6e67 2074 6865 2073 696e 676c 6520  sing the single 
-000093e0: 5461 736b 2054 7970 652c 2075 6e6c 6573  Task Type, unles
-000093f0: 7320 6f76 6572 7269 6464 656e 2e0a 0a46  s overridden...F
-00009400: 6f72 2074 6865 202a 2a60 6261 7368 602a  or the **`bash`*
-00009410: 2a2c 202a 2a60 706f 7765 7273 6865 6c6c  *, **`powershell
-00009420: 602a 2a2c 202a 2a60 636d 6460 2a2a 2f2a  `**, **`cmd`**/*
-00009430: 2a60 6261 7460 2a2a 2061 6e64 202a 2a60  *`bat`** and **`
-00009440: 646f 636b 6572 602a 2a20 7461 736b 2074  docker`** task t
-00009450: 7970 6573 2c20 736f 6d65 2061 7574 6f6d  ypes, some autom
-00009460: 6174 6963 2070 726f 6365 7373 696e 6720  atic processing 
-00009470: 7769 6c6c 2062 6520 7065 7266 6f72 6d65  will be performe
-00009480: 6420 6966 2074 6865 202a 2a60 6578 6563  d if the **`exec
-00009490: 7574 6162 6c65 602a 2a20 7072 6f70 6572  utable`** proper
-000094a0: 7479 2069 7320 7365 742e 0a0a 2323 2323  ty is set...####
-000094b0: 2042 6173 682c 2050 7974 686f 6e2c 2050   Bash, Python, P
-000094c0: 6f77 6572 5368 656c 6c20 616e 6420 636d  owerShell and cm
-000094d0: 642f 6261 7420 5461 736b 730a 0a41 7320  d/bat Tasks..As 
-000094e0: 6120 636f 6e76 656e 6965 6e63 652c 2066  a convenience, f
-000094f0: 6f72 2074 6865 202a 2a60 6261 7368 602a  or the **`bash`*
-00009500: 2a2c 202a 2a60 7079 7468 6f6e 602a 2a2c  *, **`python`**,
-00009510: 202a 2a60 706f 7765 7273 6865 6c6c 602a   **`powershell`*
-00009520: 2a2c 2061 6e64 202a 2a60 636d 6460 2a2a  *, and **`cmd`**
-00009530: 2028 6f72 202a 2a60 6261 7460 2a2a 2920   (or **`bat`**) 
-00009540: 5461 736b 2054 7970 6573 2c20 7468 6520  Task Types, the 
-00009550: 7363 7269 7074 206e 6f6d 696e 6174 6564  script nominated
-00009560: 2069 6e20 7468 6520 2a2a 6065 7865 6375   in the **`execu
-00009570: 7461 626c 6560 2a2a 2070 726f 7065 7274  table`** propert
-00009580: 7920 6973 2061 7574 6f6d 6174 6963 616c  y is automatical
-00009590: 6c79 2061 6464 6564 2074 6f20 7468 6520  ly added to the 
-000095a0: 6069 6e70 7574 7360 206c 6973 7420 2869  `inputs` list (i
-000095b0: 6620 6e6f 7420 616c 7265 6164 7920 7072  f not already pr
-000095c0: 6573 656e 7429 2e20 5468 6973 206d 6561  esent). This mea
-000095d0: 6e73 2074 6865 2073 6372 6970 7420 6669  ns the script fi
-000095e0: 6c65 2077 696c 6c20 6265 2075 706c 6f61  le will be uploa
-000095f0: 6465 6420 746f 2074 6865 204f 626a 6563  ded to the Objec
-00009600: 7420 5374 6f72 652c 2061 6e64 206d 6164  t Store, and mad
-00009610: 6520 6120 7265 7175 6972 656d 656e 7420  e a requirement 
-00009620: 6f66 2074 6865 2054 6173 6b20 7768 656e  of the Task when
-00009630: 2069 7420 7275 6e73 2e0a 0a55 7369 6e67   it runs...Using
-00009640: 2061 2042 6173 6820 5461 736b 2061 7320   a Bash Task as 
-00009650: 616e 2065 7861 6d70 6c65 2028 696e 2054  an example (in T
-00009660: 4f4d 4c20 666f 726d 293a 0a0a 6060 6074  OML form):..```t
-00009670: 6f6d 6c0a 7461 736b 5479 7065 203d 2022  oml.taskType = "
-00009680: 6261 7368 220a 6578 6563 7574 6162 6c65  bash".executable
-00009690: 203d 2022 6d79 5f62 6173 685f 7363 7269   = "my_bash_scri
-000096a0: 7074 2e73 6822 0a61 7267 756d 656e 7473  pt.sh".arguments
-000096b0: 203d 205b 2231 222c 2022 3222 2c20 2233   = ["1", "2", "3
-000096c0: 225d 0a60 6060 0a69 7320 6571 7569 7661  "].```.is equiva
-000096d0: 6c65 6e74 2074 6f3a 0a0a 6060 6074 6f6d  lent to:..```tom
-000096e0: 6c0a 7461 736b 5479 7065 203d 2022 6261  l.taskType = "ba
-000096f0: 7368 220a 696e 7075 7473 203d 205b 226d  sh".inputs = ["m
-00009700: 795f 6261 7368 5f73 6372 6970 742e 7368  y_bash_script.sh
-00009710: 225d 0a61 7267 756d 656e 7473 203d 205b  "].arguments = [
-00009720: 227b 7b77 725f 6e61 6d65 7d7d 2f6d 795f  "{{wr_name}}/my_
-00009730: 6261 7368 5f73 6372 6970 742e 7368 222c  bash_script.sh",
-00009740: 2022 3122 2c20 2232 222c 2022 3322 5d0a   "1", "2", "3"].
-00009750: 6060 600a 0a49 6e20 7468 6520 6361 7365  ```..In the case
-00009760: 206f 6620 5769 6e64 6f77 7320 6261 7463   of Windows batc
-00009770: 6820 2860 2e62 6174 6029 2066 696c 6573  h (`.bat`) files
-00009780: 2c20 6120 602f 6360 2066 6c61 6720 6973  , a `/c` flag is
-00009790: 2070 7265 7065 6e64 6564 2074 6f20 7468   prepended to th
-000097a0: 6520 6063 6d64 2e65 7865 6020 6172 6775  e `cmd.exe` argu
-000097b0: 6d65 6e74 206c 6973 7420 746f 2065 6e73  ment list to ens
-000097c0: 7572 6520 636f 7272 6563 7420 6578 6563  ure correct exec
-000097d0: 7574 696f 6e20 6261 6861 7669 6f75 722e  ution bahaviour.
-000097e0: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a60   For example:..`
-000097f0: 6060 746f 6d6c 0a74 6173 6b54 7970 6520  ``toml.taskType 
-00009800: 3d20 2263 6d64 2220 2023 206f 7220 2262  = "cmd"  # or "b
-00009810: 6174 220a 6578 6563 7574 6162 6c65 203d  at".executable =
-00009820: 2022 6d79 5f73 6372 6970 742e 6261 7422   "my_script.bat"
-00009830: 0a61 7267 756d 656e 7473 203d 205b 2231  .arguments = ["1
-00009840: 222c 2022 3222 2c20 2233 225d 0a60 6060  ", "2", "3"].```
-00009850: 0a0a 6973 2065 7175 6976 616c 656e 7420  ..is equivalent 
-00009860: 746f 3a0a 0a60 6060 746f 6d6c 0a74 6173  to:..```toml.tas
-00009870: 6b54 7970 6520 3d20 2263 6d64 2220 2023  kType = "cmd"  #
-00009880: 206f 7220 2262 6174 220a 696e 7075 7473   or "bat".inputs
-00009890: 203d 205b 226d 795f 7363 7269 7074 2e62   = ["my_script.b
-000098a0: 6174 225d 0a61 7267 756d 656e 7473 203d  at"].arguments =
-000098b0: 205b 222f 6322 2c20 227b 7b77 725f 6e61   ["/c", "{{wr_na
-000098c0: 6d65 7d7d 5c5c 6d79 5f73 6372 6970 742e  me}}\\my_script.
-000098d0: 6261 7422 2c20 2231 222c 2022 3222 2c20  bat", "1", "2", 
-000098e0: 2233 225d 0a60 6060 0a0a 4e6f 7465 2074  "3"].```..Note t
-000098f0: 6865 2060 5c5c 6020 7265 7175 6972 656d  he `\\` requirem
-00009900: 656e 7420 666f 7220 6469 7265 6374 6f72  ent for director
-00009910: 7920 7365 7061 7261 746f 7273 2077 6865  y separators whe
-00009920: 6e20 6465 6669 6e69 6e67 2054 6173 6b73  n defining Tasks
-00009930: 206f 6e20 5769 6e64 6f77 7320 686f 7374   on Windows host
-00009940: 732e 204e 6f74 6520 616c 736f 2074 6861  s. Note also tha
-00009950: 7420 7468 6520 602f 6360 2069 7320 7265  t the `/c` is re
-00009960: 7175 6972 6564 2077 6865 6e20 7275 6e6e  quired when runn
-00009970: 696e 6720 636f 6d6d 616e 6473 206f 7220  ing commands or 
-00009980: 6261 7463 6820 7363 7269 7074 7320 7573  batch scripts us
-00009990: 696e 6720 6063 6d64 2e65 7865 602c 206f  ing `cmd.exe`, o
-000099a0: 7468 6572 7769 7365 2074 6865 2060 636d  therwise the `cm
-000099b0: 642e 6578 6560 2070 726f 6365 7373 2063  d.exe` process c
-000099c0: 7265 6174 6564 2074 6f20 6578 6563 7574  reated to execut
-000099d0: 6520 7468 6520 5461 736b 2077 696c 6c20  e the Task will 
-000099e0: 6e6f 7420 7465 726d 696e 6174 652e 0a0a  not terminate...
-000099f0: 2323 2323 2044 6f63 6b65 7220 5461 736b  #### Docker Task
-00009a00: 730a 0a46 6f72 2074 6865 202a 2a60 646f  s..For the **`do
-00009a10: 636b 6572 602a 2a20 5461 736b 2054 7970  cker`** Task Typ
-00009a20: 652c 2074 6865 2076 6172 6961 626c 6573  e, the variables
-00009a30: 2073 7570 706c 6965 6420 696e 2074 6865   supplied in the
-00009a40: 2060 646f 636b 6572 456e 7669 726f 6e6d   `dockerEnvironm
-00009a50: 656e 7460 2070 726f 7065 7274 7920 6172  ent` property ar
-00009a60: 6520 756e 7061 636b 6564 2069 6e74 6f20  e unpacked into 
-00009a70: 7468 6520 6172 6775 6d65 6e74 206c 6973  the argument lis
-00009a80: 7420 6173 2060 2d2d 656e 7660 2065 6e74  t as `--env` ent
-00009a90: 7269 6573 2c20 7468 6520 446f 636b 6572  ries, the Docker
-00009aa0: 2063 6f6e 7461 696e 6572 206e 616d 6520   container name 
-00009ab0: 7375 7070 6c69 6564 2069 6e20 7468 6520  supplied in the 
-00009ac0: 6065 7865 6375 7461 626c 6560 2070 726f  `executable` pro
-00009ad0: 7065 7274 7920 6973 2074 6865 6e20 6164  perty is then ad
-00009ae0: 6465 6420 746f 2074 6865 2061 7267 756d  ded to the argum
-00009af0: 656e 7473 206c 6973 742c 2066 6f6c 6c6f  ents list, follo
-00009b00: 7765 6420 6279 2074 6865 2061 7267 756d  wed by the argum
-00009b10: 656e 7473 2073 7570 706c 6965 6420 696e  ents supplied in
-00009b20: 2074 6865 2060 6172 6775 6d65 6e74 7360   the `arguments`
-00009b30: 2070 726f 7065 7274 792e 2054 6865 2060   property. The `
-00009b40: 646f 636b 6572 5573 6572 6e61 6d65 6020  dockerUsername` 
-00009b50: 616e 6420 6064 6f63 6b65 7250 6173 7377  and `dockerPassw
-00009b60: 6f72 6460 2070 726f 7065 7274 6965 732c  ord` properties,
-00009b70: 2069 6620 7375 7070 6c69 6564 2c20 6172   if supplied, ar
-00009b80: 6520 6164 6465 6420 746f 2074 6865 2060  e added to the `
-00009b90: 656e 7669 726f 6e6d 656e 7460 2070 726f  environment` pro
-00009ba0: 7065 7274 792e 0a0a 466f 7220 6578 616d  perty...For exam
-00009bb0: 706c 653a 0a60 6060 746f 6d6c 0a74 6173  ple:.```toml.tas
-00009bc0: 6b54 7970 6520 3d20 2264 6f63 6b65 7222  kType = "docker"
-00009bd0: 0a65 7865 6375 7461 626c 6520 3d20 226d  .executable = "m
-00009be0: 795f 646f 636b 6572 6875 625f 7265 706f  y_dockerhub_repo
-00009bf0: 2f6d 795f 636f 6e74 6169 6e65 725f 696d  /my_container_im
-00009c00: 6167 6522 0a64 6f63 6b65 7245 6e76 6972  age".dockerEnvir
-00009c10: 6f6e 6d65 6e74 203d 207b 4531 203d 2022  onment = {E1 = "
-00009c20: 4565 654f 6e65 227d 0a64 6f63 6b65 7255  EeeOne"}.dockerU
-00009c30: 7365 726e 616d 6520 3d20 226d 795f 7573  sername = "my_us
-00009c40: 6572 220a 646f 636b 6572 5061 7373 776f  er".dockerPasswo
-00009c50: 7264 203d 2022 6d79 5f70 6173 7377 6f72  rd = "my_passwor
-00009c60: 6422 0a61 7267 756d 656e 7473 203d 205b  d".arguments = [
-00009c70: 2231 222c 2022 3222 2c20 2233 225d 0a60  "1", "2", "3"].`
-00009c80: 6060 0a0a 6973 2065 7175 6976 616c 656e  ``..is equivalen
-00009c90: 7420 746f 2074 6865 2066 6f6c 6c6f 7769  t to the followi
-00009ca0: 6e67 2062 6569 6e67 2073 656e 7420 666f  ng being sent fo
-00009cb0: 7220 7072 6f63 6573 7369 6e67 2062 7920  r processing by 
-00009cc0: 7468 6520 6064 6f63 6b65 7260 2054 6173  the `docker` Tas
-00009cd0: 6b20 5479 7065 2c20 7468 6520 5965 6c6c  k Type, the Yell
-00009ce0: 6f77 446f 6720 7665 7273 696f 6e20 6f66  owDog version of
-00009cf0: 2077 6869 6368 2077 696c 6c20 6c6f 6720   which will log 
-00009d00: 696e 2074 6f20 7468 6520 446f 636b 6572  in to the Docker
-00009d10: 2072 6570 6f20 2869 6620 7265 7175 6972   repo (if requir
-00009d20: 6564 2920 7468 656e 2069 7373 7565 2061  ed) then issue a
-00009d30: 2060 646f 636b 6572 2072 756e 6020 636f   `docker run` co
-00009d40: 6d6d 616e 6420 7769 7468 2074 6865 2061  mmand with the a
-00009d50: 7267 756d 656e 7473 2073 7570 706c 6965  rguments supplie
-00009d60: 643a 0a0a 6060 6074 6f6d 6c0a 7461 736b  d:..```toml.task
-00009d70: 5479 7065 203d 2022 646f 636b 6572 220a  Type = "docker".
-00009d80: 6172 6775 6d65 6e74 7320 3d20 5b22 2d2d  arguments = ["--
-00009d90: 656e 7620 4531 3d45 6565 4f6e 6522 2c20  env E1=EeeOne", 
-00009da0: 226d 795f 646f 636b 6572 6875 6272 6570  "my_dockerhubrep
-00009db0: 6f2f 6d79 5f63 6f6e 7461 696e 6572 5f69  o/my_container_i
-00009dc0: 6d61 6765 222c 2022 3122 2c20 2232 222c  mage", "1", "2",
-00009dd0: 2022 3322 5d0a 656e 7669 726f 6e6d 656e   "3"].environmen
-00009de0: 7420 3d20 7b44 4f43 4b45 525f 5553 4552  t = {DOCKER_USER
-00009df0: 4e41 4d45 203d 2022 6d79 5f75 7365 7222  NAME = "my_user"
-00009e00: 2c20 444f 434b 4552 5f50 4153 5357 4f52  , DOCKER_PASSWOR
-00009e10: 4420 3d20 226d 795f 7061 7373 776f 7264  D = "my_password
-00009e20: 227d 0a60 6060 0a0a 2323 2323 2042 6173  "}.```..#### Bas
-00009e30: 682c 2050 7974 686f 6e2c 2050 6f77 6572  h, Python, Power
-00009e40: 5368 656c 6c2c 2063 6d64 2e65 7865 2f62  Shell, cmd.exe/b
-00009e50: 6174 6368 2c20 616e 6420 446f 636b 6572  atch, and Docker
-00009e60: 2077 6974 686f 7574 2041 7574 6f6d 6174   without Automat
-00009e70: 6963 2050 726f 6365 7373 696e 670a 0a49  ic Processing..I
-00009e80: 6620 7468 6520 6065 7865 6375 7461 626c  f the `executabl
-00009e90: 6560 2070 726f 7065 7274 7920 6973 206e  e` property is n
-00009ea0: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
-00009eb0: 2061 7574 6f6d 6174 6963 2070 726f 6365   automatic proce
-00009ec0: 7373 696e 6720 6465 7363 7269 6265 6420  ssing described 
-00009ed0: 6162 6f76 6520 666f 7220 6062 6173 6860  above for `bash`
-00009ee0: 2c20 6070 7974 686f 6e60 2c20 6070 6f77  , `python`, `pow
-00009ef0: 6572 7368 656c 6c60 2c20 6063 6d64 6020  ershell`, `cmd` 
-00009f00: 286f 7220 6062 6174 6029 2061 6e64 2060  (or `bat`) and `
-00009f10: 646f 636b 6572 6020 7461 736b 2074 7970  docker` task typ
-00009f20: 6573 2069 7320 6e6f 7420 6170 706c 6965  es is not applie
-00009f30: 642e 0a0a 2323 2320 5461 736b 2043 6f75  d...### Task Cou
-00009f40: 6e74 730a 0a54 6869 7320 7072 6f70 6572  nts..This proper
-00009f50: 7479 2077 696c 6c20 6578 7061 6e64 2074  ty will expand t
-00009f60: 6865 206e 756d 6265 7220 6f66 2054 6173  he number of Tas
-00009f70: 6b73 2074 6f20 6d61 7463 6820 6074 6173  ks to match `tas
-00009f80: 6b43 6f75 6e74 602e 0a0a 5468 6520 6074  kCount`...The `t
-00009f90: 6173 6b43 6f75 6e74 6020 7072 6f70 6572  askCount` proper
-00009fa0: 7479 2063 616e 2062 6520 7365 7420 6f6e  ty can be set on
-00009fb0: 6c79 2069 6e20 7468 6520 6077 6f72 6b52  ly in the `workR
-00009fc0: 6571 7569 7265 6d65 6e74 6020 7365 6374  equirement` sect
-00009fd0: 696f 6e20 6f66 2074 6865 2060 636f 6e66  ion of the `conf
-00009fe0: 6967 2e74 6f6d 6c60 2066 696c 652c 206f  ig.toml` file, o
-00009ff0: 7220 696e 2074 6865 2060 7461 736b 4772  r in the `taskGr
-0000a000: 6f75 7060 2073 6563 7469 6f6e 2873 2920  oup` section(s) 
-0000a010: 6f66 2061 204a 534f 4e20 576f 726b 2052  of a JSON Work R
-0000a020: 6571 7569 7265 6d65 6e74 2064 6566 696e  equirement defin
-0000a030: 6974 696f 6e2e 0a0a 496e 2074 6865 2066  ition...In the f
-0000a040: 6f72 6d65 7220 6361 7365 2c20 7468 6520  ormer case, the 
-0000a050: 6074 6173 6b43 6f75 6e74 6020 6170 706c  `taskCount` appl
-0000a060: 6965 7320 6f6e 6c79 2074 6f20 7468 6520  ies only to the 
-0000a070: 5461 736b 2073 7065 6369 6669 6564 2077  Task specified w
-0000a080: 6974 6869 6e20 7468 6520 6063 6f6e 6669  ithin the `confi
-0000a090: 672e 746f 6d6c 6020 6669 6c65 2061 6e64  g.toml` file and
-0000a0a0: 2069 7320 6e6f 7420 696e 6865 7269 7465   is not inherite
-0000a0b0: 6420 6279 204a 534f 4e20 576f 726b 2052  d by JSON Work R
-0000a0c0: 6571 7569 7265 6d65 6e74 2073 7065 6369  equirement speci
-0000a0d0: 6669 6361 7469 6f6e 732e 0a0a 496e 2074  fications...In t
-0000a0e0: 6865 206c 6174 7465 7220 6361 7365 2c20  he latter case, 
-0000a0f0: 7468 6520 6074 6173 6b43 6f75 6e74 6020  the `taskCount` 
-0000a100: 6170 706c 6965 7320 746f 2074 6865 2054  applies to the T
-0000a110: 6173 6b20 7370 6563 6966 6965 6420 7769  ask specified wi
-0000a120: 7468 696e 2074 6865 2054 6173 6b20 4772  thin the Task Gr
-0000a130: 6f75 702c 2061 6e64 2074 6865 7265 206d  oup, and there m
-0000a140: 7573 7420 6265 207a 6572 6f20 6f72 206f  ust be zero or o
-0000a150: 6e65 2054 6173 6b28 7329 206c 6973 7465  ne Task(s) liste
-0000a160: 6420 7769 7468 696e 2074 6865 2067 726f  d within the gro
-0000a170: 7570 206f 7220 6074 6173 6b43 6f75 6e74  up or `taskCount
-0000a180: 6020 6973 2069 676e 6f72 6564 2e0a 0a23  ` is ignored...#
-0000a190: 2320 4578 616d 706c 6573 0a0a 2323 2320  # Examples..### 
-0000a1a0: 544f 4d4c 2050 726f 7065 7274 6965 7320  TOML Properties 
-0000a1b0: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
-0000a1c0: 6972 656d 656e 7460 2053 6563 7469 6f6e  irement` Section
-0000a1d0: 0a0a 4865 7265 2773 2061 6e20 6578 616d  ..Here's an exam
-0000a1e0: 706c 6520 6f66 2074 6865 2060 776f 726b  ple of the `work
-0000a1f0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
-0000a200: 7469 6f6e 206f 6620 6120 544f 4d4c 2063  tion of a TOML c
-0000a210: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-0000a220: 652c 2073 686f 7769 6e67 2061 6c6c 2074  e, showing all t
-0000a230: 6865 2070 6f73 7369 626c 6520 7072 6f70  he possible prop
-0000a240: 6572 7469 6573 2074 6861 7420 6361 6e20  erties that can 
-0000a250: 6265 2073 6574 3a0a 0a60 6060 746f 6d6c  be set:..```toml
-0000a260: 0a5b 776f 726b 5265 7175 6972 656d 656e  .[workRequiremen
-0000a270: 745d 0a20 2020 2061 7267 756d 656e 7473  t].    arguments
-0000a280: 203d 205b 2231 222c 2022 5457 4f22 5d0a   = ["1", "TWO"].
-0000a290: 2020 2020 6361 7074 7572 6554 6173 6b4f      captureTaskO
-0000a2a0: 7574 7075 7420 3d20 7472 7565 0a20 2020  utput = true.   
-0000a2b0: 2063 6f6d 706c 6574 6564 5461 736b 5474   completedTaskTt
-0000a2c0: 6c20 3d20 3130 0a20 2020 2063 7376 4669  l = 10.    csvFi
-0000a2d0: 6c65 203d 2022 6669 6c65 312e 6373 7622  le = "file1.csv"
-0000a2e0: 0a20 2020 2063 7376 4669 6c65 7320 3d20  .    csvFiles = 
-0000a2f0: 5b22 6669 6c65 312e 6373 7622 2c20 2266  ["file1.csv", "f
-0000a300: 696c 6533 2e63 7376 3a33 225d 0a20 2020  ile3.csv:3"].   
-0000a310: 2064 6f63 6b65 7245 6e76 6972 6f6e 6d65   dockerEnvironme
-0000a320: 6e74 203d 207b 4d59 5f44 4f43 4b45 525f  nt = {MY_DOCKER_
-0000a330: 5641 5220 3d20 3130 307d 0a20 2020 2064  VAR = 100}.    d
-0000a340: 6f63 6b65 7250 6173 7377 6f72 6420 3d20  ockerPassword = 
-0000a350: 226d 7950 6173 7377 6f72 6422 0a20 2020  "myPassword".   
-0000a360: 2064 6f63 6b65 7255 7365 726e 616d 6520   dockerUsername 
-0000a370: 3d20 226d 7955 7365 726e 616d 6522 0a20  = "myUsername". 
-0000a380: 2020 2065 6e76 6972 6f6e 6d65 6e74 203d     environment =
-0000a390: 207b 4d59 5f56 4152 203d 2031 3030 7d0a   {MY_VAR = 100}.
-0000a3a0: 2020 2020 6578 636c 7573 6976 6557 6f72      exclusiveWor
-0000a3b0: 6b65 7273 203d 2066 616c 7365 0a20 2020  kers = false.   
-0000a3c0: 2065 7865 6375 7461 626c 6520 3d20 226d   executable = "m
-0000a3d0: 792d 636f 6e74 6169 6e65 7222 0a20 2020  y-container".   
-0000a3e0: 2066 696e 6973 6849 6641 6c6c 5461 736b   finishIfAllTask
-0000a3f0: 7346 696e 6973 6865 6420 3d20 7472 7565  sFinished = true
-0000a400: 0a20 2020 2066 696e 6973 6849 6641 6e79  .    finishIfAny
-0000a410: 5461 736b 4661 696c 6564 203d 2066 616c  TaskFailed = fal
-0000a420: 7365 0a20 2020 2066 6c61 7474 656e 496e  se.    flattenIn
-0000a430: 7075 7450 6174 6873 203d 2066 616c 7365  putPaths = false
-0000a440: 0a20 2020 2066 6c61 7474 656e 5570 6c6f  .    flattenUplo
-0000a450: 6164 5061 7468 7320 3d20 6661 6c73 650a  adPaths = false.
-0000a460: 2020 2020 6675 6c66 696c 4f6e 5375 626d      fulfilOnSubm
-0000a470: 6974 203d 2066 616c 7365 0a20 2020 2069  it = false.    i
-0000a480: 6e70 7574 7320 3d20 5b0a 2020 2020 2020  nputs = [.      
-0000a490: 2020 222e 2e2f 6170 702f 6d61 696e 2e70    "../app/main.p
-0000a4a0: 7922 2c0a 2020 2020 2020 2020 222e 2e2f  y",.        "../
-0000a4b0: 6170 702f 7265 7175 6972 656d 656e 7473  app/requirements
-0000a4c0: 2e74 7874 220a 2020 2020 5d0a 2020 2020  .txt".    ].    
-0000a4d0: 696e 7075 7473 4f70 7469 6f6e 616c 203d  inputsOptional =
-0000a4e0: 205b 226f 7074 696f 6e61 6c2e 7478 7422   ["optional.txt"
-0000a4f0: 5d0a 2020 2020 696e 7374 616e 6365 5479  ].    instanceTy
-0000a500: 7065 7320 3d20 5b22 7433 612e 6d69 6372  pes = ["t3a.micr
-0000a510: 6f22 2c20 2274 332e 6d69 6372 6f22 5d0a  o", "t3.micro"].
-0000a520: 2020 2020 6d61 7857 6f72 6b65 7273 203d      maxWorkers =
-0000a530: 2031 0a20 2020 206d 6178 696d 756d 5461   1.    maximumTa
-0000a540: 736b 5265 7472 6965 7320 3d20 300a 2020  skRetries = 0.  
-0000a550: 2020 6d69 6e57 6f72 6b65 7273 203d 2031    minWorkers = 1
-0000a560: 0a20 2020 206e 616d 6520 3d20 226d 792d  .    name = "my-
-0000a570: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
-0000a580: 220a 2020 2020 6f75 7470 7574 7320 3d20  ".    outputs = 
-0000a590: 5b22 7265 7375 6c74 732e 7478 7422 5d0a  ["results.txt"].
-0000a5a0: 2020 2020 6f75 7470 7574 7352 6571 7569      outputsRequi
-0000a5b0: 7265 6420 3d20 5b22 7265 7375 6c74 735f  red = ["results_
-0000a5c0: 7265 7175 6972 6564 2e74 7874 225d 0a20  required.txt"]. 
-0000a5d0: 2020 2070 7269 6f72 6974 7920 3d20 302e     priority = 0.
-0000a5e0: 300a 2020 2020 7072 6f76 6964 6572 7320  0.    providers 
-0000a5f0: 3d20 5b22 4157 5322 5d0a 2020 2020 7261  = ["AWS"].    ra
-0000a600: 6d20 3d20 5b30 2e35 2c20 322e 305d 0a20  m = [0.5, 2.0]. 
-0000a610: 2020 2072 6567 696f 6e73 203d 205b 2265     regions = ["e
-0000a620: 752d 7765 7374 2d32 225d 0a20 2020 2074  u-west-2"].    t
-0000a630: 6173 6b42 6174 6368 5369 7a65 203d 2031  askBatchSize = 1
-0000a640: 3030 300a 2020 2020 7461 736b 436f 756e  000.    taskCoun
-0000a650: 7420 3d20 3130 300a 2020 2020 7461 736b  t = 100.    task
-0000a660: 4461 7461 203d 2022 6d79 5f64 6174 615f  Data = "my_data_
-0000a670: 7374 7269 6e67 220a 2020 2020 7461 736b  string".    task
-0000a680: 4461 7461 4669 6c65 203d 2022 6d79 5f64  DataFile = "my_d
-0000a690: 6174 615f 6669 6c65 2e74 7874 220a 2020  ata_file.txt".  
-0000a6a0: 2020 7461 736b 4e61 6d65 203d 2022 6d79    taskName = "my
-0000a6b0: 5f74 6173 6b5f 6e75 6d62 6572 5f7b 7b74  _task_number_{{t
-0000a6c0: 6173 6b5f 6e75 6d62 6572 7d7d 220a 2020  ask_number}}".  
-0000a6d0: 2020 7461 736b 4772 6f75 704e 616d 6520    taskGroupName 
-0000a6e0: 3d20 226d 795f 7461 736b 5f67 726f 7570  = "my_task_group
-0000a6f0: 5f6e 756d 6265 725f 7b7b 7461 736b 5f67  _number_{{task_g
-0000a700: 726f 7570 5f6e 756d 6265 727d 7d22 0a20  roup_number}}". 
-0000a710: 2020 2074 6173 6b54 7970 6520 3d20 2264     taskType = "d
-0000a720: 6f63 6b65 7222 0a20 2020 2074 6173 6b73  ocker".    tasks
-0000a730: 5065 7257 6f72 6b65 7220 3d20 310a 2020  PerWorker = 1.  
-0000a740: 2020 7570 6c6f 6164 4669 6c65 7320 3d20    uploadFiles = 
-0000a750: 5b7b 6c6f 6361 6c50 6174 6820 3d20 2266  [{localPath = "f
-0000a760: 696c 655f 312e 7478 7422 2c20 7570 6c6f  ile_1.txt", uplo
-0000a770: 6164 5061 7468 203d 2022 6669 6c65 5f31  adPath = "file_1
-0000a780: 2e74 7874 227d 5d0a 2020 2020 7663 7075  .txt"}].    vcpu
-0000a790: 7320 3d20 5b31 2c20 345d 0a20 2020 2076  s = [1, 4].    v
-0000a7a0: 6572 6966 7941 7453 7461 7274 203d 205b  erifyAtStart = [
-0000a7b0: 2272 6561 6479 5f72 6573 756c 7473 2e74  "ready_results.t
-0000a7c0: 7874 225d 0a20 2020 2076 6572 6966 7957  xt"].    verifyW
-0000a7d0: 6169 7420 3d20 5b22 7761 6974 5f66 6f72  ait = ["wait_for
-0000a7e0: 5f72 6573 756c 7473 2e74 7874 225d 0a20  _results.txt"]. 
-0000a7f0: 2020 2077 6f72 6b65 7254 6167 7320 3d20     workerTags = 
-0000a800: 5b22 7461 672d 7b7b 7573 6572 6e61 6d65  ["tag-{{username
-0000a810: 7d7d 225d 0a20 2020 2077 6f72 6b52 6571  }}"].    workReq
-0000a820: 7569 7265 6d65 6e74 4461 7461 203d 2022  uirementData = "
-0000a830: 776f 726b 5f72 6571 7569 7265 6d65 6e74  work_requirement
-0000a840: 2e6a 736f 6e22 0a60 6060 0a0a 2323 2320  .json".```..### 
-0000a850: 4a53 4f4e 2050 726f 7065 7274 6965 7320  JSON Properties 
-0000a860: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
-0000a870: 6972 656d 656e 7420 4c65 7665 6c0a 0a53  irement Level..S
-0000a880: 686f 7769 6e67 2061 6c6c 2070 6f73 7369  howing all possi
-0000a890: 626c 6520 7072 6f70 6572 7469 6573 2061  ble properties a
-0000a8a0: 7420 7468 6520 576f 726b 2052 6571 7569  t the Work Requi
-0000a8b0: 7265 6d65 6e74 206c 6576 656c 3a0a 0a60  rement level:..`
-0000a8c0: 6060 6a73 6f6e 0a7b 0a20 2022 6172 6775  ``json.{.  "argu
-0000a8d0: 6d65 6e74 7322 3a20 5b31 2c20 2254 574f  ments": [1, "TWO
-0000a8e0: 225d 2c0a 2020 2263 6170 7475 7265 5461  "],.  "captureTa
-0000a8f0: 736b 4f75 7470 7574 223a 2074 7275 652c  skOutput": true,
-0000a900: 0a20 2022 636f 6d70 6c65 7465 6454 6173  .  "completedTas
-0000a910: 6b54 746c 223a 2031 302c 0a20 2022 646f  kTtl": 10,.  "do
-0000a920: 636b 6572 456e 7669 726f 6e6d 656e 7422  ckerEnvironment"
-0000a930: 3a20 7b22 4d59 5f44 4f43 4b45 525f 5641  : {"MY_DOCKER_VA
-0000a940: 5222 3a20 3130 307d 2c0a 2020 2264 6f63  R": 100},.  "doc
-0000a950: 6b65 7250 6173 7377 6f72 6422 3a20 226d  kerPassword": "m
-0000a960: 7950 6173 7377 6f72 6422 2c0a 2020 2264  yPassword",.  "d
-0000a970: 6f63 6b65 7255 7365 726e 616d 6522 3a20  ockerUsername": 
-0000a980: 226d 7955 7365 726e 616d 6522 2c0a 2020  "myUsername",.  
-0000a990: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-0000a9a0: 224d 595f 5641 5222 3a20 3130 307d 2c0a  "MY_VAR": 100},.
-0000a9b0: 2020 2265 7863 6c75 7369 7665 576f 726b    "exclusiveWork
-0000a9c0: 6572 7322 3a20 6661 6c73 652c 0a20 2022  ers": false,.  "
-0000a9d0: 6578 6563 7574 6162 6c65 223a 2022 6d79  executable": "my
-0000a9e0: 2d63 6f6e 7461 696e 6572 222c 0a20 2022  -container",.  "
-0000a9f0: 6669 6e69 7368 4966 416c 6c54 6173 6b73  finishIfAllTasks
-0000aa00: 4669 6e69 7368 6564 223a 2074 7275 652c  Finished": true,
-0000aa10: 0a20 2022 6669 6e69 7368 4966 416e 7954  .  "finishIfAnyT
-0000aa20: 6173 6b46 6169 6c65 6422 3a20 6661 6c73  askFailed": fals
-0000aa30: 652c 0a20 2022 666c 6174 7465 6e49 6e70  e,.  "flattenInp
-0000aa40: 7574 5061 7468 7322 3a20 6661 6c73 652c  utPaths": false,
-0000aa50: 0a20 2022 666c 6174 7465 6e55 706c 6f61  .  "flattenUploa
-0000aa60: 6450 6174 6873 223a 2066 616c 7365 2c0a  dPaths": false,.
-0000aa70: 2020 2266 756c 6669 6c4f 6e53 7562 6d69    "fulfilOnSubmi
-0000aa80: 7422 3a20 6661 6c73 652c 0a20 2022 696e  t": false,.  "in
-0000aa90: 7075 7473 223a 205b 2261 7070 2f6d 6169  puts": ["app/mai
-0000aaa0: 6e2e 7079 222c 2022 6170 702f 7265 7175  n.py", "app/requ
-0000aab0: 6972 656d 656e 7473 2e74 7874 225d 2c0a  irements.txt"],.
-0000aac0: 2020 2269 6e70 7574 734f 7074 696f 6e61    "inputsOptiona
-0000aad0: 6c22 3a20 5b22 6f70 7469 6f6e 616c 2e74  l": ["optional.t
-0000aae0: 7874 225d 2c0a 2020 2269 6e73 7461 6e63  xt"],.  "instanc
-0000aaf0: 6554 7970 6573 223a 205b 2274 3361 2e6d  eTypes": ["t3a.m
-0000ab00: 6963 726f 222c 2022 7433 2e6d 6963 726f  icro", "t3.micro
-0000ab10: 225d 2c0a 2020 226d 6178 576f 726b 6572  "],.  "maxWorker
-0000ab20: 7322 3a20 312c 0a20 2022 6d61 7869 6d75  s": 1,.  "maximu
-0000ab30: 6d54 6173 6b52 6574 7269 6573 223a 2030  mTaskRetries": 0
-0000ab40: 2c0a 2020 226d 696e 576f 726b 6572 7322  ,.  "minWorkers"
-0000ab50: 3a20 312c 0a20 2022 6e61 6d65 223a 2022  : 1,.  "name": "
-0000ab60: 6d79 2d77 6f72 6b2d 7265 7175 6972 656d  my-work-requirem
-0000ab70: 656e 7422 2c0a 2020 226f 7574 7075 7473  ent",.  "outputs
-0000ab80: 223a 205b 2272 6573 756c 7473 2e74 7874  ": ["results.txt
-0000ab90: 225d 2c0a 2020 226f 7574 7075 7473 5265  "],.  "outputsRe
-0000aba0: 7175 6972 6564 223a 205b 2272 6573 756c  quired": ["resul
-0000abb0: 7473 5f72 6571 7569 7265 642e 7478 7422  ts_required.txt"
-0000abc0: 5d2c 0a20 2022 7072 696f 7269 7479 223a  ],.  "priority":
-0000abd0: 2030 2e30 2c0a 2020 2270 726f 7669 6465   0.0,.  "provide
-0000abe0: 7273 223a 205b 2241 5753 225d 2c0a 2020  rs": ["AWS"],.  
-0000abf0: 2272 616d 223a 205b 302e 352c 2032 5d2c  "ram": [0.5, 2],
-0000ac00: 0a20 2022 7265 6769 6f6e 7322 3a20 5b22  .  "regions": ["
-0000ac10: 6575 2d77 6573 742d 3222 5d2c 0a20 2022  eu-west-2"],.  "
-0000ac20: 7461 736b 4461 7461 223a 2022 6d79 5f74  taskData": "my_t
-0000ac30: 6173 6b5f 6461 7461 5f73 7472 696e 6722  ask_data_string"
-0000ac40: 2c0a 2020 2274 6173 6b44 6174 6146 696c  ,.  "taskDataFil
-0000ac50: 6522 3a20 226d 795f 6461 7461 5f66 696c  e": "my_data_fil
-0000ac60: 652e 7478 7422 2c0a 2020 2274 6173 6b54  e.txt",.  "taskT
-0000ac70: 7970 6573 223a 205b 2264 6f63 6b65 7222  ypes": ["docker"
-0000ac80: 5d2c 0a20 2022 7461 736b 7350 6572 576f  ],.  "tasksPerWo
-0000ac90: 726b 6572 223a 2031 2c0a 2020 2275 706c  rker": 1,.  "upl
-0000aca0: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
-0000acb0: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
-0000acc0: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
-0000acd0: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
-0000ace0: 7422 7d5d 2c0a 2020 2276 6370 7573 223a  t"}],.  "vcpus":
-0000acf0: 205b 312c 2034 5d2c 0a20 2022 7665 7269   [1, 4],.  "veri
-0000ad00: 6679 4174 5374 6172 7422 3a20 5b22 7265  fyAtStart": ["re
-0000ad10: 6164 795f 7265 7375 6c74 732e 7478 7422  ady_results.txt"
-0000ad20: 5d2c 0a20 2022 7665 7269 6679 5761 6974  ],.  "verifyWait
-0000ad30: 223a 205b 2277 6169 745f 666f 725f 7265  ": ["wait_for_re
-0000ad40: 7375 6c74 732e 7478 7422 5d2c 0a20 2022  sults.txt"],.  "
-0000ad50: 776f 726b 6572 5461 6773 223a 205b 5d2c  workerTags": [],
-0000ad60: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
-0000ad70: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-0000ad80: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
-0000ad90: 2020 7b7d 0a20 2020 2020 205d 0a20 2020    {}.      ].   
-0000ada0: 207d 0a20 205d 0a7d 0a0a 6060 600a 0a23   }.  ].}..```..#
-0000adb0: 2323 204a 534f 4e20 5072 6f70 6572 7469  ## JSON Properti
-0000adc0: 6573 2061 7420 7468 6520 5461 736b 2047  es at the Task G
-0000add0: 726f 7570 204c 6576 656c 0a0a 5368 6f77  roup Level..Show
-0000ade0: 696e 6720 616c 6c20 706f 7373 6962 6c65  ing all possible
-0000adf0: 2070 726f 7065 7274 6965 7320 6174 2074   properties at t
-0000ae00: 6865 2054 6173 6b20 4772 6f75 7020 6c65  he Task Group le
-0000ae10: 7665 6c3a 0a0a 6060 606a 736f 6e0a 7b0a  vel:..```json.{.
-0000ae20: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
-0000ae30: 5b0a 2020 2020 7b0a 2020 2020 2020 2261  [.    {.      "a
-0000ae40: 7267 756d 656e 7473 223a 205b 312c 2022  rguments": [1, "
-0000ae50: 5457 4f22 5d2c 0a20 2020 2020 2022 6361  TWO"],.      "ca
-0000ae60: 7074 7572 6554 6173 6b4f 7574 7075 7422  ptureTaskOutput"
-0000ae70: 3a20 7472 7565 2c0a 2020 2020 2020 2263  : true,.      "c
-0000ae80: 6f6d 706c 6574 6564 5461 736b 5474 6c22  ompletedTaskTtl"
-0000ae90: 3a20 3130 2c0a 2020 2020 2020 2264 6f63  : 10,.      "doc
-0000aea0: 6b65 7245 6e76 6972 6f6e 6d65 6e74 223a  kerEnvironment":
-0000aeb0: 207b 224d 595f 444f 434b 4552 5f56 4152   {"MY_DOCKER_VAR
-0000aec0: 223a 2031 3030 7d2c 0a20 2020 2020 2022  ": 100},.      "
-0000aed0: 646f 636b 6572 5061 7373 776f 7264 223a  dockerPassword":
-0000aee0: 2022 6d79 5061 7373 776f 7264 222c 0a20   "myPassword",. 
-0000aef0: 2020 2020 2022 646f 636b 6572 5573 6572       "dockerUser
-0000af00: 6e61 6d65 223a 2022 6d79 5573 6572 6e61  name": "myUserna
-0000af10: 6d65 222c 0a20 2020 2020 2022 656e 7669  me",.      "envi
-0000af20: 726f 6e6d 656e 7422 3a20 7b22 4d59 5f56  ronment": {"MY_V
-0000af30: 4152 223a 2031 3030 7d2c 0a20 2020 2020  AR": 100},.     
-0000af40: 2022 6578 636c 7573 6976 6557 6f72 6b65   "exclusiveWorke
-0000af50: 7273 223a 2066 616c 7365 2c0a 2020 2020  rs": false,.    
-0000af60: 2020 2265 7865 6375 7461 626c 6522 3a20    "executable": 
-0000af70: 226d 792d 636f 6e74 6169 6e65 7222 2c0a  "my-container",.
-0000af80: 2020 2020 2020 2266 696e 6973 6849 6641        "finishIfA
-0000af90: 6c6c 5461 736b 7346 696e 6973 6865 6422  llTasksFinished"
-0000afa0: 3a20 7472 7565 2c0a 2020 2020 2020 2266  : true,.      "f
-0000afb0: 696e 6973 6849 6641 6e79 5461 736b 4661  inishIfAnyTaskFa
-0000afc0: 696c 6564 223a 2066 616c 7365 2c0a 2020  iled": false,.  
-0000afd0: 2020 2020 2266 6c61 7474 656e 496e 7075      "flattenInpu
-0000afe0: 7450 6174 6873 223a 2066 616c 7365 2c0a  tPaths": false,.
-0000aff0: 2020 2020 2020 2269 6e70 7574 7322 3a20        "inputs": 
-0000b000: 5b22 6170 702f 6d61 696e 2e70 7922 2c20  ["app/main.py", 
-0000b010: 2261 7070 2f72 6571 7569 7265 6d65 6e74  "app/requirement
-0000b020: 732e 7478 7422 5d2c 0a20 2020 2020 2022  s.txt"],.      "
-0000b030: 696e 7075 7473 4f70 7469 6f6e 616c 223a  inputsOptional":
-0000b040: 205b 226f 7074 696f 6e61 6c2e 7478 7422   ["optional.txt"
-0000b050: 5d2c 0a20 2020 2020 2022 696e 7374 616e  ],.      "instan
-0000b060: 6365 5479 7065 7322 3a20 5b22 7433 612e  ceTypes": ["t3a.
-0000b070: 6d69 6372 6f22 2c20 2274 332e 6d69 6372  micro", "t3.micr
-0000b080: 6f22 5d2c 0a20 2020 2020 2022 6d61 7869  o"],.      "maxi
-0000b090: 6d75 6d54 6173 6b52 6574 7269 6573 223a  mumTaskRetries":
-0000b0a0: 2030 2c0a 2020 2020 2020 226d 6178 576f   0,.      "maxWo
-0000b0b0: 726b 6572 7322 3a20 312c 0a20 2020 2020  rkers": 1,.     
-0000b0c0: 2022 6d69 6e57 6f72 6b65 7273 223a 2031   "minWorkers": 1
-0000b0d0: 2c0a 2020 2020 2020 226e 616d 6522 3a20  ,.      "name": 
-0000b0e0: 2266 6972 7374 2d74 6173 6b2d 6772 6f75  "first-task-grou
-0000b0f0: 7022 2c0a 2020 2020 2020 226f 7574 7075  p",.      "outpu
-0000b100: 7473 223a 205b 2272 6573 756c 7473 2e74  ts": ["results.t
-0000b110: 7874 225d 2c0a 2020 2020 2020 226f 7574  xt"],.      "out
-0000b120: 7075 7473 5265 7175 6972 6564 223a 205b  putsRequired": [
-0000b130: 2272 6573 756c 7473 5f72 6571 7569 7265  "results_require
-0000b140: 642e 7478 7422 5d2c 0a20 2020 2020 2022  d.txt"],.      "
-0000b150: 7072 696f 7269 7479 223a 2030 2e30 2c0a  priority": 0.0,.
-0000b160: 2020 2020 2020 2270 726f 7669 6465 7273        "providers
-0000b170: 223a 205b 2241 5753 225d 2c0a 2020 2020  ": ["AWS"],.    
-0000b180: 2020 2272 616d 223a 205b 302e 352c 2032    "ram": [0.5, 2
-0000b190: 5d2c 0a20 2020 2020 2022 7265 6769 6f6e  ],.      "region
-0000b1a0: 7322 3a20 5b22 6575 2d77 6573 742d 3222  s": ["eu-west-2"
-0000b1b0: 5d2c 0a20 2020 2020 2022 7461 736b 436f  ],.      "taskCo
-0000b1c0: 756e 7422 3a20 352c 0a20 2020 2020 2022  unt": 5,.      "
-0000b1d0: 7461 736b 4461 7461 223a 2022 6d79 5f74  taskData": "my_t
-0000b1e0: 6173 6b5f 6461 7461 5f73 7472 696e 6722  ask_data_string"
-0000b1f0: 2c0a 2020 2020 2020 2274 6173 6b44 6174  ,.      "taskDat
-0000b200: 6146 696c 6522 3a20 226d 795f 6461 7461  aFile": "my_data
-0000b210: 5f66 696c 652e 7478 7422 2c0a 2020 2020  _file.txt",.    
-0000b220: 2020 2274 6173 6b54 7970 6573 223a 205b    "taskTypes": [
-0000b230: 2264 6f63 6b65 7222 5d2c 0a20 2020 2020  "docker"],.     
-0000b240: 2022 7461 736b 7350 6572 576f 726b 6572   "tasksPerWorker
-0000b250: 223a 2031 2c0a 2020 2020 2020 2275 706c  ": 1,.      "upl
-0000b260: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
-0000b270: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
-0000b280: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
-0000b290: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
-0000b2a0: 7422 7d5d 2c0a 2020 2020 2020 2276 6370  t"}],.      "vcp
-0000b2b0: 7573 223a 205b 312c 2034 5d2c 0a20 2020  us": [1, 4],.   
-0000b2c0: 2020 2022 7665 7269 6679 4174 5374 6172     "verifyAtStar
-0000b2d0: 7422 3a20 5b22 7265 6164 795f 7265 7375  t": ["ready_resu
-0000b2e0: 6c74 732e 7478 7422 5d2c 0a20 2020 2020  lts.txt"],.     
-0000b2f0: 2022 7665 7269 6679 5761 6974 223a 205b   "verifyWait": [
-0000b300: 2277 6169 745f 666f 725f 7265 7375 6c74  "wait_for_result
-0000b310: 732e 7478 7422 5d2c 0a20 2020 2020 2022  s.txt"],.      "
-0000b320: 776f 726b 6572 5461 6773 223a 205b 5d2c  workerTags": [],
-0000b330: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-0000b340: 5b0a 2020 2020 2020 2020 7b7d 0a20 2020  [.        {}.   
-0000b350: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
-0000b360: 7b0a 2020 2020 2020 226e 616d 6522 3a20  {.      "name": 
-0000b370: 2273 6563 6f6e 642d 7461 736b 2d67 726f  "second-task-gro
-0000b380: 7570 222c 0a20 2020 2020 2022 6465 7065  up",.      "depe
-0000b390: 6e64 656e 744f 6e22 3a20 2266 6972 7374  ndentOn": "first
-0000b3a0: 2d74 6173 6b2d 6772 6f75 7022 2c0a 2020  -task-group",.  
-0000b3b0: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
-0000b3c0: 2020 2020 2020 207b 7d0a 2020 2020 2020         {}.      
-0000b3d0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
-0000b3e0: 600a 0a23 2323 204a 534f 4e20 5072 6f70  `..### JSON Prop
-0000b3f0: 6572 7469 6573 2061 7420 7468 6520 5461  erties at the Ta
-0000b400: 736b 204c 6576 656c 0a0a 5368 6f77 696e  sk Level..Showin
-0000b410: 6720 616c 6c20 706f 7373 6962 6c65 2070  g all possible p
-0000b420: 726f 7065 7274 6965 7320 6174 2074 6865  roperties at the
-0000b430: 2054 6173 6b20 6c65 7665 6c3a 0a0a 6060   Task level:..``
-0000b440: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
-0000b450: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
-0000b460: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
-0000b470: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-0000b480: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
-0000b490: 3a20 5b31 2c20 325d 2c0a 2020 2020 2020  : [1, 2],.      
-0000b4a0: 2020 2020 2263 6170 7475 7265 5461 736b      "captureTask
-0000b4b0: 4f75 7470 7574 223a 2074 7275 652c 0a20  Output": true,. 
-0000b4c0: 2020 2020 2020 2020 2022 646f 636b 6572           "docker
-0000b4d0: 456e 7669 726f 6e6d 656e 7422 3a20 7b22  Environment": {"
-0000b4e0: 4d59 5f44 4f43 4b45 525f 5641 5222 3a20  MY_DOCKER_VAR": 
-0000b4f0: 3130 307d 2c0a 2020 2020 2020 2020 2020  100},.          
-0000b500: 2264 6f63 6b65 7250 6173 7377 6f72 6422  "dockerPassword"
-0000b510: 3a20 226d 7950 6173 7377 6f72 6422 2c0a  : "myPassword",.
-0000b520: 2020 2020 2020 2020 2020 2264 6f63 6b65            "docke
-0000b530: 7255 7365 726e 616d 6522 3a20 226d 7955  rUsername": "myU
-0000b540: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
-0000b550: 2020 2020 2265 6e76 6972 6f6e 6d65 6e74      "environment
-0000b560: 223a 207b 224d 595f 5641 5222 3a20 3130  ": {"MY_VAR": 10
-0000b570: 307d 2c0a 2020 2020 2020 2020 2020 2265  0},.          "e
-0000b580: 7865 6375 7461 626c 6522 3a20 226d 792d  xecutable": "my-
-0000b590: 636f 6e74 6169 6e65 7222 2c0a 2020 2020  container",.    
-0000b5a0: 2020 2020 2020 2266 6c61 7474 656e 496e        "flattenIn
-0000b5b0: 7075 7450 6174 6873 223a 2066 616c 7365  putPaths": false
-0000b5c0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-0000b5d0: 7574 7322 3a20 5b22 6170 702f 6d61 696e  uts": ["app/main
-0000b5e0: 2e70 7922 2c20 2261 7070 2f72 6571 7569  .py", "app/requi
-0000b5f0: 7265 6d65 6e74 732e 7478 7422 5d2c 0a20  rements.txt"],. 
-0000b600: 2020 2020 2020 2020 2022 696e 7075 7473           "inputs
-0000b610: 4f70 7469 6f6e 616c 223a 205b 226f 7074  Optional": ["opt
-0000b620: 696f 6e61 6c2e 7478 7422 5d2c 0a20 2020  ional.txt"],.   
-0000b630: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-0000b640: 6d79 2d74 6173 6b22 2c0a 2020 2020 2020  my-task",.      
-0000b650: 2020 2020 226f 7574 7075 7473 223a 205b      "outputs": [
-0000b660: 2272 6573 756c 7473 2e74 7874 225d 2c0a  "results.txt"],.
-0000b670: 2020 2020 2020 2020 2020 226f 7574 7075            "outpu
-0000b680: 7473 5265 7175 6972 6564 223a 205b 2272  tsRequired": ["r
-0000b690: 6573 756c 7473 5f72 6571 7569 7265 642e  esults_required.
-0000b6a0: 7478 7422 5d2c 0a20 2020 2020 2020 2020  txt"],.         
-0000b6b0: 2022 7461 736b 4461 7461 223a 2022 6d79   "taskData": "my
-0000b6c0: 5f74 6173 6b5f 6461 7461 5f73 7472 696e  _task_data_strin
-0000b6d0: 6722 2c0a 2020 2020 2020 2020 2020 2274  g",.          "t
-0000b6e0: 6173 6b44 6174 6146 696c 6522 3a20 226d  askDataFile": "m
-0000b6f0: 795f 6461 7461 5f66 696c 652e 7478 7422  y_data_file.txt"
-0000b700: 2c0a 2020 2020 2020 2020 2020 2274 6173  ,.          "tas
-0000b710: 6b54 7970 6522 3a20 2264 6f63 6b65 7222  kType": "docker"
-0000b720: 2c0a 2020 2020 2020 2020 2020 2275 706c  ,.          "upl
-0000b730: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
-0000b740: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
-0000b750: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
-0000b760: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
-0000b770: 7422 7d5d 2c0a 2020 2020 2020 2020 2020  t"}],.          
-0000b780: 2276 6572 6966 7941 7453 7461 7274 223a  "verifyAtStart":
-0000b790: 205b 2272 6561 6479 5f72 6573 756c 7473   ["ready_results
-0000b7a0: 2e74 7874 225d 2c0a 2020 2020 2020 2020  .txt"],.        
-0000b7b0: 2020 2276 6572 6966 7957 6169 7422 3a20    "verifyWait": 
-0000b7c0: 5b22 7761 6974 5f66 6f72 5f72 6573 756c  ["wait_for_resul
-0000b7d0: 7473 2e74 7874 225d 0a20 2020 2020 2020  ts.txt"].       
-0000b7e0: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
-0000b7f0: 0a20 205d 0a7d 0a60 6060 0a0a 2323 2056  .  ].}.```..## V
-0000b800: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
-0000b810: 7469 6f6e 7320 696e 2057 6f72 6b20 5265  tions in Work Re
-0000b820: 7175 6972 656d 656e 7420 5072 6f70 6572  quirement Proper
-0000b830: 7469 6573 0a0a 5661 7269 6162 6c65 2073  ties..Variable s
-0000b840: 7562 7374 6974 7574 696f 6e73 2063 616e  ubstitutions can
-0000b850: 2062 6520 7573 6564 2077 6974 6869 6e20   be used within 
-0000b860: 616e 7920 7072 6f70 6572 7479 2076 616c  any property val
-0000b870: 7565 2069 6e20 544f 4d4c 2063 6f6e 6669  ue in TOML confi
-0000b880: 6775 7261 7469 6f6e 2066 696c 6573 206f  guration files o
-0000b890: 7220 576f 726b 2052 6571 7569 7265 6d65  r Work Requireme
-0000b8a0: 6e74 204a 534f 4e20 6669 6c65 732e 2053  nt JSON files. S
-0000b8b0: 6565 2074 6865 2064 6573 6372 6970 7469  ee the descripti
-0000b8c0: 6f6e 205b 6162 6f76 655d 2823 7661 7269  on [above](#vari
-0000b8d0: 6162 6c65 2d73 7562 7374 6974 7574 696f  able-substitutio
-0000b8e0: 6e73 2920 666f 7220 6d6f 7265 2064 6574  ns) for more det
-0000b8f0: 6169 6c73 206f 6e20 7661 7269 6162 6c65  ails on variable
-0000b900: 2073 7562 7374 6974 7574 696f 6e73 2e20   substitutions. 
-0000b910: 5468 6973 2069 7320 6120 706f 7765 7266  This is a powerf
-0000b920: 756c 2066 6561 7475 7265 2074 6861 7420  ul feature that 
-0000b930: 616c 6c6f 7773 2057 6f72 6b20 5265 7175  allows Work Requ
-0000b940: 6972 656d 656e 7473 2074 6f20 6265 2070  irements to be p
-0000b950: 6172 616d 6574 6572 6973 6564 2062 7920  arameterised by 
-0000b960: 7375 7070 6c79 696e 6720 7661 6c75 6573  supplying values
-0000b970: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
-0000b980: 6c69 6e65 2c20 7669 6120 656e 7669 726f  line, via enviro
-0000b990: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-0000b9a0: 6f72 2076 6961 2074 6865 2054 4f4d 4c20  or via the TOML 
-0000b9b0: 6669 6c65 2e0a 0a23 2323 2054 6173 6b20  file...### Task 
-0000b9c0: 616e 6420 5461 736b 2047 726f 7570 204e  and Task Group N
-0000b9d0: 616d 6520 5375 6273 7469 7475 7469 6f6e  ame Substitution
-0000b9e0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-0000b9f0: 6e75 6d62 6572 696e 6720 616e 6420 6e61  numbering and na
-0000ba00: 6d69 6e67 2073 7562 7374 6974 7574 696f  ming substitutio
-0000ba10: 6e73 2061 7265 2061 7661 696c 6162 6c65  ns are available
-0000ba20: 2066 6f72 2075 7365 2069 6e20 5461 736b   for use in Task
-0000ba30: 2061 6e64 2054 6173 6b20 4772 6f75 7020   and Task Group 
-0000ba40: 6e61 6d69 6e67 2c20 6f6e 6c79 2077 6865  naming, only whe
-0000ba50: 6e20 7468 6520 576f 726b 2052 6571 7569  n the Work Requi
-0000ba60: 7265 6d65 6e74 2069 7320 7370 6563 6966  rement is specif
-0000ba70: 6965 6420 6173 2020 4a53 4f4e 2064 6f63  ied as  JSON doc
-0000ba80: 756d 656e 742c 2069 2e65 2e2c 2074 6865  ument, i.e., the
-0000ba90: 7920 6361 6e20 6265 2075 7365 6420 696e  y can be used in
-0000baa0: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
-0000bab0: 6572 7469 6573 2066 6f72 2054 6173 6b73  erties for Tasks
-0000bac0: 2061 6e64 2054 6173 6b20 4772 6f75 7073   and Task Groups
-0000bad0: 2069 6e20 4a53 4f4e 2073 7065 6369 6669   in JSON specifi
-0000bae0: 6361 7469 6f6e 732e 0a0a 5468 6520 666f  cations...The fo
-0000baf0: 6c6c 6f77 696e 6720 7461 626c 6520 6465  llowing table de
-0000bb00: 6669 6e65 7320 7468 6520 636f 6e74 6578  fines the contex
-0000bb10: 7428 7329 2069 6e20 7768 6963 6820 6561  t(s) in which ea
-0000bb20: 6368 2076 6172 6961 626c 6520 6361 6e20  ch variable can 
-0000bb30: 6265 2075 7365 643a 0a0a 7c20 4469 7265  be used:..| Dire
-0000bb40: 6374 6976 6520 2020 2020 2020 2020 2020  ctive           
-0000bb50: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
-0000bb60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb80: 2020 2020 2020 2020 7c20 5461 736b 207c          | Task |
-0000bb90: 2054 6173 6b20 4772 6f75 7020 7c0a 7c3a   Task Group |.|:
-0000bba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bbb0: 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d  --------|:------
-0000bbc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bbd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bbe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
-0000bbf0: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
-0000bc00: 7c0a 7c20 607b 7b74 6173 6b5f 6e75 6d62  |.| `{{task_numb
-0000bc10: 6572 7d7d 6020 2020 2020 2020 7c20 5468  er}}`       | Th
-0000bc20: 6520 6375 7272 656e 7420 5461 736b 206e  e current Task n
-0000bc30: 756d 6265 7220 2020 2020 2020 2020 2020  umber           
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 7c20 5965 7320 207c 2020 2020 2020 2020  | Yes  |        
-0000bc60: 2020 2020 7c0a 7c20 607b 7b74 6173 6b5f      |.| `{{task_
-0000bc70: 6e61 6d65 7d7d 6020 2020 2020 2020 2020  name}}`         
-0000bc80: 7c20 5468 6520 6375 7272 656e 7420 5461  | The current Ta
-0000bc90: 736b 206e 616d 6520 2020 2020 2020 2020  sk name         
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 2020 2020 7c20 5965 7320 207c 2020 2020      | Yes  |    
-0000bcc0: 2020 2020 2020 2020 7c0a 7c20 607b 7b74          |.| `{{t
-0000bcd0: 6173 6b5f 6772 6f75 705f 6e61 6d65 7d7d  ask_group_name}}
-0000bce0: 6020 2020 7c20 5468 6520 6375 7272 656e  `   | The curren
-0000bcf0: 7420 5461 736b 2047 726f 7570 206e 616d  t Task Group nam
-0000bd00: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-0000bd10: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-0000bd20: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-0000bd30: 607b 7b74 6173 6b5f 636f 756e 747d 7d60  `{{task_count}}`
-0000bd40: 2020 2020 2020 2020 7c20 5468 6520 6e75          | The nu
-0000bd50: 6d62 6572 206f 6620 5461 736b 7320 696e  mber of Tasks in
-0000bd60: 2074 6865 2063 7572 7265 6e74 2054 6173   the current Tas
-0000bd70: 6b20 4772 6f75 7020 2020 2020 7c20 5965  k Group     | Ye
-0000bd80: 7320 207c 2059 6573 2020 2020 2020 2020  s  | Yes        
-0000bd90: 7c0a 7c20 607b 7b74 6173 6b5f 6772 6f75  |.| `{{task_grou
-0000bda0: 705f 6e75 6d62 6572 7d7d 6020 7c20 5468  p_number}}` | Th
-0000bdb0: 6520 6375 7272 656e 7420 5461 736b 2047  e current Task G
-0000bdc0: 726f 7570 206e 756d 6265 7220 2020 2020  roup number     
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 7c20 5965 7320 207c 2059 6573 2020 2020  | Yes  | Yes    
-0000bdf0: 2020 2020 7c0a 7c20 607b 7b74 6173 6b5f      |.| `{{task_
-0000be00: 6772 6f75 705f 636f 756e 747d 7d60 2020  group_count}}`  
-0000be10: 7c20 5468 6520 6e75 6d62 6572 206f 6620  | The number of 
-0000be20: 5461 736b 2047 726f 7570 7320 696e 2074  Task Groups in t
-0000be30: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-0000be40: 656e 7420 7c20 5965 7320 207c 2059 6573  ent | Yes  | Yes
-0000be50: 2020 2020 2020 2020 7c0a 0a49 6e20 6164          |..In ad
-0000be60: 6469 7469 6f6e 2c20 2a2a 5461 736b 732a  dition, **Tasks*
-0000be70: 2a20 6465 6669 6e65 6420 696e 204a 534f  * defined in JSO
-0000be80: 4e20 646f 6375 6d65 6e74 7320 6361 6e20  N documents can 
-0000be90: 7573 6520 616e 7920 6f66 2074 6865 2073  use any of the s
-0000bea0: 7562 7374 6974 7574 696f 6e73 2061 626f  ubstitutions abo
-0000beb0: 7665 2069 6e20 616e 7920 6f66 2074 6865  ve in any of the
-0000bec0: 6972 2070 726f 7065 7274 6965 732c 206e  ir properties, n
-0000bed0: 6f74 206a 7573 7420 606e 616d 6560 2e0a  ot just `name`..
-0000bee0: 0a4e 756d 6265 7273 2061 7265 207a 6572  .Numbers are zer
-0000bef0: 6f2d 7061 6464 6564 2066 6f72 206e 6561  o-padded for nea
-0000bf00: 7420 666f 726d 6174 7469 6e67 2061 6e64  t formatting and
-0000bf10: 2073 6f72 7469 6e67 2c20 652e 672e 2c20   sorting, e.g., 
-0000bf20: 5461 736b 206e 756d 6265 7220 6033 3760  Task number `37`
-0000bf30: 206f 6620 6031 3030 3060 2054 6173 6b73   of `1000` Tasks
-0000bf40: 2077 6f75 6c64 2062 6520 7375 6273 7469   would be substi
-0000bf50: 7475 7465 6420 6173 2060 3030 3337 602e  tuted as `0037`.
-0000bf60: 0a0a 4173 2061 6e20 6578 616d 706c 652c  ..As an example,
-0000bf70: 2074 6865 2066 6f6c 6c6f 7769 6e67 204a   the following J
-0000bf80: 534f 4e20 576f 726b 2052 6571 7569 7265  SON Work Require
-0000bf90: 6d65 6e74 3a0a 0a60 6060 6a73 6f6e 0a7b  ment:..```json.{
-0000bfa0: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
-0000bfb0: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-0000bfc0: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
-0000bfd0: 6772 6f75 705f 7b7b 7461 736b 5f67 726f  group_{{task_gro
-0000bfe0: 7570 5f6e 756d 6265 727d 7d5f 6131 222c  up_number}}_a1",
-0000bff0: 0a20 2020 2020 2022 6578 6563 7574 6162  .      "executab
-0000c000: 6c65 223a 2022 6578 312e 7368 222c 0a20  le": "ex1.sh",. 
-0000c010: 2020 2020 2022 7461 736b 436f 756e 7422       "taskCount"
-0000c020: 3a20 322c 0a20 2020 2020 2022 7461 736b  : 2,.      "task
-0000c030: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
-0000c040: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0000c050: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
-0000c060: 6b5f 6e75 6d62 6572 7d7d 2d6f 662d 7b7b  k_number}}-of-{{
-0000c070: 7461 736b 5f63 6f75 6e74 7d7d 222c 0a20  task_count}}",. 
-0000c080: 2020 2020 2020 2020 2022 656e 7669 726f           "enviro
-0000c090: 6e6d 656e 7422 3a20 7b22 5441 534b 5f4e  nment": {"TASK_N
-0000c0a0: 554d 4245 5222 3a20 227b 7b74 6173 6b5f  UMBER": "{{task_
-0000c0b0: 6e75 6d62 6572 7d7d 227d 0a20 2020 2020  number}}"}.     
-0000c0c0: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
-0000c0d0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-0000c0e0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
-0000c0f0: 5f67 726f 7570 5f7b 7b74 6173 6b5f 6772  _group_{{task_gr
-0000c100: 6f75 705f 6e75 6d62 6572 7d7d 5f62 3122  oup_number}}_b1"
-0000c110: 2c0a 2020 2020 2020 2265 7865 6375 7461  ,.      "executa
-0000c120: 626c 6522 3a20 2265 7832 2e73 6822 2c0a  ble": "ex2.sh",.
-0000c130: 2020 2020 2020 2274 6173 6b43 6f75 6e74        "taskCount
-0000c140: 223a 2032 2c0a 2020 2020 2020 2274 6173  ": 2,.      "tas
-0000c150: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
-0000c160: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
-0000c170: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
-0000c180: 736b 5f6e 756d 6265 727d 7d2d 6f66 2d7b  sk_number}}-of-{
-0000c190: 7b74 6173 6b5f 636f 756e 747d 7d22 0a20  {task_count}}". 
-0000c1a0: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-0000c1b0: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
-0000c1c0: 0a0a 2e2e 2e20 776f 756c 6420 6372 6561  ..... would crea
-0000c1d0: 7465 2054 6173 6b20 4772 6f75 7073 206e  te Task Groups n
-0000c1e0: 616d 6564 2060 6d79 5f74 6173 6b5f 6772  amed `my_task_gr
-0000c1f0: 6f75 705f 315f 6131 6020 616e 6420 606d  oup_1_a1` and `m
-0000c200: 795f 7461 736b 5f67 726f 7570 5f32 5f62  y_task_group_2_b
-0000c210: 3160 2c20 6561 6368 2063 6f6e 7461 696e  1`, each contain
-0000c220: 696e 6720 5461 736b 7320 6e61 6d65 6420  ing Tasks named 
-0000c230: 606d 795f 7461 736b 5f31 2d6f 662d 3260  `my_task_1-of-2`
-0000c240: 2c20 606d 795f 7461 736b 5f32 2d6f 662d  , `my_task_2-of-
-0000c250: 3260 2e0a 0a23 2323 2057 6f72 6b20 5265  2`...### Work Re
-0000c260: 7175 6972 656d 656e 7420 4e61 6d65 2053  quirement Name S
-0000c270: 7562 7374 6974 7574 696f 6e0a 0a54 6865  ubstitution..The
-0000c280: 206e 616d 6520 6f66 2074 6865 2057 6f72   name of the Wor
-0000c290: 6b20 5265 7175 6972 656d 656e 7420 6974  k Requirement it
-0000c2a0: 7365 6c66 2063 616e 2062 6520 7573 6564  self can be used
-0000c2b0: 2076 6961 2074 6865 2076 6172 6961 626c   via the variabl
-0000c2c0: 6520 7375 6273 7469 7475 7469 6f6e 2060  e substitution `
-0000c2d0: 7b7b 7772 5f6e 616d 657d 7d60 2e20 5468  {{wr_name}}`. Th
-0000c2e0: 6973 2063 616e 2062 6520 7573 6564 2061  is can be used a
-0000c2f0: 6e79 7768 6572 6520 696e 2061 2054 4f4d  nywhere in a TOM
-0000c300: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
-0000c310: 6669 6c65 206f 7220 696e 2061 204a 534f  file or in a JSO
-0000c320: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
-0000c330: 6e74 2e0a 0a23 2320 4472 792d 5275 6e6e  nt...## Dry-Runn
-0000c340: 696e 6720 576f 726b 2052 6571 7569 7265  ing Work Require
-0000c350: 6d65 6e74 2053 7562 6d69 7373 696f 6e73  ment Submissions
-0000c360: 0a0a 546f 2065 7861 6d69 6e65 2074 6865  ..To examine the
-0000c370: 204a 534f 4e20 7468 6174 2077 696c 6c20   JSON that will 
-0000c380: 6163 7475 616c 6c79 2062 6520 7365 6e74  actually be sent
-0000c390: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
-0000c3a0: 6720 4150 4920 6166 7465 7220 616c 6c20  g API after all 
-0000c3b0: 7072 6f63 6573 7369 6e67 2c20 7573 6520  processing, use 
-0000c3c0: 7468 6520 602d 2d64 7279 2d72 756e 6020  the `--dry-run` 
-0000c3d0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-0000c3e0: 696f 6e20 7768 656e 2072 756e 6e69 6e67  ion when running
-0000c3f0: 2060 7964 2d73 7562 6d69 7460 2e20 5468   `yd-submit`. Th
-0000c400: 6973 2077 696c 6c20 7072 696e 7420 7468  is will print th
-0000c410: 6520 6675 6c6c 7920 7072 6f63 6573 7365  e fully processe
-0000c420: 6420 4a53 4f4e 2066 6f72 2074 6865 2057  d JSON for the W
-0000c430: 6f72 6b20 5265 7175 6972 656d 656e 742e  ork Requirement.
-0000c440: 204e 6f74 6869 6e67 2077 696c 6c20 6265   Nothing will be
-0000c450: 2073 7562 6d69 7474 6564 2074 6f20 7468   submitted to th
-0000c460: 6520 506c 6174 666f 726d 2e0a 0a54 6865  e Platform...The
-0000c470: 2064 7279 2d72 756e 2069 7320 7573 6566   dry-run is usef
-0000c480: 756c 2066 6f72 2069 6e73 7065 6374 696e  ul for inspectin
-0000c490: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
-0000c4a0: 2061 6c6c 2074 6865 2070 726f 6365 7373   all the process
-0000c4b0: 696e 6720 7468 6174 2773 2062 6565 6e20  ing that's been 
-0000c4c0: 7065 7266 6f72 6d65 642e 2054 6f20 7375  performed. To su
-0000c4d0: 7070 7265 7373 2061 6c6c 206f 7574 7075  ppress all outpu
-0000c4e0: 7420 6578 6365 7074 2066 6f72 2074 6865  t except for the
-0000c4f0: 204a 534f 4e20 6974 7365 6c66 2c20 7573   JSON itself, us
-0000c500: 6520 7468 6520 602d 2d71 7569 6574 6020  e the `--quiet` 
-0000c510: 2860 2d71 6029 2063 6f6d 6d61 6e64 206c  (`-q`) command l
-0000c520: 696e 6520 6f70 7469 6f6e 2e0a 0a4e 6f74  ine option...Not
-0000c530: 6520 7468 6174 2074 6865 2067 656e 6572  e that the gener
-0000c540: 6174 6564 204a 534f 4e20 6973 2061 2063  ated JSON is a c
-0000c550: 6f6e 736f 6c69 6461 7465 6420 666f 726d  onsolidated form
-0000c560: 206f 6620 7768 6174 2077 6f75 6c64 2062   of what would b
-0000c570: 6520 7375 626d 6974 7465 6420 746f 2074  e submitted to t
-0000c580: 6865 2059 656c 6c6f 7744 6f67 2041 5049  he YellowDog API
-0000c590: 2c20 616e 6420 5461 736b 7320 6172 6520  , and Tasks are 
-0000c5a0: 6465 6669 6e65 6420 6469 7265 6374 6c79  defined directly
-0000c5b0: 2077 6974 6869 6e20 7468 6569 7220 5461   within their Ta
-0000c5c0: 736b 2047 726f 7570 7320 666f 7220 6561  sk Groups for ea
-0000c5d0: 7365 206f 6620 636f 6d70 7265 6865 6e73  se of comprehens
-0000c5e0: 696f 6e2e 2049 6e20 6163 7475 616c 2041  ion. In actual A
-0000c5f0: 5049 2073 7562 6d69 7373 696f 6e73 2c20  PI submissions, 
-0000c600: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000c610: 6d65 6e74 2077 6974 6820 6974 7320 5461  ment with its Ta
-0000c620: 736b 2047 726f 7570 7320 6973 2073 7562  sk Groups is sub
-0000c630: 6d69 7474 6564 2066 6972 7374 2c20 616e  mitted first, an
-0000c640: 6420 5461 736b 7320 6172 6520 7468 656e  d Tasks are then
-0000c650: 2061 6464 6564 2074 6f20 5461 736b 2047   added to Task G
-0000c660: 726f 7570 7320 7365 7061 7261 7465 6c79  roups separately
-0000c670: 2069 6e20 7375 6273 6571 7565 6e74 2041   in subsequent A
-0000c680: 5049 2063 616c 6c73 2e0a 0a41 2073 696d  PI calls...A sim
-0000c690: 706c 6520 6578 616d 706c 6520 6f66 2074  ple example of t
-0000c6a0: 6865 204a 534f 4e20 6f75 7470 7574 2069  he JSON output i
-0000c6b0: 7320 7368 6f77 6e20 6265 6c6f 772c 2073  s shown below, s
-0000c6c0: 686f 7769 6e67 2061 2057 6f72 6b20 5265  howing a Work Re
-0000c6d0: 7175 6972 656d 656e 7420 7769 7468 2061  quirement with a
-0000c6e0: 2073 696e 676c 6520 5461 736b 2047 726f   single Task Gro
-0000c6f0: 7570 2c20 636f 6e74 6169 6e69 6e67 2061  up, containing a
-0000c700: 2073 696e 676c 6520 5461 736b 2e0a 0a60   single Task...`
-0000c710: 2520 7964 2d73 7562 6d69 7420 2d2d 6472  % yd-submit --dr
-0000c720: 792d 7275 6e20 2d2d 7175 6965 7460 0a60  y-run --quiet`.`
-0000c730: 6060 6a73 6f6e 0a7b 0a20 2022 6675 6c66  ``json.{.  "fulf
-0000c740: 696c 4f6e 5375 626d 6974 223a 2066 616c  ilOnSubmit": fal
-0000c750: 7365 2c0a 2020 226e 616d 6522 3a20 2270  se,.  "name": "p
-0000c760: 7965 782d 6261 7368 5f32 3330 3131 342d  yex-bash_230114-
-0000c770: 3039 3535 3034 2d35 3361 222c 0a20 2022  095504-53a",.  "
-0000c780: 6e61 6d65 7370 6163 6522 3a20 2270 7965  namespace": "pye
-0000c790: 7861 6d70 6c65 7322 2c0a 2020 2270 7269  xamples",.  "pri
-0000c7a0: 6f72 6974 7922 3a20 302c 0a20 2022 7461  ority": 0,.  "ta
-0000c7b0: 6722 3a20 2270 7965 782d 6261 7368 222c  g": "pyex-bash",
-0000c7c0: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
-0000c7d0: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-0000c7e0: 6669 6e69 7368 4966 416c 6c54 6173 6b73  finishIfAllTasks
-0000c7f0: 4669 6e69 7368 6564 223a 2074 7275 652c  Finished": true,
-0000c800: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
-0000c810: 416e 7954 6173 6b46 6169 6c65 6422 3a20  AnyTaskFailed": 
-0000c820: 6661 6c73 652c 0a20 2020 2020 2022 6e61  false,.      "na
-0000c830: 6d65 223a 2022 7461 736b 5f67 726f 7570  me": "task_group
-0000c840: 5f31 222c 0a20 2020 2020 2022 7072 696f  _1",.      "prio
-0000c850: 7269 7479 223a 2030 2c0a 2020 2020 2020  rity": 0,.      
-0000c860: 2272 756e 5370 6563 6966 6963 6174 696f  "runSpecificatio
-0000c870: 6e22 3a20 7b0a 2020 2020 2020 2020 226d  n": {.        "m
-0000c880: 6178 696d 756d 5461 736b 5265 7472 6965  aximumTaskRetrie
-0000c890: 7322 3a20 302c 0a20 2020 2020 2020 2022  s": 0,.        "
-0000c8a0: 7461 736b 5479 7065 7322 3a20 5b22 6261  taskTypes": ["ba
-0000c8b0: 7368 225d 2c0a 2020 2020 2020 2020 2277  sh"],.        "w
-0000c8c0: 6f72 6b65 7254 6167 7322 3a20 5b22 7079  orkerTags": ["py
-0000c8d0: 6578 2d62 6173 6822 5d0a 2020 2020 2020  ex-bash"].      
-0000c8e0: 7d2c 0a20 2020 2020 2022 7461 736b 7322  },.      "tasks"
-0000c8f0: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-0000c900: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-0000c910: 7473 223a 205b 2270 7965 782d 6261 7368  ts": ["pyex-bash
-0000c920: 5f32 3330 3131 342d 3039 3535 3034 2d35  _230114-095504-5
-0000c930: 3361 2f73 6c65 6570 5f73 6372 6970 742e  3a/sleep_script.
-0000c940: 7368 225d 2c0a 2020 2020 2020 2020 2020  sh"],.          
-0000c950: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-0000c960: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
-0000c970: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
-0000c980: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-0000c990: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
-0000c9a0: 5061 7474 6572 6e22 3a20 2270 7965 782d  Pattern": "pyex-
-0000c9b0: 6261 7368 5f32 3330 3131 342d 3039 3535  bash_230114-0955
-0000c9c0: 3034 2d35 3361 2f73 6c65 6570 5f73 6372  04-53a/sleep_scr
-0000c9d0: 6970 742e 7368 222c 0a20 2020 2020 2020  ipt.sh",.       
-0000c9e0: 2020 2020 2020 2022 736f 7572 6365 223a         "source":
-0000c9f0: 2022 5441 534b 5f4e 414d 4553 5041 4345   "TASK_NAMESPACE
-0000ca00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000ca10: 2022 7665 7269 6669 6361 7469 6f6e 223a   "verification":
-0000ca20: 2022 5645 5249 4659 5f57 4149 5422 0a20   "VERIFY_WAIT". 
-0000ca30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0000ca40: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-0000ca50: 2020 2020 226e 616d 6522 3a20 2274 6173      "name": "tas
-0000ca60: 6b5f 3031 222c 0a20 2020 2020 2020 2020  k_01",.         
-0000ca70: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
-0000ca80: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
-0000ca90: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
-0000caa0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-0000cab0: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
-0000cac0: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
-0000cad0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-0000cae0: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
-0000caf0: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
-0000cb00: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
-0000cb10: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2323  }.  ].}.```..###
-0000cb20: 2053 7562 6d69 7474 696e 6720 2752 6177   Submitting 'Raw
-0000cb30: 2720 4a53 4f4e 2057 6f72 6b20 5265 7175  ' JSON Work Requ
-0000cb40: 6972 656d 656e 7420 5370 6563 6966 6963  irement Specific
-0000cb50: 6174 696f 6e73 0a0a 4974 2773 2070 6f73  ations..It's pos
-0000cb60: 7369 626c 6520 746f 2075 7365 2074 6865  sible to use the
-0000cb70: 204a 534f 4e20 6f75 7470 7574 206f 6620   JSON output of 
-0000cb80: 6079 642d 7375 626d 6974 202d 2d64 7279  `yd-submit --dry
-0000cb90: 2d72 756e 6020 2873 7563 6820 6173 2074  -run` (such as t
-0000cba0: 6865 2065 7861 6d70 6c65 2061 626f 7665  he example above
-0000cbb0: 2920 6173 2061 2073 656c 662d 636f 6e74  ) as a self-cont
-0000cbc0: 6169 6e65 642c 2066 756c 6c79 2d73 7065  ained, fully-spe
-0000cbd0: 6369 6669 6564 2057 6f72 6b20 5265 7175  cified Work Requ
-0000cbe0: 6972 656d 656e 7420 7370 6563 6966 6963  irement specific
-0000cbf0: 6174 696f 6e2c 2075 7369 6e67 2074 6865  ation, using the
-0000cc00: 2060 2d2d 6a73 6f6e 2d72 6177 6020 286f   `--json-raw` (o
-0000cc10: 7220 602d 6a60 2920 636f 6d6d 616e 6420  r `-j`) command 
-0000cc20: 6c69 6e65 206f 7074 696f 6e2c 2069 2e65  line option, i.e
-0000cc30: 2e3a 2060 7964 2d73 7562 6d69 7420 2d2d  .: `yd-submit --
-0000cc40: 6a73 6f6e 2d72 6177 203c 6669 6c65 6e61  json-raw <filena
-0000cc50: 6d65 2e6a 736f 6e3e 602e 0a0a 5468 6973  me.json>`...This
-0000cc60: 2077 696c 6c20 7375 626d 6974 2074 6865   will submit the
-0000cc70: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-0000cc80: 742c 2074 6865 6e20 6164 6420 616c 6c20  t, then add all 
-0000cc90: 7468 6520 7370 6563 6966 6965 6420 5461  the specified Ta
-0000cca0: 736b 732e 0a0a 4e6f 7465 2074 6861 7420  sks...Note that 
-0000ccb0: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
-0000ccc0: 7574 696f 6e73 202a 2a63 616e 2a2a 2062  utions **can** b
-0000ccd0: 6520 7573 6564 2069 6e20 7468 6520 7261  e used in the ra
-0000cce0: 7720 4a53 4f4e 2066 696c 652c 206a 7573  w JSON file, jus
-0000ccf0: 7420 6173 2069 6e20 7468 6520 6f74 6865  t as in the othe
-0000cd00: 7220 576f 726b 2052 6571 7569 7265 6d65  r Work Requireme
-0000cd10: 6e74 204a 534f 4e20 6578 616d 706c 6573  nt JSON examples
-0000cd20: 2c20 6275 7420 7468 6572 6520 6973 206e  , but there is n
-0000cd30: 6f20 7072 6f70 6572 7479 2069 6e68 6572  o property inher
-0000cd40: 6974 616e 6365 2c20 696e 636c 7564 696e  itance, includin
-0000cd50: 6720 6672 6f6d 2074 6865 2060 5b77 6f72  g from the `[wor
-0000cd60: 6b52 6571 7569 7265 6d65 6e74 5d60 2073  kRequirement]` s
-0000cd70: 6563 7469 6f6e 206f 6620 7468 6520 544f  ection of the TO
-0000cd80: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-0000cd90: 206f 7220 6672 6f6d 2057 6f72 6b20 5265   or from Work Re
-0000cda0: 7175 6972 656d 656e 7420 7072 6f70 6572  quirement proper
-0000cdb0: 7469 6573 2073 7570 706c 6965 6420 6f6e  ties supplied on
-0000cdc0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-0000cdd0: 652e 0a0a 4e6f 7465 2074 6861 7420 7468  e...Note that th
-0000cde0: 6572 6520 6973 206e 6f20 6175 746f 6d61  ere is no automa
-0000cdf0: 7469 6320 6669 6c65 2075 706c 6f61 6420  tic file upload 
-0000ce00: 7768 656e 2075 7369 6e67 2074 6869 7320  when using this 
-0000ce10: 6f70 7469 6f6e 2c20 736f 2061 6e79 2066  option, so any f
-0000ce20: 696c 6573 2072 6571 7569 7265 6420 6174  iles required at
-0000ce30: 2074 6865 2073 7461 7274 206f 6620 7468   the start of th
-0000ce40: 6520 7461 736b 2028 7370 6563 6966 6965  e task (specifie
-0000ce50: 6420 7573 696e 6720 6056 4552 4946 595f  d using `VERIFY_
-0000ce60: 4154 5f53 5441 5254 6029 206d 7573 7420  AT_START`) must 
-0000ce70: 6265 2070 7265 7365 6e74 2062 6566 6f72  be present befor
-0000ce80: 6520 7468 6520 5461 736b 7320 6172 6520  e the Tasks are 
-0000ce90: 7570 6c6f 6164 6564 2c20 6f72 2074 6865  uploaded, or the
-0000cea0: 2054 6173 6b73 2077 696c 6c20 6661 696c   Tasks will fail
-0000ceb0: 2069 6d6d 6564 6961 7465 6c79 2e20 5468   immediately. Th
-0000cec0: 6520 6079 642d 7570 6c6f 6164 6020 636f  e `yd-upload` co
-0000ced0: 6d6d 616e 6420 6361 6e20 6265 2075 7365  mmand can be use
-0000cee0: 6420 746f 2075 706c 6f61 6420 7468 6573  d to upload thes
-0000cef0: 6520 6669 6c65 732c 2061 6e64 2060 7964  e files, and `yd
-0000cf00: 2d73 7562 6d69 7460 2077 696c 6c20 7061  -submit` will pa
-0000cf10: 7573 6520 746f 2061 6c6c 6f77 2074 6869  use to allow thi
-0000cf20: 7320 746f 2068 6170 7065 6e2e 0a0a 2323  s to happen...##
-0000cf30: 2046 696c 6520 5374 6f72 6167 6520 4c6f   File Storage Lo
-0000cf40: 6361 7469 6f6e 7320 616e 6420 4669 6c65  cations and File
-0000cf50: 2055 7361 6765 0a0a 5468 6973 2073 6563   Usage..This sec
-0000cf60: 7469 6f6e 2064 6973 6375 7373 6573 2068  tion discusses h
-0000cf70: 6f77 2074 6f20 7570 6c6f 6164 2066 696c  ow to upload fil
-0000cf80: 6573 2066 726f 6d20 6c6f 6361 6c20 7374  es from local st
-0000cf90: 6f72 6167 6520 746f 2074 6865 2059 656c  orage to the Yel
-0000cfa0: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
-0000cfb0: 6f72 652c 2068 6f77 2074 686f 7365 2066  ore, how those f
-0000cfc0: 696c 6573 2061 7265 2074 7261 6e73 6665  iles are transfe
-0000cfd0: 7272 6564 2074 6f20 576f 726b 6572 204e  rred to Worker N
-0000cfe0: 6f64 6573 2066 6f72 2054 6173 6b20 7072  odes for Task pr
-0000cff0: 6f63 6573 7369 6e67 2c20 686f 7720 7468  ocessing, how th
-0000d000: 6520 7265 7375 6c74 7320 6f66 2054 6173  e results of Tas
-0000d010: 6b20 7072 6f63 6573 7369 6e67 2061 7265  k processing are
-0000d020: 2072 6574 7572 6e65 6420 6279 2057 6f72   returned by Wor
-0000d030: 6b65 7220 4e6f 6465 732c 2061 6e64 2068  ker Nodes, and h
-0000d040: 6f77 2066 696c 6573 2061 7265 2074 7261  ow files are tra
-0000d050: 6e73 6665 7272 6564 2062 6163 6b20 6672  nsferred back fr
-0000d060: 6f6d 2074 6865 2059 656c 6c6f 7744 6f67  om the YellowDog
-0000d070: 204f 626a 6563 7420 5374 6f72 6520 746f   Object Store to
-0000d080: 206c 6f63 616c 2073 746f 7261 6765 2e0a   local storage..
-0000d090: 0a23 2323 2046 696c 6573 2055 706c 6f61  .### Files Uploa
-0000d0a0: 6465 6420 746f 2074 6865 204f 626a 6563  ded to the Objec
-0000d0b0: 7420 5374 6f72 6520 6672 6f6d 204c 6f63  t Store from Loc
-0000d0c0: 616c 2053 746f 7261 6765 0a0a 2323 2323  al Storage..####
-0000d0d0: 2046 696c 6573 2069 6e20 7468 6520 6069   Files in the `i
-0000d0e0: 6e70 7574 7360 204c 6973 740a 0a57 6865  nputs` List..Whe
-0000d0f0: 6e20 6120 576f 726b 2052 6571 7569 7265  n a Work Require
-0000d100: 6d65 6e74 2069 7320 7375 626d 6974 7465  ment is submitte
-0000d110: 6420 7573 696e 6720 6079 642d 7375 626d  d using `yd-subm
-0000d120: 6974 602c 2066 696c 6573 2061 7265 2075  it`, files are u
-0000d130: 706c 6f61 6465 6420 746f 2074 6865 2059  ploaded to the Y
-0000d140: 656c 6c6f 7744 6f67 204f 626a 6563 7420  ellowDog Object 
-0000d150: 5374 6f72 6520 6966 2074 6865 7927 7265  Store if they're
-0000d160: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
-0000d170: 206c 6973 7420 6f66 2066 696c 6573 2069   list of files i
-0000d180: 6e20 7468 6520 6069 6e70 7574 7360 2070  n the `inputs` p
-0000d190: 726f 7065 7274 792e 2028 466f 7220 7468  roperty. (For th
-0000d1a0: 6520 6361 7365 206f 6620 7468 6520 6062  e case of the `b
-0000d1b0: 6173 6860 2054 6173 6b20 5479 7065 2c20  ash` Task Type, 
-0000d1c0: 7468 6520 7363 7269 7074 2073 7065 6369  the script speci
-0000d1d0: 6669 6564 2069 6e20 7468 6520 6065 7865  fied in the `exe
-0000d1e0: 6375 7461 626c 6560 2070 726f 7065 7274  cutable` propert
-0000d1f0: 7920 6973 2061 6c73 6f20 6175 746f 6d61  y is also automa
-0000d200: 7469 6361 6c6c 7920 7570 6c6f 6164 6564  tically uploaded
-0000d210: 2061 7320 6120 636f 6e76 656e 6965 6e63   as a convenienc
-0000d220: 652c 2065 7665 6e20 6966 206e 6f74 2069  e, even if not i
-0000d230: 6e63 6c75 6465 6420 696e 2074 6865 2060  ncluded in the `
-0000d240: 696e 7075 7473 6020 6c69 7374 2e29 0a0a  inputs` list.)..
-0000d250: 4669 6c65 7320 6172 6520 7570 6c6f 6164  Files are upload
-0000d260: 6564 2074 6f20 7468 6520 4e61 6d65 7370  ed to the Namesp
-0000d270: 6163 6520 7370 6563 6966 6965 6420 696e  ace specified in
-0000d280: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
-0000d290: 6f6e 2e20 5769 7468 696e 2074 6865 204e  on. Within the N
-0000d2a0: 616d 6573 7061 6365 2c20 6561 6368 2057  amespace, each W
-0000d2b0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-0000d2c0: 6861 7320 6120 7365 7061 7261 7465 2066  has a separate f
-0000d2d0: 6f6c 6465 7220 7468 6174 2073 6861 7265  older that share
-0000d2e0: 7320 7468 6520 6e61 6d65 206f 6620 7468  s the name of th
-0000d2f0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-0000d300: 6e74 2c20 616e 6420 696e 2077 6869 6368  nt, and in which
-0000d310: 2061 6c6c 2066 696c 6573 2072 656c 6174   all files relat
-0000d320: 6564 2074 6f20 7468 6520 576f 726b 2052  ed to the Work R
-0000d330: 6571 7569 7265 6d65 6e74 2061 7265 2073  equirement are s
-0000d340: 746f 7265 642e 0a0a 312e 2046 696c 6573  tored...1. Files
-0000d350: 2074 6f20 6265 2075 706c 6f61 6465 6420   to be uploaded 
-0000d360: 7468 6174 2061 7265 2069 6e20 7468 6520  that are in the 
-0000d370: 2a2a 7361 6d65 2064 6972 6563 746f 7279  **same directory
-0000d380: 2061 7320 7468 6520 576f 726b 2052 6571   as the Work Req
-0000d390: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
-0000d3a0: 6361 7469 6f6e 2a2a 2028 7468 6520 544f  cation** (the TO
-0000d3b0: 4d4c 206f 7220 4a53 4f4e 2066 696c 6529  ML or JSON file)
-0000d3c0: 2061 7265 2075 706c 6f61 6465 6420 746f   are uploaded to
-0000d3d0: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
-0000d3e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-0000d3f0: 7420 666f 6c64 6572 2e0a 0a0a 322e 2046  t folder....2. F
-0000d400: 696c 6573 2074 6f20 6265 2075 706c 6f61  iles to be uploa
-0000d410: 6465 6420 7468 6174 2061 7265 2069 6e20  ded that are in 
-0000d420: 2a2a 7375 6264 6972 6563 746f 7269 6573  **subdirectories
-0000d430: 2062 656c 6f77 2074 6865 2057 6f72 6b20   below the Work 
-0000d440: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
-0000d450: 6966 6963 6174 696f 6e2c 206f 7220 7768  ification, or wh
-0000d460: 6572 6520 6162 736f 6c75 7465 2070 6174  ere absolute pat
-0000d470: 686e 616d 6573 2061 7265 2073 7570 706c  hnames are suppl
-0000d480: 6965 642a 2a20 6172 6520 706c 6163 6564  ied** are placed
-0000d490: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
-0000d4a0: 746f 7265 2069 6e20 6469 7265 6374 6f72  tore in director
-0000d4b0: 6965 7320 7468 6174 206d 6972 726f 7220  ies that mirror 
-0000d4c0: 7468 6569 7220 6c6f 6361 6c20 7374 6f72  their local stor
-0000d4d0: 6167 6520 6c6f 6361 7469 6f6e 732e 0a0a  age locations...
-0000d4e0: 0a33 2e20 4669 6c65 7320 746f 2062 6520  .3. Files to be 
-0000d4f0: 7570 6c6f 6164 6564 2074 6861 7420 6172  uploaded that ar
-0000d500: 6520 696e 202a 2a64 6972 6563 746f 7269  e in **directori
-0000d510: 6573 2072 656c 6174 6976 6520 746f 2074  es relative to t
-0000d520: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-0000d530: 656e 7420 7370 6563 6966 6963 6174 696f  ent specificatio
-0000d540: 6e2c 2075 7369 6e67 2060 2e2e 6020 7265  n, using `..` re
-0000d550: 6c61 7469 7665 2070 6174 6873 2a2a 2061  lative paths** a
-0000d560: 7265 2070 6c61 6365 6420 696e 204f 626a  re placed in Obj
-0000d570: 6563 7420 5374 6f72 6520 6469 7265 6374  ect Store direct
-0000d580: 6f72 6965 7320 696e 2077 6869 6368 2074  ories in which t
-0000d590: 6865 2060 2e2e 6020 7061 7274 7320 6f66  he `..` parts of
-0000d5a0: 2074 6865 2070 6174 686e 616d 6520 6172   the pathname ar
-0000d5b0: 6520 7265 706c 6163 6564 2077 6974 6820  e replaced with 
-0000d5c0: 616e 2069 6e74 6567 6572 2063 6f75 6e74  an integer count
-0000d5d0: 206f 6620 7468 6520 6e75 6d62 6572 206f   of the number o
-0000d5e0: 6620 602e 2e60 2065 6e74 7269 6573 2028  f `..` entries (
-0000d5f0: 6265 6361 7573 6520 7765 2063 616e 2774  because we can't
-0000d600: 2075 7365 2074 6865 2060 2e2e 6020 7265   use the `..` re
-0000d610: 6c61 7469 7665 2066 6f72 6d20 696e 2074  lative form in t
-0000d620: 6865 204f 626a 6563 7420 5374 6f72 6529  he Object Store)
-0000d630: 2e0a 0a41 7373 756d 696e 6720 6120 4e61  ...Assuming a Na
-0000d640: 6d65 7370 6163 6520 6361 6c6c 6564 2060  mespace called `
-0000d650: 6465 7665 6c6f 706d 656e 7460 2061 6e64  development` and
-0000d660: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
-0000d670: 656e 7420 6e61 6d65 6420 6074 6573 7472  ent named `testr
-0000d680: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
-0000d690: 2d37 6432 602c 2074 6865 2066 6f6c 6c6f  -7d2`, the follo
-0000d6a0: 7769 6e67 206c 6f63 6174 696f 6e73 2061  wing locations a
-0000d6b0: 7265 2075 7365 6420 7768 656e 2075 706c  re used when upl
-0000d6c0: 6f61 6469 6e67 2066 696c 6573 2066 6f6c  oading files fol
-0000d6d0: 6c6f 7769 6e67 2074 6865 2070 6174 7465  lowing the patte
-0000d6e0: 726e 7320 6162 6f76 653a 0a0a 6060 6073  rns above:..```s
-0000d6f0: 6865 6c6c 0a22 696e 7075 7473 2220 3a20  hell."inputs" : 
-0000d700: 5b22 6669 6c65 5f31 2e74 7874 225d 202d  ["file_1.txt"] -
-0000d710: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
-0000d720: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000d730: 3034 3034 2d37 6432 2f66 696c 655f 312e  0404-7d2/file_1.
-0000d740: 7478 740a 2269 6e70 7574 7322 203a 205b  txt."inputs" : [
-0000d750: 2264 6576 2f66 696c 655f 312e 7478 7422  "dev/file_1.txt"
-0000d760: 5d20 2d3e 2064 6576 656c 6f70 6d65 6e74  ] -> development
-0000d770: 3a3a 7465 7374 7275 6e5f 3232 3131 3038  ::testrun_221108
-0000d780: 2d31 3230 3430 342d 3764 322f 6465 762f  -120404-7d2/dev/
-0000d790: 6669 6c65 5f31 2e74 7874 0a22 696e 7075  file_1.txt."inpu
-0000d7a0: 7473 2220 3a20 5b22 2f68 6f6d 652f 6465  ts" : ["/home/de
-0000d7b0: 762f 6669 6c65 5f31 2e74 7874 225d 202d  v/file_1.txt"] -
-0000d7c0: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
-0000d7d0: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000d7e0: 3034 3034 2d37 6432 2f68 6f6d 652f 6465  0404-7d2/home/de
-0000d7f0: 762f 6669 6c65 5f31 2e74 7874 0a22 696e  v/file_1.txt."in
-0000d800: 7075 7473 2220 3a20 5b22 2e2e 2f64 6576  puts" : ["../dev
-0000d810: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
-0000d820: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
-0000d830: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
-0000d840: 3430 342d 3764 322f 312f 6465 762f 6669  404-7d2/1/dev/fi
-0000d850: 6c65 5f31 2e74 7874 0a22 696e 7075 7473  le_1.txt."inputs
-0000d860: 2220 3a20 5b22 2e2e 2f2e 2e2f 6465 762f  " : ["../../dev/
-0000d870: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000d880: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
-0000d890: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
-0000d8a0: 3034 2d37 6432 2f32 2f64 6576 2f66 696c  04-7d2/2/dev/fil
-0000d8b0: 655f 312e 7478 740a 6060 600a 0a2a 2a55  e_1.txt.```..**U
-0000d8c0: 7369 6e67 2060 666c 6174 7465 6e55 706c  sing `flattenUpl
-0000d8d0: 6f61 6450 6174 6873 602a 2a0a 0a54 6865  oadPaths`**..The
-0000d8e0: 2060 666c 6174 7465 6e55 706c 6f61 6450   `flattenUploadP
-0000d8f0: 6174 6873 6020 7072 6f70 6572 7479 2063  aths` property c
-0000d900: 616e 2062 6520 7573 6564 2074 6f20 7375  an be used to su
-0000d910: 7070 7265 7373 2074 6865 206d 6972 726f  ppress the mirro
-0000d920: 7269 6e67 206f 6620 616e 7920 6c6f 6361  ring of any loca
-0000d930: 6c20 6469 7265 6374 6f72 7920 7374 7275  l directory stru
-0000d940: 6374 7572 6520 7768 656e 2075 706c 6f61  cture when uploa
-0000d950: 6469 6e67 2066 696c 6573 2074 6f20 7468  ding files to th
-0000d960: 6520 4f62 6a65 6374 2053 746f 7265 2e20  e Object Store. 
-0000d970: 4966 2073 6574 2074 6f20 6074 7275 6560  If set to `true`
-0000d980: 2c20 616c 6c20 6669 6c65 7320 7769 6c6c  , all files will
-0000d990: 2062 6520 7570 6c6f 6164 6564 2074 6f20   be uploaded to 
-0000d9a0: 7468 6520 726f 6f74 206f 6620 7468 6520  the root of the 
-0000d9b0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000d9c0: 2066 6f6c 6465 722e 2046 6f72 2065 7861   folder. For exa
-0000d9d0: 6d70 6c65 3a0a 0a60 6060 7368 656c 6c0a  mple:..```shell.
-0000d9e0: 2269 6e70 7574 7322 203a 205b 2266 696c  "inputs" : ["fil
-0000d9f0: 655f 312e 7478 7422 5d20 2d3e 2064 6576  e_1.txt"] -> dev
-0000da00: 656c 6f70 6d65 6e74 3a3a 7465 7374 7275  elopment::testru
-0000da10: 6e5f 3232 3131 3038 2d31 3230 3430 342d  n_221108-120404-
-0000da20: 3764 322f 6669 6c65 5f31 2e74 7874 0a22  7d2/file_1.txt."
-0000da30: 696e 7075 7473 2220 3a20 5b22 6465 762f  inputs" : ["dev/
-0000da40: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000da50: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
-0000da60: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
-0000da70: 3034 2d37 6432 2f66 696c 655f 312e 7478  04-7d2/file_1.tx
-0000da80: 740a 2269 6e70 7574 7322 203a 205b 222f  t."inputs" : ["/
-0000da90: 686f 6d65 2f64 6576 2f66 696c 655f 312e  home/dev/file_1.
-0000daa0: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
-0000dab0: 6d65 6e74 3a3a 7465 7374 7275 6e5f 3232  ment::testrun_22
-0000dac0: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
-0000dad0: 6669 6c65 5f31 2e74 7874 0a22 696e 7075  file_1.txt."inpu
-0000dae0: 7473 2220 3a20 5b22 2e2e 2f64 6576 2f66  ts" : ["../dev/f
-0000daf0: 696c 655f 312e 7478 7422 5d20 2d3e 2064  ile_1.txt"] -> d
-0000db00: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
-0000db10: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000db20: 342d 3764 322f 6669 6c65 5f31 2e74 7874  4-7d2/file_1.txt
-0000db30: 0a22 696e 7075 7473 2220 3a20 5b22 2e2e  ."inputs" : ["..
-0000db40: 2f2e 2e2f 6465 762f 6669 6c65 5f31 2e74  /../dev/file_1.t
-0000db50: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
-0000db60: 656e 743a 3a74 6573 7472 756e 5f32 3231  ent::testrun_221
-0000db70: 3130 382d 3132 3034 3034 2d37 6432 2f66  108-120404-7d2/f
-0000db80: 696c 655f 312e 7478 740a 6060 600a 0a54  ile_1.txt.```..T
-0000db90: 6865 2070 726f 7065 7274 7920 6465 6661  he property defa
-0000dba0: 756c 7420 6973 2060 6661 6c73 6560 2e20  ult is `false`. 
-0000dbb0: 5468 6973 2070 726f 7065 7274 7920 2a2a  This property **
-0000dbc0: 6361 6e20 6f6e 6c79 2062 6520 7365 7420  can only be set 
-0000dbd0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
-0000dbe0: 6972 656d 656e 7420 6c65 7665 6c2a 2a20  irement level** 
-0000dbf0: 616e 6420 7769 6c6c 2074 6865 7265 666f  and will therefo
-0000dc00: 7265 2061 7070 6c79 2074 6f20 616c 6c20  re apply to all 
-0000dc10: 5461 736b 2047 726f 7570 7320 616e 6420  Task Groups and 
-0000dc20: 5461 736b 7320 7769 7468 696e 2061 2057  Tasks within a W
-0000dc30: 6f72 6b20 5265 7175 6972 656d 656e 742e  ork Requirement.
-0000dc40: 0a0a 5768 656e 2066 696c 6573 2061 7070  ..When files app
-0000dc50: 6561 7220 696e 2074 6865 2060 696e 7075  ear in the `inpu
-0000dc60: 7473 6020 6c69 7374 2c20 7468 6579 2061  ts` list, they a
-0000dc70: 7265 2061 6c73 6f20 6175 746f 6d61 7469  re also automati
-0000dc80: 6361 6c6c 7920 6164 6465 6420 746f 2074  cally added to t
-0000dc90: 6865 206c 6973 7420 6f66 2066 696c 6573  he list of files
-0000dca0: 2072 6571 7569 7265 6420 6279 2074 6865   required by the
-0000dcb0: 2072 656c 6576 616e 7420 5461 736b 2873   relevant Task(s
-0000dcc0: 2920 6173 2060 5665 7269 6679 4174 5374  ) as `VerifyAtSt
-0000dcd0: 6172 7460 2064 6570 656e 6465 6e63 6965  art` dependencie
-0000dce0: 732e 0a0a 2323 2323 2046 696c 6573 2069  s...#### Files i
-0000dcf0: 6e20 7468 6520 6075 706c 6f61 6446 696c  n the `uploadFil
-0000dd00: 6573 6020 4c69 7374 0a0a 5468 6520 6075  es` List..The `u
-0000dd10: 706c 6f61 6446 696c 6573 6020 7072 6f70  ploadFiles` prop
-0000dd20: 6572 7479 2061 6c6c 6f77 7320 6d6f 7265  erty allows more
-0000dd30: 2066 6c65 7869 626c 6520 636f 6e74 726f   flexible contro
-0000dd40: 6c20 6f76 6572 2074 6865 2066 696c 6573  l over the files
-0000dd50: 2074 6f20 6265 2075 706c 6f61 6465 6420   to be uploaded 
-0000dd60: 6672 6f6d 206c 6f63 616c 2073 746f 7261  from local stora
-0000dd70: 6765 2074 6f20 7468 6520 4f62 6a65 6374  ge to the Object
-0000dd80: 2053 746f 7265 2077 6865 6e20 6079 642d   Store when `yd-
-0000dd90: 7375 626d 6974 6020 6973 2072 756e 2e20  submit` is run. 
-0000dda0: 5468 6520 7072 6f70 6572 7479 2063 616e  The property can
-0000ddb0: 2062 6520 7573 6564 2061 7420 616c 6c20   be used at all 
-0000ddc0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000ddd0: 206c 6576 656c 732c 2066 726f 6d20 7468   levels, from th
-0000dde0: 6520 544f 4d4c 2066 696c 6520 7468 726f  e TOML file thro
-0000ddf0: 7567 6820 746f 2069 6e64 6976 6964 7561  ugh to individua
-0000de00: 6c20 5461 736b 2073 7065 6369 6669 6361  l Task specifica
-0000de10: 7469 6f6e 732e 0a0a 5468 6520 7072 6f70  tions...The prop
-0000de20: 6572 7479 2069 7320 7375 7070 6c69 6564  erty is supplied
-0000de30: 2061 7320 6120 6c69 7374 206f 6620 6469   as a list of di
-0000de40: 6374 696f 6e61 7279 2069 7465 6d73 2c20  ctionary items, 
-0000de50: 6561 6368 206f 6620 7768 6963 6820 6d75  each of which mu
-0000de60: 7374 2069 6e63 6c75 6465 2074 6865 2070  st include the p
-0000de70: 726f 7065 7274 6965 7320 606c 6f63 616c  roperties `local
-0000de80: 5061 7468 6020 616e 6420 6075 706c 6f61  Path` and `uploa
-0000de90: 6450 6174 6860 2e20 0a0a 2d20 606c 6f63  dPath`. ..- `loc
-0000dea0: 616c 5061 7468 6020 7370 6563 6966 6965  alPath` specifie
-0000deb0: 7320 7468 6520 7061 7468 6e61 6d65 206f  s the pathname o
-0000dec0: 6620 7468 6520 6669 6c65 206f 6e20 6c6f  f the file on lo
-0000ded0: 6361 6c20 7374 6f72 6167 650a 2d20 6075  cal storage.- `u
-0000dee0: 706c 6f61 6450 6174 6860 2073 7065 6369  ploadPath` speci
-0000def0: 6669 6573 2074 6865 206e 616d 6520 616e  fies the name an
-0000df00: 6420 6c6f 6361 7469 6f6e 206f 6620 7468  d location of th
-0000df10: 6520 6669 6c65 2773 2064 6573 7469 6e61  e file's destina
-0000df20: 7469 6f6e 2069 6e20 7468 6520 4f62 6a65  tion in the Obje
-0000df30: 6374 2053 746f 7265 0a0a 466f 7220 6578  ct Store..For ex
-0000df40: 616d 706c 652c 2069 6e20 544f 4d4c 3a0a  ample, in TOML:.
-0000df50: 6060 6074 6f6d 6c0a 7570 6c6f 6164 4669  ```toml.uploadFi
-0000df60: 6c65 7320 3d20 5b0a 2020 2020 7b6c 6f63  les = [.    {loc
-0000df70: 616c 5061 7468 203d 2022 6669 6c65 5f31  alPath = "file_1
-0000df80: 2e74 7874 222c 2075 706c 6f61 6450 6174  .txt", uploadPat
-0000df90: 6820 3d20 2266 696c 655f 312e 7478 7422  h = "file_1.txt"
-0000dfa0: 7d2c 0a20 2020 207b 6c6f 6361 6c50 6174  },.    {localPat
-0000dfb0: 6820 3d20 2264 6972 5f32 2f66 696c 655f  h = "dir_2/file_
-0000dfc0: 322e 7478 7422 2c20 7570 6c6f 6164 5061  2.txt", uploadPa
-0000dfd0: 7468 203d 2022 3a3a 6669 6c65 5f32 2e74  th = "::file_2.t
-0000dfe0: 7874 227d 2c0a 2020 2020 7b6c 6f63 616c  xt"},.    {local
-0000dff0: 5061 7468 203d 2022 6669 6c65 5f33 2e74  Path = "file_3.t
-0000e000: 7874 222c 2075 706c 6f61 6450 6174 6820  xt", uploadPath 
-0000e010: 3d20 226f 7468 6572 5f6e 616d 6573 7061  = "other_namespa
-0000e020: 6365 3a3a 6669 6c65 5f33 2e74 7874 227d  ce::file_3.txt"}
-0000e030: 0a5d 0a60 6060 0a41 6e64 2069 6e20 4a53  .].```.And in JS
-0000e040: 4f4e 2c20 7769 7468 2074 6865 2070 726f  ON, with the pro
-0000e050: 7065 7274 7920 7365 7420 6174 2074 6865  perty set at the
-0000e060: 2054 6173 6b20 6c65 7665 6c2c 2074 6865   Task level, the
-0000e070: 2073 616d 6520 7370 6563 6966 6963 6174   same specificat
-0000e080: 696f 6e20 776f 756c 6420 6265 3a0a 6060  ion would be:.``
-0000e090: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
-0000e0a0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
-0000e0b0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
-0000e0c0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-0000e0d0: 2020 2020 2022 7570 6c6f 6164 4669 6c65       "uploadFile
-0000e0e0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-0000e0f0: 2020 7b22 6c6f 6361 6c50 6174 6822 3a20    {"localPath": 
-0000e100: 2266 696c 655f 312e 7478 7422 2c20 2275  "file_1.txt", "u
-0000e110: 706c 6f61 6450 6174 6822 3a20 2266 696c  ploadPath": "fil
-0000e120: 655f 312e 7478 7422 7d2c 0a20 2020 2020  e_1.txt"},.     
-0000e130: 2020 2020 2020 207b 226c 6f63 616c 5061         {"localPa
-0000e140: 7468 223a 2022 6469 725f 322f 6669 6c65  th": "dir_2/file
-0000e150: 5f32 2e74 7874 222c 2022 7570 6c6f 6164  _2.txt", "upload
-0000e160: 5061 7468 223a 2022 3a3a 6669 6c65 5f32  Path": "::file_2
-0000e170: 2e74 7874 227d 2c0a 2020 2020 2020 2020  .txt"},.        
-0000e180: 2020 2020 7b22 6c6f 6361 6c50 6174 6822      {"localPath"
-0000e190: 3a20 2266 696c 655f 332e 7478 7422 2c20  : "file_3.txt", 
-0000e1a0: 2275 706c 6f61 6450 6174 6822 3a20 226f  "uploadPath": "o
-0000e1b0: 7468 6572 5f6e 616d 6573 7061 6365 3a3a  ther_namespace::
-0000e1c0: 6669 6c65 5f33 2e74 7874 227d 0a20 2020  file_3.txt"}.   
-0000e1d0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0000e1e0: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
-0000e1f0: 0a20 205d 0a7d 0a60 6060 0a0a 5768 656e  .  ].}.```..When
-0000e200: 2072 756e 6e69 6e67 2074 6865 2050 7974   running the Pyt
-0000e210: 686f 6e20 4578 616d 706c 6573 2063 6f6d  hon Examples com
-0000e220: 6d61 6e64 7320 6f6e 202a 2a57 696e 646f  mands on **Windo
-0000e230: 7773 2a2a 2068 6f73 7473 2c20 6e6f 7465  ws** hosts, note
-0000e240: 2074 6861 7420 6569 7468 6572 2057 696e   that either Win
-0000e250: 646f 7773 206f 7220 556e 6978 2064 6972  dows or Unix dir
-0000e260: 6563 746f 7279 2073 6570 6172 6174 6f72  ectory separator
-0000e270: 7320 6361 6e20 6265 2075 7365 6420 666f  s can be used fo
-0000e280: 7220 7468 6520 606c 6f63 616c 5061 7468  r the `localPath
-0000e290: 6020 7061 7468 6e61 6d65 7320 286f 7220  ` pathnames (or 
-0000e2a0: 7468 6520 7061 7468 6e61 6d65 7320 696e  the pathnames in
-0000e2b0: 2060 696e 7075 7473 6029 2c20 6275 7420   `inputs`), but 
-0000e2c0: 7468 6520 556e 6978 2063 6f6e 7665 6e74  the Unix convent
-0000e2d0: 696f 6e20 6d75 7374 2062 6520 7573 6564  ion must be used
-0000e2e0: 2066 6f72 2074 6865 2060 7570 6c6f 6164   for the `upload
-0000e2f0: 5061 7468 6020 6e61 6d65 732c 2065 2e67  Path` names, e.g
-0000e300: 2e3a 0a0a 6060 6074 6f6d 6c0a 7570 6c6f  .:..```toml.uplo
-0000e310: 6164 4669 6c65 7320 3d20 5b0a 2020 2020  adFiles = [.    
-0000e320: 7b6c 6f63 616c 5061 7468 203d 2022 6469  {localPath = "di
-0000e330: 725f 325c 5c66 696c 655f 322e 7478 7422  r_2\\file_2.txt"
-0000e340: 2c20 7570 6c6f 6164 5061 7468 203d 2022  , uploadPath = "
-0000e350: 3a3a 6d79 5f64 6972 6563 746f 7279 2f66  ::my_directory/f
-0000e360: 696c 655f 322e 7478 7422 7d2c 0a5d 0a60  ile_2.txt"},.].`
-0000e370: 6060 0a0a 5468 6520 6075 706c 6f61 6446  ``..The `uploadF
-0000e380: 696c 6573 6020 7072 6f70 6572 7479 2063  iles` property c
-0000e390: 616e 2061 6c73 6f20 6265 2073 6574 2061  an also be set a
-0000e3a0: 7420 7468 6520 576f 726b 2052 6571 7569  t the Work Requi
-0000e3b0: 7265 6d65 6e74 2061 6e64 2054 6173 6b20  rement and Task 
-0000e3c0: 4772 6f75 7020 6c65 7665 6c73 2c20 616e  Group levels, an
-0000e3d0: 6420 7072 6f70 6572 7479 2069 6e68 6572  d property inher
-0000e3e0: 6974 616e 6365 206f 7065 7261 7465 7320  itance operates 
-0000e3f0: 6173 206e 6f72 6d61 6c2e 0a0a 466f 7220  as normal...For 
-0000e400: 6075 706c 6f61 6450 6174 6860 2c20 7468  `uploadPath`, th
-0000e410: 6520 7361 6d65 2060 3a3a 6020 6e61 6d69  e same `::` nami
-0000e420: 6e67 2063 6f6e 7665 6e74 696f 6e20 6973  ng convention is
-0000e430: 2061 7661 696c 6162 6c65 2061 7320 6973   available as is
-0000e440: 2075 7365 6420 696e 2074 6865 2060 7665   used in the `ve
-0000e450: 7269 6679 4174 5374 6172 7460 2c20 6076  rifyAtStart`, `v
-0000e460: 6572 6966 7957 6169 7460 2061 6e64 2060  erifyWait` and `
-0000e470: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
-0000e480: 7072 6f70 6572 7469 6573 2064 6973 6375  properties discu
-0000e490: 7373 6564 2062 656c 6f77 3a0a 0a2d 2049  ssed below:..- I
-0000e4a0: 6620 603a 3a60 2069 7320 6e6f 7420 7573  f `::` is not us
-0000e4b0: 6564 2c20 7468 656e 2074 6865 2066 696c  ed, then the fil
-0000e4c0: 6520 6973 2075 706c 6f61 6465 6420 7265  e is uploaded re
-0000e4d0: 6c61 7469 7665 2074 6f20 7468 6520 6375  lative to the cu
-0000e4e0: 7272 656e 7420 6e61 6d65 7370 6163 6520  rrent namespace 
-0000e4f0: 696e 2061 2064 6972 6563 746f 7279 206e  in a directory n
-0000e500: 616d 6564 2061 6674 6572 2074 6865 206e  amed after the n
-0000e510: 616d 6520 6f66 2074 6865 2057 6f72 6b20  ame of the Work 
-0000e520: 5265 7175 6972 656d 656e 740a 2d20 4966  Requirement.- If
-0000e530: 2060 3a3a 6020 6973 2075 7365 6420 6174   `::` is used at
-0000e540: 2074 6865 2073 7461 7274 206f 6620 7468   the start of th
-0000e550: 6520 6075 706c 6f61 6450 6174 6860 2c20  e `uploadPath`, 
-0000e560: 7468 6520 6669 6c65 2069 7320 7570 6c6f  the file is uplo
-0000e570: 6164 6564 2072 656c 6174 6976 6520 746f  aded relative to
-0000e580: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
-0000e590: 2063 7572 7265 6e74 206e 616d 6573 7061   current namespa
-0000e5a0: 6365 0a2d 2049 6620 603c 6e61 6d65 7370  ce.- If `<namesp
-0000e5b0: 6163 653e 3a3a 6020 6973 2075 7365 6420  ace>::` is used 
-0000e5c0: 6174 2074 6865 2073 7461 7274 206f 6620  at the start of 
-0000e5d0: 6075 706c 6f61 6450 6174 6860 2c20 7468  `uploadPath`, th
-0000e5e0: 6520 6669 6c65 2069 7320 7570 6c6f 6164  e file is upload
-0000e5f0: 6564 2072 656c 6174 6976 6520 746f 2074  ed relative to t
-0000e600: 6865 2072 6f6f 7420 6f66 2060 3c6e 616d  he root of `<nam
-0000e610: 6573 7061 6365 3e60 0a0a 4561 6368 2066  espace>`..Each f
-0000e620: 696c 6520 7370 6563 6966 6965 6420 696e  ile specified in
-0000e630: 2074 6865 2060 7570 6c6f 6164 4669 6c65   the `uploadFile
-0000e640: 7360 206c 6973 7473 2077 696c 6c20 6f6e  s` lists will on
-0000e650: 6c79 2062 6520 7570 6c6f 6164 6564 206f  ly be uploaded o
-0000e660: 6e63 6520 746f 2065 6163 6820 756e 6971  nce to each uniq
-0000e670: 7565 2075 706c 6f61 6420 6c6f 6361 7469  ue upload locati
-0000e680: 6f6e 2066 6f72 2061 6e79 2067 6976 656e  on for any given
-0000e690: 2069 6e76 6f63 6174 696f 6e20 6f66 2060   invocation of `
-0000e6a0: 7964 2d73 7562 6d69 7460 2e0a 0a49 6620  yd-submit`...If 
-0000e6b0: 6120 6669 6c65 2069 6e20 7468 6520 6075  a file in the `u
-0000e6c0: 706c 6f61 6446 696c 6573 6020 6c69 7374  ploadFiles` list
-0000e6d0: 2069 7320 7265 7175 6972 6564 2062 7920   is required by 
-0000e6e0: 6120 5461 736b 2c20 6974 206d 7573 7420  a Task, it must 
-0000e6f0: 7365 7061 7261 7465 6c79 2062 6520 6164  separately be ad
-0000e700: 6465 6420 746f 2074 6865 2060 7665 7269  ded to the `veri
-0000e710: 6679 4174 5374 6172 7460 206f 7220 6076  fyAtStart` or `v
-0000e720: 6572 6966 7957 6169 7460 206c 6973 7473  erifyWait` lists
-0000e730: 2064 6973 6375 7373 6564 2062 656c 6f77   discussed below
-0000e740: 2e20 5468 6973 2069 7320 6e6f 7420 646f  . This is not do
-0000e750: 6e65 2061 7574 6f6d 6174 6963 616c 6c79  ne automatically
-0000e760: 2e20 4e6f 7465 2061 6c73 6f20 7468 6174  . Note also that
-0000e770: 2074 6865 2060 666c 6174 7465 6e55 706c   the `flattenUpl
-0000e780: 6f61 6450 6174 6873 6020 7072 6f70 6572  oadPaths` proper
-0000e790: 7479 2069 7320 6967 6e6f 7265 6420 666f  ty is ignored fo
-0000e7a0: 7220 6669 6c65 7320 696e 2074 6865 2060  r files in the `
-0000e7b0: 7570 6c6f 6164 4669 6c65 7360 206c 6973  uploadFiles` lis
-0000e7c0: 742e 0a0a 2323 2320 4669 6c65 2044 6570  t...### File Dep
-0000e7d0: 656e 6465 6e63 6965 7320 5573 696e 6720  endencies Using 
-0000e7e0: 6076 6572 6966 7941 7453 7461 7274 6020  `verifyAtStart` 
-0000e7f0: 616e 6420 6076 6572 6966 7957 6169 7460  and `verifyWait`
-0000e800: 0a0a 4974 2773 2070 6f73 7369 626c 6520  ..It's possible 
-0000e810: 746f 206d 616b 6520 5461 736b 7320 6465  to make Tasks de
-0000e820: 7065 6e64 656e 7420 6f6e 2074 6865 2070  pendent on the p
-0000e830: 7265 7365 6e63 6520 6f66 2066 696c 6573  resence of files
-0000e840: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
-0000e850: 746f 7265 2062 7920 7573 696e 6720 7468  tore by using th
-0000e860: 6520 6076 6572 6966 7941 7453 7461 7274  e `verifyAtStart
-0000e870: 6020 616e 6420 6076 6572 6966 7957 6169  ` and `verifyWai
-0000e880: 7460 206c 6973 7473 2e20 5468 6573 6520  t` lists. These 
-0000e890: 6669 6c65 7320 6172 6520 6e6f 7420 6175  files are not au
-0000e8a0: 746f 6d61 7469 6361 6c6c 7920 7570 6c6f  tomatically uplo
-0000e8b0: 6164 6564 2077 6865 6e20 7573 696e 6720  aded when using 
-0000e8c0: 6079 642d 7375 626d 6974 6020 736f 2061  `yd-submit` so a
-0000e8d0: 7265 2065 6974 6865 7220 7570 6c6f 6164  re either upload
-0000e8e0: 6564 206d 616e 7561 6c6c 7920 2865 2e67  ed manually (e.g
-0000e8f0: 2e2c 2062 7920 7573 696e 6720 6079 642d  ., by using `yd-
-0000e900: 7570 6c6f 6164 6029 2c20 6f72 2061 7265  upload`), or are
-0000e910: 2063 7265 6174 6564 2061 7320 6120 7265   created as a re
-0000e920: 7375 6c74 206f 6620 7468 6520 6578 6563  sult of the exec
-0000e930: 7574 696f 6e20 6f66 206f 7468 6572 2054  ution of other T
-0000e940: 6173 6b73 2e0a 0a4e 6f74 6520 7468 6174  asks...Note that
-0000e950: 2061 2067 6976 656e 2066 696c 6520 6361   a given file ca
-0000e960: 6e20 6f6e 6c79 2061 7070 6561 7220 696e  n only appear in
-0000e970: 202a 6f6e 652a 206f 6620 7468 6520 6069   *one* of the `i
-0000e980: 6e70 7574 7360 2c20 6076 6572 6966 7941  nputs`, `verifyA
-0000e990: 7453 7461 7274 6020 6f72 2060 7665 7269  tStart` or `veri
-0000e9a0: 6679 5761 6974 6020 6c69 7374 732e 0a0a  fyWait` lists...
-0000e9b0: 5461 736b 7320 7769 7468 2060 7665 7269  Tasks with `veri
-0000e9c0: 6679 4174 5374 6172 7460 2064 6570 656e  fyAtStart` depen
-0000e9d0: 6465 6e63 6965 7320 7769 6c6c 2066 6169  dencies will fai
-0000e9e0: 6c20 696d 6d65 6469 6174 656c 7920 6966  l immediately if
-0000e9f0: 2074 6865 2072 6571 7569 7265 6420 6669   the required fi
-0000ea00: 6c65 7320 6172 6520 6e6f 7420 7072 6573  les are not pres
-0000ea10: 656e 7420 7768 656e 2074 6865 2054 6173  ent when the Tas
-0000ea20: 6b20 6973 2073 7562 6d69 7474 6564 2e20  k is submitted. 
-0000ea30: 5461 736b 7320 7769 7468 2060 7665 7269  Tasks with `veri
-0000ea40: 6679 5761 6974 6020 6465 7065 6e64 656e  fyWait` dependen
-0000ea50: 6369 6573 2077 696c 6c20 6e6f 7420 6265  cies will not be
-0000ea60: 636f 6d65 2060 5245 4144 5960 2074 6f20  come `READY` to 
-0000ea70: 6265 2073 6368 6564 756c 6564 2074 6f20  be scheduled to 
-0000ea80: 576f 726b 6572 7320 756e 7469 6c20 7468  Workers until th
-0000ea90: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
-0000eaa0: 7265 2073 6174 6973 6669 6564 2e0a 0a57  re satisfied...W
-0000eab0: 6865 6e20 7370 6563 6966 7969 6e67 2066  hen specifying f
-0000eac0: 696c 6573 2069 6e20 7468 6520 6076 6572  iles in the `ver
-0000ead0: 6966 7941 7453 7461 7274 6020 616e 6420  ifyAtStart` and 
-0000eae0: 6076 6572 6966 7957 6169 7460 206c 6973  `verifyWait` lis
-0000eaf0: 7473 2c20 6173 2077 6974 6820 7468 6520  ts, as with the 
-0000eb00: 6075 706c 6f61 6450 6174 6860 2070 726f  `uploadPath` pro
-0000eb10: 7065 7274 7920 6469 7363 7573 7365 6420  perty discussed 
-0000eb20: 6162 6f76 652c 2074 6865 2066 696c 6520  above, the file 
-0000eb30: 6c6f 6361 7469 6f6e 7320 6361 6e20 6265  locations can be
-0000eb40: 2028 3129 2072 656c 6174 6976 6520 746f   (1) relative to
-0000eb50: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-0000eb60: 656d 656e 7420 6e61 6d65 2069 6e20 7468  ement name in th
-0000eb70: 6520 6375 7272 656e 7420 6e61 6d65 7370  e current namesp
-0000eb80: 6163 6520 2874 6865 2064 6566 6175 6c74  ace (the default
-0000eb90: 292c 2028 3229 2072 656c 6174 6976 6520  ), (2) relative 
-0000eba0: 746f 2074 6865 2072 6f6f 7420 6f66 2074  to the root of t
-0000ebb0: 6865 2063 7572 7265 6e74 206e 616d 6573  he current names
-0000ebc0: 7061 6365 2c20 6f72 2028 3329 2072 656c  pace, or (3) rel
-0000ebd0: 6174 6976 6520 746f 2074 6865 2072 6f6f  ative to the roo
-0000ebe0: 7420 6f66 2061 2064 6966 6665 7265 6e74  t of a different
-0000ebf0: 206e 616d 6573 7061 6365 2069 6e20 7468   namespace in th
-0000ec00: 6520 7573 6572 2773 2041 6363 6f75 6e74  e user's Account
-0000ec10: 2e0a 0a31 2e20 466f 7220 6669 6c65 7320  ...1. For files 
-0000ec20: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
-0000ec30: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000ec40: 206e 616d 6520 696e 2074 6865 2063 7572   name in the cur
-0000ec50: 7265 6e74 206e 616d 6573 7061 6365 2c20  rent namespace, 
-0000ec60: 6a75 7374 2075 7365 2074 6865 2066 696c  just use the fil
-0000ec70: 6520 7061 7468 2c20 652e 672e 0a60 6060  e path, e.g..```
-0000ec80: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
-0000ec90: 7422 3a20 5b22 6669 6c65 5f31 2e74 7874  t": ["file_1.txt
-0000eca0: 225d 202d 3e20 6465 7665 6c6f 706d 656e  "] -> developmen
-0000ecb0: 743a 7465 7374 7275 6e5f 3232 3131 3038  t:testrun_221108
-0000ecc0: 2d31 3230 3430 342d 3764 322f 6669 6c65  -120404-7d2/file
-0000ecd0: 5f31 2e74 7874 0a60 6060 0a0a 322e 2046  _1.txt.```..2. F
-0000ece0: 6f72 2066 696c 6573 2072 656c 6174 6976  or files relativ
-0000ecf0: 6520 746f 2074 6865 2072 6f6f 7420 6f66  e to the root of
-0000ed00: 2074 6865 2063 7572 7265 6e74 206e 616d   the current nam
-0000ed10: 6573 7061 6365 2c20 7072 6566 6978 2074  espace, prefix t
-0000ed20: 6865 2066 696c 6520 7061 7468 2077 6974  he file path wit
-0000ed30: 6820 603a 3a60 2c20 652e 672e 0a60 6060  h `::`, e.g..```
-0000ed40: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
-0000ed50: 7422 3a20 5b22 3a3a 6669 6c65 5f31 2e74  t": ["::file_1.t
-0000ed60: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
-0000ed70: 656e 743a 6669 6c65 5f31 2e74 7874 0a60  ent:file_1.txt.`
-0000ed80: 6060 0a0a 332e 2046 6f72 2066 696c 6573  ``..3. For files
-0000ed90: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-0000eda0: 2072 6f6f 7420 6f66 2061 2064 6966 6665   root of a diffe
-0000edb0: 7265 6e74 206e 616d 6573 7061 6365 2c20  rent namespace, 
-0000edc0: 7072 6566 6978 2074 6865 2066 696c 6520  prefix the file 
-0000edd0: 7061 7468 2077 6974 6820 7468 6520 6e61  path with the na
-0000ede0: 6d65 7370 6163 6520 6e61 6d65 2061 6e64  mespace name and
-0000edf0: 2060 3a3a 602c 2065 2e67 2e0a 6060 6073   `::`, e.g..```s
-0000ee00: 6865 6c6c 0a22 7665 7269 6679 5761 6974  hell."verifyWait
-0000ee10: 223a 205b 226f 7468 6572 5f6e 616d 6573  ": ["other_names
-0000ee20: 7061 6365 3a3a 6669 6c65 5f31 2e74 7874  pace::file_1.txt
-0000ee30: 225d 202d 3e20 6f74 6865 725f 6e61 6d65  "] -> other_name
-0000ee40: 7370 6163 653a 6669 6c65 5f31 2e74 7874  space:file_1.txt
-0000ee50: 0a60 6060 0a0a 5468 6520 7573 6520 6f66  .```..The use of
-0000ee60: 2074 6865 2074 6872 6565 2064 6966 6665   the three diffe
-0000ee70: 7265 6e74 2066 6f72 6d73 2063 616e 2062  rent forms can b
-0000ee80: 6520 6d69 7865 6420 7769 7468 696e 2061  e mixed within a
-0000ee90: 2073 696e 676c 6520 6c69 7374 2c20 652e   single list, e.
-0000eea0: 672e 3a0a 6060 6073 6865 6c6c 0a22 7665  g.:.```shell."ve
-0000eeb0: 7269 6679 4174 5374 6172 7422 3a20 5b22  rifyAtStart": ["
-0000eec0: 6669 6c65 5f31 2e74 7874 222c 2022 3a3a  file_1.txt", "::
-0000eed0: 6469 725f 322f 6669 6c65 5f32 2e74 7874  dir_2/file_2.txt
-0000eee0: 222c 2022 6f74 6865 725f 6e61 6d65 7370  ", "other_namesp
-0000eef0: 6163 653a 3a64 6972 5f33 2f66 696c 655f  ace::dir_3/file_
-0000ef00: 332e 7478 7422 5d0a 6060 600a 0a23 2323  3.txt"].```..###
-0000ef10: 2046 696c 6573 2044 6f77 6e6c 6f61 6465   Files Downloade
-0000ef20: 6420 5573 696e 6720 6069 6e70 7574 734f  d Using `inputsO
-0000ef30: 7074 696f 6e61 6c60 0a0a 5468 6520 6069  ptional`..The `i
-0000ef40: 6e70 7574 734f 7074 696f 6e61 6c60 2070  nputsOptional` p
-0000ef50: 726f 7065 7274 7920 776f 726b 7320 696e  roperty works in
-0000ef60: 2061 2073 696d 696c 6172 2066 6173 6869   a similar fashi
-0000ef70: 6f6e 2074 6f20 7468 6520 6076 6572 6966  on to the `verif
-0000ef80: 792a 6020 7072 6f70 6572 7469 6573 2061  y*` properties a
-0000ef90: 626f 7665 2c20 6275 7420 7468 6520 6669  bove, but the fi
-0000efa0: 6c65 7320 7370 6563 6966 6965 6420 696e  les specified in
-0000efb0: 2074 6869 7320 6c69 7374 2061 7265 206f   this list are o
-0000efc0: 7074 696f 6e61 6c2e 2054 6869 7320 7072  ptional. This pr
-0000efd0: 6f70 6572 7479 2061 6c73 6f20 616c 6c6f  operty also allo
-0000efe0: 7773 2066 6f72 2074 6865 2075 7365 206f  ws for the use o
-0000eff0: 6620 7769 6c64 6361 7264 7320 602a 6020  f wildcards `*` 
-0000f000: 616e 6420 602a 2a60 2074 6f20 636f 6c6c  and `**` to coll
-0000f010: 6563 7420 6669 6c65 7320 7573 696e 6720  ect files using 
-0000f020: 7769 6c64 6361 7264 2070 6174 6873 2e20  wildcard paths. 
-0000f030: 5468 6520 2a2a 616e 742a 2a20 636f 6e76  The **ant** conv
-0000f040: 656e 7469 6f6e 7320 6172 6520 7573 6564  entions are used
-0000f050: 2066 6f72 2074 6865 7365 2077 696c 6463   for these wildc
-0000f060: 6172 6473 2e0a 0a23 2323 2046 696c 6573  ards...### Files
-0000f070: 2044 6f77 6e6c 6f61 6465 6420 746f 2061   Downloaded to a
-0000f080: 204e 6f64 6520 666f 7220 7573 6520 696e   Node for use in
-0000f090: 2054 6173 6b20 4578 6563 7574 696f 6e0a   Task Execution.
-0000f0a0: 0a57 6865 6e20 6120 5461 736b 2069 7320  .When a Task is 
-0000f0b0: 6578 6563 7574 6564 2062 7920 6120 576f  executed by a Wo
-0000f0c0: 726b 6572 206f 6e20 6120 4e6f 6465 2c20  rker on a Node, 
-0000f0d0: 6974 7320 7265 7175 6972 6564 2066 696c  its required fil
-0000f0e0: 6573 2061 7265 2064 6f77 6e6c 6f61 6465  es are downloade
-0000f0f0: 6420 6672 6f6d 2074 6865 204f 626a 6563  d from the Objec
-0000f100: 7420 5374 6f72 6520 7072 696f 7220 746f  t Store prior to
-0000f110: 2054 6173 6b20 6578 6563 7574 696f 6e2e   Task execution.
-0000f120: 2041 6e79 2066 696c 6520 6c69 7374 6564   Any file listed
-0000f130: 2069 6e20 7468 6520 6069 6e70 7574 7360   in the `inputs`
-0000f140: 2066 6f72 2061 2054 6173 6b20 6973 2061   for a Task is a
-0000f150: 7373 756d 6564 2074 6f20 6265 2072 6571  ssumed to be req
-0000f160: 7569 7265 642c 2061 6c6f 6e67 2077 6974  uired, along wit
-0000f170: 6820 616e 7920 6164 6469 7469 6f6e 616c  h any additional
-0000f180: 2066 696c 6573 2073 7065 6369 6669 6564   files specified
-0000f190: 2069 6e20 7468 6520 6076 6572 6966 7941   in the `verifyA
-0000f1a0: 7453 7461 7274 6020 616e 6420 6076 6572  tStart` and `ver
-0000f1b0: 6966 7957 6169 7460 206c 6973 7473 2e20  ifyWait` lists. 
-0000f1c0: 4669 6c65 7320 7370 6563 6966 6965 6420  Files specified 
-0000f1d0: 7573 696e 6720 7468 6520 6069 6e70 7574  using the `input
-0000f1e0: 734f 7074 696f 6e61 6c60 2070 726f 7065  sOptional` prope
-0000f1f0: 7274 7920 6172 6520 6f70 7469 6f6e 616c  rty are optional
-0000f200: 6c79 2064 6f77 6e6c 6f61 6465 6420 6672  ly downloaded fr
-0000f210: 6f6d 2074 6865 204f 626a 6563 7420 5374  om the Object St
-0000f220: 6f72 652e 2028 4e6f 7465 2074 6861 7420  ore. (Note that 
-0000f230: 6120 6669 6c65 2073 686f 756c 6420 6f6e  a file should on
-0000f240: 6c79 2061 7070 6561 7220 696e 206f 6e65  ly appear in one
-0000f250: 206f 6620 7468 6573 6520 666f 7572 206c   of these four l
-0000f260: 6973 7473 2c20 6f74 6865 7277 6973 6520  ists, otherwise 
-0000f270: 6079 642d 7375 626d 6974 6020 7769 6c6c  `yd-submit` will
-0000f280: 2072 6574 7572 6e20 616e 2065 7272 6f72   return an error
-0000f290: 2e29 0a0a 5768 656e 2061 2054 6173 6b20  .)..When a Task 
-0000f2a0: 6973 2073 7461 7274 6564 2062 7920 7468  is started by th
-0000f2b0: 6520 4167 656e 742c 2069 7473 2077 6f72  e Agent, its wor
-0000f2c0: 6b69 6e67 2064 6972 6563 746f 7279 2068  king directory h
-0000f2d0: 6173 2061 2070 6174 7465 726e 2073 6f6d  as a pattern som
-0000f2e0: 6574 6869 6e67 206c 696b 653a 0a0a 602f  ething like:..`/
-0000f2f0: 7661 722f 6f70 742f 7965 6c6c 6f77 646f  var/opt/yellowdo
-0000f300: 672f 7964 2d61 6765 6e74 2d34 2f64 6174  g/yd-agent-4/dat
-0000f310: 612f 776f 726b 6572 732f 312f 7964 6964  a/workers/1/ydid
-0000f320: 5f74 6173 6b5f 4430 4430 4430 5f36 3866  _task_D0D0D0_68f
-0000f330: 3565 3562 652d 6463 3933 2d34 3965 622d  5e5be-dc93-49eb-
-0000f340: 6138 3234 2d31 6663 6462 3532 6639 3139  a824-1fcdb52f919
-0000f350: 355f 315f 3160 0a0a 2860 7964 6964 5f74  5_1_1`..(`ydid_t
-0000f360: 6173 6b5f 4430 4430 4430 5f36 3866 3565  ask_D0D0D0_68f5e
-0000f370: 3562 652d 6463 3933 2d34 3965 622d 6138  5be-dc93-49eb-a8
-0000f380: 3234 2d31 6663 6462 3532 6639 3139 355f  24-1fcdb52f9195_
-0000f390: 315f 3160 2069 7320 616e 2065 7068 656d  1_1` is an ephem
-0000f3a0: 6572 616c 2064 6972 6563 746f 7279 2074  eral directory t
-0000f3b0: 6861 7420 6973 2072 656d 6f76 6564 2061  hat is removed a
-0000f3c0: 6674 6572 2074 6865 2054 6173 6b20 6669  fter the Task fi
-0000f3d0: 6e69 7368 6573 2061 6e64 2061 6e79 206f  nishes and any o
-0000f3e0: 7574 7075 7473 2068 6176 6520 6265 656e  utputs have been
-0000f3f0: 2075 706c 6f61 6465 642e 290a 0a46 696c   uploaded.)..Fil
-0000f400: 6573 2074 6861 7420 6172 6520 646f 776e  es that are down
-0000f410: 6c6f 6164 6564 2062 7920 7468 6520 4167  loaded by the Ag
-0000f420: 656e 7420 7072 696f 7220 746f 2054 6173  ent prior to Tas
-0000f430: 6b20 6578 6563 7574 696f 6e20 6172 6520  k execution are 
-0000f440: 6c6f 6361 7465 6420 6173 2066 6f6c 6c6f  located as follo
-0000f450: 7773 3a0a 0a31 2e20 4966 2074 6865 2060  ws:..1. If the `
-0000f460: 666c 6174 7465 6e49 6e70 7574 5061 7468  flattenInputPath
-0000f470: 7360 2070 726f 7065 7274 7920 6973 2073  s` property is s
-0000f480: 6574 2074 6f20 7468 6520 6465 6661 756c  et to the defaul
-0000f490: 7420 6f66 2060 6661 6c73 6560 2066 6f72  t of `false` for
-0000f4a0: 2074 6865 2054 6173 6b2c 2074 6865 2064   the Task, the d
-0000f4b0: 6f77 6e6c 6f61 6465 6420 6f62 6a65 6374  ownloaded object
-0000f4c0: 7320 6172 6520 706c 6163 6564 2069 6e20  s are placed in 
-0000f4d0: 7375 6264 6972 6563 746f 7269 6573 2074  subdirectories t
-0000f4e0: 6861 7420 6d69 7272 6f72 2074 686f 7365  hat mirror those
-0000f4f0: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
-0000f500: 746f 7265 2c20 696e 636c 7564 696e 6720  tore, including 
-0000f510: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000f520: 6d65 6e74 206e 616d 652c 2073 6974 7561  ment name, situa
-0000f530: 7465 6420 6265 6e65 6174 6820 7468 6520  ted beneath the 
-0000f540: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-0000f550: 792e 0a0a 0a32 2e20 4966 2074 6865 2060  y....2. If the `
-0000f560: 666c 6174 7465 6e49 6e70 7574 5061 7468  flattenInputPath
-0000f570: 7360 2070 726f 7065 7274 7920 6973 2073  s` property is s
-0000f580: 6574 2074 6f20 6074 7275 6560 2066 6f72  et to `true` for
-0000f590: 2074 6865 2054 6173 6b2c 2074 6865 2064   the Task, the d
-0000f5a0: 6f77 6e6c 6f61 6465 6420 6f62 6a65 6374  ownloaded object
-0000f5b0: 7320 6172 6520 616c 6c20 706c 6163 6564  s are all placed
-0000f5c0: 2064 6972 6563 746c 7920 696e 2072 6f6f   directly in roo
-0000f5d0: 7420 6f66 2074 6865 2054 6173 6b27 7320  t of the Task's 
-0000f5e0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-0000f5f0: 792e 0a0a 466f 7220 6578 616d 706c 653a  y...For example:
-0000f600: 0a0a 6060 6073 6865 6c6c 0a49 6620 7468  ..```shell.If th
-0000f610: 6520 7265 7175 6972 6564 206f 626a 6563  e required objec
-0000f620: 7420 6973 3a20 6465 7665 6c6f 706d 656e  t is: developmen
-0000f630: 743a 3a74 6573 7472 756e 5f32 3231 3130  t::testrun_22110
-0000f640: 382d 3132 3034 3034 2d37 6432 2f64 6576  8-120404-7d2/dev
-0000f650: 2f66 696c 655f 312e 7478 740a 0a74 6865  /file_1.txt..the
-0000f660: 6e2c 2069 6620 666c 6174 7465 6e49 6e70  n, if flattenInp
-0000f670: 7574 5061 7468 7320 6973 2066 616c 7365  utPaths is false
-0000f680: 2c20 7468 6520 6669 6c65 2077 696c 6c20  , the file will 
-0000f690: 6265 2066 6f75 6e64 2061 743a 0a20 2d3e  be found at:. ->
-0000f6a0: 203c 776f 726b 696e 675f 6469 7265 6374   <working_direct
-0000f6b0: 6f72 793e 2f74 6573 7472 756e 5f32 3231  ory>/testrun_221
-0000f6c0: 3130 382d 3132 3034 3034 2d37 6432 2f64  108-120404-7d2/d
-0000f6d0: 6576 2f66 696c 655f 312e 7478 740a 200a  ev/file_1.txt. .
-0000f6e0: 656c 7365 2c20 6966 2066 6c61 7474 656e  else, if flatten
-0000f6f0: 496e 7075 7450 6174 6873 2069 7320 7472  InputPaths is tr
-0000f700: 7565 2c20 7468 6520 6669 6c65 2077 696c  ue, the file wil
-0000f710: 6c20 6265 2066 6f75 6e64 2061 743a 0a20  l be found at:. 
-0000f720: 2d3e 203c 776f 726b 696e 675f 6469 7265  -> <working_dire
-0000f730: 6374 6f72 793e 2f66 696c 655f 312e 7478  ctory>/file_1.tx
-0000f740: 7420 0a20 0a77 6865 7265 203c 776f 726b  t . .where <work
-0000f750: 696e 675f 6469 7265 6374 6f72 793e 2069  ing_directory> i
-0000f760: 733a 0a20 202f 7661 722f 6f70 742f 7965  s:.  /var/opt/ye
-0000f770: 6c6c 6f77 646f 672f 7964 2d61 6765 6e74  llowdog/yd-agent
-0000f780: 2d34 2f64 6174 612f 776f 726b 6572 732f  -4/data/workers/
-0000f790: 312f 7964 6964 5f74 6173 6b5f 4430 4430  1/ydid_task_D0D0
-0000f7a0: 4430 5f36 3866 3565 3562 652d 6463 3933  D0_68f5e5be-dc93
-0000f7b0: 2d34 3965 622d 6138 3234 2d31 6663 6462  -49eb-a824-1fcdb
-0000f7c0: 3532 6639 3139 355f 315f 312f 0a60 6060  52f9195_1_1/.```
-0000f7d0: 0a0a 4e6f 7465 2074 6861 7420 576f 726b  ..Note that Work
-0000f7e0: 2052 6571 7569 7265 6d65 6e74 206e 616d   Requirement nam
-0000f7f0: 6520 2865 2e67 2e2c 2060 7465 7374 7275  e (e.g., `testru
-0000f800: 6e5f 3232 3131 3038 2d31 3230 3430 342d  n_221108-120404-
-0000f810: 3764 3260 2920 6973 2061 7661 696c 6162  7d2`) is availab
-0000f820: 6c65 2076 6961 2074 6865 2076 6172 6961  le via the varia
-0000f830: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
-0000f840: 2060 7772 5f6e 616d 6560 2c20 736f 2074   `wr_name`, so t
-0000f850: 6869 7320 636f 756c 6420 6265 2073 7570  his could be sup
-0000f860: 706c 6965 6420 746f 2074 6865 2054 6173  plied to the Tas
-0000f870: 6b20 746f 2068 656c 7020 6974 206c 6f63  k to help it loc
-0000f880: 6174 6520 6974 7320 646f 776e 6c6f 6164  ate its download
-0000f890: 6564 2066 696c 6573 2e20 466f 7220 6578  ed files. For ex
-0000f8a0: 616d 706c 652c 2069 6e20 7468 6520 6077  ample, in the `w
-0000f8b0: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
-0000f8c0: 7365 6374 696f 6e20 6f66 2074 6865 2060  section of the `
-0000f8d0: 636f 6e66 6967 2e74 6f6d 6c60 2066 696c  config.toml` fil
-0000f8e0: 652c 2049 2063 6f75 6c64 2073 7065 6369  e, I could speci
-0000f8f0: 6679 3a0a 0a60 6060 746f 6d6c 0a65 6e76  fy:..```toml.env
-0000f900: 6972 6f6e 6d65 6e74 203d 207b 5752 5f44  ironment = {WR_D
-0000f910: 4952 4543 544f 5259 203d 2022 7b7b 7772  IRECTORY = "{{wr
-0000f920: 5f6e 616d 657d 7d22 7d0a 6060 600a 0a54  _name}}"}.```..T
-0000f930: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-0000f940: 656e 7420 6e61 6d65 2077 6f75 6c64 2074  ent name would t
-0000f950: 6865 6e20 6265 2061 7661 696c 6162 6c65  hen be available
-0000f960: 2074 6f20 7468 6520 5461 736b 2069 6e20   to the Task in 
-0000f970: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-0000f980: 7661 7269 6162 6c65 2060 2457 525f 4449  variable `$WR_DI
-0000f990: 5245 4354 4f52 5960 2e0a 0a23 2323 2046  RECTORY`...### F
-0000f9a0: 696c 6573 2055 706c 6f61 6465 6420 6672  iles Uploaded fr
-0000f9b0: 6f6d 2061 204e 6f64 6520 746f 2074 6865  om a Node to the
-0000f9c0: 204f 626a 6563 7420 5374 6f72 6520 6166   Object Store af
-0000f9d0: 7465 7220 5461 736b 2045 7865 6375 7469  ter Task Executi
-0000f9e0: 6f6e 0a0a 4166 7465 7220 5461 736b 2063  on..After Task c
-0000f9f0: 6f6d 706c 6574 696f 6e2c 2074 6865 2041  ompletion, the A
-0000fa00: 6765 6e74 2077 696c 6c20 7570 6c6f 6164  gent will upload
-0000fa10: 2073 7065 6369 6669 6564 206f 7574 7075   specified outpu
-0000fa20: 7420 6669 6c65 7320 746f 2074 6865 204f  t files to the O
-0000fa30: 626a 6563 7420 5374 6f72 652e 2054 6865  bject Store. The
-0000fa40: 2066 696c 6573 2074 6f20 6265 2075 706c   files to be upl
-0000fa50: 6f61 6465 6420 6172 6520 7468 6f73 6520  oaded are those 
-0000fa60: 6c69 7374 6564 2069 6e20 7468 6520 606f  listed in the `o
-0000fa70: 7574 7075 7473 6020 616e 6420 606f 7574  utputs` and `out
-0000fa80: 7075 7473 5265 7175 6972 6564 6020 7072  putsRequired` pr
-0000fa90: 6f70 6572 7469 6573 2066 6f72 2074 6865  operties for the
-0000faa0: 2054 6173 6b2e 0a0a 496e 2061 6464 6974   Task...In addit
-0000fab0: 696f 6e2c 2074 6865 2063 6f6e 736f 6c65  ion, the console
-0000fac0: 206f 7574 7075 7420 6f66 2074 6865 2054   output of the T
-0000fad0: 6173 6b20 6973 2063 6170 7475 7265 6420  ask is captured 
-0000fae0: 696e 2061 2066 696c 6520 6361 6c6c 6564  in a file called
-0000faf0: 2060 7461 736b 6f75 7470 7574 2e74 7874   `taskoutput.txt
-0000fb00: 6020 696e 2074 6865 2072 6f6f 7420 6f66  ` in the root of
-0000fb10: 2074 6865 2054 6173 6b27 7320 776f 726b   the Task's work
-0000fb20: 696e 6720 6469 7265 6374 6f72 792e 2057  ing directory. W
-0000fb30: 6865 7468 6572 2074 6865 2060 7461 736b  hether the `task
-0000fb40: 6f75 7470 7574 2e74 7874 6020 6669 6c65  output.txt` file
-0000fb50: 2069 7320 7570 6c6f 6164 6564 2074 6f20   is uploaded to 
-0000fb60: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
-0000fb70: 2069 7320 6465 7465 726d 696e 6564 2062   is determined b
-0000fb80: 7920 7468 6520 6063 6170 7475 7265 5461  y the `captureTa
-0000fb90: 736b 4f75 7470 7574 6020 7072 6f70 6572  skOutput` proper
-0000fba0: 7479 2066 6f72 2074 6865 2054 6173 6b2c  ty for the Task,
-0000fbb0: 2061 6e64 2074 6869 7320 6973 2073 6574   and this is set
-0000fbc0: 2074 6f20 2774 7275 6527 2062 7920 6465   to 'true' by de
-0000fbd0: 6661 756c 742e 0a0a 4966 2054 6173 6b20  fault...If Task 
-0000fbe0: 6f75 7470 7574 7320 6172 6520 6372 6561  outputs are crea
-0000fbf0: 7465 6420 696e 2073 7562 6469 7265 6374  ted in subdirect
-0000fc00: 6f72 6965 7320 6265 6c6f 7720 7468 6520  ories below the 
-0000fc10: 5461 736b 2773 2077 6f72 6b69 6e67 2064  Task's working d
-0000fc20: 6972 6563 746f 7279 2c20 696e 636c 7564  irectory, includ
-0000fc30: 6520 7468 6520 6469 7265 6374 6f72 6965  e the directorie
-0000fc40: 7320 666f 7220 6669 6c65 7320 696e 2074  s for files in t
-0000fc50: 6865 2060 6f75 7470 7574 7360 2070 726f  he `outputs` pro
-0000fc60: 7065 7274 792e 2045 2e67 2e2c 2069 6620  perty. E.g., if 
-0000fc70: 6120 5461 736b 2063 7265 6174 6573 2066  a Task creates f
-0000fc80: 696c 6573 2060 7265 7375 6c74 732f 6f70  iles `results/op
-0000fc90: 656e 666f 616d 2e74 6172 2e67 7a60 2061  enfoam.tar.gz` a
-0000fca0: 6e64 2060 7265 7375 6c74 732f 6f70 656e  nd `results/open
-0000fcb0: 666f 616d 2e6c 6f67 602c 2074 6865 6e20  foam.log`, then 
-0000fcc0: 7370 6563 6966 7920 7468 6573 6520 666f  specify these fo
-0000fcd0: 7220 7570 6c6f 6164 2069 6e20 7468 6520  r upload in the 
-0000fce0: 606f 7574 7075 7473 6020 7072 6f70 6572  `outputs` proper
-0000fcf0: 7479 2061 7320 666f 6c6c 6f77 733a 0a0a  ty as follows:..
-0000fd00: 6022 6f75 7470 7574 7322 3a20 5b22 7265  `"outputs": ["re
-0000fd10: 7375 6c74 732f 6f70 656e 666f 616d 2e74  sults/openfoam.t
-0000fd20: 6172 2e67 7a22 2c20 2272 6573 756c 7473  ar.gz", "results
-0000fd30: 2f6f 7065 6e66 6f61 6d2e 6c6f 6722 5d60  /openfoam.log"]`
-0000fd40: 0a0a 5768 656e 206f 7574 7075 7420 6669  ..When output fi
-0000fd50: 6c65 7320 6172 6520 7570 6c6f 6164 6564  les are uploaded
-0000fd60: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
-0000fd70: 746f 7265 2c20 7468 6579 2061 7265 2070  tore, they are p
-0000fd80: 6c61 6365 6420 696e 2061 2054 6173 6b20  laced in a Task 
-0000fd90: 4772 6f75 7020 616e 6420 5461 736b 2073  Group and Task s
-0000fda0: 7065 6369 6669 6320 6469 7265 6374 6f72  pecific director
-0000fdb0: 792e 2053 6f2c 2069 6620 7468 6520 4e61  y. So, if the Na
-0000fdc0: 6d65 7370 6163 6520 6973 2060 6465 7665  mespace is `deve
-0000fdd0: 6c6f 706d 656e 7460 2c20 7468 6520 576f  lopment`, the Wo
-0000fde0: 726b 2052 6571 7569 7265 6d65 6e74 2069  rk Requirement i
-0000fdf0: 7320 6074 6573 7472 756e 5f32 3231 3130  s `testrun_22110
-0000fe00: 382d 3132 3034 3034 2d37 6432 602c 2074  8-120404-7d2`, t
-0000fe10: 6865 2054 6173 6b20 4772 6f75 7020 6973  he Task Group is
-0000fe20: 2060 7461 736b 5f67 726f 7570 5f31 6020   `task_group_1` 
-0000fe30: 616e 6420 7468 6520 5461 736b 2069 7320  and the Task is 
-0000fe40: 6074 6173 6b5f 3160 2c20 7468 656e 2074  `task_1`, then t
-0000fe50: 6865 2066 696c 6573 2061 626f 7665 2077  he files above w
-0000fe60: 6f75 6c64 2062 6520 7570 6c6f 6164 6564  ould be uploaded
-0000fe70: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
-0000fe80: 746f 7265 2061 7320 666f 6c6c 6f77 733a  tore as follows:
-0000fe90: 0a0a 6060 6073 6865 6c6c 0a64 6576 656c  ..```shell.devel
-0000fea0: 6f70 6d65 6e74 3a3a 7465 7374 7275 6e5f  opment::testrun_
-0000feb0: 3232 3131 3038 2d31 3230 3430 342d 3764  221108-120404-7d
-0000fec0: 322f 7461 736b 5f67 726f 7570 5f31 2f74  2/task_group_1/t
-0000fed0: 6173 6b5f 312f 7265 7375 6c74 732f 6f70  ask_1/results/op
-0000fee0: 656e 666f 616d 2e74 6172 2e67 7a0a 6465  enfoam.tar.gz.de
-0000fef0: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
-0000ff00: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
-0000ff10: 2d37 6432 2f74 6173 6b5f 6772 6f75 705f  -7d2/task_group_
-0000ff20: 312f 7461 736b 5f31 2f72 6573 756c 7473  1/task_1/results
-0000ff30: 2f6f 7065 6e66 6f61 6d2e 6c6f 670a 6465  /openfoam.log.de
-0000ff40: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
-0000ff50: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
-0000ff60: 2d37 6432 2f74 6173 6b5f 6772 6f75 705f  -7d2/task_group_
-0000ff70: 312f 7461 736b 5f31 2f74 6173 6b6f 7574  1/task_1/taskout
-0000ff80: 7075 742e 7478 740a 6060 600a 0a54 6865  put.txt.```..The
-0000ff90: 202a 2a60 6f75 7470 7574 7352 6571 7569   **`outputsRequi
-0000ffa0: 7265 6460 2a2a 2070 726f 7065 7274 7920  red`** property 
-0000ffb0: 6361 6e20 6265 2075 7365 6420 696e 7374  can be used inst
-0000ffc0: 6561 6420 6f66 2028 6f72 2069 6e20 6164  ead of (or in ad
-0000ffd0: 6469 7469 6f6e 2074 6f29 2074 6865 2060  dition to) the `
-0000ffe0: 6f75 7470 7574 7360 2070 726f 7065 7274  outputs` propert
-0000fff0: 792c 2069 6620 7468 6520 6f75 7470 7574  y, if the output
-00010000: 2066 696c 6528 7329 202a 2a6d 7573 742a   file(s) **must*
-00010010: 2a20 6265 2061 7661 696c 6162 6c65 2066  * be available f
-00010020: 6f72 2075 706c 6f61 6420 746f 2074 6865  or upload to the
-00010030: 204f 626a 6563 7420 5374 6f72 6520 6174   Object Store at
-00010040: 2074 6865 2063 6f6e 636c 7573 696f 6e20   the conclusion 
-00010050: 6f66 2074 6865 2054 6173 6b20 6f72 2074  of the Task or t
-00010060: 6865 2054 6173 6b20 7769 6c6c 2062 6520  he Task will be 
-00010070: 6d61 726b 6564 2061 7320 6046 6169 6c65  marked as `Faile
-00010080: 6460 2c20 652e 672e 3a0a 0a60 226f 7574  d`, e.g.:..`"out
-00010090: 7075 7473 5265 7175 6972 6564 223a 205b  putsRequired": [
-000100a0: 2272 6573 756c 7473 2f70 726f 6365 7373  "results/process
-000100b0: 5f6f 7574 7075 742e 7478 7422 5d60 0a0a  _output.txt"]`..
-000100c0: 2323 2320 4669 6c65 7320 446f 776e 6c6f  ### Files Downlo
-000100d0: 6164 6564 2066 726f 6d20 7468 6520 4f62  aded from the Ob
-000100e0: 6a65 6374 2053 746f 7265 2074 6f20 4c6f  ject Store to Lo
-000100f0: 6361 6c20 5374 6f72 6167 650a 0a54 6865  cal Storage..The
-00010100: 2060 7964 2d64 6f77 6e6c 6f61 6460 2063   `yd-download` c
-00010110: 6f6d 6d61 6e64 2077 696c 6c20 646f 776e  ommand will down
-00010120: 6c6f 6164 2061 6c6c 206f 626a 6563 7473  load all objects
-00010130: 2066 726f 6d20 7468 6520 4f62 6a65 6374   from the Object
-00010140: 2053 746f 7265 2074 6f20 6120 6c6f 6361   Store to a loca
-00010150: 6c20 6469 7265 6374 6f72 792c 206f 6e20  l directory, on 
-00010160: 6120 7065 7220 576f 726b 2052 6571 7569  a per Work Requi
-00010170: 7265 6d65 6e74 2062 6173 6973 2028 696e  rement basis (in
-00010180: 636c 7564 696e 6720 616e 7920 6669 6c65  cluding any file
-00010190: 7320 7468 6174 2068 6176 6520 6265 656e  s that have been
-000101a0: 2075 706c 6f61 6465 6429 2e20 4120 6c6f   uploaded). A lo
-000101b0: 6361 6c20 6469 7265 6374 6f72 7920 6973  cal directory is
-000101c0: 2063 7265 6174 6564 2077 6974 6820 7468   created with th
-000101d0: 6520 7361 6d65 206e 616d 6520 6173 2074  e same name as t
-000101e0: 6865 204e 616d 6573 7061 6365 2061 6e64  he Namespace and
-000101f0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00010200: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00010210: 2064 6972 6563 746f 7269 6573 2e0a 0a55   directories...U
-00010220: 7365 2074 6865 2060 2d2d 696e 7465 7261  se the `--intera
-00010230: 6374 6976 6560 206f 7074 696f 6e20 7769  ctive` option wi
-00010240: 7468 2060 7964 2d64 6f77 6e6c 6f61 6460  th `yd-download`
-00010250: 2074 6f20 7365 6c65 6374 2077 6869 6368   to select which
-00010260: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00010270: 7428 7329 2074 6f20 646f 776e 6c6f 6164  t(s) to download
-00010280: 2e0a 0a46 6f72 2074 6865 2065 7861 6d70  ...For the examp
-00010290: 6c65 2061 626f 7665 2c20 6079 642d 646f  le above, `yd-do
-000102a0: 776e 6c6f 6164 6020 776f 756c 6420 6372  wnload` would cr
-000102b0: 6561 7465 2061 2064 6972 6563 746f 7279  eate a directory
-000102c0: 2063 616c 6c65 6420 6064 6576 656c 6f70   called `develop
-000102d0: 6d65 6e74 6020 696e 2074 6865 2063 7572  ment` in the cur
-000102e0: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
-000102f0: 6563 746f 7279 2c20 636f 6e74 6169 6e69  ectory, containi
-00010300: 6e67 2073 6f6d 6574 6869 6e67 206c 696b  ng something lik
-00010310: 653a 0a0a 6060 6073 6865 6c6c 0a64 6576  e:..```shell.dev
-00010320: 656c 6f70 6d65 6e74 0ae2 9494 e294 80e2  elopment........
-00010330: 9480 2074 6573 7472 756e 5f32 3231 3130  .. testrun_22110
-00010340: 382d 3132 3034 3034 2d37 6432 0a20 2020  8-120404-7d2.   
-00010350: 20e2 949c e294 80e2 9480 2062 6173 685f   ......... bash_
-00010360: 7363 7269 7074 2e73 680a 2020 2020 e294  script.sh.    ..
-00010370: 9ce2 9480 e294 8020 6669 6c65 5f31 2e74  ....... file_1.t
-00010380: 7874 0a20 2020 20e2 9494 e294 80e2 9480  xt.    .........
-00010390: 2074 6173 6b5f 6772 6f75 705f 310a 2020   task_group_1.  
-000103a0: 2020 2020 2020 e294 94e2 9480 e294 8020        ......... 
-000103b0: 7461 736b 5f31 0a20 2020 2020 2020 2020  task_1.         
-000103c0: 2020 20e2 949c e294 80e2 9480 2072 6573     ......... res
-000103d0: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
-000103e0: 20e2 9482 c2a0 c2a0 20e2 949c e294 80e2   ....... .......
-000103f0: 9480 206f 7065 6e66 6f61 6d2e 6c6f 670a  .. openfoam.log.
-00010400: 2020 2020 2020 2020 2020 2020 e294 82c2              ....
-00010410: a0c2 a020 e294 94e2 9480 e294 8020 6f70  ... ......... op
-00010420: 656e 666f 616d 2e74 6172 2e67 7a0a 2020  enfoam.tar.gz.  
-00010430: 2020 2020 2020 2020 2020 e294 94e2 9480            ......
-00010440: e294 8020 7461 736b 6f75 7470 7574 2e74  ... taskoutput.t
-00010450: 7874 0a60 6060 0a0a 4e6f 7465 2074 6861  xt.```..Note tha
-00010460: 7420 6576 6572 7974 6869 6e67 2077 6974  t everything wit
-00010470: 6869 6e20 7468 6520 606e 616d 6573 7061  hin the `namespa
-00010480: 6365 3a3a 776f 726b 2d72 6571 7569 7265  ce::work-require
-00010490: 6d65 6e74 6020 6469 7265 6374 6f72 7920  ment` directory 
-000104a0: 696e 2074 6865 204f 626a 6563 7420 5374  in the Object St
-000104b0: 6f72 6520 6973 2064 6f77 6e6c 6f61 6465  ore is downloade
-000104c0: 642c 2069 6e63 6c75 6469 6e67 2061 6e79  d, including any
-000104d0: 2066 696c 6573 2074 6861 7420 7765 7265   files that were
-000104e0: 2073 7065 6369 6669 6564 2069 6e20 6069   specified in `i
-000104f0: 6e70 7574 7360 2061 6e64 2075 706c 6f61  nputs` and uploa
-00010500: 6465 6420 6173 2070 6172 7420 6f66 2074  ded as part of t
-00010510: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-00010520: 656e 7420 7375 626d 6973 7369 6f6e 2e20  ent submission. 
-00010530: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
-00010540: 6f75 7073 2c20 616e 6420 6d75 6c74 6970  oups, and multip
-00010550: 6c65 2054 6173 6b73 2077 696c 6c20 616c  le Tasks will al
-00010560: 6c20 6170 7065 6172 2069 6e20 7468 6520  l appear in the 
-00010570: 6469 7265 6374 6f72 7920 7374 7275 6374  directory struct
-00010580: 7572 652e 0a0a 4966 2074 6865 2060 6465  ure...If the `de
-00010590: 7665 6c6f 706d 656e 7460 2064 6972 6563  velopment` direc
-000105a0: 746f 7279 2061 6c72 6561 6479 2065 7869  tory already exi
-000105b0: 7374 732c 2060 7964 2d64 6f77 6e6c 6f61  sts, `yd-downloa
-000105c0: 6460 2077 696c 6c20 7472 7920 6064 6576  d` will try `dev
-000105d0: 656c 6f70 6d65 6e74 2e30 3160 2c20 6574  elopment.01`, et
-000105e0: 632e 2c20 746f 2061 766f 6964 206f 7665  c., to avoid ove
-000105f0: 7277 7269 7469 6e67 2070 7265 7669 6f75  rwriting previou
-00010600: 7320 646f 776e 6c6f 6164 732e 0a0a 2323  s downloads...##
-00010610: 2054 6173 6b20 4578 6563 7574 696f 6e20   Task Execution 
-00010620: 436f 6e74 6578 740a 0a54 6869 7320 7365  Context..This se
-00010630: 6374 696f 6e20 6469 7363 7573 7365 7320  ction discusses 
-00010640: 7468 6520 636f 6e74 6578 7420 7769 7468  the context with
-00010650: 696e 2077 6869 6368 2061 2054 6173 6b20  in which a Task 
-00010660: 6f70 6572 6174 6573 2077 6865 6e20 6974  operates when it
-00010670: 2773 2065 7865 6375 7465 6420 6279 2061  's executed by a
-00010680: 2057 6f72 6b65 7220 6f6e 2061 206e 6f64   Worker on a nod
-00010690: 652e 2049 7420 6170 706c 6965 7320 7370  e. It applies sp
-000106a0: 6563 6966 6963 616c 6c79 2074 6f20 7468  ecifically to th
-000106b0: 6520 5965 6c6c 6f77 446f 6720 4167 656e  e YellowDog Agen
-000106c0: 7420 7275 6e6e 696e 6720 6f6e 2061 204c  t running on a L
-000106d0: 696e 7578 206e 6f64 652c 2061 6e64 2063  inux node, and c
-000106e0: 6f6e 6669 6775 7265 6420 7573 696e 6720  onfigured using 
-000106f0: 7468 6520 6465 6661 756c 7420 7573 6572  the default user
-00010700: 6e61 6d65 2c20 6469 7265 6374 6f72 6965  name, directorie
-00010710: 732c 2065 7463 2e20 436f 6e66 6967 7572  s, etc. Configur
-00010720: 6174 696f 6e73 2063 616e 2076 6172 792e  ations can vary.
-00010730: 0a0a 2323 2320 5461 736b 2045 7865 6375  ..### Task Execu
-00010740: 7469 6f6e 2053 7465 7073 0a0a 5768 656e  tion Steps..When
-00010750: 2061 2054 6173 6b20 6973 2061 6c6c 6f63   a Task is alloc
-00010760: 6174 6564 2074 6f20 6120 576f 726b 6572  ated to a Worker
-00010770: 206f 6e20 6120 6e6f 6465 2062 7920 7468   on a node by th
-00010780: 6520 5965 6c6c 6f77 446f 6720 5363 6865  e YellowDog Sche
-00010790: 6475 6c65 722c 2074 6865 2066 6f6c 6c6f  duler, the follo
-000107a0: 7769 6e67 2073 7465 7073 2061 7265 2066  wing steps are f
-000107b0: 6f6c 6c6f 7765 643a 0a0a 312e 2054 6865  ollowed:..1. The
-000107c0: 2041 6765 6e74 2072 756e 6e69 6e67 206f   Agent running o
-000107d0: 6e20 7468 6520 6e6f 6465 2064 6f77 6e6c  n the node downl
-000107e0: 6f61 6473 2074 6865 2054 6173 6b27 7320  oads the Task's 
-000107f0: 7072 6f70 6572 7469 6573 3a20 6974 7320  properties: its 
-00010800: 6074 6173 6b54 7970 6560 2c20 2060 6172  `taskType`,  `ar
-00010810: 6775 6d65 6e74 7360 2c20 6065 6e76 6972  guments`, `envir
-00010820: 6f6e 6d65 6e74 602c 2060 7461 736b 6461  onment`, `taskda
-00010830: 7461 602c 2061 6e64 2028 6672 6f6d 2074  ta`, and (from t
-00010840: 6865 204f 626a 6563 7420 5374 6f72 6529  he Object Store)
-00010850: 2061 6e79 2066 696c 6573 2069 6e20 7468   any files in th
-00010860: 6520 6069 6e70 7574 7360 206c 6973 7420  e `inputs` list 
-00010870: 616e 6420 616e 7920 6176 6169 6c61 626c  and any availabl
-00010880: 6520 6669 6c65 7320 696e 2074 6865 2060  e files in the `
-00010890: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
-000108a0: 6c69 7374 2e0a 322e 2054 6865 7365 2066  list..2. These f
-000108b0: 696c 6573 2061 7265 2070 6c61 6365 6420  iles are placed 
-000108c0: 696e 2061 6e20 6570 6865 6d65 7261 6c20  in an ephemeral 
-000108d0: 6469 7265 6374 6f72 7920 6372 6561 7465  directory create
-000108e0: 6420 666f 7220 7468 6973 2054 6173 6b27  d for this Task'
-000108f0: 7320 6578 6563 7574 696f 6e2c 2061 6e64  s execution, and
-00010900: 2069 6e74 6f20 7768 6963 6820 616e 7920   into which any 
-00010910: 6f75 7470 7574 2066 696c 6573 2061 7265  output files are
-00010920: 2061 6c73 6f20 706c 6163 6564 2062 7920   also placed by 
-00010930: 6465 6661 756c 742e 0a32 2e20 5468 6520  default..2. The 
-00010940: 4167 656e 7420 7275 6e73 2074 6865 2063  Agent runs the c
-00010950: 6f6d 6d61 6e64 2073 7065 6369 6669 6564  ommand specified
-00010960: 2066 6f72 2074 6865 2060 7461 736b 5479   for the `taskTy
-00010970: 7065 6020 696e 2074 6865 2041 6765 6e74  pe` in the Agent
-00010980: 2773 2060 6170 706c 6963 6174 696f 6e2e  's `application.
-00010990: 7961 6d6c 6020 636f 6e66 6967 7572 6174  yaml` configurat
-000109a0: 696f 6e20 6669 6c65 2e20 5468 6973 2064  ion file. This d
-000109b0: 6f6e 6520 6173 2061 2073 696d 706c 6520  one as a simple 
-000109c0: 6065 7865 6360 206f 6620 6120 7375 6270  `exec` of a subp
-000109d0: 726f 6365 7373 2e0a 332e 2057 6865 6e20  rocess..3. When 
-000109e0: 7468 6520 5461 736b 2063 6f6e 636c 7564  the Task conclud
-000109f0: 6573 2c20 7468 6520 4167 656e 7420 7573  es, the Agent us
-00010a00: 6573 2074 6865 2065 7869 7420 636f 6465  es the exit code
-00010a10: 206f 6620 7468 6520 7375 6270 726f 6365   of the subproce
-00010a20: 7373 2074 6f20 7265 706f 7274 2073 7563  ss to report suc
-00010a30: 6365 7373 2028 7a65 726f 2920 6f72 2066  cess (zero) or f
-00010a40: 6169 6c75 7265 2028 6e6f 6e2d 7a65 726f  ailure (non-zero
-00010a50: 292e 0a34 2e20 5468 6520 4167 656e 7420  )..4. The Agent 
-00010a60: 7468 656e 2067 6174 6865 7273 2061 6e79  then gathers any
-00010a70: 2066 696c 6573 2069 6e20 7468 6520 606f   files in the `o
-00010a80: 7574 7075 7473 6020 616e 6420 606f 7574  utputs` and `out
-00010a90: 7075 7473 5265 7175 6972 6564 6020 6c69  putsRequired` li
-00010aa0: 7374 7320 616e 6420 7570 6c6f 6164 7320  sts and uploads 
-00010ab0: 7468 656d 2074 6f20 7468 6520 4f62 6a65  them to the Obje
-00010ac0: 6374 2053 746f 7265 2e20 4966 2061 2066  ct Store. If a f
-00010ad0: 696c 6520 696e 2074 6865 2060 6f75 7470  ile in the `outp
-00010ae0: 7574 7352 6571 7569 7265 6460 206c 6973  utsRequired` lis
-00010af0: 7420 6973 206e 6f74 2066 6f75 6e64 2c20  t is not found, 
-00010b00: 7468 6520 5461 736b 2077 696c 6c20 6265  the Task will be
-00010b10: 2072 6570 6f72 7465 6420 6173 2066 6169   reported as fai
-00010b20: 6c65 642e 2054 6865 2041 6765 6e74 2077  led. The Agent w
-00010b30: 696c 6c20 616c 736f 206f 7074 696f 6e61  ill also optiona
-00010b40: 6c6c 7920 7570 6c6f 6164 2074 6865 2063  lly upload the c
-00010b50: 6f6e 736f 6c65 206f 7574 7075 7420 2869  onsole output (i
-00010b60: 6e63 6c75 6469 6e67 2062 6f74 6820 6073  ncluding both `s
-00010b70: 7464 6f75 7460 2061 6e64 2060 7374 6465  tdout` and `stde
-00010b80: 7272 6029 206f 6620 7468 6520 5461 736b  rr`) of the Task
-00010b90: 2c20 636f 6e74 6169 6e65 6420 696e 2074  , contained in t
-00010ba0: 6865 2060 7461 736b 6f75 7470 7574 2e74  he `taskoutput.t
-00010bb0: 7874 6020 6669 6c65 2e0a 352e 2054 6865  xt` file..5. The
-00010bc0: 2065 7068 656d 6572 616c 2054 6173 6b20   ephemeral Task 
-00010bd0: 6469 7265 6374 6f72 7920 6973 2074 6865  directory is the
-00010be0: 6e20 6465 6c65 7465 642e 0a0a 4e6f 7465  n deleted...Note
-00010bf0: 2074 6861 7420 6966 2061 2054 6173 6b20   that if a Task 
-00010c00: 6973 2061 626f 7274 6564 2064 7572 696e  is aborted durin
-00010c10: 6720 6578 6563 7574 696f 6e2c 2074 6865  g execution, the
-00010c20: 2054 6173 6b27 7320 7375 6270 726f 6365   Task's subproce
-00010c30: 7373 2069 7320 7365 6e74 2061 2060 5349  ss is sent a `SI
-00010c40: 4749 4e54 602c 2061 6c6c 6f77 696e 6720  GINT`, allowing 
-00010c50: 7468 6520 5461 736b 2061 6e20 6f70 706f  the Task an oppo
-00010c60: 7274 756e 6974 7920 746f 2074 6572 6d69  rtunity to termi
-00010c70: 6e61 7465 2061 6e79 2063 6869 6c64 2070  nate any child p
-00010c80: 726f 6365 7373 6573 206f 7220 6f74 6865  rocesses or othe
-00010c90: 7220 7265 736f 7572 6365 7320 2865 2e67  r resources (e.g
-00010ca0: 2e2c 2063 6f6e 7461 696e 6572 7329 2074  ., containers) t
-00010cb0: 6861 7420 6d61 7920 6861 7665 2062 6565  hat may have bee
-00010cc0: 6e20 7374 6172 7465 6420 6173 2070 6172  n started as par
-00010cd0: 7420 6f66 2054 6173 6b20 6578 6563 7574  t of Task execut
-00010ce0: 696f 6e2e 0a0a 4f6e 6365 2074 6865 2073  ion...Once the s
-00010cf0: 7465 7073 2061 626f 7665 2068 6176 6520  teps above have 
-00010d00: 6265 656e 2063 6f6d 706c 6574 6564 2c20  been completed, 
-00010d10: 7468 6520 576f 726b 6572 2069 7320 7265  the Worker is re
-00010d20: 6164 7920 746f 2061 6363 6570 7420 6974  ady to accept it
-00010d30: 7320 6e65 7874 2054 6173 6b20 6672 6f6d  s next Task from
-00010d40: 2074 6865 2059 656c 6c6f 7744 6f67 2073   the YellowDog s
-00010d50: 6368 6564 756c 6572 2e0a 0a4e 6f74 6520  cheduler...Note 
-00010d60: 7468 6174 2069 6620 7468 6520 4167 656e  that if the Agen
-00010d70: 7420 6f6e 2061 206e 6f64 6520 6861 7320  t on a node has 
-00010d80: 6d75 6c74 6970 6c65 2057 6f72 6b65 7273  multiple Workers
-00010d90: 2c20 7468 656e 2054 6173 6b73 2061 7265  , then Tasks are
-00010da0: 2065 7865 6375 7465 6420 696e 2070 6172   executed in par
-00010db0: 616c 6c65 6c20 6f6e 2074 6865 206e 6f64  allel on the nod
-00010dc0: 6520 616e 6420 6361 6e20 7374 6172 7420  e and can start 
-00010dd0: 616e 6420 7374 6f70 2069 6e64 6570 656e  and stop indepen
-00010de0: 6465 6e74 6c79 2e0a 0a23 2323 2054 6865  dently...### The
-00010df0: 2055 7365 7220 616e 6420 4772 6f75 7020   User and Group 
-00010e00: 7573 6564 2066 6f72 2054 6173 6b73 0a0a  used for Tasks..
-00010e10: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
-00010e20: 4167 656e 7420 7275 6e73 2061 7320 7573  Agent runs as us
-00010e30: 6572 2061 6e64 2067 726f 7570 2060 7964  er and group `yd
-00010e40: 2d61 6765 6e74 602c 2061 6e64 2068 656e  -agent`, and hen
-00010e50: 6365 2054 6173 6b73 2061 6c73 6f20 6578  ce Tasks also ex
-00010e60: 6563 7574 6520 756e 6465 7220 7468 6973  ecute under this
-00010e70: 2075 7365 722e 0a0a 6079 642d 6167 656e   user...`yd-agen
-00010e80: 7460 2064 6f65 7320 6e6f 7420 6861 7665  t` does not have
-00010e90: 2060 7375 646f 6020 7072 6976 696c 6567   `sudo` privileg
-00010ea0: 6573 2061 7320 7374 616e 6461 7264 2c20  es as standard, 
-00010eb0: 6275 7420 7468 6973 2063 616e 2062 6520  but this can be 
-00010ec0: 6164 6465 6420 6966 2072 6571 7569 7265  added if require
-00010ed0: 6420 6174 2069 6e73 7461 6e63 6520 626f  d at instance bo
-00010ee0: 6f74 2074 696d 6520 7669 6120 7468 6520  ot time via the 
-00010ef0: 6075 7365 7244 6174 6160 2070 726f 7065  `userData` prope
-00010f00: 7274 7920 6f66 2061 2070 726f 7669 7369  rty of a provisi
-00010f10: 6f6e 696e 6720 7265 7175 6573 742e 2045  oning request. E
-00010f20: 2e67 2e20 2866 6f72 2055 6275 6e74 7529  .g. (for Ubuntu)
-00010f30: 3a0a 0a60 6060 7368 656c 6c0a 7573 6572  :..```shell.user
-00010f40: 6d6f 6420 2d61 4720 7768 6565 6c20 7964  mod -aG wheel yd
-00010f50: 2d61 6765 6e74 0a65 6368 6f20 2d65 2022  -agent.echo -e "
-00010f60: 7964 2d61 6765 6e74 5c74 414c 4c3d 2841  yd-agent\tALL=(A
-00010f70: 4c4c 295c 744e 4f50 4153 5357 443a 2041  LL)\tNOPASSWD: A
-00010f80: 4c4c 2220 3e20 2f65 7463 2f73 7564 6f65  LL" > /etc/sudoe
-00010f90: 7273 2e64 2f30 3230 2d79 642d 6167 656e  rs.d/020-yd-agen
-00010fa0: 740a 6060 600a 0a23 2323 2048 6f6d 6520  t.```..### Home 
-00010fb0: 4469 7265 6374 6f72 7920 666f 7220 6079  Directory for `y
-00010fc0: 642d 6167 656e 7460 0a0a 4279 2064 6566  d-agent`..By def
-00010fd0: 6175 6c74 2c20 7468 6520 686f 6d65 2064  ault, the home d
-00010fe0: 6972 6563 746f 7279 206f 6620 7468 6520  irectory of the 
-00010ff0: 6079 642d 6167 656e 7460 2075 7365 7220  `yd-agent` user 
-00011000: 6973 2060 2f6f 7074 2f79 656c 6c6f 7764  is `/opt/yellowd
-00011010: 6f67 2f61 6765 6e74 602e 2054 6869 7320  og/agent`. This 
-00011020: 6469 7265 6374 6f72 7920 7479 7069 6361  directory typica
-00011030: 6c6c 7920 636f 6e74 6169 6e73 2074 6865  lly contains the
-00011040: 2060 6170 706c 6963 6174 696f 6e2e 7961   `application.ya
-00011050: 6d6c 6020 6669 6c65 2075 7365 6420 746f  ml` file used to
-00011060: 2063 6f6e 6669 6775 7265 2074 6865 2041   configure the A
-00011070: 6765 6e74 2c20 6173 2077 656c 6c20 6173  gent, as well as
-00011080: 2061 6e79 2073 6372 6970 7473 2074 6861   any scripts tha
-00011090: 7420 6172 6520 7573 6564 2074 6f20 6578  t are used to ex
-000110a0: 6563 7574 6520 7468 6520 5461 736b 2054  ecute the Task T
-000110b0: 7970 6573 2074 6861 7420 7468 6520 6e6f  ypes that the no
-000110c0: 6465 2073 7570 706f 7274 732e 0a0a 4966  de supports...If
-000110d0: 206f 6e65 2077 616e 7473 2074 6f20 5353   one wants to SS
-000110e0: 4820 746f 2061 6e20 696e 7374 616e 6365  H to an instance
-000110f0: 2061 7320 7573 6572 2060 7964 2d61 6765   as user `yd-age
-00011100: 6e74 602c 2070 6572 6861 7073 2066 6f72  nt`, perhaps for
-00011110: 2064 6562 7567 6769 6e67 2070 7572 706f   debugging purpo
-00011120: 7365 732c 2053 5348 206b 6579 7320 6361  ses, SSH keys ca
-00011130: 6e20 6265 2069 6e73 6572 7465 6420 7669  n be inserted vi
-00011140: 6120 696e 7374 616e 6365 2060 7573 6572  a instance `user
-00011150: 4461 7461 602c 2065 2e67 2e3a 0a0a 6060  Data`, e.g.:..``
-00011160: 6073 6865 6c6c 0a59 4441 5f48 4f4d 453d  `shell.YDA_HOME=
-00011170: 2f6f 7074 2f79 656c 6c6f 7764 6f67 2f61  /opt/yellowdog/a
-00011180: 6765 6e74 0a6d 6b64 6972 202d 7020 2459  gent.mkdir -p $Y
-00011190: 4441 5f48 4f4d 452f 2e73 7368 0a63 686d  DA_HOME/.ssh.chm
-000111a0: 6f64 206f 672d 7277 7820 2459 4441 5f48  od og-rwx $YDA_H
-000111b0: 4f4d 452f 2e73 7368 0a63 6174 203e 3e20  OME/.ssh.cat >> 
-000111c0: 2459 4441 5f48 4f4d 452f 2e73 7368 2f61  $YDA_HOME/.ssh/a
-000111d0: 7574 686f 7269 7a65 645f 6b65 7973 203c  uthorized_keys <
-000111e0: 3c20 454f 460a 3c3c 496e 7365 7274 5f50  < EOF.<<Insert_P
-000111f0: 7562 6c69 635f 6b65 795f 4865 7265 3e3e  ublic_key_Here>>
-00011200: 0a45 4f46 0a63 686d 6f64 206f 672d 7277  .EOF.chmod og-rw
-00011210: 2024 5944 415f 484f 4d45 2f2e 7373 682f   $YDA_HOME/.ssh/
-00011220: 6175 7468 6f72 697a 6564 5f6b 6579 730a  authorized_keys.
-00011230: 6368 6f77 6e20 2d52 2079 642d 6167 656e  chown -R yd-agen
-00011240: 743a 7964 2d61 6765 6e74 2024 5944 415f  t:yd-agent $YDA_
-00011250: 484f 4d45 2f2e 7373 680a 6060 600a 0a23  HOME/.ssh.```..#
-00011260: 2323 2054 6173 6b20 4578 6563 7574 696f  ## Task Executio
-00011270: 6e20 4469 7265 6374 6f72 790a 0a45 7068  n Directory..Eph
-00011280: 656d 6572 616c 2054 6173 6b20 6469 7265  emeral Task dire
-00011290: 6374 6f72 6965 7320 6172 6520 6279 2064  ctories are by d
-000112a0: 6566 6175 6c74 2063 7265 6174 6564 2075  efault created u
-000112b0: 6e64 6572 2060 2f76 6172 2f6f 7074 2f79  nder `/var/opt/y
-000112c0: 656c 6c6f 7764 6f67 2f61 6765 6e74 2f64  ellowdog/agent/d
-000112d0: 6174 612f 776f 726b 6572 7360 2e20 5468  ata/workers`. Th
-000112e0: 6973 2064 6972 6563 746f 7279 2063 6f6e  is directory con
-000112f0: 7461 696e 7320 6f6e 6520 6f72 206d 6f72  tains one or mor
-00011300: 6520 6e75 6d62 6572 6564 2073 7562 6469  e numbered subdi
-00011310: 7265 6374 6f72 6965 7320 7768 6572 6520  rectories where 
-00011320: 6561 6368 206e 756d 6265 7265 6420 6469  each numbered di
-00011330: 7265 6374 6f72 7920 636f 7272 6573 706f  rectory correspo
-00011340: 6e64 7320 746f 2061 2057 6f72 6b65 7220  nds to a Worker 
-00011350: 6f6e 2074 6865 206e 6f64 652e 0a0a 284f  on the node...(O
-00011360: 6e20 5769 6e64 6f77 7320 686f 7374 732c  n Windows hosts,
-00011370: 2074 6865 2054 6173 6b20 6469 7265 6374   the Task direct
-00011380: 6f72 6965 7320 6172 6520 666f 756e 6420  ories are found 
-00011390: 756e 6465 7220 6025 4170 7044 6174 6125  under `%AppData%
-000113a0: 5c79 656c 6c6f 7764 6f67 5c61 6765 6e74  \yellowdog\agent
-000113b0: 5c64 6174 615c 776f 726b 6572 7360 2e29  \data\workers`.)
-000113c0: 0a0a 5768 656e 2061 2054 6173 6b20 6973  ..When a Task is
-000113d0: 2061 6c6c 6f63 6174 6564 2074 6f20 6120   allocated to a 
-000113e0: 6e6f 6465 2c20 616e 2065 7068 656d 6572  node, an ephemer
-000113f0: 616c 2064 6972 6563 746f 7279 2069 7320  al directory is 
-00011400: 6372 6561 7465 6420 756e 6465 7220 7468  created under th
-00011410: 6520 6170 706c 6963 6162 6c65 2057 6f72  e applicable Wor
-00011420: 6b65 7220 6469 7265 6374 6f72 792c 2077  ker directory, w
-00011430: 6974 6820 6120 6e61 6d65 2063 6f72 7265  ith a name corre
-00011440: 7370 6f6e 6469 6e67 2074 6865 2059 656c  sponding the Yel
-00011450: 6c6f 7744 6f67 2049 4420 666f 7220 7468  lowDog ID for th
-00011460: 6520 5461 736b 2e20 466f 7220 6578 616d  e Task. For exam
-00011470: 706c 652c 2074 6869 7320 6973 2061 6e20  ple, this is an 
-00011480: 6570 6865 6d65 7261 6c20 6469 7265 6374  ephemeral direct
-00011490: 6f72 7920 6265 696e 6720 7573 6564 2062  ory being used b
-000114a0: 7920 576f 726b 6572 206e 756d 6265 7220  y Worker number 
-000114b0: 6031 603a 0a0a 602f 7661 722f 6f70 742f  `1`:..`/var/opt/
-000114c0: 7965 6c6c 6f77 646f 672f 6167 656e 742f  yellowdog/agent/
-000114d0: 6461 7461 2f77 6f72 6b65 7273 2f31 2f79  data/workers/1/y
-000114e0: 6469 645f 7461 736b 5f35 3539 4542 455f  did_task_559EBE_
-000114f0: 3734 3934 3933 3336 2d61 6332 622d 3438  74949336-ac2b-48
-00011500: 3131 2d61 3764 352d 6633 6563 6439 3733  11-a7d5-f3ecd973
-00011510: 3939 3038 5f31 5f31 600a 0a54 6869 7320  9908_1_1`..This 
-00011520: 6973 2074 6865 2064 6972 6563 746f 7279  is the directory
-00011530: 2069 6e74 6f20 7768 6963 6820 646f 776e   into which down
-00011540: 6c6f 6164 6564 206f 626a 6563 7473 2061  loaded objects a
-00011550: 7265 2070 6c61 6365 642c 2061 6e64 2069  re placed, and i
-00011560: 6e20 7768 6963 6820 6f75 7470 7574 2066  n which output f
-00011570: 696c 6573 2061 7265 2063 7265 6174 6564  iles are created
-00011580: 2062 7920 6465 6661 756c 742e 2054 6865   by default. The
-00011590: 2063 6f6e 736f 6c65 206f 7574 7075 7420   console output 
-000115a0: 6074 6173 6b6f 7574 7075 742e 7478 7460  `taskoutput.txt`
-000115b0: 2066 696c 6520 7769 6c6c 2061 6c73 6f20   file will also 
-000115c0: 6265 2063 7265 6174 6564 2069 6e20 7468  be created in th
-000115d0: 6973 2064 6972 6563 746f 7279 2e0a 0a53  is directory...S
-000115e0: 6565 2074 6865 205b 4669 6c65 7320 446f  ee the [Files Do
-000115f0: 776e 6c6f 6164 6564 2074 6f20 6120 4e6f  wnloaded to a No
-00011600: 6465 5d28 2366 696c 6573 2d64 6f77 6e6c  de](#files-downl
-00011610: 6f61 6465 642d 746f 2d61 2d6e 6f64 652d  oaded-to-a-node-
-00011620: 666f 722d 7573 652d 696e 2d74 6173 6b2d  for-use-in-task-
-00011630: 6578 6563 7574 696f 6e29 2073 6563 7469  execution) secti
-00011640: 6f6e 2061 626f 7665 2066 6f72 206d 6f72  on above for mor
-00011650: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
-00011660: 2066 696c 6573 2069 6e20 7468 6973 2064   files in this d
-00011670: 6972 6563 746f 7279 2061 7265 2068 616e  irectory are han
-00011680: 646c 6564 2e0a 0a41 7420 7468 6520 636f  dled...At the co
-00011690: 6e63 6c75 7369 6f6e 206f 6620 7468 6520  nclusion of the 
-000116a0: 5461 736b 2c20 6166 7465 7220 616e 7920  Task, after any 
-000116b0: 6669 6c65 7320 7265 7175 6573 7465 6420  files requested 
-000116c0: 666f 7220 7570 6c6f 6164 2068 6176 6520  for upload have 
-000116d0: 6265 656e 2075 706c 6f61 6465 6420 746f  been uploaded to
-000116e0: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
-000116f0: 6520 2873 6565 2074 6865 205b 4669 6c65  e (see the [File
-00011700: 7320 5570 6c6f 6164 6564 2066 726f 6d20  s Uploaded from 
-00011710: 6120 4e6f 6465 5d28 2366 696c 6573 2d75  a Node](#files-u
-00011720: 706c 6f61 6465 642d 6672 6f6d 2d61 2d6e  ploaded-from-a-n
-00011730: 6f64 652d 746f 2d74 6865 2d6f 626a 6563  ode-to-the-objec
-00011740: 742d 7374 6f72 652d 6166 7465 722d 7461  t-store-after-ta
-00011750: 736b 2d65 7865 6375 7469 6f6e 2920 7365  sk-execution) se
-00011760: 6374 696f 6e20 666f 7220 6d6f 7265 2069  ction for more i
-00011770: 6e66 6f72 6d61 7469 6f6e 292c 2074 6865  nformation), the
-00011780: 2060 7964 6964 5f74 6173 6b5f 3535 3945   `ydid_task_559E
-00011790: 4245 5f37 3439 3439 3333 362d 6163 3262  BE_74949336-ac2b
-000117a0: 2d34 3831 312d 6137 6435 2d66 3365 6364  -4811-a7d5-f3ecd
-000117b0: 3937 3339 3930 385f 315f 3160 2077 696c  9739908_1_1` wil
-000117c0: 6c20 6265 2072 656d 6f76 6564 2e0a 0a23  l be removed...#
-000117d0: 2320 5370 6563 6966 7969 6e67 2057 6f72  # Specifying Wor
-000117e0: 6b20 5265 7175 6972 656d 656e 7473 2075  k Requirements u
-000117f0: 7369 6e67 2043 5356 2044 6174 610a 0a43  sing CSV Data..C
-00011800: 5356 2064 6174 6120 6669 6c65 7320 6361  SV data files ca
-00011810: 6e20 6265 2075 7365 6420 746f 2064 7269  n be used to dri
-00011820: 7665 2074 6865 2067 656e 6572 6174 696f  ve the generatio
-00011830: 6e20 6f66 206c 6973 7473 206f 6620 5461  n of lists of Ta
-00011840: 736b 732c 2061 7320 666f 6c6c 6f77 733a  sks, as follows:
-00011850: 0a0a 2d20 4120 2a2a 7072 6f74 6f74 7970  ..- A **prototyp
-00011860: 652a 2a20 5461 736b 2073 7065 6369 6669  e** Task specifi
-00011870: 6361 7469 6f6e 2069 7320 6372 6561 7465  cation is create
-00011880: 6420 7769 7468 696e 2061 204a 534f 4e20  d within a JSON 
-00011890: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-000118a0: 2073 7065 6369 6669 6361 7469 6f6e 206f   specification o
-000118b0: 7220 696e 2074 6865 2060 776f 726b 5265  r in the `workRe
-000118c0: 7175 6972 656d 656e 7460 2073 6563 7469  quirement` secti
-000118d0: 6f6e 206f 6620 7468 6520 544f 4d4c 2063  on of the TOML c
-000118e0: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-000118f0: 650a 2d20 5468 6520 7072 6f74 6f74 7970  e.- The prototyp
-00011900: 6520 7461 736b 2069 6e63 6c75 6465 7320  e task includes 
-00011910: 6f6e 6520 6f72 206d 6f72 6520 7661 7269  one or more vari
-00011920: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00011930: 6e73 0a2d 2041 2043 5356 2066 696c 6520  ns.- A CSV file 
-00011940: 6973 2063 7265 6174 6564 2c20 7769 7468  is created, with
-00011950: 2074 6865 202a 2a68 6561 6465 7273 2a2a   the **headers**
-00011960: 2028 6669 7273 7420 726f 7729 206d 6174   (first row) mat
-00011970: 6368 696e 6720 7468 6520 6e61 6d65 7320  ching the names 
-00011980: 6f66 2074 6865 2076 6172 6961 626c 6520  of the variable 
-00011990: 7375 6273 7469 7475 7469 6f6e 7320 696e  substitutions in
-000119a0: 2074 6865 2054 6173 6b20 7072 6f74 6f74   the Task protot
-000119b0: 7970 650a 2d20 4561 6368 2073 7562 7365  ype.- Each subse
-000119c0: 7175 656e 7420 726f 7720 6f66 2074 6865  quent row of the
-000119d0: 2043 5356 2066 696c 6520 7265 7072 6573   CSV file repres
-000119e0: 656e 7473 2061 206e 6577 2054 6173 6b20  ents a new Task 
-000119f0: 6275 696c 7420 7573 696e 6720 7468 6520  built using the 
-00011a00: 7072 6f74 6f74 7970 652c 2077 6974 6820  prototype, with 
-00011a10: 7468 6520 7661 7269 6162 6c65 7320 7375  the variables su
-00011a20: 6273 7469 7475 7465 6420 6279 2074 6865  bstituted by the
-00011a30: 2076 616c 7565 7320 696e 2074 6865 2072   values in the r
-00011a40: 6f77 0a2d 2041 2054 6173 6b20 7769 6c6c  ow.- A Task will
-00011a50: 2062 6520 6372 6561 7465 6420 666f 7220   be created for 
-00011a60: 6561 6368 2064 6174 6120 726f 770a 0a23  each data row..#
-00011a70: 2323 2057 6f72 6b20 5265 7175 6972 656d  ## Work Requirem
-00011a80: 656e 7420 4353 5620 4461 7461 2045 7861  ent CSV Data Exa
-00011a90: 6d70 6c65 0a0a 4173 2061 6e20 6578 616d  mple..As an exam
-00011aa0: 706c 652c 2063 6f6e 7369 6465 7220 7468  ple, consider th
-00011ab0: 6520 666f 6c6c 6f77 696e 6720 4a53 4f4e  e following JSON
-00011ac0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00011ad0: 7420 6077 722e 6a73 6f6e 603a 0a0a 6060  t `wr.json`:..``
-00011ae0: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
-00011af0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
-00011b00: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
-00011b10: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00011b20: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
-00011b30: 3a20 5b22 7b7b 6172 675f 317d 7d22 2c20  : ["{{arg_1}}", 
-00011b40: 227b 7b61 7267 5f32 7d7d 222c 2022 7b7b  "{{arg_2}}", "{{
-00011b50: 6172 675f 337d 7d22 5d2c 0a20 2020 2020  arg_3}}"],.     
-00011b60: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-00011b70: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
-00011b80: 3a20 227b 7b65 6e76 5f31 7d7d 227d 0a20  : "{{env_1}}"}. 
-00011b90: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-00011ba0: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
-00011bb0: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
-00011bc0: 5461 736b 2047 726f 7570 206d 7573 7420  Task Group must 
-00011bd0: 636f 6e74 6169 6e20 6f6e 6c79 2061 2073  contain only a s
-00011be0: 696e 676c 6520 5461 736b 2c20 6163 7469  ingle Task, acti
-00011bf0: 6e67 2061 7320 7468 6520 7072 6f74 6f74  ng as the protot
-00011c00: 7970 652e 0a0a 4e6f 7720 636f 6e73 6964  ype...Now consid
-00011c10: 6572 2061 2043 5356 2066 696c 6520 6077  er a CSV file `w
-00011c20: 725f 6461 7461 2e63 7376 6020 7769 7468  r_data.csv` with
-00011c30: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00011c40: 6f6e 7465 6e74 733a 0a0a 6060 6074 6578  ontents:..```tex
-00011c50: 740a 6172 675f 312c 2061 7267 5f32 2c20  t.arg_1, arg_2, 
-00011c60: 6172 675f 332c 2065 6e76 5f31 0a41 2c20  arg_3, env_1.A, 
-00011c70: 2020 2020 422c 2020 2020 2043 2c20 2020      B,     C,   
-00011c80: 2020 452d 310a 442c 2020 2020 2045 2c20    E-1.D,     E, 
-00011c90: 2020 2020 462c 2020 2020 2045 2d32 0a47      F,     E-2.G
-00011ca0: 2c20 2020 2020 482c 2020 2020 2049 2c20  ,     H,     I, 
-00011cb0: 2020 2020 452d 330a 6060 600a 0a4e 6f74      E-3.```..Not
-00011cc0: 6520 7468 6174 2074 6865 2028 6f70 7469  e that the (opti
-00011cd0: 6f6e 616c 2920 6c65 6164 696e 6720 7370  onal) leading sp
-00011ce0: 6163 6573 2061 6674 6572 2065 6163 6820  aces after each 
-00011cf0: 636f 6d6d 6120 6172 6520 6967 6e6f 7265  comma are ignore
-00011d00: 642c 2062 7574 2074 7261 696c 696e 6720  d, but trailing 
-00011d10: 7370 6163 6573 2061 7265 206e 6f74 2061  spaces are not a
-00011d20: 6e64 2077 696c 6c20 666f 726d 2070 6172  nd will form par
-00011d30: 7420 6f66 2074 6865 2069 6d70 6f72 7465  t of the importe
-00011d40: 6420 6461 7461 2e0a 0a49 6620 7468 6573  d data...If thes
-00011d50: 6520 6669 6c65 7320 6172 6520 7072 6f63  e files are proc
-00011d60: 6573 7365 6420 7573 696e 6720 6079 642d  essed using `yd-
-00011d70: 7375 626d 6974 202d 7220 7772 2e6a 736f  submit -r wr.jso
-00011d80: 6e20 2d56 2077 725f 6461 7461 2e63 7376  n -V wr_data.csv
-00011d90: 602c 2074 6865 2066 6f6c 6c6f 7769 6e67  `, the following
-00011da0: 2065 7870 616e 6465 6420 6c69 7374 206f   expanded list o
-00011db0: 6620 7468 7265 6520 5461 736b 7320 7769  f three Tasks wi
-00011dc0: 6c6c 2062 6520 6372 6561 7465 6420 7072  ll be created pr
-00011dd0: 696f 7220 746f 2066 7572 7468 6572 2070  ior to further p
-00011de0: 726f 6365 7373 696e 6720 6279 2074 6865  rocessing by the
-00011df0: 2060 7964 2d73 7562 6d69 7460 2073 6372   `yd-submit` scr
-00011e00: 6970 743a 0a0a 6060 606a 736f 6e0a 7b0a  ipt:..```json.{.
-00011e10: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
-00011e20: 5b0a 2020 2020 7b0a 2020 2020 2020 2274  [.    {.      "t
-00011e30: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
-00011e40: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-00011e50: 6775 6d65 6e74 7322 3a20 5b22 4122 2c20  guments": ["A", 
-00011e60: 2242 222c 2022 4322 5d2c 0a20 2020 2020  "B", "C"],.     
-00011e70: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-00011e80: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
-00011e90: 3a20 2245 2d31 227d 0a20 2020 2020 2020  : "E-1"}.       
-00011ea0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00011eb0: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00011ec0: 7473 223a 205b 2244 222c 2022 4522 2c20  ts": ["D", "E", 
-00011ed0: 2246 225d 2c0a 2020 2020 2020 2020 2020  "F"],.          
-00011ee0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-00011ef0: 2245 4e56 5f56 4152 5f31 223a 2022 452d  "ENV_VAR_1": "E-
-00011f00: 3222 7d0a 2020 2020 2020 2020 7d2c 0a20  2"}.        },. 
-00011f10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00011f20: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
-00011f30: 5b22 4722 2c20 2248 222c 2022 4922 5d2c  ["G", "H", "I"],
-00011f40: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
-00011f50: 726f 6e6d 656e 7422 3a20 7b22 454e 565f  ronment": {"ENV_
-00011f60: 5641 525f 3122 3a20 2245 2d33 227d 0a20  VAR_1": "E-3"}. 
-00011f70: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-00011f80: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
-00011f90: 0a0a 2323 2320 4353 5620 5661 7269 6162  ..### CSV Variab
-00011fa0: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
-00011fb0: 0a0a 5768 656e 2074 6865 2043 5356 2066  ..When the CSV f
-00011fc0: 696c 6520 6461 7461 2069 7320 7072 6f63  ile data is proc
-00011fd0: 6573 7365 642c 2074 6865 206f 6e6c 7920  essed, the only 
-00011fe0: 7375 6273 7469 7475 7469 6f6e 7320 6d61  substitutions ma
-00011ff0: 6465 2061 7265 2074 686f 7365 2077 6869  de are those whi
-00012000: 6368 206d 6174 6368 2074 6865 2076 6172  ch match the var
-00012010: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00012020: 6f6e 7320 696e 2074 6865 2070 726f 746f  ons in the proto
-00012030: 7479 7065 2054 6173 6b2e 2054 6865 2043  type Task. The C
-00012040: 5356 2066 696c 6520 6973 2074 6865 202a  SV file is the *
-00012050: 2a6f 6e6c 792a 2a20 736f 7572 6365 206f  *only** source o
-00012060: 6620 7375 6273 7469 7475 7469 6f6e 7320  f substitutions 
-00012070: 7573 6564 2066 6f72 2074 6869 7320 7072  used for this pr
-00012080: 6f63 6573 7369 6e67 2070 6861 7365 3b20  ocessing phase; 
-00012090: 616c 6c20 6f74 6865 7220 7661 7269 6162  all other variab
-000120a0: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
-000120b0: 2028 7375 7070 6c69 6564 206f 6e20 7468   (supplied on th
-000120c0: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
-000120d0: 696e 2074 6865 2054 4f4d 4c20 636f 6e66  in the TOML conf
-000120e0: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
-000120f0: 6f72 2066 726f 6d20 656e 7669 726f 6e6d  or from environm
-00012100: 656e 7420 7661 7269 6162 6c65 7329 2061  ent variables) a
-00012110: 7265 2069 676e 6f72 6564 202d 2d20 692e  re ignored -- i.
-00012120: 652e 2c20 7468 6579 2064 6f20 6e6f 7420  e., they do not 
-00012130: 6f76 6572 7269 6465 2074 6865 2063 6f6e  override the con
-00012140: 7465 6e74 7320 6f66 2074 6865 2043 5356  tents of the CSV
-00012150: 2066 696c 652e 0a0a 416c 6c20 7661 7269   file...All vari
-00012160: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00012170: 6e73 2075 6e72 656c 6174 6564 2074 6f20  ns unrelated to 
-00012180: 7468 6520 4353 5620 6669 6c65 2064 6174  the CSV file dat
-00012190: 6120 6172 6520 6c65 6674 2075 6e63 6861  a are left uncha
-000121a0: 6e67 6564 2c20 666f 7220 7375 6273 6571  nged, for subseq
-000121b0: 7565 6e74 2070 726f 6365 7373 696e 6720  uent processing 
-000121c0: 6279 2060 7964 2d73 7562 6d69 7460 2e0a  by `yd-submit`..
-000121d0: 0a49 6620 7468 6520 7661 6c75 6520 746f  .If the value to
-000121e0: 2062 6520 696e 7365 7274 6564 2069 7320   be inserted is 
-000121f0: 6120 6e75 6d62 6572 2028 616e 2069 6e74  a number (an int
-00012200: 6567 6572 206f 7220 666c 6f61 7469 6e67  eger or floating
-00012210: 2070 6f69 6e74 2076 616c 7565 2920 6f72   point value) or
-00012220: 2042 6f6f 6c65 616e 2c20 7468 6520 607b   Boolean, the `{
-00012230: 7b6e 756d 3a6d 795f 6e75 6d62 6572 5f76  {num:my_number_v
-00012240: 6172 7d7d 6020 616e 6420 607b 7b62 6f6f  ar}}` and `{{boo
-00012250: 6c3a 6d79 5f62 6f6f 6c65 616e 5f76 6172  l:my_boolean_var
-00012260: 7d7d 6020 666f 726d 7320 6361 6e20 6265  }}` forms can be
-00012270: 2075 7365 6420 696e 2074 6865 204a 534f   used in the JSO
-00012280: 4e20 6669 6c65 2c20 6173 2077 6974 6820  N file, as with 
-00012290: 7468 6569 7220 7573 6520 696e 206f 7468  their use in oth
-000122a0: 6572 2070 6172 7473 206f 6620 7468 6520  er parts of the 
-000122b0: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
-000122c0: 656d 656e 7420 7370 6563 6966 6963 6174  ement specificat
-000122d0: 696f 6e2e 2054 6865 2073 7562 7374 6974  ion. The substit
-000122e0: 7574 6564 2076 616c 7565 2077 696c 6c20  uted value will 
-000122f0: 6173 7375 6d65 2074 6865 206e 6f6d 696e  assume the nomin
-00012300: 6174 6564 2074 7970 6520 7261 7468 6572  ated type rather
-00012310: 2074 6861 6e20 6265 696e 6720 6120 7374   than being a st
-00012320: 7269 6e67 2e0a 0a23 2323 2050 726f 7065  ring...### Prope
-00012330: 7274 7920 496e 6865 7269 7461 6e63 650a  rty Inheritance.
-00012340: 0a41 6c6c 2074 6865 2075 7375 616c 2070  .All the usual p
-00012350: 726f 7065 7274 7920 696e 6865 7269 7461  roperty inherita
-00012360: 6e63 6520 6665 6174 7572 6573 206f 7065  nce features ope
-00012370: 7261 7465 2061 7320 6e6f 726d 616c 2e20  rate as normal. 
-00012380: 5072 6f70 6572 7469 6573 2061 7265 2069  Properties are i
-00012390: 6e68 6572 6974 6564 2066 726f 6d20 7468  nherited from th
-000123a0: 6520 6063 6f6e 6669 672e 746f 6d6c 6020  e `config.toml` 
-000123b0: 6669 6c65 2c20 616e 6420 6672 6f6d 2074  file, and from t
-000123c0: 6865 2072 656c 6576 616e 7420 7365 6374  he relevant sect
-000123d0: 696f 6e73 206f 6620 7468 6520 4a53 4f4e  ions of the JSON
-000123e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-000123f0: 7420 6669 6c65 2e20 416e 7920 7072 6f70  t file. Any prop
-00012400: 6572 7469 6573 2073 6574 2077 6974 6869  erties set withi
-00012410: 6e20 6120 5461 736b 2070 726f 746f 7479  n a Task prototy
-00012420: 7065 2061 7265 2063 6f70 6965 6420 746f  pe are copied to
-00012430: 2061 6c6c 2074 6865 2067 656e 6572 6174   all the generat
-00012440: 6564 2054 6173 6b73 2e0a 0a23 2323 204d  ed Tasks...### M
-00012450: 756c 7469 706c 6520 5461 736b 2047 726f  ultiple Task Gro
-00012460: 7570 7320 7573 696e 6720 4d75 6c74 6970  ups using Multip
-00012470: 6c65 2043 5356 2046 696c 6573 0a0a 5468  le CSV Files..Th
-00012480: 6520 7573 6520 6f66 206d 756c 7469 706c  e use of multipl
-00012490: 6520 5461 736b 2047 726f 7570 7320 6973  e Task Groups is
-000124a0: 2061 6c73 6f20 7375 7070 6f72 7465 642c   also supported,
-000124b0: 2062 7920 7573 696e 6720 6f6e 6520 4353   by using one CS
-000124c0: 5620 6669 6c65 2070 6572 2054 6173 6b20  V file per Task 
-000124d0: 4772 6f75 702e 2045 6163 6820 5461 736b  Group. Each Task
-000124e0: 2047 726f 7570 206d 7573 7420 636f 6e74   Group must cont
-000124f0: 6169 6e20 6f6e 6c79 2061 2073 696e 676c  ain only a singl
-00012500: 6520 7072 6f74 6f74 7970 6520 5461 736b  e prototype Task
-00012510: 2e0a 0a54 6865 2043 5356 2066 696c 6573  ...The CSV files
-00012520: 2061 7265 2073 7570 706c 6965 6420 6f6e   are supplied on
-00012530: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00012540: 6520 696e 2074 6865 206f 7264 6572 206f  e in the order o
-00012550: 6620 7468 6520 5461 736b 2047 726f 7570  f the Task Group
-00012560: 7320 746f 2077 6869 6368 2074 6865 7920  s to which they 
-00012570: 6170 706c 792e 2046 6f72 2065 7861 6d70  apply. For examp
-00012580: 6c65 2c20 6966 2060 7772 5f6a 736f 6e60  le, if `wr_json`
-00012590: 2063 6f6e 7461 696e 7320 7477 6f20 5461   contains two Ta
-000125a0: 736b 2047 726f 7570 732c 2061 7320 666f  sk Groups, as fo
-000125b0: 6c6c 6f77 733a 0a0a 6060 606a 736f 6e0a  llows:..```json.
-000125c0: 7b0a 2020 2274 6173 6b47 726f 7570 7322  {.  "taskGroups"
-000125d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-000125e0: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
-000125f0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00012600: 6172 6775 6d65 6e74 7322 3a20 5b22 7b7b  arguments": ["{{
-00012610: 6172 675f 317d 7d22 2c20 227b 7b61 7267  arg_1}}", "{{arg
-00012620: 5f32 7d7d 222c 2022 7b7b 6172 675f 337d  _2}}", "{{arg_3}
-00012630: 7d22 5d2c 0a20 2020 2020 2020 2020 2022  }"],.          "
-00012640: 656e 7669 726f 6e6d 656e 7422 3a20 7b22  environment": {"
-00012650: 454e 565f 5641 525f 3122 3a20 227b 7b65  ENV_VAR_1": "{{e
-00012660: 6e76 5f31 7d7d 227d 0a20 2020 2020 2020  nv_1}}"}.       
-00012670: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
-00012680: 2c0a 2020 2020 7b0a 2020 2020 2020 2274  ,.    {.      "t
-00012690: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
-000126a0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-000126b0: 6775 6d65 6e74 7322 3a20 5b22 7b7b 6172  guments": ["{{ar
-000126c0: 675f 317d 7d22 2c20 227b 7b61 7267 5f32  g_1}}", "{{arg_2
-000126d0: 7d7d 225d 2c0a 2020 2020 2020 2020 2020  }}"],.          
-000126e0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-000126f0: 2245 4e56 5f56 4152 5f31 223a 2022 7b7b  "ENV_VAR_1": "{{
-00012700: 656e 765f 317d 7d22 2c20 2245 4e56 5f56  env_1}}", "ENV_V
-00012710: 4152 5f32 223a 2022 7b7b 656e 765f 327d  AR_2": "{{env_2}
-00012720: 7d22 7d0a 2020 2020 2020 2020 7d0a 2020  }"}.        }.  
-00012730: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
-00012740: 7d0a 6060 600a 0a54 6865 2060 7964 2d73  }.```..The `yd-s
-00012750: 7562 6d69 7460 2063 6f6d 6d61 6e64 2077  ubmit` command w
-00012760: 6f75 6c64 2074 6865 6e20 6265 2069 6e76  ould then be inv
-00012770: 6f6b 6564 2077 6974 6820 6120 7365 7061  oked with a sepa
-00012780: 7261 7465 2043 5356 2066 696c 6520 666f  rate CSV file fo
-00012790: 7220 6561 6368 2054 6173 6b20 4772 6f75  r each Task Grou
-000127a0: 702c 2065 2e67 2e3a 0a0a 6060 6073 6865  p, e.g.:..```she
-000127b0: 6c6c 0a79 642d 7375 626d 6974 202d 7220  ll.yd-submit -r 
-000127c0: 7772 2e6a 736f 6e20 2d56 2077 725f 6461  wr.json -V wr_da
-000127d0: 7461 5f74 6173 6b5f 6772 6f75 705f 312e  ta_task_group_1.
-000127e0: 6373 7620 2d56 2077 725f 6461 7461 5f74  csv -V wr_data_t
-000127f0: 6173 6b5f 6772 6f75 705f 322e 6373 760a  ask_group_2.csv.
-00012800: 6060 600a 0a49 6620 7468 6572 6520 6172  ```..If there ar
-00012810: 6520 2a2a 6665 7765 722a 2a20 4353 5620  e **fewer** CSV 
-00012820: 6669 6c65 7320 7468 616e 2054 6173 6b20  files than Task 
-00012830: 4772 6f75 7073 2061 2077 6172 6e69 6e67  Groups a warning
-00012840: 2077 696c 6c20 6265 2070 7269 6e74 6564   will be printed
-00012850: 2061 6e64 2c20 6966 2074 6865 7265 2061   and, if there a
-00012860: 7265 2027 6e27 2043 5356 2066 696c 6573  re 'n' CSV files
-00012870: 2c20 4353 5620 6461 7461 2070 726f 6365  , CSV data proce
-00012880: 7373 696e 6720 7769 6c6c 2062 6520 6170  ssing will be ap
-00012890: 706c 6965 6420 746f 2074 6865 2066 6972  plied to the fir
-000128a0: 7374 2027 6e27 2054 6173 6b20 4772 6f75  st 'n' Task Grou
-000128b0: 7073 2069 6e20 7468 6520 576f 726b 2052  ps in the Work R
-000128c0: 6571 7569 7265 6d65 6e74 2062 7920 6465  equirement by de
-000128d0: 6661 756c 742c 2069 6e20 7468 6520 6f72  fault, in the or
-000128e0: 6465 7220 696e 2077 6869 6368 2074 6865  der in which the
-000128f0: 2043 5356 2066 696c 6573 2077 6572 6520   CSV files were 
-00012900: 7375 7070 6c69 6564 2e20 4966 2074 6865  supplied. If the
-00012910: 7265 2061 7265 202a 2a6d 6f72 652a 2a20  re are **more** 
-00012920: 4353 5620 6669 6c65 7320 7468 616e 2054  CSV files than T
-00012930: 6173 6b20 4772 6f75 7073 2c20 616e 2065  ask Groups, an e
-00012940: 7272 6f72 2077 696c 6c20 6265 2072 6169  rror will be rai
-00012950: 7365 6420 616e 6420 7072 6f63 6573 7369  sed and processi
-00012960: 6e67 2077 696c 6c20 7374 6f70 2e0a 0a49  ng will stop...I
-00012970: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
-00012980: 2061 7070 6c79 2043 5356 2066 696c 6573   apply CSV files
-00012990: 2065 7870 6c69 6369 746c 7920 746f 2073   explicitly to s
-000129a0: 7065 6369 6669 6320 5461 736b 2047 726f  pecific Task Gro
-000129b0: 7570 732c 2062 7920 7573 696e 6720 616e  ups, by using an
-000129c0: 206f 7074 696f 6e61 6c20 2a2a 696e 6465   optional **inde
-000129d0: 7820 706f 7374 6669 782a 2a20 2865 2e67  x postfix** (e.g
-000129e0: 2e2c 2060 3a32 6029 2061 7420 7468 6520  ., `:2`) at the 
-000129f0: 656e 6420 6f66 2065 6163 6820 4353 5620  end of each CSV 
-00012a00: 6669 6c65 6e61 6d65 2e20 466f 7220 6578  filename. For ex
-00012a10: 616d 706c 652c 2069 6620 7468 6572 6520  ample, if there 
-00012a20: 6172 6520 7477 6f20 4353 5620 6669 6c65  are two CSV file
-00012a30: 7320 746f 2062 6520 6170 706c 6965 6420  s to be applied 
-00012a40: 746f 2074 6865 2073 6563 6f6e 6420 616e  to the second an
-00012a50: 6420 666f 7572 7468 2054 6173 6b20 4772  d fourth Task Gr
-00012a60: 6f75 7073 2069 6e20 6120 4a53 4f4e 2057  oups in a JSON W
-00012a70: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
-00012a80: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00012a90: 6e67 2073 796e 7461 783a 0a0a 6060 6073  ng syntax:..```s
-00012aa0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
-00012ab0: 7220 7772 2e6a 736f 6e20 2d56 2077 725f  r wr.json -V wr_
-00012ac0: 6461 7461 5f74 6173 6b5f 6772 6f75 705f  data_task_group_
-00012ad0: 322e 6373 763a 3220 2d56 2077 725f 6461  2.csv:2 -V wr_da
-00012ae0: 7461 5f74 6173 6b5f 6772 6f75 705f 342e  ta_task_group_4.
-00012af0: 6373 763a 340a 6060 600a 0a41 6c74 6572  csv:4.```..Alter
-00012b00: 6e61 7469 7665 6c79 2c20 7468 6520 2a2a  natively, the **
-00012b10: 5461 736b 2047 726f 7570 206e 616d 652a  Task Group name*
-00012b20: 2a20 2869 6620 7375 7070 6c69 6564 2069  * (if supplied i
-00012b30: 6e20 7468 6520 4a53 4f4e 2066 696c 6529  n the JSON file)
-00012b40: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
-00012b50: 7468 6520 706f 7374 6669 782e 2046 6f72  the postfix. For
-00012b60: 2065 7861 6d70 6c65 2c20 6966 2074 6865   example, if the
-00012b70: 2054 6173 6b20 4772 6f75 7073 2061 626f   Task Groups abo
-00012b80: 7665 2061 7265 206e 616d 6564 2060 7467  ve are named `tg
-00012b90: 5f74 776f 6020 616e 6420 6074 675f 666f  _two` and `tg_fo
-00012ba0: 7572 602c 2074 6865 2060 7964 2d73 7562  ur`, the `yd-sub
-00012bb0: 6d69 7460 2063 6f6d 6d61 6e64 2077 6f75  mit` command wou
-00012bc0: 6c64 2062 6563 6f6d 653a 0a0a 6060 6073  ld become:..```s
-00012bd0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
-00012be0: 7220 7772 2e6a 736f 6e20 2d56 2077 725f  r wr.json -V wr_
-00012bf0: 6461 7461 5f74 6173 6b5f 6772 6f75 705f  data_task_group_
-00012c00: 322e 6373 763a 7467 5f74 776f 202d 5620  2.csv:tg_two -V 
-00012c10: 7772 5f64 6174 615f 7461 736b 5f67 726f  wr_data_task_gro
-00012c20: 7570 5f34 2e63 7376 3a74 675f 666f 7572  up_4.csv:tg_four
-00012c30: 0a60 6060 0a0a 4e6f 7465 2074 6861 7420  .```..Note that 
-00012c40: 6f6e 6c79 206f 6e65 2043 5356 2066 696c  only one CSV fil
-00012c50: 6520 6361 6e20 6265 2061 7070 6c69 6564  e can be applied
-00012c60: 2074 6f20 616e 7920 6769 7665 6e20 5461   to any given Ta
-00012c70: 736b 2047 726f 7570 2e20 4120 7369 6e67  sk Group. A sing
-00012c80: 6c65 2043 5356 2066 696c 6520 6361 6e2c  le CSV file can,
-00012c90: 2068 6f77 6576 6572 2c20 6265 2072 6575   however, be reu
-00012ca0: 7365 6420 666f 7220 6d75 6c74 6970 6c65  sed for multiple
-00012cb0: 2054 6173 6b20 4772 6f75 7073 2e0a 0a23   Task Groups...#
-00012cc0: 2323 2055 7369 6e67 2043 5356 2044 6174  ## Using CSV Dat
-00012cd0: 6120 7769 7468 2053 696d 706c 652c 2054  a with Simple, T
-00012ce0: 4f4d 4c2d 4f6e 6c79 2057 6f72 6b20 5265  OML-Only Work Re
-00012cf0: 7175 6972 656d 656e 7420 5370 6563 6966  quirement Specif
-00012d00: 6963 6174 696f 6e73 0a0a 4974 2773 2070  ications..It's p
-00012d10: 6f73 7369 626c 6520 746f 2075 7365 2054  ossible to use T
-00012d20: 4f4d 4c20 6578 636c 7573 6976 656c 7920  OML exclusively 
-00012d30: 746f 2064 6572 6976 6520 6120 6c69 7374  to derive a list
-00012d40: 206f 6620 5461 736b 7320 6672 6f6d 2043   of Tasks from C
-00012d50: 5356 2064 6174 6120 2d2d 2069 2e65 2e2c  SV data -- i.e.,
-00012d60: 2061 204a 534f 4e20 576f 726b 2052 6571   a JSON Work Req
-00012d70: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
-00012d80: 6361 7469 6f6e 2069 7320 6e6f 7420 7265  cation is not re
-00012d90: 7175 6972 6564 2e0a 0a54 6f20 6d61 6b65  quired...To make
-00012da0: 2075 7365 206f 6620 7468 6973 3a0a 0a31   use of this:..1
-00012db0: 2e20 456e 7375 7265 2074 6861 7420 6e6f  . Ensure that no
-00012dc0: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
-00012dd0: 7265 6d65 6e74 2064 6f63 756d 656e 7420  rement document 
-00012de0: 6973 2073 7065 6369 6669 6564 2028 6e6f  is specified (no
-00012df0: 2060 776f 726b 5265 7175 6972 656d 656e   `workRequiremen
-00012e00: 7444 6174 6160 2069 6e20 7468 6520 544f  tData` in the TO
-00012e10: 4d4c 2066 696c 652c 206f 7220 602d 2d77  ML file, or `--w
-00012e20: 6f72 6b2d 7265 7175 6972 656d 656e 7460  ork-requirement`
-00012e30: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
-00012e40: 6c69 6e65 290a 322e 2049 6e73 6572 7420  line).2. Insert 
-00012e50: 7468 6520 7265 7175 6972 6564 2043 5356  the required CSV
-00012e60: 2d73 7570 706c 6965 6420 7661 7269 6162  -supplied variab
-00012e70: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
-00012e80: 2064 6972 6563 746c 7920 696e 746f 2074   directly into t
-00012e90: 6865 2054 4f4d 4c20 7072 6f70 6572 7469  he TOML properti
-00012ea0: 6573 2c20 652e 672e 2060 6172 6775 6d65  es, e.g. `argume
-00012eb0: 6e74 7320 3d20 5b22 7b7b 6172 675f 317d  nts = ["{{arg_1}
-00012ec0: 7d22 2c20 227b 7b61 7267 5f32 7d7d 225d  }", "{{arg_2}}"]
-00012ed0: 600a 332e 2053 7065 6369 6679 2061 2073  `.3. Specify a s
-00012ee0: 696e 676c 6520 4353 5620 6669 6c65 2069  ingle CSV file i
-00012ef0: 6e20 7468 6520 6063 7376 4669 6c65 7360  n the `csvFiles`
-00012f00: 2054 4f4d 4c20 7072 6f70 6572 7479 2c20   TOML property, 
-00012f10: 652e 672e 2060 6373 7646 696c 6573 203d  e.g. `csvFiles =
-00012f20: 205b 2277 725f 6461 7461 2e63 7376 225d   ["wr_data.csv"]
-00012f30: 602c 206f 7220 7072 6f76 6964 6520 7468  `, or provide th
-00012f40: 6520 4353 5620 6669 6c65 206f 6e20 7468  e CSV file on th
-00012f50: 6520 636f 6d6d 616e 6420 6c69 6e65 2060  e command line `
-00012f60: 2d56 2077 725f 6461 7461 2e63 7376 600a  -V wr_data.csv`.
-00012f70: 0a57 6865 6e20 6079 642d 7375 626d 6974  .When `yd-submit
-00012f80: 6020 6973 2072 756e 2c20 6974 2077 696c  ` is run, it wil
-00012f90: 6c20 6578 7061 6e64 2074 6865 2054 6173  l expand the Tas
-00012fa0: 6b20 6c69 7374 2074 6f20 6d61 7463 6820  k list to match 
-00012fb0: 7468 6520 6e75 6d62 6572 206f 6620 6461  the number of da
-00012fc0: 7461 2072 6f77 7320 696e 2074 6865 2043  ta rows in the C
-00012fd0: 5356 2066 696c 652e 0a0a 2323 2320 496e  SV file...### In
-00012fe0: 7370 6563 7469 6e67 2074 6865 2052 6573  specting the Res
-00012ff0: 756c 7473 206f 6620 4353 5620 5661 7269  ults of CSV Vari
-00013000: 6162 6c65 2053 7562 7374 6974 7574 696f  able Substitutio
-00013010: 6e0a 0a54 6865 2060 2d2d 7072 6f63 6573  n..The `--proces
-00013020: 732d 6373 762d 6f6e 6c79 6020 286f 7220  s-csv-only` (or 
-00013030: 602d 7060 2920 6f70 7469 6f6e 2063 616e  `-p`) option can
-00013040: 2062 6520 7573 6564 2077 6974 6820 6079   be used with `y
-00013050: 642d 7375 626d 6974 6020 746f 206f 7574  d-submit` to out
-00013060: 7075 7420 7468 6520 4a53 4f4e 2057 6f72  put the JSON Wor
-00013070: 6b20 5265 7175 6972 656d 656e 7420 6166  k Requirement af
-00013080: 7465 7220 4353 5620 7661 7269 6162 6c65  ter CSV variable
-00013090: 2073 7562 7374 6974 7574 696f 6e73 206f   substitutions o
-000130a0: 6e6c 792c 2070 7269 6f72 2074 6f20 616c  nly, prior to al
-000130b0: 6c20 6f74 6865 7220 7375 6273 7469 7475  l other substitu
-000130c0: 7469 6f6e 7320 616e 6420 7072 6f70 6572  tions and proper
-000130d0: 7479 2069 6e68 6572 6974 616e 6365 2061  ty inheritance a
-000130e0: 7070 6c69 6564 2062 7920 6079 642d 7375  pplied by `yd-su
-000130f0: 626d 6974 602e 0a0a 2320 576f 726b 6572  bmit`...# Worker
-00013100: 2050 6f6f 6c20 5072 6f70 6572 7469 6573   Pool Properties
-00013110: 0a0a 5468 6520 6077 6f72 6b65 7250 6f6f  ..The `workerPoo
-00013120: 6c60 2073 6563 7469 6f6e 206f 6620 7468  l` section of th
-00013130: 6520 544f 4d4c 2066 696c 6520 6465 6669  e TOML file defi
-00013140: 6e65 7320 7468 6520 7072 6f70 6572 7469  nes the properti
-00013150: 6573 206f 6620 7468 6520 576f 726b 6572  es of the Worker
-00013160: 2050 6f6f 6c20 746f 2062 6520 6372 6561   Pool to be crea
-00013170: 7465 642c 2061 6e64 2069 7320 7573 6564  ted, and is used
-00013180: 2062 7920 7468 6520 6079 642d 7072 6f76   by the `yd-prov
-00013190: 6973 696f 6e60 2063 6f6d 6d61 6e64 2e20  ision` command. 
-000131a0: 4120 7375 6273 6574 206f 6620 7468 6520  A subset of the 
-000131b0: 7072 6f70 6572 7469 6573 2069 7320 616c  properties is al
-000131c0: 736f 2075 7365 6420 6279 2074 6865 2060  so used by the `
-000131d0: 7964 2d69 6e73 7461 6e74 6961 7465 6020  yd-instantiate` 
-000131e0: 636f 6d6d 616e 642c 2066 6f72 2063 7265  command, for cre
-000131f0: 6174 696e 6720 7374 616e 6461 6c6f 6e65  ating standalone
-00013200: 2043 6f6d 7075 7465 2052 6571 7569 7265   Compute Require
-00013210: 6d65 6e74 7320 7468 6174 2061 7265 206e  ments that are n
-00013220: 6f74 2061 7373 6f63 6961 7465 6420 7769  ot associated wi
-00013230: 7468 2057 6f72 6b65 7220 506f 6f6c 732e  th Worker Pools.
-00013240: 0a0a 5468 6520 6f6e 6c79 206d 616e 6461  ..The only manda
-00013250: 746f 7279 2070 726f 7065 7274 7920 6973  tory property is
-00013260: 2060 7465 6d70 6c61 7465 4964 602e 2041   `templateId`. A
-00013270: 6c6c 206f 7468 6572 2070 726f 7065 7274  ll other propert
-00013280: 6965 7320 6861 7665 2064 6566 6175 6c74  ies have default
-00013290: 7320 286f 7220 6172 6520 6e6f 7420 7265  s (or are not re
-000132a0: 7175 6972 6564 292e 0a0a 5468 6520 666f  quired)...The fo
-000132b0: 6c6c 6f77 696e 6720 7072 6f70 6572 7469  llowing properti
-000132c0: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
-000132d0: 3a0a 0a7c 2050 726f 7065 7274 7920 2020  :..| Property   
-000132e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000132f0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 2020 2020 2020 2020 207c 2044 6566 6175           | Defau
-00013370: 6c74 2020 2020 2020 2020 2020 2020 2020  lt              
-00013380: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
-00013390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133a0: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
-000133b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
-00013420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013430: 2d2d 2d2d 2d7c 0a7c 2060 6964 6c65 4e6f  -----|.| `idleNo
-00013440: 6465 5368 7574 646f 776e 456e 6162 6c65  deShutdownEnable
-00013450: 6460 207c 2057 6865 7468 6572 2074 6f20  d` | Whether to 
-00013460: 7368 7574 2064 6f77 6e20 6e6f 6465 7320  shut down nodes 
-00013470: 7468 6174 2068 6176 6520 6265 656e 2069  that have been i
-00013480: 646c 6520 666f 7220 6069 646c 654e 6f64  dle for `idleNod
-00013490: 6553 6875 7464 6f77 6e54 696d 656f 7574  eShutdownTimeout
-000134a0: 6020 6d69 6e75 7465 732e 2020 2020 2020  ` minutes.      
-000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134c0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-000134d0: 5472 7565 6020 2020 2020 2020 2020 2020  True`           
-000134e0: 2020 2020 2020 207c 0a7c 2060 6964 6c65         |.| `idle
-000134f0: 4e6f 6465 5368 7574 646f 776e 5469 6d65  NodeShutdownTime
-00013500: 6f75 7460 207c 2054 6865 2074 696d 656f  out` | The timeo
-00013510: 7574 2069 6e20 6d69 6e75 7465 7320 6166  ut in minutes af
-00013520: 7465 7220 7768 6963 6820 616e 2069 646c  ter which an idl
-00013530: 6520 6e6f 6465 2077 696c 6c20 6265 2073  e node will be s
-00013540: 6875 7420 646f 776e 2069 6620 6069 646c  hut down if `idl
-00013550: 654e 6f64 6553 6875 7464 6f77 6e45 6e61  eNodeShutdownEna
-00013560: 626c 6564 6020 6973 2073 6574 2074 6f20  bled` is set to 
-00013570: 6054 7275 6560 2e20 2020 2020 2020 207c  `True`.        |
-00013580: 2060 352e 3060 2020 2020 2020 2020 2020   `5.0`          
-00013590: 2020 2020 2020 2020 207c 0a7c 2060 6964           |.| `id
-000135a0: 6c65 506f 6f6c 5368 7574 646f 776e 456e  lePoolShutdownEn
-000135b0: 6162 6c65 6460 207c 2057 6865 7468 6572  abled` | Whether
-000135c0: 2074 6f20 7368 7574 2064 6f77 6e20 7468   to shut down th
-000135d0: 6520 576f 726b 6572 2050 6f6f 6c20 7768  e Worker Pool wh
-000135e0: 656e 2069 7420 6861 7320 6265 656e 2069  en it has been i
-000135f0: 646c 6520 666f 7220 6069 646c 6550 6f6f  dle for `idlePoo
-00013600: 6c53 6875 7464 6f77 6e54 696d 656f 7574  lShutdownTimeout
-00013610: 6020 6d69 6e75 7465 732e 2020 2020 2020  ` minutes.      
-00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 207c 2060 5472 7565 6020 2020 2020 2020   | `True`       
-00013640: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-00013650: 6964 6c65 506f 6f6c 5368 7574 646f 776e  idlePoolShutdown
-00013660: 5469 6d65 6f75 7460 207c 2054 6865 2074  Timeout` | The t
-00013670: 696d 656f 7574 2069 6e20 6d69 6e75 7465  imeout in minute
-00013680: 7320 6166 7465 7220 7768 6963 6820 616e  s after which an
-00013690: 2069 646c 6520 576f 726b 6572 2050 6f6f   idle Worker Poo
-000136a0: 6c20 7769 6c6c 2062 6520 7368 7574 2064  l will be shut d
-000136b0: 6f77 6e20 6966 2060 6964 6c65 506f 6f6c  own if `idlePool
-000136c0: 5368 7574 646f 776e 456e 6162 6c65 6460  ShutdownEnabled`
-000136d0: 2069 7320 7365 7420 746f 2060 5472 7565   is set to `True
-000136e0: 602e 207c 2060 3330 2e30 6020 2020 2020  `. | `30.0`     
-000136f0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00013700: 2060 696d 6167 6573 4964 6020 2020 2020   `imagesId`     
-00013710: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00013720: 2069 6d61 6765 7320 4944 2074 6f20 7573   images ID to us
-00013730: 6520 7768 656e 2062 6f6f 7469 6e67 2069  e when booting i
-00013740: 6e73 7461 6e63 6573 2e20 2020 2020 2020  nstances.       
-00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013790: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000137a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000137b0: 0a7c 2060 696e 7374 616e 6365 5461 6773  .| `instanceTags
-000137c0: 6020 2020 2020 2020 2020 2020 207c 2054  `            | T
-000137d0: 6865 2064 6963 7469 6f6e 6172 7920 6f66  he dictionary of
-000137e0: 2069 6e73 7461 6e63 6520 7461 6773 2074   instance tags t
-000137f0: 6f20 6170 706c 7920 746f 2074 6865 2069  o apply to the i
-00013800: 6e73 7461 6e63 6573 2e20 2020 2020 2020  nstances.       
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00008690: 2059 6573 2020 7c20 2020 2020 7c20 2020   Yes  |     |   
+000086a0: 2020 207c 2059 6573 2020 7c0a 7c20 6074     | Yes  |.| `t
+000086b0: 6173 6b54 7970 6573 6020 2020 2020 2020  askTypes`       
+000086c0: 2020 2020 2020 2020 207c 2054 6865 206c           | The l
+000086d0: 6973 7420 6f66 2054 6173 6b20 5479 7065  ist of Task Type
+000086e0: 7320 7265 7175 6972 6564 2062 7920 7468  s required by th
+000086f0: 6520 7261 6e67 6520 6f66 2054 6173 6b73  e range of Tasks
+00008700: 2069 6e20 6120 5461 736b 2047 726f 7570   in a Task Group
+00008710: 2e20 452e 672e 2c20 605b 2264 6f63 6b65  . E.g., `["docke
+00008720: 7222 2c20 6261 7368 225d 602e 2020 2020  r", bash"]`.    
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2020 2020 7c20 2020 2020 207c 2059 6573      |      | Yes
+00008780: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
+00008790: 0a7c 2060 7461 736b 7350 6572 576f 726b  .| `tasksPerWork
+000087a0: 6572 6020 2020 2020 2020 2020 2020 7c20  er`           | 
+000087b0: 4465 7465 726d 696e 6573 2074 6865 206e  Determines the n
+000087c0: 756d 6265 7220 6f66 2057 6f72 6b65 7220  umber of Worker 
+000087d0: 636c 6169 6d73 2062 6173 6564 206f 6e20  claims based on 
+000087e0: 7370 6c69 7474 696e 6720 7468 6520 6e75  splitting the nu
+000087f0: 6d62 6572 206f 6620 756e 6669 6e69 7368  mber of unfinish
+00008800: 6564 2054 6173 6b73 2061 6372 6f73 7320  ed Tasks across 
+00008810: 576f 726b 6572 732e 2045 2e67 2e2c 2060  Workers. E.g., `
+00008820: 3160 2e20 2020 2020 2020 2020 2020 2020  1`.             
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008850: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+00008860: 7c20 5965 7320 7c20 5965 7320 207c 2020  | Yes | Yes  |  
+00008870: 2020 2020 7c0a 7c20 6075 706c 6f61 6446      |.| `uploadF
+00008880: 696c 6573 6020 2020 2020 2020 2020 2020  iles`           
+00008890: 2020 207c 2054 6865 206c 6973 7420 6f66     | The list of
+000088a0: 2066 696c 6573 2074 6f20 6265 2075 706c   files to be upl
+000088b0: 6f61 6465 6420 746f 2074 6865 2059 656c  oaded to the Yel
+000088c0: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
+000088d0: 6f72 652e 2045 2e67 2e2c 2028 4a53 4f4e  ore. E.g., (JSON
+000088e0: 293a 2060 5b7b 226c 6f63 616c 5061 7468  ): `[{"localPath
+000088f0: 223a 2066 696c 655f 312e 7478 7422 2c20  ": file_1.txt", 
+00008900: 2275 706c 6f61 6450 6174 6822 3a20 2266  "uploadPath": "f
+00008910: 696c 655f 312e 7478 7422 7d5d 602e 2020  ile_1.txt"}]`.  
+00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008930: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00008940: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
+00008950: 2020 7c20 5965 7320 207c 0a7c 2060 7663    | Yes  |.| `vc
+00008960: 7075 7360 2020 2020 2020 2020 2020 2020  pus`            
+00008970: 2020 2020 2020 2020 7c20 5261 6e67 6520          | Range 
+00008980: 636f 6e73 7472 6169 6e74 206f 6e20 6e75  constraint on nu
+00008990: 6d62 6572 206f 6620 7643 5055 7320 7468  mber of vCPUs th
+000089a0: 6174 2061 7265 2072 6571 7569 7265 6420  at are required 
+000089b0: 746f 2065 7865 6375 7465 2054 6173 6b73  to execute Tasks
+000089c0: 2045 2e67 2e2c 2060 5b32 2e30 2c20 342e   E.g., `[2.0, 4.
+000089d0: 305d 602e 2020 2020 2020 2020 2020 2020  0]`.            
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a20: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00008a30: 7c20 5965 7320 207c 2020 2020 2020 7c0a  | Yes  |      |.
+00008a40: 7c20 6076 6572 6966 7941 7453 7461 7274  | `verifyAtStart
+00008a50: 6020 2020 2020 2020 2020 2020 207c 2041  `            | A
+00008a60: 206c 6973 7420 6f66 2066 696c 6573 2072   list of files r
+00008a70: 6571 7569 7265 6420 6279 2061 2054 6173  equired by a Tas
+00008a80: 6b2e 204d 7573 7420 6265 2070 7265 7365  k. Must be prese
+00008a90: 6e74 2077 6865 6e20 7468 6520 5461 736b  nt when the Task
+00008aa0: 2069 7320 7265 6164 7920 746f 2073 7461   is ready to sta
+00008ab0: 7274 206f 7220 7468 6520 5461 736b 2077  rt or the Task w
+00008ac0: 696c 6c20 6661 696c 2e20 452e 672e 3a20  ill fail. E.g.: 
+00008ad0: 605b 2274 6173 6b5f 6772 6f75 705f 312f  `["task_group_1/
+00008ae0: 7461 736b 5f31 2f72 6573 756c 7473 2e74  task_1/results.t
+00008af0: 7874 225d 602e 2020 2020 2020 2020 2020  xt"]`.          
+00008b00: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00008b10: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+00008b20: 7320 207c 0a7c 2060 7665 7269 6679 5761  s  |.| `verifyWa
+00008b30: 6974 6020 2020 2020 2020 2020 2020 2020  it`             
+00008b40: 2020 7c20 4120 6c69 7374 206f 6620 6669    | A list of fi
+00008b50: 6c65 7320 7265 7175 6972 6564 2062 7920  les required by 
+00008b60: 6120 5461 736b 2e20 5468 6520 5461 736b  a Task. The Task
+00008b70: 2077 696c 6c20 7761 6974 2075 6e74 696c   will wait until
+00008b80: 2074 6865 2066 696c 6573 2061 7265 2061   the files are a
+00008b90: 7661 696c 6162 6c65 2062 6566 6f72 6520  vailable before 
+00008ba0: 7374 6172 7469 6e67 2e20 452e 672e 3a20  starting. E.g.: 
+00008bb0: 605b 2274 6173 6b5f 6772 6f75 705f 312f  `["task_group_1/
+00008bc0: 7461 736b 5f31 2f72 6573 756c 7473 2e74  task_1/results.t
+00008bd0: 7874 225d 602e 2020 2020 2020 2020 2020  xt"]`.          
+00008be0: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+00008bf0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+00008c00: 207c 2059 6573 2020 7c0a 7c20 6077 6f72   | Yes  |.| `wor
+00008c10: 6b65 7254 6167 7360 2020 2020 2020 2020  kerTags`        
+00008c20: 2020 2020 2020 207c 2054 6865 206c 6973         | The lis
+00008c30: 7420 6f66 2057 6f72 6b65 7220 5461 6773  t of Worker Tags
+00008c40: 2074 6861 7420 7769 6c6c 2062 6520 7573   that will be us
+00008c50: 6564 2074 6f20 6d61 7463 6820 6167 6169  ed to match agai
+00008c60: 6e73 7420 7468 6520 576f 726b 6572 2054  nst the Worker T
+00008c70: 6167 206f 6620 6120 6361 6e64 6964 6174  ag of a candidat
+00008c80: 6520 576f 726b 6572 2e20 452e 672e 2c20  e Worker. E.g., 
+00008c90: 605b 2274 6167 5f78 222c 2022 7461 675f  `["tag_x", "tag_
+00008ca0: 7922 5d60 2e20 2020 2020 2020 2020 2020  y"]`.           
+00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cd0: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00008ce0: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
+00008cf0: 2060 776f 726b 5265 7175 6972 656d 656e   `workRequiremen
+00008d00: 7444 6174 6160 2020 2020 2020 7c20 5468  tData`      | Th
+00008d10: 6520 6e61 6d65 206f 6620 7468 6520 6669  e name of the fi
+00008d20: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
+00008d30: 6520 4a53 4f4e 2064 6f63 756d 656e 7420  e JSON document 
+00008d40: 696e 2077 6869 6368 2074 6865 2057 6f72  in which the Wor
+00008d50: 6b20 5265 7175 6972 656d 656e 7420 6973  k Requirement is
+00008d60: 2064 6566 696e 6564 2e20 452e 672e 2c20   defined. E.g., 
+00008d70: 6022 7465 7374 5f77 6f72 6b72 6571 2e6a  `"test_workreq.j
+00008d80: 736f 6e22 602e 2020 2020 2020 2020 2020  son"`.          
+00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00008dc0: 2020 2020 7c20 2020 2020 207c 2020 2020      |      |    
+00008dd0: 2020 7c0a 0a23 2320 4175 746f 6d61 7469    |..## Automati
+00008de0: 6320 5072 6f70 6572 7469 6573 0a0a 496e  c Properties..In
+00008df0: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
+00008e00: 2069 6e68 6572 6974 616e 6365 206d 6563   inheritance mec
+00008e10: 6861 6e69 736d 2c20 736f 6d65 2070 726f  hanism, some pro
+00008e20: 7065 7274 6965 7320 6172 6520 7365 7420  perties are set 
+00008e30: 6175 746f 6d61 7469 6361 6c6c 7920 6279  automatically by
+00008e40: 2074 6865 2060 7964 2d73 7562 6d69 7460   the `yd-submit`
+00008e50: 2063 6f6d 6d61 6e64 2c20 6173 2061 2075   command, as a u
+00008e60: 7361 6765 2063 6f6e 7665 6e69 656e 6365  sage convenience
+00008e70: 2069 6620 7468 6579 2772 6520 6e6f 7420   if they're not 
+00008e80: 6578 706c 6963 6974 6c79 2070 726f 7669  explicitly provi
+00008e90: 6465 642e 0a0a 2323 2320 576f 726b 2052  ded...### Work R
+00008ea0: 6571 7569 7265 6d65 6e74 2c20 5461 736b  equirement, Task
+00008eb0: 2047 726f 7570 2061 6e64 2054 6173 6b20   Group and Task 
+00008ec0: 4e61 6d69 6e67 0a0a 2d20 5468 6520 2a2a  Naming..- The **
+00008ed0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00008ee0: 2a2a 206e 616d 6520 6973 2061 7574 6f6d  ** name is autom
+00008ef0: 6174 6963 616c 6c79 2073 6574 2075 7369  atically set usi
+00008f00: 6e67 2061 2063 6f6e 6361 7465 6e61 7469  ng a concatenati
+00008f10: 6f6e 206f 6620 7468 6520 6074 6167 6020  on of the `tag` 
+00008f20: 7072 6f70 6572 7479 2c20 6120 5554 4320  property, a UTC 
+00008f30: 7469 6d65 7374 616d 702c 2061 6e64 2074  timestamp, and t
+00008f40: 6872 6565 2072 616e 646f 6d20 6865 7820  hree random hex 
+00008f50: 6368 6172 6163 7465 7273 3a20 652c 672c  characters: e,g,
+00008f60: 2e20 606d 7974 6167 5f32 3231 3032 342d  . `mytag_221024-
+00008f70: 3135 3535 3234 2d34 3061 602e 0a2d 202a  155524-40a`..- *
+00008f80: 2a54 6173 6b20 4772 6f75 702a 2a20 6e61  *Task Group** na
+00008f90: 6d65 7320 6172 6520 6175 746f 6d61 7469  mes are automati
+00008fa0: 6361 6c6c 7920 6372 6561 7465 6420 666f  cally created fo
+00008fb0: 7220 616e 7920 5461 736b 2047 726f 7570  r any Task Group
+00008fc0: 2074 6861 7420 6973 206e 6f74 2065 7870   that is not exp
+00008fd0: 6c69 6369 746c 7920 6e61 6d65 642c 2075  licitly named, u
+00008fe0: 7369 6e67 206e 616d 6573 206f 6620 7468  sing names of th
+00008ff0: 6520 666f 726d 2060 7461 736b 5f67 726f  e form `task_gro
+00009000: 7570 5f31 6020 286f 7220 6074 6173 6b5f  up_1` (or `task_
+00009010: 6772 6f75 705f 3031 602c 2065 7463 2e2c  group_01`, etc.,
+00009020: 2066 6f72 206c 6172 6765 7220 6e75 6d62   for larger numb
+00009030: 6572 7320 6f66 2054 6173 6b20 4772 6f75  ers of Task Grou
+00009040: 7073 292e 2054 6173 6b20 4772 6f75 7020  ps). Task Group 
+00009050: 6e75 6d62 6572 7320 6361 6e20 616c 736f  numbers can also
+00009060: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
+00009070: 7573 6572 2d64 6566 696e 6564 2054 6173  user-defined Tas
+00009080: 6b20 4772 6f75 7020 6e61 6d65 7320 7573  k Group names us
+00009090: 696e 6720 7468 6520 607b 7b74 6173 6b5f  ing the `{{task_
+000090a0: 6772 6f75 705f 6e75 6d62 6572 7d7d 6020  group_number}}` 
+000090b0: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+000090c0: 7574 696f 6e20 6469 7363 7573 7365 6420  ution discussed 
+000090d0: 6265 6c6f 772e 0a2d 202a 2a54 6173 6b2a  below..- **Task*
+000090e0: 2a20 6e61 6d65 7320 6172 6520 6175 746f  * names are auto
+000090f0: 6d61 7469 6361 6c6c 7920 6372 6561 7465  matically create
+00009100: 6420 666f 7220 616e 7920 5461 736b 2074  d for any Task t
+00009110: 6861 7420 6973 206e 6f74 2065 7870 6c69  hat is not expli
+00009120: 6369 746c 7920 6e61 6d65 642c 2075 7369  citly named, usi
+00009130: 6e67 206e 616d 6573 206f 6620 7468 6520  ng names of the 
+00009140: 666f 726d 2060 7461 736b 5f31 6020 286f  form `task_1` (o
+00009150: 7220 6074 6173 6b5f 3031 602c 2065 7463  r `task_01`, etc
+00009160: 2e2c 2066 6f72 206c 6172 6765 7220 6e75  ., for larger nu
+00009170: 6d62 6572 7320 6f66 2054 6173 6b73 292e  mbers of Tasks).
+00009180: 2054 6865 2054 6173 6b20 636f 756e 7465   The Task counte
+00009190: 7220 7265 7365 7473 2066 6f72 2065 6163  r resets for eac
+000091a0: 6820 6469 6666 6572 656e 7420 5461 736b  h different Task
+000091b0: 2047 726f 7570 2e20 5461 736b 206e 756d   Group. Task num
+000091c0: 6265 7273 2063 616e 2061 6c73 6f20 6265  bers can also be
+000091d0: 2069 6e63 6c75 6465 6420 696e 2075 7365   included in use
+000091e0: 722d 6465 6669 6e65 6420 5461 736b 206e  r-defined Task n
+000091f0: 616d 6573 2075 7369 6e67 2074 6865 2060  ames using the `
+00009200: 7b7b 7461 736b 5f6e 756d 6265 727d 7d60  {{task_number}}`
+00009210: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+00009220: 7475 7469 6f6e 2064 6973 6375 7373 6564  tution discussed
+00009230: 2062 656c 6f77 2e0a 0a23 2323 2054 6173   below...### Tas
+00009240: 6b20 5479 7065 730a 0a2d 2049 6620 6074  k Types..- If `t
+00009250: 6173 6b54 7970 6560 2069 7320 7365 7420  askType` is set 
+00009260: 6f6e 6c79 2061 7420 7468 6520 544f 4d4c  only at the TOML
+00009270: 2066 696c 6520 6c65 7665 6c2c 2074 6865   file level, the
+00009280: 6e20 6074 6173 6b54 7970 6573 6020 6973  n `taskTypes` is
+00009290: 2061 7574 6f6d 6174 6963 616c 6c79 2070   automatically p
+000092a0: 6f70 756c 6174 6564 2066 6f72 2054 6173  opulated for Tas
+000092b0: 6b20 4772 6f75 7073 2c20 756e 6c65 7373  k Groups, unless
+000092c0: 206f 7665 7272 6964 6465 6e2e 0a2d 2049   overridden..- I
+000092d0: 6620 6074 6173 6b54 7970 6560 2069 7320  f `taskType` is 
+000092e0: 7365 7420 6174 2074 6865 2054 6173 6b20  set at the Task 
+000092f0: 6c65 7665 6c2c 2074 6865 6e20 6074 6173  level, then `tas
+00009300: 6b54 7970 6573 6020 6973 2061 7574 6f6d  kTypes` is autom
+00009310: 6174 6963 616c 6c79 2070 6f70 756c 6174  atically populat
+00009320: 6564 2066 6f72 2074 6865 2054 6173 6b20  ed for the Task 
+00009330: 4772 6f75 7073 206c 6576 656c 2075 7369  Groups level usi
+00009340: 6e67 2074 6865 2061 6363 756d 756c 6174  ng the accumulat
+00009350: 6564 2054 6173 6b20 5479 7065 7320 6672  ed Task Types fr
+00009360: 6f6d 2074 6865 2054 6173 6b73 2069 6e63  om the Tasks inc
+00009370: 6c75 6465 6420 696e 2065 6163 6820 5461  luded in each Ta
+00009380: 736b 2047 726f 7570 2c20 756e 6c65 7373  sk Group, unless
+00009390: 206f 7665 7272 6964 6465 6e2e 0a2d 2049   overridden..- I
+000093a0: 6620 6074 6173 6b54 7970 6573 6020 6973  f `taskTypes` is
+000093b0: 2073 6574 2061 7420 7468 6520 5461 736b   set at the Task
+000093c0: 2047 726f 7570 204c 6576 656c 2c20 616e   Group Level, an
+000093d0: 6420 6861 7320 6f6e 6c79 206f 6e65 2054  d has only one T
+000093e0: 6173 6b20 5479 7065 2065 6e74 7279 2c20  ask Type entry, 
+000093f0: 7468 656e 2060 7461 736b 5479 7065 6020  then `taskType` 
+00009400: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+00009410: 2073 6574 2061 7420 7468 6520 5461 736b   set at the Task
+00009420: 204c 6576 656c 2075 7369 6e67 2074 6865   Level using the
+00009430: 2073 696e 676c 6520 5461 736b 2054 7970   single Task Typ
+00009440: 652c 2075 6e6c 6573 7320 6f76 6572 7269  e, unless overri
+00009450: 6464 656e 2e0a 0a46 6f72 2074 6865 202a  dden...For the *
+00009460: 2a60 6261 7368 602a 2a2c 202a 2a60 706f  *`bash`**, **`po
+00009470: 7765 7273 6865 6c6c 602a 2a2c 202a 2a60  wershell`**, **`
+00009480: 636d 6460 2a2a 2f2a 2a60 6261 7460 2a2a  cmd`**/**`bat`**
+00009490: 2061 6e64 202a 2a60 646f 636b 6572 602a   and **`docker`*
+000094a0: 2a20 7461 736b 2074 7970 6573 2c20 736f  * task types, so
+000094b0: 6d65 2061 7574 6f6d 6174 6963 2070 726f  me automatic pro
+000094c0: 6365 7373 696e 6720 7769 6c6c 2062 6520  cessing will be 
+000094d0: 7065 7266 6f72 6d65 6420 6966 2074 6865  performed if the
+000094e0: 202a 2a60 6578 6563 7574 6162 6c65 602a   **`executable`*
+000094f0: 2a20 7072 6f70 6572 7479 2069 7320 7365  * property is se
+00009500: 742e 0a0a 2323 2323 2042 6173 682c 2050  t...#### Bash, P
+00009510: 7974 686f 6e2c 2050 6f77 6572 5368 656c  ython, PowerShel
+00009520: 6c20 616e 6420 636d 642f 6261 7420 5461  l and cmd/bat Ta
+00009530: 736b 730a 0a41 7320 6120 636f 6e76 656e  sks..As a conven
+00009540: 6965 6e63 652c 2066 6f72 2074 6865 202a  ience, for the *
+00009550: 2a60 6261 7368 602a 2a2c 202a 2a60 7079  *`bash`**, **`py
+00009560: 7468 6f6e 602a 2a2c 202a 2a60 706f 7765  thon`**, **`powe
+00009570: 7273 6865 6c6c 602a 2a2c 2061 6e64 202a  rshell`**, and *
+00009580: 2a60 636d 6460 2a2a 2028 6f72 202a 2a60  *`cmd`** (or **`
+00009590: 6261 7460 2a2a 2920 5461 736b 2054 7970  bat`**) Task Typ
+000095a0: 6573 2c20 7468 6520 7363 7269 7074 206e  es, the script n
+000095b0: 6f6d 696e 6174 6564 2069 6e20 7468 6520  ominated in the 
+000095c0: 2a2a 6065 7865 6375 7461 626c 6560 2a2a  **`executable`**
+000095d0: 2070 726f 7065 7274 7920 6973 2061 7574   property is aut
+000095e0: 6f6d 6174 6963 616c 6c79 2061 6464 6564  omatically added
+000095f0: 2074 6f20 7468 6520 6069 6e70 7574 7360   to the `inputs`
+00009600: 206c 6973 7420 2869 6620 6e6f 7420 616c   list (if not al
+00009610: 7265 6164 7920 7072 6573 656e 7429 2e20  ready present). 
+00009620: 5468 6973 206d 6561 6e73 2074 6865 2073  This means the s
+00009630: 6372 6970 7420 6669 6c65 2077 696c 6c20  cript file will 
+00009640: 6265 2075 706c 6f61 6465 6420 746f 2074  be uploaded to t
+00009650: 6865 204f 626a 6563 7420 5374 6f72 652c  he Object Store,
+00009660: 2061 6e64 206d 6164 6520 6120 7265 7175   and made a requ
+00009670: 6972 656d 656e 7420 6f66 2074 6865 2054  irement of the T
+00009680: 6173 6b20 7768 656e 2069 7420 7275 6e73  ask when it runs
+00009690: 2e0a 0a55 7369 6e67 2061 2042 6173 6820  ...Using a Bash 
+000096a0: 5461 736b 2061 7320 616e 2065 7861 6d70  Task as an examp
+000096b0: 6c65 2028 696e 2054 4f4d 4c20 666f 726d  le (in TOML form
+000096c0: 293a 0a0a 6060 6074 6f6d 6c0a 7461 736b  ):..```toml.task
+000096d0: 5479 7065 203d 2022 6261 7368 220a 6578  Type = "bash".ex
+000096e0: 6563 7574 6162 6c65 203d 2022 6d79 5f62  ecutable = "my_b
+000096f0: 6173 685f 7363 7269 7074 2e73 6822 0a61  ash_script.sh".a
+00009700: 7267 756d 656e 7473 203d 205b 2231 222c  rguments = ["1",
+00009710: 2022 3222 2c20 2233 225d 0a60 6060 0a69   "2", "3"].```.i
+00009720: 7320 6571 7569 7661 6c65 6e74 2074 6f3a  s equivalent to:
+00009730: 0a0a 6060 6074 6f6d 6c0a 7461 736b 5479  ..```toml.taskTy
+00009740: 7065 203d 2022 6261 7368 220a 696e 7075  pe = "bash".inpu
+00009750: 7473 203d 205b 226d 795f 6261 7368 5f73  ts = ["my_bash_s
+00009760: 6372 6970 742e 7368 225d 0a61 7267 756d  cript.sh"].argum
+00009770: 656e 7473 203d 205b 227b 7b77 725f 6e61  ents = ["{{wr_na
+00009780: 6d65 7d7d 2f6d 795f 6261 7368 5f73 6372  me}}/my_bash_scr
+00009790: 6970 742e 7368 222c 2022 3122 2c20 2232  ipt.sh", "1", "2
+000097a0: 222c 2022 3322 5d0a 6060 600a 0a49 6e20  ", "3"].```..In 
+000097b0: 7468 6520 6361 7365 206f 6620 5769 6e64  the case of Wind
+000097c0: 6f77 7320 6261 7463 6820 2860 2e62 6174  ows batch (`.bat
+000097d0: 6029 2066 696c 6573 2c20 6120 602f 6360  `) files, a `/c`
+000097e0: 2066 6c61 6720 6973 2070 7265 7065 6e64   flag is prepend
+000097f0: 6564 2074 6f20 7468 6520 6063 6d64 2e65  ed to the `cmd.e
+00009800: 7865 6020 6172 6775 6d65 6e74 206c 6973  xe` argument lis
+00009810: 7420 746f 2065 6e73 7572 6520 636f 7272  t to ensure corr
+00009820: 6563 7420 6578 6563 7574 696f 6e20 6261  ect execution ba
+00009830: 6861 7669 6f75 722e 2046 6f72 2065 7861  haviour. For exa
+00009840: 6d70 6c65 3a0a 0a60 6060 746f 6d6c 0a74  mple:..```toml.t
+00009850: 6173 6b54 7970 6520 3d20 2263 6d64 2220  askType = "cmd" 
+00009860: 2023 206f 7220 2262 6174 220a 6578 6563   # or "bat".exec
+00009870: 7574 6162 6c65 203d 2022 6d79 5f73 6372  utable = "my_scr
+00009880: 6970 742e 6261 7422 0a61 7267 756d 656e  ipt.bat".argumen
+00009890: 7473 203d 205b 2231 222c 2022 3222 2c20  ts = ["1", "2", 
+000098a0: 2233 225d 0a60 6060 0a0a 6973 2065 7175  "3"].```..is equ
+000098b0: 6976 616c 656e 7420 746f 3a0a 0a60 6060  ivalent to:..```
+000098c0: 746f 6d6c 0a74 6173 6b54 7970 6520 3d20  toml.taskType = 
+000098d0: 2263 6d64 2220 2023 206f 7220 2262 6174  "cmd"  # or "bat
+000098e0: 220a 696e 7075 7473 203d 205b 226d 795f  ".inputs = ["my_
+000098f0: 7363 7269 7074 2e62 6174 225d 0a61 7267  script.bat"].arg
+00009900: 756d 656e 7473 203d 205b 222f 6322 2c20  uments = ["/c", 
+00009910: 227b 7b77 725f 6e61 6d65 7d7d 5c5c 6d79  "{{wr_name}}\\my
+00009920: 5f73 6372 6970 742e 6261 7422 2c20 2231  _script.bat", "1
+00009930: 222c 2022 3222 2c20 2233 225d 0a60 6060  ", "2", "3"].```
+00009940: 0a0a 4e6f 7465 2074 6865 2060 5c5c 6020  ..Note the `\\` 
+00009950: 7265 7175 6972 656d 656e 7420 666f 7220  requirement for 
+00009960: 6469 7265 6374 6f72 7920 7365 7061 7261  directory separa
+00009970: 746f 7273 2077 6865 6e20 6465 6669 6e69  tors when defini
+00009980: 6e67 2054 6173 6b73 206f 6e20 5769 6e64  ng Tasks on Wind
+00009990: 6f77 7320 686f 7374 732e 204e 6f74 6520  ows hosts. Note 
+000099a0: 616c 736f 2074 6861 7420 7468 6520 602f  also that the `/
+000099b0: 6360 2069 7320 7265 7175 6972 6564 2077  c` is required w
+000099c0: 6865 6e20 7275 6e6e 696e 6720 636f 6d6d  hen running comm
+000099d0: 616e 6473 206f 7220 6261 7463 6820 7363  ands or batch sc
+000099e0: 7269 7074 7320 7573 696e 6720 6063 6d64  ripts using `cmd
+000099f0: 2e65 7865 602c 206f 7468 6572 7769 7365  .exe`, otherwise
+00009a00: 2074 6865 2060 636d 642e 6578 6560 2070   the `cmd.exe` p
+00009a10: 726f 6365 7373 2063 7265 6174 6564 2074  rocess created t
+00009a20: 6f20 6578 6563 7574 6520 7468 6520 5461  o execute the Ta
+00009a30: 736b 2077 696c 6c20 6e6f 7420 7465 726d  sk will not term
+00009a40: 696e 6174 652e 0a0a 2323 2323 2044 6f63  inate...#### Doc
+00009a50: 6b65 7220 5461 736b 730a 0a46 6f72 2074  ker Tasks..For t
+00009a60: 6865 202a 2a60 646f 636b 6572 602a 2a20  he **`docker`** 
+00009a70: 5461 736b 2054 7970 652c 2074 6865 2076  Task Type, the v
+00009a80: 6172 6961 626c 6573 2073 7570 706c 6965  ariables supplie
+00009a90: 6420 696e 2074 6865 2060 646f 636b 6572  d in the `docker
+00009aa0: 456e 7669 726f 6e6d 656e 7460 2070 726f  Environment` pro
+00009ab0: 7065 7274 7920 6172 6520 756e 7061 636b  perty are unpack
+00009ac0: 6564 2069 6e74 6f20 7468 6520 6172 6775  ed into the argu
+00009ad0: 6d65 6e74 206c 6973 7420 6173 2060 2d2d  ment list as `--
+00009ae0: 656e 7660 2065 6e74 7269 6573 2c20 7468  env` entries, th
+00009af0: 6520 446f 636b 6572 2063 6f6e 7461 696e  e Docker contain
+00009b00: 6572 206e 616d 6520 7375 7070 6c69 6564  er name supplied
+00009b10: 2069 6e20 7468 6520 6065 7865 6375 7461   in the `executa
+00009b20: 626c 6560 2070 726f 7065 7274 7920 6973  ble` property is
+00009b30: 2074 6865 6e20 6164 6465 6420 746f 2074   then added to t
+00009b40: 6865 2061 7267 756d 656e 7473 206c 6973  he arguments lis
+00009b50: 742c 2066 6f6c 6c6f 7765 6420 6279 2074  t, followed by t
+00009b60: 6865 2061 7267 756d 656e 7473 2073 7570  he arguments sup
+00009b70: 706c 6965 6420 696e 2074 6865 2060 6172  plied in the `ar
+00009b80: 6775 6d65 6e74 7360 2070 726f 7065 7274  guments` propert
+00009b90: 792e 2054 6865 2060 646f 636b 6572 5573  y. The `dockerUs
+00009ba0: 6572 6e61 6d65 6020 616e 6420 6064 6f63  ername` and `doc
+00009bb0: 6b65 7250 6173 7377 6f72 6460 2070 726f  kerPassword` pro
+00009bc0: 7065 7274 6965 732c 2069 6620 7375 7070  perties, if supp
+00009bd0: 6c69 6564 2c20 6172 6520 6164 6465 6420  lied, are added 
+00009be0: 746f 2074 6865 2060 656e 7669 726f 6e6d  to the `environm
+00009bf0: 656e 7460 2070 726f 7065 7274 792e 0a0a  ent` property...
+00009c00: 466f 7220 6578 616d 706c 653a 0a60 6060  For example:.```
+00009c10: 746f 6d6c 0a74 6173 6b54 7970 6520 3d20  toml.taskType = 
+00009c20: 2264 6f63 6b65 7222 0a65 7865 6375 7461  "docker".executa
+00009c30: 626c 6520 3d20 226d 795f 646f 636b 6572  ble = "my_docker
+00009c40: 6875 625f 7265 706f 2f6d 795f 636f 6e74  hub_repo/my_cont
+00009c50: 6169 6e65 725f 696d 6167 6522 0a64 6f63  ainer_image".doc
+00009c60: 6b65 7245 6e76 6972 6f6e 6d65 6e74 203d  kerEnvironment =
+00009c70: 207b 4531 203d 2022 4565 654f 6e65 227d   {E1 = "EeeOne"}
+00009c80: 0a64 6f63 6b65 7255 7365 726e 616d 6520  .dockerUsername 
+00009c90: 3d20 226d 795f 7573 6572 220a 646f 636b  = "my_user".dock
+00009ca0: 6572 5061 7373 776f 7264 203d 2022 6d79  erPassword = "my
+00009cb0: 5f70 6173 7377 6f72 6422 0a61 7267 756d  _password".argum
+00009cc0: 656e 7473 203d 205b 2231 222c 2022 3222  ents = ["1", "2"
+00009cd0: 2c20 2233 225d 0a60 6060 0a0a 6973 2065  , "3"].```..is e
+00009ce0: 7175 6976 616c 656e 7420 746f 2074 6865  quivalent to the
+00009cf0: 2066 6f6c 6c6f 7769 6e67 2062 6569 6e67   following being
+00009d00: 2073 656e 7420 666f 7220 7072 6f63 6573   sent for proces
+00009d10: 7369 6e67 2062 7920 7468 6520 6064 6f63  sing by the `doc
+00009d20: 6b65 7260 2054 6173 6b20 5479 7065 2c20  ker` Task Type, 
+00009d30: 7468 6520 5965 6c6c 6f77 446f 6720 7665  the YellowDog ve
+00009d40: 7273 696f 6e20 6f66 2077 6869 6368 2077  rsion of which w
+00009d50: 696c 6c20 6c6f 6720 696e 2074 6f20 7468  ill log in to th
+00009d60: 6520 446f 636b 6572 2072 6570 6f20 2869  e Docker repo (i
+00009d70: 6620 7265 7175 6972 6564 2920 7468 656e  f required) then
+00009d80: 2069 7373 7565 2061 2060 646f 636b 6572   issue a `docker
+00009d90: 2072 756e 6020 636f 6d6d 616e 6420 7769   run` command wi
+00009da0: 7468 2074 6865 2061 7267 756d 656e 7473  th the arguments
+00009db0: 2073 7570 706c 6965 643a 0a0a 6060 6074   supplied:..```t
+00009dc0: 6f6d 6c0a 7461 736b 5479 7065 203d 2022  oml.taskType = "
+00009dd0: 646f 636b 6572 220a 6172 6775 6d65 6e74  docker".argument
+00009de0: 7320 3d20 5b22 2d2d 656e 7620 4531 3d45  s = ["--env E1=E
+00009df0: 6565 4f6e 6522 2c20 226d 795f 646f 636b  eeOne", "my_dock
+00009e00: 6572 6875 6272 6570 6f2f 6d79 5f63 6f6e  erhubrepo/my_con
+00009e10: 7461 696e 6572 5f69 6d61 6765 222c 2022  tainer_image", "
+00009e20: 3122 2c20 2232 222c 2022 3322 5d0a 656e  1", "2", "3"].en
+00009e30: 7669 726f 6e6d 656e 7420 3d20 7b44 4f43  vironment = {DOC
+00009e40: 4b45 525f 5553 4552 4e41 4d45 203d 2022  KER_USERNAME = "
+00009e50: 6d79 5f75 7365 7222 2c20 444f 434b 4552  my_user", DOCKER
+00009e60: 5f50 4153 5357 4f52 4420 3d20 226d 795f  _PASSWORD = "my_
+00009e70: 7061 7373 776f 7264 227d 0a60 6060 0a0a  password"}.```..
+00009e80: 2323 2323 2042 6173 682c 2050 7974 686f  #### Bash, Pytho
+00009e90: 6e2c 2050 6f77 6572 5368 656c 6c2c 2063  n, PowerShell, c
+00009ea0: 6d64 2e65 7865 2f62 6174 6368 2c20 616e  md.exe/batch, an
+00009eb0: 6420 446f 636b 6572 2077 6974 686f 7574  d Docker without
+00009ec0: 2041 7574 6f6d 6174 6963 2050 726f 6365   Automatic Proce
+00009ed0: 7373 696e 670a 0a49 6620 7468 6520 6065  ssing..If the `e
+00009ee0: 7865 6375 7461 626c 6560 2070 726f 7065  xecutable` prope
+00009ef0: 7274 7920 6973 206e 6f74 2073 7570 706c  rty is not suppl
+00009f00: 6965 642c 2074 6865 2061 7574 6f6d 6174  ied, the automat
+00009f10: 6963 2070 726f 6365 7373 696e 6720 6465  ic processing de
+00009f20: 7363 7269 6265 6420 6162 6f76 6520 666f  scribed above fo
+00009f30: 7220 6062 6173 6860 2c20 6070 7974 686f  r `bash`, `pytho
+00009f40: 6e60 2c20 6070 6f77 6572 7368 656c 6c60  n`, `powershell`
+00009f50: 2c20 6063 6d64 6020 286f 7220 6062 6174  , `cmd` (or `bat
+00009f60: 6029 2061 6e64 2060 646f 636b 6572 6020  `) and `docker` 
+00009f70: 7461 736b 2074 7970 6573 2069 7320 6e6f  task types is no
+00009f80: 7420 6170 706c 6965 642e 0a0a 2323 2320  t applied...### 
+00009f90: 5461 736b 2043 6f75 6e74 730a 0a54 6869  Task Counts..Thi
+00009fa0: 7320 7072 6f70 6572 7479 2077 696c 6c20  s property will 
+00009fb0: 6578 7061 6e64 2074 6865 206e 756d 6265  expand the numbe
+00009fc0: 7220 6f66 2054 6173 6b73 2074 6f20 6d61  r of Tasks to ma
+00009fd0: 7463 6820 6074 6173 6b43 6f75 6e74 602e  tch `taskCount`.
+00009fe0: 0a0a 5468 6520 6074 6173 6b43 6f75 6e74  ..The `taskCount
+00009ff0: 6020 7072 6f70 6572 7479 2063 616e 2062  ` property can b
+0000a000: 6520 7365 7420 6f6e 6c79 2069 6e20 7468  e set only in th
+0000a010: 6520 6077 6f72 6b52 6571 7569 7265 6d65  e `workRequireme
+0000a020: 6e74 6020 7365 6374 696f 6e20 6f66 2074  nt` section of t
+0000a030: 6865 2060 636f 6e66 6967 2e74 6f6d 6c60  he `config.toml`
+0000a040: 2066 696c 652c 206f 7220 696e 2074 6865   file, or in the
+0000a050: 2060 7461 736b 4772 6f75 7060 2073 6563   `taskGroup` sec
+0000a060: 7469 6f6e 2873 2920 6f66 2061 204a 534f  tion(s) of a JSO
+0000a070: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
+0000a080: 6e74 2064 6566 696e 6974 696f 6e2e 0a0a  nt definition...
+0000a090: 496e 2074 6865 2066 6f72 6d65 7220 6361  In the former ca
+0000a0a0: 7365 2c20 7468 6520 6074 6173 6b43 6f75  se, the `taskCou
+0000a0b0: 6e74 6020 6170 706c 6965 7320 6f6e 6c79  nt` applies only
+0000a0c0: 2074 6f20 7468 6520 5461 736b 2073 7065   to the Task spe
+0000a0d0: 6369 6669 6564 2077 6974 6869 6e20 7468  cified within th
+0000a0e0: 6520 6063 6f6e 6669 672e 746f 6d6c 6020  e `config.toml` 
+0000a0f0: 6669 6c65 2061 6e64 2069 7320 6e6f 7420  file and is not 
+0000a100: 696e 6865 7269 7465 6420 6279 204a 534f  inherited by JSO
+0000a110: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
+0000a120: 6e74 2073 7065 6369 6669 6361 7469 6f6e  nt specification
+0000a130: 732e 0a0a 496e 2074 6865 206c 6174 7465  s...In the latte
+0000a140: 7220 6361 7365 2c20 7468 6520 6074 6173  r case, the `tas
+0000a150: 6b43 6f75 6e74 6020 6170 706c 6965 7320  kCount` applies 
+0000a160: 746f 2074 6865 2054 6173 6b20 7370 6563  to the Task spec
+0000a170: 6966 6965 6420 7769 7468 696e 2074 6865  ified within the
+0000a180: 2054 6173 6b20 4772 6f75 702c 2061 6e64   Task Group, and
+0000a190: 2074 6865 7265 206d 7573 7420 6265 207a   there must be z
+0000a1a0: 6572 6f20 6f72 206f 6e65 2054 6173 6b28  ero or one Task(
+0000a1b0: 7329 206c 6973 7465 6420 7769 7468 696e  s) listed within
+0000a1c0: 2074 6865 2067 726f 7570 206f 7220 6074   the group or `t
+0000a1d0: 6173 6b43 6f75 6e74 6020 6973 2069 676e  askCount` is ign
+0000a1e0: 6f72 6564 2e0a 0a23 2320 4578 616d 706c  ored...## Exampl
+0000a1f0: 6573 0a0a 2323 2320 544f 4d4c 2050 726f  es..### TOML Pro
+0000a200: 7065 7274 6965 7320 696e 2074 6865 2060  perties in the `
+0000a210: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+0000a220: 2053 6563 7469 6f6e 0a0a 4865 7265 2773   Section..Here's
+0000a230: 2061 6e20 6578 616d 706c 6520 6f66 2074   an example of t
+0000a240: 6865 2060 776f 726b 5265 7175 6972 656d  he `workRequirem
+0000a250: 656e 7460 2073 6563 7469 6f6e 206f 6620  ent` section of 
+0000a260: 6120 544f 4d4c 2063 6f6e 6669 6775 7261  a TOML configura
+0000a270: 7469 6f6e 2066 696c 652c 2073 686f 7769  tion file, showi
+0000a280: 6e67 2061 6c6c 2074 6865 2070 6f73 7369  ng all the possi
+0000a290: 626c 6520 7072 6f70 6572 7469 6573 2074  ble properties t
+0000a2a0: 6861 7420 6361 6e20 6265 2073 6574 3a0a  hat can be set:.
+0000a2b0: 0a60 6060 746f 6d6c 0a5b 776f 726b 5265  .```toml.[workRe
+0000a2c0: 7175 6972 656d 656e 745d 0a20 2020 2061  quirement].    a
+0000a2d0: 7267 756d 656e 7473 203d 205b 2231 222c  rguments = ["1",
+0000a2e0: 2022 5457 4f22 5d0a 2020 2020 6361 7074   "TWO"].    capt
+0000a2f0: 7572 6554 6173 6b4f 7574 7075 7420 3d20  ureTaskOutput = 
+0000a300: 7472 7565 0a20 2020 2063 6f6d 706c 6574  true.    complet
+0000a310: 6564 5461 736b 5474 6c20 3d20 3130 0a20  edTaskTtl = 10. 
+0000a320: 2020 2063 7376 4669 6c65 203d 2022 6669     csvFile = "fi
+0000a330: 6c65 312e 6373 7622 0a20 2020 2063 7376  le1.csv".    csv
+0000a340: 4669 6c65 7320 3d20 5b22 6669 6c65 312e  Files = ["file1.
+0000a350: 6373 7622 2c20 2266 696c 6533 2e63 7376  csv", "file3.csv
+0000a360: 3a33 225d 0a20 2020 2064 6f63 6b65 7245  :3"].    dockerE
+0000a370: 6e76 6972 6f6e 6d65 6e74 203d 207b 4d59  nvironment = {MY
+0000a380: 5f44 4f43 4b45 525f 5641 5220 3d20 3130  _DOCKER_VAR = 10
+0000a390: 307d 0a20 2020 2064 6f63 6b65 7250 6173  0}.    dockerPas
+0000a3a0: 7377 6f72 6420 3d20 226d 7950 6173 7377  sword = "myPassw
+0000a3b0: 6f72 6422 0a20 2020 2064 6f63 6b65 7255  ord".    dockerU
+0000a3c0: 7365 726e 616d 6520 3d20 226d 7955 7365  sername = "myUse
+0000a3d0: 726e 616d 6522 0a20 2020 2065 6e76 6972  rname".    envir
+0000a3e0: 6f6e 6d65 6e74 203d 207b 4d59 5f56 4152  onment = {MY_VAR
+0000a3f0: 203d 2031 3030 7d0a 2020 2020 6578 636c   = 100}.    excl
+0000a400: 7573 6976 6557 6f72 6b65 7273 203d 2066  usiveWorkers = f
+0000a410: 616c 7365 0a20 2020 2065 7865 6375 7461  alse.    executa
+0000a420: 626c 6520 3d20 226d 792d 636f 6e74 6169  ble = "my-contai
+0000a430: 6e65 7222 0a20 2020 2066 696e 6973 6849  ner".    finishI
+0000a440: 6641 6c6c 5461 736b 7346 696e 6973 6865  fAllTasksFinishe
+0000a450: 6420 3d20 7472 7565 0a20 2020 2066 696e  d = true.    fin
+0000a460: 6973 6849 6641 6e79 5461 736b 4661 696c  ishIfAnyTaskFail
+0000a470: 6564 203d 2066 616c 7365 0a20 2020 2066  ed = false.    f
+0000a480: 6c61 7474 656e 496e 7075 7450 6174 6873  lattenInputPaths
+0000a490: 203d 2066 616c 7365 0a20 2020 2066 6c61   = false.    fla
+0000a4a0: 7474 656e 5570 6c6f 6164 5061 7468 7320  ttenUploadPaths 
+0000a4b0: 3d20 6661 6c73 650a 2020 2020 6675 6c66  = false.    fulf
+0000a4c0: 696c 4f6e 5375 626d 6974 203d 2066 616c  ilOnSubmit = fal
+0000a4d0: 7365 0a20 2020 2069 6e70 7574 7320 3d20  se.    inputs = 
+0000a4e0: 5b0a 2020 2020 2020 2020 222e 2e2f 6170  [.        "../ap
+0000a4f0: 702f 6d61 696e 2e70 7922 2c0a 2020 2020  p/main.py",.    
+0000a500: 2020 2020 222e 2e2f 6170 702f 7265 7175      "../app/requ
+0000a510: 6972 656d 656e 7473 2e74 7874 220a 2020  irements.txt".  
+0000a520: 2020 5d0a 2020 2020 696e 7075 7473 4f70    ].    inputsOp
+0000a530: 7469 6f6e 616c 203d 205b 226f 7074 696f  tional = ["optio
+0000a540: 6e61 6c2e 7478 7422 5d0a 2020 2020 696e  nal.txt"].    in
+0000a550: 7374 616e 6365 5479 7065 7320 3d20 5b22  stanceTypes = ["
+0000a560: 7433 612e 6d69 6372 6f22 2c20 2274 332e  t3a.micro", "t3.
+0000a570: 6d69 6372 6f22 5d0a 2020 2020 6d61 7857  micro"].    maxW
+0000a580: 6f72 6b65 7273 203d 2031 0a20 2020 206d  orkers = 1.    m
+0000a590: 6178 696d 756d 5461 736b 5265 7472 6965  aximumTaskRetrie
+0000a5a0: 7320 3d20 300a 2020 2020 6d69 6e57 6f72  s = 0.    minWor
+0000a5b0: 6b65 7273 203d 2031 0a20 2020 206e 616d  kers = 1.    nam
+0000a5c0: 6520 3d20 226d 792d 776f 726b 2d72 6571  e = "my-work-req
+0000a5d0: 7569 7265 6d65 6e74 220a 2020 2020 6f75  uirement".    ou
+0000a5e0: 7470 7574 7320 3d20 5b22 7265 7375 6c74  tputs = ["result
+0000a5f0: 732e 7478 7422 5d0a 2020 2020 6f75 7470  s.txt"].    outp
+0000a600: 7574 7352 6571 7569 7265 6420 3d20 5b22  utsRequired = ["
+0000a610: 7265 7375 6c74 735f 7265 7175 6972 6564  results_required
+0000a620: 2e74 7874 225d 0a20 2020 2070 7269 6f72  .txt"].    prior
+0000a630: 6974 7920 3d20 302e 300a 2020 2020 7072  ity = 0.0.    pr
+0000a640: 6f76 6964 6572 7320 3d20 5b22 4157 5322  oviders = ["AWS"
+0000a650: 5d0a 2020 2020 7261 6d20 3d20 5b30 2e35  ].    ram = [0.5
+0000a660: 2c20 322e 305d 0a20 2020 2072 6567 696f  , 2.0].    regio
+0000a670: 6e73 203d 205b 2265 752d 7765 7374 2d32  ns = ["eu-west-2
+0000a680: 225d 0a20 2020 2074 6173 6b42 6174 6368  "].    taskBatch
+0000a690: 5369 7a65 203d 2031 3030 300a 2020 2020  Size = 1000.    
+0000a6a0: 7461 736b 436f 756e 7420 3d20 3130 300a  taskCount = 100.
+0000a6b0: 2020 2020 7461 736b 4461 7461 203d 2022      taskData = "
+0000a6c0: 6d79 5f64 6174 615f 7374 7269 6e67 220a  my_data_string".
+0000a6d0: 2020 2020 7461 736b 4461 7461 4669 6c65      taskDataFile
+0000a6e0: 203d 2022 6d79 5f64 6174 615f 6669 6c65   = "my_data_file
+0000a6f0: 2e74 7874 220a 2020 2020 7461 736b 4e61  .txt".    taskNa
+0000a700: 6d65 203d 2022 6d79 5f74 6173 6b5f 6e75  me = "my_task_nu
+0000a710: 6d62 6572 5f7b 7b74 6173 6b5f 6e75 6d62  mber_{{task_numb
+0000a720: 6572 7d7d 220a 2020 2020 7461 736b 4772  er}}".    taskGr
+0000a730: 6f75 704e 616d 6520 3d20 226d 795f 7461  oupName = "my_ta
+0000a740: 736b 5f67 726f 7570 5f6e 756d 6265 725f  sk_group_number_
+0000a750: 7b7b 7461 736b 5f67 726f 7570 5f6e 756d  {{task_group_num
+0000a760: 6265 727d 7d22 0a20 2020 2074 6173 6b54  ber}}".    taskT
+0000a770: 7970 6520 3d20 2264 6f63 6b65 7222 0a20  ype = "docker". 
+0000a780: 2020 2074 6173 6b73 5065 7257 6f72 6b65     tasksPerWorke
+0000a790: 7220 3d20 310a 2020 2020 7570 6c6f 6164  r = 1.    upload
+0000a7a0: 4669 6c65 7320 3d20 5b7b 6c6f 6361 6c50  Files = [{localP
+0000a7b0: 6174 6820 3d20 2266 696c 655f 312e 7478  ath = "file_1.tx
+0000a7c0: 7422 2c20 7570 6c6f 6164 5061 7468 203d  t", uploadPath =
+0000a7d0: 2022 6669 6c65 5f31 2e74 7874 227d 5d0a   "file_1.txt"}].
+0000a7e0: 2020 2020 7663 7075 7320 3d20 5b31 2c20      vcpus = [1, 
+0000a7f0: 345d 0a20 2020 2076 6572 6966 7941 7453  4].    verifyAtS
+0000a800: 7461 7274 203d 205b 2272 6561 6479 5f72  tart = ["ready_r
+0000a810: 6573 756c 7473 2e74 7874 225d 0a20 2020  esults.txt"].   
+0000a820: 2076 6572 6966 7957 6169 7420 3d20 5b22   verifyWait = ["
+0000a830: 7761 6974 5f66 6f72 5f72 6573 756c 7473  wait_for_results
+0000a840: 2e74 7874 225d 0a20 2020 2077 6f72 6b65  .txt"].    worke
+0000a850: 7254 6167 7320 3d20 5b22 7461 672d 7b7b  rTags = ["tag-{{
+0000a860: 7573 6572 6e61 6d65 7d7d 225d 0a20 2020  username}}"].   
+0000a870: 2077 6f72 6b52 6571 7569 7265 6d65 6e74   workRequirement
+0000a880: 4461 7461 203d 2022 776f 726b 5f72 6571  Data = "work_req
+0000a890: 7569 7265 6d65 6e74 2e6a 736f 6e22 0a60  uirement.json".`
+0000a8a0: 6060 0a0a 2323 2320 4a53 4f4e 2050 726f  ``..### JSON Pro
+0000a8b0: 7065 7274 6965 7320 6174 2074 6865 2057  perties at the W
+0000a8c0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000a8d0: 4c65 7665 6c0a 0a53 686f 7769 6e67 2061  Level..Showing a
+0000a8e0: 6c6c 2070 6f73 7369 626c 6520 7072 6f70  ll possible prop
+0000a8f0: 6572 7469 6573 2061 7420 7468 6520 576f  erties at the Wo
+0000a900: 726b 2052 6571 7569 7265 6d65 6e74 206c  rk Requirement l
+0000a910: 6576 656c 3a0a 0a60 6060 6a73 6f6e 0a7b  evel:..```json.{
+0000a920: 0a20 2022 6172 6775 6d65 6e74 7322 3a20  .  "arguments": 
+0000a930: 5b31 2c20 2254 574f 225d 2c0a 2020 2263  [1, "TWO"],.  "c
+0000a940: 6170 7475 7265 5461 736b 4f75 7470 7574  aptureTaskOutput
+0000a950: 223a 2074 7275 652c 0a20 2022 636f 6d70  ": true,.  "comp
+0000a960: 6c65 7465 6454 6173 6b54 746c 223a 2031  letedTaskTtl": 1
+0000a970: 302c 0a20 2022 646f 636b 6572 456e 7669  0,.  "dockerEnvi
+0000a980: 726f 6e6d 656e 7422 3a20 7b22 4d59 5f44  ronment": {"MY_D
+0000a990: 4f43 4b45 525f 5641 5222 3a20 3130 307d  OCKER_VAR": 100}
+0000a9a0: 2c0a 2020 2264 6f63 6b65 7250 6173 7377  ,.  "dockerPassw
+0000a9b0: 6f72 6422 3a20 226d 7950 6173 7377 6f72  ord": "myPasswor
+0000a9c0: 6422 2c0a 2020 2264 6f63 6b65 7255 7365  d",.  "dockerUse
+0000a9d0: 726e 616d 6522 3a20 226d 7955 7365 726e  rname": "myUsern
+0000a9e0: 616d 6522 2c0a 2020 2265 6e76 6972 6f6e  ame",.  "environ
+0000a9f0: 6d65 6e74 223a 207b 224d 595f 5641 5222  ment": {"MY_VAR"
+0000aa00: 3a20 3130 307d 2c0a 2020 2265 7863 6c75  : 100},.  "exclu
+0000aa10: 7369 7665 576f 726b 6572 7322 3a20 6661  siveWorkers": fa
+0000aa20: 6c73 652c 0a20 2022 6578 6563 7574 6162  lse,.  "executab
+0000aa30: 6c65 223a 2022 6d79 2d63 6f6e 7461 696e  le": "my-contain
+0000aa40: 6572 222c 0a20 2022 6669 6e69 7368 4966  er",.  "finishIf
+0000aa50: 416c 6c54 6173 6b73 4669 6e69 7368 6564  AllTasksFinished
+0000aa60: 223a 2074 7275 652c 0a20 2022 6669 6e69  ": true,.  "fini
+0000aa70: 7368 4966 416e 7954 6173 6b46 6169 6c65  shIfAnyTaskFaile
+0000aa80: 6422 3a20 6661 6c73 652c 0a20 2022 666c  d": false,.  "fl
+0000aa90: 6174 7465 6e49 6e70 7574 5061 7468 7322  attenInputPaths"
+0000aaa0: 3a20 6661 6c73 652c 0a20 2022 666c 6174  : false,.  "flat
+0000aab0: 7465 6e55 706c 6f61 6450 6174 6873 223a  tenUploadPaths":
+0000aac0: 2066 616c 7365 2c0a 2020 2266 756c 6669   false,.  "fulfi
+0000aad0: 6c4f 6e53 7562 6d69 7422 3a20 6661 6c73  lOnSubmit": fals
+0000aae0: 652c 0a20 2022 696e 7075 7473 223a 205b  e,.  "inputs": [
+0000aaf0: 2261 7070 2f6d 6169 6e2e 7079 222c 2022  "app/main.py", "
+0000ab00: 6170 702f 7265 7175 6972 656d 656e 7473  app/requirements
+0000ab10: 2e74 7874 225d 2c0a 2020 2269 6e70 7574  .txt"],.  "input
+0000ab20: 734f 7074 696f 6e61 6c22 3a20 5b22 6f70  sOptional": ["op
+0000ab30: 7469 6f6e 616c 2e74 7874 225d 2c0a 2020  tional.txt"],.  
+0000ab40: 2269 6e73 7461 6e63 6554 7970 6573 223a  "instanceTypes":
+0000ab50: 205b 2274 3361 2e6d 6963 726f 222c 2022   ["t3a.micro", "
+0000ab60: 7433 2e6d 6963 726f 225d 2c0a 2020 226d  t3.micro"],.  "m
+0000ab70: 6178 576f 726b 6572 7322 3a20 312c 0a20  axWorkers": 1,. 
+0000ab80: 2022 6d61 7869 6d75 6d54 6173 6b52 6574   "maximumTaskRet
+0000ab90: 7269 6573 223a 2030 2c0a 2020 226d 696e  ries": 0,.  "min
+0000aba0: 576f 726b 6572 7322 3a20 312c 0a20 2022  Workers": 1,.  "
+0000abb0: 6e61 6d65 223a 2022 6d79 2d77 6f72 6b2d  name": "my-work-
+0000abc0: 7265 7175 6972 656d 656e 7422 2c0a 2020  requirement",.  
+0000abd0: 226f 7574 7075 7473 223a 205b 2272 6573  "outputs": ["res
+0000abe0: 756c 7473 2e74 7874 225d 2c0a 2020 226f  ults.txt"],.  "o
+0000abf0: 7574 7075 7473 5265 7175 6972 6564 223a  utputsRequired":
+0000ac00: 205b 2272 6573 756c 7473 5f72 6571 7569   ["results_requi
+0000ac10: 7265 642e 7478 7422 5d2c 0a20 2022 7072  red.txt"],.  "pr
+0000ac20: 696f 7269 7479 223a 2030 2e30 2c0a 2020  iority": 0.0,.  
+0000ac30: 2270 726f 7669 6465 7273 223a 205b 2241  "providers": ["A
+0000ac40: 5753 225d 2c0a 2020 2272 616d 223a 205b  WS"],.  "ram": [
+0000ac50: 302e 352c 2032 5d2c 0a20 2022 7265 6769  0.5, 2],.  "regi
+0000ac60: 6f6e 7322 3a20 5b22 6575 2d77 6573 742d  ons": ["eu-west-
+0000ac70: 3222 5d2c 0a20 2022 7461 736b 4461 7461  2"],.  "taskData
+0000ac80: 223a 2022 6d79 5f74 6173 6b5f 6461 7461  ": "my_task_data
+0000ac90: 5f73 7472 696e 6722 2c0a 2020 2274 6173  _string",.  "tas
+0000aca0: 6b44 6174 6146 696c 6522 3a20 226d 795f  kDataFile": "my_
+0000acb0: 6461 7461 5f66 696c 652e 7478 7422 2c0a  data_file.txt",.
+0000acc0: 2020 2274 6173 6b54 7970 6573 223a 205b    "taskTypes": [
+0000acd0: 2264 6f63 6b65 7222 5d2c 0a20 2022 7461  "docker"],.  "ta
+0000ace0: 736b 7350 6572 576f 726b 6572 223a 2031  sksPerWorker": 1
+0000acf0: 2c0a 2020 2275 706c 6f61 6446 696c 6573  ,.  "uploadFiles
+0000ad00: 223a 205b 7b22 6c6f 6361 6c50 6174 6822  ": [{"localPath"
+0000ad10: 3a20 2266 696c 655f 312e 7478 7422 2c20  : "file_1.txt", 
+0000ad20: 2275 706c 6f61 6450 6174 6822 3a20 2266  "uploadPath": "f
+0000ad30: 696c 655f 312e 7478 7422 7d5d 2c0a 2020  ile_1.txt"}],.  
+0000ad40: 2276 6370 7573 223a 205b 312c 2034 5d2c  "vcpus": [1, 4],
+0000ad50: 0a20 2022 7665 7269 6679 4174 5374 6172  .  "verifyAtStar
+0000ad60: 7422 3a20 5b22 7265 6164 795f 7265 7375  t": ["ready_resu
+0000ad70: 6c74 732e 7478 7422 5d2c 0a20 2022 7665  lts.txt"],.  "ve
+0000ad80: 7269 6679 5761 6974 223a 205b 2277 6169  rifyWait": ["wai
+0000ad90: 745f 666f 725f 7265 7375 6c74 732e 7478  t_for_results.tx
+0000ada0: 7422 5d2c 0a20 2022 776f 726b 6572 5461  t"],.  "workerTa
+0000adb0: 6773 223a 205b 5d2c 0a20 2022 7461 736b  gs": [],.  "task
+0000adc0: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+0000add0: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+0000ade0: 5b0a 2020 2020 2020 2020 7b7d 0a20 2020  [.        {}.   
+0000adf0: 2020 205d 0a20 2020 207d 0a20 205d 0a7d     ].    }.  ].}
+0000ae00: 0a0a 6060 600a 0a23 2323 204a 534f 4e20  ..```..### JSON 
+0000ae10: 5072 6f70 6572 7469 6573 2061 7420 7468  Properties at th
+0000ae20: 6520 5461 736b 2047 726f 7570 204c 6576  e Task Group Lev
+0000ae30: 656c 0a0a 5368 6f77 696e 6720 616c 6c20  el..Showing all 
+0000ae40: 706f 7373 6962 6c65 2070 726f 7065 7274  possible propert
+0000ae50: 6965 7320 6174 2074 6865 2054 6173 6b20  ies at the Task 
+0000ae60: 4772 6f75 7020 6c65 7665 6c3a 0a0a 6060  Group level:..``
+0000ae70: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
+0000ae80: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+0000ae90: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
+0000aea0: 223a 205b 312c 2022 5457 4f22 5d2c 0a20  ": [1, "TWO"],. 
+0000aeb0: 2020 2020 2022 6361 7074 7572 6554 6173       "captureTas
+0000aec0: 6b4f 7574 7075 7422 3a20 7472 7565 2c0a  kOutput": true,.
+0000aed0: 2020 2020 2020 2263 6f6d 706c 6574 6564        "completed
+0000aee0: 5461 736b 5474 6c22 3a20 3130 2c0a 2020  TaskTtl": 10,.  
+0000aef0: 2020 2020 2264 6f63 6b65 7245 6e76 6972      "dockerEnvir
+0000af00: 6f6e 6d65 6e74 223a 207b 224d 595f 444f  onment": {"MY_DO
+0000af10: 434b 4552 5f56 4152 223a 2031 3030 7d2c  CKER_VAR": 100},
+0000af20: 0a20 2020 2020 2022 646f 636b 6572 5061  .      "dockerPa
+0000af30: 7373 776f 7264 223a 2022 6d79 5061 7373  ssword": "myPass
+0000af40: 776f 7264 222c 0a20 2020 2020 2022 646f  word",.      "do
+0000af50: 636b 6572 5573 6572 6e61 6d65 223a 2022  ckerUsername": "
+0000af60: 6d79 5573 6572 6e61 6d65 222c 0a20 2020  myUsername",.   
+0000af70: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
+0000af80: 3a20 7b22 4d59 5f56 4152 223a 2031 3030  : {"MY_VAR": 100
+0000af90: 7d2c 0a20 2020 2020 2022 6578 636c 7573  },.      "exclus
+0000afa0: 6976 6557 6f72 6b65 7273 223a 2066 616c  iveWorkers": fal
+0000afb0: 7365 2c0a 2020 2020 2020 2265 7865 6375  se,.      "execu
+0000afc0: 7461 626c 6522 3a20 226d 792d 636f 6e74  table": "my-cont
+0000afd0: 6169 6e65 7222 2c0a 2020 2020 2020 2266  ainer",.      "f
+0000afe0: 696e 6973 6849 6641 6c6c 5461 736b 7346  inishIfAllTasksF
+0000aff0: 696e 6973 6865 6422 3a20 7472 7565 2c0a  inished": true,.
+0000b000: 2020 2020 2020 2266 696e 6973 6849 6641        "finishIfA
+0000b010: 6e79 5461 736b 4661 696c 6564 223a 2066  nyTaskFailed": f
+0000b020: 616c 7365 2c0a 2020 2020 2020 2266 6c61  alse,.      "fla
+0000b030: 7474 656e 496e 7075 7450 6174 6873 223a  ttenInputPaths":
+0000b040: 2066 616c 7365 2c0a 2020 2020 2020 2269   false,.      "i
+0000b050: 6e70 7574 7322 3a20 5b22 6170 702f 6d61  nputs": ["app/ma
+0000b060: 696e 2e70 7922 2c20 2261 7070 2f72 6571  in.py", "app/req
+0000b070: 7569 7265 6d65 6e74 732e 7478 7422 5d2c  uirements.txt"],
+0000b080: 0a20 2020 2020 2022 696e 7075 7473 4f70  .      "inputsOp
+0000b090: 7469 6f6e 616c 223a 205b 226f 7074 696f  tional": ["optio
+0000b0a0: 6e61 6c2e 7478 7422 5d2c 0a20 2020 2020  nal.txt"],.     
+0000b0b0: 2022 696e 7374 616e 6365 5479 7065 7322   "instanceTypes"
+0000b0c0: 3a20 5b22 7433 612e 6d69 6372 6f22 2c20  : ["t3a.micro", 
+0000b0d0: 2274 332e 6d69 6372 6f22 5d2c 0a20 2020  "t3.micro"],.   
+0000b0e0: 2020 2022 6d61 7869 6d75 6d54 6173 6b52     "maximumTaskR
+0000b0f0: 6574 7269 6573 223a 2030 2c0a 2020 2020  etries": 0,.    
+0000b100: 2020 226d 6178 576f 726b 6572 7322 3a20    "maxWorkers": 
+0000b110: 312c 0a20 2020 2020 2022 6d69 6e57 6f72  1,.      "minWor
+0000b120: 6b65 7273 223a 2031 2c0a 2020 2020 2020  kers": 1,.      
+0000b130: 226e 616d 6522 3a20 2266 6972 7374 2d74  "name": "first-t
+0000b140: 6173 6b2d 6772 6f75 7022 2c0a 2020 2020  ask-group",.    
+0000b150: 2020 226f 7574 7075 7473 223a 205b 2272    "outputs": ["r
+0000b160: 6573 756c 7473 2e74 7874 225d 2c0a 2020  esults.txt"],.  
+0000b170: 2020 2020 226f 7574 7075 7473 5265 7175      "outputsRequ
+0000b180: 6972 6564 223a 205b 2272 6573 756c 7473  ired": ["results
+0000b190: 5f72 6571 7569 7265 642e 7478 7422 5d2c  _required.txt"],
+0000b1a0: 0a20 2020 2020 2022 7072 696f 7269 7479  .      "priority
+0000b1b0: 223a 2030 2e30 2c0a 2020 2020 2020 2270  ": 0.0,.      "p
+0000b1c0: 726f 7669 6465 7273 223a 205b 2241 5753  roviders": ["AWS
+0000b1d0: 225d 2c0a 2020 2020 2020 2272 616d 223a  "],.      "ram":
+0000b1e0: 205b 302e 352c 2032 5d2c 0a20 2020 2020   [0.5, 2],.     
+0000b1f0: 2022 7265 6769 6f6e 7322 3a20 5b22 6575   "regions": ["eu
+0000b200: 2d77 6573 742d 3222 5d2c 0a20 2020 2020  -west-2"],.     
+0000b210: 2022 7461 736b 436f 756e 7422 3a20 352c   "taskCount": 5,
+0000b220: 0a20 2020 2020 2022 7461 736b 4461 7461  .      "taskData
+0000b230: 223a 2022 6d79 5f74 6173 6b5f 6461 7461  ": "my_task_data
+0000b240: 5f73 7472 696e 6722 2c0a 2020 2020 2020  _string",.      
+0000b250: 2274 6173 6b44 6174 6146 696c 6522 3a20  "taskDataFile": 
+0000b260: 226d 795f 6461 7461 5f66 696c 652e 7478  "my_data_file.tx
+0000b270: 7422 2c0a 2020 2020 2020 2274 6173 6b54  t",.      "taskT
+0000b280: 7970 6573 223a 205b 2264 6f63 6b65 7222  ypes": ["docker"
+0000b290: 5d2c 0a20 2020 2020 2022 7461 736b 7350  ],.      "tasksP
+0000b2a0: 6572 576f 726b 6572 223a 2031 2c0a 2020  erWorker": 1,.  
+0000b2b0: 2020 2020 2275 706c 6f61 6446 696c 6573      "uploadFiles
+0000b2c0: 223a 205b 7b22 6c6f 6361 6c50 6174 6822  ": [{"localPath"
+0000b2d0: 3a20 2266 696c 655f 312e 7478 7422 2c20  : "file_1.txt", 
+0000b2e0: 2275 706c 6f61 6450 6174 6822 3a20 2266  "uploadPath": "f
+0000b2f0: 696c 655f 312e 7478 7422 7d5d 2c0a 2020  ile_1.txt"}],.  
+0000b300: 2020 2020 2276 6370 7573 223a 205b 312c      "vcpus": [1,
+0000b310: 2034 5d2c 0a20 2020 2020 2022 7665 7269   4],.      "veri
+0000b320: 6679 4174 5374 6172 7422 3a20 5b22 7265  fyAtStart": ["re
+0000b330: 6164 795f 7265 7375 6c74 732e 7478 7422  ady_results.txt"
+0000b340: 5d2c 0a20 2020 2020 2022 7665 7269 6679  ],.      "verify
+0000b350: 5761 6974 223a 205b 2277 6169 745f 666f  Wait": ["wait_fo
+0000b360: 725f 7265 7375 6c74 732e 7478 7422 5d2c  r_results.txt"],
+0000b370: 0a20 2020 2020 2022 776f 726b 6572 5461  .      "workerTa
+0000b380: 6773 223a 205b 5d2c 0a20 2020 2020 2022  gs": [],.      "
+0000b390: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
+0000b3a0: 2020 7b7d 0a20 2020 2020 205d 0a20 2020    {}.      ].   
+0000b3b0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+0000b3c0: 226e 616d 6522 3a20 2273 6563 6f6e 642d  "name": "second-
+0000b3d0: 7461 736b 2d67 726f 7570 222c 0a20 2020  task-group",.   
+0000b3e0: 2020 2022 6465 7065 6e64 656e 744f 6e22     "dependentOn"
+0000b3f0: 3a20 2266 6972 7374 2d74 6173 6b2d 6772  : "first-task-gr
+0000b400: 6f75 7022 2c0a 2020 2020 2020 2274 6173  oup",.      "tas
+0000b410: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
+0000b420: 7d0a 2020 2020 2020 5d0a 2020 2020 7d0a  }.      ].    }.
+0000b430: 2020 5d0a 7d0a 6060 600a 0a23 2323 204a    ].}.```..### J
+0000b440: 534f 4e20 5072 6f70 6572 7469 6573 2061  SON Properties a
+0000b450: 7420 7468 6520 5461 736b 204c 6576 656c  t the Task Level
+0000b460: 0a0a 5368 6f77 696e 6720 616c 6c20 706f  ..Showing all po
+0000b470: 7373 6962 6c65 2070 726f 7065 7274 6965  ssible propertie
+0000b480: 7320 6174 2074 6865 2054 6173 6b20 6c65  s at the Task le
+0000b490: 7665 6c3a 0a0a 6060 606a 736f 6e0a 7b0a  vel:..```json.{.
+0000b4a0: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
+0000b4b0: 5b0a 2020 2020 7b0a 2020 2020 2020 2274  [.    {.      "t
+0000b4c0: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
+0000b4d0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+0000b4e0: 6775 6d65 6e74 7322 3a20 5b31 2c20 325d  guments": [1, 2]
+0000b4f0: 2c0a 2020 2020 2020 2020 2020 2263 6170  ,.          "cap
+0000b500: 7475 7265 5461 736b 4f75 7470 7574 223a  tureTaskOutput":
+0000b510: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+0000b520: 2022 646f 636b 6572 456e 7669 726f 6e6d   "dockerEnvironm
+0000b530: 656e 7422 3a20 7b22 4d59 5f44 4f43 4b45  ent": {"MY_DOCKE
+0000b540: 525f 5641 5222 3a20 3130 307d 2c0a 2020  R_VAR": 100},.  
+0000b550: 2020 2020 2020 2020 2264 6f63 6b65 7250          "dockerP
+0000b560: 6173 7377 6f72 6422 3a20 226d 7950 6173  assword": "myPas
+0000b570: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
+0000b580: 2020 2264 6f63 6b65 7255 7365 726e 616d    "dockerUsernam
+0000b590: 6522 3a20 226d 7955 7365 726e 616d 6522  e": "myUsername"
+0000b5a0: 2c0a 2020 2020 2020 2020 2020 2265 6e76  ,.          "env
+0000b5b0: 6972 6f6e 6d65 6e74 223a 207b 224d 595f  ironment": {"MY_
+0000b5c0: 5641 5222 3a20 3130 307d 2c0a 2020 2020  VAR": 100},.    
+0000b5d0: 2020 2020 2020 2265 7865 6375 7461 626c        "executabl
+0000b5e0: 6522 3a20 226d 792d 636f 6e74 6169 6e65  e": "my-containe
+0000b5f0: 7222 2c0a 2020 2020 2020 2020 2020 2266  r",.          "f
+0000b600: 6c61 7474 656e 496e 7075 7450 6174 6873  lattenInputPaths
+0000b610: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+0000b620: 2020 2020 2269 6e70 7574 7322 3a20 5b22      "inputs": ["
+0000b630: 6170 702f 6d61 696e 2e70 7922 2c20 2261  app/main.py", "a
+0000b640: 7070 2f72 6571 7569 7265 6d65 6e74 732e  pp/requirements.
+0000b650: 7478 7422 5d2c 0a20 2020 2020 2020 2020  txt"],.         
+0000b660: 2022 696e 7075 7473 4f70 7469 6f6e 616c   "inputsOptional
+0000b670: 223a 205b 226f 7074 696f 6e61 6c2e 7478  ": ["optional.tx
+0000b680: 7422 5d2c 0a20 2020 2020 2020 2020 2022  t"],.          "
+0000b690: 6e61 6d65 223a 2022 6d79 2d74 6173 6b22  name": "my-task"
+0000b6a0: 2c0a 2020 2020 2020 2020 2020 226f 7574  ,.          "out
+0000b6b0: 7075 7473 223a 205b 2272 6573 756c 7473  puts": ["results
+0000b6c0: 2e74 7874 225d 2c0a 2020 2020 2020 2020  .txt"],.        
+0000b6d0: 2020 226f 7574 7075 7473 5265 7175 6972    "outputsRequir
+0000b6e0: 6564 223a 205b 2272 6573 756c 7473 5f72  ed": ["results_r
+0000b6f0: 6571 7569 7265 642e 7478 7422 5d2c 0a20  equired.txt"],. 
+0000b700: 2020 2020 2020 2020 2022 7461 736b 4461           "taskDa
+0000b710: 7461 223a 2022 6d79 5f74 6173 6b5f 6461  ta": "my_task_da
+0000b720: 7461 5f73 7472 696e 6722 2c0a 2020 2020  ta_string",.    
+0000b730: 2020 2020 2020 2274 6173 6b44 6174 6146        "taskDataF
+0000b740: 696c 6522 3a20 226d 795f 6461 7461 5f66  ile": "my_data_f
+0000b750: 696c 652e 7478 7422 2c0a 2020 2020 2020  ile.txt",.      
+0000b760: 2020 2020 2274 6173 6b54 7970 6522 3a20      "taskType": 
+0000b770: 2264 6f63 6b65 7222 2c0a 2020 2020 2020  "docker",.      
+0000b780: 2020 2020 2275 706c 6f61 6446 696c 6573      "uploadFiles
+0000b790: 223a 205b 7b22 6c6f 6361 6c50 6174 6822  ": [{"localPath"
+0000b7a0: 3a20 2266 696c 655f 312e 7478 7422 2c20  : "file_1.txt", 
+0000b7b0: 2275 706c 6f61 6450 6174 6822 3a20 2266  "uploadPath": "f
+0000b7c0: 696c 655f 312e 7478 7422 7d5d 2c0a 2020  ile_1.txt"}],.  
+0000b7d0: 2020 2020 2020 2020 2276 6572 6966 7941          "verifyA
+0000b7e0: 7453 7461 7274 223a 205b 2272 6561 6479  tStart": ["ready
+0000b7f0: 5f72 6573 756c 7473 2e74 7874 225d 2c0a  _results.txt"],.
+0000b800: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
+0000b810: 7957 6169 7422 3a20 5b22 7761 6974 5f66  yWait": ["wait_f
+0000b820: 6f72 5f72 6573 756c 7473 2e74 7874 225d  or_results.txt"]
+0000b830: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0000b840: 205d 0a20 2020 207d 0a20 205d 0a7d 0a60   ].    }.  ].}.`
+0000b850: 6060 0a0a 2323 2056 6172 6961 626c 6520  ``..## Variable 
+0000b860: 5375 6273 7469 7475 7469 6f6e 7320 696e  Substitutions in
+0000b870: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000b880: 7420 5072 6f70 6572 7469 6573 0a0a 5661  t Properties..Va
+0000b890: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+0000b8a0: 696f 6e73 2063 616e 2062 6520 7573 6564  ions can be used
+0000b8b0: 2077 6974 6869 6e20 616e 7920 7072 6f70   within any prop
+0000b8c0: 6572 7479 2076 616c 7565 2069 6e20 544f  erty value in TO
+0000b8d0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+0000b8e0: 2066 696c 6573 206f 7220 576f 726b 2052   files or Work R
+0000b8f0: 6571 7569 7265 6d65 6e74 204a 534f 4e20  equirement JSON 
+0000b900: 6669 6c65 732e 2053 6565 2074 6865 2064  files. See the d
+0000b910: 6573 6372 6970 7469 6f6e 205b 6162 6f76  escription [abov
+0000b920: 655d 2823 7661 7269 6162 6c65 2d73 7562  e](#variable-sub
+0000b930: 7374 6974 7574 696f 6e73 2920 666f 7220  stitutions) for 
+0000b940: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
+0000b950: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+0000b960: 7574 696f 6e73 2e20 5468 6973 2069 7320  utions. This is 
+0000b970: 6120 706f 7765 7266 756c 2066 6561 7475  a powerful featu
+0000b980: 7265 2074 6861 7420 616c 6c6f 7773 2057  re that allows W
+0000b990: 6f72 6b20 5265 7175 6972 656d 656e 7473  ork Requirements
+0000b9a0: 2074 6f20 6265 2070 6172 616d 6574 6572   to be parameter
+0000b9b0: 6973 6564 2062 7920 7375 7070 6c79 696e  ised by supplyin
+0000b9c0: 6720 7661 6c75 6573 206f 6e20 7468 6520  g values on the 
+0000b9d0: 636f 6d6d 616e 6420 6c69 6e65 2c20 7669  command line, vi
+0000b9e0: 6120 656e 7669 726f 6e6d 656e 7420 7661  a environment va
+0000b9f0: 7269 6162 6c65 7320 6f72 2076 6961 2074  riables or via t
+0000ba00: 6865 2054 4f4d 4c20 6669 6c65 2e0a 0a23  he TOML file...#
+0000ba10: 2323 2054 6173 6b20 616e 6420 5461 736b  ## Task and Task
+0000ba20: 2047 726f 7570 204e 616d 6520 5375 6273   Group Name Subs
+0000ba30: 7469 7475 7469 6f6e 0a0a 5468 6520 666f  titution..The fo
+0000ba40: 6c6c 6f77 696e 6720 6e75 6d62 6572 696e  llowing numberin
+0000ba50: 6720 616e 6420 6e61 6d69 6e67 2073 7562  g and naming sub
+0000ba60: 7374 6974 7574 696f 6e73 2061 7265 2061  stitutions are a
+0000ba70: 7661 696c 6162 6c65 2066 6f72 2075 7365  vailable for use
+0000ba80: 2069 6e20 5461 736b 2061 6e64 2054 6173   in Task and Tas
+0000ba90: 6b20 4772 6f75 7020 6e61 6d69 6e67 2c20  k Group naming, 
+0000baa0: 6f6e 6c79 2077 6865 6e20 7468 6520 576f  only when the Wo
+0000bab0: 726b 2052 6571 7569 7265 6d65 6e74 2069  rk Requirement i
+0000bac0: 7320 7370 6563 6966 6965 6420 6173 2020  s specified as  
+0000bad0: 4a53 4f4e 2064 6f63 756d 656e 742c 2069  JSON document, i
+0000bae0: 2e65 2e2c 2074 6865 7920 6361 6e20 6265  .e., they can be
+0000baf0: 2075 7365 6420 696e 2074 6865 2060 6e61   used in the `na
+0000bb00: 6d65 6020 7072 6f70 6572 7469 6573 2066  me` properties f
+0000bb10: 6f72 2054 6173 6b73 2061 6e64 2054 6173  or Tasks and Tas
+0000bb20: 6b20 4772 6f75 7073 2069 6e20 4a53 4f4e  k Groups in JSON
+0000bb30: 2073 7065 6369 6669 6361 7469 6f6e 732e   specifications.
+0000bb40: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
+0000bb50: 7461 626c 6520 6465 6669 6e65 7320 7468  table defines th
+0000bb60: 6520 636f 6e74 6578 7428 7329 2069 6e20  e context(s) in 
+0000bb70: 7768 6963 6820 6561 6368 2076 6172 6961  which each varia
+0000bb80: 626c 6520 6361 6e20 6265 2075 7365 643a  ble can be used:
+0000bb90: 0a0a 7c20 4469 7265 6374 6976 6520 2020  ..| Directive   
+0000bba0: 2020 2020 2020 2020 2020 2020 7c20 4465              | De
+0000bbb0: 7363 7269 7074 696f 6e20 2020 2020 2020  scription       
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 7c20 5461 736b 207c 2054 6173 6b20 4772  | Task | Task Gr
+0000bbf0: 6f75 7020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d  oup |.|:--------
+0000bc00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc10: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+0000bc20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc40: 2d2d 2d2d 7c3a 2d2d 2d2d 2d7c 3a2d 2d2d  ----|:-----|:---
+0000bc50: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 607b 7b74  --------|.| `{{t
+0000bc60: 6173 6b5f 6e75 6d62 6572 7d7d 6020 2020  ask_number}}`   
+0000bc70: 2020 2020 7c20 5468 6520 6375 7272 656e      | The curren
+0000bc80: 7420 5461 736b 206e 756d 6265 7220 2020  t Task number   
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+0000bcb0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0000bcc0: 607b 7b74 6173 6b5f 6e61 6d65 7d7d 6020  `{{task_name}}` 
+0000bcd0: 2020 2020 2020 2020 7c20 5468 6520 6375          | The cu
+0000bce0: 7272 656e 7420 5461 736b 206e 616d 6520  rrent Task name 
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd00: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+0000bd10: 7320 207c 2020 2020 2020 2020 2020 2020  s  |            
+0000bd20: 7c0a 7c20 607b 7b74 6173 6b5f 6772 6f75  |.| `{{task_grou
+0000bd30: 705f 6e61 6d65 7d7d 6020 2020 7c20 5468  p_name}}`   | Th
+0000bd40: 6520 6375 7272 656e 7420 5461 736b 2047  e current Task G
+0000bd50: 726f 7570 206e 616d 6520 2020 2020 2020  roup name       
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 7c20 5965 7320 207c 2020 2020 2020 2020  | Yes  |        
+0000bd80: 2020 2020 7c0a 7c20 607b 7b74 6173 6b5f      |.| `{{task_
+0000bd90: 636f 756e 747d 7d60 2020 2020 2020 2020  count}}`        
+0000bda0: 7c20 5468 6520 6e75 6d62 6572 206f 6620  | The number of 
+0000bdb0: 5461 736b 7320 696e 2074 6865 2063 7572  Tasks in the cur
+0000bdc0: 7265 6e74 2054 6173 6b20 4772 6f75 7020  rent Task Group 
+0000bdd0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+0000bde0: 2020 2020 2020 2020 7c0a 7c20 607b 7b74          |.| `{{t
+0000bdf0: 6173 6b5f 6772 6f75 705f 6e75 6d62 6572  ask_group_number
+0000be00: 7d7d 6020 7c20 5468 6520 6375 7272 656e  }}` | The curren
+0000be10: 7420 5461 736b 2047 726f 7570 206e 756d  t Task Group num
+0000be20: 6265 7220 2020 2020 2020 2020 2020 2020  ber             
+0000be30: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+0000be40: 2059 6573 2020 2020 2020 2020 7c0a 7c20   Yes        |.| 
+0000be50: 607b 7b74 6173 6b5f 6772 6f75 705f 636f  `{{task_group_co
+0000be60: 756e 747d 7d60 2020 7c20 5468 6520 6e75  unt}}`  | The nu
+0000be70: 6d62 6572 206f 6620 5461 736b 2047 726f  mber of Task Gro
+0000be80: 7570 7320 696e 2074 6865 2057 6f72 6b20  ups in the Work 
+0000be90: 5265 7175 6972 656d 656e 7420 7c20 5965  Requirement | Ye
+0000bea0: 7320 207c 2059 6573 2020 2020 2020 2020  s  | Yes        
+0000beb0: 7c0a 0a49 6e20 6164 6469 7469 6f6e 2c20  |..In addition, 
+0000bec0: 2a2a 5461 736b 732a 2a20 6465 6669 6e65  **Tasks** define
+0000bed0: 6420 696e 204a 534f 4e20 646f 6375 6d65  d in JSON docume
+0000bee0: 6e74 7320 6361 6e20 7573 6520 616e 7920  nts can use any 
+0000bef0: 6f66 2074 6865 2073 7562 7374 6974 7574  of the substitut
+0000bf00: 696f 6e73 2061 626f 7665 2069 6e20 616e  ions above in an
+0000bf10: 7920 6f66 2074 6865 6972 2070 726f 7065  y of their prope
+0000bf20: 7274 6965 732c 206e 6f74 206a 7573 7420  rties, not just 
+0000bf30: 606e 616d 6560 2e0a 0a4e 756d 6265 7273  `name`...Numbers
+0000bf40: 2061 7265 207a 6572 6f2d 7061 6464 6564   are zero-padded
+0000bf50: 2066 6f72 206e 6561 7420 666f 726d 6174   for neat format
+0000bf60: 7469 6e67 2061 6e64 2073 6f72 7469 6e67  ting and sorting
+0000bf70: 2c20 652e 672e 2c20 5461 736b 206e 756d  , e.g., Task num
+0000bf80: 6265 7220 6033 3760 206f 6620 6031 3030  ber `37` of `100
+0000bf90: 3060 2054 6173 6b73 2077 6f75 6c64 2062  0` Tasks would b
+0000bfa0: 6520 7375 6273 7469 7475 7465 6420 6173  e substituted as
+0000bfb0: 2060 3030 3337 602e 0a0a 4173 2061 6e20   `0037`...As an 
+0000bfc0: 6578 616d 706c 652c 2074 6865 2066 6f6c  example, the fol
+0000bfd0: 6c6f 7769 6e67 204a 534f 4e20 576f 726b  lowing JSON Work
+0000bfe0: 2052 6571 7569 7265 6d65 6e74 3a0a 0a60   Requirement:..`
+0000bff0: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
+0000c000: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+0000c010: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
+0000c020: 6d79 5f74 6173 6b5f 6772 6f75 705f 7b7b  my_task_group_{{
+0000c030: 7461 736b 5f67 726f 7570 5f6e 756d 6265  task_group_numbe
+0000c040: 727d 7d5f 6131 222c 0a20 2020 2020 2022  r}}_a1",.      "
+0000c050: 6578 6563 7574 6162 6c65 223a 2022 6578  executable": "ex
+0000c060: 312e 7368 222c 0a20 2020 2020 2022 7461  1.sh",.      "ta
+0000c070: 736b 436f 756e 7422 3a20 322c 0a20 2020  skCount": 2,.   
+0000c080: 2020 2022 7461 736b 7322 3a20 5b0a 2020     "tasks": [.  
+0000c090: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0000c0a0: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
+0000c0b0: 736b 5f7b 7b74 6173 6b5f 6e75 6d62 6572  sk_{{task_number
+0000c0c0: 7d7d 2d6f 662d 7b7b 7461 736b 5f63 6f75  }}-of-{{task_cou
+0000c0d0: 6e74 7d7d 222c 0a20 2020 2020 2020 2020  nt}}",.         
+0000c0e0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+0000c0f0: 7b22 5441 534b 5f4e 554d 4245 5222 3a20  {"TASK_NUMBER": 
+0000c100: 227b 7b74 6173 6b5f 6e75 6d62 6572 7d7d  "{{task_number}}
+0000c110: 227d 0a20 2020 2020 2020 207d 0a20 2020  "}.        }.   
+0000c120: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
+0000c130: 7b0a 2020 2020 2020 226e 616d 6522 3a20  {.      "name": 
+0000c140: 226d 795f 7461 736b 5f67 726f 7570 5f7b  "my_task_group_{
+0000c150: 7b74 6173 6b5f 6772 6f75 705f 6e75 6d62  {task_group_numb
+0000c160: 6572 7d7d 5f62 3122 2c0a 2020 2020 2020  er}}_b1",.      
+0000c170: 2265 7865 6375 7461 626c 6522 3a20 2265  "executable": "e
+0000c180: 7832 2e73 6822 2c0a 2020 2020 2020 2274  x2.sh",.      "t
+0000c190: 6173 6b43 6f75 6e74 223a 2032 2c0a 2020  askCount": 2,.  
+0000c1a0: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
+0000c1b0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000c1c0: 2020 2022 6e61 6d65 223a 2022 6d79 5f74     "name": "my_t
+0000c1d0: 6173 6b5f 7b7b 7461 736b 5f6e 756d 6265  ask_{{task_numbe
+0000c1e0: 727d 7d2d 6f66 2d7b 7b74 6173 6b5f 636f  r}}-of-{{task_co
+0000c1f0: 756e 747d 7d22 0a20 2020 2020 2020 207d  unt}}".        }
+0000c200: 0a20 2020 2020 205d 0a20 2020 207d 0a20  .      ].    }. 
+0000c210: 205d 0a7d 0a60 6060 0a0a 2e2e 2e20 776f   ].}.```..... wo
+0000c220: 756c 6420 6372 6561 7465 2054 6173 6b20  uld create Task 
+0000c230: 4772 6f75 7073 206e 616d 6564 2060 6d79  Groups named `my
+0000c240: 5f74 6173 6b5f 6772 6f75 705f 315f 6131  _task_group_1_a1
+0000c250: 6020 616e 6420 606d 795f 7461 736b 5f67  ` and `my_task_g
+0000c260: 726f 7570 5f32 5f62 3160 2c20 6561 6368  roup_2_b1`, each
+0000c270: 2063 6f6e 7461 696e 696e 6720 5461 736b   containing Task
+0000c280: 7320 6e61 6d65 6420 606d 795f 7461 736b  s named `my_task
+0000c290: 5f31 2d6f 662d 3260 2c20 606d 795f 7461  _1-of-2`, `my_ta
+0000c2a0: 736b 5f32 2d6f 662d 3260 2e0a 0a23 2323  sk_2-of-2`...###
+0000c2b0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000c2c0: 7420 4e61 6d65 2053 7562 7374 6974 7574  t Name Substitut
+0000c2d0: 696f 6e0a 0a54 6865 206e 616d 6520 6f66  ion..The name of
+0000c2e0: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+0000c2f0: 656d 656e 7420 6974 7365 6c66 2063 616e  ement itself can
+0000c300: 2062 6520 7573 6564 2076 6961 2074 6865   be used via the
+0000c310: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+0000c320: 7475 7469 6f6e 2060 7b7b 7772 5f6e 616d  tution `{{wr_nam
+0000c330: 657d 7d60 2e20 5468 6973 2063 616e 2062  e}}`. This can b
+0000c340: 6520 7573 6564 2061 6e79 7768 6572 6520  e used anywhere 
+0000c350: 696e 2061 2054 4f4d 4c20 636f 6e66 6967  in a TOML config
+0000c360: 7572 6174 696f 6e20 6669 6c65 206f 7220  uration file or 
+0000c370: 696e 2061 204a 534f 4e20 576f 726b 2052  in a JSON Work R
+0000c380: 6571 7569 7265 6d65 6e74 2e0a 0a23 2320  equirement...## 
+0000c390: 4472 792d 5275 6e6e 696e 6720 576f 726b  Dry-Running Work
+0000c3a0: 2052 6571 7569 7265 6d65 6e74 2053 7562   Requirement Sub
+0000c3b0: 6d69 7373 696f 6e73 0a0a 546f 2065 7861  missions..To exa
+0000c3c0: 6d69 6e65 2074 6865 204a 534f 4e20 7468  mine the JSON th
+0000c3d0: 6174 2077 696c 6c20 6163 7475 616c 6c79  at will actually
+0000c3e0: 2062 6520 7365 6e74 2074 6f20 7468 6520   be sent to the 
+0000c3f0: 5965 6c6c 6f77 446f 6720 4150 4920 6166  YellowDog API af
+0000c400: 7465 7220 616c 6c20 7072 6f63 6573 7369  ter all processi
+0000c410: 6e67 2c20 7573 6520 7468 6520 602d 2d64  ng, use the `--d
+0000c420: 7279 2d72 756e 6020 636f 6d6d 616e 6420  ry-run` command 
+0000c430: 6c69 6e65 206f 7074 696f 6e20 7768 656e  line option when
+0000c440: 2072 756e 6e69 6e67 2060 7964 2d73 7562   running `yd-sub
+0000c450: 6d69 7460 2e20 5468 6973 2077 696c 6c20  mit`. This will 
+0000c460: 7072 696e 7420 7468 6520 6675 6c6c 7920  print the fully 
+0000c470: 7072 6f63 6573 7365 6420 4a53 4f4e 2066  processed JSON f
+0000c480: 6f72 2074 6865 2057 6f72 6b20 5265 7175  or the Work Requ
+0000c490: 6972 656d 656e 742e 204e 6f74 6869 6e67  irement. Nothing
+0000c4a0: 2077 696c 6c20 6265 2073 7562 6d69 7474   will be submitt
+0000c4b0: 6564 2074 6f20 7468 6520 506c 6174 666f  ed to the Platfo
+0000c4c0: 726d 2e0a 0a54 6865 2064 7279 2d72 756e  rm...The dry-run
+0000c4d0: 2069 7320 7573 6566 756c 2066 6f72 2069   is useful for i
+0000c4e0: 6e73 7065 6374 696e 6720 7468 6520 7265  nspecting the re
+0000c4f0: 7375 6c74 7320 6f66 2061 6c6c 2074 6865  sults of all the
+0000c500: 2070 726f 6365 7373 696e 6720 7468 6174   processing that
+0000c510: 2773 2062 6565 6e20 7065 7266 6f72 6d65  's been performe
+0000c520: 642e 2054 6f20 7375 7070 7265 7373 2061  d. To suppress a
+0000c530: 6c6c 206f 7574 7075 7420 6578 6365 7074  ll output except
+0000c540: 2066 6f72 2074 6865 204a 534f 4e20 6974   for the JSON it
+0000c550: 7365 6c66 2c20 7573 6520 7468 6520 602d  self, use the `-
+0000c560: 2d71 7569 6574 6020 2860 2d71 6029 2063  -quiet` (`-q`) c
+0000c570: 6f6d 6d61 6e64 206c 696e 6520 6f70 7469  ommand line opti
+0000c580: 6f6e 2e0a 0a4e 6f74 6520 7468 6174 2074  on...Note that t
+0000c590: 6865 2067 656e 6572 6174 6564 204a 534f  he generated JSO
+0000c5a0: 4e20 6973 2061 2063 6f6e 736f 6c69 6461  N is a consolida
+0000c5b0: 7465 6420 666f 726d 206f 6620 7768 6174  ted form of what
+0000c5c0: 2077 6f75 6c64 2062 6520 7375 626d 6974   would be submit
+0000c5d0: 7465 6420 746f 2074 6865 2059 656c 6c6f  ted to the Yello
+0000c5e0: 7744 6f67 2041 5049 2c20 616e 6420 5461  wDog API, and Ta
+0000c5f0: 736b 7320 6172 6520 6465 6669 6e65 6420  sks are defined 
+0000c600: 6469 7265 6374 6c79 2077 6974 6869 6e20  directly within 
+0000c610: 7468 6569 7220 5461 736b 2047 726f 7570  their Task Group
+0000c620: 7320 666f 7220 6561 7365 206f 6620 636f  s for ease of co
+0000c630: 6d70 7265 6865 6e73 696f 6e2e 2049 6e20  mprehension. In 
+0000c640: 6163 7475 616c 2041 5049 2073 7562 6d69  actual API submi
+0000c650: 7373 696f 6e73 2c20 7468 6520 576f 726b  ssions, the Work
+0000c660: 2052 6571 7569 7265 6d65 6e74 2077 6974   Requirement wit
+0000c670: 6820 6974 7320 5461 736b 2047 726f 7570  h its Task Group
+0000c680: 7320 6973 2073 7562 6d69 7474 6564 2066  s is submitted f
+0000c690: 6972 7374 2c20 616e 6420 5461 736b 7320  irst, and Tasks 
+0000c6a0: 6172 6520 7468 656e 2061 6464 6564 2074  are then added t
+0000c6b0: 6f20 5461 736b 2047 726f 7570 7320 7365  o Task Groups se
+0000c6c0: 7061 7261 7465 6c79 2069 6e20 7375 6273  parately in subs
+0000c6d0: 6571 7565 6e74 2041 5049 2063 616c 6c73  equent API calls
+0000c6e0: 2e0a 0a41 2073 696d 706c 6520 6578 616d  ...A simple exam
+0000c6f0: 706c 6520 6f66 2074 6865 204a 534f 4e20  ple of the JSON 
+0000c700: 6f75 7470 7574 2069 7320 7368 6f77 6e20  output is shown 
+0000c710: 6265 6c6f 772c 2073 686f 7769 6e67 2061  below, showing a
+0000c720: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000c730: 7420 7769 7468 2061 2073 696e 676c 6520  t with a single 
+0000c740: 5461 736b 2047 726f 7570 2c20 636f 6e74  Task Group, cont
+0000c750: 6169 6e69 6e67 2061 2073 696e 676c 6520  aining a single 
+0000c760: 5461 736b 2e0a 0a60 2520 7964 2d73 7562  Task...`% yd-sub
+0000c770: 6d69 7420 2d2d 6472 792d 7275 6e20 2d2d  mit --dry-run --
+0000c780: 7175 6965 7460 0a60 6060 6a73 6f6e 0a7b  quiet`.```json.{
+0000c790: 0a20 2022 6675 6c66 696c 4f6e 5375 626d  .  "fulfilOnSubm
+0000c7a0: 6974 223a 2066 616c 7365 2c0a 2020 226e  it": false,.  "n
+0000c7b0: 616d 6522 3a20 2270 7965 782d 6261 7368  ame": "pyex-bash
+0000c7c0: 5f32 3330 3131 342d 3039 3535 3034 2d35  _230114-095504-5
+0000c7d0: 3361 222c 0a20 2022 6e61 6d65 7370 6163  3a",.  "namespac
+0000c7e0: 6522 3a20 2270 7965 7861 6d70 6c65 7322  e": "pyexamples"
+0000c7f0: 2c0a 2020 2270 7269 6f72 6974 7922 3a20  ,.  "priority": 
+0000c800: 302c 0a20 2022 7461 6722 3a20 2270 7965  0,.  "tag": "pye
+0000c810: 782d 6261 7368 222c 0a20 2022 7461 736b  x-bash",.  "task
+0000c820: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+0000c830: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
+0000c840: 416c 6c54 6173 6b73 4669 6e69 7368 6564  AllTasksFinished
+0000c850: 223a 2074 7275 652c 0a20 2020 2020 2022  ": true,.      "
+0000c860: 6669 6e69 7368 4966 416e 7954 6173 6b46  finishIfAnyTaskF
+0000c870: 6169 6c65 6422 3a20 6661 6c73 652c 0a20  ailed": false,. 
+0000c880: 2020 2020 2022 6e61 6d65 223a 2022 7461       "name": "ta
+0000c890: 736b 5f67 726f 7570 5f31 222c 0a20 2020  sk_group_1",.   
+0000c8a0: 2020 2022 7072 696f 7269 7479 223a 2030     "priority": 0
+0000c8b0: 2c0a 2020 2020 2020 2272 756e 5370 6563  ,.      "runSpec
+0000c8c0: 6966 6963 6174 696f 6e22 3a20 7b0a 2020  ification": {.  
+0000c8d0: 2020 2020 2020 226d 6178 696d 756d 5461        "maximumTa
+0000c8e0: 736b 5265 7472 6965 7322 3a20 302c 0a20  skRetries": 0,. 
+0000c8f0: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+0000c900: 7322 3a20 5b22 6261 7368 225d 2c0a 2020  s": ["bash"],.  
+0000c910: 2020 2020 2020 2277 6f72 6b65 7254 6167        "workerTag
+0000c920: 7322 3a20 5b22 7079 6578 2d62 6173 6822  s": ["pyex-bash"
+0000c930: 5d0a 2020 2020 2020 7d2c 0a20 2020 2020  ].      },.     
+0000c940: 2022 7461 736b 7322 3a20 5b0a 2020 2020   "tasks": [.    
+0000c950: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000c960: 2261 7267 756d 656e 7473 223a 205b 2270  "arguments": ["p
+0000c970: 7965 782d 6261 7368 5f32 3330 3131 342d  yex-bash_230114-
+0000c980: 3039 3535 3034 2d35 3361 2f73 6c65 6570  095504-53a/sleep
+0000c990: 5f73 6372 6970 742e 7368 225d 2c0a 2020  _script.sh"],.  
+0000c9a0: 2020 2020 2020 2020 2265 6e76 6972 6f6e          "environ
+0000c9b0: 6d65 6e74 223a 207b 7d2c 0a20 2020 2020  ment": {},.     
+0000c9c0: 2020 2020 2022 696e 7075 7473 223a 205b       "inputs": [
+0000c9d0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+0000c9e0: 2020 2020 2020 2020 2020 2020 2022 6f62               "ob
+0000c9f0: 6a65 6374 4e61 6d65 5061 7474 6572 6e22  jectNamePattern"
+0000ca00: 3a20 2270 7965 782d 6261 7368 5f32 3330  : "pyex-bash_230
+0000ca10: 3131 342d 3039 3535 3034 2d35 3361 2f73  114-095504-53a/s
+0000ca20: 6c65 6570 5f73 6372 6970 742e 7368 222c  leep_script.sh",
+0000ca30: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+0000ca40: 736f 7572 6365 223a 2022 5441 534b 5f4e  source": "TASK_N
+0000ca50: 414d 4553 5041 4345 222c 0a20 2020 2020  AMESPACE",.     
+0000ca60: 2020 2020 2020 2020 2022 7665 7269 6669           "verifi
+0000ca70: 6361 7469 6f6e 223a 2022 5645 5249 4659  cation": "VERIFY
+0000ca80: 5f57 4149 5422 0a20 2020 2020 2020 2020  _WAIT".         
+0000ca90: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
+0000caa0: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
+0000cab0: 6522 3a20 2274 6173 6b5f 3031 222c 0a20  e": "task_01",. 
+0000cac0: 2020 2020 2020 2020 2022 6f75 7470 7574           "output
+0000cad0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+0000cae0: 2020 7b22 616c 7761 7973 5570 6c6f 6164    {"alwaysUpload
+0000caf0: 223a 2074 7275 652c 2022 7265 7175 6972  ": true, "requir
+0000cb00: 6564 223a 2066 616c 7365 2c20 2273 6f75  ed": false, "sou
+0000cb10: 7263 6522 3a20 2250 524f 4345 5353 5f4f  rce": "PROCESS_O
+0000cb20: 5554 5055 5422 7d0a 2020 2020 2020 2020  UTPUT"}.        
+0000cb30: 2020 5d2c 0a20 2020 2020 2020 2020 2022    ],.          "
+0000cb40: 7461 736b 5479 7065 223a 2022 6261 7368  taskType": "bash
+0000cb50: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
+0000cb60: 2020 5d0a 2020 2020 7d0a 2020 5d0a 7d0a    ].    }.  ].}.
+0000cb70: 6060 600a 0a23 2323 2053 7562 6d69 7474  ```..### Submitt
+0000cb80: 696e 6720 2752 6177 2720 4a53 4f4e 2057  ing 'Raw' JSON W
+0000cb90: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000cba0: 5370 6563 6966 6963 6174 696f 6e73 0a0a  Specifications..
+0000cbb0: 4974 2773 2070 6f73 7369 626c 6520 746f  It's possible to
+0000cbc0: 2075 7365 2074 6865 204a 534f 4e20 6f75   use the JSON ou
+0000cbd0: 7470 7574 206f 6620 6079 642d 7375 626d  tput of `yd-subm
+0000cbe0: 6974 202d 2d64 7279 2d72 756e 6020 2873  it --dry-run` (s
+0000cbf0: 7563 6820 6173 2074 6865 2065 7861 6d70  uch as the examp
+0000cc00: 6c65 2061 626f 7665 2920 6173 2061 2073  le above) as a s
+0000cc10: 656c 662d 636f 6e74 6169 6e65 642c 2066  elf-contained, f
+0000cc20: 756c 6c79 2d73 7065 6369 6669 6564 2057  ully-specified W
+0000cc30: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000cc40: 7370 6563 6966 6963 6174 696f 6e2c 2075  specification, u
+0000cc50: 7369 6e67 2074 6865 2060 2d2d 6a73 6f6e  sing the `--json
+0000cc60: 2d72 6177 6020 286f 7220 602d 6a60 2920  -raw` (or `-j`) 
+0000cc70: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
+0000cc80: 696f 6e2c 2069 2e65 2e3a 2060 7964 2d73  ion, i.e.: `yd-s
+0000cc90: 7562 6d69 7420 2d2d 6a73 6f6e 2d72 6177  ubmit --json-raw
+0000cca0: 203c 6669 6c65 6e61 6d65 2e6a 736f 6e3e   <filename.json>
+0000ccb0: 602e 0a0a 5468 6973 2077 696c 6c20 7375  `...This will su
+0000ccc0: 626d 6974 2074 6865 2057 6f72 6b20 5265  bmit the Work Re
+0000ccd0: 7175 6972 656d 656e 742c 2074 6865 6e20  quirement, then 
+0000cce0: 6164 6420 616c 6c20 7468 6520 7370 6563  add all the spec
+0000ccf0: 6966 6965 6420 5461 736b 732e 0a0a 4e6f  ified Tasks...No
+0000cd00: 7465 2074 6861 7420 7661 7269 6162 6c65  te that variable
+0000cd10: 2073 7562 7374 6974 7574 696f 6e73 202a   substitutions *
+0000cd20: 2a63 616e 2a2a 2062 6520 7573 6564 2069  *can** be used i
+0000cd30: 6e20 7468 6520 7261 7720 4a53 4f4e 2066  n the raw JSON f
+0000cd40: 696c 652c 206a 7573 7420 6173 2069 6e20  ile, just as in 
+0000cd50: 7468 6520 6f74 6865 7220 576f 726b 2052  the other Work R
+0000cd60: 6571 7569 7265 6d65 6e74 204a 534f 4e20  equirement JSON 
+0000cd70: 6578 616d 706c 6573 2c20 6275 7420 7468  examples, but th
+0000cd80: 6572 6520 6973 206e 6f20 7072 6f70 6572  ere is no proper
+0000cd90: 7479 2069 6e68 6572 6974 616e 6365 2c20  ty inheritance, 
+0000cda0: 696e 636c 7564 696e 6720 6672 6f6d 2074  including from t
+0000cdb0: 6865 2060 5b77 6f72 6b52 6571 7569 7265  he `[workRequire
+0000cdc0: 6d65 6e74 5d60 2073 6563 7469 6f6e 206f  ment]` section o
+0000cdd0: 6620 7468 6520 544f 4d4c 2063 6f6e 6669  f the TOML confi
+0000cde0: 6775 7261 7469 6f6e 206f 7220 6672 6f6d  guration or from
+0000cdf0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000ce00: 7420 7072 6f70 6572 7469 6573 2073 7570  t properties sup
+0000ce10: 706c 6965 6420 6f6e 2074 6865 2063 6f6d  plied on the com
+0000ce20: 6d61 6e64 206c 696e 652e 0a0a 4e6f 7465  mand line...Note
+0000ce30: 2074 6861 7420 7468 6572 6520 6973 206e   that there is n
+0000ce40: 6f20 6175 746f 6d61 7469 6320 6669 6c65  o automatic file
+0000ce50: 2075 706c 6f61 6420 7768 656e 2075 7369   upload when usi
+0000ce60: 6e67 2074 6869 7320 6f70 7469 6f6e 2c20  ng this option, 
+0000ce70: 736f 2061 6e79 2066 696c 6573 2072 6571  so any files req
+0000ce80: 7569 7265 6420 6174 2074 6865 2073 7461  uired at the sta
+0000ce90: 7274 206f 6620 7468 6520 7461 736b 2028  rt of the task (
+0000cea0: 7370 6563 6966 6965 6420 7573 696e 6720  specified using 
+0000ceb0: 6056 4552 4946 595f 4154 5f53 5441 5254  `VERIFY_AT_START
+0000cec0: 6029 206d 7573 7420 6265 2070 7265 7365  `) must be prese
+0000ced0: 6e74 2062 6566 6f72 6520 7468 6520 5461  nt before the Ta
+0000cee0: 736b 7320 6172 6520 7570 6c6f 6164 6564  sks are uploaded
+0000cef0: 2c20 6f72 2074 6865 2054 6173 6b73 2077  , or the Tasks w
+0000cf00: 696c 6c20 6661 696c 2069 6d6d 6564 6961  ill fail immedia
+0000cf10: 7465 6c79 2e20 5468 6520 6079 642d 7570  tely. The `yd-up
+0000cf20: 6c6f 6164 6020 636f 6d6d 616e 6420 6361  load` command ca
+0000cf30: 6e20 6265 2075 7365 6420 746f 2075 706c  n be used to upl
+0000cf40: 6f61 6420 7468 6573 6520 6669 6c65 732c  oad these files,
+0000cf50: 2061 6e64 2060 7964 2d73 7562 6d69 7460   and `yd-submit`
+0000cf60: 2077 696c 6c20 7061 7573 6520 746f 2061   will pause to a
+0000cf70: 6c6c 6f77 2074 6869 7320 746f 2068 6170  llow this to hap
+0000cf80: 7065 6e2e 0a0a 2323 2046 696c 6520 5374  pen...## File St
+0000cf90: 6f72 6167 6520 4c6f 6361 7469 6f6e 7320  orage Locations 
+0000cfa0: 616e 6420 4669 6c65 2055 7361 6765 0a0a  and File Usage..
+0000cfb0: 5468 6973 2073 6563 7469 6f6e 2064 6973  This section dis
+0000cfc0: 6375 7373 6573 2068 6f77 2074 6f20 7570  cusses how to up
+0000cfd0: 6c6f 6164 2066 696c 6573 2066 726f 6d20  load files from 
+0000cfe0: 6c6f 6361 6c20 7374 6f72 6167 6520 746f  local storage to
+0000cff0: 2074 6865 2059 656c 6c6f 7744 6f67 204f   the YellowDog O
+0000d000: 626a 6563 7420 5374 6f72 652c 2068 6f77  bject Store, how
+0000d010: 2074 686f 7365 2066 696c 6573 2061 7265   those files are
+0000d020: 2074 7261 6e73 6665 7272 6564 2074 6f20   transferred to 
+0000d030: 576f 726b 6572 204e 6f64 6573 2066 6f72  Worker Nodes for
+0000d040: 2054 6173 6b20 7072 6f63 6573 7369 6e67   Task processing
+0000d050: 2c20 686f 7720 7468 6520 7265 7375 6c74  , how the result
+0000d060: 7320 6f66 2054 6173 6b20 7072 6f63 6573  s of Task proces
+0000d070: 7369 6e67 2061 7265 2072 6574 7572 6e65  sing are returne
+0000d080: 6420 6279 2057 6f72 6b65 7220 4e6f 6465  d by Worker Node
+0000d090: 732c 2061 6e64 2068 6f77 2066 696c 6573  s, and how files
+0000d0a0: 2061 7265 2074 7261 6e73 6665 7272 6564   are transferred
+0000d0b0: 2062 6163 6b20 6672 6f6d 2074 6865 2059   back from the Y
+0000d0c0: 656c 6c6f 7744 6f67 204f 626a 6563 7420  ellowDog Object 
+0000d0d0: 5374 6f72 6520 746f 206c 6f63 616c 2073  Store to local s
+0000d0e0: 746f 7261 6765 2e0a 0a23 2323 2046 696c  torage...### Fil
+0000d0f0: 6573 2055 706c 6f61 6465 6420 746f 2074  es Uploaded to t
+0000d100: 6865 204f 626a 6563 7420 5374 6f72 6520  he Object Store 
+0000d110: 6672 6f6d 204c 6f63 616c 2053 746f 7261  from Local Stora
+0000d120: 6765 0a0a 2323 2323 2046 696c 6573 2069  ge..#### Files i
+0000d130: 6e20 7468 6520 6069 6e70 7574 7360 204c  n the `inputs` L
+0000d140: 6973 740a 0a57 6865 6e20 6120 576f 726b  ist..When a Work
+0000d150: 2052 6571 7569 7265 6d65 6e74 2069 7320   Requirement is 
+0000d160: 7375 626d 6974 7465 6420 7573 696e 6720  submitted using 
+0000d170: 6079 642d 7375 626d 6974 602c 2066 696c  `yd-submit`, fil
+0000d180: 6573 2061 7265 2075 706c 6f61 6465 6420  es are uploaded 
+0000d190: 746f 2074 6865 2059 656c 6c6f 7744 6f67  to the YellowDog
+0000d1a0: 204f 626a 6563 7420 5374 6f72 6520 6966   Object Store if
+0000d1b0: 2074 6865 7927 7265 2069 6e63 6c75 6465   they're include
+0000d1c0: 6420 696e 2074 6865 206c 6973 7420 6f66  d in the list of
+0000d1d0: 2066 696c 6573 2069 6e20 7468 6520 6069   files in the `i
+0000d1e0: 6e70 7574 7360 2070 726f 7065 7274 792e  nputs` property.
+0000d1f0: 2028 466f 7220 7468 6520 6361 7365 206f   (For the case o
+0000d200: 6620 7468 6520 6062 6173 6860 2054 6173  f the `bash` Tas
+0000d210: 6b20 5479 7065 2c20 7468 6520 7363 7269  k Type, the scri
+0000d220: 7074 2073 7065 6369 6669 6564 2069 6e20  pt specified in 
+0000d230: 7468 6520 6065 7865 6375 7461 626c 6560  the `executable`
+0000d240: 2070 726f 7065 7274 7920 6973 2061 6c73   property is als
+0000d250: 6f20 6175 746f 6d61 7469 6361 6c6c 7920  o automatically 
+0000d260: 7570 6c6f 6164 6564 2061 7320 6120 636f  uploaded as a co
+0000d270: 6e76 656e 6965 6e63 652c 2065 7665 6e20  nvenience, even 
+0000d280: 6966 206e 6f74 2069 6e63 6c75 6465 6420  if not included 
+0000d290: 696e 2074 6865 2060 696e 7075 7473 6020  in the `inputs` 
+0000d2a0: 6c69 7374 2e29 0a0a 5468 6520 6069 6e70  list.)..The `inp
+0000d2b0: 7574 7360 2070 726f 7065 7274 7920 6163  uts` property ac
+0000d2c0: 6365 7074 7320 7769 6c64 6361 7264 2066  cepts wildcard f
+0000d2d0: 696c 656e 616d 6573 2c20 652e 672e 3a20  ilenames, e.g.: 
+0000d2e0: 605b 222a 2e73 6822 2c20 222a 2e74 7874  `["*.sh", "*.txt
+0000d2f0: 225d 602e 2054 6869 7320 6361 6e20 6265  "]`. This can be
+0000d300: 2075 7365 6420 746f 2061 6464 2074 6865   used to add the
+0000d310: 2063 6f6e 7465 6e74 7320 6f66 2064 6972   contents of dir
+0000d320: 6563 746f 7269 6573 2c20 652e 672e 3a20  ectories, e.g.: 
+0000d330: 605b 226d 795f 6469 722f 2a22 2c20 2264  `["my_dir/*", "d
+0000d340: 6174 612a 2f2a 225d 602e 0a0a 4669 6c65  ata*/*"]`...File
+0000d350: 7320 6172 6520 7570 6c6f 6164 6564 2074  s are uploaded t
+0000d360: 6f20 7468 6520 4e61 6d65 7370 6163 6520  o the Namespace 
+0000d370: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
+0000d380: 2063 6f6e 6669 6775 7261 7469 6f6e 2e20   configuration. 
+0000d390: 5769 7468 696e 2074 6865 204e 616d 6573  Within the Names
+0000d3a0: 7061 6365 2c20 6561 6368 2057 6f72 6b20  pace, each Work 
+0000d3b0: 5265 7175 6972 656d 656e 7420 6861 7320  Requirement has 
+0000d3c0: 6120 7365 7061 7261 7465 2066 6f6c 6465  a separate folde
+0000d3d0: 7220 7468 6174 2073 6861 7265 7320 7468  r that shares th
+0000d3e0: 6520 6e61 6d65 206f 6620 7468 6520 576f  e name of the Wo
+0000d3f0: 726b 2052 6571 7569 7265 6d65 6e74 2c20  rk Requirement, 
+0000d400: 616e 6420 696e 2077 6869 6368 2061 6c6c  and in which all
+0000d410: 2066 696c 6573 2072 656c 6174 6564 2074   files related t
+0000d420: 6f20 7468 6520 576f 726b 2052 6571 7569  o the Work Requi
+0000d430: 7265 6d65 6e74 2061 7265 2073 746f 7265  rement are store
+0000d440: 642e 0a0a 312e 2046 696c 6573 2074 6f20  d...1. Files to 
+0000d450: 6265 2075 706c 6f61 6465 6420 7468 6174  be uploaded that
+0000d460: 2061 7265 2069 6e20 7468 6520 2a2a 7361   are in the **sa
+0000d470: 6d65 2064 6972 6563 746f 7279 2061 7320  me directory as 
+0000d480: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+0000d490: 6d65 6e74 2073 7065 6369 6669 6361 7469  ment specificati
+0000d4a0: 6f6e 2a2a 2028 7468 6520 544f 4d4c 206f  on** (the TOML o
+0000d4b0: 7220 4a53 4f4e 2066 696c 6529 2061 7265  r JSON file) are
+0000d4c0: 2075 706c 6f61 6465 6420 746f 2074 6865   uploaded to the
+0000d4d0: 2072 6f6f 7420 6f66 2074 6865 2057 6f72   root of the Wor
+0000d4e0: 6b20 5265 7175 6972 656d 656e 7420 666f  k Requirement fo
+0000d4f0: 6c64 6572 2e0a 0a0a 322e 2046 696c 6573  lder....2. Files
+0000d500: 2074 6f20 6265 2075 706c 6f61 6465 6420   to be uploaded 
+0000d510: 7468 6174 2061 7265 2069 6e20 2a2a 7375  that are in **su
+0000d520: 6264 6972 6563 746f 7269 6573 2062 656c  bdirectories bel
+0000d530: 6f77 2074 6865 2057 6f72 6b20 5265 7175  ow the Work Requ
+0000d540: 6972 656d 656e 7420 7370 6563 6966 6963  irement specific
+0000d550: 6174 696f 6e2c 206f 7220 7768 6572 6520  ation, or where 
+0000d560: 6162 736f 6c75 7465 2070 6174 686e 616d  absolute pathnam
+0000d570: 6573 2061 7265 2073 7570 706c 6965 642a  es are supplied*
+0000d580: 2a20 6172 6520 706c 6163 6564 2069 6e20  * are placed in 
+0000d590: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+0000d5a0: 2069 6e20 6469 7265 6374 6f72 6965 7320   in directories 
+0000d5b0: 7468 6174 206d 6972 726f 7220 7468 6569  that mirror thei
+0000d5c0: 7220 6c6f 6361 6c20 7374 6f72 6167 6520  r local storage 
+0000d5d0: 6c6f 6361 7469 6f6e 732e 0a0a 0a33 2e20  locations....3. 
+0000d5e0: 4669 6c65 7320 746f 2062 6520 7570 6c6f  Files to be uplo
+0000d5f0: 6164 6564 2074 6861 7420 6172 6520 696e  aded that are in
+0000d600: 202a 2a64 6972 6563 746f 7269 6573 2072   **directories r
+0000d610: 656c 6174 6976 6520 746f 2074 6865 2057  elative to the W
+0000d620: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000d630: 7370 6563 6966 6963 6174 696f 6e2c 2075  specification, u
+0000d640: 7369 6e67 2060 2e2e 6020 7265 6c61 7469  sing `..` relati
+0000d650: 7665 2070 6174 6873 2a2a 2061 7265 2070  ve paths** are p
+0000d660: 6c61 6365 6420 696e 204f 626a 6563 7420  laced in Object 
+0000d670: 5374 6f72 6520 6469 7265 6374 6f72 6965  Store directorie
+0000d680: 7320 696e 2077 6869 6368 2074 6865 2060  s in which the `
+0000d690: 2e2e 6020 7061 7274 7320 6f66 2074 6865  ..` parts of the
+0000d6a0: 2070 6174 686e 616d 6520 6172 6520 7265   pathname are re
+0000d6b0: 706c 6163 6564 2077 6974 6820 616e 2069  placed with an i
+0000d6c0: 6e74 6567 6572 2063 6f75 6e74 206f 6620  nteger count of 
+0000d6d0: 7468 6520 6e75 6d62 6572 206f 6620 602e  the number of `.
+0000d6e0: 2e60 2065 6e74 7269 6573 2028 6265 6361  .` entries (beca
+0000d6f0: 7573 6520 7765 2063 616e 2774 2075 7365  use we can't use
+0000d700: 2074 6865 2060 2e2e 6020 7265 6c61 7469   the `..` relati
+0000d710: 7665 2066 6f72 6d20 696e 2074 6865 204f  ve form in the O
+0000d720: 626a 6563 7420 5374 6f72 6529 2e0a 0a41  bject Store)...A
+0000d730: 7373 756d 696e 6720 6120 4e61 6d65 7370  ssuming a Namesp
+0000d740: 6163 6520 6361 6c6c 6564 2060 6465 7665  ace called `deve
+0000d750: 6c6f 706d 656e 7460 2061 6e64 2061 2057  lopment` and a W
+0000d760: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000d770: 6e61 6d65 6420 6074 6573 7472 756e 5f32  named `testrun_2
+0000d780: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
+0000d790: 602c 2074 6865 2066 6f6c 6c6f 7769 6e67  `, the following
+0000d7a0: 206c 6f63 6174 696f 6e73 2061 7265 2075   locations are u
+0000d7b0: 7365 6420 7768 656e 2075 706c 6f61 6469  sed when uploadi
+0000d7c0: 6e67 2066 696c 6573 2066 6f6c 6c6f 7769  ng files followi
+0000d7d0: 6e67 2074 6865 2070 6174 7465 726e 7320  ng the patterns 
+0000d7e0: 6162 6f76 653a 0a0a 6060 6073 6865 6c6c  above:..```shell
+0000d7f0: 0a22 696e 7075 7473 2220 3a20 5b22 6669  ."inputs" : ["fi
+0000d800: 6c65 5f31 2e74 7874 225d 202d 3e20 6465  le_1.txt"] -> de
+0000d810: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
+0000d820: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000d830: 2d37 6432 2f66 696c 655f 312e 7478 740a  -7d2/file_1.txt.
+0000d840: 2269 6e70 7574 7322 203a 205b 2264 6576  "inputs" : ["dev
+0000d850: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
+0000d860: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
+0000d870: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
+0000d880: 3430 342d 3764 322f 6465 762f 6669 6c65  404-7d2/dev/file
+0000d890: 5f31 2e74 7874 0a22 696e 7075 7473 2220  _1.txt."inputs" 
+0000d8a0: 3a20 5b22 2f68 6f6d 652f 6465 762f 6669  : ["/home/dev/fi
+0000d8b0: 6c65 5f31 2e74 7874 225d 202d 3e20 6465  le_1.txt"] -> de
+0000d8c0: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
+0000d8d0: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000d8e0: 2d37 6432 2f68 6f6d 652f 6465 762f 6669  -7d2/home/dev/fi
+0000d8f0: 6c65 5f31 2e74 7874 0a22 696e 7075 7473  le_1.txt."inputs
+0000d900: 2220 3a20 5b22 2e2e 2f64 6576 2f66 696c  " : ["../dev/fil
+0000d910: 655f 312e 7478 7422 5d20 2d3e 2064 6576  e_1.txt"] -> dev
+0000d920: 656c 6f70 6d65 6e74 3a3a 7465 7374 7275  elopment::testru
+0000d930: 6e5f 3232 3131 3038 2d31 3230 3430 342d  n_221108-120404-
+0000d940: 3764 322f 312f 6465 762f 6669 6c65 5f31  7d2/1/dev/file_1
+0000d950: 2e74 7874 0a22 696e 7075 7473 2220 3a20  .txt."inputs" : 
+0000d960: 5b22 2e2e 2f2e 2e2f 6465 762f 6669 6c65  ["../../dev/file
+0000d970: 5f31 2e74 7874 225d 202d 3e20 6465 7665  _1.txt"] -> deve
+0000d980: 6c6f 706d 656e 743a 3a74 6573 7472 756e  lopment::testrun
+0000d990: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
+0000d9a0: 6432 2f32 2f64 6576 2f66 696c 655f 312e  d2/2/dev/file_1.
+0000d9b0: 7478 740a 6060 600a 0a2a 2a55 7369 6e67  txt.```..**Using
+0000d9c0: 2060 666c 6174 7465 6e55 706c 6f61 6450   `flattenUploadP
+0000d9d0: 6174 6873 602a 2a0a 0a54 6865 2060 666c  aths`**..The `fl
+0000d9e0: 6174 7465 6e55 706c 6f61 6450 6174 6873  attenUploadPaths
+0000d9f0: 6020 7072 6f70 6572 7479 2063 616e 2062  ` property can b
+0000da00: 6520 7573 6564 2074 6f20 7375 7070 7265  e used to suppre
+0000da10: 7373 2074 6865 206d 6972 726f 7269 6e67  ss the mirroring
+0000da20: 206f 6620 616e 7920 6c6f 6361 6c20 6469   of any local di
+0000da30: 7265 6374 6f72 7920 7374 7275 6374 7572  rectory structur
+0000da40: 6520 7768 656e 2075 706c 6f61 6469 6e67  e when uploading
+0000da50: 2066 696c 6573 2074 6f20 7468 6520 4f62   files to the Ob
+0000da60: 6a65 6374 2053 746f 7265 2e20 4966 2073  ject Store. If s
+0000da70: 6574 2074 6f20 6074 7275 6560 2c20 616c  et to `true`, al
+0000da80: 6c20 6669 6c65 7320 7769 6c6c 2062 6520  l files will be 
+0000da90: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
+0000daa0: 726f 6f74 206f 6620 7468 6520 576f 726b  root of the Work
+0000dab0: 2052 6571 7569 7265 6d65 6e74 2066 6f6c   Requirement fol
+0000dac0: 6465 722e 2046 6f72 2065 7861 6d70 6c65  der. For example
+0000dad0: 3a0a 0a60 6060 7368 656c 6c0a 2269 6e70  :..```shell."inp
+0000dae0: 7574 7322 203a 205b 2266 696c 655f 312e  uts" : ["file_1.
+0000daf0: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
+0000db00: 6d65 6e74 3a3a 7465 7374 7275 6e5f 3232  ment::testrun_22
+0000db10: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
+0000db20: 6669 6c65 5f31 2e74 7874 0a22 696e 7075  file_1.txt."inpu
+0000db30: 7473 2220 3a20 5b22 6465 762f 6669 6c65  ts" : ["dev/file
+0000db40: 5f31 2e74 7874 225d 202d 3e20 6465 7665  _1.txt"] -> deve
+0000db50: 6c6f 706d 656e 743a 3a74 6573 7472 756e  lopment::testrun
+0000db60: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
+0000db70: 6432 2f66 696c 655f 312e 7478 740a 2269  d2/file_1.txt."i
+0000db80: 6e70 7574 7322 203a 205b 222f 686f 6d65  nputs" : ["/home
+0000db90: 2f64 6576 2f66 696c 655f 312e 7478 7422  /dev/file_1.txt"
+0000dba0: 5d20 2d3e 2064 6576 656c 6f70 6d65 6e74  ] -> development
+0000dbb0: 3a3a 7465 7374 7275 6e5f 3232 3131 3038  ::testrun_221108
+0000dbc0: 2d31 3230 3430 342d 3764 322f 6669 6c65  -120404-7d2/file
+0000dbd0: 5f31 2e74 7874 0a22 696e 7075 7473 2220  _1.txt."inputs" 
+0000dbe0: 3a20 5b22 2e2e 2f64 6576 2f66 696c 655f  : ["../dev/file_
+0000dbf0: 312e 7478 7422 5d20 2d3e 2064 6576 656c  1.txt"] -> devel
+0000dc00: 6f70 6d65 6e74 3a3a 7465 7374 7275 6e5f  opment::testrun_
+0000dc10: 3232 3131 3038 2d31 3230 3430 342d 3764  221108-120404-7d
+0000dc20: 322f 6669 6c65 5f31 2e74 7874 0a22 696e  2/file_1.txt."in
+0000dc30: 7075 7473 2220 3a20 5b22 2e2e 2f2e 2e2f  puts" : ["../../
+0000dc40: 6465 762f 6669 6c65 5f31 2e74 7874 225d  dev/file_1.txt"]
+0000dc50: 202d 3e20 6465 7665 6c6f 706d 656e 743a   -> development:
+0000dc60: 3a74 6573 7472 756e 5f32 3231 3130 382d  :testrun_221108-
+0000dc70: 3132 3034 3034 2d37 6432 2f66 696c 655f  120404-7d2/file_
+0000dc80: 312e 7478 740a 6060 600a 0a54 6865 2070  1.txt.```..The p
+0000dc90: 726f 7065 7274 7920 6465 6661 756c 7420  roperty default 
+0000dca0: 6973 2060 6661 6c73 6560 2e20 5468 6973  is `false`. This
+0000dcb0: 2070 726f 7065 7274 7920 2a2a 6361 6e20   property **can 
+0000dcc0: 6f6e 6c79 2062 6520 7365 7420 6174 2074  only be set at t
+0000dcd0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+0000dce0: 656e 7420 6c65 7665 6c2a 2a20 616e 6420  ent level** and 
+0000dcf0: 7769 6c6c 2074 6865 7265 666f 7265 2061  will therefore a
+0000dd00: 7070 6c79 2074 6f20 616c 6c20 5461 736b  pply to all Task
+0000dd10: 2047 726f 7570 7320 616e 6420 5461 736b   Groups and Task
+0000dd20: 7320 7769 7468 696e 2061 2057 6f72 6b20  s within a Work 
+0000dd30: 5265 7175 6972 656d 656e 742e 0a0a 5768  Requirement...Wh
+0000dd40: 656e 2066 696c 6573 2061 7070 6561 7220  en files appear 
+0000dd50: 696e 2074 6865 2060 696e 7075 7473 6020  in the `inputs` 
+0000dd60: 6c69 7374 2c20 7468 6579 2061 7265 2061  list, they are a
+0000dd70: 6c73 6f20 6175 746f 6d61 7469 6361 6c6c  lso automaticall
+0000dd80: 7920 6164 6465 6420 746f 2074 6865 206c  y added to the l
+0000dd90: 6973 7420 6f66 2066 696c 6573 2072 6571  ist of files req
+0000dda0: 7569 7265 6420 6279 2074 6865 2072 656c  uired by the rel
+0000ddb0: 6576 616e 7420 5461 736b 2873 2920 6173  evant Task(s) as
+0000ddc0: 2060 5665 7269 6679 4174 5374 6172 7460   `VerifyAtStart`
+0000ddd0: 2064 6570 656e 6465 6e63 6965 732e 0a0a   dependencies...
+0000dde0: 2323 2323 2046 696c 6573 2069 6e20 7468  #### Files in th
+0000ddf0: 6520 6075 706c 6f61 6446 696c 6573 6020  e `uploadFiles` 
+0000de00: 4c69 7374 0a0a 5468 6520 6075 706c 6f61  List..The `uploa
+0000de10: 6446 696c 6573 6020 7072 6f70 6572 7479  dFiles` property
+0000de20: 2061 6c6c 6f77 7320 6d6f 7265 2066 6c65   allows more fle
+0000de30: 7869 626c 6520 636f 6e74 726f 6c20 6f76  xible control ov
+0000de40: 6572 2074 6865 2066 696c 6573 2074 6f20  er the files to 
+0000de50: 6265 2075 706c 6f61 6465 6420 6672 6f6d  be uploaded from
+0000de60: 206c 6f63 616c 2073 746f 7261 6765 2074   local storage t
+0000de70: 6f20 7468 6520 4f62 6a65 6374 2053 746f  o the Object Sto
+0000de80: 7265 2077 6865 6e20 6079 642d 7375 626d  re when `yd-subm
+0000de90: 6974 6020 6973 2072 756e 2e20 5468 6520  it` is run. The 
+0000dea0: 7072 6f70 6572 7479 2063 616e 2062 6520  property can be 
+0000deb0: 7573 6564 2061 7420 616c 6c20 576f 726b  used at all Work
+0000dec0: 2052 6571 7569 7265 6d65 6e74 206c 6576   Requirement lev
+0000ded0: 656c 732c 2066 726f 6d20 7468 6520 544f  els, from the TO
+0000dee0: 4d4c 2066 696c 6520 7468 726f 7567 6820  ML file through 
+0000def0: 746f 2069 6e64 6976 6964 7561 6c20 5461  to individual Ta
+0000df00: 736b 2073 7065 6369 6669 6361 7469 6f6e  sk specification
+0000df10: 732e 0a0a 5468 6520 7072 6f70 6572 7479  s...The property
+0000df20: 2069 7320 7375 7070 6c69 6564 2061 7320   is supplied as 
+0000df30: 6120 6c69 7374 206f 6620 6469 6374 696f  a list of dictio
+0000df40: 6e61 7279 2069 7465 6d73 2c20 6561 6368  nary items, each
+0000df50: 206f 6620 7768 6963 6820 6d75 7374 2069   of which must i
+0000df60: 6e63 6c75 6465 2074 6865 2070 726f 7065  nclude the prope
+0000df70: 7274 6965 7320 606c 6f63 616c 5061 7468  rties `localPath
+0000df80: 6020 616e 6420 6075 706c 6f61 6450 6174  ` and `uploadPat
+0000df90: 6860 2e20 0a0a 2d20 606c 6f63 616c 5061  h`. ..- `localPa
+0000dfa0: 7468 6020 7370 6563 6966 6965 7320 7468  th` specifies th
+0000dfb0: 6520 7061 7468 6e61 6d65 206f 6620 7468  e pathname of th
+0000dfc0: 6520 6669 6c65 206f 6e20 6c6f 6361 6c20  e file on local 
+0000dfd0: 7374 6f72 6167 650a 2d20 6075 706c 6f61  storage.- `uploa
+0000dfe0: 6450 6174 6860 2073 7065 6369 6669 6573  dPath` specifies
+0000dff0: 2074 6865 206e 616d 6520 616e 6420 6c6f   the name and lo
+0000e000: 6361 7469 6f6e 206f 6620 7468 6520 6669  cation of the fi
+0000e010: 6c65 2773 2064 6573 7469 6e61 7469 6f6e  le's destination
+0000e020: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
+0000e030: 746f 7265 0a0a 466f 7220 6578 616d 706c  tore..For exampl
+0000e040: 652c 2069 6e20 544f 4d4c 3a0a 6060 6074  e, in TOML:.```t
+0000e050: 6f6d 6c0a 7570 6c6f 6164 4669 6c65 7320  oml.uploadFiles 
+0000e060: 3d20 5b0a 2020 2020 7b6c 6f63 616c 5061  = [.    {localPa
+0000e070: 7468 203d 2022 6669 6c65 5f31 2e74 7874  th = "file_1.txt
+0000e080: 222c 2075 706c 6f61 6450 6174 6820 3d20  ", uploadPath = 
+0000e090: 2266 696c 655f 312e 7478 7422 7d2c 0a20  "file_1.txt"},. 
+0000e0a0: 2020 207b 6c6f 6361 6c50 6174 6820 3d20     {localPath = 
+0000e0b0: 2264 6972 5f32 2f66 696c 655f 322e 7478  "dir_2/file_2.tx
+0000e0c0: 7422 2c20 7570 6c6f 6164 5061 7468 203d  t", uploadPath =
+0000e0d0: 2022 3a3a 6669 6c65 5f32 2e74 7874 227d   "::file_2.txt"}
+0000e0e0: 2c0a 2020 2020 7b6c 6f63 616c 5061 7468  ,.    {localPath
+0000e0f0: 203d 2022 6669 6c65 5f33 2e74 7874 222c   = "file_3.txt",
+0000e100: 2075 706c 6f61 6450 6174 6820 3d20 226f   uploadPath = "o
+0000e110: 7468 6572 5f6e 616d 6573 7061 6365 3a3a  ther_namespace::
+0000e120: 6669 6c65 5f33 2e74 7874 227d 0a5d 0a60  file_3.txt"}.].`
+0000e130: 6060 0a41 6e64 2069 6e20 4a53 4f4e 2c20  ``.And in JSON, 
+0000e140: 7769 7468 2074 6865 2070 726f 7065 7274  with the propert
+0000e150: 7920 7365 7420 6174 2074 6865 2054 6173  y set at the Tas
+0000e160: 6b20 6c65 7665 6c2c 2074 6865 2073 616d  k level, the sam
+0000e170: 6520 7370 6563 6966 6963 6174 696f 6e20  e specification 
+0000e180: 776f 756c 6420 6265 3a0a 6060 606a 736f  would be:.```jso
+0000e190: 6e0a 7b0a 2020 2274 6173 6b47 726f 7570  n.{.  "taskGroup
+0000e1a0: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
+0000e1b0: 2020 2274 6173 6b73 223a 205b 0a20 2020    "tasks": [.   
+0000e1c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+0000e1d0: 2022 7570 6c6f 6164 4669 6c65 7322 3a20   "uploadFiles": 
+0000e1e0: 5b0a 2020 2020 2020 2020 2020 2020 7b22  [.            {"
+0000e1f0: 6c6f 6361 6c50 6174 6822 3a20 2266 696c  localPath": "fil
+0000e200: 655f 312e 7478 7422 2c20 2275 706c 6f61  e_1.txt", "uploa
+0000e210: 6450 6174 6822 3a20 2266 696c 655f 312e  dPath": "file_1.
+0000e220: 7478 7422 7d2c 0a20 2020 2020 2020 2020  txt"},.         
+0000e230: 2020 207b 226c 6f63 616c 5061 7468 223a     {"localPath":
+0000e240: 2022 6469 725f 322f 6669 6c65 5f32 2e74   "dir_2/file_2.t
+0000e250: 7874 222c 2022 7570 6c6f 6164 5061 7468  xt", "uploadPath
+0000e260: 223a 2022 3a3a 6669 6c65 5f32 2e74 7874  ": "::file_2.txt
+0000e270: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+0000e280: 7b22 6c6f 6361 6c50 6174 6822 3a20 2266  {"localPath": "f
+0000e290: 696c 655f 332e 7478 7422 2c20 2275 706c  ile_3.txt", "upl
+0000e2a0: 6f61 6450 6174 6822 3a20 226f 7468 6572  oadPath": "other
+0000e2b0: 5f6e 616d 6573 7061 6365 3a3a 6669 6c65  _namespace::file
+0000e2c0: 5f33 2e74 7874 227d 0a20 2020 2020 2020  _3.txt"}.       
+0000e2d0: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
+0000e2e0: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+0000e2f0: 0a7d 0a60 6060 0a0a 5768 656e 2072 756e  .}.```..When run
+0000e300: 6e69 6e67 2074 6865 2050 7974 686f 6e20  ning the Python 
+0000e310: 4578 616d 706c 6573 2063 6f6d 6d61 6e64  Examples command
+0000e320: 7320 6f6e 202a 2a57 696e 646f 7773 2a2a  s on **Windows**
+0000e330: 2068 6f73 7473 2c20 6e6f 7465 2074 6861   hosts, note tha
+0000e340: 7420 6569 7468 6572 2057 696e 646f 7773  t either Windows
+0000e350: 206f 7220 556e 6978 2064 6972 6563 746f   or Unix directo
+0000e360: 7279 2073 6570 6172 6174 6f72 7320 6361  ry separators ca
+0000e370: 6e20 6265 2075 7365 6420 666f 7220 7468  n be used for th
+0000e380: 6520 606c 6f63 616c 5061 7468 6020 7061  e `localPath` pa
+0000e390: 7468 6e61 6d65 7320 286f 7220 7468 6520  thnames (or the 
+0000e3a0: 7061 7468 6e61 6d65 7320 696e 2060 696e  pathnames in `in
+0000e3b0: 7075 7473 6029 2c20 6275 7420 7468 6520  puts`), but the 
+0000e3c0: 556e 6978 2063 6f6e 7665 6e74 696f 6e20  Unix convention 
+0000e3d0: 6d75 7374 2062 6520 7573 6564 2066 6f72  must be used for
+0000e3e0: 2074 6865 2060 7570 6c6f 6164 5061 7468   the `uploadPath
+0000e3f0: 6020 6e61 6d65 732c 2065 2e67 2e3a 0a0a  ` names, e.g.:..
+0000e400: 6060 6074 6f6d 6c0a 7570 6c6f 6164 4669  ```toml.uploadFi
+0000e410: 6c65 7320 3d20 5b0a 2020 2020 7b6c 6f63  les = [.    {loc
+0000e420: 616c 5061 7468 203d 2022 6469 725f 325c  alPath = "dir_2\
+0000e430: 5c66 696c 655f 322e 7478 7422 2c20 7570  \file_2.txt", up
+0000e440: 6c6f 6164 5061 7468 203d 2022 3a3a 6d79  loadPath = "::my
+0000e450: 5f64 6972 6563 746f 7279 2f66 696c 655f  _directory/file_
+0000e460: 322e 7478 7422 7d2c 0a5d 0a60 6060 0a0a  2.txt"},.].```..
+0000e470: 5468 6520 6075 706c 6f61 6446 696c 6573  The `uploadFiles
+0000e480: 6020 7072 6f70 6572 7479 2063 616e 2061  ` property can a
+0000e490: 6c73 6f20 6265 2073 6574 2061 7420 7468  lso be set at th
+0000e4a0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000e4b0: 6e74 2061 6e64 2054 6173 6b20 4772 6f75  nt and Task Grou
+0000e4c0: 7020 6c65 7665 6c73 2c20 616e 6420 7072  p levels, and pr
+0000e4d0: 6f70 6572 7479 2069 6e68 6572 6974 616e  operty inheritan
+0000e4e0: 6365 206f 7065 7261 7465 7320 6173 206e  ce operates as n
+0000e4f0: 6f72 6d61 6c2e 0a0a 466f 7220 6075 706c  ormal...For `upl
+0000e500: 6f61 6450 6174 6860 2c20 7468 6520 7361  oadPath`, the sa
+0000e510: 6d65 2060 3a3a 6020 6e61 6d69 6e67 2063  me `::` naming c
+0000e520: 6f6e 7665 6e74 696f 6e20 6973 2061 7661  onvention is ava
+0000e530: 696c 6162 6c65 2061 7320 6973 2075 7365  ilable as is use
+0000e540: 6420 696e 2074 6865 2060 7665 7269 6679  d in the `verify
+0000e550: 4174 5374 6172 7460 2c20 6076 6572 6966  AtStart`, `verif
+0000e560: 7957 6169 7460 2061 6e64 2060 696e 7075  yWait` and `inpu
+0000e570: 7473 4f70 7469 6f6e 616c 6020 7072 6f70  tsOptional` prop
+0000e580: 6572 7469 6573 2064 6973 6375 7373 6564  erties discussed
+0000e590: 2062 656c 6f77 3a0a 0a2d 2049 6620 603a   below:..- If `:
+0000e5a0: 3a60 2069 7320 6e6f 7420 7573 6564 2c20  :` is not used, 
+0000e5b0: 7468 656e 2074 6865 2066 696c 6520 6973  then the file is
+0000e5c0: 2075 706c 6f61 6465 6420 7265 6c61 7469   uploaded relati
+0000e5d0: 7665 2074 6f20 7468 6520 6375 7272 656e  ve to the curren
+0000e5e0: 7420 6e61 6d65 7370 6163 6520 696e 2061  t namespace in a
+0000e5f0: 2064 6972 6563 746f 7279 206e 616d 6564   directory named
+0000e600: 2061 6674 6572 2074 6865 206e 616d 6520   after the name 
+0000e610: 6f66 2074 6865 2057 6f72 6b20 5265 7175  of the Work Requ
+0000e620: 6972 656d 656e 740a 2d20 4966 2060 3a3a  irement.- If `::
+0000e630: 6020 6973 2075 7365 6420 6174 2074 6865  ` is used at the
+0000e640: 2073 7461 7274 206f 6620 7468 6520 6075   start of the `u
+0000e650: 706c 6f61 6450 6174 6860 2c20 7468 6520  ploadPath`, the 
+0000e660: 6669 6c65 2069 7320 7570 6c6f 6164 6564  file is uploaded
+0000e670: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+0000e680: 2072 6f6f 7420 6f66 2074 6865 2063 7572   root of the cur
+0000e690: 7265 6e74 206e 616d 6573 7061 6365 0a2d  rent namespace.-
+0000e6a0: 2049 6620 603c 6e61 6d65 7370 6163 653e   If `<namespace>
+0000e6b0: 3a3a 6020 6973 2075 7365 6420 6174 2074  ::` is used at t
+0000e6c0: 6865 2073 7461 7274 206f 6620 6075 706c  he start of `upl
+0000e6d0: 6f61 6450 6174 6860 2c20 7468 6520 6669  oadPath`, the fi
+0000e6e0: 6c65 2069 7320 7570 6c6f 6164 6564 2072  le is uploaded r
+0000e6f0: 656c 6174 6976 6520 746f 2074 6865 2072  elative to the r
+0000e700: 6f6f 7420 6f66 2060 3c6e 616d 6573 7061  oot of `<namespa
+0000e710: 6365 3e60 0a0a 4561 6368 2066 696c 6520  ce>`..Each file 
+0000e720: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
+0000e730: 2060 7570 6c6f 6164 4669 6c65 7360 206c   `uploadFiles` l
+0000e740: 6973 7473 2077 696c 6c20 6f6e 6c79 2062  ists will only b
+0000e750: 6520 7570 6c6f 6164 6564 206f 6e63 6520  e uploaded once 
+0000e760: 746f 2065 6163 6820 756e 6971 7565 2075  to each unique u
+0000e770: 706c 6f61 6420 6c6f 6361 7469 6f6e 2066  pload location f
+0000e780: 6f72 2061 6e79 2067 6976 656e 2069 6e76  or any given inv
+0000e790: 6f63 6174 696f 6e20 6f66 2060 7964 2d73  ocation of `yd-s
+0000e7a0: 7562 6d69 7460 2e0a 0a49 6620 6120 6669  ubmit`...If a fi
+0000e7b0: 6c65 2069 6e20 7468 6520 6075 706c 6f61  le in the `uploa
+0000e7c0: 6446 696c 6573 6020 6c69 7374 2069 7320  dFiles` list is 
+0000e7d0: 7265 7175 6972 6564 2062 7920 6120 5461  required by a Ta
+0000e7e0: 736b 2c20 6974 206d 7573 7420 7365 7061  sk, it must sepa
+0000e7f0: 7261 7465 6c79 2062 6520 6164 6465 6420  rately be added 
+0000e800: 746f 2074 6865 2060 7665 7269 6679 4174  to the `verifyAt
+0000e810: 5374 6172 7460 206f 7220 6076 6572 6966  Start` or `verif
+0000e820: 7957 6169 7460 206c 6973 7473 2064 6973  yWait` lists dis
+0000e830: 6375 7373 6564 2062 656c 6f77 2e20 5468  cussed below. Th
+0000e840: 6973 2069 7320 6e6f 7420 646f 6e65 2061  is is not done a
+0000e850: 7574 6f6d 6174 6963 616c 6c79 2e20 4e6f  utomatically. No
+0000e860: 7465 2061 6c73 6f20 7468 6174 2074 6865  te also that the
+0000e870: 2060 666c 6174 7465 6e55 706c 6f61 6450   `flattenUploadP
+0000e880: 6174 6873 6020 7072 6f70 6572 7479 2069  aths` property i
+0000e890: 7320 6967 6e6f 7265 6420 666f 7220 6669  s ignored for fi
+0000e8a0: 6c65 7320 696e 2074 6865 2060 7570 6c6f  les in the `uplo
+0000e8b0: 6164 4669 6c65 7360 206c 6973 742e 0a0a  adFiles` list...
+0000e8c0: 2323 2323 2055 7369 6e67 2057 696c 6463  #### Using Wildc
+0000e8d0: 6172 6473 2069 6e20 7468 6520 6075 706c  ards in the `upl
+0000e8e0: 6f61 6446 696c 6573 6020 4c69 7374 0a0a  oadFiles` List..
+0000e8f0: 4669 6c65 2061 6e64 2064 6972 6563 746f  File and directo
+0000e900: 7279 206e 616d 6520 7769 6c64 6361 7264  ry name wildcard
+0000e910: 7320 6361 6e20 6265 2075 7365 6420 696e  s can be used in
+0000e920: 2060 6c6f 6361 6c50 6174 6860 2070 726f   `localPath` pro
+0000e930: 7065 7274 6965 732e 2049 6620 7769 6c64  perties. If wild
+0000e940: 6361 7264 7320 6172 6520 7573 6564 2c20  cards are used, 
+0000e950: 7468 656e 2074 6865 2060 7570 6c6f 6164  then the `upload
+0000e960: 5061 7468 6020 7072 6f70 6572 7479 206d  Path` property m
+0000e970: 7573 7420 656e 6420 7769 7468 2061 2060  ust end with a `
+0000e980: 2a60 2c20 7768 6963 6820 7769 6c6c 2062  *`, which will b
+0000e990: 6520 7265 706c 6163 6564 2077 6974 6820  e replaced with 
+0000e9a0: 7468 6520 6e61 6d65 206f 6620 6561 6368  the name of each
+0000e9b0: 2066 696c 6520 7468 6174 206d 6174 6368   file that match
+0000e9c0: 6573 2074 6865 2077 696c 6463 6172 642c  es the wildcard,
+0000e9d0: 2065 2e67 2e3a 0a0a 6060 6074 6f6d 6c0a   e.g.:..```toml.
+0000e9e0: 7570 6c6f 6164 4669 6c65 7320 3d20 5b0a  uploadFiles = [.
+0000e9f0: 2020 2020 7b6c 6f63 616c 5061 7468 203d      {localPath =
+0000ea00: 2022 2a2e 7368 222c 2075 706c 6f61 6450   "*.sh", uploadP
+0000ea10: 6174 6820 3d20 2273 6372 6970 7473 2f2a  ath = "scripts/*
+0000ea20: 227d 2c0a 2020 2020 7b6c 6f63 616c 5061  "},.    {localPa
+0000ea30: 7468 203d 2022 7465 7874 2f2a 2e74 7874  th = "text/*.txt
+0000ea40: 222c 2075 706c 6f61 6450 6174 6820 3d20  ", uploadPath = 
+0000ea50: 223a 3a74 6f70 2d6c 6576 656c 2f2a 227d  "::top-level/*"}
+0000ea60: 2c0a 2020 2020 7b6c 6f63 616c 5061 7468  ,.    {localPath
+0000ea70: 203d 2022 7372 632f 2a2e 7079 222c 2075   = "src/*.py", u
+0000ea80: 706c 6f61 6450 6174 6820 3d20 226f 7468  ploadPath = "oth
+0000ea90: 6572 2d6e 616d 6573 7061 6365 3a3a 2a22  er-namespace::*"
+0000eaa0: 7d2c 0a5d 0a60 6060 0a0a 5468 6520 602d  },.].```..The `-
+0000eab0: 2d64 7279 2d72 756e 6020 2860 2d44 6029  -dry-run` (`-D`)
+0000eac0: 206f 7074 696f 6e20 6361 6e20 6265 2075   option can be u
+0000ead0: 7365 6420 7769 7468 2060 7964 2d73 7562  sed with `yd-sub
+0000eae0: 6d69 7460 2074 6f20 7072 696e 7420 6f75  mit` to print ou
+0000eaf0: 7420 7468 6520 6669 6c65 7320 7468 6174  t the files that
+0000eb00: 2077 6f75 6c64 2062 6520 7570 6c6f 6164   would be upload
+0000eb10: 6564 2c20 616e 6420 7468 6569 7220 7570  ed, and their up
+0000eb20: 6c6f 6164 206c 6f63 6174 696f 6e73 2e20  load locations. 
+0000eb30: 0a0a 2323 2320 4669 6c65 2044 6570 656e  ..### File Depen
+0000eb40: 6465 6e63 6965 7320 5573 696e 6720 6076  dencies Using `v
+0000eb50: 6572 6966 7941 7453 7461 7274 6020 616e  erifyAtStart` an
+0000eb60: 6420 6076 6572 6966 7957 6169 7460 0a0a  d `verifyWait`..
+0000eb70: 4974 2773 2070 6f73 7369 626c 6520 746f  It's possible to
+0000eb80: 206d 616b 6520 5461 736b 7320 6465 7065   make Tasks depe
+0000eb90: 6e64 656e 7420 6f6e 2074 6865 2070 7265  ndent on the pre
+0000eba0: 7365 6e63 6520 6f66 2066 696c 6573 2069  sence of files i
+0000ebb0: 6e20 7468 6520 4f62 6a65 6374 2053 746f  n the Object Sto
+0000ebc0: 7265 2062 7920 7573 696e 6720 7468 6520  re by using the 
+0000ebd0: 6076 6572 6966 7941 7453 7461 7274 6020  `verifyAtStart` 
+0000ebe0: 616e 6420 6076 6572 6966 7957 6169 7460  and `verifyWait`
+0000ebf0: 206c 6973 7473 2e20 5468 6573 6520 6669   lists. These fi
+0000ec00: 6c65 7320 6172 6520 6e6f 7420 6175 746f  les are not auto
+0000ec10: 6d61 7469 6361 6c6c 7920 7570 6c6f 6164  matically upload
+0000ec20: 6564 2077 6865 6e20 7573 696e 6720 6079  ed when using `y
+0000ec30: 642d 7375 626d 6974 6020 736f 2061 7265  d-submit` so are
+0000ec40: 2075 706c 6f61 6465 6420 6d61 6e75 616c   uploaded manual
+0000ec50: 6c79 2028 652e 672e 2c20 6279 2075 7369  ly (e.g., by usi
+0000ec60: 6e67 2060 7964 2d75 706c 6f61 6460 292c  ng `yd-upload`),
+0000ec70: 2075 706c 6f61 6465 6420 7573 696e 6720   uploaded using 
+0000ec80: 7468 6520 6075 706c 6f61 6446 696c 6573  the `uploadFiles
+0000ec90: 6020 7072 6f70 6572 7479 2c20 6f72 2061  ` property, or a
+0000eca0: 7265 2063 7265 6174 6564 2061 7320 6120  re created as a 
+0000ecb0: 7265 7375 6c74 206f 6620 7468 6520 6578  result of the ex
+0000ecc0: 6563 7574 696f 6e20 6f66 206f 7468 6572  ecution of other
+0000ecd0: 2054 6173 6b73 2e0a 0a4e 6f74 6520 7468   Tasks...Note th
+0000ece0: 6174 2061 2067 6976 656e 2066 696c 6520  at a given file 
+0000ecf0: 6361 6e20 6f6e 6c79 2061 7070 6561 7220  can only appear 
+0000ed00: 696e 202a 6f6e 652a 206f 6620 7468 6520  in *one* of the 
+0000ed10: 6069 6e70 7574 7360 2c20 6076 6572 6966  `inputs`, `verif
+0000ed20: 7941 7453 7461 7274 6020 6f72 2060 7665  yAtStart` or `ve
+0000ed30: 7269 6679 5761 6974 6020 6c69 7374 732e  rifyWait` lists.
+0000ed40: 0a0a 5461 736b 7320 7769 7468 2060 7665  ..Tasks with `ve
+0000ed50: 7269 6679 4174 5374 6172 7460 2064 6570  rifyAtStart` dep
+0000ed60: 656e 6465 6e63 6965 7320 7769 6c6c 2066  endencies will f
+0000ed70: 6169 6c20 696d 6d65 6469 6174 656c 7920  ail immediately 
+0000ed80: 6966 2074 6865 2072 6571 7569 7265 6420  if the required 
+0000ed90: 6669 6c65 7320 6172 6520 6e6f 7420 7072  files are not pr
+0000eda0: 6573 656e 7420 7768 656e 2074 6865 2054  esent when the T
+0000edb0: 6173 6b20 6973 2073 7562 6d69 7474 6564  ask is submitted
+0000edc0: 2e20 5461 736b 7320 7769 7468 2060 7665  . Tasks with `ve
+0000edd0: 7269 6679 5761 6974 6020 6465 7065 6e64  rifyWait` depend
+0000ede0: 656e 6369 6573 2077 696c 6c20 6e6f 7420  encies will not 
+0000edf0: 6265 636f 6d65 2060 5245 4144 5960 2074  become `READY` t
+0000ee00: 6f20 6265 2073 6368 6564 756c 6564 2074  o be scheduled t
+0000ee10: 6f20 576f 726b 6572 7320 756e 7469 6c20  o Workers until 
+0000ee20: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+0000ee30: 2061 7265 2073 6174 6973 6669 6564 2e0a   are satisfied..
+0000ee40: 0a57 6865 6e20 7370 6563 6966 7969 6e67  .When specifying
+0000ee50: 2066 696c 6573 2069 6e20 7468 6520 6076   files in the `v
+0000ee60: 6572 6966 7941 7453 7461 7274 6020 616e  erifyAtStart` an
+0000ee70: 6420 6076 6572 6966 7957 6169 7460 206c  d `verifyWait` l
+0000ee80: 6973 7473 2c20 6173 2077 6974 6820 7468  ists, as with th
+0000ee90: 6520 6075 706c 6f61 6450 6174 6860 2070  e `uploadPath` p
+0000eea0: 726f 7065 7274 7920 6469 7363 7573 7365  roperty discusse
+0000eeb0: 6420 6162 6f76 652c 2074 6865 2066 696c  d above, the fil
+0000eec0: 6520 6c6f 6361 7469 6f6e 7320 6361 6e20  e locations can 
+0000eed0: 6265 2028 3129 2072 656c 6174 6976 6520  be (1) relative 
+0000eee0: 746f 2074 6865 2057 6f72 6b20 5265 7175  to the Work Requ
+0000eef0: 6972 656d 656e 7420 6e61 6d65 2069 6e20  irement name in 
+0000ef00: 7468 6520 6375 7272 656e 7420 6e61 6d65  the current name
+0000ef10: 7370 6163 6520 2874 6865 2064 6566 6175  space (the defau
+0000ef20: 6c74 292c 2028 3229 2072 656c 6174 6976  lt), (2) relativ
+0000ef30: 6520 746f 2074 6865 2072 6f6f 7420 6f66  e to the root of
+0000ef40: 2074 6865 2063 7572 7265 6e74 206e 616d   the current nam
+0000ef50: 6573 7061 6365 2c20 6f72 2028 3329 2072  espace, or (3) r
+0000ef60: 656c 6174 6976 6520 746f 2074 6865 2072  elative to the r
+0000ef70: 6f6f 7420 6f66 2061 2064 6966 6665 7265  oot of a differe
+0000ef80: 6e74 206e 616d 6573 7061 6365 2069 6e20  nt namespace in 
+0000ef90: 7468 6520 7573 6572 2773 2041 6363 6f75  the user's Accou
+0000efa0: 6e74 2e0a 0a31 2e20 466f 7220 6669 6c65  nt...1. For file
+0000efb0: 7320 7265 6c61 7469 7665 2074 6f20 7468  s relative to th
+0000efc0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000efd0: 6e74 206e 616d 6520 696e 2074 6865 2063  nt name in the c
+0000efe0: 7572 7265 6e74 206e 616d 6573 7061 6365  urrent namespace
+0000eff0: 2c20 6a75 7374 2075 7365 2074 6865 2066  , just use the f
+0000f000: 696c 6520 7061 7468 2c20 652e 672e 0a60  ile path, e.g..`
+0000f010: 6060 7368 656c 6c0a 2276 6572 6966 7957  ``shell."verifyW
+0000f020: 6169 7422 3a20 5b22 6669 6c65 5f31 2e74  ait": ["file_1.t
+0000f030: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
+0000f040: 656e 743a 7465 7374 7275 6e5f 3232 3131  ent:testrun_2211
+0000f050: 3038 2d31 3230 3430 342d 3764 322f 6669  08-120404-7d2/fi
+0000f060: 6c65 5f31 2e74 7874 0a60 6060 0a0a 322e  le_1.txt.```..2.
+0000f070: 2046 6f72 2066 696c 6573 2072 656c 6174   For files relat
+0000f080: 6976 6520 746f 2074 6865 2072 6f6f 7420  ive to the root 
+0000f090: 6f66 2074 6865 2063 7572 7265 6e74 206e  of the current n
+0000f0a0: 616d 6573 7061 6365 2c20 7072 6566 6978  amespace, prefix
+0000f0b0: 2074 6865 2066 696c 6520 7061 7468 2077   the file path w
+0000f0c0: 6974 6820 603a 3a60 2c20 652e 672e 0a60  ith `::`, e.g..`
+0000f0d0: 6060 7368 656c 6c0a 2276 6572 6966 7957  ``shell."verifyW
+0000f0e0: 6169 7422 3a20 5b22 3a3a 6669 6c65 5f31  ait": ["::file_1
+0000f0f0: 2e74 7874 225d 202d 3e20 6465 7665 6c6f  .txt"] -> develo
+0000f100: 706d 656e 743a 6669 6c65 5f31 2e74 7874  pment:file_1.txt
+0000f110: 0a60 6060 0a0a 332e 2046 6f72 2066 696c  .```..3. For fil
+0000f120: 6573 2072 656c 6174 6976 6520 746f 2074  es relative to t
+0000f130: 6865 2072 6f6f 7420 6f66 2061 2064 6966  he root of a dif
+0000f140: 6665 7265 6e74 206e 616d 6573 7061 6365  ferent namespace
+0000f150: 2c20 7072 6566 6978 2074 6865 2066 696c  , prefix the fil
+0000f160: 6520 7061 7468 2077 6974 6820 7468 6520  e path with the 
+0000f170: 6e61 6d65 7370 6163 6520 6e61 6d65 2061  namespace name a
+0000f180: 6e64 2060 3a3a 602c 2065 2e67 2e0a 6060  nd `::`, e.g..``
+0000f190: 6073 6865 6c6c 0a22 7665 7269 6679 5761  `shell."verifyWa
+0000f1a0: 6974 223a 205b 226f 7468 6572 5f6e 616d  it": ["other_nam
+0000f1b0: 6573 7061 6365 3a3a 6669 6c65 5f31 2e74  espace::file_1.t
+0000f1c0: 7874 225d 202d 3e20 6f74 6865 725f 6e61  xt"] -> other_na
+0000f1d0: 6d65 7370 6163 653a 6669 6c65 5f31 2e74  mespace:file_1.t
+0000f1e0: 7874 0a60 6060 0a0a 5468 6520 7573 6520  xt.```..The use 
+0000f1f0: 6f66 2074 6865 2074 6872 6565 2064 6966  of the three dif
+0000f200: 6665 7265 6e74 2066 6f72 6d73 2063 616e  ferent forms can
+0000f210: 2062 6520 6d69 7865 6420 7769 7468 696e   be mixed within
+0000f220: 2061 2073 696e 676c 6520 6c69 7374 2c20   a single list, 
+0000f230: 652e 672e 3a0a 6060 6073 6865 6c6c 0a22  e.g.:.```shell."
+0000f240: 7665 7269 6679 4174 5374 6172 7422 3a20  verifyAtStart": 
+0000f250: 5b22 6669 6c65 5f31 2e74 7874 222c 2022  ["file_1.txt", "
+0000f260: 3a3a 6469 725f 322f 6669 6c65 5f32 2e74  ::dir_2/file_2.t
+0000f270: 7874 222c 2022 6f74 6865 725f 6e61 6d65  xt", "other_name
+0000f280: 7370 6163 653a 3a64 6972 5f33 2f66 696c  space::dir_3/fil
+0000f290: 655f 332e 7478 7422 5d0a 6060 600a 0a23  e_3.txt"].```..#
+0000f2a0: 2323 2046 696c 6573 2044 6f77 6e6c 6f61  ## Files Downloa
+0000f2b0: 6465 6420 5573 696e 6720 6069 6e70 7574  ded Using `input
+0000f2c0: 734f 7074 696f 6e61 6c60 0a0a 5468 6520  sOptional`..The 
+0000f2d0: 6069 6e70 7574 734f 7074 696f 6e61 6c60  `inputsOptional`
+0000f2e0: 2070 726f 7065 7274 7920 776f 726b 7320   property works 
+0000f2f0: 696e 2061 2073 696d 696c 6172 2066 6173  in a similar fas
+0000f300: 6869 6f6e 2074 6f20 7468 6520 6076 6572  hion to the `ver
+0000f310: 6966 792a 6020 7072 6f70 6572 7469 6573  ify*` properties
+0000f320: 2061 626f 7665 2c20 6275 7420 7468 6520   above, but the 
+0000f330: 6669 6c65 7320 7370 6563 6966 6965 6420  files specified 
+0000f340: 696e 2074 6869 7320 6c69 7374 2061 7265  in this list are
+0000f350: 206f 7074 696f 6e61 6c2e 2054 6869 7320   optional. This 
+0000f360: 7072 6f70 6572 7479 2061 6c73 6f20 616c  property also al
+0000f370: 6c6f 7773 2066 6f72 2074 6865 2075 7365  lows for the use
+0000f380: 206f 6620 7769 6c64 6361 7264 7320 602a   of wildcards `*
+0000f390: 6020 616e 6420 602a 2a60 2074 6f20 636f  ` and `**` to co
+0000f3a0: 6c6c 6563 7420 6669 6c65 7320 7573 696e  llect files usin
+0000f3b0: 6720 7769 6c64 6361 7264 2070 6174 6873  g wildcard paths
+0000f3c0: 2e20 5468 6520 2a2a 616e 742a 2a20 636f  . The **ant** co
+0000f3d0: 6e76 656e 7469 6f6e 7320 6172 6520 7573  nventions are us
+0000f3e0: 6564 2066 6f72 2074 6865 7365 2077 696c  ed for these wil
+0000f3f0: 6463 6172 6473 2e0a 0a23 2323 2046 696c  dcards...### Fil
+0000f400: 6573 2044 6f77 6e6c 6f61 6465 6420 746f  es Downloaded to
+0000f410: 2061 204e 6f64 6520 666f 7220 7573 6520   a Node for use 
+0000f420: 696e 2054 6173 6b20 4578 6563 7574 696f  in Task Executio
+0000f430: 6e0a 0a57 6865 6e20 6120 5461 736b 2069  n..When a Task i
+0000f440: 7320 6578 6563 7574 6564 2062 7920 6120  s executed by a 
+0000f450: 576f 726b 6572 206f 6e20 6120 4e6f 6465  Worker on a Node
+0000f460: 2c20 6974 7320 7265 7175 6972 6564 2066  , its required f
+0000f470: 696c 6573 2061 7265 2064 6f77 6e6c 6f61  iles are downloa
+0000f480: 6465 6420 6672 6f6d 2074 6865 204f 626a  ded from the Obj
+0000f490: 6563 7420 5374 6f72 6520 7072 696f 7220  ect Store prior 
+0000f4a0: 746f 2054 6173 6b20 6578 6563 7574 696f  to Task executio
+0000f4b0: 6e2e 2041 6e79 2066 696c 6520 6c69 7374  n. Any file list
+0000f4c0: 6564 2069 6e20 7468 6520 6069 6e70 7574  ed in the `input
+0000f4d0: 7360 2066 6f72 2061 2054 6173 6b20 6973  s` for a Task is
+0000f4e0: 2061 7373 756d 6564 2074 6f20 6265 2072   assumed to be r
+0000f4f0: 6571 7569 7265 642c 2061 6c6f 6e67 2077  equired, along w
+0000f500: 6974 6820 616e 7920 6164 6469 7469 6f6e  ith any addition
+0000f510: 616c 2066 696c 6573 2073 7065 6369 6669  al files specifi
+0000f520: 6564 2069 6e20 7468 6520 6076 6572 6966  ed in the `verif
+0000f530: 7941 7453 7461 7274 6020 616e 6420 6076  yAtStart` and `v
+0000f540: 6572 6966 7957 6169 7460 206c 6973 7473  erifyWait` lists
+0000f550: 2e20 4669 6c65 7320 7370 6563 6966 6965  . Files specifie
+0000f560: 6420 7573 696e 6720 7468 6520 6069 6e70  d using the `inp
+0000f570: 7574 734f 7074 696f 6e61 6c60 2070 726f  utsOptional` pro
+0000f580: 7065 7274 7920 6172 6520 6f70 7469 6f6e  perty are option
+0000f590: 616c 6c79 2064 6f77 6e6c 6f61 6465 6420  ally downloaded 
+0000f5a0: 6672 6f6d 2074 6865 204f 626a 6563 7420  from the Object 
+0000f5b0: 5374 6f72 652e 2028 4e6f 7465 2074 6861  Store. (Note tha
+0000f5c0: 7420 6120 6669 6c65 2073 686f 756c 6420  t a file should 
+0000f5d0: 6f6e 6c79 2061 7070 6561 7220 696e 206f  only appear in o
+0000f5e0: 6e65 206f 6620 7468 6573 6520 666f 7572  ne of these four
+0000f5f0: 206c 6973 7473 2c20 6f74 6865 7277 6973   lists, otherwis
+0000f600: 6520 6079 642d 7375 626d 6974 6020 7769  e `yd-submit` wi
+0000f610: 6c6c 2072 6574 7572 6e20 616e 2065 7272  ll return an err
+0000f620: 6f72 2e29 0a0a 5768 656e 2061 2054 6173  or.)..When a Tas
+0000f630: 6b20 6973 2073 7461 7274 6564 2062 7920  k is started by 
+0000f640: 7468 6520 4167 656e 742c 2069 7473 2077  the Agent, its w
+0000f650: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
+0000f660: 2068 6173 2061 2070 6174 7465 726e 2073   has a pattern s
+0000f670: 6f6d 6574 6869 6e67 206c 696b 653a 0a0a  omething like:..
+0000f680: 602f 7661 722f 6f70 742f 7965 6c6c 6f77  `/var/opt/yellow
+0000f690: 646f 672f 7964 2d61 6765 6e74 2d34 2f64  dog/yd-agent-4/d
+0000f6a0: 6174 612f 776f 726b 6572 732f 312f 7964  ata/workers/1/yd
+0000f6b0: 6964 5f74 6173 6b5f 4430 4430 4430 5f36  id_task_D0D0D0_6
+0000f6c0: 3866 3565 3562 652d 6463 3933 2d34 3965  8f5e5be-dc93-49e
+0000f6d0: 622d 6138 3234 2d31 6663 6462 3532 6639  b-a824-1fcdb52f9
+0000f6e0: 3139 355f 315f 3160 0a0a 2860 7964 6964  195_1_1`..(`ydid
+0000f6f0: 5f74 6173 6b5f 4430 4430 4430 5f36 3866  _task_D0D0D0_68f
+0000f700: 3565 3562 652d 6463 3933 2d34 3965 622d  5e5be-dc93-49eb-
+0000f710: 6138 3234 2d31 6663 6462 3532 6639 3139  a824-1fcdb52f919
+0000f720: 355f 315f 3160 2069 7320 616e 2065 7068  5_1_1` is an eph
+0000f730: 656d 6572 616c 2064 6972 6563 746f 7279  emeral directory
+0000f740: 2074 6861 7420 6973 2072 656d 6f76 6564   that is removed
+0000f750: 2061 6674 6572 2074 6865 2054 6173 6b20   after the Task 
+0000f760: 6669 6e69 7368 6573 2061 6e64 2061 6e79  finishes and any
+0000f770: 206f 7574 7075 7473 2068 6176 6520 6265   outputs have be
+0000f780: 656e 2075 706c 6f61 6465 642e 290a 0a46  en uploaded.)..F
+0000f790: 696c 6573 2074 6861 7420 6172 6520 646f  iles that are do
+0000f7a0: 776e 6c6f 6164 6564 2062 7920 7468 6520  wnloaded by the 
+0000f7b0: 4167 656e 7420 7072 696f 7220 746f 2054  Agent prior to T
+0000f7c0: 6173 6b20 6578 6563 7574 696f 6e20 6172  ask execution ar
+0000f7d0: 6520 6c6f 6361 7465 6420 6173 2066 6f6c  e located as fol
+0000f7e0: 6c6f 7773 3a0a 0a31 2e20 4966 2074 6865  lows:..1. If the
+0000f7f0: 2060 666c 6174 7465 6e49 6e70 7574 5061   `flattenInputPa
+0000f800: 7468 7360 2070 726f 7065 7274 7920 6973  ths` property is
+0000f810: 2073 6574 2074 6f20 7468 6520 6465 6661   set to the defa
+0000f820: 756c 7420 6f66 2060 6661 6c73 6560 2066  ult of `false` f
+0000f830: 6f72 2074 6865 2054 6173 6b2c 2074 6865  or the Task, the
+0000f840: 2064 6f77 6e6c 6f61 6465 6420 6f62 6a65   downloaded obje
+0000f850: 6374 7320 6172 6520 706c 6163 6564 2069  cts are placed i
+0000f860: 6e20 7375 6264 6972 6563 746f 7269 6573  n subdirectories
+0000f870: 2074 6861 7420 6d69 7272 6f72 2074 686f   that mirror tho
+0000f880: 7365 2069 6e20 7468 6520 4f62 6a65 6374  se in the Object
+0000f890: 2053 746f 7265 2c20 696e 636c 7564 696e   Store, includin
+0000f8a0: 6720 7468 6520 576f 726b 2052 6571 7569  g the Work Requi
+0000f8b0: 7265 6d65 6e74 206e 616d 652c 2073 6974  rement name, sit
+0000f8c0: 7561 7465 6420 6265 6e65 6174 6820 7468  uated beneath th
+0000f8d0: 6520 776f 726b 696e 6720 6469 7265 6374  e working direct
+0000f8e0: 6f72 792e 0a0a 0a32 2e20 4966 2074 6865  ory....2. If the
+0000f8f0: 2060 666c 6174 7465 6e49 6e70 7574 5061   `flattenInputPa
+0000f900: 7468 7360 2070 726f 7065 7274 7920 6973  ths` property is
+0000f910: 2073 6574 2074 6f20 6074 7275 6560 2066   set to `true` f
+0000f920: 6f72 2074 6865 2054 6173 6b2c 2074 6865  or the Task, the
+0000f930: 2064 6f77 6e6c 6f61 6465 6420 6f62 6a65   downloaded obje
+0000f940: 6374 7320 6172 6520 616c 6c20 706c 6163  cts are all plac
+0000f950: 6564 2064 6972 6563 746c 7920 696e 2072  ed directly in r
+0000f960: 6f6f 7420 6f66 2074 6865 2054 6173 6b27  oot of the Task'
+0000f970: 7320 776f 726b 696e 6720 6469 7265 6374  s working direct
+0000f980: 6f72 792e 0a0a 466f 7220 6578 616d 706c  ory...For exampl
+0000f990: 653a 0a0a 6060 6073 6865 6c6c 0a49 6620  e:..```shell.If 
+0000f9a0: 7468 6520 7265 7175 6972 6564 206f 626a  the required obj
+0000f9b0: 6563 7420 6973 3a20 6465 7665 6c6f 706d  ect is: developm
+0000f9c0: 656e 743a 3a74 6573 7472 756e 5f32 3231  ent::testrun_221
+0000f9d0: 3130 382d 3132 3034 3034 2d37 6432 2f64  108-120404-7d2/d
+0000f9e0: 6576 2f66 696c 655f 312e 7478 740a 0a74  ev/file_1.txt..t
+0000f9f0: 6865 6e2c 2069 6620 666c 6174 7465 6e49  hen, if flattenI
+0000fa00: 6e70 7574 5061 7468 7320 6973 2066 616c  nputPaths is fal
+0000fa10: 7365 2c20 7468 6520 6669 6c65 2077 696c  se, the file wil
+0000fa20: 6c20 6265 2066 6f75 6e64 2061 743a 0a20  l be found at:. 
+0000fa30: 2d3e 203c 776f 726b 696e 675f 6469 7265  -> <working_dire
+0000fa40: 6374 6f72 793e 2f74 6573 7472 756e 5f32  ctory>/testrun_2
+0000fa50: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
+0000fa60: 2f64 6576 2f66 696c 655f 312e 7478 740a  /dev/file_1.txt.
+0000fa70: 200a 656c 7365 2c20 6966 2066 6c61 7474   .else, if flatt
+0000fa80: 656e 496e 7075 7450 6174 6873 2069 7320  enInputPaths is 
+0000fa90: 7472 7565 2c20 7468 6520 6669 6c65 2077  true, the file w
+0000faa0: 696c 6c20 6265 2066 6f75 6e64 2061 743a  ill be found at:
+0000fab0: 0a20 2d3e 203c 776f 726b 696e 675f 6469  . -> <working_di
+0000fac0: 7265 6374 6f72 793e 2f66 696c 655f 312e  rectory>/file_1.
+0000fad0: 7478 7420 0a20 0a77 6865 7265 203c 776f  txt . .where <wo
+0000fae0: 726b 696e 675f 6469 7265 6374 6f72 793e  rking_directory>
+0000faf0: 2069 733a 0a20 202f 7661 722f 6f70 742f   is:.  /var/opt/
+0000fb00: 7965 6c6c 6f77 646f 672f 7964 2d61 6765  yellowdog/yd-age
+0000fb10: 6e74 2d34 2f64 6174 612f 776f 726b 6572  nt-4/data/worker
+0000fb20: 732f 312f 7964 6964 5f74 6173 6b5f 4430  s/1/ydid_task_D0
+0000fb30: 4430 4430 5f36 3866 3565 3562 652d 6463  D0D0_68f5e5be-dc
+0000fb40: 3933 2d34 3965 622d 6138 3234 2d31 6663  93-49eb-a824-1fc
+0000fb50: 6462 3532 6639 3139 355f 315f 312f 0a60  db52f9195_1_1/.`
+0000fb60: 6060 0a0a 4e6f 7465 2074 6861 7420 7468  ``..Note that th
+0000fb70: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000fb80: 6e74 206e 616d 6520 2865 2e67 2e2c 2060  nt name (e.g., `
+0000fb90: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
+0000fba0: 3230 3430 342d 3764 3260 2920 6973 2061  20404-7d2`) is a
+0000fbb0: 7661 696c 6162 6c65 2076 6961 2074 6865  vailable via the
+0000fbc0: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+0000fbd0: 7475 7469 6f6e 2060 7772 5f6e 616d 6560  tution `wr_name`
+0000fbe0: 2c20 736f 2074 6869 7320 636f 756c 6420  , so this could 
+0000fbf0: 6265 2073 7570 706c 6965 6420 746f 2074  be supplied to t
+0000fc00: 6865 2054 6173 6b20 746f 2068 656c 7020  he Task to help 
+0000fc10: 6974 206c 6f63 6174 6520 6974 7320 646f  it locate its do
+0000fc20: 776e 6c6f 6164 6564 2066 696c 6573 2e20  wnloaded files. 
+0000fc30: 466f 7220 6578 616d 706c 652c 2069 6e20  For example, in 
+0000fc40: 7468 6520 6077 6f72 6b52 6571 7569 7265  the `workRequire
+0000fc50: 6d65 6e74 6020 7365 6374 696f 6e20 6f66  ment` section of
+0000fc60: 2074 6865 2060 636f 6e66 6967 2e74 6f6d   the `config.tom
+0000fc70: 6c60 2066 696c 652c 2049 2063 6f75 6c64  l` file, I could
+0000fc80: 2073 7065 6369 6679 3a0a 0a60 6060 746f   specify:..```to
+0000fc90: 6d6c 0a65 6e76 6972 6f6e 6d65 6e74 203d  ml.environment =
+0000fca0: 207b 5752 5f44 4952 4543 544f 5259 203d   {WR_DIRECTORY =
+0000fcb0: 2022 7b7b 7772 5f6e 616d 657d 7d22 7d0a   "{{wr_name}}"}.
+0000fcc0: 6060 600a 0a54 6865 2057 6f72 6b20 5265  ```..The Work Re
+0000fcd0: 7175 6972 656d 656e 7420 6e61 6d65 2077  quirement name w
+0000fce0: 6f75 6c64 2074 6865 6e20 6265 2061 7661  ould then be ava
+0000fcf0: 696c 6162 6c65 2074 6f20 7468 6520 5461  ilable to the Ta
+0000fd00: 736b 2069 6e20 7468 6520 656e 7669 726f  sk in the enviro
+0000fd10: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
+0000fd20: 2457 525f 4449 5245 4354 4f52 5960 2e0a  $WR_DIRECTORY`..
+0000fd30: 0a23 2323 2046 696c 6573 2055 706c 6f61  .### Files Uploa
+0000fd40: 6465 6420 6672 6f6d 2061 204e 6f64 6520  ded from a Node 
+0000fd50: 746f 2074 6865 204f 626a 6563 7420 5374  to the Object St
+0000fd60: 6f72 6520 6166 7465 7220 5461 736b 2045  ore after Task E
+0000fd70: 7865 6375 7469 6f6e 0a0a 4166 7465 7220  xecution..After 
+0000fd80: 5461 736b 2063 6f6d 706c 6574 696f 6e2c  Task completion,
+0000fd90: 2074 6865 2041 6765 6e74 2077 696c 6c20   the Agent will 
+0000fda0: 7570 6c6f 6164 2073 7065 6369 6669 6564  upload specified
+0000fdb0: 206f 7574 7075 7420 6669 6c65 7320 746f   output files to
+0000fdc0: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
+0000fdd0: 652e 2054 6865 2066 696c 6573 2074 6f20  e. The files to 
+0000fde0: 6265 2075 706c 6f61 6465 6420 6172 6520  be uploaded are 
+0000fdf0: 7468 6f73 6520 6c69 7374 6564 2069 6e20  those listed in 
+0000fe00: 7468 6520 606f 7574 7075 7473 6020 616e  the `outputs` an
+0000fe10: 6420 606f 7574 7075 7473 5265 7175 6972  d `outputsRequir
+0000fe20: 6564 6020 7072 6f70 6572 7469 6573 2066  ed` properties f
+0000fe30: 6f72 2074 6865 2054 6173 6b2e 0a0a 496e  or the Task...In
+0000fe40: 2061 6464 6974 696f 6e2c 2074 6865 2063   addition, the c
+0000fe50: 6f6e 736f 6c65 206f 7574 7075 7420 6f66  onsole output of
+0000fe60: 2074 6865 2054 6173 6b20 6973 2063 6170   the Task is cap
+0000fe70: 7475 7265 6420 696e 2061 2066 696c 6520  tured in a file 
+0000fe80: 6361 6c6c 6564 2060 7461 736b 6f75 7470  called `taskoutp
+0000fe90: 7574 2e74 7874 6020 696e 2074 6865 2072  ut.txt` in the r
+0000fea0: 6f6f 7420 6f66 2074 6865 2054 6173 6b27  oot of the Task'
+0000feb0: 7320 776f 726b 696e 6720 6469 7265 6374  s working direct
+0000fec0: 6f72 792e 2057 6865 7468 6572 2074 6865  ory. Whether the
+0000fed0: 2060 7461 736b 6f75 7470 7574 2e74 7874   `taskoutput.txt
+0000fee0: 6020 6669 6c65 2069 7320 7570 6c6f 6164  ` file is upload
+0000fef0: 6564 2074 6f20 7468 6520 4f62 6a65 6374  ed to the Object
+0000ff00: 2053 746f 7265 2069 7320 6465 7465 726d   Store is determ
+0000ff10: 696e 6564 2062 7920 7468 6520 6063 6170  ined by the `cap
+0000ff20: 7475 7265 5461 736b 4f75 7470 7574 6020  tureTaskOutput` 
+0000ff30: 7072 6f70 6572 7479 2066 6f72 2074 6865  property for the
+0000ff40: 2054 6173 6b2c 2061 6e64 2074 6869 7320   Task, and this 
+0000ff50: 6973 2073 6574 2074 6f20 2774 7275 6527  is set to 'true'
+0000ff60: 2062 7920 6465 6661 756c 742e 0a0a 4966   by default...If
+0000ff70: 2054 6173 6b20 6f75 7470 7574 7320 6172   Task outputs ar
+0000ff80: 6520 6372 6561 7465 6420 696e 2073 7562  e created in sub
+0000ff90: 6469 7265 6374 6f72 6965 7320 6265 6c6f  directories belo
+0000ffa0: 7720 7468 6520 5461 736b 2773 2077 6f72  w the Task's wor
+0000ffb0: 6b69 6e67 2064 6972 6563 746f 7279 2c20  king directory, 
+0000ffc0: 696e 636c 7564 6520 7468 6520 6469 7265  include the dire
+0000ffd0: 6374 6f72 6965 7320 666f 7220 6669 6c65  ctories for file
+0000ffe0: 7320 696e 2074 6865 2060 6f75 7470 7574  s in the `output
+0000fff0: 7360 2070 726f 7065 7274 792e 2045 2e67  s` property. E.g
+00010000: 2e2c 2069 6620 6120 5461 736b 2063 7265  ., if a Task cre
+00010010: 6174 6573 2066 696c 6573 2060 7265 7375  ates files `resu
+00010020: 6c74 732f 6f70 656e 666f 616d 2e74 6172  lts/openfoam.tar
+00010030: 2e67 7a60 2061 6e64 2060 7265 7375 6c74  .gz` and `result
+00010040: 732f 6f70 656e 666f 616d 2e6c 6f67 602c  s/openfoam.log`,
+00010050: 2074 6865 6e20 7370 6563 6966 7920 7468   then specify th
+00010060: 6573 6520 666f 7220 7570 6c6f 6164 2069  ese for upload i
+00010070: 6e20 7468 6520 606f 7574 7075 7473 6020  n the `outputs` 
+00010080: 7072 6f70 6572 7479 2061 7320 666f 6c6c  property as foll
+00010090: 6f77 733a 0a0a 6022 6f75 7470 7574 7322  ows:..`"outputs"
+000100a0: 3a20 5b22 7265 7375 6c74 732f 6f70 656e  : ["results/open
+000100b0: 666f 616d 2e74 6172 2e67 7a22 2c20 2272  foam.tar.gz", "r
+000100c0: 6573 756c 7473 2f6f 7065 6e66 6f61 6d2e  esults/openfoam.
+000100d0: 6c6f 6722 5d60 0a0a 5768 656e 206f 7574  log"]`..When out
+000100e0: 7075 7420 6669 6c65 7320 6172 6520 7570  put files are up
+000100f0: 6c6f 6164 6564 2074 6f20 7468 6520 4f62  loaded to the Ob
+00010100: 6a65 6374 2053 746f 7265 2c20 7468 6579  ject Store, they
+00010110: 2061 7265 2070 6c61 6365 6420 696e 2061   are placed in a
+00010120: 2054 6173 6b20 4772 6f75 7020 616e 6420   Task Group and 
+00010130: 5461 736b 2073 7065 6369 6669 6320 6469  Task specific di
+00010140: 7265 6374 6f72 792e 2053 6f2c 2069 6620  rectory. So, if 
+00010150: 7468 6520 4e61 6d65 7370 6163 6520 6973  the Namespace is
+00010160: 2060 6465 7665 6c6f 706d 656e 7460 2c20   `development`, 
+00010170: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+00010180: 6d65 6e74 2069 7320 6074 6573 7472 756e  ment is `testrun
+00010190: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
+000101a0: 6432 602c 2074 6865 2054 6173 6b20 4772  d2`, the Task Gr
+000101b0: 6f75 7020 6973 2060 7461 736b 5f67 726f  oup is `task_gro
+000101c0: 7570 5f31 6020 616e 6420 7468 6520 5461  up_1` and the Ta
+000101d0: 736b 2069 7320 6074 6173 6b5f 3160 2c20  sk is `task_1`, 
+000101e0: 7468 656e 2074 6865 2066 696c 6573 2061  then the files a
+000101f0: 626f 7665 2077 6f75 6c64 2062 6520 7570  bove would be up
+00010200: 6c6f 6164 6564 2074 6f20 7468 6520 4f62  loaded to the Ob
+00010210: 6a65 6374 2053 746f 7265 2061 7320 666f  ject Store as fo
+00010220: 6c6c 6f77 733a 0a0a 6060 6073 6865 6c6c  llows:..```shell
+00010230: 0a64 6576 656c 6f70 6d65 6e74 3a3a 7465  .development::te
+00010240: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
+00010250: 3430 342d 3764 322f 7461 736b 5f67 726f  404-7d2/task_gro
+00010260: 7570 5f31 2f74 6173 6b5f 312f 7265 7375  up_1/task_1/resu
+00010270: 6c74 732f 6f70 656e 666f 616d 2e74 6172  lts/openfoam.tar
+00010280: 2e67 7a0a 6465 7665 6c6f 706d 656e 743a  .gz.development:
+00010290: 3a74 6573 7472 756e 5f32 3231 3130 382d  :testrun_221108-
+000102a0: 3132 3034 3034 2d37 6432 2f74 6173 6b5f  120404-7d2/task_
+000102b0: 6772 6f75 705f 312f 7461 736b 5f31 2f72  group_1/task_1/r
+000102c0: 6573 756c 7473 2f6f 7065 6e66 6f61 6d2e  esults/openfoam.
+000102d0: 6c6f 670a 6465 7665 6c6f 706d 656e 743a  log.development:
+000102e0: 3a74 6573 7472 756e 5f32 3231 3130 382d  :testrun_221108-
+000102f0: 3132 3034 3034 2d37 6432 2f74 6173 6b5f  120404-7d2/task_
+00010300: 6772 6f75 705f 312f 7461 736b 5f31 2f74  group_1/task_1/t
+00010310: 6173 6b6f 7574 7075 742e 7478 740a 6060  askoutput.txt.``
+00010320: 600a 0a54 6865 202a 2a60 6f75 7470 7574  `..The **`output
+00010330: 7352 6571 7569 7265 6460 2a2a 2070 726f  sRequired`** pro
+00010340: 7065 7274 7920 6361 6e20 6265 2075 7365  perty can be use
+00010350: 6420 696e 7374 6561 6420 6f66 2028 6f72  d instead of (or
+00010360: 2069 6e20 6164 6469 7469 6f6e 2074 6f29   in addition to)
+00010370: 2074 6865 2060 6f75 7470 7574 7360 2070   the `outputs` p
+00010380: 726f 7065 7274 792c 2069 6620 7468 6520  roperty, if the 
+00010390: 6f75 7470 7574 2066 696c 6528 7329 202a  output file(s) *
+000103a0: 2a6d 7573 742a 2a20 6265 2061 7661 696c  *must** be avail
+000103b0: 6162 6c65 2066 6f72 2075 706c 6f61 6420  able for upload 
+000103c0: 746f 2074 6865 204f 626a 6563 7420 5374  to the Object St
+000103d0: 6f72 6520 6174 2074 6865 2063 6f6e 636c  ore at the concl
+000103e0: 7573 696f 6e20 6f66 2074 6865 2054 6173  usion of the Tas
+000103f0: 6b20 6f72 2074 6865 2054 6173 6b20 7769  k or the Task wi
+00010400: 6c6c 2062 6520 6d61 726b 6564 2061 7320  ll be marked as 
+00010410: 6046 6169 6c65 6460 2c20 652e 672e 3a0a  `Failed`, e.g.:.
+00010420: 0a60 226f 7574 7075 7473 5265 7175 6972  .`"outputsRequir
+00010430: 6564 223a 205b 2272 6573 756c 7473 2f70  ed": ["results/p
+00010440: 726f 6365 7373 5f6f 7574 7075 742e 7478  rocess_output.tx
+00010450: 7422 5d60 0a0a 2323 2320 4669 6c65 7320  t"]`..### Files 
+00010460: 446f 776e 6c6f 6164 6564 2066 726f 6d20  Downloaded from 
+00010470: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+00010480: 2074 6f20 4c6f 6361 6c20 5374 6f72 6167   to Local Storag
+00010490: 650a 0a54 6865 2060 7964 2d64 6f77 6e6c  e..The `yd-downl
+000104a0: 6f61 6460 2063 6f6d 6d61 6e64 2077 696c  oad` command wil
+000104b0: 6c20 646f 776e 6c6f 6164 2061 6c6c 206f  l download all o
+000104c0: 626a 6563 7473 2066 726f 6d20 7468 6520  bjects from the 
+000104d0: 4f62 6a65 6374 2053 746f 7265 2074 6f20  Object Store to 
+000104e0: 6120 6c6f 6361 6c20 6469 7265 6374 6f72  a local director
+000104f0: 792c 206f 6e20 6120 7065 7220 576f 726b  y, on a per Work
+00010500: 2052 6571 7569 7265 6d65 6e74 2062 6173   Requirement bas
+00010510: 6973 2028 696e 636c 7564 696e 6720 616e  is (including an
+00010520: 7920 6669 6c65 7320 7468 6174 2068 6176  y files that hav
+00010530: 6520 6265 656e 2075 706c 6f61 6465 6429  e been uploaded)
+00010540: 2e20 4120 6c6f 6361 6c20 6469 7265 6374  . A local direct
+00010550: 6f72 7920 6973 2063 7265 6174 6564 2077  ory is created w
+00010560: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
+00010570: 6520 6173 2074 6865 204e 616d 6573 7061  e as the Namespa
+00010580: 6365 2061 6e64 2063 6f6e 7461 696e 696e  ce and containin
+00010590: 6720 7468 6520 576f 726b 2052 6571 7569  g the Work Requi
+000105a0: 7265 6d65 6e74 2064 6972 6563 746f 7269  rement directori
+000105b0: 6573 2e0a 0a55 7365 2074 6865 2060 2d2d  es...Use the `--
+000105c0: 696e 7465 7261 6374 6976 6560 206f 7074  interactive` opt
+000105d0: 696f 6e20 7769 7468 2060 7964 2d64 6f77  ion with `yd-dow
+000105e0: 6e6c 6f61 6460 2074 6f20 7365 6c65 6374  nload` to select
+000105f0: 2077 6869 6368 2057 6f72 6b20 5265 7175   which Work Requ
+00010600: 6972 656d 656e 7428 7329 2074 6f20 646f  irement(s) to do
+00010610: 776e 6c6f 6164 2e0a 0a46 6f72 2074 6865  wnload...For the
+00010620: 2065 7861 6d70 6c65 2061 626f 7665 2c20   example above, 
+00010630: 6079 642d 646f 776e 6c6f 6164 6020 776f  `yd-download` wo
+00010640: 756c 6420 6372 6561 7465 2061 2064 6972  uld create a dir
+00010650: 6563 746f 7279 2063 616c 6c65 6420 6064  ectory called `d
+00010660: 6576 656c 6f70 6d65 6e74 6020 696e 2074  evelopment` in t
+00010670: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
+00010680: 6e67 2064 6972 6563 746f 7279 2c20 636f  ng directory, co
+00010690: 6e74 6169 6e69 6e67 2073 6f6d 6574 6869  ntaining somethi
+000106a0: 6e67 206c 696b 653a 0a0a 6060 6073 6865  ng like:..```she
+000106b0: 6c6c 0a64 6576 656c 6f70 6d65 6e74 0ae2  ll.development..
+000106c0: 9494 e294 80e2 9480 2074 6573 7472 756e  ........ testrun
+000106d0: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
+000106e0: 6432 0a20 2020 20e2 949c e294 80e2 9480  d2.    .........
+000106f0: 2062 6173 685f 7363 7269 7074 2e73 680a   bash_script.sh.
+00010700: 2020 2020 e294 9ce2 9480 e294 8020 6669      ......... fi
+00010710: 6c65 5f31 2e74 7874 0a20 2020 20e2 9494  le_1.txt.    ...
+00010720: e294 80e2 9480 2074 6173 6b5f 6772 6f75  ...... task_grou
+00010730: 705f 310a 2020 2020 2020 2020 e294 94e2  p_1.        ....
+00010740: 9480 e294 8020 7461 736b 5f31 0a20 2020  ..... task_1.   
+00010750: 2020 2020 2020 2020 20e2 949c e294 80e2           .......
+00010760: 9480 2072 6573 756c 7473 0a20 2020 2020  .. results.     
+00010770: 2020 2020 2020 20e2 9482 c2a0 c2a0 20e2         ....... .
+00010780: 949c e294 80e2 9480 206f 7065 6e66 6f61  ........ openfoa
+00010790: 6d2e 6c6f 670a 2020 2020 2020 2020 2020  m.log.          
+000107a0: 2020 e294 82c2 a0c2 a020 e294 94e2 9480    ....... ......
+000107b0: e294 8020 6f70 656e 666f 616d 2e74 6172  ... openfoam.tar
+000107c0: 2e67 7a0a 2020 2020 2020 2020 2020 2020  .gz.            
+000107d0: e294 94e2 9480 e294 8020 7461 736b 6f75  ......... taskou
+000107e0: 7470 7574 2e74 7874 0a60 6060 0a0a 4e6f  tput.txt.```..No
+000107f0: 7465 2074 6861 7420 6576 6572 7974 6869  te that everythi
+00010800: 6e67 2077 6974 6869 6e20 7468 6520 606e  ng within the `n
+00010810: 616d 6573 7061 6365 3a3a 776f 726b 2d72  amespace::work-r
+00010820: 6571 7569 7265 6d65 6e74 6020 6469 7265  equirement` dire
+00010830: 6374 6f72 7920 696e 2074 6865 204f 626a  ctory in the Obj
+00010840: 6563 7420 5374 6f72 6520 6973 2064 6f77  ect Store is dow
+00010850: 6e6c 6f61 6465 642c 2069 6e63 6c75 6469  nloaded, includi
+00010860: 6e67 2061 6e79 2066 696c 6573 2074 6861  ng any files tha
+00010870: 7420 7765 7265 2073 7065 6369 6669 6564  t were specified
+00010880: 2069 6e20 6069 6e70 7574 7360 2061 6e64   in `inputs` and
+00010890: 2075 706c 6f61 6465 6420 6173 2070 6172   uploaded as par
+000108a0: 7420 6f66 2074 6865 2057 6f72 6b20 5265  t of the Work Re
+000108b0: 7175 6972 656d 656e 7420 7375 626d 6973  quirement submis
+000108c0: 7369 6f6e 2e20 4d75 6c74 6970 6c65 2054  sion. Multiple T
+000108d0: 6173 6b20 4772 6f75 7073 2c20 616e 6420  ask Groups, and 
+000108e0: 6d75 6c74 6970 6c65 2054 6173 6b73 2077  multiple Tasks w
+000108f0: 696c 6c20 616c 6c20 6170 7065 6172 2069  ill all appear i
+00010900: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
+00010910: 7374 7275 6374 7572 652e 0a0a 4966 2074  structure...If t
+00010920: 6865 2060 6465 7665 6c6f 706d 656e 7460  he `development`
+00010930: 2064 6972 6563 746f 7279 2061 6c72 6561   directory alrea
+00010940: 6479 2065 7869 7374 732c 2060 7964 2d64  dy exists, `yd-d
+00010950: 6f77 6e6c 6f61 6460 2077 696c 6c20 7472  ownload` will tr
+00010960: 7920 6064 6576 656c 6f70 6d65 6e74 2e30  y `development.0
+00010970: 3160 2c20 6574 632e 2c20 746f 2061 766f  1`, etc., to avo
+00010980: 6964 206f 7665 7277 7269 7469 6e67 2070  id overwriting p
+00010990: 7265 7669 6f75 7320 646f 776e 6c6f 6164  revious download
+000109a0: 732e 0a0a 2323 2054 6173 6b20 4578 6563  s...## Task Exec
+000109b0: 7574 696f 6e20 436f 6e74 6578 740a 0a54  ution Context..T
+000109c0: 6869 7320 7365 6374 696f 6e20 6469 7363  his section disc
+000109d0: 7573 7365 7320 7468 6520 636f 6e74 6578  usses the contex
+000109e0: 7420 7769 7468 696e 2077 6869 6368 2061  t within which a
+000109f0: 2054 6173 6b20 6f70 6572 6174 6573 2077   Task operates w
+00010a00: 6865 6e20 6974 2773 2065 7865 6375 7465  hen it's execute
+00010a10: 6420 6279 2061 2057 6f72 6b65 7220 6f6e  d by a Worker on
+00010a20: 2061 206e 6f64 652e 2049 7420 6170 706c   a node. It appl
+00010a30: 6965 7320 7370 6563 6966 6963 616c 6c79  ies specifically
+00010a40: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
+00010a50: 6720 4167 656e 7420 7275 6e6e 696e 6720  g Agent running 
+00010a60: 6f6e 2061 204c 696e 7578 206e 6f64 652c  on a Linux node,
+00010a70: 2061 6e64 2063 6f6e 6669 6775 7265 6420   and configured 
+00010a80: 7573 696e 6720 7468 6520 6465 6661 756c  using the defaul
+00010a90: 7420 7573 6572 6e61 6d65 2c20 6469 7265  t username, dire
+00010aa0: 6374 6f72 6965 732c 2065 7463 2e20 436f  ctories, etc. Co
+00010ab0: 6e66 6967 7572 6174 696f 6e73 2063 616e  nfigurations can
+00010ac0: 2076 6172 792e 0a0a 2323 2320 5461 736b   vary...### Task
+00010ad0: 2045 7865 6375 7469 6f6e 2053 7465 7073   Execution Steps
+00010ae0: 0a0a 5768 656e 2061 2054 6173 6b20 6973  ..When a Task is
+00010af0: 2061 6c6c 6f63 6174 6564 2074 6f20 6120   allocated to a 
+00010b00: 576f 726b 6572 206f 6e20 6120 6e6f 6465  Worker on a node
+00010b10: 2062 7920 7468 6520 5965 6c6c 6f77 446f   by the YellowDo
+00010b20: 6720 5363 6865 6475 6c65 722c 2074 6865  g Scheduler, the
+00010b30: 2066 6f6c 6c6f 7769 6e67 2073 7465 7073   following steps
+00010b40: 2061 7265 2066 6f6c 6c6f 7765 643a 0a0a   are followed:..
+00010b50: 312e 2054 6865 2041 6765 6e74 2072 756e  1. The Agent run
+00010b60: 6e69 6e67 206f 6e20 7468 6520 6e6f 6465  ning on the node
+00010b70: 2064 6f77 6e6c 6f61 6473 2074 6865 2054   downloads the T
+00010b80: 6173 6b27 7320 7072 6f70 6572 7469 6573  ask's properties
+00010b90: 3a20 6974 7320 6074 6173 6b54 7970 6560  : its `taskType`
+00010ba0: 2c20 2060 6172 6775 6d65 6e74 7360 2c20  ,  `arguments`, 
+00010bb0: 6065 6e76 6972 6f6e 6d65 6e74 602c 2060  `environment`, `
+00010bc0: 7461 736b 6461 7461 602c 2061 6e64 2028  taskdata`, and (
+00010bd0: 6672 6f6d 2074 6865 204f 626a 6563 7420  from the Object 
+00010be0: 5374 6f72 6529 2061 6e79 2066 696c 6573  Store) any files
+00010bf0: 2069 6e20 7468 6520 6069 6e70 7574 7360   in the `inputs`
+00010c00: 206c 6973 7420 616e 6420 616e 7920 6176   list and any av
+00010c10: 6169 6c61 626c 6520 6669 6c65 7320 696e  ailable files in
+00010c20: 2074 6865 2060 696e 7075 7473 4f70 7469   the `inputsOpti
+00010c30: 6f6e 616c 6020 6c69 7374 2e0a 322e 2054  onal` list..2. T
+00010c40: 6865 7365 2066 696c 6573 2061 7265 2070  hese files are p
+00010c50: 6c61 6365 6420 696e 2061 6e20 6570 6865  laced in an ephe
+00010c60: 6d65 7261 6c20 6469 7265 6374 6f72 7920  meral directory 
+00010c70: 6372 6561 7465 6420 666f 7220 7468 6973  created for this
+00010c80: 2054 6173 6b27 7320 6578 6563 7574 696f   Task's executio
+00010c90: 6e2c 2061 6e64 2069 6e74 6f20 7768 6963  n, and into whic
+00010ca0: 6820 616e 7920 6f75 7470 7574 2066 696c  h any output fil
+00010cb0: 6573 2061 7265 2061 6c73 6f20 706c 6163  es are also plac
+00010cc0: 6564 2062 7920 6465 6661 756c 742e 0a32  ed by default..2
+00010cd0: 2e20 5468 6520 4167 656e 7420 7275 6e73  . The Agent runs
+00010ce0: 2074 6865 2063 6f6d 6d61 6e64 2073 7065   the command spe
+00010cf0: 6369 6669 6564 2066 6f72 2074 6865 2060  cified for the `
+00010d00: 7461 736b 5479 7065 6020 696e 2074 6865  taskType` in the
+00010d10: 2041 6765 6e74 2773 2060 6170 706c 6963   Agent's `applic
+00010d20: 6174 696f 6e2e 7961 6d6c 6020 636f 6e66  ation.yaml` conf
+00010d30: 6967 7572 6174 696f 6e20 6669 6c65 2e20  iguration file. 
+00010d40: 5468 6973 2064 6f6e 6520 6173 2061 2073  This done as a s
+00010d50: 696d 706c 6520 6065 7865 6360 206f 6620  imple `exec` of 
+00010d60: 6120 7375 6270 726f 6365 7373 2e0a 332e  a subprocess..3.
+00010d70: 2057 6865 6e20 7468 6520 5461 736b 2063   When the Task c
+00010d80: 6f6e 636c 7564 6573 2c20 7468 6520 4167  oncludes, the Ag
+00010d90: 656e 7420 7573 6573 2074 6865 2065 7869  ent uses the exi
+00010da0: 7420 636f 6465 206f 6620 7468 6520 7375  t code of the su
+00010db0: 6270 726f 6365 7373 2074 6f20 7265 706f  bprocess to repo
+00010dc0: 7274 2073 7563 6365 7373 2028 7a65 726f  rt success (zero
+00010dd0: 2920 6f72 2066 6169 6c75 7265 2028 6e6f  ) or failure (no
+00010de0: 6e2d 7a65 726f 292e 0a34 2e20 5468 6520  n-zero)..4. The 
+00010df0: 4167 656e 7420 7468 656e 2067 6174 6865  Agent then gathe
+00010e00: 7273 2061 6e79 2066 696c 6573 2069 6e20  rs any files in 
+00010e10: 7468 6520 606f 7574 7075 7473 6020 616e  the `outputs` an
+00010e20: 6420 606f 7574 7075 7473 5265 7175 6972  d `outputsRequir
+00010e30: 6564 6020 6c69 7374 7320 616e 6420 7570  ed` lists and up
+00010e40: 6c6f 6164 7320 7468 656d 2074 6f20 7468  loads them to th
+00010e50: 6520 4f62 6a65 6374 2053 746f 7265 2e20  e Object Store. 
+00010e60: 4966 2061 2066 696c 6520 696e 2074 6865  If a file in the
+00010e70: 2060 6f75 7470 7574 7352 6571 7569 7265   `outputsRequire
+00010e80: 6460 206c 6973 7420 6973 206e 6f74 2066  d` list is not f
+00010e90: 6f75 6e64 2c20 7468 6520 5461 736b 2077  ound, the Task w
+00010ea0: 696c 6c20 6265 2072 6570 6f72 7465 6420  ill be reported 
+00010eb0: 6173 2066 6169 6c65 642e 2054 6865 2041  as failed. The A
+00010ec0: 6765 6e74 2077 696c 6c20 616c 736f 206f  gent will also o
+00010ed0: 7074 696f 6e61 6c6c 7920 7570 6c6f 6164  ptionally upload
+00010ee0: 2074 6865 2063 6f6e 736f 6c65 206f 7574   the console out
+00010ef0: 7075 7420 2869 6e63 6c75 6469 6e67 2062  put (including b
+00010f00: 6f74 6820 6073 7464 6f75 7460 2061 6e64  oth `stdout` and
+00010f10: 2060 7374 6465 7272 6029 206f 6620 7468   `stderr`) of th
+00010f20: 6520 5461 736b 2c20 636f 6e74 6169 6e65  e Task, containe
+00010f30: 6420 696e 2074 6865 2060 7461 736b 6f75  d in the `taskou
+00010f40: 7470 7574 2e74 7874 6020 6669 6c65 2e0a  tput.txt` file..
+00010f50: 352e 2054 6865 2065 7068 656d 6572 616c  5. The ephemeral
+00010f60: 2054 6173 6b20 6469 7265 6374 6f72 7920   Task directory 
+00010f70: 6973 2074 6865 6e20 6465 6c65 7465 642e  is then deleted.
+00010f80: 0a0a 4e6f 7465 2074 6861 7420 6966 2061  ..Note that if a
+00010f90: 2054 6173 6b20 6973 2061 626f 7274 6564   Task is aborted
+00010fa0: 2064 7572 696e 6720 6578 6563 7574 696f   during executio
+00010fb0: 6e2c 2074 6865 2054 6173 6b27 7320 7375  n, the Task's su
+00010fc0: 6270 726f 6365 7373 2069 7320 7365 6e74  bprocess is sent
+00010fd0: 2061 2060 5349 4749 4e54 602c 2061 6c6c   a `SIGINT`, all
+00010fe0: 6f77 696e 6720 7468 6520 5461 736b 2061  owing the Task a
+00010ff0: 6e20 6f70 706f 7274 756e 6974 7920 746f  n opportunity to
+00011000: 2074 6572 6d69 6e61 7465 2061 6e79 2063   terminate any c
+00011010: 6869 6c64 2070 726f 6365 7373 6573 206f  hild processes o
+00011020: 7220 6f74 6865 7220 7265 736f 7572 6365  r other resource
+00011030: 7320 2865 2e67 2e2c 2063 6f6e 7461 696e  s (e.g., contain
+00011040: 6572 7329 2074 6861 7420 6d61 7920 6861  ers) that may ha
+00011050: 7665 2062 6565 6e20 7374 6172 7465 6420  ve been started 
+00011060: 6173 2070 6172 7420 6f66 2054 6173 6b20  as part of Task 
+00011070: 6578 6563 7574 696f 6e2e 0a0a 4f6e 6365  execution...Once
+00011080: 2074 6865 2073 7465 7073 2061 626f 7665   the steps above
+00011090: 2068 6176 6520 6265 656e 2063 6f6d 706c   have been compl
+000110a0: 6574 6564 2c20 7468 6520 576f 726b 6572  eted, the Worker
+000110b0: 2069 7320 7265 6164 7920 746f 2061 6363   is ready to acc
+000110c0: 6570 7420 6974 7320 6e65 7874 2054 6173  ept its next Tas
+000110d0: 6b20 6672 6f6d 2074 6865 2059 656c 6c6f  k from the Yello
+000110e0: 7744 6f67 2073 6368 6564 756c 6572 2e0a  wDog scheduler..
+000110f0: 0a4e 6f74 6520 7468 6174 2069 6620 7468  .Note that if th
+00011100: 6520 4167 656e 7420 6f6e 2061 206e 6f64  e Agent on a nod
+00011110: 6520 6861 7320 6d75 6c74 6970 6c65 2057  e has multiple W
+00011120: 6f72 6b65 7273 2c20 7468 656e 2054 6173  orkers, then Tas
+00011130: 6b73 2061 7265 2065 7865 6375 7465 6420  ks are executed 
+00011140: 696e 2070 6172 616c 6c65 6c20 6f6e 2074  in parallel on t
+00011150: 6865 206e 6f64 6520 616e 6420 6361 6e20  he node and can 
+00011160: 7374 6172 7420 616e 6420 7374 6f70 2069  start and stop i
+00011170: 6e64 6570 656e 6465 6e74 6c79 2e0a 0a23  ndependently...#
+00011180: 2323 2054 6865 2055 7365 7220 616e 6420  ## The User and 
+00011190: 4772 6f75 7020 7573 6564 2066 6f72 2054  Group used for T
+000111a0: 6173 6b73 0a0a 4279 2064 6566 6175 6c74  asks..By default
+000111b0: 2c20 7468 6520 4167 656e 7420 7275 6e73  , the Agent runs
+000111c0: 2061 7320 7573 6572 2061 6e64 2067 726f   as user and gro
+000111d0: 7570 2060 7964 2d61 6765 6e74 602c 2061  up `yd-agent`, a
+000111e0: 6e64 2068 656e 6365 2054 6173 6b73 2061  nd hence Tasks a
+000111f0: 6c73 6f20 6578 6563 7574 6520 756e 6465  lso execute unde
+00011200: 7220 7468 6973 2075 7365 722e 0a0a 6079  r this user...`y
+00011210: 642d 6167 656e 7460 2064 6f65 7320 6e6f  d-agent` does no
+00011220: 7420 6861 7665 2060 7375 646f 6020 7072  t have `sudo` pr
+00011230: 6976 696c 6567 6573 2061 7320 7374 616e  ivileges as stan
+00011240: 6461 7264 2c20 6275 7420 7468 6973 2063  dard, but this c
+00011250: 616e 2062 6520 6164 6465 6420 6966 2072  an be added if r
+00011260: 6571 7569 7265 6420 6174 2069 6e73 7461  equired at insta
+00011270: 6e63 6520 626f 6f74 2074 696d 6520 7669  nce boot time vi
+00011280: 6120 7468 6520 6075 7365 7244 6174 6160  a the `userData`
+00011290: 2070 726f 7065 7274 7920 6f66 2061 2070   property of a p
+000112a0: 726f 7669 7369 6f6e 696e 6720 7265 7175  rovisioning requ
+000112b0: 6573 742e 2045 2e67 2e20 2866 6f72 2055  est. E.g. (for U
+000112c0: 6275 6e74 7529 3a0a 0a60 6060 7368 656c  buntu):..```shel
+000112d0: 6c0a 7573 6572 6d6f 6420 2d61 4720 7768  l.usermod -aG wh
+000112e0: 6565 6c20 7964 2d61 6765 6e74 0a65 6368  eel yd-agent.ech
+000112f0: 6f20 2d65 2022 7964 2d61 6765 6e74 5c74  o -e "yd-agent\t
+00011300: 414c 4c3d 2841 4c4c 295c 744e 4f50 4153  ALL=(ALL)\tNOPAS
+00011310: 5357 443a 2041 4c4c 2220 3e20 2f65 7463  SWD: ALL" > /etc
+00011320: 2f73 7564 6f65 7273 2e64 2f30 3230 2d79  /sudoers.d/020-y
+00011330: 642d 6167 656e 740a 6060 600a 0a23 2323  d-agent.```..###
+00011340: 2048 6f6d 6520 4469 7265 6374 6f72 7920   Home Directory 
+00011350: 666f 7220 6079 642d 6167 656e 7460 0a0a  for `yd-agent`..
+00011360: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
+00011370: 686f 6d65 2064 6972 6563 746f 7279 206f  home directory o
+00011380: 6620 7468 6520 6079 642d 6167 656e 7460  f the `yd-agent`
+00011390: 2075 7365 7220 6973 2060 2f6f 7074 2f79   user is `/opt/y
+000113a0: 656c 6c6f 7764 6f67 2f61 6765 6e74 602e  ellowdog/agent`.
+000113b0: 2054 6869 7320 6469 7265 6374 6f72 7920   This directory 
+000113c0: 7479 7069 6361 6c6c 7920 636f 6e74 6169  typically contai
+000113d0: 6e73 2074 6865 2060 6170 706c 6963 6174  ns the `applicat
+000113e0: 696f 6e2e 7961 6d6c 6020 6669 6c65 2075  ion.yaml` file u
+000113f0: 7365 6420 746f 2063 6f6e 6669 6775 7265  sed to configure
+00011400: 2074 6865 2041 6765 6e74 2c20 6173 2077   the Agent, as w
+00011410: 656c 6c20 6173 2061 6e79 2073 6372 6970  ell as any scrip
+00011420: 7473 2074 6861 7420 6172 6520 7573 6564  ts that are used
+00011430: 2074 6f20 6578 6563 7574 6520 7468 6520   to execute the 
+00011440: 5461 736b 2054 7970 6573 2074 6861 7420  Task Types that 
+00011450: 7468 6520 6e6f 6465 2073 7570 706f 7274  the node support
+00011460: 732e 0a0a 4966 206f 6e65 2077 616e 7473  s...If one wants
+00011470: 2074 6f20 5353 4820 746f 2061 6e20 696e   to SSH to an in
+00011480: 7374 616e 6365 2061 7320 7573 6572 2060  stance as user `
+00011490: 7964 2d61 6765 6e74 602c 2070 6572 6861  yd-agent`, perha
+000114a0: 7073 2066 6f72 2064 6562 7567 6769 6e67  ps for debugging
+000114b0: 2070 7572 706f 7365 732c 2053 5348 206b   purposes, SSH k
+000114c0: 6579 7320 6361 6e20 6265 2069 6e73 6572  eys can be inser
+000114d0: 7465 6420 7669 6120 696e 7374 616e 6365  ted via instance
+000114e0: 2060 7573 6572 4461 7461 602c 2065 2e67   `userData`, e.g
+000114f0: 2e3a 0a0a 6060 6073 6865 6c6c 0a59 4441  .:..```shell.YDA
+00011500: 5f48 4f4d 453d 2f6f 7074 2f79 656c 6c6f  _HOME=/opt/yello
+00011510: 7764 6f67 2f61 6765 6e74 0a6d 6b64 6972  wdog/agent.mkdir
+00011520: 202d 7020 2459 4441 5f48 4f4d 452f 2e73   -p $YDA_HOME/.s
+00011530: 7368 0a63 686d 6f64 206f 672d 7277 7820  sh.chmod og-rwx 
+00011540: 2459 4441 5f48 4f4d 452f 2e73 7368 0a63  $YDA_HOME/.ssh.c
+00011550: 6174 203e 3e20 2459 4441 5f48 4f4d 452f  at >> $YDA_HOME/
+00011560: 2e73 7368 2f61 7574 686f 7269 7a65 645f  .ssh/authorized_
+00011570: 6b65 7973 203c 3c20 454f 460a 3c3c 496e  keys << EOF.<<In
+00011580: 7365 7274 5f50 7562 6c69 635f 6b65 795f  sert_Public_key_
+00011590: 4865 7265 3e3e 0a45 4f46 0a63 686d 6f64  Here>>.EOF.chmod
+000115a0: 206f 672d 7277 2024 5944 415f 484f 4d45   og-rw $YDA_HOME
+000115b0: 2f2e 7373 682f 6175 7468 6f72 697a 6564  /.ssh/authorized
+000115c0: 5f6b 6579 730a 6368 6f77 6e20 2d52 2079  _keys.chown -R y
+000115d0: 642d 6167 656e 743a 7964 2d61 6765 6e74  d-agent:yd-agent
+000115e0: 2024 5944 415f 484f 4d45 2f2e 7373 680a   $YDA_HOME/.ssh.
+000115f0: 6060 600a 0a23 2323 2054 6173 6b20 4578  ```..### Task Ex
+00011600: 6563 7574 696f 6e20 4469 7265 6374 6f72  ecution Director
+00011610: 790a 0a45 7068 656d 6572 616c 2054 6173  y..Ephemeral Tas
+00011620: 6b20 6469 7265 6374 6f72 6965 7320 6172  k directories ar
+00011630: 6520 6279 2064 6566 6175 6c74 2063 7265  e by default cre
+00011640: 6174 6564 2075 6e64 6572 2060 2f76 6172  ated under `/var
+00011650: 2f6f 7074 2f79 656c 6c6f 7764 6f67 2f61  /opt/yellowdog/a
+00011660: 6765 6e74 2f64 6174 612f 776f 726b 6572  gent/data/worker
+00011670: 7360 2e20 5468 6973 2064 6972 6563 746f  s`. This directo
+00011680: 7279 2063 6f6e 7461 696e 7320 6f6e 6520  ry contains one 
+00011690: 6f72 206d 6f72 6520 6e75 6d62 6572 6564  or more numbered
+000116a0: 2073 7562 6469 7265 6374 6f72 6965 7320   subdirectories 
+000116b0: 7768 6572 6520 6561 6368 206e 756d 6265  where each numbe
+000116c0: 7265 6420 6469 7265 6374 6f72 7920 636f  red directory co
+000116d0: 7272 6573 706f 6e64 7320 746f 2061 2057  rresponds to a W
+000116e0: 6f72 6b65 7220 6f6e 2074 6865 206e 6f64  orker on the nod
+000116f0: 652e 0a0a 284f 6e20 5769 6e64 6f77 7320  e...(On Windows 
+00011700: 686f 7374 732c 2074 6865 2054 6173 6b20  hosts, the Task 
+00011710: 6469 7265 6374 6f72 6965 7320 6172 6520  directories are 
+00011720: 666f 756e 6420 756e 6465 7220 6025 4170  found under `%Ap
+00011730: 7044 6174 6125 5c79 656c 6c6f 7764 6f67  pData%\yellowdog
+00011740: 5c61 6765 6e74 5c64 6174 615c 776f 726b  \agent\data\work
+00011750: 6572 7360 2e29 0a0a 5768 656e 2061 2054  ers`.)..When a T
+00011760: 6173 6b20 6973 2061 6c6c 6f63 6174 6564  ask is allocated
+00011770: 2074 6f20 6120 6e6f 6465 2c20 616e 2065   to a node, an e
+00011780: 7068 656d 6572 616c 2064 6972 6563 746f  phemeral directo
+00011790: 7279 2069 7320 6372 6561 7465 6420 756e  ry is created un
+000117a0: 6465 7220 7468 6520 6170 706c 6963 6162  der the applicab
+000117b0: 6c65 2057 6f72 6b65 7220 6469 7265 6374  le Worker direct
+000117c0: 6f72 792c 2077 6974 6820 6120 6e61 6d65  ory, with a name
+000117d0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+000117e0: 6865 2059 656c 6c6f 7744 6f67 2049 4420  he YellowDog ID 
+000117f0: 666f 7220 7468 6520 5461 736b 2e20 466f  for the Task. Fo
+00011800: 7220 6578 616d 706c 652c 2074 6869 7320  r example, this 
+00011810: 6973 2061 6e20 6570 6865 6d65 7261 6c20  is an ephemeral 
+00011820: 6469 7265 6374 6f72 7920 6265 696e 6720  directory being 
+00011830: 7573 6564 2062 7920 576f 726b 6572 206e  used by Worker n
+00011840: 756d 6265 7220 6031 603a 0a0a 602f 7661  umber `1`:..`/va
+00011850: 722f 6f70 742f 7965 6c6c 6f77 646f 672f  r/opt/yellowdog/
+00011860: 6167 656e 742f 6461 7461 2f77 6f72 6b65  agent/data/worke
+00011870: 7273 2f31 2f79 6469 645f 7461 736b 5f35  rs/1/ydid_task_5
+00011880: 3539 4542 455f 3734 3934 3933 3336 2d61  59EBE_74949336-a
+00011890: 6332 622d 3438 3131 2d61 3764 352d 6633  c2b-4811-a7d5-f3
+000118a0: 6563 6439 3733 3939 3038 5f31 5f31 600a  ecd9739908_1_1`.
+000118b0: 0a54 6869 7320 6973 2074 6865 2064 6972  .This is the dir
+000118c0: 6563 746f 7279 2069 6e74 6f20 7768 6963  ectory into whic
+000118d0: 6820 646f 776e 6c6f 6164 6564 206f 626a  h downloaded obj
+000118e0: 6563 7473 2061 7265 2070 6c61 6365 642c  ects are placed,
+000118f0: 2061 6e64 2069 6e20 7768 6963 6820 6f75   and in which ou
+00011900: 7470 7574 2066 696c 6573 2061 7265 2063  tput files are c
+00011910: 7265 6174 6564 2062 7920 6465 6661 756c  reated by defaul
+00011920: 742e 2054 6865 2063 6f6e 736f 6c65 206f  t. The console o
+00011930: 7574 7075 7420 6074 6173 6b6f 7574 7075  utput `taskoutpu
+00011940: 742e 7478 7460 2066 696c 6520 7769 6c6c  t.txt` file will
+00011950: 2061 6c73 6f20 6265 2063 7265 6174 6564   also be created
+00011960: 2069 6e20 7468 6973 2064 6972 6563 746f   in this directo
+00011970: 7279 2e0a 0a53 6565 2074 6865 205b 4669  ry...See the [Fi
+00011980: 6c65 7320 446f 776e 6c6f 6164 6564 2074  les Downloaded t
+00011990: 6f20 6120 4e6f 6465 5d28 2366 696c 6573  o a Node](#files
+000119a0: 2d64 6f77 6e6c 6f61 6465 642d 746f 2d61  -downloaded-to-a
+000119b0: 2d6e 6f64 652d 666f 722d 7573 652d 696e  -node-for-use-in
+000119c0: 2d74 6173 6b2d 6578 6563 7574 696f 6e29  -task-execution)
+000119d0: 2073 6563 7469 6f6e 2061 626f 7665 2066   section above f
+000119e0: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
+000119f0: 6f6e 2068 6f77 2066 696c 6573 2069 6e20  on how files in 
+00011a00: 7468 6973 2064 6972 6563 746f 7279 2061  this directory a
+00011a10: 7265 2068 616e 646c 6564 2e0a 0a41 7420  re handled...At 
+00011a20: 7468 6520 636f 6e63 6c75 7369 6f6e 206f  the conclusion o
+00011a30: 6620 7468 6520 5461 736b 2c20 6166 7465  f the Task, afte
+00011a40: 7220 616e 7920 6669 6c65 7320 7265 7175  r any files requ
+00011a50: 6573 7465 6420 666f 7220 7570 6c6f 6164  ested for upload
+00011a60: 2068 6176 6520 6265 656e 2075 706c 6f61   have been uploa
+00011a70: 6465 6420 746f 2074 6865 204f 626a 6563  ded to the Objec
+00011a80: 7420 5374 6f72 6520 2873 6565 2074 6865  t Store (see the
+00011a90: 205b 4669 6c65 7320 5570 6c6f 6164 6564   [Files Uploaded
+00011aa0: 2066 726f 6d20 6120 4e6f 6465 5d28 2366   from a Node](#f
+00011ab0: 696c 6573 2d75 706c 6f61 6465 642d 6672  iles-uploaded-fr
+00011ac0: 6f6d 2d61 2d6e 6f64 652d 746f 2d74 6865  om-a-node-to-the
+00011ad0: 2d6f 626a 6563 742d 7374 6f72 652d 6166  -object-store-af
+00011ae0: 7465 722d 7461 736b 2d65 7865 6375 7469  ter-task-executi
+00011af0: 6f6e 2920 7365 6374 696f 6e20 666f 7220  on) section for 
+00011b00: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00011b10: 292c 2074 6865 2060 7964 6964 5f74 6173  ), the `ydid_tas
+00011b20: 6b5f 3535 3945 4245 5f37 3439 3439 3333  k_559EBE_7494933
+00011b30: 362d 6163 3262 2d34 3831 312d 6137 6435  6-ac2b-4811-a7d5
+00011b40: 2d66 3365 6364 3937 3339 3930 385f 315f  -f3ecd9739908_1_
+00011b50: 3160 2077 696c 6c20 6265 2072 656d 6f76  1` will be remov
+00011b60: 6564 2e0a 0a23 2320 5370 6563 6966 7969  ed...## Specifyi
+00011b70: 6e67 2057 6f72 6b20 5265 7175 6972 656d  ng Work Requirem
+00011b80: 656e 7473 2075 7369 6e67 2043 5356 2044  ents using CSV D
+00011b90: 6174 610a 0a43 5356 2064 6174 6120 6669  ata..CSV data fi
+00011ba0: 6c65 7320 6361 6e20 6265 2075 7365 6420  les can be used 
+00011bb0: 746f 2064 7269 7665 2074 6865 2067 656e  to drive the gen
+00011bc0: 6572 6174 696f 6e20 6f66 206c 6973 7473  eration of lists
+00011bd0: 206f 6620 5461 736b 732c 2061 7320 666f   of Tasks, as fo
+00011be0: 6c6c 6f77 733a 0a0a 2d20 4120 2a2a 7072  llows:..- A **pr
+00011bf0: 6f74 6f74 7970 652a 2a20 5461 736b 2073  ototype** Task s
+00011c00: 7065 6369 6669 6361 7469 6f6e 2069 7320  pecification is 
+00011c10: 6372 6561 7465 6420 7769 7468 696e 2061  created within a
+00011c20: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
+00011c30: 7265 6d65 6e74 2073 7065 6369 6669 6361  rement specifica
+00011c40: 7469 6f6e 206f 7220 696e 2074 6865 2060  tion or in the `
+00011c50: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+00011c60: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+00011c70: 544f 4d4c 2063 6f6e 6669 6775 7261 7469  TOML configurati
+00011c80: 6f6e 2066 696c 650a 2d20 5468 6520 7072  on file.- The pr
+00011c90: 6f74 6f74 7970 6520 7461 736b 2069 6e63  ototype task inc
+00011ca0: 6c75 6465 7320 6f6e 6520 6f72 206d 6f72  ludes one or mor
+00011cb0: 6520 7661 7269 6162 6c65 2073 7562 7374  e variable subst
+00011cc0: 6974 7574 696f 6e73 0a2d 2041 2043 5356  itutions.- A CSV
+00011cd0: 2066 696c 6520 6973 2063 7265 6174 6564   file is created
+00011ce0: 2c20 7769 7468 2074 6865 202a 2a68 6561  , with the **hea
+00011cf0: 6465 7273 2a2a 2028 6669 7273 7420 726f  ders** (first ro
+00011d00: 7729 206d 6174 6368 696e 6720 7468 6520  w) matching the 
+00011d10: 6e61 6d65 7320 6f66 2074 6865 2076 6172  names of the var
+00011d20: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00011d30: 6f6e 7320 696e 2074 6865 2054 6173 6b20  ons in the Task 
+00011d40: 7072 6f74 6f74 7970 650a 2d20 4561 6368  prototype.- Each
+00011d50: 2073 7562 7365 7175 656e 7420 726f 7720   subsequent row 
+00011d60: 6f66 2074 6865 2043 5356 2066 696c 6520  of the CSV file 
+00011d70: 7265 7072 6573 656e 7473 2061 206e 6577  represents a new
+00011d80: 2054 6173 6b20 6275 696c 7420 7573 696e   Task built usin
+00011d90: 6720 7468 6520 7072 6f74 6f74 7970 652c  g the prototype,
+00011da0: 2077 6974 6820 7468 6520 7661 7269 6162   with the variab
+00011db0: 6c65 7320 7375 6273 7469 7475 7465 6420  les substituted 
+00011dc0: 6279 2074 6865 2076 616c 7565 7320 696e  by the values in
+00011dd0: 2074 6865 2072 6f77 0a2d 2041 2054 6173   the row.- A Tas
+00011de0: 6b20 7769 6c6c 2062 6520 6372 6561 7465  k will be create
+00011df0: 6420 666f 7220 6561 6368 2064 6174 6120  d for each data 
+00011e00: 726f 770a 0a23 2323 2057 6f72 6b20 5265  row..### Work Re
+00011e10: 7175 6972 656d 656e 7420 4353 5620 4461  quirement CSV Da
+00011e20: 7461 2045 7861 6d70 6c65 0a0a 4173 2061  ta Example..As a
+00011e30: 6e20 6578 616d 706c 652c 2063 6f6e 7369  n example, consi
+00011e40: 6465 7220 7468 6520 666f 6c6c 6f77 696e  der the followin
+00011e50: 6720 4a53 4f4e 2057 6f72 6b20 5265 7175  g JSON Work Requ
+00011e60: 6972 656d 656e 7420 6077 722e 6a73 6f6e  irement `wr.json
+00011e70: 603a 0a0a 6060 606a 736f 6e0a 7b0a 2020  `:..```json.{.  
+00011e80: 2274 6173 6b47 726f 7570 7322 3a20 5b0a  "taskGroups": [.
+00011e90: 2020 2020 7b0a 2020 2020 2020 2274 6173      {.      "tas
+00011ea0: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
+00011eb0: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
+00011ec0: 6d65 6e74 7322 3a20 5b22 7b7b 6172 675f  ments": ["{{arg_
+00011ed0: 317d 7d22 2c20 227b 7b61 7267 5f32 7d7d  1}}", "{{arg_2}}
+00011ee0: 222c 2022 7b7b 6172 675f 337d 7d22 5d2c  ", "{{arg_3}}"],
+00011ef0: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
+00011f00: 726f 6e6d 656e 7422 3a20 7b22 454e 565f  ronment": {"ENV_
+00011f10: 5641 525f 3122 3a20 227b 7b65 6e76 5f31  VAR_1": "{{env_1
+00011f20: 7d7d 227d 0a20 2020 2020 2020 207d 0a20  }}"}.        }. 
+00011f30: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+00011f40: 0a7d 0a60 6060 0a0a 4e6f 7465 2074 6861  .}.```..Note tha
+00011f50: 7420 7468 6520 5461 736b 2047 726f 7570  t the Task Group
+00011f60: 206d 7573 7420 636f 6e74 6169 6e20 6f6e   must contain on
+00011f70: 6c79 2061 2073 696e 676c 6520 5461 736b  ly a single Task
+00011f80: 2c20 6163 7469 6e67 2061 7320 7468 6520  , acting as the 
+00011f90: 7072 6f74 6f74 7970 652e 0a0a 4e6f 7720  prototype...Now 
+00011fa0: 636f 6e73 6964 6572 2061 2043 5356 2066  consider a CSV f
+00011fb0: 696c 6520 6077 725f 6461 7461 2e63 7376  ile `wr_data.csv
+00011fc0: 6020 7769 7468 2074 6865 2066 6f6c 6c6f  ` with the follo
+00011fd0: 7769 6e67 2063 6f6e 7465 6e74 733a 0a0a  wing contents:..
+00011fe0: 6060 6074 6578 740a 6172 675f 312c 2061  ```text.arg_1, a
+00011ff0: 7267 5f32 2c20 6172 675f 332c 2065 6e76  rg_2, arg_3, env
+00012000: 5f31 0a41 2c20 2020 2020 422c 2020 2020  _1.A,     B,    
+00012010: 2043 2c20 2020 2020 452d 310a 442c 2020   C,     E-1.D,  
+00012020: 2020 2045 2c20 2020 2020 462c 2020 2020     E,     F,    
+00012030: 2045 2d32 0a47 2c20 2020 2020 482c 2020   E-2.G,     H,  
+00012040: 2020 2049 2c20 2020 2020 452d 330a 6060     I,     E-3.``
+00012050: 600a 0a4e 6f74 6520 7468 6174 2074 6865  `..Note that the
+00012060: 2028 6f70 7469 6f6e 616c 2920 6c65 6164   (optional) lead
+00012070: 696e 6720 7370 6163 6573 2061 6674 6572  ing spaces after
+00012080: 2065 6163 6820 636f 6d6d 6120 6172 6520   each comma are 
+00012090: 6967 6e6f 7265 642c 2062 7574 2074 7261  ignored, but tra
+000120a0: 696c 696e 6720 7370 6163 6573 2061 7265  iling spaces are
+000120b0: 206e 6f74 2061 6e64 2077 696c 6c20 666f   not and will fo
+000120c0: 726d 2070 6172 7420 6f66 2074 6865 2069  rm part of the i
+000120d0: 6d70 6f72 7465 6420 6461 7461 2e0a 0a49  mported data...I
+000120e0: 6620 7468 6573 6520 6669 6c65 7320 6172  f these files ar
+000120f0: 6520 7072 6f63 6573 7365 6420 7573 696e  e processed usin
+00012100: 6720 6079 642d 7375 626d 6974 202d 7220  g `yd-submit -r 
+00012110: 7772 2e6a 736f 6e20 2d56 2077 725f 6461  wr.json -V wr_da
+00012120: 7461 2e63 7376 602c 2074 6865 2066 6f6c  ta.csv`, the fol
+00012130: 6c6f 7769 6e67 2065 7870 616e 6465 6420  lowing expanded 
+00012140: 6c69 7374 206f 6620 7468 7265 6520 5461  list of three Ta
+00012150: 736b 7320 7769 6c6c 2062 6520 6372 6561  sks will be crea
+00012160: 7465 6420 7072 696f 7220 746f 2066 7572  ted prior to fur
+00012170: 7468 6572 2070 726f 6365 7373 696e 6720  ther processing 
+00012180: 6279 2074 6865 2060 7964 2d73 7562 6d69  by the `yd-submi
+00012190: 7460 2073 6372 6970 743a 0a0a 6060 606a  t` script:..```j
+000121a0: 736f 6e0a 7b0a 2020 2274 6173 6b47 726f  son.{.  "taskGro
+000121b0: 7570 7322 3a20 5b0a 2020 2020 7b0a 2020  ups": [.    {.  
+000121c0: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
+000121d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000121e0: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
+000121f0: 5b22 4122 2c20 2242 222c 2022 4322 5d2c  ["A", "B", "C"],
+00012200: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
+00012210: 726f 6e6d 656e 7422 3a20 7b22 454e 565f  ronment": {"ENV_
+00012220: 5641 525f 3122 3a20 2245 2d31 227d 0a20  VAR_1": "E-1"}. 
+00012230: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00012240: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00012250: 7267 756d 656e 7473 223a 205b 2244 222c  rguments": ["D",
+00012260: 2022 4522 2c20 2246 225d 2c0a 2020 2020   "E", "F"],.    
+00012270: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
+00012280: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
+00012290: 223a 2022 452d 3222 7d0a 2020 2020 2020  ": "E-2"}.      
+000122a0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+000122b0: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+000122c0: 6e74 7322 3a20 5b22 4722 2c20 2248 222c  nts": ["G", "H",
+000122d0: 2022 4922 5d2c 0a20 2020 2020 2020 2020   "I"],.         
+000122e0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+000122f0: 7b22 454e 565f 5641 525f 3122 3a20 2245  {"ENV_VAR_1": "E
+00012300: 2d33 227d 0a20 2020 2020 2020 207d 0a20  -3"}.        }. 
+00012310: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+00012320: 0a7d 0a60 6060 0a0a 2323 2320 4353 5620  .}.```..### CSV 
+00012330: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
+00012340: 7574 696f 6e73 0a0a 5768 656e 2074 6865  utions..When the
+00012350: 2043 5356 2066 696c 6520 6461 7461 2069   CSV file data i
+00012360: 7320 7072 6f63 6573 7365 642c 2074 6865  s processed, the
+00012370: 206f 6e6c 7920 7375 6273 7469 7475 7469   only substituti
+00012380: 6f6e 7320 6d61 6465 2061 7265 2074 686f  ons made are tho
+00012390: 7365 2077 6869 6368 206d 6174 6368 2074  se which match t
+000123a0: 6865 2076 6172 6961 626c 6520 7375 6273  he variable subs
+000123b0: 7469 7475 7469 6f6e 7320 696e 2074 6865  titutions in the
+000123c0: 2070 726f 746f 7479 7065 2054 6173 6b2e   prototype Task.
+000123d0: 2054 6865 2043 5356 2066 696c 6520 6973   The CSV file is
+000123e0: 2074 6865 202a 2a6f 6e6c 792a 2a20 736f   the **only** so
+000123f0: 7572 6365 206f 6620 7375 6273 7469 7475  urce of substitu
+00012400: 7469 6f6e 7320 7573 6564 2066 6f72 2074  tions used for t
+00012410: 6869 7320 7072 6f63 6573 7369 6e67 2070  his processing p
+00012420: 6861 7365 3b20 616c 6c20 6f74 6865 7220  hase; all other 
+00012430: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+00012440: 7574 696f 6e73 2028 7375 7070 6c69 6564  utions (supplied
+00012450: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
+00012460: 6c69 6e65 2c20 696e 2074 6865 2054 4f4d  line, in the TOM
+00012470: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+00012480: 6669 6c65 2c20 6f72 2066 726f 6d20 656e  file, or from en
+00012490: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+000124a0: 6c65 7329 2061 7265 2069 676e 6f72 6564  les) are ignored
+000124b0: 202d 2d20 692e 652e 2c20 7468 6579 2064   -- i.e., they d
+000124c0: 6f20 6e6f 7420 6f76 6572 7269 6465 2074  o not override t
+000124d0: 6865 2063 6f6e 7465 6e74 7320 6f66 2074  he contents of t
+000124e0: 6865 2043 5356 2066 696c 652e 0a0a 416c  he CSV file...Al
+000124f0: 6c20 7661 7269 6162 6c65 2073 7562 7374  l variable subst
+00012500: 6974 7574 696f 6e73 2075 6e72 656c 6174  itutions unrelat
+00012510: 6564 2074 6f20 7468 6520 4353 5620 6669  ed to the CSV fi
+00012520: 6c65 2064 6174 6120 6172 6520 6c65 6674  le data are left
+00012530: 2075 6e63 6861 6e67 6564 2c20 666f 7220   unchanged, for 
+00012540: 7375 6273 6571 7565 6e74 2070 726f 6365  subsequent proce
+00012550: 7373 696e 6720 6279 2060 7964 2d73 7562  ssing by `yd-sub
+00012560: 6d69 7460 2e0a 0a49 6620 7468 6520 7661  mit`...If the va
+00012570: 6c75 6520 746f 2062 6520 696e 7365 7274  lue to be insert
+00012580: 6564 2069 7320 6120 6e75 6d62 6572 2028  ed is a number (
+00012590: 616e 2069 6e74 6567 6572 206f 7220 666c  an integer or fl
+000125a0: 6f61 7469 6e67 2070 6f69 6e74 2076 616c  oating point val
+000125b0: 7565 2920 6f72 2042 6f6f 6c65 616e 2c20  ue) or Boolean, 
+000125c0: 7468 6520 607b 7b6e 756d 3a6d 795f 6e75  the `{{num:my_nu
+000125d0: 6d62 6572 5f76 6172 7d7d 6020 616e 6420  mber_var}}` and 
+000125e0: 607b 7b62 6f6f 6c3a 6d79 5f62 6f6f 6c65  `{{bool:my_boole
+000125f0: 616e 5f76 6172 7d7d 6020 666f 726d 7320  an_var}}` forms 
+00012600: 6361 6e20 6265 2075 7365 6420 696e 2074  can be used in t
+00012610: 6865 204a 534f 4e20 6669 6c65 2c20 6173  he JSON file, as
+00012620: 2077 6974 6820 7468 6569 7220 7573 6520   with their use 
+00012630: 696e 206f 7468 6572 2070 6172 7473 206f  in other parts o
+00012640: 6620 7468 6520 4a53 4f4e 2057 6f72 6b20  f the JSON Work 
+00012650: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
+00012660: 6966 6963 6174 696f 6e2e 2054 6865 2073  ification. The s
+00012670: 7562 7374 6974 7574 6564 2076 616c 7565  ubstituted value
+00012680: 2077 696c 6c20 6173 7375 6d65 2074 6865   will assume the
+00012690: 206e 6f6d 696e 6174 6564 2074 7970 6520   nominated type 
+000126a0: 7261 7468 6572 2074 6861 6e20 6265 696e  rather than bein
+000126b0: 6720 6120 7374 7269 6e67 2e0a 0a23 2323  g a string...###
+000126c0: 2050 726f 7065 7274 7920 496e 6865 7269   Property Inheri
+000126d0: 7461 6e63 650a 0a41 6c6c 2074 6865 2075  tance..All the u
+000126e0: 7375 616c 2070 726f 7065 7274 7920 696e  sual property in
+000126f0: 6865 7269 7461 6e63 6520 6665 6174 7572  heritance featur
+00012700: 6573 206f 7065 7261 7465 2061 7320 6e6f  es operate as no
+00012710: 726d 616c 2e20 5072 6f70 6572 7469 6573  rmal. Properties
+00012720: 2061 7265 2069 6e68 6572 6974 6564 2066   are inherited f
+00012730: 726f 6d20 7468 6520 6063 6f6e 6669 672e  rom the `config.
+00012740: 746f 6d6c 6020 6669 6c65 2c20 616e 6420  toml` file, and 
+00012750: 6672 6f6d 2074 6865 2072 656c 6576 616e  from the relevan
+00012760: 7420 7365 6374 696f 6e73 206f 6620 7468  t sections of th
+00012770: 6520 4a53 4f4e 2057 6f72 6b20 5265 7175  e JSON Work Requ
+00012780: 6972 656d 656e 7420 6669 6c65 2e20 416e  irement file. An
+00012790: 7920 7072 6f70 6572 7469 6573 2073 6574  y properties set
+000127a0: 2077 6974 6869 6e20 6120 5461 736b 2070   within a Task p
+000127b0: 726f 746f 7479 7065 2061 7265 2063 6f70  rototype are cop
+000127c0: 6965 6420 746f 2061 6c6c 2074 6865 2067  ied to all the g
+000127d0: 656e 6572 6174 6564 2054 6173 6b73 2e0a  enerated Tasks..
+000127e0: 0a23 2323 204d 756c 7469 706c 6520 5461  .### Multiple Ta
+000127f0: 736b 2047 726f 7570 7320 7573 696e 6720  sk Groups using 
+00012800: 4d75 6c74 6970 6c65 2043 5356 2046 696c  Multiple CSV Fil
+00012810: 6573 0a0a 5468 6520 7573 6520 6f66 206d  es..The use of m
+00012820: 756c 7469 706c 6520 5461 736b 2047 726f  ultiple Task Gro
+00012830: 7570 7320 6973 2061 6c73 6f20 7375 7070  ups is also supp
+00012840: 6f72 7465 642c 2062 7920 7573 696e 6720  orted, by using 
+00012850: 6f6e 6520 4353 5620 6669 6c65 2070 6572  one CSV file per
+00012860: 2054 6173 6b20 4772 6f75 702e 2045 6163   Task Group. Eac
+00012870: 6820 5461 736b 2047 726f 7570 206d 7573  h Task Group mus
+00012880: 7420 636f 6e74 6169 6e20 6f6e 6c79 2061  t contain only a
+00012890: 2073 696e 676c 6520 7072 6f74 6f74 7970   single prototyp
+000128a0: 6520 5461 736b 2e0a 0a54 6865 2043 5356  e Task...The CSV
+000128b0: 2066 696c 6573 2061 7265 2073 7570 706c   files are suppl
+000128c0: 6965 6420 6f6e 2074 6865 2063 6f6d 6d61  ied on the comma
+000128d0: 6e64 206c 696e 6520 696e 2074 6865 206f  nd line in the o
+000128e0: 7264 6572 206f 6620 7468 6520 5461 736b  rder of the Task
+000128f0: 2047 726f 7570 7320 746f 2077 6869 6368   Groups to which
+00012900: 2074 6865 7920 6170 706c 792e 2046 6f72   they apply. For
+00012910: 2065 7861 6d70 6c65 2c20 6966 2060 7772   example, if `wr
+00012920: 5f6a 736f 6e60 2063 6f6e 7461 696e 7320  _json` contains 
+00012930: 7477 6f20 5461 736b 2047 726f 7570 732c  two Task Groups,
+00012940: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
+00012950: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
+00012960: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+00012970: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+00012980: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00012990: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+000129a0: 3a20 5b22 7b7b 6172 675f 317d 7d22 2c20  : ["{{arg_1}}", 
+000129b0: 227b 7b61 7267 5f32 7d7d 222c 2022 7b7b  "{{arg_2}}", "{{
+000129c0: 6172 675f 337d 7d22 5d2c 0a20 2020 2020  arg_3}}"],.     
+000129d0: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+000129e0: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
+000129f0: 3a20 227b 7b65 6e76 5f31 7d7d 227d 0a20  : "{{env_1}}"}. 
+00012a00: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00012a10: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00012a20: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
+00012a30: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00012a40: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
+00012a50: 5b22 7b7b 6172 675f 317d 7d22 2c20 227b  ["{{arg_1}}", "{
+00012a60: 7b61 7267 5f32 7d7d 225d 2c0a 2020 2020  {arg_2}}"],.    
+00012a70: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
+00012a80: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
+00012a90: 223a 2022 7b7b 656e 765f 317d 7d22 2c20  ": "{{env_1}}", 
+00012aa0: 2245 4e56 5f56 4152 5f32 223a 2022 7b7b  "ENV_VAR_2": "{{
+00012ab0: 656e 765f 327d 7d22 7d0a 2020 2020 2020  env_2}}"}.      
+00012ac0: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00012ad0: 7d0a 2020 5d0a 7d0a 6060 600a 0a54 6865  }.  ].}.```..The
+00012ae0: 2060 7964 2d73 7562 6d69 7460 2063 6f6d   `yd-submit` com
+00012af0: 6d61 6e64 2077 6f75 6c64 2074 6865 6e20  mand would then 
+00012b00: 6265 2069 6e76 6f6b 6564 2077 6974 6820  be invoked with 
+00012b10: 6120 7365 7061 7261 7465 2043 5356 2066  a separate CSV f
+00012b20: 696c 6520 666f 7220 6561 6368 2054 6173  ile for each Tas
+00012b30: 6b20 4772 6f75 702c 2065 2e67 2e3a 0a0a  k Group, e.g.:..
+00012b40: 6060 6073 6865 6c6c 0a79 642d 7375 626d  ```shell.yd-subm
+00012b50: 6974 202d 7220 7772 2e6a 736f 6e20 2d56  it -r wr.json -V
+00012b60: 2077 725f 6461 7461 5f74 6173 6b5f 6772   wr_data_task_gr
+00012b70: 6f75 705f 312e 6373 7620 2d56 2077 725f  oup_1.csv -V wr_
+00012b80: 6461 7461 5f74 6173 6b5f 6772 6f75 705f  data_task_group_
+00012b90: 322e 6373 760a 6060 600a 0a49 6620 7468  2.csv.```..If th
+00012ba0: 6572 6520 6172 6520 2a2a 6665 7765 722a  ere are **fewer*
+00012bb0: 2a20 4353 5620 6669 6c65 7320 7468 616e  * CSV files than
+00012bc0: 2054 6173 6b20 4772 6f75 7073 2061 2077   Task Groups a w
+00012bd0: 6172 6e69 6e67 2077 696c 6c20 6265 2070  arning will be p
+00012be0: 7269 6e74 6564 2061 6e64 2c20 6966 2074  rinted and, if t
+00012bf0: 6865 7265 2061 7265 2027 6e27 2043 5356  here are 'n' CSV
+00012c00: 2066 696c 6573 2c20 4353 5620 6461 7461   files, CSV data
+00012c10: 2070 726f 6365 7373 696e 6720 7769 6c6c   processing will
+00012c20: 2062 6520 6170 706c 6965 6420 746f 2074   be applied to t
+00012c30: 6865 2066 6972 7374 2027 6e27 2054 6173  he first 'n' Tas
+00012c40: 6b20 4772 6f75 7073 2069 6e20 7468 6520  k Groups in the 
+00012c50: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00012c60: 2062 7920 6465 6661 756c 742c 2069 6e20   by default, in 
+00012c70: 7468 6520 6f72 6465 7220 696e 2077 6869  the order in whi
+00012c80: 6368 2074 6865 2043 5356 2066 696c 6573  ch the CSV files
+00012c90: 2077 6572 6520 7375 7070 6c69 6564 2e20   were supplied. 
+00012ca0: 4966 2074 6865 7265 2061 7265 202a 2a6d  If there are **m
+00012cb0: 6f72 652a 2a20 4353 5620 6669 6c65 7320  ore** CSV files 
+00012cc0: 7468 616e 2054 6173 6b20 4772 6f75 7073  than Task Groups
+00012cd0: 2c20 616e 2065 7272 6f72 2077 696c 6c20  , an error will 
+00012ce0: 6265 2072 6169 7365 6420 616e 6420 7072  be raised and pr
+00012cf0: 6f63 6573 7369 6e67 2077 696c 6c20 7374  ocessing will st
+00012d00: 6f70 2e0a 0a49 7420 6973 2070 6f73 7369  op...It is possi
+00012d10: 626c 6520 746f 2061 7070 6c79 2043 5356  ble to apply CSV
+00012d20: 2066 696c 6573 2065 7870 6c69 6369 746c   files explicitl
+00012d30: 7920 746f 2073 7065 6369 6669 6320 5461  y to specific Ta
+00012d40: 736b 2047 726f 7570 732c 2062 7920 7573  sk Groups, by us
+00012d50: 696e 6720 616e 206f 7074 696f 6e61 6c20  ing an optional 
+00012d60: 2a2a 696e 6465 7820 706f 7374 6669 782a  **index postfix*
+00012d70: 2a20 2865 2e67 2e2c 2060 3a32 6029 2061  * (e.g., `:2`) a
+00012d80: 7420 7468 6520 656e 6420 6f66 2065 6163  t the end of eac
+00012d90: 6820 4353 5620 6669 6c65 6e61 6d65 2e20  h CSV filename. 
+00012da0: 466f 7220 6578 616d 706c 652c 2069 6620  For example, if 
+00012db0: 7468 6572 6520 6172 6520 7477 6f20 4353  there are two CS
+00012dc0: 5620 6669 6c65 7320 746f 2062 6520 6170  V files to be ap
+00012dd0: 706c 6965 6420 746f 2074 6865 2073 6563  plied to the sec
+00012de0: 6f6e 6420 616e 6420 666f 7572 7468 2054  ond and fourth T
+00012df0: 6173 6b20 4772 6f75 7073 2069 6e20 6120  ask Groups in a 
+00012e00: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
+00012e10: 656d 656e 742c 2075 7365 2074 6865 2066  ement, use the f
+00012e20: 6f6c 6c6f 7769 6e67 2073 796e 7461 783a  ollowing syntax:
+00012e30: 0a0a 6060 6073 6865 6c6c 0a79 642d 7375  ..```shell.yd-su
+00012e40: 626d 6974 202d 7220 7772 2e6a 736f 6e20  bmit -r wr.json 
+00012e50: 2d56 2077 725f 6461 7461 5f74 6173 6b5f  -V wr_data_task_
+00012e60: 6772 6f75 705f 322e 6373 763a 3220 2d56  group_2.csv:2 -V
+00012e70: 2077 725f 6461 7461 5f74 6173 6b5f 6772   wr_data_task_gr
+00012e80: 6f75 705f 342e 6373 763a 340a 6060 600a  oup_4.csv:4.```.
+00012e90: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+00012ea0: 7468 6520 2a2a 5461 736b 2047 726f 7570  the **Task Group
+00012eb0: 206e 616d 652a 2a20 2869 6620 7375 7070   name** (if supp
+00012ec0: 6c69 6564 2069 6e20 7468 6520 4a53 4f4e  lied in the JSON
+00012ed0: 2066 696c 6529 2063 616e 2062 6520 7573   file) can be us
+00012ee0: 6564 2061 7320 7468 6520 706f 7374 6669  ed as the postfi
+00012ef0: 782e 2046 6f72 2065 7861 6d70 6c65 2c20  x. For example, 
+00012f00: 6966 2074 6865 2054 6173 6b20 4772 6f75  if the Task Grou
+00012f10: 7073 2061 626f 7665 2061 7265 206e 616d  ps above are nam
+00012f20: 6564 2060 7467 5f74 776f 6020 616e 6420  ed `tg_two` and 
+00012f30: 6074 675f 666f 7572 602c 2074 6865 2060  `tg_four`, the `
+00012f40: 7964 2d73 7562 6d69 7460 2063 6f6d 6d61  yd-submit` comma
+00012f50: 6e64 2077 6f75 6c64 2062 6563 6f6d 653a  nd would become:
+00012f60: 0a0a 6060 6073 6865 6c6c 0a79 642d 7375  ..```shell.yd-su
+00012f70: 626d 6974 202d 7220 7772 2e6a 736f 6e20  bmit -r wr.json 
+00012f80: 2d56 2077 725f 6461 7461 5f74 6173 6b5f  -V wr_data_task_
+00012f90: 6772 6f75 705f 322e 6373 763a 7467 5f74  group_2.csv:tg_t
+00012fa0: 776f 202d 5620 7772 5f64 6174 615f 7461  wo -V wr_data_ta
+00012fb0: 736b 5f67 726f 7570 5f34 2e63 7376 3a74  sk_group_4.csv:t
+00012fc0: 675f 666f 7572 0a60 6060 0a0a 4e6f 7465  g_four.```..Note
+00012fd0: 2074 6861 7420 6f6e 6c79 206f 6e65 2043   that only one C
+00012fe0: 5356 2066 696c 6520 6361 6e20 6265 2061  SV file can be a
+00012ff0: 7070 6c69 6564 2074 6f20 616e 7920 6769  pplied to any gi
+00013000: 7665 6e20 5461 736b 2047 726f 7570 2e20  ven Task Group. 
+00013010: 4120 7369 6e67 6c65 2043 5356 2066 696c  A single CSV fil
+00013020: 6520 6361 6e2c 2068 6f77 6576 6572 2c20  e can, however, 
+00013030: 6265 2072 6575 7365 6420 666f 7220 6d75  be reused for mu
+00013040: 6c74 6970 6c65 2054 6173 6b20 4772 6f75  ltiple Task Grou
+00013050: 7073 2e0a 0a23 2323 2055 7369 6e67 2043  ps...### Using C
+00013060: 5356 2044 6174 6120 7769 7468 2053 696d  SV Data with Sim
+00013070: 706c 652c 2054 4f4d 4c2d 4f6e 6c79 2057  ple, TOML-Only W
+00013080: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+00013090: 5370 6563 6966 6963 6174 696f 6e73 0a0a  Specifications..
+000130a0: 4974 2773 2070 6f73 7369 626c 6520 746f  It's possible to
+000130b0: 2075 7365 2054 4f4d 4c20 6578 636c 7573   use TOML exclus
+000130c0: 6976 656c 7920 746f 2064 6572 6976 6520  ively to derive 
+000130d0: 6120 6c69 7374 206f 6620 5461 736b 7320  a list of Tasks 
+000130e0: 6672 6f6d 2043 5356 2064 6174 6120 2d2d  from CSV data --
+000130f0: 2069 2e65 2e2c 2061 204a 534f 4e20 576f   i.e., a JSON Wo
+00013100: 726b 2052 6571 7569 7265 6d65 6e74 2073  rk Requirement s
+00013110: 7065 6369 6669 6361 7469 6f6e 2069 7320  pecification is 
+00013120: 6e6f 7420 7265 7175 6972 6564 2e0a 0a54  not required...T
+00013130: 6f20 6d61 6b65 2075 7365 206f 6620 7468  o make use of th
+00013140: 6973 3a0a 0a31 2e20 456e 7375 7265 2074  is:..1. Ensure t
+00013150: 6861 7420 6e6f 204a 534f 4e20 576f 726b  hat no JSON Work
+00013160: 2052 6571 7569 7265 6d65 6e74 2064 6f63   Requirement doc
+00013170: 756d 656e 7420 6973 2073 7065 6369 6669  ument is specifi
+00013180: 6564 2028 6e6f 2060 776f 726b 5265 7175  ed (no `workRequ
+00013190: 6972 656d 656e 7444 6174 6160 2069 6e20  irementData` in 
+000131a0: 7468 6520 544f 4d4c 2066 696c 652c 206f  the TOML file, o
+000131b0: 7220 602d 2d77 6f72 6b2d 7265 7175 6972  r `--work-requir
+000131c0: 656d 656e 7460 206f 6e20 7468 6520 636f  ement` on the co
+000131d0: 6d6d 616e 6420 6c69 6e65 290a 322e 2049  mmand line).2. I
+000131e0: 6e73 6572 7420 7468 6520 7265 7175 6972  nsert the requir
+000131f0: 6564 2043 5356 2d73 7570 706c 6965 6420  ed CSV-supplied 
+00013200: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+00013210: 7574 696f 6e73 2064 6972 6563 746c 7920  utions directly 
+00013220: 696e 746f 2074 6865 2054 4f4d 4c20 7072  into the TOML pr
+00013230: 6f70 6572 7469 6573 2c20 652e 672e 2060  operties, e.g. `
+00013240: 6172 6775 6d65 6e74 7320 3d20 5b22 7b7b  arguments = ["{{
+00013250: 6172 675f 317d 7d22 2c20 227b 7b61 7267  arg_1}}", "{{arg
+00013260: 5f32 7d7d 225d 600a 332e 2053 7065 6369  _2}}"]`.3. Speci
+00013270: 6679 2061 2073 696e 676c 6520 4353 5620  fy a single CSV 
+00013280: 6669 6c65 2069 6e20 7468 6520 6063 7376  file in the `csv
+00013290: 4669 6c65 7360 2054 4f4d 4c20 7072 6f70  Files` TOML prop
+000132a0: 6572 7479 2c20 652e 672e 2060 6373 7646  erty, e.g. `csvF
+000132b0: 696c 6573 203d 205b 2277 725f 6461 7461  iles = ["wr_data
+000132c0: 2e63 7376 225d 602c 206f 7220 7072 6f76  .csv"]`, or prov
+000132d0: 6964 6520 7468 6520 4353 5620 6669 6c65  ide the CSV file
+000132e0: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
+000132f0: 6c69 6e65 2060 2d56 2077 725f 6461 7461  line `-V wr_data
+00013300: 2e63 7376 600a 0a57 6865 6e20 6079 642d  .csv`..When `yd-
+00013310: 7375 626d 6974 6020 6973 2072 756e 2c20  submit` is run, 
+00013320: 6974 2077 696c 6c20 6578 7061 6e64 2074  it will expand t
+00013330: 6865 2054 6173 6b20 6c69 7374 2074 6f20  he Task list to 
+00013340: 6d61 7463 6820 7468 6520 6e75 6d62 6572  match the number
+00013350: 206f 6620 6461 7461 2072 6f77 7320 696e   of data rows in
+00013360: 2074 6865 2043 5356 2066 696c 652e 0a0a   the CSV file...
+00013370: 2323 2320 496e 7370 6563 7469 6e67 2074  ### Inspecting t
+00013380: 6865 2052 6573 756c 7473 206f 6620 4353  he Results of CS
+00013390: 5620 5661 7269 6162 6c65 2053 7562 7374  V Variable Subst
+000133a0: 6974 7574 696f 6e0a 0a54 6865 2060 2d2d  itution..The `--
+000133b0: 7072 6f63 6573 732d 6373 762d 6f6e 6c79  process-csv-only
+000133c0: 6020 286f 7220 602d 7060 2920 6f70 7469  ` (or `-p`) opti
+000133d0: 6f6e 2063 616e 2062 6520 7573 6564 2077  on can be used w
+000133e0: 6974 6820 6079 642d 7375 626d 6974 6020  ith `yd-submit` 
+000133f0: 746f 206f 7574 7075 7420 7468 6520 4a53  to output the JS
+00013400: 4f4e 2057 6f72 6b20 5265 7175 6972 656d  ON Work Requirem
+00013410: 656e 7420 6166 7465 7220 4353 5620 7661  ent after CSV va
+00013420: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+00013430: 696f 6e73 206f 6e6c 792c 2070 7269 6f72  ions only, prior
+00013440: 2074 6f20 616c 6c20 6f74 6865 7220 7375   to all other su
+00013450: 6273 7469 7475 7469 6f6e 7320 616e 6420  bstitutions and 
+00013460: 7072 6f70 6572 7479 2069 6e68 6572 6974  property inherit
+00013470: 616e 6365 2061 7070 6c69 6564 2062 7920  ance applied by 
+00013480: 6079 642d 7375 626d 6974 602e 0a0a 2320  `yd-submit`...# 
+00013490: 576f 726b 6572 2050 6f6f 6c20 5072 6f70  Worker Pool Prop
+000134a0: 6572 7469 6573 0a0a 5468 6520 6077 6f72  erties..The `wor
+000134b0: 6b65 7250 6f6f 6c60 2073 6563 7469 6f6e  kerPool` section
+000134c0: 206f 6620 7468 6520 544f 4d4c 2066 696c   of the TOML fil
+000134d0: 6520 6465 6669 6e65 7320 7468 6520 7072  e defines the pr
+000134e0: 6f70 6572 7469 6573 206f 6620 7468 6520  operties of the 
+000134f0: 576f 726b 6572 2050 6f6f 6c20 746f 2062  Worker Pool to b
+00013500: 6520 6372 6561 7465 642c 2061 6e64 2069  e created, and i
+00013510: 7320 7573 6564 2062 7920 7468 6520 6079  s used by the `y
+00013520: 642d 7072 6f76 6973 696f 6e60 2063 6f6d  d-provision` com
+00013530: 6d61 6e64 2e20 4120 7375 6273 6574 206f  mand. A subset o
+00013540: 6620 7468 6520 7072 6f70 6572 7469 6573  f the properties
+00013550: 2069 7320 616c 736f 2075 7365 6420 6279   is also used by
+00013560: 2074 6865 2060 7964 2d69 6e73 7461 6e74   the `yd-instant
+00013570: 6961 7465 6020 636f 6d6d 616e 642c 2066  iate` command, f
+00013580: 6f72 2063 7265 6174 696e 6720 7374 616e  or creating stan
+00013590: 6461 6c6f 6e65 2043 6f6d 7075 7465 2052  dalone Compute R
+000135a0: 6571 7569 7265 6d65 6e74 7320 7468 6174  equirements that
+000135b0: 2061 7265 206e 6f74 2061 7373 6f63 6961   are not associa
+000135c0: 7465 6420 7769 7468 2057 6f72 6b65 7220  ted with Worker 
+000135d0: 506f 6f6c 732e 0a0a 5468 6520 6f6e 6c79  Pools...The only
+000135e0: 206d 616e 6461 746f 7279 2070 726f 7065   mandatory prope
+000135f0: 7274 7920 6973 2060 7465 6d70 6c61 7465  rty is `template
+00013600: 4964 602e 2041 6c6c 206f 7468 6572 2070  Id`. All other p
+00013610: 726f 7065 7274 6965 7320 6861 7665 2064  roperties have d
+00013620: 6566 6175 6c74 7320 286f 7220 6172 6520  efaults (or are 
+00013630: 6e6f 7420 7265 7175 6972 6564 292e 0a0a  not required)...
+00013640: 5468 6520 666f 6c6c 6f77 696e 6720 7072  The following pr
+00013650: 6f70 6572 7469 6573 2061 7265 2061 7661  operties are ava
+00013660: 696c 6162 6c65 3a0a 0a7c 2050 726f 7065  ilable:..| Prope
+00013670: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
+00013680: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
+00013690: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+000136a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013700: 2044 6566 6175 6c74 2020 2020 2020 2020   Default        
+00013710: 2020 2020 2020 2020 207c 0a7c 3a2d 2d2d           |.|:---
+00013720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013730: 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d  -------|:-------
+00013740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000137a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000137b0: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
+000137c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2060  -----------|.| `
+000137d0: 6964 6c65 4e6f 6465 5368 7574 646f 776e  idleNodeShutdown
+000137e0: 456e 6162 6c65 6460 207c 2057 6865 7468  Enabled` | Wheth
+000137f0: 6572 2074 6f20 7368 7574 2064 6f77 6e20  er to shut down 
+00013800: 6e6f 6465 7320 7468 6174 2068 6176 6520  nodes that have 
+00013810: 6265 656e 2069 646c 6520 666f 7220 6069  been idle for `i
+00013820: 646c 654e 6f64 6553 6875 7464 6f77 6e54  dleNodeShutdownT
+00013830: 696d 656f 7574 6020 6d69 6e75 7465 732e  imeout` minutes.
+00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013860: 207c 0a7c 2060 6d69 6e4e 6f64 6573 6020   |.| `minNodes` 
-00013870: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00013880: 2054 6865 206d 696e 696d 756d 206e 756d   The minimum num
-00013890: 6265 7220 6f66 206e 6f64 6573 2074 6f20  ber of nodes to 
-000138a0: 7768 6963 6820 7468 6520 576f 726b 6572  which the Worker
-000138b0: 2050 6f6f 6c20 6361 6e20 6265 2073 6361   Pool can be sca
-000138c0: 6c65 6420 646f 776e 2e20 2020 2020 2020  led down.       
-000138d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 2020 2020 2020 207c 2060 3060 2020           | `0`  
-00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013910: 2020 207c 0a7c 2060 6d61 784e 6f64 6573     |.| `maxNodes
-00013920: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00013930: 207c 2054 6865 206d 6178 696d 756d 206e   | The maximum n
-00013940: 756d 6265 7220 6f66 206e 6f64 6573 2074  umber of nodes t
-00013950: 6f20 7768 6963 6820 7468 6520 576f 726b  o which the Work
-00013960: 6572 2050 6f6f 6c20 6361 6e20 6265 2073  er Pool can be s
-00013970: 6361 6c65 6420 7570 2e20 2020 2020 2020  caled up.       
-00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 2020 2020 2020 2020 207c 2060 3160             | `1`
+00013860: 2020 207c 2060 5472 7565 6020 2020 2020     | `True`     
+00013870: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00013880: 2060 6964 6c65 4e6f 6465 5368 7574 646f   `idleNodeShutdo
+00013890: 776e 5469 6d65 6f75 7460 207c 2054 6865  wnTimeout` | The
+000138a0: 2074 696d 656f 7574 2069 6e20 6d69 6e75   timeout in minu
+000138b0: 7465 7320 6166 7465 7220 7768 6963 6820  tes after which 
+000138c0: 616e 2069 646c 6520 6e6f 6465 2077 696c  an idle node wil
+000138d0: 6c20 6265 2073 6875 7420 646f 776e 2069  l be shut down i
+000138e0: 6620 6069 646c 654e 6f64 6553 6875 7464  f `idleNodeShutd
+000138f0: 6f77 6e45 6e61 626c 6564 6020 6973 2073  ownEnabled` is s
+00013900: 6574 2074 6f20 6054 7275 6560 2e20 2020  et to `True`.   
+00013910: 2020 2020 207c 2060 352e 3060 2020 2020       | `5.0`    
+00013920: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013930: 0a7c 2060 6964 6c65 506f 6f6c 5368 7574  .| `idlePoolShut
+00013940: 646f 776e 456e 6162 6c65 6460 207c 2057  downEnabled` | W
+00013950: 6865 7468 6572 2074 6f20 7368 7574 2064  hether to shut d
+00013960: 6f77 6e20 7468 6520 576f 726b 6572 2050  own the Worker P
+00013970: 6f6f 6c20 7768 656e 2069 7420 6861 7320  ool when it has 
+00013980: 6265 656e 2069 646c 6520 666f 7220 6069  been idle for `i
+00013990: 646c 6550 6f6f 6c53 6875 7464 6f77 6e54  dlePoolShutdownT
+000139a0: 696d 656f 7574 6020 6d69 6e75 7465 732e  imeout` minutes.
 000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139c0: 2020 2020 207c 0a7c 2060 6e61 6d65 6020       |.| `name` 
+000139c0: 2020 2020 2020 207c 2060 5472 7565 6020         | `True` 
 000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 2020 207c 2054 6865 206e 616d 6520 6f66     | The name of
-000139f0: 2074 6865 2057 6f72 6b65 7220 506f 6f6c   the Worker Pool
-00013a00: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 2020 2020 2020 2020 2020 2020 207c 2041               | A
-00013a60: 7574 6f6d 6174 6963 616c 6c79 2047 656e  utomatically Gen
-00013a70: 6572 6174 6564 207c 0a7c 2060 6e6f 6465  erated |.| `node
-00013a80: 426f 6f74 5469 6d65 6f75 7460 2020 2020  BootTimeout`    
-00013a90: 2020 2020 207c 2054 6865 2074 696d 6520       | The time 
-00013aa0: 696e 206d 696e 7574 6573 2061 6c6c 6f77  in minutes allow
-00013ab0: 6564 2066 6f72 2061 206e 6f64 6520 746f  ed for a node to
-00013ac0: 2062 6f6f 7420 616e 6420 7265 6769 7374   boot and regist
-00013ad0: 6572 2077 6974 6820 7468 6520 706c 6174  er with the plat
-00013ae0: 666f 726d 2c20 6f74 6865 7277 6973 6520  form, otherwise 
-00013af0: 6974 2077 696c 6c20 6265 2074 6572 6d69  it will be termi
-00013b00: 6e61 7465 642e 2020 2020 2020 2020 207c  nated.         |
-00013b10: 2060 3130 2e30 6020 2020 2020 2020 2020   `10.0`         
-00013b20: 2020 2020 2020 2020 207c 0a7c 2060 7461           |.| `ta
-00013b30: 7267 6574 496e 7374 616e 6365 436f 756e  rgetInstanceCoun
-00013b40: 7460 2020 2020 207c 2054 6865 2069 6e69  t`     | The ini
-00013b50: 7469 616c 206e 756d 6265 7220 6f66 206e  tial number of n
-00013b60: 6f64 6573 2074 6f20 6372 6561 7465 2066  odes to create f
-00013b70: 6f72 2074 6865 2057 6f72 6b65 7220 506f  or the Worker Po
-00013b80: 6f6c 2e20 2020 2020 2020 2020 2020 2020  ol.             
-00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139e0: 207c 0a7c 2060 6964 6c65 506f 6f6c 5368   |.| `idlePoolSh
+000139f0: 7574 646f 776e 5469 6d65 6f75 7460 207c  utdownTimeout` |
+00013a00: 2054 6865 2074 696d 656f 7574 2069 6e20   The timeout in 
+00013a10: 6d69 6e75 7465 7320 6166 7465 7220 7768  minutes after wh
+00013a20: 6963 6820 616e 2069 646c 6520 576f 726b  ich an idle Work
+00013a30: 6572 2050 6f6f 6c20 7769 6c6c 2062 6520  er Pool will be 
+00013a40: 7368 7574 2064 6f77 6e20 6966 2060 6964  shut down if `id
+00013a50: 6c65 506f 6f6c 5368 7574 646f 776e 456e  lePoolShutdownEn
+00013a60: 6162 6c65 6460 2069 7320 7365 7420 746f  abled` is set to
+00013a70: 2060 5472 7565 602e 207c 2060 3330 2e30   `True`. | `30.0
+00013a80: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00013a90: 2020 207c 0a7c 2060 696d 6167 6573 4964     |.| `imagesId
+00013aa0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00013ab0: 207c 2054 6865 2069 6d61 6765 7320 4944   | The images ID
+00013ac0: 2074 6f20 7573 6520 7768 656e 2062 6f6f   to use when boo
+00013ad0: 7469 6e67 2069 6e73 7461 6e63 6573 2e20  ting instances. 
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b20: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00013b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b40: 2020 2020 207c 0a7c 2060 696e 7374 616e       |.| `instan
+00013b50: 6365 5461 6773 6020 2020 2020 2020 2020  ceTags`         
+00013b60: 2020 207c 2054 6865 2064 6963 7469 6f6e     | The diction
+00013b70: 6172 7920 6f66 2069 6e73 7461 6e63 6520  ary of instance 
+00013b80: 7461 6773 2074 6f20 6170 706c 7920 746f  tags to apply to
+00013b90: 2074 6865 2069 6e73 7461 6e63 6573 2e20   the instances. 
 00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 207c 2060 3160 2020 2020 2020 2020 2020   | `1`          
-00013bd0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-00013be0: 7465 6d70 6c61 7465 4964 6020 2020 2020  templateId`     
-00013bf0: 2020 2020 2020 2020 207c 2054 6865 2059           | The Y
-00013c00: 656c 6c6f 7744 6f67 2043 6f6d 7075 7465  ellowDog Compute
-00013c10: 2054 656d 706c 6174 6520 4944 2074 6f20   Template ID to 
-00013c20: 7573 6520 666f 7220 7072 6f76 6973 696f  use for provisio
-00013c30: 6e69 6e67 2e20 282a 2a52 6571 7569 7265  ning. (**Require
-00013c40: 642a 2a2c 206e 6f20 6465 6661 756c 7420  d**, no default 
-00013c50: 7072 6f76 6964 6564 2e29 2020 2020 2020  provided.)      
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bf0: 2020 2020 2020 207c 0a7c 2060 6d69 6e4e         |.| `minN
+00013c00: 6f64 6573 6020 2020 2020 2020 2020 2020  odes`           
+00013c10: 2020 2020 207c 2054 6865 206d 696e 696d       | The minim
+00013c20: 756d 206e 756d 6265 7220 6f66 206e 6f64  um number of nod
+00013c30: 6573 2074 6f20 7768 6963 6820 7468 6520  es to which the 
+00013c40: 576f 726b 6572 2050 6f6f 6c20 6361 6e20  Worker Pool can 
+00013c50: 6265 2073 6361 6c65 6420 646f 776e 2e20  be scaled down. 
 00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00013c80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00013c90: 2060 7573 6572 4461 7461 6020 2020 2020   `userData`     
-00013ca0: 2020 2020 2020 2020 2020 207c 2055 7365             | Use
-00013cb0: 7220 4461 7461 2074 6f20 6265 2073 7570  r Data to be sup
-00013cc0: 706c 6965 6420 746f 2069 6e73 7461 6e63  plied to instanc
-00013cd0: 6573 206f 6e20 626f 6f74 2e20 2020 2020  es on boot.     
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013c90: 2060 3060 2020 2020 2020 2020 2020 2020   `0`            
+00013ca0: 2020 2020 2020 2020 207c 0a7c 2060 6d61           |.| `ma
+00013cb0: 784e 6f64 6573 6020 2020 2020 2020 2020  xNodes`         
+00013cc0: 2020 2020 2020 207c 2054 6865 206d 6178         | The max
+00013cd0: 696d 756d 206e 756d 6265 7220 6f66 206e  imum number of n
+00013ce0: 6f64 6573 2074 6f20 7768 6963 6820 7468  odes to which th
+00013cf0: 6520 576f 726b 6572 2050 6f6f 6c20 6361  e Worker Pool ca
+00013d00: 6e20 6265 2073 6361 6c65 6420 7570 2e20  n be scaled up. 
 00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d20: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00013d30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00013d40: 0a7c 2060 7573 6572 4461 7461 4669 6c65  .| `userDataFile
-00013d50: 6020 2020 2020 2020 2020 2020 207c 2041  `            | A
-00013d60: 7320 6162 6f76 652c 2062 7574 2072 6561  s above, but rea
-00013d70: 6420 7468 6520 5573 6572 2044 6174 6120  d the User Data 
-00013d80: 6672 6f6d 2074 6865 2066 696c 656e 616d  from the filenam
-00013d90: 6520 7375 7070 6c69 6564 2069 6e20 7468  e supplied in th
-00013da0: 6973 2070 726f 7065 7274 792e 2020 2020  is property.    
+00013d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d40: 207c 2060 3160 2020 2020 2020 2020 2020   | `1`          
+00013d50: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00013d60: 6e61 6d65 6020 2020 2020 2020 2020 2020  name`           
+00013d70: 2020 2020 2020 2020 207c 2054 6865 206e           | The n
+00013d80: 616d 6520 6f66 2074 6865 2057 6f72 6b65  ame of the Worke
+00013d90: 7220 506f 6f6c 2e20 2020 2020 2020 2020  r Pool.         
+00013da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 207c 0a7c 2060 7573 6572 4461 7461 4669   |.| `userDataFi
-00013e00: 6c65 7360 2020 2020 2020 2020 2020 207c  les`           |
-00013e10: 2041 7320 6162 6f76 652c 2062 7574 2063   As above, but c
-00013e20: 7265 6174 6520 7468 6520 5573 6572 2044  reate the User D
-00013e30: 6174 6120 6279 2063 6f6e 6361 7465 6e61  ata by concatena
-00013e40: 7469 6e67 2074 6865 2063 6f6e 7465 6e74  ting the content
-00013e50: 7320 6f66 2074 6865 206c 6973 7420 6f66  s of the list of
-00013e60: 2066 696c 656e 616d 6573 2073 7570 706c   filenames suppl
-00013e70: 6965 6420 696e 2074 6869 7320 7072 6f70  ied in this prop
-00013e80: 6572 7479 2e20 2020 207c 2020 2020 2020  erty.    |      
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 207c 0a7c 2060 776f 726b 6572 7350     |.| `workersP
-00013eb0: 6572 5643 5055 6020 2020 2020 2020 2020  erVCPU`         
-00013ec0: 207c 2054 6865 206e 756d 6265 7220 6f66   | The number of
-00013ed0: 2057 6f72 6b65 7273 2074 6f20 6573 7461   Workers to esta
-00013ee0: 626c 6973 6820 7065 7220 7643 5055 206f  blish per vCPU o
-00013ef0: 6e20 6561 6368 206e 6f64 6520 696e 2074  n each node in t
-00013f00: 6865 2057 6f72 6b65 7220 506f 6f6c 2e20  he Worker Pool. 
-00013f10: 284f 7665 7272 6964 6573 2060 776f 726b  (Overrides `work
-00013f20: 6572 7350 6572 4e6f 6465 602e 2920 2020  ersPerNode`.)   
-00013f30: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00013df0: 2020 207c 2041 7574 6f6d 6174 6963 616c     | Automatical
+00013e00: 6c79 2047 656e 6572 6174 6564 207c 0a7c  ly Generated |.|
+00013e10: 2060 6e6f 6465 426f 6f74 5469 6d65 6f75   `nodeBootTimeou
+00013e20: 7460 2020 2020 2020 2020 207c 2054 6865  t`         | The
+00013e30: 2074 696d 6520 696e 206d 696e 7574 6573   time in minutes
+00013e40: 2061 6c6c 6f77 6564 2066 6f72 2061 206e   allowed for a n
+00013e50: 6f64 6520 746f 2062 6f6f 7420 616e 6420  ode to boot and 
+00013e60: 7265 6769 7374 6572 2077 6974 6820 7468  register with th
+00013e70: 6520 706c 6174 666f 726d 2c20 6f74 6865  e platform, othe
+00013e80: 7277 6973 6520 6974 2077 696c 6c20 6265  rwise it will be
+00013e90: 2074 6572 6d69 6e61 7465 642e 2020 2020   terminated.    
+00013ea0: 2020 2020 207c 2060 3130 2e30 6020 2020       | `10.0`   
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013ec0: 0a7c 2060 7461 7267 6574 496e 7374 616e  .| `targetInstan
+00013ed0: 6365 436f 756e 7460 2020 2020 207c 2054  ceCount`     | T
+00013ee0: 6865 2069 6e69 7469 616c 206e 756d 6265  he initial numbe
+00013ef0: 7220 6f66 206e 6f64 6573 2074 6f20 6372  r of nodes to cr
+00013f00: 6561 7465 2066 6f72 2074 6865 2057 6f72  eate for the Wor
+00013f10: 6b65 7220 506f 6f6c 2e20 2020 2020 2020  ker Pool.       
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f50: 2020 2020 207c 0a7c 2060 776f 726b 6572       |.| `worker
-00013f60: 7350 6572 4e6f 6465 6020 2020 2020 2020  sPerNode`       
-00013f70: 2020 207c 2054 6865 206e 756d 6265 7220     | The number 
-00013f80: 6f66 2057 6f72 6b65 7273 2074 6f20 6573  of Workers to es
-00013f90: 7461 626c 6973 6820 6f6e 2065 6163 6820  tablish on each 
-00013fa0: 6e6f 6465 2069 6e20 7468 6520 576f 726b  node in the Work
-00013fb0: 6572 2050 6f6f 6c2e 2020 2020 2020 2020  er Pool.        
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fe0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-00013ff0: 3160 2020 2020 2020 2020 2020 2020 2020  1`              
-00014000: 2020 2020 2020 207c 0a7c 2060 776f 726b         |.| `work
-00014010: 6572 506f 6f6c 4461 7461 6020 2020 2020  erPoolData`     
-00014020: 2020 2020 207c 2054 6865 206e 616d 6520       | The name 
-00014030: 6f66 2061 2066 696c 6520 636f 6e74 6169  of a file contai
-00014040: 6e69 6e67 2061 204a 534f 4e20 646f 6375  ning a JSON docu
-00014050: 6d65 6e74 2064 6566 696e 696e 6720 6120  ment defining a 
-00014060: 576f 726b 6572 2050 6f6f 6c2e 2020 2020  Worker Pool.    
-00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f50: 2020 2020 2020 207c 2060 3160 2020 2020         | `1`    
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f70: 207c 0a7c 2060 7465 6d70 6c61 7465 4964   |.| `templateId
+00013f80: 6020 2020 2020 2020 2020 2020 2020 207c  `              |
+00013f90: 2054 6865 2059 656c 6c6f 7744 6f67 2043   The YellowDog C
+00013fa0: 6f6d 7075 7465 2054 656d 706c 6174 6520  ompute Template 
+00013fb0: 4944 2074 6f20 7573 6520 666f 7220 7072  ID to use for pr
+00013fc0: 6f76 6973 696f 6e69 6e67 2e20 282a 2a52  ovisioning. (**R
+00013fd0: 6571 7569 7265 642a 2a2c 206e 6f20 6465  equired**, no de
+00013fe0: 6661 756c 7420 7072 6f76 6964 6564 2e29  fault provided.)
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014020: 2020 207c 0a7c 2060 7573 6572 4461 7461     |.| `userData
+00014030: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00014040: 207c 2055 7365 7220 4461 7461 2074 6f20   | User Data to 
+00014050: 6265 2073 7570 706c 6965 6420 746f 2069  be supplied to i
+00014060: 6e73 7461 6e63 6573 206f 6e20 626f 6f74  nstances on boot
+00014070: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140b0: 2020 2020 2020 2020 207c 0a7c 2060 776f           |.| `wo
-000140c0: 726b 6572 5461 6760 2020 2020 2020 2020  rkerTag`        
-000140d0: 2020 2020 2020 207c 2054 6865 2057 6f72         | The Wor
-000140e0: 6b65 7220 5461 6720 746f 2070 7562 6c69  ker Tag to publi
-000140f0: 7368 2066 6f72 2074 6865 2061 6c6c 206f  sh for the all o
-00014100: 6620 7468 6520 576f 726b 6572 7320 6f6e  f the Workers on
-00014110: 2074 6865 206e 6f64 652e 2020 2020 2020   the node.      
-00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014150: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00014160: 2020 2020 2020 2020 2020 207c 0a0a 2323             |..##
-00014170: 2041 7574 6f6d 6174 6963 2050 726f 7065   Automatic Prope
-00014180: 7274 6965 730a 0a54 6865 206e 616d 6520  rties..The name 
-00014190: 6f66 2074 6865 2057 6f72 6b65 7220 506f  of the Worker Po
-000141a0: 6f6c 2c20 6966 206e 6f74 2073 7570 706c  ol, if not suppl
-000141b0: 6965 642c 2069 7320 6175 746f 6d61 7469  ied, is automati
-000141c0: 6361 6c6c 7920 6765 6e65 7261 7465 6420  cally generated 
-000141d0: 7573 696e 6720 6120 636f 6e63 6174 656e  using a concaten
-000141e0: 6174 696f 6e20 6f66 2060 7770 5f60 2c20  ation of `wp_`, 
-000141f0: 7468 6520 6074 6167 6020 7072 6f70 6572  the `tag` proper
-00014200: 7479 2c20 6120 5554 4320 7469 6d65 7374  ty, a UTC timest
-00014210: 616d 702c 2061 6e64 2074 6872 6565 2072  amp, and three r
-00014220: 616e 646f 6d20 6865 7820 6368 6172 6163  andom hex charac
-00014230: 7465 7273 3a20 652c 672c 2e20 6077 705f  ters: e,g,. `wp_
-00014240: 6d79 7461 675f 3232 3130 3234 2d31 3535  mytag_221024-155
-00014250: 3532 342d 6230 6160 2e0a 0a23 2320 544f  524-b0a`...## TO
-00014260: 4d4c 2050 726f 7065 7274 6965 7320 696e  ML Properties in
-00014270: 2074 6865 2060 776f 726b 6572 506f 6f6c   the `workerPool
-00014280: 6020 5365 6374 696f 6e0a 0a48 6572 6527  ` Section..Here'
-00014290: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
-000142a0: 7468 6520 6077 6f72 6b65 7250 6f6f 6c60  the `workerPool`
-000142b0: 2073 6563 7469 6f6e 206f 6620 6120 544f   section of a TO
-000142c0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-000142d0: 2066 696c 652c 2073 686f 7769 6e67 2061   file, showing a
-000142e0: 6c6c 2074 6865 2070 6f73 7369 626c 6520  ll the possible 
-000142f0: 7072 6f70 6572 7469 6573 2074 6861 7420  properties that 
-00014300: 6361 6e20 6265 2073 6574 3a0a 0a60 6060  can be set:..```
-00014310: 746f 6d6c 0a5b 776f 726b 6572 506f 6f6c  toml.[workerPool
-00014320: 5d0a 2020 2020 6964 6c65 4e6f 6465 5368  ].    idleNodeSh
-00014330: 7574 646f 776e 456e 6162 6c65 6420 3d20  utdownEnabled = 
-00014340: 7472 7565 0a20 2020 2069 646c 654e 6f64  true.    idleNod
-00014350: 6553 6875 7464 6f77 6e54 696d 656f 7574  eShutdownTimeout
-00014360: 203d 2031 302e 300a 2020 2020 6964 6c65   = 10.0.    idle
-00014370: 506f 6f6c 5368 7574 646f 776e 456e 6162  PoolShutdownEnab
-00014380: 6c65 6420 3d20 7472 7565 0a20 2020 2069  led = true.    i
-00014390: 646c 6550 6f6f 6c53 6875 7464 6f77 6e54  dlePoolShutdownT
-000143a0: 696d 656f 7574 203d 2036 302e 300a 2020  imeout = 60.0.  
-000143b0: 2020 696d 6167 6573 4964 203d 2022 7964    imagesId = "yd
-000143c0: 6964 3a69 6d67 6661 6d3a 3030 3030 3030  id:imgfam:000000
-000143d0: 3a34 3139 3632 3539 322d 3537 3763 2d34  :41962592-577c-4
-000143e0: 6664 652d 6162 3033 2d64 3835 3234 3635  fde-ab03-d852465
-000143f0: 6537 6638 6222 0a20 2020 2069 6e73 7461  e7f8b".    insta
-00014400: 6e63 6554 6167 7320 3d20 7b7d 0a20 2020  nceTags = {}.   
-00014410: 206d 6178 4e6f 6465 7320 3d20 310a 2020   maxNodes = 1.  
-00014420: 2020 6d69 6e4e 6f64 6573 203d 2031 0a20    minNodes = 1. 
-00014430: 2020 206e 616d 6520 3d20 226d 792d 776f     name = "my-wo
-00014440: 726b 6572 2d70 6f6f 6c22 0a20 2020 206e  rker-pool".    n
-00014450: 6f64 6542 6f6f 7454 696d 656f 7574 203d  odeBootTimeout =
-00014460: 2035 0a20 2020 2074 6172 6765 7449 6e73   5.    targetIns
-00014470: 7461 6e63 6543 6f75 6e74 203d 2031 0a20  tanceCount = 1. 
-00014480: 2020 2074 656d 706c 6174 6549 6420 3d20     templateId = 
-00014490: 2279 6469 643a 6372 743a 4439 4335 3438  "ydid:crt:D9C548
-000144a0: 3a34 3635 6131 3037 632d 3763 6561 2d34  :465a107c-7cea-4
-000144b0: 3665 332d 3966 6464 2d31 3531 3136 6362  6e3-9fdd-15116cb
-000144c0: 3932 6334 3022 0a20 2020 2023 204e 6f74  92c40".    # Not
-000144d0: 653a 206f 6e6c 7920 6f6e 6520 6f66 2027  e: only one of '
-000144e0: 7573 6572 4461 7461 272f 2775 7365 7244  userData'/'userD
-000144f0: 6174 6146 696c 6527 2f27 7573 6572 4461  ataFile'/'userDa
-00014500: 7461 4669 6c65 7327 2073 686f 756c 6420  taFiles' should 
-00014510: 6265 2073 6574 0a20 2020 2075 7365 7244  be set.    userD
-00014520: 6174 6120 3d20 2222 0a20 2020 2075 7365  ata = "".    use
-00014530: 7244 6174 6146 696c 6520 3d20 226d 7975  rDataFile = "myu
-00014540: 7365 7264 6174 612e 7478 7422 0a20 2020  serdata.txt".   
-00014550: 2075 7365 7244 6174 6146 696c 6573 203d   userDataFiles =
-00014560: 205b 226d 7975 7365 7264 6174 6131 2e74   ["myuserdata1.t
-00014570: 7874 222c 2022 6d79 7573 6572 6461 7461  xt", "myuserdata
-00014580: 322e 7478 7422 5d0a 2020 2020 776f 726b  2.txt"].    work
-00014590: 6572 5461 6720 3d20 2274 6167 2d7b 7b75  erTag = "tag-{{u
-000145a0: 7365 726e 616d 657d 7d22 0a20 2020 2023  sername}}".    #
-000145b0: 2053 7065 6369 6679 2065 6974 6865 7220   Specify either 
-000145c0: 776f 726b 6572 7350 6572 4e6f 6465 206f  workersPerNode o
-000145d0: 7220 776f 726b 6572 7350 6572 5643 5055  r workersPerVCPU
-000145e0: 0a20 2020 2077 6f72 6b65 7273 5065 724e  .    workersPerN
-000145f0: 6f64 6520 3d20 310a 2020 2020 776f 726b  ode = 1.    work
-00014600: 6572 7350 6572 5643 5055 203d 2031 0a23  ersPerVCPU = 1.#
-00014610: 2020 2077 6f72 6b65 7250 6f6f 6c44 6174     workerPoolDat
-00014620: 6120 3d20 2277 6f72 6b65 725f 706f 6f6c  a = "worker_pool
-00014630: 2e6a 736f 6e22 0a60 6060 0a0a 2323 2057  .json".```..## W
-00014640: 6f72 6b65 7220 506f 6f6c 2053 7065 6369  orker Pool Speci
-00014650: 6669 6361 7469 6f6e 2055 7369 6e67 204a  fication Using J
-00014660: 534f 4e20 446f 6375 6d65 6e74 730a 0a49  SON Documents..I
-00014670: 7427 7320 616c 736f 2070 6f73 7369 626c  t's also possibl
-00014680: 6520 746f 2063 6170 7475 7265 2061 2057  e to capture a W
-00014690: 6f72 6b65 7220 506f 6f6c 2064 6566 696e  orker Pool defin
-000146a0: 6974 696f 6e20 6173 2061 204a 534f 4e20  ition as a JSON 
-000146b0: 646f 6375 6d65 6e74 2e20 5468 6520 4a53  document. The JS
-000146c0: 4f4e 2066 696c 656e 616d 6520 6361 6e20  ON filename can 
-000146d0: 6265 2073 7570 706c 6965 6420 6569 7468  be supplied eith
-000146e0: 6572 2075 7369 6e67 2074 6865 2063 6f6d  er using the com
-000146f0: 6d61 6e64 206c 696e 6520 7769 7468 2074  mand line with t
-00014700: 6865 2060 2d2d 776f 726b 6572 2d70 6f6f  he `--worker-poo
-00014710: 6c60 206f 7220 602d 7060 2070 6172 616d  l` or `-p` param
-00014720: 6574 6572 2077 6974 6820 6079 642d 7072  eter with `yd-pr
-00014730: 6f76 6973 696f 6e60 2c20 6f72 2062 7920  ovision`, or by 
-00014740: 706f 7075 6c61 7469 6e67 2074 6865 2060  populating the `
-00014750: 776f 726b 6572 506f 6f6c 4461 7461 6020  workerPoolData` 
-00014760: 7072 6f70 6572 7479 2069 6e20 7468 6520  property in the 
-00014770: 544f 4d4c 2063 6f6e 6669 6775 7261 7469  TOML configurati
-00014780: 6f6e 2066 696c 6520 7769 7468 2074 6865  on file with the
-00014790: 204a 534f 4e20 6669 6c65 6e61 6d65 2e20   JSON filename. 
-000147a0: 436f 6d6d 616e 6420 6c69 6e65 2073 7065  Command line spe
-000147b0: 6369 6669 6361 7469 6f6e 2074 616b 6573  cification takes
-000147c0: 2070 7269 6f72 6974 7920 6f76 6572 2054   priority over T
-000147d0: 4f4d 4c20 7370 6563 6966 6963 6174 696f  OML specificatio
-000147e0: 6e2e 0a0a 5468 6520 4a53 4f4e 2073 7065  n...The JSON spe
-000147f0: 6369 6669 6361 7469 6f6e 2061 6c6c 6f77  cification allow
-00014800: 7320 7468 6520 6372 6561 7469 6f6e 206f  s the creation o
-00014810: 6620 2a2a 4164 7661 6e63 6564 2057 6f72  f **Advanced Wor
-00014820: 6b65 7220 506f 6f6c 732a 2a2c 2077 6974  ker Pools**, wit
-00014830: 6820 6469 6666 6572 656e 7420 6e6f 6465  h different node
-00014840: 2074 7970 6573 2061 6e64 2074 6865 2061   types and the a
-00014850: 6269 6c69 7479 2074 6f20 7370 6563 6966  bility to specif
-00014860: 7920 4e6f 6465 2041 6374 696f 6e73 2e0a  y Node Actions..
-00014870: 0a57 6865 6e20 7573 696e 6720 6120 4a53  .When using a JS
-00014880: 4f4e 2064 6f63 756d 656e 7420 746f 2073  ON document to s
-00014890: 7065 6369 6679 2074 6865 2057 6f72 6b65  pecify the Worke
-000148a0: 7220 506f 6f6c 2c20 7468 6520 7363 6865  r Pool, the sche
-000148b0: 6d61 206f 6620 7468 6520 646f 6375 6d65  ma of the docume
-000148c0: 6e74 2069 7320 6964 656e 7469 6361 6c20  nt is identical 
-000148d0: 746f 2074 6861 7420 6578 7065 6374 6564  to that expected
-000148e0: 2062 7920 7468 6520 5965 6c6c 6f77 446f   by the YellowDo
-000148f0: 6720 5245 5354 2041 5049 2066 6f72 2057  g REST API for W
-00014900: 6f72 6b65 7220 506f 6f6c 2050 726f 7669  orker Pool Provi
-00014910: 7369 6f6e 696e 672e 0a0a 2323 2320 576f  sioning...### Wo
-00014920: 726b 6572 2050 6f6f 6c20 4a53 4f4e 2045  rker Pool JSON E
-00014930: 7861 6d70 6c65 730a 0a54 6865 2065 7861  xamples..The exa
-00014940: 6d70 6c65 2062 656c 6f77 2069 7320 6f66  mple below is of
-00014950: 2061 2073 696d 706c 6520 4a53 4f4e 2073   a simple JSON s
-00014960: 7065 6369 6669 6361 7469 6f6e 206f 6620  pecification of 
-00014970: 6120 576f 726b 6572 2050 6f6f 6c20 7769  a Worker Pool wi
-00014980: 7468 206f 6e65 2069 6e69 7469 616c 206e  th one initial n
-00014990: 6f64 652c 2057 6f72 6b65 7220 506f 6f6c  ode, Worker Pool
-000149a0: 2073 6875 7464 6f77 6e2c 2065 7463 2e0a   shutdown, etc..
-000149b0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7265  .```json.{.  "re
-000149c0: 7175 6972 656d 656e 7454 656d 706c 6174  quirementTemplat
-000149d0: 6555 7361 6765 223a 207b 0a20 2020 2022  eUsage": {.    "
-000149e0: 6d61 696e 7461 696e 496e 7374 616e 6365  maintainInstance
-000149f0: 436f 756e 7422 3a20 6661 6c73 652c 0a20  Count": false,. 
-00014a00: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
-00014a10: 616d 6522 3a20 2277 705f 7079 6578 2d70  ame": "wp_pyex-p
-00014a20: 7269 6d65 735f 3233 3031 3133 2d31 3631  rimes_230113-161
-00014a30: 3532 382d 6461 3022 2c0a 2020 2020 2272  528-da0",.    "r
-00014a40: 6571 7569 7265 6d65 6e74 4e61 6d65 7370  equirementNamesp
-00014a50: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
-00014a60: 7322 2c0a 2020 2020 2272 6571 7569 7265  s",.    "require
-00014a70: 6d65 6e74 5461 6722 3a20 2270 7965 782d  mentTag": "pyex-
-00014a80: 7072 696d 6573 222c 0a20 2020 2022 7461  primes",.    "ta
-00014a90: 7267 6574 496e 7374 616e 6365 436f 756e  rgetInstanceCoun
-00014aa0: 7422 3a20 312c 0a20 2020 2022 7465 6d70  t": 1,.    "temp
-00014ab0: 6c61 7465 4964 223a 2022 7964 6964 3a63  lateId": "ydid:c
-00014ac0: 7274 3a44 3943 3534 383a 3436 3561 3130  rt:D9C548:465a10
-00014ad0: 3763 2d37 6365 612d 3436 6533 2d39 6664  7c-7cea-46e3-9fd
-00014ae0: 642d 3135 3131 3663 6239 3263 3430 220a  d-15116cb92c40".
-00014af0: 2020 7d2c 0a20 2022 7072 6f76 6973 696f    },.  "provisio
-00014b00: 6e65 6450 726f 7065 7274 6965 7322 3a20  nedProperties": 
-00014b10: 7b0a 2020 2020 2269 646c 654e 6f64 6553  {.    "idleNodeS
-00014b20: 6875 7464 6f77 6e22 3a20 7b22 656e 6162  hutdown": {"enab
-00014b30: 6c65 6422 3a20 7472 7565 2c20 2274 696d  led": true, "tim
-00014b40: 656f 7574 223a 2022 5054 3130 4d22 7d2c  eout": "PT10M"},
-00014b50: 0a20 2020 2022 6964 6c65 506f 6f6c 5368  .    "idlePoolSh
-00014b60: 7574 646f 776e 223a 207b 2265 6e61 626c  utdown": {"enabl
-00014b70: 6564 223a 2074 7275 652c 2022 7469 6d65  ed": true, "time
-00014b80: 6f75 7422 3a20 2250 5431 4822 7d2c 0a20  out": "PT1H"},. 
-00014b90: 2020 2022 6372 6561 7465 4e6f 6465 576f     "createNodeWo
-00014ba0: 726b 6572 7322 3a20 7b22 7461 7267 6574  rkers": {"target
-00014bb0: 436f 756e 7422 3a20 312c 2022 7461 7267  Count": 1, "targ
-00014bc0: 6574 5479 7065 223a 2022 5045 525f 5643  etType": "PER_VC
-00014bd0: 5055 227d 2c0a 2020 2020 226d 6178 4e6f  PU"},.    "maxNo
-00014be0: 6465 7322 3a20 352c 0a20 2020 2022 6d69  des": 5,.    "mi
-00014bf0: 6e4e 6f64 6573 223a 2030 2c0a 2020 2020  nNodes": 0,.    
-00014c00: 226e 6f64 6542 6f6f 7454 696d 656f 7574  "nodeBootTimeout
-00014c10: 223a 2022 5054 354d 222c 0a20 2020 2022  ": "PT5M",.    "
-00014c20: 6e6f 6465 4964 6c65 4772 6163 6550 6572  nodeIdleGracePer
-00014c30: 696f 6422 3a20 2250 5433 4d22 2c0a 2020  iod": "PT3M",.  
-00014c40: 2020 226e 6f64 6549 646c 6554 696d 654c    "nodeIdleTimeL
-00014c50: 696d 6974 223a 2022 5054 334d 222c 0a20  imit": "PT3M",. 
-00014c60: 2020 2022 776f 726b 6572 5461 6722 3a20     "workerTag": 
-00014c70: 2270 7965 782d 6261 7368 2d64 6f63 6b65  "pyex-bash-docke
-00014c80: 7222 0a20 207d 0a7d 0a60 6060 0a0a 5468  r".  }.}.```..Th
-00014c90: 6520 6e65 7874 2065 7861 6d70 6c65 2069  e next example i
-00014ca0: 7320 6f66 2061 2072 656c 6174 6976 656c  s of a relativel
-00014cb0: 7920 7269 6368 204a 534f 4e20 7370 6563  y rich JSON spec
-00014cc0: 6966 6963 6174 696f 6e20 6f66 2061 6e20  ification of an 
-00014cd0: 4164 7661 6e63 6564 2057 6f72 6b65 7220  Advanced Worker 
-00014ce0: 506f 6f6c 2c20 6672 6f6d 206f 6e65 206f  Pool, from one o
-00014cf0: 6620 7468 6520 5965 6c6c 6f77 446f 6720  f the YellowDog 
-00014d00: 6465 6d6f 732e 2049 7420 696e 636c 7564  demos. It includ
-00014d10: 6573 206e 6f64 6520 7370 6563 6961 6c69  es node speciali
-00014d20: 7361 7469 6f6e 2c20 616e 6420 6163 7469  sation, and acti
-00014d30: 6f6e 2067 726f 7570 7320 7468 6174 2072  on groups that r
-00014d40: 6573 706f 6e64 2074 6f20 7468 6520 6053  espond to the `S
-00014d50: 5441 5254 5550 5f4e 4f44 4553 5f41 4444  TARTUP_NODES_ADD
-00014d60: 4544 6020 616e 6420 604e 4f44 4553 5f41  ED` and `NODES_A
-00014d70: 4444 4544 6020 6576 656e 7473 2074 6f20  DDED` events to 
-00014d80: 6472 6976 6520 2a2a 4e6f 6465 2041 6374  drive **Node Act
-00014d90: 696f 6e73 2a2a 2e0a 0a60 6060 6a73 6f6e  ions**...```json
-00014da0: 0a7b 0a20 2022 7265 7175 6972 656d 656e  .{.  "requiremen
-00014db0: 7454 656d 706c 6174 6555 7361 6765 223a  tTemplateUsage":
-00014dc0: 207b 0a20 2020 2022 6d61 696e 7461 696e   {.    "maintain
-00014dd0: 496e 7374 616e 6365 436f 756e 7422 3a20  InstanceCount": 
-00014de0: 6661 6c73 652c 0a20 2020 2022 7461 7267  false,.    "targ
-00014df0: 6574 496e 7374 616e 6365 436f 756e 7422  etInstanceCount"
-00014e00: 3a20 362c 0a20 2020 2022 7465 6d70 6c61  : 6,.    "templa
-00014e10: 7465 4964 223a 2022 7964 6964 3a63 7274  teId": "ydid:crt
-00014e20: 3a44 3943 3534 383a 6137 6564 6132 3837  :D9C548:a7eda287
-00014e30: 2d66 3964 362d 3462 6338 2d62 3264 632d  -f9d6-4bc8-b2dc-
-00014e40: 3435 3533 3434 3035 3732 3537 222c 0a20  455344057257",. 
-00014e50: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
-00014e60: 616d 6522 3a20 2277 705f 7079 6578 2d73  ame": "wp_pyex-s
-00014e70: 6c75 726d 5f32 3330 3131 332d 3136 3536  lurm_230113-1656
-00014e80: 3135 2d32 6237 222c 0a20 2020 2022 7265  15-2b7",.    "re
-00014e90: 7175 6972 656d 656e 744e 616d 6573 7061  quirementNamespa
-00014ea0: 6365 223a 2022 7079 6578 616d 706c 6573  ce": "pyexamples
-00014eb0: 222c 0a20 2020 2022 7265 7175 6972 656d  ",.    "requirem
-00014ec0: 656e 7454 6167 223a 2022 7079 6578 2d73  entTag": "pyex-s
-00014ed0: 6c75 726d 220a 2020 7d2c 0a20 2022 7072  lurm".  },.  "pr
-00014ee0: 6f76 6973 696f 6e65 6450 726f 7065 7274  ovisionedPropert
-00014ef0: 6965 7322 3a20 7b0a 2020 2020 2263 7265  ies": {.    "cre
-00014f00: 6174 654e 6f64 6557 6f72 6b65 7273 223a  ateNodeWorkers":
-00014f10: 207b 2274 6172 6765 7443 6f75 6e74 223a   {"targetCount":
-00014f20: 2030 2c20 2274 6172 6765 7454 7970 6522   0, "targetType"
-00014f30: 3a20 2250 4552 5f4e 4f44 4522 7d2c 0a20  : "PER_NODE"},. 
-00014f40: 2020 2022 6e6f 6465 436f 6e66 6967 7572     "nodeConfigur
-00014f50: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
-00014f60: 226e 6f64 6554 7970 6573 223a 205b 0a20  "nodeTypes": [. 
-00014f70: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00014f80: 2273 6c75 726d 6374 6c64 222c 2022 636f  "slurmctld", "co
-00014f90: 756e 7422 3a20 317d 2c0a 2020 2020 2020  unt": 1},.      
-00014fa0: 2020 7b22 6e61 6d65 223a 2022 736c 7572    {"name": "slur
-00014fb0: 6d64 222c 2022 6d69 6e22 3a20 352c 2022  md", "min": 5, "
-00014fc0: 736c 6f74 4e75 6d62 6572 696e 6722 3a20  slotNumbering": 
-00014fd0: 2252 4555 5341 424c 4522 7d0a 2020 2020  "REUSABLE"}.    
-00014fe0: 2020 5d2c 0a20 2020 2020 2022 6e6f 6465    ],.      "node
-00014ff0: 4576 656e 7473 223a 207b 0a20 2020 2020  Events": {.     
-00015000: 2020 2022 5354 4152 5455 505f 4e4f 4445     "STARTUP_NODE
-00015010: 535f 4144 4445 4422 3a20 5b0a 2020 2020  S_ADDED": [.    
-00015020: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00015030: 2020 2020 2261 6374 696f 6e73 223a 205b      "actions": [
-00015040: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00015050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015060: 2022 6163 7469 6f6e 223a 2022 5752 4954   "action": "WRIT
-00015070: 455f 4649 4c45 222c 0a20 2020 2020 2020  E_FILE",.       
-00015080: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
-00015090: 2022 6e6f 6465 732e 6a73 6f6e 222c 0a20   "nodes.json",. 
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000150b0: 636f 6e74 656e 7422 3a20 227b 5c6e 2020  content": "{\n  
-000150c0: 5c22 6e6f 6465 735c 223a 205b 5c6e 7b7b  \"nodes\": [\n{{
-000150d0: 236f 7468 6572 4e6f 6465 737d 7d5c 6e20  #otherNodes}}\n 
-000150e0: 2020 207b 5c6e 2020 2020 2020 5c22 6e61     {\n      \"na
-000150f0: 6d65 5c22 3a20 5c22 736c 7572 6d64 7b7b  me\": \"slurmd{{
-00015100: 6465 7461 696c 732e 6e6f 6465 536c 6f74  details.nodeSlot
-00015110: 7d7d 5c22 2c5c 6e20 2020 2020 205c 2269  }}\",\n      \"i
-00015120: 705c 223a 205c 227b 7b64 6574 6169 6c73  p\": \"{{details
-00015130: 2e70 7269 7661 7465 4970 4164 6472 6573  .privateIpAddres
-00015140: 737d 7d5c 225c 6e20 2020 207d 7b7b 5e2d  s}}\"\n    }{{^-
-00015150: 6c61 7374 7d7d 2c7b 7b2f 2d6c 6173 747d  last}},{{/-last}
-00015160: 7d5c 6e7b 7b2f 6f74 6865 724e 6f64 6573  }\n{{/otherNodes
-00015170: 7d7d 5c6e 2020 5d5c 6e7d 222c 0a20 2020  }}\n  ]\n}",.   
-00015180: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00015190: 6465 5479 7065 7322 3a20 5b22 736c 7572  deTypes": ["slur
-000151a0: 6d63 746c 6422 5d0a 2020 2020 2020 2020  mctld"].        
-000151b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000151c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000151d0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
-000151e0: 223a 2022 5255 4e5f 434f 4d4d 414e 4422  ": "RUN_COMMAND"
-000151f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015200: 2020 2270 6174 6822 3a20 2273 7461 7274    "path": "start
-00015210: 5f73 696d 706c 655f 736c 7572 6d63 746c  _simple_slurmctl
-00015220: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-00015230: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
-00015240: 205b 226e 6f64 6573 2e6a 736f 6e22 5d2c   ["nodes.json"],
-00015250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015260: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-00015270: 7b22 4558 414d 504c 4522 3a20 2246 4f4f  {"EXAMPLE": "FOO
-00015280: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
-00015290: 2020 2020 226e 6f64 6554 7970 6573 223a      "nodeTypes":
-000152a0: 205b 2273 6c75 726d 6374 6c64 225d 0a20   ["slurmctld"]. 
-000152b0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-000152c0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000152d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000152e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000152f0: 2020 2261 6374 696f 6e73 223a 205b 0a20    "actions": [. 
-00015300: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00015310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00015320: 6163 7469 6f6e 223a 2022 5255 4e5f 434f  action": "RUN_CO
-00015330: 4d4d 414e 4422 2c0a 2020 2020 2020 2020  MMAND",.        
-00015340: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
-00015350: 2273 7461 7274 5f73 696d 706c 655f 736c  "start_simple_sl
-00015360: 7572 6d64 222c 0a20 2020 2020 2020 2020  urmd",.         
-00015370: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
-00015380: 7322 3a20 5b22 7b7b 6e6f 6465 7342 7954  s": ["{{nodesByT
-00015390: 7970 652e 736c 7572 6d63 746c 642e 302e  ype.slurmctld.0.
-000153a0: 6465 7461 696c 732e 7072 6976 6174 6549  details.privateI
-000153b0: 7041 6464 7265 7373 7d7d 222c 2022 7b7b  pAddress}}", "{{
-000153c0: 6e6f 6465 2e64 6574 6169 6c73 2e6e 6f64  node.details.nod
-000153d0: 6553 6c6f 747d 7d22 5d2c 0a20 2020 2020  eSlot}}"],.     
-000153e0: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
-000153f0: 5479 7065 7322 3a20 5b22 736c 7572 6d64  Types": ["slurmd
-00015400: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00015410: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
-00015420: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
-00015430: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00015440: 2020 2020 2020 2261 6374 696f 6e73 223a        "actions":
-00015450: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00015460: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00015470: 2020 2022 6163 7469 6f6e 223a 2022 4352     "action": "CR
-00015480: 4541 5445 5f57 4f52 4b45 5253 222c 0a20  EATE_WORKERS",. 
-00015490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000154a0: 746f 7461 6c57 6f72 6b65 7273 223a 2031  totalWorkers": 1
-000154b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000154c0: 2020 226e 6f64 6554 7970 6573 223a 205b    "nodeTypes": [
-000154d0: 2273 6c75 726d 6374 6c64 225d 0a20 2020  "slurmctld"].   
-000154e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000154f0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00015500: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
-00015510: 2c0a 2020 2020 2020 2020 224e 4f44 4553  ,.        "NODES
-00015520: 5f41 4444 4544 223a 205b 0a20 2020 2020  _ADDED": [.     
-00015530: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00015540: 2020 2022 6163 7469 6f6e 7322 3a20 5b0a     "actions": [.
-00015550: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2261 6374 696f 6e22 3a20 2257 5249 5445  "action": "WRITE
-00015580: 5f46 494c 4522 2c0a 2020 2020 2020 2020  _FILE",.        
+000140b0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140d0: 2020 2020 207c 0a7c 2060 7573 6572 4461       |.| `userDa
+000140e0: 7461 4669 6c65 6020 2020 2020 2020 2020  taFile`         
+000140f0: 2020 207c 2041 7320 6162 6f76 652c 2062     | As above, b
+00014100: 7574 2072 6561 6420 7468 6520 5573 6572  ut read the User
+00014110: 2044 6174 6120 6672 6f6d 2074 6865 2066   Data from the f
+00014120: 696c 656e 616d 6520 7375 7070 6c69 6564  ilename supplied
+00014130: 2069 6e20 7468 6973 2070 726f 7065 7274   in this propert
+00014140: 792e 2020 2020 2020 2020 2020 2020 2020  y.              
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014180: 2020 2020 2020 207c 0a7c 2060 7573 6572         |.| `user
+00014190: 4461 7461 4669 6c65 7360 2020 2020 2020  DataFiles`      
+000141a0: 2020 2020 207c 2041 7320 6162 6f76 652c       | As above,
+000141b0: 2062 7574 2063 7265 6174 6520 7468 6520   but create the 
+000141c0: 5573 6572 2044 6174 6120 6279 2063 6f6e  User Data by con
+000141d0: 6361 7465 6e61 7469 6e67 2074 6865 2063  catenating the c
+000141e0: 6f6e 7465 6e74 7320 6f66 2074 6865 206c  ontents of the l
+000141f0: 6973 7420 6f66 2066 696c 656e 616d 6573  ist of filenames
+00014200: 2073 7570 706c 6965 6420 696e 2074 6869   supplied in thi
+00014210: 7320 7072 6f70 6572 7479 2e20 2020 207c  s property.    |
+00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014230: 2020 2020 2020 2020 207c 0a7c 2060 776f           |.| `wo
+00014240: 726b 6572 7350 6572 5643 5055 6020 2020  rkersPerVCPU`   
+00014250: 2020 2020 2020 207c 2054 6865 206e 756d         | The num
+00014260: 6265 7220 6f66 2057 6f72 6b65 7273 2074  ber of Workers t
+00014270: 6f20 6573 7461 626c 6973 6820 7065 7220  o establish per 
+00014280: 7643 5055 206f 6e20 6561 6368 206e 6f64  vCPU on each nod
+00014290: 6520 696e 2074 6865 2057 6f72 6b65 7220  e in the Worker 
+000142a0: 506f 6f6c 2e20 284f 7665 7272 6964 6573  Pool. (Overrides
+000142b0: 2060 776f 726b 6572 7350 6572 4e6f 6465   `workersPerNode
+000142c0: 602e 2920 2020 2020 2020 2020 2020 2020  `.)             
+000142d0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000142e0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+000142f0: 776f 726b 6572 7350 6572 4e6f 6465 6020  workersPerNode` 
+00014300: 2020 2020 2020 2020 207c 2054 6865 206e           | The n
+00014310: 756d 6265 7220 6f66 2057 6f72 6b65 7273  umber of Workers
+00014320: 2074 6f20 6573 7461 626c 6973 6820 6f6e   to establish on
+00014330: 2065 6163 6820 6e6f 6465 2069 6e20 7468   each node in th
+00014340: 6520 576f 726b 6572 2050 6f6f 6c2e 2020  e Worker Pool.  
+00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014380: 2020 207c 2060 3160 2020 2020 2020 2020     | `1`        
+00014390: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000143a0: 2060 776f 726b 6572 506f 6f6c 4461 7461   `workerPoolData
+000143b0: 6020 2020 2020 2020 2020 207c 2054 6865  `          | The
+000143c0: 206e 616d 6520 6f66 2061 2066 696c 6520   name of a file 
+000143d0: 636f 6e74 6169 6e69 6e67 2061 204a 534f  containing a JSO
+000143e0: 4e20 646f 6375 6d65 6e74 2064 6566 696e  N document defin
+000143f0: 696e 6720 6120 576f 726b 6572 2050 6f6f  ing a Worker Poo
+00014400: 6c2e 2020 2020 2020 2020 2020 2020 2020  l.              
+00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014430: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00014440: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00014450: 0a7c 2060 776f 726b 6572 5461 6760 2020  .| `workerTag`  
+00014460: 2020 2020 2020 2020 2020 2020 207c 2054               | T
+00014470: 6865 2057 6f72 6b65 7220 5461 6720 746f  he Worker Tag to
+00014480: 2070 7562 6c69 7368 2066 6f72 2074 6865   publish for the
+00014490: 2061 6c6c 206f 6620 7468 6520 576f 726b   all of the Work
+000144a0: 6572 7320 6f6e 2074 6865 206e 6f64 652e  ers on the node.
+000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144e0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014500: 207c 0a0a 2323 2041 7574 6f6d 6174 6963   |..## Automatic
+00014510: 2050 726f 7065 7274 6965 730a 0a54 6865   Properties..The
+00014520: 206e 616d 6520 6f66 2074 6865 2057 6f72   name of the Wor
+00014530: 6b65 7220 506f 6f6c 2c20 6966 206e 6f74  ker Pool, if not
+00014540: 2073 7570 706c 6965 642c 2069 7320 6175   supplied, is au
+00014550: 746f 6d61 7469 6361 6c6c 7920 6765 6e65  tomatically gene
+00014560: 7261 7465 6420 7573 696e 6720 6120 636f  rated using a co
+00014570: 6e63 6174 656e 6174 696f 6e20 6f66 2060  ncatenation of `
+00014580: 7770 5f60 2c20 7468 6520 6074 6167 6020  wp_`, the `tag` 
+00014590: 7072 6f70 6572 7479 2c20 6120 5554 4320  property, a UTC 
+000145a0: 7469 6d65 7374 616d 702c 2061 6e64 2074  timestamp, and t
+000145b0: 6872 6565 2072 616e 646f 6d20 6865 7820  hree random hex 
+000145c0: 6368 6172 6163 7465 7273 3a20 652c 672c  characters: e,g,
+000145d0: 2e20 6077 705f 6d79 7461 675f 3232 3130  . `wp_mytag_2210
+000145e0: 3234 2d31 3535 3532 342d 6230 6160 2e0a  24-155524-b0a`..
+000145f0: 0a23 2320 544f 4d4c 2050 726f 7065 7274  .## TOML Propert
+00014600: 6965 7320 696e 2074 6865 2060 776f 726b  ies in the `work
+00014610: 6572 506f 6f6c 6020 5365 6374 696f 6e0a  erPool` Section.
+00014620: 0a48 6572 6527 7320 616e 2065 7861 6d70  .Here's an examp
+00014630: 6c65 206f 6620 7468 6520 6077 6f72 6b65  le of the `worke
+00014640: 7250 6f6f 6c60 2073 6563 7469 6f6e 206f  rPool` section o
+00014650: 6620 6120 544f 4d4c 2063 6f6e 6669 6775  f a TOML configu
+00014660: 7261 7469 6f6e 2066 696c 652c 2073 686f  ration file, sho
+00014670: 7769 6e67 2061 6c6c 2074 6865 2070 6f73  wing all the pos
+00014680: 7369 626c 6520 7072 6f70 6572 7469 6573  sible properties
+00014690: 2074 6861 7420 6361 6e20 6265 2073 6574   that can be set
+000146a0: 3a0a 0a60 6060 746f 6d6c 0a5b 776f 726b  :..```toml.[work
+000146b0: 6572 506f 6f6c 5d0a 2020 2020 6964 6c65  erPool].    idle
+000146c0: 4e6f 6465 5368 7574 646f 776e 456e 6162  NodeShutdownEnab
+000146d0: 6c65 6420 3d20 7472 7565 0a20 2020 2069  led = true.    i
+000146e0: 646c 654e 6f64 6553 6875 7464 6f77 6e54  dleNodeShutdownT
+000146f0: 696d 656f 7574 203d 2031 302e 300a 2020  imeout = 10.0.  
+00014700: 2020 6964 6c65 506f 6f6c 5368 7574 646f    idlePoolShutdo
+00014710: 776e 456e 6162 6c65 6420 3d20 7472 7565  wnEnabled = true
+00014720: 0a20 2020 2069 646c 6550 6f6f 6c53 6875  .    idlePoolShu
+00014730: 7464 6f77 6e54 696d 656f 7574 203d 2036  tdownTimeout = 6
+00014740: 302e 300a 2020 2020 696d 6167 6573 4964  0.0.    imagesId
+00014750: 203d 2022 7964 6964 3a69 6d67 6661 6d3a   = "ydid:imgfam:
+00014760: 3030 3030 3030 3a34 3139 3632 3539 322d  000000:41962592-
+00014770: 3537 3763 2d34 6664 652d 6162 3033 2d64  577c-4fde-ab03-d
+00014780: 3835 3234 3635 6537 6638 6222 0a20 2020  852465e7f8b".   
+00014790: 2069 6e73 7461 6e63 6554 6167 7320 3d20   instanceTags = 
+000147a0: 7b7d 0a20 2020 206d 6178 4e6f 6465 7320  {}.    maxNodes 
+000147b0: 3d20 310a 2020 2020 6d69 6e4e 6f64 6573  = 1.    minNodes
+000147c0: 203d 2031 0a20 2020 206e 616d 6520 3d20   = 1.    name = 
+000147d0: 226d 792d 776f 726b 6572 2d70 6f6f 6c22  "my-worker-pool"
+000147e0: 0a20 2020 206e 6f64 6542 6f6f 7454 696d  .    nodeBootTim
+000147f0: 656f 7574 203d 2035 0a20 2020 2074 6172  eout = 5.    tar
+00014800: 6765 7449 6e73 7461 6e63 6543 6f75 6e74  getInstanceCount
+00014810: 203d 2031 0a20 2020 2074 656d 706c 6174   = 1.    templat
+00014820: 6549 6420 3d20 2279 6469 643a 6372 743a  eId = "ydid:crt:
+00014830: 4439 4335 3438 3a34 3635 6131 3037 632d  D9C548:465a107c-
+00014840: 3763 6561 2d34 3665 332d 3966 6464 2d31  7cea-46e3-9fdd-1
+00014850: 3531 3136 6362 3932 6334 3022 0a20 2020  5116cb92c40".   
+00014860: 2023 204e 6f74 653a 206f 6e6c 7920 6f6e   # Note: only on
+00014870: 6520 6f66 2027 7573 6572 4461 7461 272f  e of 'userData'/
+00014880: 2775 7365 7244 6174 6146 696c 6527 2f27  'userDataFile'/'
+00014890: 7573 6572 4461 7461 4669 6c65 7327 2073  userDataFiles' s
+000148a0: 686f 756c 6420 6265 2073 6574 0a20 2020  hould be set.   
+000148b0: 2075 7365 7244 6174 6120 3d20 2222 0a20   userData = "". 
+000148c0: 2020 2075 7365 7244 6174 6146 696c 6520     userDataFile 
+000148d0: 3d20 226d 7975 7365 7264 6174 612e 7478  = "myuserdata.tx
+000148e0: 7422 0a20 2020 2075 7365 7244 6174 6146  t".    userDataF
+000148f0: 696c 6573 203d 205b 226d 7975 7365 7264  iles = ["myuserd
+00014900: 6174 6131 2e74 7874 222c 2022 6d79 7573  ata1.txt", "myus
+00014910: 6572 6461 7461 322e 7478 7422 5d0a 2020  erdata2.txt"].  
+00014920: 2020 776f 726b 6572 5461 6720 3d20 2274    workerTag = "t
+00014930: 6167 2d7b 7b75 7365 726e 616d 657d 7d22  ag-{{username}}"
+00014940: 0a20 2020 2023 2053 7065 6369 6679 2065  .    # Specify e
+00014950: 6974 6865 7220 776f 726b 6572 7350 6572  ither workersPer
+00014960: 4e6f 6465 206f 7220 776f 726b 6572 7350  Node or workersP
+00014970: 6572 5643 5055 0a20 2020 2077 6f72 6b65  erVCPU.    worke
+00014980: 7273 5065 724e 6f64 6520 3d20 310a 2020  rsPerNode = 1.  
+00014990: 2020 776f 726b 6572 7350 6572 5643 5055    workersPerVCPU
+000149a0: 203d 2031 0a23 2020 2077 6f72 6b65 7250   = 1.#   workerP
+000149b0: 6f6f 6c44 6174 6120 3d20 2277 6f72 6b65  oolData = "worke
+000149c0: 725f 706f 6f6c 2e6a 736f 6e22 0a60 6060  r_pool.json".```
+000149d0: 0a0a 2323 2057 6f72 6b65 7220 506f 6f6c  ..## Worker Pool
+000149e0: 2053 7065 6369 6669 6361 7469 6f6e 2055   Specification U
+000149f0: 7369 6e67 204a 534f 4e20 446f 6375 6d65  sing JSON Docume
+00014a00: 6e74 730a 0a49 7427 7320 616c 736f 2070  nts..It's also p
+00014a10: 6f73 7369 626c 6520 746f 2063 6170 7475  ossible to captu
+00014a20: 7265 2061 2057 6f72 6b65 7220 506f 6f6c  re a Worker Pool
+00014a30: 2064 6566 696e 6974 696f 6e20 6173 2061   definition as a
+00014a40: 204a 534f 4e20 646f 6375 6d65 6e74 2e20   JSON document. 
+00014a50: 5468 6520 4a53 4f4e 2066 696c 656e 616d  The JSON filenam
+00014a60: 6520 6361 6e20 6265 2073 7570 706c 6965  e can be supplie
+00014a70: 6420 6569 7468 6572 2075 7369 6e67 2074  d either using t
+00014a80: 6865 2063 6f6d 6d61 6e64 206c 696e 6520  he command line 
+00014a90: 7769 7468 2074 6865 2060 2d2d 776f 726b  with the `--work
+00014aa0: 6572 2d70 6f6f 6c60 206f 7220 602d 7060  er-pool` or `-p`
+00014ab0: 2070 6172 616d 6574 6572 2077 6974 6820   parameter with 
+00014ac0: 6079 642d 7072 6f76 6973 696f 6e60 2c20  `yd-provision`, 
+00014ad0: 6f72 2062 7920 706f 7075 6c61 7469 6e67  or by populating
+00014ae0: 2074 6865 2060 776f 726b 6572 506f 6f6c   the `workerPool
+00014af0: 4461 7461 6020 7072 6f70 6572 7479 2069  Data` property i
+00014b00: 6e20 7468 6520 544f 4d4c 2063 6f6e 6669  n the TOML confi
+00014b10: 6775 7261 7469 6f6e 2066 696c 6520 7769  guration file wi
+00014b20: 7468 2074 6865 204a 534f 4e20 6669 6c65  th the JSON file
+00014b30: 6e61 6d65 2e20 436f 6d6d 616e 6420 6c69  name. Command li
+00014b40: 6e65 2073 7065 6369 6669 6361 7469 6f6e  ne specification
+00014b50: 2074 616b 6573 2070 7269 6f72 6974 7920   takes priority 
+00014b60: 6f76 6572 2054 4f4d 4c20 7370 6563 6966  over TOML specif
+00014b70: 6963 6174 696f 6e2e 0a0a 5468 6520 4a53  ication...The JS
+00014b80: 4f4e 2073 7065 6369 6669 6361 7469 6f6e  ON specification
+00014b90: 2061 6c6c 6f77 7320 7468 6520 6372 6561   allows the crea
+00014ba0: 7469 6f6e 206f 6620 2a2a 4164 7661 6e63  tion of **Advanc
+00014bb0: 6564 2057 6f72 6b65 7220 506f 6f6c 732a  ed Worker Pools*
+00014bc0: 2a2c 2077 6974 6820 6469 6666 6572 656e  *, with differen
+00014bd0: 7420 6e6f 6465 2074 7970 6573 2061 6e64  t node types and
+00014be0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
+00014bf0: 7370 6563 6966 7920 4e6f 6465 2041 6374  specify Node Act
+00014c00: 696f 6e73 2e0a 0a57 6865 6e20 7573 696e  ions...When usin
+00014c10: 6720 6120 4a53 4f4e 2064 6f63 756d 656e  g a JSON documen
+00014c20: 7420 746f 2073 7065 6369 6679 2074 6865  t to specify the
+00014c30: 2057 6f72 6b65 7220 506f 6f6c 2c20 7468   Worker Pool, th
+00014c40: 6520 7363 6865 6d61 206f 6620 7468 6520  e schema of the 
+00014c50: 646f 6375 6d65 6e74 2069 7320 6964 656e  document is iden
+00014c60: 7469 6361 6c20 746f 2074 6861 7420 6578  tical to that ex
+00014c70: 7065 6374 6564 2062 7920 7468 6520 5965  pected by the Ye
+00014c80: 6c6c 6f77 446f 6720 5245 5354 2041 5049  llowDog REST API
+00014c90: 2066 6f72 2057 6f72 6b65 7220 506f 6f6c   for Worker Pool
+00014ca0: 2050 726f 7669 7369 6f6e 696e 672e 0a0a   Provisioning...
+00014cb0: 2323 2320 576f 726b 6572 2050 6f6f 6c20  ### Worker Pool 
+00014cc0: 4a53 4f4e 2045 7861 6d70 6c65 730a 0a54  JSON Examples..T
+00014cd0: 6865 2065 7861 6d70 6c65 2062 656c 6f77  he example below
+00014ce0: 2069 7320 6f66 2061 2073 696d 706c 6520   is of a simple 
+00014cf0: 4a53 4f4e 2073 7065 6369 6669 6361 7469  JSON specificati
+00014d00: 6f6e 206f 6620 6120 576f 726b 6572 2050  on of a Worker P
+00014d10: 6f6f 6c20 7769 7468 206f 6e65 2069 6e69  ool with one ini
+00014d20: 7469 616c 206e 6f64 652c 2057 6f72 6b65  tial node, Worke
+00014d30: 7220 506f 6f6c 2073 6875 7464 6f77 6e2c  r Pool shutdown,
+00014d40: 2065 7463 2e0a 0a60 6060 6a73 6f6e 0a7b   etc...```json.{
+00014d50: 0a20 2022 7265 7175 6972 656d 656e 7454  .  "requirementT
+00014d60: 656d 706c 6174 6555 7361 6765 223a 207b  emplateUsage": {
+00014d70: 0a20 2020 2022 6d61 696e 7461 696e 496e  .    "maintainIn
+00014d80: 7374 616e 6365 436f 756e 7422 3a20 6661  stanceCount": fa
+00014d90: 6c73 652c 0a20 2020 2022 7265 7175 6972  lse,.    "requir
+00014da0: 656d 656e 744e 616d 6522 3a20 2277 705f  ementName": "wp_
+00014db0: 7079 6578 2d70 7269 6d65 735f 3233 3031  pyex-primes_2301
+00014dc0: 3133 2d31 3631 3532 382d 6461 3022 2c0a  13-161528-da0",.
+00014dd0: 2020 2020 2272 6571 7569 7265 6d65 6e74      "requirement
+00014de0: 4e61 6d65 7370 6163 6522 3a20 2270 7965  Namespace": "pye
+00014df0: 7861 6d70 6c65 7322 2c0a 2020 2020 2272  xamples",.    "r
+00014e00: 6571 7569 7265 6d65 6e74 5461 6722 3a20  equirementTag": 
+00014e10: 2270 7965 782d 7072 696d 6573 222c 0a20  "pyex-primes",. 
+00014e20: 2020 2022 7461 7267 6574 496e 7374 616e     "targetInstan
+00014e30: 6365 436f 756e 7422 3a20 312c 0a20 2020  ceCount": 1,.   
+00014e40: 2022 7465 6d70 6c61 7465 4964 223a 2022   "templateId": "
+00014e50: 7964 6964 3a63 7274 3a44 3943 3534 383a  ydid:crt:D9C548:
+00014e60: 3436 3561 3130 3763 2d37 6365 612d 3436  465a107c-7cea-46
+00014e70: 6533 2d39 6664 642d 3135 3131 3663 6239  e3-9fdd-15116cb9
+00014e80: 3263 3430 220a 2020 7d2c 0a20 2022 7072  2c40".  },.  "pr
+00014e90: 6f76 6973 696f 6e65 6450 726f 7065 7274  ovisionedPropert
+00014ea0: 6965 7322 3a20 7b0a 2020 2020 2269 646c  ies": {.    "idl
+00014eb0: 654e 6f64 6553 6875 7464 6f77 6e22 3a20  eNodeShutdown": 
+00014ec0: 7b22 656e 6162 6c65 6422 3a20 7472 7565  {"enabled": true
+00014ed0: 2c20 2274 696d 656f 7574 223a 2022 5054  , "timeout": "PT
+00014ee0: 3130 4d22 7d2c 0a20 2020 2022 6964 6c65  10M"},.    "idle
+00014ef0: 506f 6f6c 5368 7574 646f 776e 223a 207b  PoolShutdown": {
+00014f00: 2265 6e61 626c 6564 223a 2074 7275 652c  "enabled": true,
+00014f10: 2022 7469 6d65 6f75 7422 3a20 2250 5431   "timeout": "PT1
+00014f20: 4822 7d2c 0a20 2020 2022 6372 6561 7465  H"},.    "create
+00014f30: 4e6f 6465 576f 726b 6572 7322 3a20 7b22  NodeWorkers": {"
+00014f40: 7461 7267 6574 436f 756e 7422 3a20 312c  targetCount": 1,
+00014f50: 2022 7461 7267 6574 5479 7065 223a 2022   "targetType": "
+00014f60: 5045 525f 5643 5055 227d 2c0a 2020 2020  PER_VCPU"},.    
+00014f70: 226d 6178 4e6f 6465 7322 3a20 352c 0a20  "maxNodes": 5,. 
+00014f80: 2020 2022 6d69 6e4e 6f64 6573 223a 2030     "minNodes": 0
+00014f90: 2c0a 2020 2020 226e 6f64 6542 6f6f 7454  ,.    "nodeBootT
+00014fa0: 696d 656f 7574 223a 2022 5054 354d 222c  imeout": "PT5M",
+00014fb0: 0a20 2020 2022 6e6f 6465 4964 6c65 4772  .    "nodeIdleGr
+00014fc0: 6163 6550 6572 696f 6422 3a20 2250 5433  acePeriod": "PT3
+00014fd0: 4d22 2c0a 2020 2020 226e 6f64 6549 646c  M",.    "nodeIdl
+00014fe0: 6554 696d 654c 696d 6974 223a 2022 5054  eTimeLimit": "PT
+00014ff0: 334d 222c 0a20 2020 2022 776f 726b 6572  3M",.    "worker
+00015000: 5461 6722 3a20 2270 7965 782d 6261 7368  Tag": "pyex-bash
+00015010: 2d64 6f63 6b65 7222 0a20 207d 0a7d 0a60  -docker".  }.}.`
+00015020: 6060 0a0a 5468 6520 6e65 7874 2065 7861  ``..The next exa
+00015030: 6d70 6c65 2069 7320 6f66 2061 2072 656c  mple is of a rel
+00015040: 6174 6976 656c 7920 7269 6368 204a 534f  atively rich JSO
+00015050: 4e20 7370 6563 6966 6963 6174 696f 6e20  N specification 
+00015060: 6f66 2061 6e20 4164 7661 6e63 6564 2057  of an Advanced W
+00015070: 6f72 6b65 7220 506f 6f6c 2c20 6672 6f6d  orker Pool, from
+00015080: 206f 6e65 206f 6620 7468 6520 5965 6c6c   one of the Yell
+00015090: 6f77 446f 6720 6465 6d6f 732e 2049 7420  owDog demos. It 
+000150a0: 696e 636c 7564 6573 206e 6f64 6520 7370  includes node sp
+000150b0: 6563 6961 6c69 7361 7469 6f6e 2c20 616e  ecialisation, an
+000150c0: 6420 6163 7469 6f6e 2067 726f 7570 7320  d action groups 
+000150d0: 7468 6174 2072 6573 706f 6e64 2074 6f20  that respond to 
+000150e0: 7468 6520 6053 5441 5254 5550 5f4e 4f44  the `STARTUP_NOD
+000150f0: 4553 5f41 4444 4544 6020 616e 6420 604e  ES_ADDED` and `N
+00015100: 4f44 4553 5f41 4444 4544 6020 6576 656e  ODES_ADDED` even
+00015110: 7473 2074 6f20 6472 6976 6520 2a2a 4e6f  ts to drive **No
+00015120: 6465 2041 6374 696f 6e73 2a2a 2e0a 0a60  de Actions**...`
+00015130: 6060 6a73 6f6e 0a7b 0a20 2022 7265 7175  ``json.{.  "requ
+00015140: 6972 656d 656e 7454 656d 706c 6174 6555  irementTemplateU
+00015150: 7361 6765 223a 207b 0a20 2020 2022 6d61  sage": {.    "ma
+00015160: 696e 7461 696e 496e 7374 616e 6365 436f  intainInstanceCo
+00015170: 756e 7422 3a20 6661 6c73 652c 0a20 2020  unt": false,.   
+00015180: 2022 7461 7267 6574 496e 7374 616e 6365   "targetInstance
+00015190: 436f 756e 7422 3a20 362c 0a20 2020 2022  Count": 6,.    "
+000151a0: 7465 6d70 6c61 7465 4964 223a 2022 7964  templateId": "yd
+000151b0: 6964 3a63 7274 3a44 3943 3534 383a 6137  id:crt:D9C548:a7
+000151c0: 6564 6132 3837 2d66 3964 362d 3462 6338  eda287-f9d6-4bc8
+000151d0: 2d62 3264 632d 3435 3533 3434 3035 3732  -b2dc-4553440572
+000151e0: 3537 222c 0a20 2020 2022 7265 7175 6972  57",.    "requir
+000151f0: 656d 656e 744e 616d 6522 3a20 2277 705f  ementName": "wp_
+00015200: 7079 6578 2d73 6c75 726d 5f32 3330 3131  pyex-slurm_23011
+00015210: 332d 3136 3536 3135 2d32 6237 222c 0a20  3-165615-2b7",. 
+00015220: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
+00015230: 616d 6573 7061 6365 223a 2022 7079 6578  amespace": "pyex
+00015240: 616d 706c 6573 222c 0a20 2020 2022 7265  amples",.    "re
+00015250: 7175 6972 656d 656e 7454 6167 223a 2022  quirementTag": "
+00015260: 7079 6578 2d73 6c75 726d 220a 2020 7d2c  pyex-slurm".  },
+00015270: 0a20 2022 7072 6f76 6973 696f 6e65 6450  .  "provisionedP
+00015280: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00015290: 2020 2263 7265 6174 654e 6f64 6557 6f72    "createNodeWor
+000152a0: 6b65 7273 223a 207b 2274 6172 6765 7443  kers": {"targetC
+000152b0: 6f75 6e74 223a 2030 2c20 2274 6172 6765  ount": 0, "targe
+000152c0: 7454 7970 6522 3a20 2250 4552 5f4e 4f44  tType": "PER_NOD
+000152d0: 4522 7d2c 0a20 2020 2022 6e6f 6465 436f  E"},.    "nodeCo
+000152e0: 6e66 6967 7572 6174 696f 6e22 3a20 7b0a  nfiguration": {.
+000152f0: 2020 2020 2020 226e 6f64 6554 7970 6573        "nodeTypes
+00015300: 223a 205b 0a20 2020 2020 2020 207b 226e  ": [.        {"n
+00015310: 616d 6522 3a20 2273 6c75 726d 6374 6c64  ame": "slurmctld
+00015320: 222c 2022 636f 756e 7422 3a20 317d 2c0a  ", "count": 1},.
+00015330: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00015340: 2022 736c 7572 6d64 222c 2022 6d69 6e22   "slurmd", "min"
+00015350: 3a20 352c 2022 736c 6f74 4e75 6d62 6572  : 5, "slotNumber
+00015360: 696e 6722 3a20 2252 4555 5341 424c 4522  ing": "REUSABLE"
+00015370: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
+00015380: 2022 6e6f 6465 4576 656e 7473 223a 207b   "nodeEvents": {
+00015390: 0a20 2020 2020 2020 2022 5354 4152 5455  .        "STARTU
+000153a0: 505f 4e4f 4445 535f 4144 4445 4422 3a20  P_NODES_ADDED": 
+000153b0: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
+000153c0: 2020 2020 2020 2020 2020 2261 6374 696f            "actio
+000153d0: 6e73 223a 205b 0a20 2020 2020 2020 2020  ns": [.         
+000153e0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000153f0: 2020 2020 2020 2022 6163 7469 6f6e 223a         "action":
+00015400: 2022 5752 4954 455f 4649 4c45 222c 0a20   "WRITE_FILE",. 
+00015410: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015420: 7061 7468 223a 2022 6e6f 6465 732e 6a73  path": "nodes.js
+00015430: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00015440: 2020 2020 2022 636f 6e74 656e 7422 3a20       "content": 
+00015450: 227b 5c6e 2020 5c22 6e6f 6465 735c 223a  "{\n  \"nodes\":
+00015460: 205b 5c6e 7b7b 236f 7468 6572 4e6f 6465   [\n{{#otherNode
+00015470: 737d 7d5c 6e20 2020 207b 5c6e 2020 2020  s}}\n    {\n    
+00015480: 2020 5c22 6e61 6d65 5c22 3a20 5c22 736c    \"name\": \"sl
+00015490: 7572 6d64 7b7b 6465 7461 696c 732e 6e6f  urmd{{details.no
+000154a0: 6465 536c 6f74 7d7d 5c22 2c5c 6e20 2020  deSlot}}\",\n   
+000154b0: 2020 205c 2269 705c 223a 205c 227b 7b64     \"ip\": \"{{d
+000154c0: 6574 6169 6c73 2e70 7269 7661 7465 4970  etails.privateIp
+000154d0: 4164 6472 6573 737d 7d5c 225c 6e20 2020  Address}}\"\n   
+000154e0: 207d 7b7b 5e2d 6c61 7374 7d7d 2c7b 7b2f   }{{^-last}},{{/
+000154f0: 2d6c 6173 747d 7d5c 6e7b 7b2f 6f74 6865  -last}}\n{{/othe
+00015500: 724e 6f64 6573 7d7d 5c6e 2020 5d5c 6e7d  rNodes}}\n  ]\n}
+00015510: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00015520: 2020 2022 6e6f 6465 5479 7065 7322 3a20     "nodeTypes": 
+00015530: 5b22 736c 7572 6d63 746c 6422 5d0a 2020  ["slurmctld"].  
+00015540: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00015550: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00015560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015570: 6163 7469 6f6e 223a 2022 5255 4e5f 434f  action": "RUN_CO
+00015580: 4d4d 414e 4422 2c0a 2020 2020 2020 2020  MMAND",.        
 00015590: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
-000155a0: 226e 6f64 6573 2e6a 736f 6e22 2c0a 2020  "nodes.json",.  
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000155c0: 6f6e 7465 6e74 223a 2022 7b5c 6e20 205c  ontent": "{\n  \
-000155d0: 226e 6f64 6573 5c22 3a20 5b5c 6e7b 7b23  "nodes\": [\n{{#
-000155e0: 6669 6c74 6572 6564 4e6f 6465 737d 7d5c  filteredNodes}}\
-000155f0: 6e20 2020 207b 5c6e 2020 2020 2020 5c22  n    {\n      \"
-00015600: 6e61 6d65 5c22 3a20 5c22 736c 7572 6d64  name\": \"slurmd
-00015610: 7b7b 6465 7461 696c 732e 6e6f 6465 536c  {{details.nodeSl
-00015620: 6f74 7d7d 5c22 2c5c 6e20 2020 2020 205c  ot}}\",\n      \
-00015630: 2269 705c 223a 205c 227b 7b64 6574 6169  "ip\": \"{{detai
-00015640: 6c73 2e70 7269 7661 7465 4970 4164 6472  ls.privateIpAddr
-00015650: 6573 737d 7d5c 225c 6e20 2020 207d 7b7b  ess}}\"\n    }{{
-00015660: 5e2d 6c61 7374 7d7d 2c7b 7b2f 2d6c 6173  ^-last}},{{/-las
-00015670: 747d 7d5c 6e7b 7b2f 6669 6c74 6572 6564  t}}\n{{/filtered
-00015680: 4e6f 6465 737d 7d5c 6e20 205d 5c6e 7d22  Nodes}}\n  ]\n}"
-00015690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000156a0: 2020 226e 6f64 6554 7970 6573 223a 205b    "nodeTypes": [
-000156b0: 2273 6c75 726d 6374 6c64 225d 0a20 2020  "slurmctld"].   
-000156c0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000156d0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000156e0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-000156f0: 6374 696f 6e22 3a20 2252 554e 5f43 4f4d  ction": "RUN_COM
-00015700: 4d41 4e44 222c 0a20 2020 2020 2020 2020  MAND",.         
-00015710: 2020 2020 2020 2022 7061 7468 223a 2022         "path": "
-00015720: 6164 645f 6e6f 6465 7322 2c0a 2020 2020  add_nodes",.    
-00015730: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
-00015740: 756d 656e 7473 223a 205b 226e 6f64 6573  uments": ["nodes
-00015750: 2e6a 736f 6e22 5d2c 0a20 2020 2020 2020  .json"],.       
-00015760: 2020 2020 2020 2020 2022 6e6f 6465 5479           "nodeTy
-00015770: 7065 7322 3a20 5b22 736c 7572 6d63 746c  pes": ["slurmctl
-00015780: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-00015790: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000157a0: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
-000157b0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-000157c0: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
-000157d0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-000157e0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000157f0: 2020 2020 2261 6374 696f 6e22 3a20 2252      "action": "R
-00015800: 554e 5f43 4f4d 4d41 4e44 222c 0a20 2020  UN_COMMAND",.   
-00015810: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00015820: 7468 223a 2022 7374 6172 745f 7369 6d70  th": "start_simp
-00015830: 6c65 5f73 6c75 726d 6422 2c0a 2020 2020  le_slurmd",.    
-00015840: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
-00015850: 756d 656e 7473 223a 205b 227b 7b6e 6f64  uments": ["{{nod
-00015860: 6573 4279 5479 7065 2e73 6c75 726d 6374  esByType.slurmct
-00015870: 6c64 2e30 2e64 6574 6169 6c73 2e70 7269  ld.0.details.pri
-00015880: 7661 7465 4970 4164 6472 6573 737d 7d22  vateIpAddress}}"
-00015890: 2c20 227b 7b6e 6f64 652e 6465 7461 696c  , "{{node.detail
-000158a0: 732e 6e6f 6465 536c 6f74 7d7d 225d 2c0a  s.nodeSlot}}"],.
-000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158c0: 226e 6f64 6549 6446 696c 7465 7222 3a20  "nodeIdFilter": 
-000158d0: 2245 5645 4e54 222c 0a20 2020 2020 2020  "EVENT",.       
-000158e0: 2020 2020 2020 2020 2022 6e6f 6465 5479           "nodeTy
-000158f0: 7065 7322 3a20 5b22 736c 7572 6d64 225d  pes": ["slurmd"]
-00015900: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
-00015910: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00015920: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00015930: 2020 205d 0a20 2020 2020 207d 0a20 2020     ].      }.   
-00015940: 207d 2c0a 2020 2020 2277 6f72 6b65 7254   },.    "workerT
-00015950: 6167 223a 2022 7079 6578 2d73 6c75 726d  ag": "pyex-slurm
-00015960: 2d63 6c75 7374 6572 220a 2020 7d0a 7d0a  -cluster".  }.}.
-00015970: 6060 600a 0a23 2323 2054 4f4d 4c20 5072  ```..### TOML Pr
-00015980: 6f70 6572 7469 6573 2049 6e68 6572 6974  operties Inherit
-00015990: 6564 2062 7920 576f 726b 6572 2050 6f6f  ed by Worker Poo
-000159a0: 6c20 4a53 4f4e 2053 7065 6369 6669 6361  l JSON Specifica
-000159b0: 7469 6f6e 730a 0a57 6865 6e20 6120 4a53  tions..When a JS
-000159c0: 4f4e 2057 6f72 6b65 7220 506f 6f6c 2073  ON Worker Pool s
-000159d0: 7065 6369 6669 6361 7469 6f6e 2069 7320  pecification is 
-000159e0: 7573 6564 2c20 7468 6520 666f 6c6c 6f77  used, the follow
-000159f0: 696e 6720 7072 6f70 6572 7469 6573 2066  ing properties f
-00015a00: 726f 6d20 7468 6520 6063 6f6e 6669 672e  rom the `config.
-00015a10: 746f 6d6c 6020 6669 6c65 2077 696c 6c20  toml` file will 
-00015a20: 6265 2069 6e68 6572 6974 6564 2069 6620  be inherited if 
-00015a30: 7468 6520 7661 6c75 6520 6973 2061 6273  the value is abs
-00015a40: 656e 7420 696e 2074 6865 204a 534f 4e20  ent in the JSON 
-00015a50: 6669 6c65 3a0a 0a2a 2a50 726f 7065 7274  file:..**Propert
-00015a60: 6965 7320 496e 6865 7269 7465 6420 7769  ies Inherited wi
-00015a70: 7468 696e 2074 6865 2060 7265 7175 6972  thin the `requir
-00015a80: 656d 656e 7454 656d 706c 6174 6555 7361  ementTemplateUsa
-00015a90: 6765 6020 7072 6f70 6572 7479 2a2a 0a0a  ge` property**..
-00015aa0: 2d20 6069 6d61 6765 7349 6460 0a2d 2060  - `imagesId`.- `
-00015ab0: 696e 7374 616e 6365 5461 6773 600a 2d20  instanceTags`.- 
-00015ac0: 6072 6571 7569 7265 6d65 6e74 4e61 6d65  `requirementName
-00015ad0: 603a 2064 6572 6976 6564 2066 726f 6d20  `: derived from 
-00015ae0: 7468 6520 606e 616d 6560 2070 726f 7065  the `name` prope
-00015af0: 7274 7920 696e 2074 6865 2060 544f 4d4c  rty in the `TOML
-00015b00: 6020 636f 6e66 6967 7572 6174 696f 6e2e  ` configuration.
-00015b10: 2028 5468 6520 6e61 6d65 2077 696c 6c20   (The name will 
-00015b20: 6265 2067 656e 6572 6174 6564 2061 7574  be generated aut
-00015b30: 6f6d 6174 6963 616c 6c79 2069 6620 6e6f  omatically if no
-00015b40: 7420 7375 7070 6c69 6564 2069 6e20 6569  t supplied in ei
-00015b50: 7468 6572 2074 6865 2054 4f4d 4c20 6669  ther the TOML fi
-00015b60: 6c65 206f 7220 7468 6520 4a53 4f4e 2073  le or the JSON s
-00015b70: 7065 6369 6669 6361 7469 6f6e 2e29 0a2d  pecification.).-
-00015b80: 2060 7265 7175 6972 656d 656e 744e 616d   `requirementNam
-00015b90: 6573 7061 6365 603a 2064 6572 6976 6564  espace`: derived
-00015ba0: 2066 726f 6d20 7468 6520 606e 616d 6573   from the `names
-00015bb0: 7061 6365 6020 7072 6f70 6572 7479 2069  pace` property i
-00015bc0: 6e20 7468 6520 6054 4f4d 4c60 2063 6f6e  n the `TOML` con
-00015bd0: 6669 6775 7261 7469 6f6e 0a2d 2060 7265  figuration.- `re
-00015be0: 7175 6972 656d 656e 7454 6167 603a 203a  quirementTag`: :
-00015bf0: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
-00015c00: 6520 6074 6167 6020 7072 6f70 6572 7479  e `tag` property
-00015c10: 2069 6e20 7468 6520 6054 4f4d 4c60 2063   in the `TOML` c
-00015c20: 6f6e 6669 6775 7261 7469 6f6e 0a2d 2060  onfiguration.- `
-00015c30: 7461 7267 6574 496e 7374 616e 6365 436f  targetInstanceCo
-00015c40: 756e 7460 0a2d 2060 7465 6d70 6c61 7465  unt`.- `template
-00015c50: 4964 600a 2d20 6075 7365 7244 6174 6160  Id`.- `userData`
-00015c60: 0a2d 2060 7573 6572 4461 7461 4669 6c65  .- `userDataFile
-00015c70: 600a 2d20 6075 7365 7244 6174 6146 696c  `.- `userDataFil
-00015c80: 6573 600a 0a2a 2a50 726f 7065 7274 6965  es`..**Propertie
-00015c90: 7320 496e 6865 7269 7465 6420 7769 7468  s Inherited with
-00015ca0: 696e 2074 6865 2060 7072 6f76 6973 696f  in the `provisio
-00015cb0: 6e65 6450 726f 7065 7274 6965 7360 2050  nedProperties` P
-00015cc0: 726f 7065 7274 792a 2a0a 0a2d 2060 6964  roperty**..- `id
-00015cd0: 6c65 4e6f 6465 5368 7574 646f 776e 456e  leNodeShutdownEn
-00015ce0: 6162 6c65 6460 0a2d 2060 6964 6c65 4e6f  abled`.- `idleNo
-00015cf0: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
-00015d00: 7460 0a2d 2060 6964 6c65 506f 6f6c 5368  t`.- `idlePoolSh
-00015d10: 7574 646f 776e 456e 6162 6c65 6460 0a2d  utdownEnabled`.-
-00015d20: 2060 6964 6c65 506f 6f6c 5368 7574 646f   `idlePoolShutdo
-00015d30: 776e 5469 6d65 6f75 7460 0a2d 2060 6e6f  wnTimeout`.- `no
-00015d40: 6465 426f 6f74 5469 6d65 6f75 7460 0a2d  deBootTimeout`.-
-00015d50: 2060 776f 726b 6572 5461 6760 0a0a 2323   `workerTag`..##
-00015d60: 2056 6172 6961 626c 6520 5375 6273 7469   Variable Substi
-00015d70: 7475 7469 6f6e 7320 696e 2057 6f72 6b65  tutions in Worke
-00015d80: 7220 506f 6f6c 2050 726f 7065 7274 6965  r Pool Propertie
-00015d90: 730a 0a56 6172 6961 626c 6520 7375 6273  s..Variable subs
-00015da0: 7469 7475 7469 6f6e 7320 6361 6e20 6265  titutions can be
-00015db0: 2075 7365 6420 7769 7468 696e 2061 6e79   used within any
-00015dc0: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
-00015dd0: 696e 2054 4f4d 4c20 636f 6e66 6967 7572  in TOML configur
-00015de0: 6174 696f 6e20 6669 6c65 7320 6f72 2057  ation files or W
-00015df0: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
-00015e00: 6669 6c65 732e 2053 6565 2074 6865 2064  files. See the d
-00015e10: 6573 6372 6970 7469 6f6e 205b 6162 6f76  escription [abov
-00015e20: 655d 2823 7661 7269 6162 6c65 2d73 7562  e](#variable-sub
-00015e30: 7374 6974 7574 696f 6e73 2920 666f 7220  stitutions) for 
-00015e40: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
-00015e50: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
-00015e60: 7574 696f 6e73 2e20 5468 6973 2069 7320  utions. This is 
-00015e70: 6120 706f 7765 7266 756c 2066 6561 7475  a powerful featu
-00015e80: 7265 2074 6861 7420 616c 6c6f 7773 2057  re that allows W
-00015e90: 6f72 6b65 7220 506f 6f6c 7320 746f 2062  orker Pools to b
-00015ea0: 6520 7061 7261 6d65 7465 7269 7365 6420  e parameterised 
-00015eb0: 6279 2073 7570 706c 7969 6e67 2076 616c  by supplying val
-00015ec0: 7565 7320 6f6e 2074 6865 2063 6f6d 6d61  ues on the comma
-00015ed0: 6e64 206c 696e 652c 2076 6961 2065 6e76  nd line, via env
-00015ee0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00015ef0: 6573 2c20 6f72 2076 6961 2074 6865 2054  es, or via the T
-00015f00: 4f4d 4c20 6669 6c65 2e0a 0a41 6e20 696d  OML file...An im
-00015f10: 706f 7274 616e 7420 6469 7374 696e 6374  portant distinct
-00015f20: 696f 6e20 2a2a 6f6e 6c79 2a2a 2077 6865  ion **only** whe
-00015f30: 6e20 7573 696e 6720 7661 7269 6162 6c65  n using variable
-00015f40: 2073 7562 7374 6974 7574 696f 6e73 2077   substitutions w
-00015f50: 6974 6869 6e20 576f 726b 6572 2050 6f6f  ithin Worker Poo
-00015f60: 6c20 4a53 4f4e 2064 6f63 756d 656e 7473  l JSON documents
-00015f70: 2069 7320 7468 6174 2065 6163 6820 6469   is that each di
-00015f80: 7265 6374 6976 6520 2a2a 6d75 7374 2062  rective **must b
-00015f90: 6520 7072 6563 6564 6564 2062 7920 6120  e preceded by a 
-00015fa0: 605f 5f60 2028 646f 7562 6c65 2075 6e64  `__` (double und
-00015fb0: 6572 7363 6f72 6529 2a2a 2074 6f20 6469  erscore)** to di
-00015fc0: 7361 6d62 6967 7561 7465 2069 7420 6672  sambiguate it fr
-00015fd0: 6f6d 2076 6172 6961 626c 6520 7375 6273  om variable subs
-00015fe0: 7469 7475 7469 6f6e 7320 7468 6174 2061  titutions that a
-00015ff0: 7265 2074 6f20 6265 2070 6173 7365 6420  re to be passed 
-00016000: 6469 7265 6374 6c79 2074 6f20 7468 6520  directly to the 
-00016010: 4150 492e 2046 6f72 2065 7861 6d70 6c65  API. For example
-00016020: 2c20 7573 653a 2060 5f5f 7b7b 7573 6572  , use: `__{{user
-00016030: 6e61 6d65 7d7d 6020 746f 2061 7070 6c79  name}}` to apply
-00016040: 2061 2073 7562 7374 6974 7574 696f 6e20   a substitution 
-00016050: 666f 7220 7468 6520 6075 7365 726e 616d  for the `usernam
-00016060: 6560 2064 6566 6175 6c74 2073 7562 7374  e` default subst
-00016070: 6974 7574 696f 6e2e 0a0a 2323 2044 7279  itution...## Dry
-00016080: 2d52 756e 6e69 6e67 2057 6f72 6b65 7220  -Running Worker 
-00016090: 506f 6f6c 2050 726f 7669 7369 6f6e 696e  Pool Provisionin
-000160a0: 670a 0a54 6f20 6578 616d 696e 6520 7468  g..To examine th
-000160b0: 6520 4a53 4f4e 2074 6861 7420 7769 6c6c  e JSON that will
-000160c0: 2061 6374 7561 6c6c 7920 6265 2073 656e   actually be sen
-000160d0: 7420 746f 2074 6865 2059 656c 6c6f 7744  t to the YellowD
-000160e0: 6f67 2041 5049 2061 6674 6572 2061 6c6c  og API after all
-000160f0: 2070 726f 6365 7373 696e 672c 2075 7365   processing, use
-00016100: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
-00016110: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
-00016120: 7469 6f6e 2077 6865 6e20 7275 6e6e 696e  tion when runnin
-00016130: 6720 6079 642d 7072 6f76 6973 696f 6e60  g `yd-provision`
-00016140: 2e20 5468 6973 2077 696c 6c20 7072 696e  . This will prin
-00016150: 7420 7468 6520 4a53 4f4e 2073 7065 6369  t the JSON speci
-00016160: 6669 6361 7469 6f6e 2066 6f72 2074 6865  fication for the
-00016170: 2057 6f72 6b65 7220 506f 6f6c 2e20 4e6f   Worker Pool. No
-00016180: 7468 696e 6720 7769 6c6c 2062 6520 7375  thing will be su
-00016190: 626d 6974 7465 6420 746f 2074 6865 2070  bmitted to the p
-000161a0: 6c61 7466 6f72 6d2e 0a0a 5468 6520 6765  latform...The ge
-000161b0: 6e65 7261 7465 6420 4a53 4f4e 2069 7320  nerated JSON is 
-000161c0: 7072 6f64 7563 6564 2061 6674 6572 2061  produced after a
-000161d0: 6c6c 2070 726f 6365 7373 696e 6720 2869  ll processing (i
-000161e0: 6e63 6f72 706f 7261 7469 6e67 2060 636f  ncorporating `co
-000161f0: 6e66 6967 2e74 6f6d 6c60 2070 726f 7065  nfig.toml` prope
-00016200: 7274 6965 732c 2076 6172 6961 626c 6520  rties, variable 
-00016210: 7375 6273 7469 7475 7469 6f6e 732c 2065  substitutions, e
-00016220: 7463 2e29 2068 6173 2062 6565 6e20 636f  tc.) has been co
-00016230: 6e63 6c75 6465 642c 2073 6f20 7468 6520  ncluded, so the 
-00016240: 6472 792d 7275 6e20 6973 2075 7365 6675  dry-run is usefu
-00016250: 6c20 666f 7220 696e 7370 6563 7469 6e67  l for inspecting
-00016260: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
-00016270: 616c 6c20 7468 6520 7072 6f63 6573 7369  all the processi
-00016280: 6e67 2074 6861 7427 7320 6265 656e 2070  ng that's been p
-00016290: 6572 666f 726d 6564 2e0a 0a54 6f20 7375  erformed...To su
-000162a0: 7070 7265 7373 2061 6c6c 206f 7574 7075  ppress all outpu
-000162b0: 7420 6578 6365 7074 2066 6f72 2074 6865  t except for the
-000162c0: 204a 534f 4e20 6974 7365 6c66 2c20 7573   JSON itself, us
-000162d0: 6520 7468 6520 602d 2d71 7569 6574 6020  e the `--quiet` 
-000162e0: 2860 2d71 6029 2063 6f6d 6d61 6e64 206c  (`-q`) command l
-000162f0: 696e 6520 6f70 7469 6f6e 2e0a 0a54 6865  ine option...The
-00016300: 204a 534f 4e20 6472 792d 7275 6e20 6f75   JSON dry-run ou
-00016310: 7470 7574 2063 6f75 6c64 2069 7473 656c  tput could itsel
-00016320: 6620 6265 2075 7365 6420 6279 2060 7964  f be used by `yd
-00016330: 2d70 726f 7669 7369 6f6e 602c 2069 6620  -provision`, if 
-00016340: 6361 7074 7572 6564 2069 6e20 6120 6669  captured in a fi
-00016350: 6c65 2c20 652e 672e 3a0a 0a60 6060 7368  le, e.g.:..```sh
-00016360: 656c 6c0a 7964 2d70 726f 7669 7369 6f6e  ell.yd-provision
-00016370: 202d 2d64 7279 2d72 756e 202d 7120 3e20   --dry-run -q > 
-00016380: 6d79 5f77 6f72 6b65 725f 706f 6f6c 2e6a  my_worker_pool.j
-00016390: 736f 6e0a 7964 2d70 726f 7669 7369 6f6e  son.yd-provision
-000163a0: 202d 7020 6d79 5f77 6f72 6b65 725f 706f   -p my_worker_po
-000163b0: 6f6c 2e6a 736f 6e0a 6060 600a 0a23 204a  ol.json.```..# J
-000163c0: 736f 6e6e 6574 2053 7570 706f 7274 0a0a  sonnet Support..
-000163d0: 496e 2061 6c6c 2063 6972 6375 6d73 7461  In all circumsta
-000163e0: 6e63 6573 2077 6865 7265 204a 534f 4e20  nces where JSON 
-000163f0: 6669 6c65 7320 6172 6520 7573 6564 2062  files are used b
-00016400: 7920 7468 6520 5079 7468 6f6e 2045 7861  y the Python Exa
-00016410: 6d70 6c65 7320 7363 7269 7074 732c 2020  mples scripts,  
-00016420: 2a2a 5b4a 736f 6e6e 6574 5d28 6874 7470  **[Jsonnet](http
-00016430: 733a 2f2f 6a73 6f6e 6e65 742e 6f72 6729  s://jsonnet.org)
-00016440: 2a2a 2066 696c 6573 2063 616e 2062 6520  ** files can be 
-00016450: 7573 6564 2069 6e73 7465 6164 2e20 5468  used instead. Th
-00016460: 6973 2061 6c6c 6f77 7320 7468 6520 7573  is allows the us
-00016470: 6520 6f66 204a 736f 6e6e 6574 2773 2070  e of Jsonnet's p
-00016480: 6f77 6572 6675 6c20 4a53 4f4e 2065 7874  owerful JSON ext
-00016490: 656e 7369 6f6e 732c 2069 6e63 6c75 6469  ensions, includi
-000164a0: 6e67 2063 6f6d 6d65 6e74 732c 2076 6172  ng comments, var
-000164b0: 6961 626c 6573 2c20 6675 6e63 7469 6f6e  iables, function
-000164c0: 732c 2065 7463 2e0a 0a41 2073 696d 706c  s, etc...A simpl
-000164d0: 6520 7573 6167 6520 6578 616d 706c 6520  e usage example 
-000164e0: 6d69 6768 7420 6265 3a0a 0a60 6060 7368  might be:..```sh
-000164f0: 656c 6c0a 7964 2d73 7562 6d69 7420 2d2d  ell.yd-submit --
-00016500: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
-00016510: 206d 795f 776f 726b 5f72 6571 2e6a 736f   my_work_req.jso
-00016520: 6e6e 6574 0a60 6060 0a0a 5468 6520 7573  nnet.```..The us
-00016530: 6520 6f66 2074 6865 2066 696c 656e 616d  e of the filenam
-00016540: 6520 6578 7465 6e73 696f 6e20 602e 6a73  e extension `.js
-00016550: 6f6e 6e65 7460 2077 696c 6c20 696e 766f  onnet` will invo
-00016560: 6b65 204a 736f 6e6e 6574 2065 7661 6c75  ke Jsonnet evalu
-00016570: 6174 696f 6e2e 2028 4e6f 7465 2074 6861  ation. (Note tha
-00016580: 7420 6120 7465 6d70 6f72 6172 7920 4a53  t a temporary JS
-00016590: 4f4e 2066 696c 6520 6973 2063 7265 6174  ON file is creat
-000165a0: 6564 2061 7320 7061 7274 206f 6620 4a73  ed as part of Js
-000165b0: 6f6e 6e65 7420 7072 6f63 6573 7369 6e67  onnet processing
-000165c0: 2c20 7768 6963 6820 796f 7520 6d61 7920  , which you may 
-000165d0: 7365 6520 7265 6665 7272 6564 2074 6f20  see referred to 
-000165e0: 696e 2065 7272 6f72 206d 6573 7361 6765  in error message
-000165f0: 733a 2074 6869 7320 6669 6c65 2077 696c  s: this file wil
-00016600: 6c20 6861 7665 2062 6565 6e20 6465 6c65  l have been dele
-00016610: 7465 6420 6265 666f 7265 2074 6865 2073  ted before the s
-00016620: 6372 6970 7420 7374 6f70 732e 290a 0a23  cript stops.)..#
-00016630: 2320 4a73 6f6e 6e65 7420 496e 7374 616c  # Jsonnet Instal
-00016640: 6c61 7469 6f6e 0a0a 4a73 6f6e 6e65 7420  lation..Jsonnet 
-00016650: 6973 202a 2a6e 6f74 2a2a 2069 6e73 7461  is **not** insta
-00016660: 6c6c 6564 2062 7920 6465 6661 756c 7420  lled by default 
-00016670: 7768 656e 2060 7965 6c6c 6f77 646f 672d  when `yellowdog-
-00016680: 7079 7468 6f6e 2d65 7861 6d70 6c65 7360  python-examples`
-00016690: 2069 7320 696e 7374 616c 6c65 642c 2062   is installed, b
-000166a0: 6563 6175 7365 2074 6865 2070 6163 6b61  ecause the packa
-000166b0: 6765 2068 6173 2062 696e 6172 7920 636f  ge has binary co
-000166c0: 6d70 6f6e 656e 7473 2077 6869 6368 2061  mponents which a
-000166d0: 7265 206e 6f74 2061 7661 696c 6162 6c65  re not available
-000166e0: 206f 6e20 5079 5049 2066 6f72 2061 6c6c   on PyPI for all
-000166f0: 2070 6c61 7466 6f72 6d73 2e20 4966 2079   platforms. If y
-00016700: 6f75 2074 7279 2074 6f20 7573 6520 6120  ou try to use a 
-00016710: 4a73 6f6e 6e65 7420 6669 6c65 2069 6e20  Jsonnet file in 
-00016720: 7468 6520 6162 7365 6e63 6520 6f66 204a  the absence of J
-00016730: 736f 6e6e 6574 2c20 7468 6520 7363 7269  sonnet, the scri
-00016740: 7074 7320 7769 6c6c 2070 7269 6e74 2061  pts will print a
-00016750: 6e20 6572 726f 7220 6d65 7373 6167 652c  n error message,
-00016760: 2061 6e64 2073 7567 6765 7374 2061 6e20   and suggest an 
-00016770: 696e 7374 616c 6c61 7469 6f6e 206d 6563  installation mec
-00016780: 6861 6e69 736d 2e0a 0a54 6f20 696e 7374  hanism...To inst
-00016790: 616c 6c20 4a73 6f6e 6e65 7420 6174 2074  all Jsonnet at t
-000167a0: 6865 2073 616d 6520 7469 6d65 2061 7320  he same time as 
-000167b0: 696e 7374 616c 6c69 6e67 206f 7220 7570  installing or up
-000167c0: 6461 7469 6e67 2074 6865 2050 7974 686f  dating the Pytho
-000167d0: 6e20 4578 616d 706c 6573 2073 6372 6970  n Examples scrip
-000167e0: 7473 2c20 6d6f 6469 6679 2074 6865 2069  ts, modify the i
-000167f0: 6e73 7461 6c6c 6174 696f 6e20 6173 2066  nstallation as f
-00016800: 6f6c 6c6f 7773 2074 6f20 696e 636c 7564  ollows to includ
-00016810: 6520 7468 6520 606a 736f 6e6e 6574 6020  e the `jsonnet` 
-00016820: 6f70 7469 6f6e 3a0a 0a60 6060 0a70 6970  option:..```.pip
-00016830: 2069 6e73 7461 6c6c 202d 5520 2279 656c   install -U "yel
-00016840: 6c6f 7764 6f67 2d70 7974 686f 6e2d 6578  lowdog-python-ex
-00016850: 616d 706c 6573 5b6a 736f 6e6e 6574 5d22  amples[jsonnet]"
-00016860: 0a60 6060 0a0a 546f 2069 6e73 7461 6c6c  .```..To install
-00016870: 204a 736f 6e6e 6574 2073 6570 6172 6174   Jsonnet separat
-00016880: 656c 7920 6672 6f6d 2060 7965 6c6c 6f77  ely from `yellow
-00016890: 646f 672d 7079 7468 6f6e 2d65 7861 6d70  dog-python-examp
-000168a0: 6c65 7360 2c20 7472 793a 0a0a 6060 6073  les`, try:..```s
-000168b0: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
-000168c0: 202d 5520 6a73 6f6e 6e65 740a 6060 600a   -U jsonnet.```.
-000168d0: 0a49 6620 7468 6973 2066 6169 6c73 2c20  .If this fails, 
-000168e0: 7472 793a 0a0a 6060 6073 6865 6c6c 0a70  try:..```shell.p
-000168f0: 6970 2069 6e73 7461 6c6c 202d 5520 6a73  ip install -U js
-00016900: 6f6e 6e65 742d 6269 6e61 7279 0a60 6060  onnet-binary.```
-00016910: 0a0a 4966 2062 6f74 6820 6f66 2074 6865  ..If both of the
-00016920: 7365 206d 6574 686f 6473 2066 6169 6c2c  se methods fail,
-00016930: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
-00016940: 656e 7375 7265 2074 6861 7420 7468 6520  ensure that the 
-00016950: 706c 6174 666f 726d 206f 6e20 7768 6963  platform on whic
-00016960: 6820 796f 7527 7265 2072 756e 6e69 6e67  h you're running
-00016970: 2068 6173 2074 6865 2072 6571 7569 7265   has the require
-00016980: 6420 6275 696c 6420 746f 6f6c 7320 6176  d build tools av
-00016990: 6169 6c61 626c 652c 2073 6f20 7468 6174  ailable, so that
-000169a0: 2074 6865 204a 736f 6e6e 6574 2062 696e   the Jsonnet bin
-000169b0: 6172 7920 636f 6d70 6f6e 656e 7473 2063  ary components c
-000169c0: 616e 2062 6520 6275 696c 7420 6c6f 6361  an be built loca
-000169d0: 6c6c 792e 2054 6865 2072 6571 7569 7265  lly. The require
-000169e0: 6420 6275 696c 6420 7061 636b 6167 6573  d build packages
-000169f0: 2076 6172 7920 6279 2070 6c61 7466 6f72   vary by platfor
-00016a00: 6d20 6275 7420 7573 7561 6c6c 7920 696e  m but usually in
-00016a10: 636c 7564 6520 6765 6e65 7261 6c20 6465  clude general de
-00016a20: 7665 6c6f 706d 656e 7420 746f 6f6c 7320  velopment tools 
-00016a30: 696e 636c 7564 696e 6720 6120 432b 2b20  including a C++ 
-00016a40: 636f 6d70 696c 6572 2c20 616e 6420 5079  compiler, and Py
-00016a50: 7468 6f6e 2064 6576 656c 6f70 6d65 6e74  thon development
-00016a60: 2074 6f6f 6c73 2069 6e63 6c75 6469 6e67   tools including
-00016a70: 2074 6865 2050 7974 686f 6e20 6865 6164   the Python head
-00016a80: 6572 732e 0a0a 506c 6561 7365 2067 6574  ers...Please get
-00016a90: 2069 6e20 746f 7563 6820 7769 7468 2059   in touch with Y
-00016aa0: 656c 6c6f 7744 6f67 2069 6620 796f 7520  ellowDog if you 
-00016ab0: 6765 7420 7374 7563 6b2e 0a0a 2323 2056  get stuck...## V
-00016ac0: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
-00016ad0: 7469 6f6e 7320 696e 204a 736f 6e6e 6574  tions in Jsonnet
-00016ae0: 2046 696c 6573 0a0a 5468 6520 7363 7269   Files..The scri
-00016af0: 7074 7320 7072 6f76 6964 6520 6675 6c6c  pts provide full
-00016b00: 2073 7570 706f 7274 2066 6f72 2076 6172   support for var
-00016b10: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00016b20: 6f6e 7320 696e 204a 736f 6e6e 6574 2066  ons in Jsonnet f
-00016b30: 696c 6573 2c20 7573 696e 6720 7468 6520  iles, using the 
-00016b40: 7361 6d65 2072 756c 6573 2061 7320 666f  same rules as fo
-00016b50: 7220 7468 6520 4a53 4f4e 2073 7065 6369  r the JSON speci
-00016b60: 6669 6361 7469 6f6e 732e 2052 656d 656d  fications. Remem
-00016b70: 6265 7220 7468 6174 2066 6f72 202a 2a57  ber that for **W
-00016b80: 6f72 6b65 7220 506f 6f6c 2a2a 2073 7065  orker Pool** spe
-00016b90: 6369 6669 6361 7469 6f6e 732c 2076 6172  cifications, var
-00016ba0: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00016bb0: 6f6e 7320 6d75 7374 2062 6520 7072 6566  ons must be pref
-00016bc0: 6978 6564 2062 7920 605f 5f60 2c20 652e  ixed by `__`, e.
-00016bd0: 672e 2060 225f 5f7b 7b75 7365 726e 616d  g. `"__{{usernam
-00016be0: 657d 7d7d 2260 2e0a 0a56 6172 6961 626c  e}}}"`...Variabl
-00016bf0: 6520 7375 6273 7469 7475 7469 6f6e 2069  e substitution i
-00016c00: 7320 7065 7266 6f72 6d65 6420 6265 666f  s performed befo
-00016c10: 7265 204a 736f 6e6e 6574 2065 7870 616e  re Jsonnet expan
-00016c20: 7369 6f6e 2069 6e74 6f20 4a53 4f4e 2c20  sion into JSON, 
-00016c30: 616e 6420 6167 6169 6e20 6166 7465 7220  and again after 
-00016c40: 7468 6520 6578 7061 6e73 696f 6e2e 0a0a  the expansion...
-00016c50: 2323 2043 6865 636b 696e 6720 4a73 6f6e  ## Checking Json
-00016c60: 6e65 7420 5072 6f63 6573 7369 6e67 0a0a  net Processing..
-00016c70: 5468 6572 6520 6172 6520 7468 7265 6520  There are three 
-00016c80: 706f 7373 6962 696c 6974 6965 7320 666f  possibilities fo
-00016c90: 7220 7665 7269 6679 696e 6720 7468 6174  r verifying that
-00016ca0: 2061 204a 736f 6e6e 6574 2073 7065 6369   a Jsonnet speci
-00016cb0: 6669 6361 7469 6f6e 2069 7320 646f 696e  fication is doin
-00016cc0: 6720 7768 6174 2069 7320 696e 7465 6e64  g what is intend
-00016cd0: 6564 3a0a 0a31 2e20 546f 2069 6e73 7065  ed:..1. To inspe
-00016ce0: 6374 2074 6865 2062 6173 6963 2063 6f6e  ct the basic con
-00016cf0: 7665 7273 696f 6e20 6f66 204a 736f 6e6e  version of Jsonn
-00016d00: 6574 2069 6e74 6f20 4a53 4f4e 2c20 7769  et into JSON, wi
-00016d10: 7468 6f75 7420 616e 7920 6164 6469 7469  thout any additi
-00016d20: 6f6e 616c 2070 726f 6365 7373 696e 6720  onal processing 
-00016d30: 6279 2074 6865 2050 7974 686f 6e20 4578  by the Python Ex
-00016d40: 616d 706c 6573 2073 6372 6970 7473 2c20  amples scripts, 
-00016d50: 7468 6520 6079 642d 6a73 6f6e 6e65 7432  the `yd-jsonnet2
-00016d60: 6a73 6f6e 6020 636f 6d6d 616e 6420 6361  json` command ca
-00016d70: 6e20 6265 2075 7365 642e 2054 6869 7320  n be used. This 
-00016d80: 7461 6b65 7320 6120 7369 6e67 6c65 2063  takes a single c
-00016d90: 6f6d 6d61 6e64 206c 696e 6520 6172 6775  ommand line argu
-00016da0: 6d65 6e74 2077 6869 6368 2069 7320 7468  ment which is th
-00016db0: 6520 6e61 6d65 206f 6620 7468 6520 6a73  e name of the js
-00016dc0: 6f6e 6e65 7420 6669 6c65 2074 6f20 6265  onnet file to be
-00016dd0: 2070 726f 6365 7373 6564 3a0a 0a60 6060   processed:..```
-00016de0: 7368 656c 6c0a 7964 2d6a 736f 6e6e 6574  shell.yd-jsonnet
-00016df0: 326a 736f 6e20 6d79 5f66 696c 652e 6a73  2json my_file.js
-00016e00: 6f6e 6e65 740a 6060 600a 0a0a 322e 2054  onnet.```...2. T
-00016e10: 6865 2060 6a73 6f6e 6e65 742d 6472 792d  he `jsonnet-dry-
-00016e20: 7275 6e60 2028 602d 4a60 2920 6f70 7469  run` (`-J`) opti
-00016e30: 6f6e 206f 6620 7468 6520 6079 642d 7375  on of the `yd-su
-00016e40: 626d 6974 602c 2060 7964 2d70 726f 7669  bmit`, `yd-provi
-00016e50: 7369 6f6e 6020 616e 6420 6079 642d 696e  sion` and `yd-in
-00016e60: 7374 616e 7469 6174 6560 2063 6f6d 6d61  stantiate` comma
-00016e70: 6e64 7320 7769 6c6c 2067 656e 6572 6174  nds will generat
-00016e80: 6520 4a53 4f4e 206f 7574 7075 7420 7265  e JSON output re
-00016e90: 7072 6573 656e 7469 6e67 2074 6865 204a  presenting the J
-00016ea0: 736f 6e6e 6574 2074 6f20 4a53 4f4e 2070  sonnet to JSON p
-00016eb0: 726f 6365 7373 696e 6720 6f6e 6c79 2c20  rocessing only, 
-00016ec0: 696e 636c 7564 696e 6720 6170 706c 6963  including applic
-00016ed0: 6162 6c65 2076 6172 6961 626c 6520 7375  able variable su
-00016ee0: 6273 7469 7475 7469 6f6e 732c 2062 7574  bstitutions, but
-00016ef0: 2062 6566 6f72 6520 6675 6c6c 2070 726f   before full pro
-00016f00: 7065 7274 7920 6578 7061 6e73 696f 6e20  perty expansion 
-00016f10: 696e 746f 2074 6865 204a 534f 4e20 7468  into the JSON th
-00016f20: 6174 2077 696c 6c20 6265 2073 7562 6d69  at will be submi
-00016f30: 7474 6564 2074 6f20 7468 6520 506c 6174  tted to the Plat
-00016f40: 666f 726d 2e0a 0a0a 332e 2054 6865 2060  form....3. The `
-00016f50: 6472 792d 7275 6e60 2028 602d 4460 2920  dry-run` (`-D`) 
-00016f60: 6f70 7469 6f6e 2077 696c 6c20 6765 6e65  option will gene
-00016f70: 7261 7465 204a 534f 4e20 6f75 7470 7574  rate JSON output
-00016f80: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00016f90: 6520 6675 6c6c 2070 726f 6365 7373 696e  e full processin
-00016fa0: 6720 6f66 2074 6865 204a 736f 6e6e 6574  g of the Jsonnet
-00016fb0: 2066 696c 6520 696e 746f 2077 6861 7420   file into what 
-00016fc0: 7769 6c6c 2062 6520 7375 626d 6974 7465  will be submitte
-00016fd0: 6420 746f 2074 6865 2041 5049 2e20 5468  d to the API. Th
-00016fe0: 6973 2061 6c6c 6f77 7320 696e 7370 6563  is allows inspec
-00016ff0: 7469 6f6e 2074 6f20 6368 6563 6b20 7468  tion to check th
-00017000: 6174 2074 6865 206f 7574 7075 7420 6d61  at the output ma
-00017010: 7463 6865 7320 6578 7065 6374 6174 696f  tches expectatio
-00017020: 6e73 2c20 7072 696f 7220 746f 2073 7562  ns, prior to sub
-00017030: 6d69 7474 696e 6720 746f 2074 6865 2050  mitting to the P
-00017040: 6c61 7466 6f72 6d2e 0a0a 2323 204a 736f  latform...## Jso
-00017050: 6e6e 6574 2045 7861 6d70 6c65 0a0a 4865  nnet Example..He
-00017060: 7265 2773 2061 6e20 6578 616d 706c 6520  re's an example 
-00017070: 6f66 2061 204a 736f 6e6e 6574 2066 696c  of a Jsonnet fil
-00017080: 6520 7468 6174 2067 656e 6572 6174 6573  e that generates
-00017090: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
-000170a0: 656e 7420 7769 7468 2066 6f75 7220 5461  ent with four Ta
-000170b0: 736b 733a 0a0a 6060 606a 736f 6e6e 6574  sks:..```jsonnet
-000170c0: 0a23 2046 756e 6374 696f 6e20 666f 7220  .# Function for 
-000170d0: 7379 6e74 6865 7369 7369 6e67 2054 6173  synthesising Tas
-000170e0: 6b73 0a6c 6f63 616c 2054 6173 6b28 6172  ks.local Task(ar
-000170f0: 6775 6d65 6e74 733d 5b5d 2c20 656e 7669  guments=[], envi
-00017100: 726f 6e6d 656e 743d 7b7d 2920 3d20 7b0a  ronment={}) = {.
-00017110: 2020 2020 6172 6775 6d65 6e74 733a 2061      arguments: a
-00017120: 7267 756d 656e 7473 2c0a 2020 2020 656e  rguments,.    en
-00017130: 7669 726f 6e6d 656e 743a 2065 6e76 6972  vironment: envir
-00017140: 6f6e 6d65 6e74 2c0a 2020 2020 6e61 6d65  onment,.    name
-00017150: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
-00017160: 6b5f 6e75 6d62 6572 7d7d 220a 7d3b 0a0a  k_number}}".};..
-00017170: 2320 576f 726b 2052 6571 7569 7265 6d65  # Work Requireme
-00017180: 6e74 0a7b 0a20 2022 6e61 6d65 223a 2022  nt.{.  "name": "
-00017190: 776f 726b 7265 715f 7b7b 6461 7465 7469  workreq_{{dateti
-000171a0: 6d65 7d7d 222c 0a20 2022 7461 736b 4772  me}}",.  "taskGr
-000171b0: 6f75 7073 223a 205b 0a20 2020 207b 0a20  oups": [.    {. 
-000171c0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
-000171d0: 2020 2020 2020 2020 5461 736b 285b 2231          Task(["1
-000171e0: 225d 2c20 7b41 3a20 2241 5f31 227d 292c  "], {A: "A_1"}),
-000171f0: 2020 2320 6172 6775 6d65 6e74 7320 616e    # arguments an
-00017200: 6420 656e 7669 726f 6e6d 656e 740a 2020  d environment.  
-00017210: 2020 2020 2020 5461 736b 285b 2232 222c        Task(["2",
-00017220: 2022 3322 5d2c 207b 7d29 2c20 2020 2020   "3"], {}),     
-00017230: 2320 6172 6775 6d65 6e74 7320 616e 6420  # arguments and 
-00017240: 656d 7074 7920 656e 7669 726f 6e6d 656e  empty environmen
-00017250: 740a 2020 2020 2020 2020 5461 736b 285b  t.        Task([
-00017260: 2234 225d 292c 2020 2020 2020 2020 2020  "4"]),          
-00017270: 2020 2020 2320 6172 6775 6d65 6e74 7320      # arguments 
-00017280: 616e 6420 6465 6661 756c 7420 656e 7669  and default envi
-00017290: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
-000172a0: 5461 736b 2829 2020 2020 2020 2020 2020  Task()          
-000172b0: 2020 2020 2020 2020 2020 2320 6465 6661            # defa
-000172c0: 756c 7420 6172 6775 6d65 6e74 7320 616e  ult arguments an
-000172d0: 6420 656e 7669 726f 6e6d 656e 740a 2020  d environment.  
-000172e0: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
-000172f0: 7d0a 6060 600a 0a57 6865 6e20 7468 6973  }.```..When this
-00017300: 2069 7320 696e 7370 6563 7465 6420 7573   is inspected us
-00017310: 696e 6720 7468 6520 606a 736f 6e6e 6574  ing the `jsonnet
-00017320: 2d64 7279 2d72 756e 6020 6f70 7469 6f6e  -dry-run` option
-00017330: 2028 6079 642d 7375 626d 6974 202d 4a71   (`yd-submit -Jq
-00017340: 202d 7220 6d79 5f77 6f72 6b5f 7265 712e   -r my_work_req.
-00017350: 6a73 6f6e 6e65 7460 292c 2074 6869 7320  jsonnet`), this 
-00017360: 6973 2074 6865 2070 726f 6365 7373 6564  is the processed
-00017370: 206f 7574 7075 743a 0a0a 6060 606a 736f   output:..```jso
-00017380: 6e0a 7b0a 2020 226e 616d 6522 3a20 2277  n.{.  "name": "w
-00017390: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
-000173a0: 3036 3435 222c 0a20 2022 7461 736b 4772  0645",.  "taskGr
-000173b0: 6f75 7073 223a 205b 0a20 2020 207b 0a20  oups": [.    {. 
-000173c0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
-000173d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000173e0: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
-000173f0: 205b 2231 225d 2c0a 2020 2020 2020 2020   ["1"],.        
-00017400: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
-00017410: 207b 2241 223a 2022 415f 3122 7d2c 0a20   {"A": "A_1"},. 
-00017420: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00017430: 2022 6d79 5f74 6173 6b5f 7b7b 7461 736b   "my_task_{{task
-00017440: 5f6e 756d 6265 727d 7d22 0a20 2020 2020  _number}}".     
-00017450: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
-00017460: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
-00017470: 656e 7473 223a 205b 2232 222c 2022 3322  ents": ["2", "3"
-00017480: 5d2c 0a20 2020 2020 2020 2020 2022 656e  ],.          "en
-00017490: 7669 726f 6e6d 656e 7422 3a20 7b7d 2c0a  vironment": {},.
-000174a0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-000174b0: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
-000174c0: 6b5f 6e75 6d62 6572 7d7d 220a 2020 2020  k_number}}".    
-000174d0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
-000174e0: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
-000174f0: 6d65 6e74 7322 3a20 5b22 3422 5d2c 0a20  ments": ["4"],. 
-00017500: 2020 2020 2020 2020 2022 656e 7669 726f           "enviro
-00017510: 6e6d 656e 7422 3a20 7b7d 2c0a 2020 2020  nment": {},.    
-00017520: 2020 2020 2020 226e 616d 6522 3a20 226d        "name": "m
-00017530: 795f 7461 736b 5f7b 7b74 6173 6b5f 6e75  y_task_{{task_nu
-00017540: 6d62 6572 7d7d 220a 2020 2020 2020 2020  mber}}".        
-00017550: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
-00017560: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
-00017570: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
-00017580: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
-00017590: 207b 7d2c 0a20 2020 2020 2020 2020 2022   {},.          "
-000175a0: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
-000175b0: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
-000175c0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-000175d0: 205d 0a20 2020 207d 0a20 205d 0a7d 0a60   ].    }.  ].}.`
-000175e0: 6060 0a0a 5768 656e 2074 6869 7320 6973  ``..When this is
-000175f0: 2069 6e73 7065 6374 6564 2075 7369 6e67   inspected using
-00017600: 2074 6865 2060 6472 792d 7275 6e60 206f   the `dry-run` o
-00017610: 7074 696f 6e20 2860 7964 2d73 7562 6d69  ption (`yd-submi
-00017620: 7420 2d44 7120 2d72 206d 795f 776f 726b  t -Dq -r my_work
-00017630: 5f72 6571 2e6a 736f 6e6e 6574 6029 2c20  _req.jsonnet`), 
-00017640: 7468 6973 2069 7320 7468 6520 7072 6f63  this is the proc
-00017650: 6573 7365 6420 6f75 7470 7574 3a0a 0a60  essed output:..`
-00017660: 6060 6a73 6f6e 0a7b 0a20 2022 6675 6c66  ``json.{.  "fulf
-00017670: 696c 4f6e 5375 626d 6974 223a 2066 616c  ilOnSubmit": fal
-00017680: 7365 2c0a 2020 226e 616d 6522 3a20 2277  se,.  "name": "w
-00017690: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
-000176a0: 3036 3435 222c 0a20 2022 6e61 6d65 7370  0645",.  "namesp
-000176b0: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
-000176c0: 7322 2c0a 2020 2270 7269 6f72 6974 7922  s",.  "priority"
-000176d0: 3a20 302c 0a20 2022 7461 6722 3a20 2270  : 0,.  "tag": "p
-000176e0: 7965 782d 6261 7368 222c 0a20 2022 7461  yex-bash",.  "ta
-000176f0: 736b 4772 6f75 7073 223a 205b 0a20 2020  skGroups": [.   
-00017700: 207b 0a20 2020 2020 2022 6669 6e69 7368   {.      "finish
-00017710: 4966 416c 6c54 6173 6b73 4669 6e69 7368  IfAllTasksFinish
-00017720: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00017730: 2022 6669 6e69 7368 4966 416e 7954 6173   "finishIfAnyTas
-00017740: 6b46 6169 6c65 6422 3a20 6661 6c73 652c  kFailed": false,
-00017750: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
-00017760: 7461 736b 5f67 726f 7570 5f31 222c 0a20  task_group_1",. 
-00017770: 2020 2020 2022 7072 696f 7269 7479 223a       "priority":
-00017780: 2030 2c0a 2020 2020 2020 2272 756e 5370   0,.      "runSp
-00017790: 6563 6966 6963 6174 696f 6e22 3a20 7b0a  ecification": {.
-000177a0: 2020 2020 2020 2020 226d 6178 696d 756d          "maximum
-000177b0: 5461 736b 5265 7472 6965 7322 3a20 302c  TaskRetries": 0,
-000177c0: 0a20 2020 2020 2020 2022 7461 736b 5479  .        "taskTy
-000177d0: 7065 7322 3a20 5b22 6261 7368 225d 2c0a  pes": ["bash"],.
-000177e0: 2020 2020 2020 2020 2277 6f72 6b65 7254          "workerT
-000177f0: 6167 7322 3a20 5b22 7079 6578 2d62 6173  ags": ["pyex-bas
-00017800: 682d 646f 636b 6572 225d 0a20 2020 2020  h-docker"].     
-00017810: 207d 2c0a 2020 2020 2020 2274 6173 6b73   },.      "tasks
-00017820: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
-00017830: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00017840: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
-00017850: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
-00017860: 6565 705f 7363 7269 7074 2e73 6822 2c20  eep_script.sh", 
-00017870: 2231 225d 2c0a 2020 2020 2020 2020 2020  "1"],.          
-00017880: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-00017890: 2241 223a 2022 415f 3122 7d2c 0a20 2020  "A": "A_1"},.   
-000178a0: 2020 2020 2020 2022 696e 7075 7473 223a         "inputs":
-000178b0: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
-000178c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000178d0: 6f62 6a65 6374 4e61 6d65 5061 7474 6572  objectNamePatter
-000178e0: 6e22 3a20 2277 6f72 6b72 6571 5f32 3330  n": "workreq_230
-000178f0: 3131 342d 3134 3036 3435 2f73 6c65 6570  114-140645/sleep
-00017900: 5f73 6372 6970 742e 7368 222c 0a20 2020  _script.sh",.   
-00017910: 2020 2020 2020 2020 2020 2022 736f 7572             "sour
-00017920: 6365 223a 2022 5441 534b 5f4e 414d 4553  ce": "TASK_NAMES
-00017930: 5041 4345 222c 0a20 2020 2020 2020 2020  PACE",.         
-00017940: 2020 2020 2022 7665 7269 6669 6361 7469       "verificati
-00017950: 6f6e 223a 2022 5645 5249 4659 5f41 545f  on": "VERIFY_AT_
-00017960: 5354 4152 5422 0a20 2020 2020 2020 2020  START".         
-00017970: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
-00017980: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
-00017990: 6522 3a20 226d 795f 7461 736b 5f31 222c  e": "my_task_1",
-000179a0: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
-000179b0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-000179c0: 2020 2020 7b22 616c 7761 7973 5570 6c6f      {"alwaysUplo
-000179d0: 6164 223a 2074 7275 652c 2022 7265 7175  ad": true, "requ
-000179e0: 6972 6564 223a 2066 616c 7365 2c20 2273  ired": false, "s
-000179f0: 6f75 7263 6522 3a20 2250 524f 4345 5353  ource": "PROCESS
-00017a00: 5f4f 5554 5055 5422 7d0a 2020 2020 2020  _OUTPUT"}.      
-00017a10: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00017a20: 2022 7461 736b 5479 7065 223a 2022 6261   "taskType": "ba
-00017a30: 7368 220a 2020 2020 2020 2020 7d2c 0a20  sh".        },. 
-00017a40: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00017a50: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
-00017a60: 5b22 776f 726b 7265 715f 3233 3031 3134  ["workreq_230114
-00017a70: 2d31 3430 3634 352f 736c 6565 705f 7363  -140645/sleep_sc
-00017a80: 7269 7074 2e73 6822 2c20 2232 222c 2022  ript.sh", "2", "
-00017a90: 3322 5d2c 0a20 2020 2020 2020 2020 2022  3"],.          "
-00017aa0: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
-00017ab0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-00017ac0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-00017ad0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00017ae0: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
-00017af0: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
-00017b00: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
-00017b10: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
-00017b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017b30: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
-00017b40: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
-00017b50: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
-00017b60: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
-00017b70: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
-00017b80: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00017b90: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00017ba0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
-00017bb0: 6b5f 3222 2c0a 2020 2020 2020 2020 2020  k_2",.          
-00017bc0: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
-00017bd0: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
-00017be0: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
-00017bf0: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
-00017c00: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
-00017c10: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
-00017c20: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017c30: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
-00017c40: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
-00017c50: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00017c60: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00017c70: 7473 223a 205b 2277 6f72 6b72 6571 5f32  ts": ["workreq_2
-00017c80: 3330 3131 342d 3134 3036 3435 2f73 6c65  30114-140645/sle
-00017c90: 6570 5f73 6372 6970 742e 7368 222c 2022  ep_script.sh", "
-00017ca0: 3422 5d2c 0a20 2020 2020 2020 2020 2022  4"],.          "
-00017cb0: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
-00017cc0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-00017cd0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-00017ce0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00017cf0: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
-00017d00: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
-00017d10: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
-00017d20: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
-00017d30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017d40: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
-00017d50: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
-00017d60: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
-00017d70: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
-00017d80: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
-00017d90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00017da0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00017db0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
-00017dc0: 6b5f 3322 2c0a 2020 2020 2020 2020 2020  k_3",.          
-00017dd0: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
-00017de0: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
-00017df0: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
-00017e00: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
-00017e10: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
-00017e20: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
-00017e30: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017e40: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
-00017e50: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
-00017e60: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00017e70: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00017e80: 7473 223a 205b 2277 6f72 6b72 6571 5f32  ts": ["workreq_2
-00017e90: 3330 3131 342d 3134 3036 3435 2f73 6c65  30114-140645/sle
-00017ea0: 6570 5f73 6372 6970 742e 7368 225d 2c0a  ep_script.sh"],.
-00017eb0: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
-00017ec0: 6f6e 6d65 6e74 223a 207b 7d2c 0a20 2020  onment": {},.   
-00017ed0: 2020 2020 2020 2022 696e 7075 7473 223a         "inputs":
-00017ee0: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
-00017ef0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00017f00: 6f62 6a65 6374 4e61 6d65 5061 7474 6572  objectNamePatter
-00017f10: 6e22 3a20 2277 6f72 6b72 6571 5f32 3330  n": "workreq_230
-00017f20: 3131 342d 3134 3036 3435 2f73 6c65 6570  114-140645/sleep
-00017f30: 5f73 6372 6970 742e 7368 222c 0a20 2020  _script.sh",.   
-00017f40: 2020 2020 2020 2020 2020 2022 736f 7572             "sour
-00017f50: 6365 223a 2022 5441 534b 5f4e 414d 4553  ce": "TASK_NAMES
-00017f60: 5041 4345 222c 0a20 2020 2020 2020 2020  PACE",.         
-00017f70: 2020 2020 2022 7665 7269 6669 6361 7469       "verificati
-00017f80: 6f6e 223a 2022 5645 5249 4659 5f41 545f  on": "VERIFY_AT_
-00017f90: 5354 4152 5422 0a20 2020 2020 2020 2020  START".         
-00017fa0: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
-00017fb0: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
-00017fc0: 6522 3a20 226d 795f 7461 736b 5f34 222c  e": "my_task_4",
-00017fd0: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
-00017fe0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-00017ff0: 2020 2020 7b22 616c 7761 7973 5570 6c6f      {"alwaysUplo
-00018000: 6164 223a 2074 7275 652c 2022 7265 7175  ad": true, "requ
-00018010: 6972 6564 223a 2066 616c 7365 2c20 2273  ired": false, "s
-00018020: 6f75 7263 6522 3a20 2250 524f 4345 5353  ource": "PROCESS
-00018030: 5f4f 5554 5055 5422 7d0a 2020 2020 2020  _OUTPUT"}.      
-00018040: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00018050: 2022 7461 736b 5479 7065 223a 2022 6261   "taskType": "ba
-00018060: 7368 220a 2020 2020 2020 2020 7d0a 2020  sh".        }.  
-00018070: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
-00018080: 7d0a 6060 600a 0a23 2043 6f6d 6d61 6e64  }.```..# Command
-00018090: 204c 6973 740a 0a48 656c 7020 6973 2061   List..Help is a
-000180a0: 7661 696c 6162 6c65 2066 6f72 2061 6c6c  vailable for all
-000180b0: 2063 6f6d 6d61 6e64 7320 6279 2069 6e76   commands by inv
-000180c0: 6f6b 696e 6720 6120 636f 6d6d 616e 6420  oking a command 
-000180d0: 7769 7468 2074 6865 2060 2d2d 6865 6c70  with the `--help
-000180e0: 6020 6f72 2060 2d68 6020 6f70 7469 6f6e  ` or `-h` option
-000180f0: 2e20 536f 6d65 2063 6f6d 6d61 6e64 206c  . Some command l
-00018100: 696e 6520 7061 7261 6d65 7465 7273 2061  ine parameters a
-00018110: 7265 2063 6f6d 6d6f 6e20 746f 2061 6c6c  re common to all
-00018120: 2063 6f6d 6d61 6e64 732c 2077 6869 6c65   commands, while
-00018130: 206f 7468 6572 7320 6172 6520 636f 6d6d   others are comm
-00018140: 616e 642d 7370 6563 6966 6963 2e0a 0a41  and-specific...A
-00018150: 6c6c 2064 6573 7472 7563 7469 7665 2063  ll destructive c
-00018160: 6f6d 6d61 6e64 7320 7265 7175 6972 6520  ommands require 
-00018170: 7573 6572 2063 6f6e 6669 726d 6174 696f  user confirmatio
-00018180: 6e20 6265 666f 7265 2074 616b 696e 6720  n before taking 
-00018190: 6566 6665 6374 2e20 5468 6973 2063 616e  effect. This can
-000181a0: 2062 6520 7375 7070 7265 7373 6564 2075   be suppressed u
-000181b0: 7369 6e67 2074 6865 2060 2d2d 7965 7360  sing the `--yes`
-000181c0: 206f 7220 602d 7960 206f 7074 696f 6e2c   or `-y` option,
-000181d0: 2069 6e20 7768 6963 6820 6361 7365 2074   in which case t
-000181e0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
-000181f0: 7072 6f63 6565 6420 7769 7468 6f75 7420  proceed without 
-00018200: 636f 6e66 6972 6d61 7469 6f6e 2e0a 0a53  confirmation...S
-00018210: 6f6d 6520 636f 6d6d 616e 6473 2073 7570  ome commands sup
-00018220: 706f 7274 2074 6865 2060 2d2d 696e 7465  port the `--inte
-00018230: 7261 6374 6976 6560 206f 7220 602d 6960  ractive` or `-i`
-00018240: 206f 7074 696f 6e2c 2061 6c6c 6f77 696e   option, allowin
-00018250: 6720 7573 6572 2073 656c 6563 7469 6f6e  g user selection
-00018260: 7320 746f 2062 6520 6d61 6465 2e20 452e  s to be made. E.
-00018270: 672e 2c20 7468 6973 2063 616e 2062 6520  g., this can be 
-00018280: 7573 6564 2074 6f20 7365 6c65 6374 2077  used to select w
-00018290: 6869 6368 206f 626a 6563 7420 7061 7468  hich object path
-000182a0: 7320 746f 2064 656c 6574 652e 0a0a 5468  s to delete...Th
-000182b0: 6520 602d 2d71 7569 6574 6020 6f72 2060  e `--quiet` or `
-000182c0: 2d71 6020 6f70 7469 6f6e 2072 6564 7563  -q` option reduc
-000182d0: 6573 2074 6865 2063 6f6d 6d61 6e64 206f  es the command o
-000182e0: 7574 7075 7420 646f 776e 2074 6f20 6573  utput down to es
-000182f0: 7365 6e74 6961 6c20 6d65 7373 6167 6573  sential messages
-00018300: 206f 6e6c 792e 2053 6f2c 2066 6f72 2065   only. So, for e
-00018310: 7861 6d70 6c65 2c20 6079 642d 6465 6c65  xample, `yd-dele
-00018320: 7465 202d 7971 6020 776f 756c 6420 6465  te -yq` would de
-00018330: 6c65 7465 2061 6c6c 206d 6174 6368 696e  lete all matchin
-00018340: 6720 6f62 6a65 6374 2070 6174 6873 2073  g object paths s
-00018350: 696c 656e 746c 792e 0a0a 4966 2079 6f75  ilently...If you
-00018360: 2065 6e63 6f75 6e74 6572 2061 6e20 6572   encounter an er
-00018370: 726f 7220 6974 2063 616e 2062 6520 7573  ror it can be us
-00018380: 6566 756c 2066 6f72 2073 7570 706f 7274  eful for support
-00018390: 2070 7572 706f 7365 7320 746f 2073 6565   purposes to see
-000183a0: 2074 6865 2066 756c 6c20 5079 7468 6f6e   the full Python
-000183b0: 2073 7461 636b 2074 7261 6365 2e20 5468   stack trace. Th
-000183c0: 6973 2063 616e 2062 6520 656e 6162 6c65  is can be enable
-000183d0: 6420 6279 2072 756e 6e69 6e67 2074 6865  d by running the
-000183e0: 2063 6f6d 6d61 6e64 2075 7369 6e67 2074   command using t
-000183f0: 6865 2060 2d2d 6465 6275 6760 206f 7074  he `--debug` opt
-00018400: 696f 6e2e 0a0a 2323 2079 642d 7375 626d  ion...## yd-subm
-00018410: 6974 0a0a 5468 6520 6079 642d 7375 626d  it..The `yd-subm
-00018420: 6974 6020 636f 6d6d 616e 6420 7375 626d  it` command subm
-00018430: 6974 7320 6120 6e65 7720 576f 726b 2052  its a new Work R
-00018440: 6571 7569 7265 6d65 6e74 2c20 6163 636f  equirement, acco
-00018450: 7264 696e 6720 746f 2074 6865 2057 6f72  rding to the Wor
-00018460: 6b20 5265 7175 6972 656d 656e 7420 6465  k Requirement de
-00018470: 6669 6e69 7469 6f6e 2066 6f75 6e64 2069  finition found i
-00018480: 6e20 7468 6520 6077 6f72 6b52 6571 7569  n the `workRequi
-00018490: 7265 6d65 6e74 6020 7365 6374 696f 6e20  rement` section 
-000184a0: 6f66 2074 6865 2054 4f4d 4c20 636f 6e66  of the TOML conf
-000184b0: 6967 7572 6174 696f 6e20 6669 6c65 2061  iguration file a
-000184c0: 6e64 2f6f 7220 7468 6520 7370 6563 6966  nd/or the specif
-000184d0: 6963 6174 696f 6e20 666f 756e 6420 696e  ication found in
-000184e0: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
-000184f0: 656e 7420 4a53 4f4e 2064 6f63 756d 656e  ent JSON documen
-00018500: 7420 7375 7070 6c69 6564 2075 7369 6e67  t supplied using
-00018510: 2074 6865 2060 2d2d 776f 726b 2d72 6571   the `--work-req
-00018520: 7569 7265 6d65 6e74 6020 6f70 7469 6f6e  uirement` option
-00018530: 2e0a 0a55 7365 2074 6865 2060 2d2d 6472  ...Use the `--dr
-00018540: 792d 7275 6e60 206f 7074 696f 6e20 746f  y-run` option to
-00018550: 2069 6e73 7065 6374 2074 6865 2064 6574   inspect the det
-00018560: 6169 6c73 206f 6620 7468 6520 576f 726b  ails of the Work
-00018570: 2052 6571 7569 7265 6d65 6e74 2c20 5461   Requirement, Ta
-00018580: 736b 2047 726f 7570 732c 2061 6e64 2054  sk Groups, and T
-00018590: 6173 6b73 2074 6861 7420 7769 6c6c 2062  asks that will b
-000185a0: 6520 7375 626d 6974 7465 642c 2069 6e20  e submitted, in 
-000185b0: 4a53 4f4e 2066 6f72 6d61 742e 0a0a 4f6e  JSON format...On
-000185c0: 6365 2073 7562 6d69 7474 6564 2c20 7468  ce submitted, th
-000185d0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-000185e0: 6e74 2077 696c 6c20 6170 7065 6172 2069  nt will appear i
-000185f0: 6e20 7468 6520 2a2a 576f 726b 2a2a 2074  n the **Work** t
-00018600: 6162 2069 6e20 7468 6520 5965 6c6c 6f77  ab in the Yellow
-00018610: 446f 6720 506f 7274 616c 2e0a 0a54 6865  Dog Portal...The
-00018620: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00018630: 7427 7320 7072 6f67 7265 7373 2063 616e  t's progress can
-00018640: 2062 6520 7472 6163 6b65 6420 746f 2063   be tracked to c
-00018650: 6f6d 706c 6574 696f 6e20 6279 2075 7369  ompletion by usi
-00018660: 6e67 2074 6865 2060 2d2d 666f 6c6c 6f77  ng the `--follow
-00018670: 6020 286f 7220 602d 6660 2920 6f70 7469  ` (or `-f`) opti
-00018680: 6f6e 2077 6865 6e20 696e 766f 6b69 6e67  on when invoking
-00018690: 2060 7964 2d73 7562 6d69 7460 3a20 7468   `yd-submit`: th
-000186a0: 6520 636f 6d6d 616e 6420 7769 6c6c 2072  e command will r
-000186b0: 6570 6f72 7420 6f6e 2054 6173 6b73 2061  eport on Tasks a
-000186c0: 7320 7468 6579 2063 6f6e 636c 7564 6520  s they conclude 
-000186d0: 616e 6420 776f 6e27 7420 7265 7475 726e  and won't return
-000186e0: 2075 6e74 696c 2074 6865 2057 6f72 6b20   until the Work 
-000186f0: 5265 7175 6972 656d 656e 7420 6861 7320  Requirement has 
-00018700: 6669 6e69 7368 6564 2e0a 0a23 2320 7964  finished...## yd
-00018710: 2d70 726f 7669 7369 6f6e 0a0a 5468 6520  -provision..The 
-00018720: 6079 642d 7072 6f76 6973 696f 6e60 2063  `yd-provision` c
-00018730: 6f6d 6d61 6e64 2070 726f 7669 7369 6f6e  ommand provision
-00018740: 7320 6120 6e65 7720 576f 726b 6572 2050  s a new Worker P
-00018750: 6f6f 6c20 6163 636f 7264 696e 6720 746f  ool according to
-00018760: 2074 6865 2073 7065 6369 6669 6361 7469   the specificati
-00018770: 6f6e 7320 696e 2074 6865 2060 776f 726b  ons in the `work
-00018780: 6572 506f 6f6c 6020 7365 6374 696f 6e20  erPool` section 
-00018790: 6f66 2074 6865 2054 4f4d 4c20 636f 6e66  of the TOML conf
-000187a0: 6967 7572 6174 696f 6e20 6669 6c65 2061  iguration file a
-000187b0: 6e64 2f6f 7220 696e 2074 6865 2073 7065  nd/or in the spe
-000187c0: 6369 6669 6361 7469 6f6e 2066 6f75 6e64  cification found
-000187d0: 2069 6e20 6120 576f 726b 6572 2050 6f6f   in a Worker Poo
-000187e0: 6c20 4a53 4f4e 2064 6f63 756d 656e 7420  l JSON document 
-000187f0: 7375 7070 6c69 6564 2075 7369 6e67 2074  supplied using t
-00018800: 6865 2060 2d2d 776f 726b 6572 2d70 6f6f  he `--worker-poo
-00018810: 6c60 206f 7074 696f 6e2e 0a0a 5573 6520  l` option...Use 
-00018820: 7468 6520 602d 2d64 7279 2d72 756e 6020  the `--dry-run` 
-00018830: 6f70 7469 6f6e 2074 6f20 696e 7370 6563  option to inspec
-00018840: 7420 7468 6520 6465 7461 696c 7320 6f66  t the details of
-00018850: 2074 6865 2057 6f72 6b65 7220 506f 6f6c   the Worker Pool
-00018860: 2073 7065 6369 6669 6361 7469 6f6e 2074   specification t
-00018870: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
-00018880: 6974 7465 642c 2069 6e20 4a53 4f4e 2066  itted, in JSON f
-00018890: 6f72 6d61 742e 0a0a 4f6e 6365 2070 726f  ormat...Once pro
-000188a0: 7669 7369 6f6e 6564 2c20 7468 6520 576f  visioned, the Wo
-000188b0: 726b 6572 2050 6f6f 6c20 7769 6c6c 2061  rker Pool will a
-000188c0: 7070 6561 7220 696e 2074 6865 202a 2a57  ppear in the **W
-000188d0: 6f72 6b65 7273 2a2a 2074 6162 2069 6e20  orkers** tab in 
-000188e0: 7468 6520 5965 6c6c 6f77 446f 6720 506f  the YellowDog Po
-000188f0: 7274 616c 2c20 616e 6420 6974 7320 6173  rtal, and its as
-00018900: 736f 6369 6174 6564 2043 6f6d 7075 7465  sociated Compute
-00018910: 2052 6571 7569 7265 6d65 6e74 2077 696c   Requirement wil
-00018920: 6c20 6170 7065 6172 2069 6e20 7468 6520  l appear in the 
-00018930: 2a2a 436f 6d70 7574 652a 2a20 7461 622e  **Compute** tab.
-00018940: 0a0a 2323 2079 642d 6361 6e63 656c 0a0a  ..## yd-cancel..
-00018950: 5468 6520 6079 642d 6361 6e63 656c 6020  The `yd-cancel` 
-00018960: 636f 6d6d 616e 6420 6361 6e63 656c 7320  command cancels 
-00018970: 616e 7920 6163 7469 7665 2057 6f72 6b20  any active Work 
-00018980: 5265 7175 6972 656d 656e 7473 2c20 696e  Requirements, in
-00018990: 636c 7564 696e 6720 616e 7920 7065 6e64  cluding any pend
-000189a0: 696e 6720 5461 736b 2047 726f 7570 7320  ing Task Groups 
-000189b0: 616e 6420 7468 6520 5461 736b 7320 7468  and the Tasks th
-000189c0: 6579 2063 6f6e 7461 696e 2e20 0a0a 5468  ey contain. ..Th
-000189d0: 6520 606e 616d 6573 7061 6365 6020 616e  e `namespace` an
-000189e0: 6420 6074 6167 6020 7661 6c75 6573 2069  d `tag` values i
-000189f0: 6e20 7468 6520 6063 6f6e 6669 672e 746f  n the `config.to
-00018a00: 6d6c 6020 6669 6c65 2061 7265 2075 7365  ml` file are use
-00018a10: 6420 746f 2069 6465 6e74 6966 7920 7768  d to identify wh
-00018a20: 6963 6820 576f 726b 2052 6571 7569 7265  ich Work Require
-00018a30: 6d65 6e74 7320 746f 2063 616e 6365 6c2e  ments to cancel.
-00018a40: 0a0a 4279 2064 6566 6175 6c74 2c20 616e  ..By default, an
-00018a50: 7920 5461 736b 7320 7468 6174 2061 7265  y Tasks that are
-00018a60: 2063 7572 7265 6e74 6c79 2072 756e 6e69   currently runni
-00018a70: 6e67 206f 6e20 576f 726b 6572 7320 7769  ng on Workers wi
-00018a80: 6c6c 2063 6f6e 7469 6e75 6520 746f 2072  ll continue to r
-00018a90: 756e 2074 6f20 636f 6d70 6c65 7469 6f6e  un to completion
-00018aa0: 206f 7220 756e 7469 6c20 7468 6579 2066   or until they f
-00018ab0: 6169 6c2e 2054 6173 6b73 2063 616e 2062  ail. Tasks can b
-00018ac0: 6520 696e 7374 7275 6374 6564 2074 6f20  e instructed to 
-00018ad0: 6162 6f72 7420 696d 6d65 6469 6174 656c  abort immediatel
-00018ae0: 7920 6279 2073 7570 706c 7969 6e67 2074  y by supplying t
-00018af0: 6865 2060 2d2d 6162 6f72 7460 206f 7220  he `--abort` or 
-00018b00: 602d 6160 206f 7074 696f 6e20 746f 2060  `-a` option to `
-00018b10: 7964 2d63 616e 6365 6c60 2e0a 0a23 2320  yd-cancel`...## 
-00018b20: 7964 2d61 626f 7274 0a0a 5468 6520 6079  yd-abort..The `y
-00018b30: 642d 6162 6f72 7460 2063 6f6d 6d61 6e64  d-abort` command
-00018b40: 2069 7320 7573 6564 2074 6f20 6162 6f72   is used to abor
-00018b50: 7420 5461 736b 7320 7468 6174 2061 7265  t Tasks that are
-00018b60: 2063 7572 7265 6e74 6c79 2072 756e 6e69   currently runni
-00018b70: 6e67 2e20 5468 6520 7573 6572 2069 6e74  ng. The user int
-00018b80: 6572 6163 7469 7665 6c79 2073 656c 6563  eractively selec
-00018b90: 7473 2074 6865 2057 6f72 6b20 5265 7175  ts the Work Requ
-00018ba0: 6972 656d 656e 7473 2074 6f20 7461 7267  irements to targ
-00018bb0: 6574 2c20 616e 6420 7468 656e 2077 6869  et, and then whi
-00018bc0: 6368 2054 6173 6b73 2077 6974 6869 6e20  ch Tasks within 
-00018bd0: 7468 6f73 6520 576f 726b 2052 6571 7569  those Work Requi
-00018be0: 7265 6d65 6e74 7320 746f 2061 626f 7274  rements to abort
-00018bf0: 2e20 5468 6520 576f 726b 2052 6571 7569  . The Work Requi
-00018c00: 7265 6d65 6e74 7320 6172 6520 6e6f 7420  rements are not 
-00018c10: 6361 6e63 656c 6c65 6420 6173 2070 6172  cancelled as par
-00018c20: 7420 6f66 2074 6869 7320 7072 6f63 6573  t of this proces
-00018c30: 732e 0a0a 5468 6520 606e 616d 6573 7061  s...The `namespa
-00018c40: 6365 6020 616e 6420 6074 6167 6020 7661  ce` and `tag` va
-00018c50: 6c75 6573 2069 6e20 7468 6520 6063 6f6e  lues in the `con
-00018c60: 6669 672e 746f 6d6c 6020 6669 6c65 2061  fig.toml` file a
-00018c70: 7265 2075 7365 6420 746f 2069 6465 6e74  re used to ident
-00018c80: 6966 7920 7768 6963 6820 576f 726b 2052  ify which Work R
-00018c90: 6571 7569 7265 6d65 6e74 7320 746f 206c  equirements to l
-00018ca0: 6973 7420 666f 7220 7365 6c65 6374 696f  ist for selectio
-00018cb0: 6e2e 0a0a 2323 2079 642d 646f 776e 6c6f  n...## yd-downlo
-00018cc0: 6164 0a0a 5468 6520 6079 642d 646f 776e  ad..The `yd-down
-00018cd0: 6c6f 6164 6020 636f 6d6d 616e 6420 646f  load` command do
-00018ce0: 776e 6c6f 6164 7320 616e 7920 6f62 6a65  wnloads any obje
-00018cf0: 6374 7320 6372 6561 7465 6420 696e 2074  cts created in t
-00018d00: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
-00018d10: 6563 7420 5374 6f72 652e 0a0a 5468 6520  ect Store...The 
-00018d20: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
-00018d30: 6074 6167 6020 7661 6c75 6573 2061 7265  `tag` values are
-00018d40: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
-00018d50: 6e65 2077 6869 6368 206f 626a 6563 7473  ne which objects
-00018d60: 2074 6f20 646f 776e 6c6f 6164 2e20 4f62   to download. Ob
-00018d70: 6a65 6374 7320 7769 6c6c 2062 6520 646f  jects will be do
-00018d80: 776e 6c6f 6164 6564 2074 6f20 6120 6469  wnloaded to a di
-00018d90: 7265 6374 6f72 7920 7769 7468 2074 6865  rectory with the
-00018da0: 2073 616d 6520 6e61 6d65 2061 7320 606e   same name as `n
-00018db0: 616d 6573 7061 6365 602e 2049 6620 6120  amespace`. If a 
-00018dc0: 6469 7265 6374 6f72 7920 616c 7265 6164  directory alread
-00018dd0: 7920 6578 6973 7473 2c20 6120 6e65 7720  y exists, a new 
-00018de0: 6469 7265 6374 6f72 7920 7769 7468 206e  directory with n
-00018df0: 616d 6520 603c 6e61 6d65 7370 6163 653e  ame `<namespace>
-00018e00: 2e30 3160 2028 6574 632e 2920 7769 6c6c  .01` (etc.) will
-00018e10: 2062 6520 6372 6561 7465 642e 0a0a 2323   be created...##
-00018e20: 2079 642d 6465 6c65 7465 0a0a 5468 6520   yd-delete..The 
-00018e30: 6079 642d 6465 6c65 7465 6020 636f 6d6d  `yd-delete` comm
-00018e40: 616e 6420 6465 6c65 7465 7320 616e 7920  and deletes any 
-00018e50: 6f62 6a65 6374 7320 6372 6561 7465 6420  objects created 
-00018e60: 696e 2074 6865 2059 656c 6c6f 7744 6f67  in the YellowDog
-00018e70: 204f 626a 6563 7420 5374 6f72 652e 0a0a   Object Store...
-00018e80: 5468 6520 606e 616d 6573 7061 6365 6020  The `namespace` 
-00018e90: 616e 6420 6074 6167 6020 7661 6c75 6573  and `tag` values
-00018ea0: 2069 6e20 7468 6520 6063 6f6e 6669 672e   in the `config.
-00018eb0: 746f 6d6c 6020 6669 6c65 2061 7265 2075  toml` file are u
-00018ec0: 7365 6420 746f 2069 6465 6e74 6966 7920  sed to identify 
-00018ed0: 7768 6963 6820 6f62 6a65 6374 7320 746f  which objects to
-00018ee0: 2064 656c 6574 652e 204e 6f74 6520 7468   delete. Note th
-00018ef0: 6174 2069 7427 7320 6561 7379 2074 6f20  at it's easy to 
-00018f00: 7573 6520 6079 642d 6465 6c65 7465 6020  use `yd-delete` 
-00018f10: 746f 2063 6c65 6172 2074 6865 2063 6f6e  to clear the con
-00018f20: 7465 6e74 7320 6f66 2061 206e 616d 6573  tents of a names
-00018f30: 7061 6365 2062 7920 7573 696e 6720 616e  pace by using an
-00018f40: 2065 6d70 7479 2060 7461 6760 2c20 6173   empty `tag`, as
-00018f50: 2066 6f6c 6c6f 7773 3a0a 0a60 6060 7368   follows:..```sh
-00018f60: 656c 6c0a 7964 2d64 656c 6574 6520 2d74  ell.yd-delete -t
-00018f70: 2022 220a 6060 600a 0a54 6869 7320 6361   "".```..This ca
-00018f80: 6e20 6265 2065 7874 656e 6465 6420 746f  n be extended to
-00018f90: 2061 6e79 206f 7468 6572 206e 616d 6573   any other names
-00018fa0: 7061 6365 2062 7920 7573 696e 6720 7468  pace by using th
-00018fb0: 6520 602d 2d6e 616d 6573 7061 6365 602f  e `--namespace`/
-00018fc0: 602d 6e60 206f 7074 696f 6e2e 0a0a 2323  `-n` option...##
-00018fd0: 2079 642d 7570 6c6f 6164 0a0a 5468 6520   yd-upload..The 
-00018fe0: 6079 642d 7570 6c6f 6164 6020 636f 6d6d  `yd-upload` comm
-00018ff0: 616e 6420 7570 6c6f 6164 7320 6669 6c65  and uploads file
-00019000: 7320 6672 6f6d 2074 6865 206c 6f63 616c  s from the local
-00019010: 2066 696c 6573 7973 7465 6d20 746f 2074   filesystem to t
-00019020: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
-00019030: 6563 7420 7374 6f72 652e 2046 696c 6573  ect store. Files
-00019040: 2061 7265 2070 6c61 6365 6420 696e 2074   are placed in t
-00019050: 6865 2063 6f6e 6669 6775 7265 6420 606e  he configured `n
-00019060: 616d 6573 7061 6365 6020 7769 7468 696e  amespace` within
-00019070: 2061 2064 6972 6563 746f 7279 2073 7570   a directory sup
-00019080: 706c 6965 6420 7573 696e 6720 7468 6520  plied using the 
-00019090: 2872 6571 7569 7265 6429 2060 2d2d 6469  (required) `--di
-000190a0: 7265 6374 6f72 7960 206f 7074 696f 6e2c  rectory` option,
-000190b0: 2065 2e67 2e3a 0a0a 6060 6073 6865 6c6c   e.g.:..```shell
-000190c0: 0a79 642d 7570 6c6f 6164 202d 2d64 6972  .yd-upload --dir
-000190d0: 6563 746f 7279 206d 795f 776f 726b 5f72  ectory my_work_r
-000190e0: 6571 7569 7265 6d65 6e74 2066 696c 655f  equirement file_
-000190f0: 3120 6669 6c65 5f32 206d 6f72 6566 696c  1 file_2 morefil
-00019100: 6573 2f66 696c 6533 0a60 6060 0a54 6f20  es/file3.```.To 
-00019110: 7375 7070 7265 7373 2074 6865 206d 6972  suppress the mir
-00019120: 726f 7269 6e67 206f 6620 7468 6520 6c6f  roring of the lo
-00019130: 6361 6c20 6469 7265 6374 6f72 7920 7374  cal directory st
-00019140: 7275 6374 7572 6520 7769 7468 696e 2074  ructure within t
-00019150: 6865 206f 626a 6563 7420 7374 6f72 652c  he object store,
-00019160: 2075 7365 2074 6865 2060 2d2d 666c 6174   use the `--flat
-00019170: 7465 6e2d 7570 6c6f 6164 2d70 6174 6873  ten-upload-paths
-00019180: 6020 6f72 2060 2d66 6020 6f70 7469 6f6e  ` or `-f` option
-00019190: 2e20 4e6f 7465 2074 6861 7420 6966 2074  . Note that if t
-000191a0: 6869 7320 6372 6561 7465 7320 6d75 6c74  his creates mult
-000191b0: 6970 6c65 2075 706c 6f61 6465 6420 6669  iple uploaded fi
-000191c0: 6c65 7320 7769 7468 2074 6865 2073 616d  les with the sam
-000191d0: 6520 7061 7468 2069 6e20 7468 6520 4f62  e path in the Ob
-000191e0: 6a65 6374 2053 746f 7265 2066 6f6c 6465  ject Store folde
-000191f0: 722c 2066 696c 6573 2077 696c 6c20 6265  r, files will be
-00019200: 206f 7665 7277 7269 7474 656e 2e0a 0a46   overwritten...F
-00019210: 696c 6573 2069 6e20 6469 7265 6374 6f72  iles in director
-00019220: 6965 7320 6d61 7920 6265 2072 6563 7572  ies may be recur
-00019230: 7369 7665 6c79 2075 706c 6f61 6465 6420  sively uploaded 
-00019240: 7573 696e 6720 7468 6520 602d 2d72 6563  using the `--rec
-00019250: 7572 7369 7665 6020 6f72 2060 2d72 6020  ursive` or `-r` 
-00019260: 6f70 7469 6f6e 2c20 652e 672e 3a0a 0a60  option, e.g.:..`
-00019270: 6060 7368 656c 6c0a 7964 2d75 706c 6f61  ``shell.yd-uploa
-00019280: 6420 2d2d 6469 7265 6374 6f72 7920 6d79  d --directory my
-00019290: 5f77 6f72 6b5f 7265 7175 6972 656d 656e  _work_requiremen
-000192a0: 7420 2d72 206d 7964 6972 206d 796f 7468  t -r mydir myoth
-000192b0: 6572 6469 720a 6060 600a 0a54 6f20 7570  erdir.```..To up
-000192c0: 6c6f 6164 2074 6f20 6f74 6865 7220 6e61  load to other na
-000192d0: 6d65 7370 6163 6573 2c20 7573 6520 7468  mespaces, use th
-000192e0: 6520 602d 2d6e 616d 6573 7061 6365 602f  e `--namespace`/
-000192f0: 602d 6e60 206f 7074 696f 6e2e 0a0a 2323  `-n` option...##
-00019300: 2079 642d 7368 7574 646f 776e 0a0a 5468   yd-shutdown..Th
-00019310: 6520 6079 642d 7368 7574 646f 776e 6020  e `yd-shutdown` 
-00019320: 636f 6d6d 616e 6420 7368 7574 7320 646f  command shuts do
-00019330: 776e 2057 6f72 6b65 7220 506f 6f6c 7320  wn Worker Pools 
-00019340: 7468 6174 206d 6174 6368 2074 6865 2060  that match the `
-00019350: 6e61 6d65 7370 6163 6560 2061 6e64 2060  namespace` and `
-00019360: 7461 6760 2066 6f75 6e64 2069 6e20 7468  tag` found in th
-00019370: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00019380: 6669 6c65 2e20 416c 6c20 7265 6d61 696e  file. All remain
-00019390: 696e 6720 776f 726b 2077 696c 6c20 6265  ing work will be
-000193a0: 2063 616e 6365 6c6c 6564 2c20 6275 7420   cancelled, but 
-000193b0: 6375 7272 656e 746c 7920 6578 6563 7574  currently execut
-000193c0: 696e 6720 5461 736b 7320 7769 6c6c 2062  ing Tasks will b
-000193d0: 6520 616c 6c6f 7765 6420 746f 2063 6f6d  e allowed to com
-000193e0: 706c 6574 652c 2061 6674 6572 2077 6869  plete, after whi
-000193f0: 6368 2074 6865 2043 6f6d 7075 7465 2052  ch the Compute R
-00019400: 6571 7569 7265 6d65 6e74 2077 696c 6c20  equirement will 
-00019410: 6265 2074 6572 6d69 6e61 7465 642e 0a0a  be terminated...
-00019420: 2323 2079 642d 696e 7374 616e 7469 6174  ## yd-instantiat
-00019430: 650a 0a54 6865 2060 7964 2d69 6e73 7461  e..The `yd-insta
-00019440: 6e74 6961 7465 6020 636f 6d6d 616e 6420  ntiate` command 
-00019450: 696e 7374 616e 7469 6174 6573 2061 2043  instantiates a C
-00019460: 6f6d 7075 7465 2052 6571 7569 7265 6d65  ompute Requireme
-00019470: 6e74 2028 692e 652e 2c20 6120 7365 7420  nt (i.e., a set 
-00019480: 6f66 2069 6e73 7461 6e63 6573 2074 6861  of instances tha
-00019490: 7420 6172 6520 6d61 6e61 6765 6420 6279  t are managed by
-000194a0: 2074 6865 6972 2063 7265 6174 6f72 2061   their creator a
-000194b0: 6e64 2064 6f20 6e6f 7420 6175 746f 6d61  nd do not automa
-000194c0: 7469 6361 6c6c 7920 6265 636f 6d65 2070  tically become p
-000194d0: 6172 7420 6f66 2061 2059 656c 6c6f 7744  art of a YellowD
-000194e0: 6f67 2057 6f72 6b65 7220 506f 6f6c 292e  og Worker Pool).
-000194f0: 0a0a 5468 6973 2063 6f6d 6d61 6e64 2075  ..This command u
-00019500: 7365 7320 7468 6520 6461 7461 2066 726f  ses the data fro
-00019510: 6d20 7468 6520 6077 6f72 6b65 7250 6f6f  m the `workerPoo
-00019520: 6c60 2063 6f6e 6669 6775 7261 7469 6f6e  l` configuration
-00019530: 2073 6563 7469 6f6e 2c20 6275 7420 6f6e   section, but on
-00019540: 6c79 2075 7365 7320 7468 6520 606e 616d  ly uses the `nam
-00019550: 6560 2c20 6074 656d 706c 6174 6549 6460  e`, `templateId`
-00019560: 2c20 6074 6172 6765 7449 6e73 7461 6e63  , `targetInstanc
-00019570: 6543 6f75 6e74 602c 2060 696e 7374 616e  eCount`, `instan
-00019580: 6365 5461 6773 602c 2060 7573 6572 4461  ceTags`, `userDa
-00019590: 7461 602c 2061 6e64 2060 696d 6167 6573  ta`, and `images
-000195a0: 4964 6020 7072 6f70 6572 7469 6573 2e20  Id` properties. 
-000195b0: 496e 2061 6464 6974 696f 6e2c 2074 6865  In addition, the
-000195c0: 2042 6f6f 6c65 616e 2070 726f 7065 7274   Boolean propert
-000195d0: 7920 606d 6169 6e74 6169 6e49 6e73 7461  y `maintainInsta
-000195e0: 6e63 6543 6f75 6e74 6020 2864 6566 6175  nceCount` (defau
-000195f0: 6c74 203d 2060 6661 6c73 6560 2920 6973  lt = `false`) is
-00019600: 2061 7661 696c 6162 6c65 2066 6f72 2075   available for u
-00019610: 7365 2077 6974 6820 6079 642d 696e 7374  se with `yd-inst
-00019620: 616e 7469 6174 6560 2e0a 0a43 6f6d 7075  antiate`...Compu
-00019630: 7465 2052 6571 7569 7265 6d65 6e74 7320  te Requirements 
-00019640: 6361 6e20 6265 2069 6e73 7461 6e74 6961  can be instantia
-00019650: 7465 6420 6469 7265 6374 6c79 2066 726f  ted directly fro
-00019660: 6d20 4a53 4f4e 2028 6f72 204a 736f 6e6e  m JSON (or Jsonn
-00019670: 6574 2920 7370 6563 6966 6963 6174 696f  et) specificatio
-00019680: 6e73 2c20 7573 696e 6720 7468 6520 602d  ns, using the `-
-00019690: 2d63 6f6d 7075 7465 2d72 6571 7569 7265  -compute-require
-000196a0: 6d65 6e74 6020 286f 7220 602d 4360 2920  ment` (or `-C`) 
-000196b0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-000196c0: 696f 6e2c 2066 6f6c 6c6f 7765 6420 6279  ion, followed by
-000196d0: 2074 6865 2066 696c 656e 616d 652e 2054   the filename. T
-000196e0: 6865 2070 726f 7065 7274 6965 7320 6c69  he properties li
-000196f0: 7374 6564 2061 626f 7665 2077 696c 6c20  sted above will 
-00019700: 6265 2069 6e68 6572 6974 6564 2066 726f  be inherited fro
-00019710: 6d20 7468 6520 636f 6e66 6967 2e74 6f6d  m the config.tom
-00019720: 6c20 6077 6f72 6b65 7250 6f6f 6c60 2073  l `workerPool` s
-00019730: 7065 6369 6669 6361 7469 6f6e 2069 6620  pecification if 
-00019740: 7468 6579 2061 7265 206e 6f74 2070 7265  they are not pre
-00019750: 7365 6e74 2069 6e20 7468 6520 4a53 4f4e  sent in the JSON
-00019760: 2066 696c 652e 2041 6e20 6578 616d 706c   file. An exampl
-00019770: 6520 4a53 4f4e 2073 7065 6369 6669 6361  e JSON specifica
-00019780: 7469 6f6e 2069 7320 7368 6f77 6e20 6265  tion is shown be
-00019790: 6c6f 773a 0a0a 6060 606a 736f 6e0a 7b0a  low:..```json.{.
-000197a0: 2020 2269 6d61 6765 7349 6422 3a20 2279    "imagesId": "y
-000197b0: 6469 643a 696d 6766 616d 3a30 3030 3030  did:imgfam:00000
-000197c0: 303a 3431 3936 3235 3932 2d35 3737 632d  0:41962592-577c-
-000197d0: 3466 6465 2d61 6230 332d 6438 3532 3436  4fde-ab03-d85246
-000197e0: 3565 3766 3862 222c 0a20 2022 696e 7374  5e7f8b",.  "inst
-000197f0: 616e 6365 5461 6773 223a 207b 2261 3122  anceTags": {"a1"
-00019800: 3a20 226f 6e65 222c 2022 6132 223a 2022  : "one", "a2": "
-00019810: 7477 6f22 7d2c 0a20 2022 7265 7175 6972  two"},.  "requir
-00019820: 656d 656e 744e 616d 6522 3a20 2263 725f  ementName": "cr_
-00019830: 7465 7374 5f7b 7b64 6174 6574 696d 657d  test_{{datetime}
-00019840: 7d22 2c0a 2020 2272 6571 7569 7265 6d65  }",.  "requireme
-00019850: 6e74 4e61 6d65 7370 6163 6522 3a20 2270  ntNamespace": "p
-00019860: 7965 7861 6d70 6c65 7322 2c0a 2020 2272  yexamples",.  "r
-00019870: 6571 7569 7265 6d65 6e74 5461 6722 3a20  equirementTag": 
-00019880: 2270 7965 7861 6d70 6c65 732d 7465 7374  "pyexamples-test
-00019890: 222c 0a20 2022 7465 6d70 6c61 7465 4964  ",.  "templateId
-000198a0: 223a 2022 7964 6964 3a63 7274 3a30 3030  ": "ydid:crt:000
-000198b0: 3030 303a 3233 3065 3961 3432 2d39 3764  000:230e9a42-97d
-000198c0: 622d 3464 3639 2d61 6139 312d 3239 6666  b-4d69-aa91-29ff
-000198d0: 3330 3939 3531 6234 222c 0a20 2022 7573  309951b4",.  "us
-000198e0: 6572 4461 7461 223a 2022 232f 6269 6e2f  erData": "#/bin/
-000198f0: 6261 7368 5c6e 234f 7468 6572 2073 7475  bash\n#Other stu
-00019900: 6666 2e2e 2e22 2c0a 2020 2274 6172 6765  ff...",.  "targe
-00019910: 7449 6e73 7461 6e63 6543 6f75 6e74 223a  tInstanceCount":
-00019920: 2031 2c0a 2020 226d 6169 6e74 6169 6e49   1,.  "maintainI
-00019930: 6e73 7461 6e63 6543 6f75 6e74 223a 2074  nstanceCount": t
-00019940: 7275 650a 7d0a 6060 600a 0a49 6620 6120  rue.}.```..If a 
-00019950: 576f 726b 6572 2050 6f6f 6c20 6973 2064  Worker Pool is d
-00019960: 6566 696e 6564 2c20 7573 696e 6720 6077  efined, using `w
-00019970: 6f72 6b65 7250 6f6f 6c44 6174 6160 2069  orkerPoolData` i
-00019980: 6e20 7468 6520 636f 6e66 6967 7572 6174  n the configurat
-00019990: 696f 6e20 6669 6c65 206f 7220 6279 2075  ion file or by u
-000199a0: 7369 6e67 2074 6865 2060 2d2d 776f 726b  sing the `--work
-000199b0: 6572 2d70 6f6f 6c60 2028 6f72 2060 2d70  er-pool` (or `-p
-000199c0: 6029 206f 7074 696f 6e2c 2060 7964 2d69  `) option, `yd-i
-000199d0: 6e73 7461 6e74 6961 7465 6020 7769 6c6c  nstantiate` will
-000199e0: 2065 7874 7261 6374 2074 6865 2043 6f6d   extract the Com
-000199f0: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
-00019a00: 2066 726f 6d20 7468 6520 576f 726b 6572   from the Worker
-00019a10: 2050 6f6f 6c20 7370 6563 6966 6963 6174   Pool specificat
-00019a20: 696f 6e20 2869 676e 6f72 696e 6720 576f  ion (ignoring Wo
-00019a30: 726b 6572 2d50 6f6f 6c2d 7370 6563 6966  rker-Pool-specif
-00019a40: 6963 2064 6174 6129 2c20 616e 6420 7573  ic data), and us
-00019a50: 6520 7468 6174 2066 6f72 2069 6e73 7461  e that for insta
-00019a60: 6e74 6961 7469 6e67 2074 6865 2043 6f6d  ntiating the Com
-00019a70: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
-00019a80: 2e0a 0a55 7365 2074 6865 2060 2d2d 6472  ...Use the `--dr
-00019a90: 792d 7275 6e60 206f 7074 696f 6e20 746f  y-run` option to
-00019aa0: 2069 6e73 7065 6374 2074 6865 2064 6574   inspect the det
-00019ab0: 6169 6c73 206f 6620 7468 6520 436f 6d70  ails of the Comp
-00019ac0: 7574 6520 5265 7175 6972 656d 656e 7420  ute Requirement 
-00019ad0: 7370 6563 6966 6963 6174 696f 6e20 7468  specification th
-00019ae0: 6174 2077 696c 6c20 6265 2073 7562 6d69  at will be submi
-00019af0: 7474 6564 2c20 696e 204a 534f 4e20 666f  tted, in JSON fo
-00019b00: 726d 6174 2e20 5468 6520 4a53 4f4e 206f  rmat. The JSON o
-00019b10: 7574 7075 7420 6f66 2074 6869 7320 636f  utput of this co
-00019b20: 6d6d 616e 6420 6361 6e20 6265 2075 7365  mmand can be use
-00019b30: 6420 7769 7468 2074 6865 2060 2d43 6020  d with the `-C` 
-00019b40: 6f70 7469 6f6e 2061 626f 7665 2028 6f72  option above (or
-00019b50: 2077 6974 6820 602d 7060 2066 6f72 2057   with `-p` for W
-00019b60: 6f72 6b65 7220 506f 6f6c 2073 7065 6369  orker Pool speci
-00019b70: 6669 6361 7469 6f6e 7329 2e0a 0a23 2323  fications)...###
-00019b80: 2054 6573 742d 5275 6e6e 696e 6720 6120   Test-Running a 
-00019b90: 4479 6e61 6d69 6320 5465 6d70 6c61 7465  Dynamic Template
-00019ba0: 0a0a 5768 656e 2061 2074 6865 2060 7465  ..When a the `te
-00019bb0: 6d70 6c61 7465 4964 6020 6f66 2061 2044  mplateId` of a D
-00019bc0: 796e 616d 6963 2052 6571 7569 7265 6d65  ynamic Requireme
-00019bd0: 6e74 2069 7320 7573 6564 2c20 7468 6520  nt is used, the 
-00019be0: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
-00019bf0: 2063 6f6d 6d61 6e64 2063 616e 2062 6520   command can be 
-00019c00: 7573 6564 2074 6f20 7265 706f 7274 206f  used to report o
-00019c10: 6e20 6120 7465 7374 2072 756e 206f 6620  n a test run of 
-00019c20: 7468 6520 5465 6d70 6c61 7465 2c20 7573  the Template, us
-00019c30: 696e 6720 7468 6520 602d 2d72 6570 6f72  ing the `--repor
-00019c40: 7460 2028 6f72 2060 2d72 6029 2063 6f6d  t` (or `-r`) com
-00019c50: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
-00019c60: 2e20 5468 6973 2063 616e 2062 6520 7573  . This can be us
-00019c70: 6564 2077 6974 6820 544f 4d4c 2d64 6566  ed with TOML-def
-00019c80: 696e 6564 2043 6f6d 7075 7465 2052 6571  ined Compute Req
-00019c90: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
-00019ca0: 6361 7469 6f6e 732c 2062 7574 206e 6f74  cations, but not
-00019cb0: 2074 686f 7365 2074 6861 7420 6172 6520   those that are 
-00019cc0: 4a53 4f4e 2d64 6566 696e 6564 2e0a 0a4e  JSON-defined...N
-00019cd0: 6f20 696e 7374 616e 6365 7320 7769 6c6c  o instances will
-00019ce0: 2062 6520 7072 6f76 6973 696f 6e65 6420   be provisioned 
-00019cf0: 6475 7269 6e67 2074 6865 2074 6573 7420  during the test 
-00019d00: 7275 6e2e 0a0a 466f 7220 6578 616d 706c  run...For exampl
-00019d10: 653a 0a0a 6060 6073 6865 6c6c 0a25 2079  e:..```shell.% y
-00019d20: 642d 696e 7374 616e 7469 6174 6520 2d2d  d-instantiate --
-00019d30: 7265 706f 7274 202d 2d71 7569 6574 0a0a  report --quiet..
-00019d40: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
-00019d50: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00019d60: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00019d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019d90: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00019da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019dd0: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00019de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019df0: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00019e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e20: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
-00019e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019e60: e294 80e2 9480 e294 80e2 9490 0ae2 9482  ................
-00019e70: 2020 2020 e294 8220 2020 5261 6e6b 20e2      ...   Rank .
-00019e80: 9482 2050 726f 7669 6465 7220 2020 e294  .. Provider   ..
-00019e90: 8220 5479 7065 2020 2020 2020 2020 2020  . Type          
-00019ea0: 2020 2020 2020 20e2 9482 2052 6567 696f         ... Regio
-00019eb0: 6e20 2020 20e2 9482 2049 6e73 7461 6e63  n    ... Instanc
-00019ec0: 6554 7970 6520 2020 e294 8220 536f 7572  eType   ... Sour
-00019ed0: 6365 204e 616d 6520 2020 2020 2020 e294  ce Name       ..
-00019ee0: 820a e294 9ce2 9480 e294 80e2 9480 e294  ................
-00019ef0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00019f00: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00019f10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019f30: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00019f40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019f60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019f70: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-00019f80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019f90: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00019fa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019fb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019fc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019fd0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00019fe0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019ff0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a000: 9480 e294 80e2 9480 e294 80e2 94a4 0ae2  ................
-0001a010: 9482 2020 3120 e294 8220 2020 2020 2031  ..  1 ...      1
-0001a020: 20e2 9482 2041 5753 2020 2020 2020 2020   ... AWS        
-0001a030: e294 8220 4177 7353 706f 7443 6f6d 7075  ... AwsSpotCompu
-0001a040: 7465 536f 7572 6365 20e2 9482 2065 752d  teSource ... eu-
-0001a050: 7765 7374 2d32 20e2 9482 2074 3361 2e6e  west-2 ... t3a.n
-0001a060: 616e 6f20 2020 2020 2020 e294 8220 6177  ano       ... aw
-0001a070: 7373 706f 742d 6575 2d77 6573 742d 3220  sspot-eu-west-2 
-0001a080: e294 820a e294 9ce2 9480 e294 80e2 9480  ................
-0001a090: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a0a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a0b0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a0c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a0d0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a0e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a0f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a100: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a110: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001a120: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a130: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a140: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a150: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a160: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a170: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a190: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a1a0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
-0001a1b0: 0ae2 9482 2020 3220 e294 8220 2020 2020  ....  2 ...     
-0001a1c0: 2032 20e2 9482 2041 5753 2020 2020 2020   2 ... AWS      
-0001a1d0: 2020 e294 8220 4177 7353 706f 7443 6f6d    ... AwsSpotCom
-0001a1e0: 7075 7465 536f 7572 6365 20e2 9482 2065  puteSource ... e
-0001a1f0: 752d 7765 7374 2d32 20e2 9482 2074 3361  u-west-2 ... t3a
-0001a200: 2e6d 6963 726f 2020 2020 2020 e294 8220  .micro      ... 
-0001a210: 6177 7373 706f 742d 6575 2d77 6573 742d  awsspot-eu-west-
-0001a220: 3220 e294 820a e294 9ce2 9480 e294 80e2  2 ..............
-0001a230: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a240: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a250: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a270: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a2a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a2b0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001a2c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a2d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a2e0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a2f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a310: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a320: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a330: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a340: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a350: 94a4 0ae2 9482 2020 3320 e294 8220 2020  ......  3 ...   
-0001a360: 2020 2033 20e2 9482 2041 5753 2020 2020     3 ... AWS    
-0001a370: 2020 2020 e294 8220 4177 7353 706f 7443      ... AwsSpotC
-0001a380: 6f6d 7075 7465 536f 7572 6365 20e2 9482  omputeSource ...
-0001a390: 2065 752d 7765 7374 2d32 20e2 9482 2074   eu-west-2 ... t
-0001a3a0: 3361 2e73 6d61 6c6c 2020 2020 2020 e294  3a.small      ..
-0001a3b0: 8220 6177 7373 706f 742d 6575 2d77 6573  . awsspot-eu-wes
-0001a3c0: 742d 3220 e294 820a e294 9ce2 9480 e294  t-2 ............
-0001a3d0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a3e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a3f0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a400: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a410: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a420: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a430: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a440: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a460: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a480: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a4a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a4b0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a4c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a4d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a4e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a4f0: 80e2 94a4 0ae2 9482 2020 3420 e294 8220  ........  4 ... 
-0001a500: 2020 2020 2034 20e2 9482 2041 5753 2020       4 ... AWS  
-0001a510: 2020 2020 2020 e294 8220 4177 7353 706f        ... AwsSpo
-0001a520: 7443 6f6d 7075 7465 536f 7572 6365 20e2  tComputeSource .
-0001a530: 9482 2065 752d 7765 7374 2d32 20e2 9482  .. eu-west-2 ...
-0001a540: 2063 3561 2e6c 6172 6765 2020 2020 2020   c5a.large      
-0001a550: e294 8220 6177 7373 706f 742d 6575 2d77  ... awsspot-eu-w
-0001a560: 6573 742d 3220 e294 820a e294 9ce2 9480  est-2 ..........
-0001a570: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a590: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a5a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a5b0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a5c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a5d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a5e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a5f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a600: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a620: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a650: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a660: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a670: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a680: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a690: e294 80e2 94a4 0ae2 9482 2020 3520 e294  ..........  5 ..
-0001a6a0: 8220 2020 2020 2034 20e2 9482 2041 5753  .      4 ... AWS
-0001a6b0: 2020 2020 2020 2020 e294 8220 4177 7353          ... AwsS
-0001a6c0: 706f 7443 6f6d 7075 7465 536f 7572 6365  potComputeSource
-0001a6d0: 20e2 9482 2065 752d 7765 7374 2d32 20e2   ... eu-west-2 .
-0001a6e0: 9482 2063 3661 2e6c 6172 6765 2020 2020  .. c6a.large    
-0001a6f0: 2020 e294 8220 6177 7373 706f 742d 6575    ... awsspot-eu
-0001a700: 2d77 6573 742d 3220 e294 820a e294 9ce2  -west-2 ........
-0001a710: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a730: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a750: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a760: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a790: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a7a0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a7b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a7c0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a7d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a7e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a7f0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a830: 9480 e294 80e2 94a4 0ae2 9482 2020 3620  ............  6 
-0001a840: e294 8220 2020 2020 2034 20e2 9482 2041  ...      4 ... A
-0001a850: 5753 2020 2020 2020 2020 e294 8220 4177  WS        ... Aw
-0001a860: 7353 706f 7443 6f6d 7075 7465 536f 7572  sSpotComputeSour
-0001a870: 6365 20e2 9482 2065 752d 7765 7374 2d32  ce ... eu-west-2
-0001a880: 20e2 9482 2074 3361 2e6d 6564 6975 6d20   ... t3a.medium 
-0001a890: 2020 2020 e294 8220 6177 7373 706f 742d      ... awsspot-
-0001a8a0: 6575 2d77 6573 742d 3220 e294 820a e294  eu-west-2 ......
-0001a8b0: 9ce2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a8c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a8d0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a8e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a8f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a900: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a910: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a920: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a930: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a940: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a960: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a990: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a9a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a9b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a9c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a9d0: 80e2 9480 e294 80e2 94a4 0ae2 9482 2020  ..............  
-0001a9e0: 3720 e294 8220 2020 2020 2035 20e2 9482  7 ...      5 ...
-0001a9f0: 2041 5753 2020 2020 2020 2020 e294 8220   AWS        ... 
-0001aa00: 4177 7353 706f 7443 6f6d 7075 7465 536f  AwsSpotComputeSo
-0001aa10: 7572 6365 20e2 9482 2065 752d 7765 7374  urce ... eu-west
-0001aa20: 2d32 20e2 9482 206d 3561 2e6c 6172 6765  -2 ... m5a.large
-0001aa30: 2020 2020 2020 e294 8220 6177 7373 706f        ... awsspo
-0001aa40: 742d 6575 2d77 6573 742d 3220 e294 820a  t-eu-west-2 ....
-0001aa50: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa60: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aa70: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001aa80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aaa0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001aab0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aac0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aae0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001aaf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ab00: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001ab10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ab20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ab30: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001ab40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ab50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ab60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ab70: e294 80e2 9480 e294 80e2 94a4 0ae2 9482  ................
-0001ab80: 2020 3820 e294 8220 2020 2020 2035 20e2    8 ...      5 .
-0001ab90: 9482 2041 5753 2020 2020 2020 2020 e294  .. AWS        ..
-0001aba0: 8220 4177 7353 706f 7443 6f6d 7075 7465  . AwsSpotCompute
-0001abb0: 536f 7572 6365 20e2 9482 2065 752d 7765  Source ... eu-we
-0001abc0: 7374 2d32 20e2 9482 206d 3561 642e 6c61  st-2 ... m5ad.la
-0001abd0: 7267 6520 2020 2020 e294 8220 6177 7373  rge     ... awss
-0001abe0: 706f 742d 6575 2d77 6573 742d 3220 e294  pot-eu-west-2 ..
-0001abf0: 820a e294 9ce2 9480 e294 80e2 9480 e294  ................
-0001ac00: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001ac10: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001ac20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ac30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ac40: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001ac50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ac60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ac70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ac80: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001ac90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aca0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001acb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001acc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001acd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ace0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001acf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ad00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ad10: 9480 e294 80e2 9480 e294 80e2 94a4 0ae2  ................
-0001ad20: 9482 2020 3920 e294 8220 2020 2020 2035  ..  9 ...      5
-0001ad30: 20e2 9482 2041 5753 2020 2020 2020 2020   ... AWS        
-0001ad40: e294 8220 4177 7353 706f 7443 6f6d 7075  ... AwsSpotCompu
-0001ad50: 7465 536f 7572 6365 20e2 9482 2065 752d  teSource ... eu-
-0001ad60: 7765 7374 2d32 20e2 9482 206d 3661 2e6c  west-2 ... m6a.l
-0001ad70: 6172 6765 2020 2020 2020 e294 8220 6177  arge      ... aw
-0001ad80: 7373 706f 742d 6575 2d77 6573 742d 3220  sspot-eu-west-2 
-0001ad90: e294 820a e294 9ce2 9480 e294 80e2 9480  ................
-0001ada0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001adb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001adc0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001add0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ade0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001adf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ae00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ae20: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001ae30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ae50: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ae60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ae80: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001ae90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aea0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aeb0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
-0001aec0: 0ae2 9482 2031 3020 e294 8220 2020 2020  .... 10 ...     
-0001aed0: 2035 20e2 9482 2041 5753 2020 2020 2020   5 ... AWS      
-0001aee0: 2020 e294 8220 4177 7353 706f 7443 6f6d    ... AwsSpotCom
-0001aef0: 7075 7465 536f 7572 6365 20e2 9482 2065  puteSource ... e
-0001af00: 752d 7765 7374 2d32 20e2 9482 2074 3361  u-west-2 ... t3a
-0001af10: 2e6c 6172 6765 2020 2020 2020 e294 8220  .large      ... 
-0001af20: 6177 7373 706f 742d 6575 2d77 6573 742d  awsspot-eu-west-
-0001af30: 3220 e294 820a e294 94e2 9480 e294 80e2  2 ..............
-0001af40: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
-0001af50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001af60: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-0001af70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001af80: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-0001af90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001afa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001afb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001afc0: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
-0001afd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001afe0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aff0: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-0001b000: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001b010: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001b020: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-0001b030: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001b040: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001b050: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001b060: 9498 0a60 6060 0a0a 2323 2079 642d 7465  ...```..## yd-te
-0001b070: 726d 696e 6174 650a 0a54 6865 2060 7964  rminate..The `yd
-0001b080: 2d74 6572 6d69 6e61 7465 6020 636f 6d6d  -terminate` comm
-0001b090: 616e 6420 696d 6d65 6469 6174 656c 7920  and immediately 
-0001b0a0: 7465 726d 696e 6174 6573 2043 6f6d 7075  terminates Compu
-0001b0b0: 7465 2052 6571 7569 7265 6d65 6e74 7320  te Requirements 
-0001b0c0: 7468 6174 206d 6174 6368 2074 6865 2060  that match the `
-0001b0d0: 6e61 6d65 7370 6163 6560 2061 6e64 2060  namespace` and `
-0001b0e0: 7461 6760 2066 6f75 6e64 2069 6e20 7468  tag` found in th
-0001b0f0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-0001b100: 6669 6c65 2e20 416e 7920 6578 6563 7574  file. Any execut
-0001b110: 696e 6720 5461 736b 7320 7769 6c6c 2062  ing Tasks will b
-0001b120: 6520 7465 726d 696e 6174 6564 2069 6d6d  e terminated imm
-0001b130: 6564 6961 7465 6c79 2c20 616e 6420 7468  ediately, and th
-0001b140: 6520 576f 726b 6572 2050 6f6f 6c20 7769  e Worker Pool wi
-0001b150: 6c6c 2062 6520 7368 7574 2064 6f77 6e2e  ll be shut down.
-0001b160: 0a                                       .
+000155a0: 2273 7461 7274 5f73 696d 706c 655f 736c  "start_simple_sl
+000155b0: 7572 6d63 746c 6422 2c0a 2020 2020 2020  urmctld",.      
+000155c0: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
+000155d0: 656e 7473 223a 205b 226e 6f64 6573 2e6a  ents": ["nodes.j
+000155e0: 736f 6e22 5d2c 0a20 2020 2020 2020 2020  son"],.         
+000155f0: 2020 2020 2020 2022 656e 7669 726f 6e6d         "environm
+00015600: 656e 7422 3a20 7b22 4558 414d 504c 4522  ent": {"EXAMPLE"
+00015610: 3a20 2246 4f4f 227d 2c0a 2020 2020 2020  : "FOO"},.      
+00015620: 2020 2020 2020 2020 2020 226e 6f64 6554            "nodeT
+00015630: 7970 6573 223a 205b 2273 6c75 726d 6374  ypes": ["slurmct
+00015640: 6c64 225d 0a20 2020 2020 2020 2020 2020  ld"].           
+00015650: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00015660: 205d 0a20 2020 2020 2020 2020 207d 2c0a   ].          },.
+00015670: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00015680: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
+00015690: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+000156a0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000156b0: 2020 2020 2022 6163 7469 6f6e 223a 2022       "action": "
+000156c0: 5255 4e5f 434f 4d4d 414e 4422 2c0a 2020  RUN_COMMAND",.  
+000156d0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000156e0: 6174 6822 3a20 2273 7461 7274 5f73 696d  ath": "start_sim
+000156f0: 706c 655f 736c 7572 6d64 222c 0a20 2020  ple_slurmd",.   
+00015700: 2020 2020 2020 2020 2020 2020 2022 6172               "ar
+00015710: 6775 6d65 6e74 7322 3a20 5b22 7b7b 6e6f  guments": ["{{no
+00015720: 6465 7342 7954 7970 652e 736c 7572 6d63  desByType.slurmc
+00015730: 746c 642e 302e 6465 7461 696c 732e 7072  tld.0.details.pr
+00015740: 6976 6174 6549 7041 6464 7265 7373 7d7d  ivateIpAddress}}
+00015750: 222c 2022 7b7b 6e6f 6465 2e64 6574 6169  ", "{{node.detai
+00015760: 6c73 2e6e 6f64 6553 6c6f 747d 7d22 5d2c  ls.nodeSlot}}"],
+00015770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015780: 2022 6e6f 6465 5479 7065 7322 3a20 5b22   "nodeTypes": ["
+00015790: 736c 7572 6d64 225d 0a20 2020 2020 2020  slurmd"].       
+000157a0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000157b0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+000157c0: 207d 2c0a 2020 2020 2020 2020 2020 7b0a   },.          {.
+000157d0: 2020 2020 2020 2020 2020 2020 2261 6374              "act
+000157e0: 696f 6e73 223a 205b 0a20 2020 2020 2020  ions": [.       
+000157f0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00015800: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
+00015810: 223a 2022 4352 4541 5445 5f57 4f52 4b45  ": "CREATE_WORKE
+00015820: 5253 222c 0a20 2020 2020 2020 2020 2020  RS",.           
+00015830: 2020 2020 2022 746f 7461 6c57 6f72 6b65       "totalWorke
+00015840: 7273 223a 2031 2c0a 2020 2020 2020 2020  rs": 1,.        
+00015850: 2020 2020 2020 2020 226e 6f64 6554 7970          "nodeTyp
+00015860: 6573 223a 205b 2273 6c75 726d 6374 6c64  es": ["slurmctld
+00015870: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00015880: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
+00015890: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
+000158a0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+000158b0: 224e 4f44 4553 5f41 4444 4544 223a 205b  "NODES_ADDED": [
+000158c0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
+000158d0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
+000158e0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+000158f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00015900: 2020 2020 2020 2261 6374 696f 6e22 3a20        "action": 
+00015910: 2257 5249 5445 5f46 494c 4522 2c0a 2020  "WRITE_FILE",.  
+00015920: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00015930: 6174 6822 3a20 226e 6f64 6573 2e6a 736f  ath": "nodes.jso
+00015940: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+00015950: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
+00015960: 7b5c 6e20 205c 226e 6f64 6573 5c22 3a20  {\n  \"nodes\": 
+00015970: 5b5c 6e7b 7b23 6669 6c74 6572 6564 4e6f  [\n{{#filteredNo
+00015980: 6465 737d 7d5c 6e20 2020 207b 5c6e 2020  des}}\n    {\n  
+00015990: 2020 2020 5c22 6e61 6d65 5c22 3a20 5c22      \"name\": \"
+000159a0: 736c 7572 6d64 7b7b 6465 7461 696c 732e  slurmd{{details.
+000159b0: 6e6f 6465 536c 6f74 7d7d 5c22 2c5c 6e20  nodeSlot}}\",\n 
+000159c0: 2020 2020 205c 2269 705c 223a 205c 227b       \"ip\": \"{
+000159d0: 7b64 6574 6169 6c73 2e70 7269 7661 7465  {details.private
+000159e0: 4970 4164 6472 6573 737d 7d5c 225c 6e20  IpAddress}}\"\n 
+000159f0: 2020 207d 7b7b 5e2d 6c61 7374 7d7d 2c7b     }{{^-last}},{
+00015a00: 7b2f 2d6c 6173 747d 7d5c 6e7b 7b2f 6669  {/-last}}\n{{/fi
+00015a10: 6c74 6572 6564 4e6f 6465 737d 7d5c 6e20  lteredNodes}}\n 
+00015a20: 205d 5c6e 7d22 2c0a 2020 2020 2020 2020   ]\n}",.        
+00015a30: 2020 2020 2020 2020 226e 6f64 6554 7970          "nodeTyp
+00015a40: 6573 223a 205b 2273 6c75 726d 6374 6c64  es": ["slurmctld
+00015a50: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00015a60: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00015a70: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00015a80: 2020 2020 2261 6374 696f 6e22 3a20 2252      "action": "R
+00015a90: 554e 5f43 4f4d 4d41 4e44 222c 0a20 2020  UN_COMMAND",.   
+00015aa0: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+00015ab0: 7468 223a 2022 6164 645f 6e6f 6465 7322  th": "add_nodes"
+00015ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015ad0: 2020 2261 7267 756d 656e 7473 223a 205b    "arguments": [
+00015ae0: 226e 6f64 6573 2e6a 736f 6e22 5d2c 0a20  "nodes.json"],. 
+00015af0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015b00: 6e6f 6465 5479 7065 7322 3a20 5b22 736c  nodeTypes": ["sl
+00015b10: 7572 6d63 746c 6422 5d0a 2020 2020 2020  urmctld"].      
+00015b20: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00015b30: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00015b40: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
+00015b50: 0a20 2020 2020 2020 2020 2020 2022 6163  .            "ac
+00015b60: 7469 6f6e 7322 3a20 5b0a 2020 2020 2020  tions": [.      
+00015b70: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00015b80: 2020 2020 2020 2020 2020 2261 6374 696f            "actio
+00015b90: 6e22 3a20 2252 554e 5f43 4f4d 4d41 4e44  n": "RUN_COMMAND
+00015ba0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00015bb0: 2020 2022 7061 7468 223a 2022 7374 6172     "path": "star
+00015bc0: 745f 7369 6d70 6c65 5f73 6c75 726d 6422  t_simple_slurmd"
+00015bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015be0: 2020 2261 7267 756d 656e 7473 223a 205b    "arguments": [
+00015bf0: 227b 7b6e 6f64 6573 4279 5479 7065 2e73  "{{nodesByType.s
+00015c00: 6c75 726d 6374 6c64 2e30 2e64 6574 6169  lurmctld.0.detai
+00015c10: 6c73 2e70 7269 7661 7465 4970 4164 6472  ls.privateIpAddr
+00015c20: 6573 737d 7d22 2c20 227b 7b6e 6f64 652e  ess}}", "{{node.
+00015c30: 6465 7461 696c 732e 6e6f 6465 536c 6f74  details.nodeSlot
+00015c40: 7d7d 225d 2c0a 2020 2020 2020 2020 2020  }}"],.          
+00015c50: 2020 2020 2020 226e 6f64 6549 6446 696c        "nodeIdFil
+00015c60: 7465 7222 3a20 2245 5645 4e54 222c 0a20  ter": "EVENT",. 
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015c80: 6e6f 6465 5479 7065 7322 3a20 5b22 736c  nodeTypes": ["sl
+00015c90: 7572 6d64 225d 0a20 2020 2020 2020 2020  urmd"].         
+00015ca0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00015cb0: 2020 205d 0a20 2020 2020 2020 2020 207d     ].          }
+00015cc0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00015cd0: 207d 0a20 2020 207d 2c0a 2020 2020 2277   }.    },.    "w
+00015ce0: 6f72 6b65 7254 6167 223a 2022 7079 6578  orkerTag": "pyex
+00015cf0: 2d73 6c75 726d 2d63 6c75 7374 6572 220a  -slurm-cluster".
+00015d00: 2020 7d0a 7d0a 6060 600a 0a23 2323 2054    }.}.```..### T
+00015d10: 4f4d 4c20 5072 6f70 6572 7469 6573 2049  OML Properties I
+00015d20: 6e68 6572 6974 6564 2062 7920 576f 726b  nherited by Work
+00015d30: 6572 2050 6f6f 6c20 4a53 4f4e 2053 7065  er Pool JSON Spe
+00015d40: 6369 6669 6361 7469 6f6e 730a 0a57 6865  cifications..Whe
+00015d50: 6e20 6120 4a53 4f4e 2057 6f72 6b65 7220  n a JSON Worker 
+00015d60: 506f 6f6c 2073 7065 6369 6669 6361 7469  Pool specificati
+00015d70: 6f6e 2069 7320 7573 6564 2c20 7468 6520  on is used, the 
+00015d80: 666f 6c6c 6f77 696e 6720 7072 6f70 6572  following proper
+00015d90: 7469 6573 2066 726f 6d20 7468 6520 6063  ties from the `c
+00015da0: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00015db0: 2077 696c 6c20 6265 2069 6e68 6572 6974   will be inherit
+00015dc0: 6564 2069 6620 7468 6520 7661 6c75 6520  ed if the value 
+00015dd0: 6973 2061 6273 656e 7420 696e 2074 6865  is absent in the
+00015de0: 204a 534f 4e20 6669 6c65 3a0a 0a2a 2a50   JSON file:..**P
+00015df0: 726f 7065 7274 6965 7320 496e 6865 7269  roperties Inheri
+00015e00: 7465 6420 7769 7468 696e 2074 6865 2060  ted within the `
+00015e10: 7265 7175 6972 656d 656e 7454 656d 706c  requirementTempl
+00015e20: 6174 6555 7361 6765 6020 7072 6f70 6572  ateUsage` proper
+00015e30: 7479 2a2a 0a0a 2d20 6069 6d61 6765 7349  ty**..- `imagesI
+00015e40: 6460 0a2d 2060 696e 7374 616e 6365 5461  d`.- `instanceTa
+00015e50: 6773 600a 2d20 6072 6571 7569 7265 6d65  gs`.- `requireme
+00015e60: 6e74 4e61 6d65 603a 2064 6572 6976 6564  ntName`: derived
+00015e70: 2066 726f 6d20 7468 6520 606e 616d 6560   from the `name`
+00015e80: 2070 726f 7065 7274 7920 696e 2074 6865   property in the
+00015e90: 2060 544f 4d4c 6020 636f 6e66 6967 7572   `TOML` configur
+00015ea0: 6174 696f 6e2e 2028 5468 6520 6e61 6d65  ation. (The name
+00015eb0: 2077 696c 6c20 6265 2067 656e 6572 6174   will be generat
+00015ec0: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
+00015ed0: 2069 6620 6e6f 7420 7375 7070 6c69 6564   if not supplied
+00015ee0: 2069 6e20 6569 7468 6572 2074 6865 2054   in either the T
+00015ef0: 4f4d 4c20 6669 6c65 206f 7220 7468 6520  OML file or the 
+00015f00: 4a53 4f4e 2073 7065 6369 6669 6361 7469  JSON specificati
+00015f10: 6f6e 2e29 0a2d 2060 7265 7175 6972 656d  on.).- `requirem
+00015f20: 656e 744e 616d 6573 7061 6365 603a 2064  entNamespace`: d
+00015f30: 6572 6976 6564 2066 726f 6d20 7468 6520  erived from the 
+00015f40: 606e 616d 6573 7061 6365 6020 7072 6f70  `namespace` prop
+00015f50: 6572 7479 2069 6e20 7468 6520 6054 4f4d  erty in the `TOM
+00015f60: 4c60 2063 6f6e 6669 6775 7261 7469 6f6e  L` configuration
+00015f70: 0a2d 2060 7265 7175 6972 656d 656e 7454  .- `requirementT
+00015f80: 6167 603a 203a 2064 6572 6976 6564 2066  ag`: : derived f
+00015f90: 726f 6d20 7468 6520 6074 6167 6020 7072  rom the `tag` pr
+00015fa0: 6f70 6572 7479 2069 6e20 7468 6520 6054  operty in the `T
+00015fb0: 4f4d 4c60 2063 6f6e 6669 6775 7261 7469  OML` configurati
+00015fc0: 6f6e 0a2d 2060 7461 7267 6574 496e 7374  on.- `targetInst
+00015fd0: 616e 6365 436f 756e 7460 0a2d 2060 7465  anceCount`.- `te
+00015fe0: 6d70 6c61 7465 4964 600a 2d20 6075 7365  mplateId`.- `use
+00015ff0: 7244 6174 6160 0a2d 2060 7573 6572 4461  rData`.- `userDa
+00016000: 7461 4669 6c65 600a 2d20 6075 7365 7244  taFile`.- `userD
+00016010: 6174 6146 696c 6573 600a 0a2a 2a50 726f  ataFiles`..**Pro
+00016020: 7065 7274 6965 7320 496e 6865 7269 7465  perties Inherite
+00016030: 6420 7769 7468 696e 2074 6865 2060 7072  d within the `pr
+00016040: 6f76 6973 696f 6e65 6450 726f 7065 7274  ovisionedPropert
+00016050: 6965 7360 2050 726f 7065 7274 792a 2a0a  ies` Property**.
+00016060: 0a2d 2060 6964 6c65 4e6f 6465 5368 7574  .- `idleNodeShut
+00016070: 646f 776e 456e 6162 6c65 6460 0a2d 2060  downEnabled`.- `
+00016080: 6964 6c65 4e6f 6465 5368 7574 646f 776e  idleNodeShutdown
+00016090: 5469 6d65 6f75 7460 0a2d 2060 6964 6c65  Timeout`.- `idle
+000160a0: 506f 6f6c 5368 7574 646f 776e 456e 6162  PoolShutdownEnab
+000160b0: 6c65 6460 0a2d 2060 6964 6c65 506f 6f6c  led`.- `idlePool
+000160c0: 5368 7574 646f 776e 5469 6d65 6f75 7460  ShutdownTimeout`
+000160d0: 0a2d 2060 6e6f 6465 426f 6f74 5469 6d65  .- `nodeBootTime
+000160e0: 6f75 7460 0a2d 2060 776f 726b 6572 5461  out`.- `workerTa
+000160f0: 6760 0a0a 2323 2056 6172 6961 626c 6520  g`..## Variable 
+00016100: 5375 6273 7469 7475 7469 6f6e 7320 696e  Substitutions in
+00016110: 2057 6f72 6b65 7220 506f 6f6c 2050 726f   Worker Pool Pro
+00016120: 7065 7274 6965 730a 0a56 6172 6961 626c  perties..Variabl
+00016130: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
+00016140: 6361 6e20 6265 2075 7365 6420 7769 7468  can be used with
+00016150: 696e 2061 6e79 2070 726f 7065 7274 7920  in any property 
+00016160: 7661 6c75 6520 696e 2054 4f4d 4c20 636f  value in TOML co
+00016170: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00016180: 7320 6f72 2057 6f72 6b65 7220 506f 6f6c  s or Worker Pool
+00016190: 204a 534f 4e20 6669 6c65 732e 2053 6565   JSON files. See
+000161a0: 2074 6865 2064 6573 6372 6970 7469 6f6e   the description
+000161b0: 205b 6162 6f76 655d 2823 7661 7269 6162   [above](#variab
+000161c0: 6c65 2d73 7562 7374 6974 7574 696f 6e73  le-substitutions
+000161d0: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+000161e0: 6c73 206f 6e20 7661 7269 6162 6c65 2073  ls on variable s
+000161f0: 7562 7374 6974 7574 696f 6e73 2e20 5468  ubstitutions. Th
+00016200: 6973 2069 7320 6120 706f 7765 7266 756c  is is a powerful
+00016210: 2066 6561 7475 7265 2074 6861 7420 616c   feature that al
+00016220: 6c6f 7773 2057 6f72 6b65 7220 506f 6f6c  lows Worker Pool
+00016230: 7320 746f 2062 6520 7061 7261 6d65 7465  s to be paramete
+00016240: 7269 7365 6420 6279 2073 7570 706c 7969  rised by supplyi
+00016250: 6e67 2076 616c 7565 7320 6f6e 2074 6865  ng values on the
+00016260: 2063 6f6d 6d61 6e64 206c 696e 652c 2076   command line, v
+00016270: 6961 2065 6e76 6972 6f6e 6d65 6e74 2076  ia environment v
+00016280: 6172 6961 626c 6573 2c20 6f72 2076 6961  ariables, or via
+00016290: 2074 6865 2054 4f4d 4c20 6669 6c65 2e0a   the TOML file..
+000162a0: 0a41 6e20 696d 706f 7274 616e 7420 6469  .An important di
+000162b0: 7374 696e 6374 696f 6e20 2a2a 6f6e 6c79  stinction **only
+000162c0: 2a2a 2077 6865 6e20 7573 696e 6720 7661  ** when using va
+000162d0: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+000162e0: 696f 6e73 2077 6974 6869 6e20 576f 726b  ions within Work
+000162f0: 6572 2050 6f6f 6c20 4a53 4f4e 2064 6f63  er Pool JSON doc
+00016300: 756d 656e 7473 2069 7320 7468 6174 2065  uments is that e
+00016310: 6163 6820 6469 7265 6374 6976 6520 2a2a  ach directive **
+00016320: 6d75 7374 2062 6520 7072 6563 6564 6564  must be preceded
+00016330: 2062 7920 6120 605f 5f60 2028 646f 7562   by a `__` (doub
+00016340: 6c65 2075 6e64 6572 7363 6f72 6529 2a2a  le underscore)**
+00016350: 2074 6f20 6469 7361 6d62 6967 7561 7465   to disambiguate
+00016360: 2069 7420 6672 6f6d 2076 6172 6961 626c   it from variabl
+00016370: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
+00016380: 7468 6174 2061 7265 2074 6f20 6265 2070  that are to be p
+00016390: 6173 7365 6420 6469 7265 6374 6c79 2074  assed directly t
+000163a0: 6f20 7468 6520 4150 492e 2046 6f72 2065  o the API. For e
+000163b0: 7861 6d70 6c65 2c20 7573 653a 2060 5f5f  xample, use: `__
+000163c0: 7b7b 7573 6572 6e61 6d65 7d7d 6020 746f  {{username}}` to
+000163d0: 2061 7070 6c79 2061 2073 7562 7374 6974   apply a substit
+000163e0: 7574 696f 6e20 666f 7220 7468 6520 6075  ution for the `u
+000163f0: 7365 726e 616d 6560 2064 6566 6175 6c74  sername` default
+00016400: 2073 7562 7374 6974 7574 696f 6e2e 0a0a   substitution...
+00016410: 2323 2044 7279 2d52 756e 6e69 6e67 2057  ## Dry-Running W
+00016420: 6f72 6b65 7220 506f 6f6c 2050 726f 7669  orker Pool Provi
+00016430: 7369 6f6e 696e 670a 0a54 6f20 6578 616d  sioning..To exam
+00016440: 696e 6520 7468 6520 4a53 4f4e 2074 6861  ine the JSON tha
+00016450: 7420 7769 6c6c 2061 6374 7561 6c6c 7920  t will actually 
+00016460: 6265 2073 656e 7420 746f 2074 6865 2059  be sent to the Y
+00016470: 656c 6c6f 7744 6f67 2041 5049 2061 6674  ellowDog API aft
+00016480: 6572 2061 6c6c 2070 726f 6365 7373 696e  er all processin
+00016490: 672c 2075 7365 2074 6865 2060 2d2d 6472  g, use the `--dr
+000164a0: 792d 7275 6e60 2063 6f6d 6d61 6e64 206c  y-run` command l
+000164b0: 696e 6520 6f70 7469 6f6e 2077 6865 6e20  ine option when 
+000164c0: 7275 6e6e 696e 6720 6079 642d 7072 6f76  running `yd-prov
+000164d0: 6973 696f 6e60 2e20 5468 6973 2077 696c  ision`. This wil
+000164e0: 6c20 7072 696e 7420 7468 6520 4a53 4f4e  l print the JSON
+000164f0: 2073 7065 6369 6669 6361 7469 6f6e 2066   specification f
+00016500: 6f72 2074 6865 2057 6f72 6b65 7220 506f  or the Worker Po
+00016510: 6f6c 2e20 4e6f 7468 696e 6720 7769 6c6c  ol. Nothing will
+00016520: 2062 6520 7375 626d 6974 7465 6420 746f   be submitted to
+00016530: 2074 6865 2070 6c61 7466 6f72 6d2e 0a0a   the platform...
+00016540: 5468 6520 6765 6e65 7261 7465 6420 4a53  The generated JS
+00016550: 4f4e 2069 7320 7072 6f64 7563 6564 2061  ON is produced a
+00016560: 6674 6572 2061 6c6c 2070 726f 6365 7373  fter all process
+00016570: 696e 6720 2869 6e63 6f72 706f 7261 7469  ing (incorporati
+00016580: 6e67 2060 636f 6e66 6967 2e74 6f6d 6c60  ng `config.toml`
+00016590: 2070 726f 7065 7274 6965 732c 2076 6172   properties, var
+000165a0: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+000165b0: 6f6e 732c 2065 7463 2e29 2068 6173 2062  ons, etc.) has b
+000165c0: 6565 6e20 636f 6e63 6c75 6465 642c 2073  een concluded, s
+000165d0: 6f20 7468 6520 6472 792d 7275 6e20 6973  o the dry-run is
+000165e0: 2075 7365 6675 6c20 666f 7220 696e 7370   useful for insp
+000165f0: 6563 7469 6e67 2074 6865 2072 6573 756c  ecting the resul
+00016600: 7473 206f 6620 616c 6c20 7468 6520 7072  ts of all the pr
+00016610: 6f63 6573 7369 6e67 2074 6861 7427 7320  ocessing that's 
+00016620: 6265 656e 2070 6572 666f 726d 6564 2e0a  been performed..
+00016630: 0a54 6f20 7375 7070 7265 7373 2061 6c6c  .To suppress all
+00016640: 206f 7574 7075 7420 6578 6365 7074 2066   output except f
+00016650: 6f72 2074 6865 204a 534f 4e20 6974 7365  or the JSON itse
+00016660: 6c66 2c20 7573 6520 7468 6520 602d 2d71  lf, use the `--q
+00016670: 7569 6574 6020 2860 2d71 6029 2063 6f6d  uiet` (`-q`) com
+00016680: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
+00016690: 2e0a 0a54 6865 204a 534f 4e20 6472 792d  ...The JSON dry-
+000166a0: 7275 6e20 6f75 7470 7574 2063 6f75 6c64  run output could
+000166b0: 2069 7473 656c 6620 6265 2075 7365 6420   itself be used 
+000166c0: 6279 2060 7964 2d70 726f 7669 7369 6f6e  by `yd-provision
+000166d0: 602c 2069 6620 6361 7074 7572 6564 2069  `, if captured i
+000166e0: 6e20 6120 6669 6c65 2c20 652e 672e 3a0a  n a file, e.g.:.
+000166f0: 0a60 6060 7368 656c 6c0a 7964 2d70 726f  .```shell.yd-pro
+00016700: 7669 7369 6f6e 202d 2d64 7279 2d72 756e  vision --dry-run
+00016710: 202d 7120 3e20 6d79 5f77 6f72 6b65 725f   -q > my_worker_
+00016720: 706f 6f6c 2e6a 736f 6e0a 7964 2d70 726f  pool.json.yd-pro
+00016730: 7669 7369 6f6e 202d 7020 6d79 5f77 6f72  vision -p my_wor
+00016740: 6b65 725f 706f 6f6c 2e6a 736f 6e0a 6060  ker_pool.json.``
+00016750: 600a 0a23 204a 736f 6e6e 6574 2053 7570  `..# Jsonnet Sup
+00016760: 706f 7274 0a0a 496e 2061 6c6c 2063 6972  port..In all cir
+00016770: 6375 6d73 7461 6e63 6573 2077 6865 7265  cumstances where
+00016780: 204a 534f 4e20 6669 6c65 7320 6172 6520   JSON files are 
+00016790: 7573 6564 2062 7920 7468 6520 5079 7468  used by the Pyth
+000167a0: 6f6e 2045 7861 6d70 6c65 7320 7363 7269  on Examples scri
+000167b0: 7074 732c 2020 2a2a 5b4a 736f 6e6e 6574  pts,  **[Jsonnet
+000167c0: 5d28 6874 7470 733a 2f2f 6a73 6f6e 6e65  ](https://jsonne
+000167d0: 742e 6f72 6729 2a2a 2066 696c 6573 2063  t.org)** files c
+000167e0: 616e 2062 6520 7573 6564 2069 6e73 7465  an be used inste
+000167f0: 6164 2e20 5468 6973 2061 6c6c 6f77 7320  ad. This allows 
+00016800: 7468 6520 7573 6520 6f66 204a 736f 6e6e  the use of Jsonn
+00016810: 6574 2773 2070 6f77 6572 6675 6c20 4a53  et's powerful JS
+00016820: 4f4e 2065 7874 656e 7369 6f6e 732c 2069  ON extensions, i
+00016830: 6e63 6c75 6469 6e67 2063 6f6d 6d65 6e74  ncluding comment
+00016840: 732c 2076 6172 6961 626c 6573 2c20 6675  s, variables, fu
+00016850: 6e63 7469 6f6e 732c 2065 7463 2e0a 0a41  nctions, etc...A
+00016860: 2073 696d 706c 6520 7573 6167 6520 6578   simple usage ex
+00016870: 616d 706c 6520 6d69 6768 7420 6265 3a0a  ample might be:.
+00016880: 0a60 6060 7368 656c 6c0a 7964 2d73 7562  .```shell.yd-sub
+00016890: 6d69 7420 2d2d 776f 726b 2d72 6571 7569  mit --work-requi
+000168a0: 7265 6d65 6e74 206d 795f 776f 726b 5f72  rement my_work_r
+000168b0: 6571 2e6a 736f 6e6e 6574 0a60 6060 0a0a  eq.jsonnet.```..
+000168c0: 5468 6520 7573 6520 6f66 2074 6865 2066  The use of the f
+000168d0: 696c 656e 616d 6520 6578 7465 6e73 696f  ilename extensio
+000168e0: 6e20 602e 6a73 6f6e 6e65 7460 2077 696c  n `.jsonnet` wil
+000168f0: 6c20 696e 766f 6b65 204a 736f 6e6e 6574  l invoke Jsonnet
+00016900: 2065 7661 6c75 6174 696f 6e2e 2028 4e6f   evaluation. (No
+00016910: 7465 2074 6861 7420 6120 7465 6d70 6f72  te that a tempor
+00016920: 6172 7920 4a53 4f4e 2066 696c 6520 6973  ary JSON file is
+00016930: 2063 7265 6174 6564 2061 7320 7061 7274   created as part
+00016940: 206f 6620 4a73 6f6e 6e65 7420 7072 6f63   of Jsonnet proc
+00016950: 6573 7369 6e67 2c20 7768 6963 6820 796f  essing, which yo
+00016960: 7520 6d61 7920 7365 6520 7265 6665 7272  u may see referr
+00016970: 6564 2074 6f20 696e 2065 7272 6f72 206d  ed to in error m
+00016980: 6573 7361 6765 733a 2074 6869 7320 6669  essages: this fi
+00016990: 6c65 2077 696c 6c20 6861 7665 2062 6565  le will have bee
+000169a0: 6e20 6465 6c65 7465 6420 6265 666f 7265  n deleted before
+000169b0: 2074 6865 2073 6372 6970 7420 7374 6f70   the script stop
+000169c0: 732e 290a 0a23 2320 4a73 6f6e 6e65 7420  s.)..## Jsonnet 
+000169d0: 496e 7374 616c 6c61 7469 6f6e 0a0a 4a73  Installation..Js
+000169e0: 6f6e 6e65 7420 6973 202a 2a6e 6f74 2a2a  onnet is **not**
+000169f0: 2069 6e73 7461 6c6c 6564 2062 7920 6465   installed by de
+00016a00: 6661 756c 7420 7768 656e 2060 7965 6c6c  fault when `yell
+00016a10: 6f77 646f 672d 7079 7468 6f6e 2d65 7861  owdog-python-exa
+00016a20: 6d70 6c65 7360 2069 7320 696e 7374 616c  mples` is instal
+00016a30: 6c65 642c 2062 6563 6175 7365 2074 6865  led, because the
+00016a40: 2070 6163 6b61 6765 2068 6173 2062 696e   package has bin
+00016a50: 6172 7920 636f 6d70 6f6e 656e 7473 2077  ary components w
+00016a60: 6869 6368 2061 7265 206e 6f74 2061 7661  hich are not ava
+00016a70: 696c 6162 6c65 206f 6e20 5079 5049 2066  ilable on PyPI f
+00016a80: 6f72 2061 6c6c 2070 6c61 7466 6f72 6d73  or all platforms
+00016a90: 2e20 4966 2079 6f75 2074 7279 2074 6f20  . If you try to 
+00016aa0: 7573 6520 6120 4a73 6f6e 6e65 7420 6669  use a Jsonnet fi
+00016ab0: 6c65 2069 6e20 7468 6520 6162 7365 6e63  le in the absenc
+00016ac0: 6520 6f66 204a 736f 6e6e 6574 2c20 7468  e of Jsonnet, th
+00016ad0: 6520 7363 7269 7074 7320 7769 6c6c 2070  e scripts will p
+00016ae0: 7269 6e74 2061 6e20 6572 726f 7220 6d65  rint an error me
+00016af0: 7373 6167 652c 2061 6e64 2073 7567 6765  ssage, and sugge
+00016b00: 7374 2061 6e20 696e 7374 616c 6c61 7469  st an installati
+00016b10: 6f6e 206d 6563 6861 6e69 736d 2e0a 0a54  on mechanism...T
+00016b20: 6f20 696e 7374 616c 6c20 4a73 6f6e 6e65  o install Jsonne
+00016b30: 7420 6174 2074 6865 2073 616d 6520 7469  t at the same ti
+00016b40: 6d65 2061 7320 696e 7374 616c 6c69 6e67  me as installing
+00016b50: 206f 7220 7570 6461 7469 6e67 2074 6865   or updating the
+00016b60: 2050 7974 686f 6e20 4578 616d 706c 6573   Python Examples
+00016b70: 2073 6372 6970 7473 2c20 6d6f 6469 6679   scripts, modify
+00016b80: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
+00016b90: 6e20 6173 2066 6f6c 6c6f 7773 2074 6f20  n as follows to 
+00016ba0: 696e 636c 7564 6520 7468 6520 606a 736f  include the `jso
+00016bb0: 6e6e 6574 6020 6f70 7469 6f6e 3a0a 0a60  nnet` option:..`
+00016bc0: 6060 0a70 6970 2069 6e73 7461 6c6c 202d  ``.pip install -
+00016bd0: 5520 2279 656c 6c6f 7764 6f67 2d70 7974  U "yellowdog-pyt
+00016be0: 686f 6e2d 6578 616d 706c 6573 5b6a 736f  hon-examples[jso
+00016bf0: 6e6e 6574 5d22 0a60 6060 0a0a 546f 2069  nnet]".```..To i
+00016c00: 6e73 7461 6c6c 204a 736f 6e6e 6574 2073  nstall Jsonnet s
+00016c10: 6570 6172 6174 656c 7920 6672 6f6d 2060  eparately from `
+00016c20: 7965 6c6c 6f77 646f 672d 7079 7468 6f6e  yellowdog-python
+00016c30: 2d65 7861 6d70 6c65 7360 2c20 7472 793a  -examples`, try:
+00016c40: 0a0a 6060 6073 6865 6c6c 0a70 6970 2069  ..```shell.pip i
+00016c50: 6e73 7461 6c6c 202d 5520 6a73 6f6e 6e65  nstall -U jsonne
+00016c60: 740a 6060 600a 0a49 6620 7468 6973 2066  t.```..If this f
+00016c70: 6169 6c73 2c20 7472 793a 0a0a 6060 6073  ails, try:..```s
+00016c80: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
+00016c90: 202d 5520 6a73 6f6e 6e65 742d 6269 6e61   -U jsonnet-bina
+00016ca0: 7279 0a60 6060 0a0a 4966 2062 6f74 6820  ry.```..If both 
+00016cb0: 6f66 2074 6865 7365 206d 6574 686f 6473  of these methods
+00016cc0: 2066 6169 6c2c 2079 6f75 276c 6c20 6e65   fail, you'll ne
+00016cd0: 6564 2074 6f20 656e 7375 7265 2074 6861  ed to ensure tha
+00016ce0: 7420 7468 6520 706c 6174 666f 726d 206f  t the platform o
+00016cf0: 6e20 7768 6963 6820 796f 7527 7265 2072  n which you're r
+00016d00: 756e 6e69 6e67 2068 6173 2074 6865 2072  unning has the r
+00016d10: 6571 7569 7265 6420 6275 696c 6420 746f  equired build to
+00016d20: 6f6c 7320 6176 6169 6c61 626c 652c 2073  ols available, s
+00016d30: 6f20 7468 6174 2074 6865 204a 736f 6e6e  o that the Jsonn
+00016d40: 6574 2062 696e 6172 7920 636f 6d70 6f6e  et binary compon
+00016d50: 656e 7473 2063 616e 2062 6520 6275 696c  ents can be buil
+00016d60: 7420 6c6f 6361 6c6c 792e 2054 6865 2072  t locally. The r
+00016d70: 6571 7569 7265 6420 6275 696c 6420 7061  equired build pa
+00016d80: 636b 6167 6573 2076 6172 7920 6279 2070  ckages vary by p
+00016d90: 6c61 7466 6f72 6d20 6275 7420 7573 7561  latform but usua
+00016da0: 6c6c 7920 696e 636c 7564 6520 6765 6e65  lly include gene
+00016db0: 7261 6c20 6465 7665 6c6f 706d 656e 7420  ral development 
+00016dc0: 746f 6f6c 7320 696e 636c 7564 696e 6720  tools including 
+00016dd0: 6120 432b 2b20 636f 6d70 696c 6572 2c20  a C++ compiler, 
+00016de0: 616e 6420 5079 7468 6f6e 2064 6576 656c  and Python devel
+00016df0: 6f70 6d65 6e74 2074 6f6f 6c73 2069 6e63  opment tools inc
+00016e00: 6c75 6469 6e67 2074 6865 2050 7974 686f  luding the Pytho
+00016e10: 6e20 6865 6164 6572 732e 0a0a 506c 6561  n headers...Plea
+00016e20: 7365 2067 6574 2069 6e20 746f 7563 6820  se get in touch 
+00016e30: 7769 7468 2059 656c 6c6f 7744 6f67 2069  with YellowDog i
+00016e40: 6620 796f 7520 6765 7420 7374 7563 6b2e  f you get stuck.
+00016e50: 0a0a 2323 2056 6172 6961 626c 6520 5375  ..## Variable Su
+00016e60: 6273 7469 7475 7469 6f6e 7320 696e 204a  bstitutions in J
+00016e70: 736f 6e6e 6574 2046 696c 6573 0a0a 5468  sonnet Files..Th
+00016e80: 6520 7363 7269 7074 7320 7072 6f76 6964  e scripts provid
+00016e90: 6520 6675 6c6c 2073 7570 706f 7274 2066  e full support f
+00016ea0: 6f72 2076 6172 6961 626c 6520 7375 6273  or variable subs
+00016eb0: 7469 7475 7469 6f6e 7320 696e 204a 736f  titutions in Jso
+00016ec0: 6e6e 6574 2066 696c 6573 2c20 7573 696e  nnet files, usin
+00016ed0: 6720 7468 6520 7361 6d65 2072 756c 6573  g the same rules
+00016ee0: 2061 7320 666f 7220 7468 6520 4a53 4f4e   as for the JSON
+00016ef0: 2073 7065 6369 6669 6361 7469 6f6e 732e   specifications.
+00016f00: 2052 656d 656d 6265 7220 7468 6174 2066   Remember that f
+00016f10: 6f72 202a 2a57 6f72 6b65 7220 506f 6f6c  or **Worker Pool
+00016f20: 2a2a 2073 7065 6369 6669 6361 7469 6f6e  ** specification
+00016f30: 732c 2076 6172 6961 626c 6520 7375 6273  s, variable subs
+00016f40: 7469 7475 7469 6f6e 7320 6d75 7374 2062  titutions must b
+00016f50: 6520 7072 6566 6978 6564 2062 7920 605f  e prefixed by `_
+00016f60: 5f60 2c20 652e 672e 2060 225f 5f7b 7b75  _`, e.g. `"__{{u
+00016f70: 7365 726e 616d 657d 7d7d 2260 2e0a 0a56  sername}}}"`...V
+00016f80: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
+00016f90: 7469 6f6e 2069 7320 7065 7266 6f72 6d65  tion is performe
+00016fa0: 6420 6265 666f 7265 204a 736f 6e6e 6574  d before Jsonnet
+00016fb0: 2065 7870 616e 7369 6f6e 2069 6e74 6f20   expansion into 
+00016fc0: 4a53 4f4e 2c20 616e 6420 6167 6169 6e20  JSON, and again 
+00016fd0: 6166 7465 7220 7468 6520 6578 7061 6e73  after the expans
+00016fe0: 696f 6e2e 0a0a 2323 2043 6865 636b 696e  ion...## Checkin
+00016ff0: 6720 4a73 6f6e 6e65 7420 5072 6f63 6573  g Jsonnet Proces
+00017000: 7369 6e67 0a0a 5468 6572 6520 6172 6520  sing..There are 
+00017010: 7468 7265 6520 706f 7373 6962 696c 6974  three possibilit
+00017020: 6965 7320 666f 7220 7665 7269 6679 696e  ies for verifyin
+00017030: 6720 7468 6174 2061 204a 736f 6e6e 6574  g that a Jsonnet
+00017040: 2073 7065 6369 6669 6361 7469 6f6e 2069   specification i
+00017050: 7320 646f 696e 6720 7768 6174 2069 7320  s doing what is 
+00017060: 696e 7465 6e64 6564 3a0a 0a31 2e20 546f  intended:..1. To
+00017070: 2069 6e73 7065 6374 2074 6865 2062 6173   inspect the bas
+00017080: 6963 2063 6f6e 7665 7273 696f 6e20 6f66  ic conversion of
+00017090: 204a 736f 6e6e 6574 2069 6e74 6f20 4a53   Jsonnet into JS
+000170a0: 4f4e 2c20 7769 7468 6f75 7420 616e 7920  ON, without any 
+000170b0: 6164 6469 7469 6f6e 616c 2070 726f 6365  additional proce
+000170c0: 7373 696e 6720 6279 2074 6865 2050 7974  ssing by the Pyt
+000170d0: 686f 6e20 4578 616d 706c 6573 2073 6372  hon Examples scr
+000170e0: 6970 7473 2c20 7468 6520 6079 642d 6a73  ipts, the `yd-js
+000170f0: 6f6e 6e65 7432 6a73 6f6e 6020 636f 6d6d  onnet2json` comm
+00017100: 616e 6420 6361 6e20 6265 2075 7365 642e  and can be used.
+00017110: 2054 6869 7320 7461 6b65 7320 6120 7369   This takes a si
+00017120: 6e67 6c65 2063 6f6d 6d61 6e64 206c 696e  ngle command lin
+00017130: 6520 6172 6775 6d65 6e74 2077 6869 6368  e argument which
+00017140: 2069 7320 7468 6520 6e61 6d65 206f 6620   is the name of 
+00017150: 7468 6520 6a73 6f6e 6e65 7420 6669 6c65  the jsonnet file
+00017160: 2074 6f20 6265 2070 726f 6365 7373 6564   to be processed
+00017170: 3a0a 0a60 6060 7368 656c 6c0a 7964 2d6a  :..```shell.yd-j
+00017180: 736f 6e6e 6574 326a 736f 6e20 6d79 5f66  sonnet2json my_f
+00017190: 696c 652e 6a73 6f6e 6e65 740a 6060 600a  ile.jsonnet.```.
+000171a0: 0a0a 322e 2054 6865 2060 6a73 6f6e 6e65  ..2. The `jsonne
+000171b0: 742d 6472 792d 7275 6e60 2028 602d 4a60  t-dry-run` (`-J`
+000171c0: 2920 6f70 7469 6f6e 206f 6620 7468 6520  ) option of the 
+000171d0: 6079 642d 7375 626d 6974 602c 2060 7964  `yd-submit`, `yd
+000171e0: 2d70 726f 7669 7369 6f6e 6020 616e 6420  -provision` and 
+000171f0: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
+00017200: 2063 6f6d 6d61 6e64 7320 7769 6c6c 2067   commands will g
+00017210: 656e 6572 6174 6520 4a53 4f4e 206f 7574  enerate JSON out
+00017220: 7075 7420 7265 7072 6573 656e 7469 6e67  put representing
+00017230: 2074 6865 204a 736f 6e6e 6574 2074 6f20   the Jsonnet to 
+00017240: 4a53 4f4e 2070 726f 6365 7373 696e 6720  JSON processing 
+00017250: 6f6e 6c79 2c20 696e 636c 7564 696e 6720  only, including 
+00017260: 6170 706c 6963 6162 6c65 2076 6172 6961  applicable varia
+00017270: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
+00017280: 732c 2062 7574 2062 6566 6f72 6520 6675  s, but before fu
+00017290: 6c6c 2070 726f 7065 7274 7920 6578 7061  ll property expa
+000172a0: 6e73 696f 6e20 696e 746f 2074 6865 204a  nsion into the J
+000172b0: 534f 4e20 7468 6174 2077 696c 6c20 6265  SON that will be
+000172c0: 2073 7562 6d69 7474 6564 2074 6f20 7468   submitted to th
+000172d0: 6520 506c 6174 666f 726d 2e0a 0a0a 332e  e Platform....3.
+000172e0: 2054 6865 2060 6472 792d 7275 6e60 2028   The `dry-run` (
+000172f0: 602d 4460 2920 6f70 7469 6f6e 2077 696c  `-D`) option wil
+00017300: 6c20 6765 6e65 7261 7465 204a 534f 4e20  l generate JSON 
+00017310: 6f75 7470 7574 2072 6570 7265 7365 6e74  output represent
+00017320: 696e 6720 7468 6520 6675 6c6c 2070 726f  ing the full pro
+00017330: 6365 7373 696e 6720 6f66 2074 6865 204a  cessing of the J
+00017340: 736f 6e6e 6574 2066 696c 6520 696e 746f  sonnet file into
+00017350: 2077 6861 7420 7769 6c6c 2062 6520 7375   what will be su
+00017360: 626d 6974 7465 6420 746f 2074 6865 2041  bmitted to the A
+00017370: 5049 2e20 5468 6973 2061 6c6c 6f77 7320  PI. This allows 
+00017380: 696e 7370 6563 7469 6f6e 2074 6f20 6368  inspection to ch
+00017390: 6563 6b20 7468 6174 2074 6865 206f 7574  eck that the out
+000173a0: 7075 7420 6d61 7463 6865 7320 6578 7065  put matches expe
+000173b0: 6374 6174 696f 6e73 2c20 7072 696f 7220  ctations, prior 
+000173c0: 746f 2073 7562 6d69 7474 696e 6720 746f  to submitting to
+000173d0: 2074 6865 2050 6c61 7466 6f72 6d2e 0a0a   the Platform...
+000173e0: 2323 204a 736f 6e6e 6574 2045 7861 6d70  ## Jsonnet Examp
+000173f0: 6c65 0a0a 4865 7265 2773 2061 6e20 6578  le..Here's an ex
+00017400: 616d 706c 6520 6f66 2061 204a 736f 6e6e  ample of a Jsonn
+00017410: 6574 2066 696c 6520 7468 6174 2067 656e  et file that gen
+00017420: 6572 6174 6573 2061 2057 6f72 6b20 5265  erates a Work Re
+00017430: 7175 6972 656d 656e 7420 7769 7468 2066  quirement with f
+00017440: 6f75 7220 5461 736b 733a 0a0a 6060 606a  our Tasks:..```j
+00017450: 736f 6e6e 6574 0a23 2046 756e 6374 696f  sonnet.# Functio
+00017460: 6e20 666f 7220 7379 6e74 6865 7369 7369  n for synthesisi
+00017470: 6e67 2054 6173 6b73 0a6c 6f63 616c 2054  ng Tasks.local T
+00017480: 6173 6b28 6172 6775 6d65 6e74 733d 5b5d  ask(arguments=[]
+00017490: 2c20 656e 7669 726f 6e6d 656e 743d 7b7d  , environment={}
+000174a0: 2920 3d20 7b0a 2020 2020 6172 6775 6d65  ) = {.    argume
+000174b0: 6e74 733a 2061 7267 756d 656e 7473 2c0a  nts: arguments,.
+000174c0: 2020 2020 656e 7669 726f 6e6d 656e 743a      environment:
+000174d0: 2065 6e76 6972 6f6e 6d65 6e74 2c0a 2020   environment,.  
+000174e0: 2020 6e61 6d65 3a20 226d 795f 7461 736b    name: "my_task
+000174f0: 5f7b 7b74 6173 6b5f 6e75 6d62 6572 7d7d  _{{task_number}}
+00017500: 220a 7d3b 0a0a 2320 576f 726b 2052 6571  ".};..# Work Req
+00017510: 7569 7265 6d65 6e74 0a7b 0a20 2022 6e61  uirement.{.  "na
+00017520: 6d65 223a 2022 776f 726b 7265 715f 7b7b  me": "workreq_{{
+00017530: 6461 7465 7469 6d65 7d7d 222c 0a20 2022  datetime}}",.  "
+00017540: 7461 736b 4772 6f75 7073 223a 205b 0a20  taskGroups": [. 
+00017550: 2020 207b 0a20 2020 2020 2022 7461 736b     {.      "task
+00017560: 7322 3a20 5b0a 2020 2020 2020 2020 5461  s": [.        Ta
+00017570: 736b 285b 2231 225d 2c20 7b41 3a20 2241  sk(["1"], {A: "A
+00017580: 5f31 227d 292c 2020 2320 6172 6775 6d65  _1"}),  # argume
+00017590: 6e74 7320 616e 6420 656e 7669 726f 6e6d  nts and environm
+000175a0: 656e 740a 2020 2020 2020 2020 5461 736b  ent.        Task
+000175b0: 285b 2232 222c 2022 3322 5d2c 207b 7d29  (["2", "3"], {})
+000175c0: 2c20 2020 2020 2320 6172 6775 6d65 6e74  ,     # argument
+000175d0: 7320 616e 6420 656d 7074 7920 656e 7669  s and empty envi
+000175e0: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
+000175f0: 5461 736b 285b 2234 225d 292c 2020 2020  Task(["4"]),    
+00017600: 2020 2020 2020 2020 2020 2320 6172 6775            # argu
+00017610: 6d65 6e74 7320 616e 6420 6465 6661 756c  ments and defaul
+00017620: 7420 656e 7669 726f 6e6d 656e 740a 2020  t environment.  
+00017630: 2020 2020 2020 5461 736b 2829 2020 2020        Task()    
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 2320 6465 6661 756c 7420 6172 6775 6d65  # default argume
+00017660: 6e74 7320 616e 6420 656e 7669 726f 6e6d  nts and environm
+00017670: 656e 740a 2020 2020 2020 5d0a 2020 2020  ent.      ].    
+00017680: 7d0a 2020 5d0a 7d0a 6060 600a 0a57 6865  }.  ].}.```..Whe
+00017690: 6e20 7468 6973 2069 7320 696e 7370 6563  n this is inspec
+000176a0: 7465 6420 7573 696e 6720 7468 6520 606a  ted using the `j
+000176b0: 736f 6e6e 6574 2d64 7279 2d72 756e 6020  sonnet-dry-run` 
+000176c0: 6f70 7469 6f6e 2028 6079 642d 7375 626d  option (`yd-subm
+000176d0: 6974 202d 4a71 202d 7220 6d79 5f77 6f72  it -Jq -r my_wor
+000176e0: 6b5f 7265 712e 6a73 6f6e 6e65 7460 292c  k_req.jsonnet`),
+000176f0: 2074 6869 7320 6973 2074 6865 2070 726f   this is the pro
+00017700: 6365 7373 6564 206f 7574 7075 743a 0a0a  cessed output:..
+00017710: 6060 606a 736f 6e0a 7b0a 2020 226e 616d  ```json.{.  "nam
+00017720: 6522 3a20 2277 6f72 6b72 6571 5f32 3330  e": "workreq_230
+00017730: 3131 342d 3134 3036 3435 222c 0a20 2022  114-140645",.  "
+00017740: 7461 736b 4772 6f75 7073 223a 205b 0a20  taskGroups": [. 
+00017750: 2020 207b 0a20 2020 2020 2022 7461 736b     {.      "task
+00017760: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
+00017770: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
+00017780: 656e 7473 223a 205b 2231 225d 2c0a 2020  ents": ["1"],.  
+00017790: 2020 2020 2020 2020 2265 6e76 6972 6f6e          "environ
+000177a0: 6d65 6e74 223a 207b 2241 223a 2022 415f  ment": {"A": "A_
+000177b0: 3122 7d2c 0a20 2020 2020 2020 2020 2022  1"},.          "
+000177c0: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
+000177d0: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
+000177e0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000177f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00017800: 2261 7267 756d 656e 7473 223a 205b 2232  "arguments": ["2
+00017810: 222c 2022 3322 5d2c 0a20 2020 2020 2020  ", "3"],.       
+00017820: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
+00017830: 3a20 7b7d 2c0a 2020 2020 2020 2020 2020  : {},.          
+00017840: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
+00017850: 5f7b 7b74 6173 6b5f 6e75 6d62 6572 7d7d  _{{task_number}}
+00017860: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00017870: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00017880: 2022 6172 6775 6d65 6e74 7322 3a20 5b22   "arguments": ["
+00017890: 3422 5d2c 0a20 2020 2020 2020 2020 2022  4"],.          "
+000178a0: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
+000178b0: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
+000178c0: 6522 3a20 226d 795f 7461 736b 5f7b 7b74  e": "my_task_{{t
+000178d0: 6173 6b5f 6e75 6d62 6572 7d7d 220a 2020  ask_number}}".  
+000178e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000178f0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+00017900: 6775 6d65 6e74 7322 3a20 5b5d 2c0a 2020  guments": [],.  
+00017910: 2020 2020 2020 2020 2265 6e76 6972 6f6e          "environ
+00017920: 6d65 6e74 223a 207b 7d2c 0a20 2020 2020  ment": {},.     
+00017930: 2020 2020 2022 6e61 6d65 223a 2022 6d79       "name": "my
+00017940: 5f74 6173 6b5f 7b7b 7461 736b 5f6e 756d  _task_{{task_num
+00017950: 6265 727d 7d22 0a20 2020 2020 2020 207d  ber}}".        }
+00017960: 0a20 2020 2020 205d 0a20 2020 207d 0a20  .      ].    }. 
+00017970: 205d 0a7d 0a60 6060 0a0a 5768 656e 2074   ].}.```..When t
+00017980: 6869 7320 6973 2069 6e73 7065 6374 6564  his is inspected
+00017990: 2075 7369 6e67 2074 6865 2060 6472 792d   using the `dry-
+000179a0: 7275 6e60 206f 7074 696f 6e20 2860 7964  run` option (`yd
+000179b0: 2d73 7562 6d69 7420 2d44 7120 2d72 206d  -submit -Dq -r m
+000179c0: 795f 776f 726b 5f72 6571 2e6a 736f 6e6e  y_work_req.jsonn
+000179d0: 6574 6029 2c20 7468 6973 2069 7320 7468  et`), this is th
+000179e0: 6520 7072 6f63 6573 7365 6420 6f75 7470  e processed outp
+000179f0: 7574 3a0a 0a60 6060 6a73 6f6e 0a7b 0a20  ut:..```json.{. 
+00017a00: 2022 6675 6c66 696c 4f6e 5375 626d 6974   "fulfilOnSubmit
+00017a10: 223a 2066 616c 7365 2c0a 2020 226e 616d  ": false,.  "nam
+00017a20: 6522 3a20 2277 6f72 6b72 6571 5f32 3330  e": "workreq_230
+00017a30: 3131 342d 3134 3036 3435 222c 0a20 2022  114-140645",.  "
+00017a40: 6e61 6d65 7370 6163 6522 3a20 2270 7965  namespace": "pye
+00017a50: 7861 6d70 6c65 7322 2c0a 2020 2270 7269  xamples",.  "pri
+00017a60: 6f72 6974 7922 3a20 302c 0a20 2022 7461  ority": 0,.  "ta
+00017a70: 6722 3a20 2270 7965 782d 6261 7368 222c  g": "pyex-bash",
+00017a80: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+00017a90: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+00017aa0: 6669 6e69 7368 4966 416c 6c54 6173 6b73  finishIfAllTasks
+00017ab0: 4669 6e69 7368 6564 223a 2074 7275 652c  Finished": true,
+00017ac0: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
+00017ad0: 416e 7954 6173 6b46 6169 6c65 6422 3a20  AnyTaskFailed": 
+00017ae0: 6661 6c73 652c 0a20 2020 2020 2022 6e61  false,.      "na
+00017af0: 6d65 223a 2022 7461 736b 5f67 726f 7570  me": "task_group
+00017b00: 5f31 222c 0a20 2020 2020 2022 7072 696f  _1",.      "prio
+00017b10: 7269 7479 223a 2030 2c0a 2020 2020 2020  rity": 0,.      
+00017b20: 2272 756e 5370 6563 6966 6963 6174 696f  "runSpecificatio
+00017b30: 6e22 3a20 7b0a 2020 2020 2020 2020 226d  n": {.        "m
+00017b40: 6178 696d 756d 5461 736b 5265 7472 6965  aximumTaskRetrie
+00017b50: 7322 3a20 302c 0a20 2020 2020 2020 2022  s": 0,.        "
+00017b60: 7461 736b 5479 7065 7322 3a20 5b22 6261  taskTypes": ["ba
+00017b70: 7368 225d 2c0a 2020 2020 2020 2020 2277  sh"],.        "w
+00017b80: 6f72 6b65 7254 6167 7322 3a20 5b22 7079  orkerTags": ["py
+00017b90: 6578 2d62 6173 682d 646f 636b 6572 225d  ex-bash-docker"]
+00017ba0: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
+00017bb0: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
+00017bc0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00017bd0: 6172 6775 6d65 6e74 7322 3a20 5b22 776f  arguments": ["wo
+00017be0: 726b 7265 715f 3233 3031 3134 2d31 3430  rkreq_230114-140
+00017bf0: 3634 352f 736c 6565 705f 7363 7269 7074  645/sleep_script
+00017c00: 2e73 6822 2c20 2231 225d 2c0a 2020 2020  .sh", "1"],.    
+00017c10: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
+00017c20: 6e74 223a 207b 2241 223a 2022 415f 3122  nt": {"A": "A_1"
+00017c30: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
+00017c40: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+00017c50: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00017c60: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
+00017c70: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
+00017c80: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
+00017c90: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
+00017ca0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017cb0: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
+00017cc0: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
+00017cd0: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
+00017ce0: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
+00017cf0: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
+00017d00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00017d10: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017d20: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
+00017d30: 736b 5f31 222c 0a20 2020 2020 2020 2020  sk_1",.         
+00017d40: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
+00017d50: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
+00017d60: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
+00017d70: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+00017d80: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
+00017d90: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
+00017da0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00017db0: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+00017dc0: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
+00017dd0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00017de0: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+00017df0: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
+00017e00: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
+00017e10: 6565 705f 7363 7269 7074 2e73 6822 2c20  eep_script.sh", 
+00017e20: 2232 222c 2022 3322 5d2c 0a20 2020 2020  "2", "3"],.     
+00017e30: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+00017e40: 7422 3a20 7b7d 2c0a 2020 2020 2020 2020  t": {},.        
+00017e50: 2020 2269 6e70 7574 7322 3a20 5b0a 2020    "inputs": [.  
+00017e60: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00017e70: 2020 2020 2020 2020 2020 226f 626a 6563            "objec
+00017e80: 744e 616d 6550 6174 7465 726e 223a 2022  tNamePattern": "
+00017e90: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
+00017ea0: 3430 3634 352f 736c 6565 705f 7363 7269  40645/sleep_scri
+00017eb0: 7074 2e73 6822 2c0a 2020 2020 2020 2020  pt.sh",.        
+00017ec0: 2020 2020 2020 2273 6f75 7263 6522 3a20        "source": 
+00017ed0: 2254 4153 4b5f 4e41 4d45 5350 4143 4522  "TASK_NAMESPACE"
+00017ee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017ef0: 2276 6572 6966 6963 6174 696f 6e22 3a20  "verification": 
+00017f00: 2256 4552 4946 595f 4154 5f53 5441 5254  "VERIFY_AT_START
+00017f10: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00017f20: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00017f30: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00017f40: 6d79 5f74 6173 6b5f 3222 2c0a 2020 2020  my_task_2",.    
+00017f50: 2020 2020 2020 226f 7574 7075 7473 223a        "outputs":
+00017f60: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
+00017f70: 2261 6c77 6179 7355 706c 6f61 6422 3a20  "alwaysUpload": 
+00017f80: 7472 7565 2c20 2272 6571 7569 7265 6422  true, "required"
+00017f90: 3a20 6661 6c73 652c 2022 736f 7572 6365  : false, "source
+00017fa0: 223a 2022 5052 4f43 4553 535f 4f55 5450  ": "PROCESS_OUTP
+00017fb0: 5554 227d 0a20 2020 2020 2020 2020 205d  UT"}.          ]
+00017fc0: 2c0a 2020 2020 2020 2020 2020 2274 6173  ,.          "tas
+00017fd0: 6b54 7970 6522 3a20 2262 6173 6822 0a20  kType": "bash". 
+00017fe0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00017ff0: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00018000: 7267 756d 656e 7473 223a 205b 2277 6f72  rguments": ["wor
+00018010: 6b72 6571 5f32 3330 3131 342d 3134 3036  kreq_230114-1406
+00018020: 3435 2f73 6c65 6570 5f73 6372 6970 742e  45/sleep_script.
+00018030: 7368 222c 2022 3422 5d2c 0a20 2020 2020  sh", "4"],.     
+00018040: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+00018050: 7422 3a20 7b7d 2c0a 2020 2020 2020 2020  t": {},.        
+00018060: 2020 2269 6e70 7574 7322 3a20 5b0a 2020    "inputs": [.  
+00018070: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00018080: 2020 2020 2020 2020 2020 226f 626a 6563            "objec
+00018090: 744e 616d 6550 6174 7465 726e 223a 2022  tNamePattern": "
+000180a0: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
+000180b0: 3430 3634 352f 736c 6565 705f 7363 7269  40645/sleep_scri
+000180c0: 7074 2e73 6822 2c0a 2020 2020 2020 2020  pt.sh",.        
+000180d0: 2020 2020 2020 2273 6f75 7263 6522 3a20        "source": 
+000180e0: 2254 4153 4b5f 4e41 4d45 5350 4143 4522  "TASK_NAMESPACE"
+000180f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018100: 2276 6572 6966 6963 6174 696f 6e22 3a20  "verification": 
+00018110: 2256 4552 4946 595f 4154 5f53 5441 5254  "VERIFY_AT_START
+00018120: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00018130: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00018140: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00018150: 6d79 5f74 6173 6b5f 3322 2c0a 2020 2020  my_task_3",.    
+00018160: 2020 2020 2020 226f 7574 7075 7473 223a        "outputs":
+00018170: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
+00018180: 2261 6c77 6179 7355 706c 6f61 6422 3a20  "alwaysUpload": 
+00018190: 7472 7565 2c20 2272 6571 7569 7265 6422  true, "required"
+000181a0: 3a20 6661 6c73 652c 2022 736f 7572 6365  : false, "source
+000181b0: 223a 2022 5052 4f43 4553 535f 4f55 5450  ": "PROCESS_OUTP
+000181c0: 5554 227d 0a20 2020 2020 2020 2020 205d  UT"}.          ]
+000181d0: 2c0a 2020 2020 2020 2020 2020 2274 6173  ,.          "tas
+000181e0: 6b54 7970 6522 3a20 2262 6173 6822 0a20  kType": "bash". 
+000181f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00018200: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00018210: 7267 756d 656e 7473 223a 205b 2277 6f72  rguments": ["wor
+00018220: 6b72 6571 5f32 3330 3131 342d 3134 3036  kreq_230114-1406
+00018230: 3435 2f73 6c65 6570 5f73 6372 6970 742e  45/sleep_script.
+00018240: 7368 225d 2c0a 2020 2020 2020 2020 2020  sh"],.          
+00018250: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00018260: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
+00018270: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+00018280: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00018290: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
+000182a0: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
+000182b0: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
+000182c0: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
+000182d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000182e0: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
+000182f0: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
+00018300: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
+00018310: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
+00018320: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
+00018330: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00018340: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00018350: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
+00018360: 736b 5f34 222c 0a20 2020 2020 2020 2020  sk_4",.         
+00018370: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
+00018380: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
+00018390: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
+000183a0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+000183b0: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
+000183c0: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
+000183d0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+000183e0: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+000183f0: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
+00018400: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00018410: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2043  }.  ].}.```..# C
+00018420: 6f6d 6d61 6e64 204c 6973 740a 0a48 656c  ommand List..Hel
+00018430: 7020 6973 2061 7661 696c 6162 6c65 2066  p is available f
+00018440: 6f72 2061 6c6c 2063 6f6d 6d61 6e64 7320  or all commands 
+00018450: 6279 2069 6e76 6f6b 696e 6720 6120 636f  by invoking a co
+00018460: 6d6d 616e 6420 7769 7468 2074 6865 2060  mmand with the `
+00018470: 2d2d 6865 6c70 6020 6f72 2060 2d68 6020  --help` or `-h` 
+00018480: 6f70 7469 6f6e 2e20 536f 6d65 2063 6f6d  option. Some com
+00018490: 6d61 6e64 206c 696e 6520 7061 7261 6d65  mand line parame
+000184a0: 7465 7273 2061 7265 2063 6f6d 6d6f 6e20  ters are common 
+000184b0: 746f 2061 6c6c 2063 6f6d 6d61 6e64 732c  to all commands,
+000184c0: 2077 6869 6c65 206f 7468 6572 7320 6172   while others ar
+000184d0: 6520 636f 6d6d 616e 642d 7370 6563 6966  e command-specif
+000184e0: 6963 2e0a 0a41 6c6c 2064 6573 7472 7563  ic...All destruc
+000184f0: 7469 7665 2063 6f6d 6d61 6e64 7320 7265  tive commands re
+00018500: 7175 6972 6520 7573 6572 2063 6f6e 6669  quire user confi
+00018510: 726d 6174 696f 6e20 6265 666f 7265 2074  rmation before t
+00018520: 616b 696e 6720 6566 6665 6374 2e20 5468  aking effect. Th
+00018530: 6973 2063 616e 2062 6520 7375 7070 7265  is can be suppre
+00018540: 7373 6564 2075 7369 6e67 2074 6865 2060  ssed using the `
+00018550: 2d2d 7965 7360 206f 7220 602d 7960 206f  --yes` or `-y` o
+00018560: 7074 696f 6e2c 2069 6e20 7768 6963 6820  ption, in which 
+00018570: 6361 7365 2074 6865 2063 6f6d 6d61 6e64  case the command
+00018580: 2077 696c 6c20 7072 6f63 6565 6420 7769   will proceed wi
+00018590: 7468 6f75 7420 636f 6e66 6972 6d61 7469  thout confirmati
+000185a0: 6f6e 2e0a 0a53 6f6d 6520 636f 6d6d 616e  on...Some comman
+000185b0: 6473 2073 7570 706f 7274 2074 6865 2060  ds support the `
+000185c0: 2d2d 696e 7465 7261 6374 6976 6560 206f  --interactive` o
+000185d0: 7220 602d 6960 206f 7074 696f 6e2c 2061  r `-i` option, a
+000185e0: 6c6c 6f77 696e 6720 7573 6572 2073 656c  llowing user sel
+000185f0: 6563 7469 6f6e 7320 746f 2062 6520 6d61  ections to be ma
+00018600: 6465 2e20 452e 672e 2c20 7468 6973 2063  de. E.g., this c
+00018610: 616e 2062 6520 7573 6564 2074 6f20 7365  an be used to se
+00018620: 6c65 6374 2077 6869 6368 206f 626a 6563  lect which objec
+00018630: 7420 7061 7468 7320 746f 2064 656c 6574  t paths to delet
+00018640: 652e 0a0a 5468 6520 602d 2d71 7569 6574  e...The `--quiet
+00018650: 6020 6f72 2060 2d71 6020 6f70 7469 6f6e  ` or `-q` option
+00018660: 2072 6564 7563 6573 2074 6865 2063 6f6d   reduces the com
+00018670: 6d61 6e64 206f 7574 7075 7420 646f 776e  mand output down
+00018680: 2074 6f20 6573 7365 6e74 6961 6c20 6d65   to essential me
+00018690: 7373 6167 6573 206f 6e6c 792e 2053 6f2c  ssages only. So,
+000186a0: 2066 6f72 2065 7861 6d70 6c65 2c20 6079   for example, `y
+000186b0: 642d 6465 6c65 7465 202d 7971 6020 776f  d-delete -yq` wo
+000186c0: 756c 6420 6465 6c65 7465 2061 6c6c 206d  uld delete all m
+000186d0: 6174 6368 696e 6720 6f62 6a65 6374 2070  atching object p
+000186e0: 6174 6873 2073 696c 656e 746c 792e 0a0a  aths silently...
+000186f0: 4966 2079 6f75 2065 6e63 6f75 6e74 6572  If you encounter
+00018700: 2061 6e20 6572 726f 7220 6974 2063 616e   an error it can
+00018710: 2062 6520 7573 6566 756c 2066 6f72 2073   be useful for s
+00018720: 7570 706f 7274 2070 7572 706f 7365 7320  upport purposes 
+00018730: 746f 2073 6565 2074 6865 2066 756c 6c20  to see the full 
+00018740: 5079 7468 6f6e 2073 7461 636b 2074 7261  Python stack tra
+00018750: 6365 2e20 5468 6973 2063 616e 2062 6520  ce. This can be 
+00018760: 656e 6162 6c65 6420 6279 2072 756e 6e69  enabled by runni
+00018770: 6e67 2074 6865 2063 6f6d 6d61 6e64 2075  ng the command u
+00018780: 7369 6e67 2074 6865 2060 2d2d 6465 6275  sing the `--debu
+00018790: 6760 206f 7074 696f 6e2e 0a0a 2323 2079  g` option...## y
+000187a0: 642d 7375 626d 6974 0a0a 5468 6520 6079  d-submit..The `y
+000187b0: 642d 7375 626d 6974 6020 636f 6d6d 616e  d-submit` comman
+000187c0: 6420 7375 626d 6974 7320 6120 6e65 7720  d submits a new 
+000187d0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+000187e0: 2c20 6163 636f 7264 696e 6720 746f 2074  , according to t
+000187f0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+00018800: 656e 7420 6465 6669 6e69 7469 6f6e 2066  ent definition f
+00018810: 6f75 6e64 2069 6e20 7468 6520 6077 6f72  ound in the `wor
+00018820: 6b52 6571 7569 7265 6d65 6e74 6020 7365  kRequirement` se
+00018830: 6374 696f 6e20 6f66 2074 6865 2054 4f4d  ction of the TOM
+00018840: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+00018850: 6669 6c65 2061 6e64 2f6f 7220 7468 6520  file and/or the 
+00018860: 7370 6563 6966 6963 6174 696f 6e20 666f  specification fo
+00018870: 756e 6420 696e 2061 2057 6f72 6b20 5265  und in a Work Re
+00018880: 7175 6972 656d 656e 7420 4a53 4f4e 2064  quirement JSON d
+00018890: 6f63 756d 656e 7420 7375 7070 6c69 6564  ocument supplied
+000188a0: 2075 7369 6e67 2074 6865 2060 2d2d 776f   using the `--wo
+000188b0: 726b 2d72 6571 7569 7265 6d65 6e74 6020  rk-requirement` 
+000188c0: 6f70 7469 6f6e 2e0a 0a55 7365 2074 6865  option...Use the
+000188d0: 2060 2d2d 6472 792d 7275 6e60 206f 7074   `--dry-run` opt
+000188e0: 696f 6e20 746f 2069 6e73 7065 6374 2074  ion to inspect t
+000188f0: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
+00018900: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+00018910: 6e74 2c20 5461 736b 2047 726f 7570 732c  nt, Task Groups,
+00018920: 2061 6e64 2054 6173 6b73 2074 6861 7420   and Tasks that 
+00018930: 7769 6c6c 2062 6520 7375 626d 6974 7465  will be submitte
+00018940: 642c 2069 6e20 4a53 4f4e 2066 6f72 6d61  d, in JSON forma
+00018950: 742e 0a0a 4f6e 6365 2073 7562 6d69 7474  t...Once submitt
+00018960: 6564 2c20 7468 6520 576f 726b 2052 6571  ed, the Work Req
+00018970: 7569 7265 6d65 6e74 2077 696c 6c20 6170  uirement will ap
+00018980: 7065 6172 2069 6e20 7468 6520 2a2a 576f  pear in the **Wo
+00018990: 726b 2a2a 2074 6162 2069 6e20 7468 6520  rk** tab in the 
+000189a0: 5965 6c6c 6f77 446f 6720 506f 7274 616c  YellowDog Portal
+000189b0: 2e0a 0a54 6865 2057 6f72 6b20 5265 7175  ...The Work Requ
+000189c0: 6972 656d 656e 7427 7320 7072 6f67 7265  irement's progre
+000189d0: 7373 2063 616e 2062 6520 7472 6163 6b65  ss can be tracke
+000189e0: 6420 746f 2063 6f6d 706c 6574 696f 6e20  d to completion 
+000189f0: 6279 2075 7369 6e67 2074 6865 2060 2d2d  by using the `--
+00018a00: 666f 6c6c 6f77 6020 286f 7220 602d 6660  follow` (or `-f`
+00018a10: 2920 6f70 7469 6f6e 2077 6865 6e20 696e  ) option when in
+00018a20: 766f 6b69 6e67 2060 7964 2d73 7562 6d69  voking `yd-submi
+00018a30: 7460 3a20 7468 6520 636f 6d6d 616e 6420  t`: the command 
+00018a40: 7769 6c6c 2072 6570 6f72 7420 6f6e 2054  will report on T
+00018a50: 6173 6b73 2061 7320 7468 6579 2063 6f6e  asks as they con
+00018a60: 636c 7564 6520 616e 6420 776f 6e27 7420  clude and won't 
+00018a70: 7265 7475 726e 2075 6e74 696c 2074 6865  return until the
+00018a80: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00018a90: 7420 6861 7320 6669 6e69 7368 6564 2e0a  t has finished..
+00018aa0: 0a23 2320 7964 2d70 726f 7669 7369 6f6e  .## yd-provision
+00018ab0: 0a0a 5468 6520 6079 642d 7072 6f76 6973  ..The `yd-provis
+00018ac0: 696f 6e60 2063 6f6d 6d61 6e64 2070 726f  ion` command pro
+00018ad0: 7669 7369 6f6e 7320 6120 6e65 7720 576f  visions a new Wo
+00018ae0: 726b 6572 2050 6f6f 6c20 6163 636f 7264  rker Pool accord
+00018af0: 696e 6720 746f 2074 6865 2073 7065 6369  ing to the speci
+00018b00: 6669 6361 7469 6f6e 7320 696e 2074 6865  fications in the
+00018b10: 2060 776f 726b 6572 506f 6f6c 6020 7365   `workerPool` se
+00018b20: 6374 696f 6e20 6f66 2074 6865 2054 4f4d  ction of the TOM
+00018b30: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+00018b40: 6669 6c65 2061 6e64 2f6f 7220 696e 2074  file and/or in t
+00018b50: 6865 2073 7065 6369 6669 6361 7469 6f6e  he specification
+00018b60: 2066 6f75 6e64 2069 6e20 6120 576f 726b   found in a Work
+00018b70: 6572 2050 6f6f 6c20 4a53 4f4e 2064 6f63  er Pool JSON doc
+00018b80: 756d 656e 7420 7375 7070 6c69 6564 2075  ument supplied u
+00018b90: 7369 6e67 2074 6865 2060 2d2d 776f 726b  sing the `--work
+00018ba0: 6572 2d70 6f6f 6c60 206f 7074 696f 6e2e  er-pool` option.
+00018bb0: 0a0a 5573 6520 7468 6520 602d 2d64 7279  ..Use the `--dry
+00018bc0: 2d72 756e 6020 6f70 7469 6f6e 2074 6f20  -run` option to 
+00018bd0: 696e 7370 6563 7420 7468 6520 6465 7461  inspect the deta
+00018be0: 696c 7320 6f66 2074 6865 2057 6f72 6b65  ils of the Worke
+00018bf0: 7220 506f 6f6c 2073 7065 6369 6669 6361  r Pool specifica
+00018c00: 7469 6f6e 2074 6861 7420 7769 6c6c 2062  tion that will b
+00018c10: 6520 7375 626d 6974 7465 642c 2069 6e20  e submitted, in 
+00018c20: 4a53 4f4e 2066 6f72 6d61 742e 0a0a 4f6e  JSON format...On
+00018c30: 6365 2070 726f 7669 7369 6f6e 6564 2c20  ce provisioned, 
+00018c40: 7468 6520 576f 726b 6572 2050 6f6f 6c20  the Worker Pool 
+00018c50: 7769 6c6c 2061 7070 6561 7220 696e 2074  will appear in t
+00018c60: 6865 202a 2a57 6f72 6b65 7273 2a2a 2074  he **Workers** t
+00018c70: 6162 2069 6e20 7468 6520 5965 6c6c 6f77  ab in the Yellow
+00018c80: 446f 6720 506f 7274 616c 2c20 616e 6420  Dog Portal, and 
+00018c90: 6974 7320 6173 736f 6369 6174 6564 2043  its associated C
+00018ca0: 6f6d 7075 7465 2052 6571 7569 7265 6d65  ompute Requireme
+00018cb0: 6e74 2077 696c 6c20 6170 7065 6172 2069  nt will appear i
+00018cc0: 6e20 7468 6520 2a2a 436f 6d70 7574 652a  n the **Compute*
+00018cd0: 2a20 7461 622e 0a0a 2323 2079 642d 6361  * tab...## yd-ca
+00018ce0: 6e63 656c 0a0a 5468 6520 6079 642d 6361  ncel..The `yd-ca
+00018cf0: 6e63 656c 6020 636f 6d6d 616e 6420 6361  ncel` command ca
+00018d00: 6e63 656c 7320 616e 7920 6163 7469 7665  ncels any active
+00018d10: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00018d20: 7473 2c20 696e 636c 7564 696e 6720 616e  ts, including an
+00018d30: 7920 7065 6e64 696e 6720 5461 736b 2047  y pending Task G
+00018d40: 726f 7570 7320 616e 6420 7468 6520 5461  roups and the Ta
+00018d50: 736b 7320 7468 6579 2063 6f6e 7461 696e  sks they contain
+00018d60: 2e20 0a0a 5468 6520 606e 616d 6573 7061  . ..The `namespa
+00018d70: 6365 6020 616e 6420 6074 6167 6020 7661  ce` and `tag` va
+00018d80: 6c75 6573 2069 6e20 7468 6520 6063 6f6e  lues in the `con
+00018d90: 6669 672e 746f 6d6c 6020 6669 6c65 2061  fig.toml` file a
+00018da0: 7265 2075 7365 6420 746f 2069 6465 6e74  re used to ident
+00018db0: 6966 7920 7768 6963 6820 576f 726b 2052  ify which Work R
+00018dc0: 6571 7569 7265 6d65 6e74 7320 746f 2063  equirements to c
+00018dd0: 616e 6365 6c2e 0a0a 4279 2064 6566 6175  ancel...By defau
+00018de0: 6c74 2c20 616e 7920 5461 736b 7320 7468  lt, any Tasks th
+00018df0: 6174 2061 7265 2063 7572 7265 6e74 6c79  at are currently
+00018e00: 2072 756e 6e69 6e67 206f 6e20 576f 726b   running on Work
+00018e10: 6572 7320 7769 6c6c 2063 6f6e 7469 6e75  ers will continu
+00018e20: 6520 746f 2072 756e 2074 6f20 636f 6d70  e to run to comp
+00018e30: 6c65 7469 6f6e 206f 7220 756e 7469 6c20  letion or until 
+00018e40: 7468 6579 2066 6169 6c2e 2054 6173 6b73  they fail. Tasks
+00018e50: 2063 616e 2062 6520 696e 7374 7275 6374   can be instruct
+00018e60: 6564 2074 6f20 6162 6f72 7420 696d 6d65  ed to abort imme
+00018e70: 6469 6174 656c 7920 6279 2073 7570 706c  diately by suppl
+00018e80: 7969 6e67 2074 6865 2060 2d2d 6162 6f72  ying the `--abor
+00018e90: 7460 206f 7220 602d 6160 206f 7074 696f  t` or `-a` optio
+00018ea0: 6e20 746f 2060 7964 2d63 616e 6365 6c60  n to `yd-cancel`
+00018eb0: 2e0a 0a23 2320 7964 2d61 626f 7274 0a0a  ...## yd-abort..
+00018ec0: 5468 6520 6079 642d 6162 6f72 7460 2063  The `yd-abort` c
+00018ed0: 6f6d 6d61 6e64 2069 7320 7573 6564 2074  ommand is used t
+00018ee0: 6f20 6162 6f72 7420 5461 736b 7320 7468  o abort Tasks th
+00018ef0: 6174 2061 7265 2063 7572 7265 6e74 6c79  at are currently
+00018f00: 2072 756e 6e69 6e67 2e20 5468 6520 7573   running. The us
+00018f10: 6572 2069 6e74 6572 6163 7469 7665 6c79  er interactively
+00018f20: 2073 656c 6563 7473 2074 6865 2057 6f72   selects the Wor
+00018f30: 6b20 5265 7175 6972 656d 656e 7473 2074  k Requirements t
+00018f40: 6f20 7461 7267 6574 2c20 616e 6420 7468  o target, and th
+00018f50: 656e 2077 6869 6368 2054 6173 6b73 2077  en which Tasks w
+00018f60: 6974 6869 6e20 7468 6f73 6520 576f 726b  ithin those Work
+00018f70: 2052 6571 7569 7265 6d65 6e74 7320 746f   Requirements to
+00018f80: 2061 626f 7274 2e20 5468 6520 576f 726b   abort. The Work
+00018f90: 2052 6571 7569 7265 6d65 6e74 7320 6172   Requirements ar
+00018fa0: 6520 6e6f 7420 6361 6e63 656c 6c65 6420  e not cancelled 
+00018fb0: 6173 2070 6172 7420 6f66 2074 6869 7320  as part of this 
+00018fc0: 7072 6f63 6573 732e 0a0a 5468 6520 606e  process...The `n
+00018fd0: 616d 6573 7061 6365 6020 616e 6420 6074  amespace` and `t
+00018fe0: 6167 6020 7661 6c75 6573 2069 6e20 7468  ag` values in th
+00018ff0: 6520 6063 6f6e 6669 672e 746f 6d6c 6020  e `config.toml` 
+00019000: 6669 6c65 2061 7265 2075 7365 6420 746f  file are used to
+00019010: 2069 6465 6e74 6966 7920 7768 6963 6820   identify which 
+00019020: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00019030: 7320 746f 206c 6973 7420 666f 7220 7365  s to list for se
+00019040: 6c65 6374 696f 6e2e 0a0a 2323 2079 642d  lection...## yd-
+00019050: 646f 776e 6c6f 6164 0a0a 5468 6520 6079  download..The `y
+00019060: 642d 646f 776e 6c6f 6164 6020 636f 6d6d  d-download` comm
+00019070: 616e 6420 646f 776e 6c6f 6164 7320 616e  and downloads an
+00019080: 7920 6f62 6a65 6374 7320 6372 6561 7465  y objects create
+00019090: 6420 696e 2074 6865 2059 656c 6c6f 7744  d in the YellowD
+000190a0: 6f67 204f 626a 6563 7420 5374 6f72 652e  og Object Store.
+000190b0: 0a0a 5468 6520 606e 616d 6573 7061 6365  ..The `namespace
+000190c0: 6020 616e 6420 6074 6167 6020 7661 6c75  ` and `tag` valu
+000190d0: 6573 2061 7265 2075 7365 6420 746f 2064  es are used to d
+000190e0: 6574 6572 6d69 6e65 2077 6869 6368 206f  etermine which o
+000190f0: 626a 6563 7473 2074 6f20 646f 776e 6c6f  bjects to downlo
+00019100: 6164 2e20 4f62 6a65 6374 7320 7769 6c6c  ad. Objects will
+00019110: 2062 6520 646f 776e 6c6f 6164 6564 2074   be downloaded t
+00019120: 6f20 6120 6469 7265 6374 6f72 7920 7769  o a directory wi
+00019130: 7468 2074 6865 2073 616d 6520 6e61 6d65  th the same name
+00019140: 2061 7320 606e 616d 6573 7061 6365 602e   as `namespace`.
+00019150: 2049 6620 6120 6469 7265 6374 6f72 7920   If a directory 
+00019160: 616c 7265 6164 7920 6578 6973 7473 2c20  already exists, 
+00019170: 6120 6e65 7720 6469 7265 6374 6f72 7920  a new directory 
+00019180: 7769 7468 206e 616d 6520 603c 6e61 6d65  with name `<name
+00019190: 7370 6163 653e 2e30 3160 2028 6574 632e  space>.01` (etc.
+000191a0: 2920 7769 6c6c 2062 6520 6372 6561 7465  ) will be create
+000191b0: 642e 0a0a 2323 2079 642d 6465 6c65 7465  d...## yd-delete
+000191c0: 0a0a 5468 6520 6079 642d 6465 6c65 7465  ..The `yd-delete
+000191d0: 6020 636f 6d6d 616e 6420 6465 6c65 7465  ` command delete
+000191e0: 7320 616e 7920 6f62 6a65 6374 7320 6372  s any objects cr
+000191f0: 6561 7465 6420 696e 2074 6865 2059 656c  eated in the Yel
+00019200: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
+00019210: 6f72 652e 0a0a 5468 6520 606e 616d 6573  ore...The `names
+00019220: 7061 6365 6020 616e 6420 6074 6167 6020  pace` and `tag` 
+00019230: 7661 6c75 6573 2069 6e20 7468 6520 6063  values in the `c
+00019240: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00019250: 2061 7265 2075 7365 6420 746f 2069 6465   are used to ide
+00019260: 6e74 6966 7920 7768 6963 6820 6f62 6a65  ntify which obje
+00019270: 6374 7320 746f 2064 656c 6574 652e 204e  cts to delete. N
+00019280: 6f74 6520 7468 6174 2069 7427 7320 6561  ote that it's ea
+00019290: 7379 2074 6f20 7573 6520 6079 642d 6465  sy to use `yd-de
+000192a0: 6c65 7465 6020 746f 2063 6c65 6172 2074  lete` to clear t
+000192b0: 6865 2063 6f6e 7465 6e74 7320 6f66 2061  he contents of a
+000192c0: 206e 616d 6573 7061 6365 2062 7920 7573   namespace by us
+000192d0: 696e 6720 616e 2065 6d70 7479 2060 7461  ing an empty `ta
+000192e0: 6760 2c20 6173 2066 6f6c 6c6f 7773 3a0a  g`, as follows:.
+000192f0: 0a60 6060 7368 656c 6c0a 7964 2d64 656c  .```shell.yd-del
+00019300: 6574 6520 2d74 2022 220a 6060 600a 0a54  ete -t "".```..T
+00019310: 6869 7320 6361 6e20 6265 2065 7874 656e  his can be exten
+00019320: 6465 6420 746f 2061 6e79 206f 7468 6572  ded to any other
+00019330: 206e 616d 6573 7061 6365 2062 7920 7573   namespace by us
+00019340: 696e 6720 7468 6520 602d 2d6e 616d 6573  ing the `--names
+00019350: 7061 6365 602f 602d 6e60 206f 7074 696f  pace`/`-n` optio
+00019360: 6e2e 0a0a 2323 2079 642d 7570 6c6f 6164  n...## yd-upload
+00019370: 0a0a 5468 6520 6079 642d 7570 6c6f 6164  ..The `yd-upload
+00019380: 6020 636f 6d6d 616e 6420 7570 6c6f 6164  ` command upload
+00019390: 7320 6669 6c65 7320 6672 6f6d 2074 6865  s files from the
+000193a0: 206c 6f63 616c 2066 696c 6573 7973 7465   local filesyste
+000193b0: 6d20 746f 2074 6865 2059 656c 6c6f 7744  m to the YellowD
+000193c0: 6f67 204f 626a 6563 7420 7374 6f72 652e  og Object store.
+000193d0: 2046 696c 6573 2061 7265 2070 6c61 6365   Files are place
+000193e0: 6420 696e 2074 6865 2063 6f6e 6669 6775  d in the configu
+000193f0: 7265 6420 606e 616d 6573 7061 6365 6020  red `namespace` 
+00019400: 7769 7468 696e 2061 2064 6972 6563 746f  within a directo
+00019410: 7279 2073 7570 706c 6965 6420 7573 696e  ry supplied usin
+00019420: 6720 7468 6520 2872 6571 7569 7265 6429  g the (required)
+00019430: 2060 2d2d 6469 7265 6374 6f72 7960 206f   `--directory` o
+00019440: 7074 696f 6e2c 2065 2e67 2e3a 0a0a 6060  ption, e.g.:..``
+00019450: 6073 6865 6c6c 0a79 642d 7570 6c6f 6164  `shell.yd-upload
+00019460: 202d 2d64 6972 6563 746f 7279 206d 795f   --directory my_
+00019470: 776f 726b 5f72 6571 7569 7265 6d65 6e74  work_requirement
+00019480: 2066 696c 655f 3120 6669 6c65 5f32 206d   file_1 file_2 m
+00019490: 6f72 6566 696c 6573 2f66 696c 6533 0a60  orefiles/file3.`
+000194a0: 6060 0a54 6f20 7375 7070 7265 7373 2074  ``.To suppress t
+000194b0: 6865 206d 6972 726f 7269 6e67 206f 6620  he mirroring of 
+000194c0: 7468 6520 6c6f 6361 6c20 6469 7265 6374  the local direct
+000194d0: 6f72 7920 7374 7275 6374 7572 6520 7769  ory structure wi
+000194e0: 7468 696e 2074 6865 206f 626a 6563 7420  thin the object 
+000194f0: 7374 6f72 652c 2075 7365 2074 6865 2060  store, use the `
+00019500: 2d2d 666c 6174 7465 6e2d 7570 6c6f 6164  --flatten-upload
+00019510: 2d70 6174 6873 6020 6f72 2060 2d66 6020  -paths` or `-f` 
+00019520: 6f70 7469 6f6e 2e20 4e6f 7465 2074 6861  option. Note tha
+00019530: 7420 6966 2074 6869 7320 6372 6561 7465  t if this create
+00019540: 7320 6d75 6c74 6970 6c65 2075 706c 6f61  s multiple uploa
+00019550: 6465 6420 6669 6c65 7320 7769 7468 2074  ded files with t
+00019560: 6865 2073 616d 6520 7061 7468 2069 6e20  he same path in 
+00019570: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+00019580: 2066 6f6c 6465 722c 2066 696c 6573 2077   folder, files w
+00019590: 696c 6c20 6265 206f 7665 7277 7269 7474  ill be overwritt
+000195a0: 656e 2e0a 0a46 696c 6573 2069 6e20 6469  en...Files in di
+000195b0: 7265 6374 6f72 6965 7320 6d61 7920 6265  rectories may be
+000195c0: 2072 6563 7572 7369 7665 6c79 2075 706c   recursively upl
+000195d0: 6f61 6465 6420 7573 696e 6720 7468 6520  oaded using the 
+000195e0: 602d 2d72 6563 7572 7369 7665 6020 6f72  `--recursive` or
+000195f0: 2060 2d72 6020 6f70 7469 6f6e 2c20 652e   `-r` option, e.
+00019600: 672e 3a0a 0a60 6060 7368 656c 6c0a 7964  g.:..```shell.yd
+00019610: 2d75 706c 6f61 6420 2d2d 6469 7265 6374  -upload --direct
+00019620: 6f72 7920 6d79 5f77 6f72 6b5f 7265 7175  ory my_work_requ
+00019630: 6972 656d 656e 7420 2d72 206d 7964 6972  irement -r mydir
+00019640: 206d 796f 7468 6572 6469 720a 6060 600a   myotherdir.```.
+00019650: 0a54 6f20 7570 6c6f 6164 2074 6f20 6f74  .To upload to ot
+00019660: 6865 7220 6e61 6d65 7370 6163 6573 2c20  her namespaces, 
+00019670: 7573 6520 7468 6520 602d 2d6e 616d 6573  use the `--names
+00019680: 7061 6365 602f 602d 6e60 206f 7074 696f  pace`/`-n` optio
+00019690: 6e2e 0a0a 2323 2079 642d 7368 7574 646f  n...## yd-shutdo
+000196a0: 776e 0a0a 5468 6520 6079 642d 7368 7574  wn..The `yd-shut
+000196b0: 646f 776e 6020 636f 6d6d 616e 6420 7368  down` command sh
+000196c0: 7574 7320 646f 776e 2057 6f72 6b65 7220  uts down Worker 
+000196d0: 506f 6f6c 7320 7468 6174 206d 6174 6368  Pools that match
+000196e0: 2074 6865 2060 6e61 6d65 7370 6163 6560   the `namespace`
+000196f0: 2061 6e64 2060 7461 6760 2066 6f75 6e64   and `tag` found
+00019700: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
+00019710: 6174 696f 6e20 6669 6c65 2e20 416c 6c20  ation file. All 
+00019720: 7265 6d61 696e 696e 6720 776f 726b 2077  remaining work w
+00019730: 696c 6c20 6265 2063 616e 6365 6c6c 6564  ill be cancelled
+00019740: 2c20 6275 7420 6375 7272 656e 746c 7920  , but currently 
+00019750: 6578 6563 7574 696e 6720 5461 736b 7320  executing Tasks 
+00019760: 7769 6c6c 2062 6520 616c 6c6f 7765 6420  will be allowed 
+00019770: 746f 2063 6f6d 706c 6574 652c 2061 6674  to complete, aft
+00019780: 6572 2077 6869 6368 2074 6865 2043 6f6d  er which the Com
+00019790: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
+000197a0: 2077 696c 6c20 6265 2074 6572 6d69 6e61   will be termina
+000197b0: 7465 642e 0a0a 2323 2079 642d 696e 7374  ted...## yd-inst
+000197c0: 616e 7469 6174 650a 0a54 6865 2060 7964  antiate..The `yd
+000197d0: 2d69 6e73 7461 6e74 6961 7465 6020 636f  -instantiate` co
+000197e0: 6d6d 616e 6420 696e 7374 616e 7469 6174  mmand instantiat
+000197f0: 6573 2061 2043 6f6d 7075 7465 2052 6571  es a Compute Req
+00019800: 7569 7265 6d65 6e74 2028 692e 652e 2c20  uirement (i.e., 
+00019810: 6120 7365 7420 6f66 2069 6e73 7461 6e63  a set of instanc
+00019820: 6573 2074 6861 7420 6172 6520 6d61 6e61  es that are mana
+00019830: 6765 6420 6279 2074 6865 6972 2063 7265  ged by their cre
+00019840: 6174 6f72 2061 6e64 2064 6f20 6e6f 7420  ator and do not 
+00019850: 6175 746f 6d61 7469 6361 6c6c 7920 6265  automatically be
+00019860: 636f 6d65 2070 6172 7420 6f66 2061 2059  come part of a Y
+00019870: 656c 6c6f 7744 6f67 2057 6f72 6b65 7220  ellowDog Worker 
+00019880: 506f 6f6c 292e 0a0a 5468 6973 2063 6f6d  Pool)...This com
+00019890: 6d61 6e64 2075 7365 7320 7468 6520 6461  mand uses the da
+000198a0: 7461 2066 726f 6d20 7468 6520 6077 6f72  ta from the `wor
+000198b0: 6b65 7250 6f6f 6c60 2063 6f6e 6669 6775  kerPool` configu
+000198c0: 7261 7469 6f6e 2073 6563 7469 6f6e 2c20  ration section, 
+000198d0: 6275 7420 6f6e 6c79 2075 7365 7320 7468  but only uses th
+000198e0: 6520 606e 616d 6560 2c20 6074 656d 706c  e `name`, `templ
+000198f0: 6174 6549 6460 2c20 6074 6172 6765 7449  ateId`, `targetI
+00019900: 6e73 7461 6e63 6543 6f75 6e74 602c 2060  nstanceCount`, `
+00019910: 696e 7374 616e 6365 5461 6773 602c 2060  instanceTags`, `
+00019920: 7573 6572 4461 7461 602c 2061 6e64 2060  userData`, and `
+00019930: 696d 6167 6573 4964 6020 7072 6f70 6572  imagesId` proper
+00019940: 7469 6573 2e20 496e 2061 6464 6974 696f  ties. In additio
+00019950: 6e2c 2074 6865 2042 6f6f 6c65 616e 2070  n, the Boolean p
+00019960: 726f 7065 7274 7920 606d 6169 6e74 6169  roperty `maintai
+00019970: 6e49 6e73 7461 6e63 6543 6f75 6e74 6020  nInstanceCount` 
+00019980: 2864 6566 6175 6c74 203d 2060 6661 6c73  (default = `fals
+00019990: 6560 2920 6973 2061 7661 696c 6162 6c65  e`) is available
+000199a0: 2066 6f72 2075 7365 2077 6974 6820 6079   for use with `y
+000199b0: 642d 696e 7374 616e 7469 6174 6560 2e0a  d-instantiate`..
+000199c0: 0a43 6f6d 7075 7465 2052 6571 7569 7265  .Compute Require
+000199d0: 6d65 6e74 7320 6361 6e20 6265 2069 6e73  ments can be ins
+000199e0: 7461 6e74 6961 7465 6420 6469 7265 6374  tantiated direct
+000199f0: 6c79 2066 726f 6d20 4a53 4f4e 2028 6f72  ly from JSON (or
+00019a00: 204a 736f 6e6e 6574 2920 7370 6563 6966   Jsonnet) specif
+00019a10: 6963 6174 696f 6e73 2c20 7573 696e 6720  ications, using 
+00019a20: 7468 6520 602d 2d63 6f6d 7075 7465 2d72  the `--compute-r
+00019a30: 6571 7569 7265 6d65 6e74 6020 286f 7220  equirement` (or 
+00019a40: 602d 4360 2920 636f 6d6d 616e 6420 6c69  `-C`) command li
+00019a50: 6e65 206f 7074 696f 6e2c 2066 6f6c 6c6f  ne option, follo
+00019a60: 7765 6420 6279 2074 6865 2066 696c 656e  wed by the filen
+00019a70: 616d 652e 2054 6865 2070 726f 7065 7274  ame. The propert
+00019a80: 6965 7320 6c69 7374 6564 2061 626f 7665  ies listed above
+00019a90: 2077 696c 6c20 6265 2069 6e68 6572 6974   will be inherit
+00019aa0: 6564 2066 726f 6d20 7468 6520 636f 6e66  ed from the conf
+00019ab0: 6967 2e74 6f6d 6c20 6077 6f72 6b65 7250  ig.toml `workerP
+00019ac0: 6f6f 6c60 2073 7065 6369 6669 6361 7469  ool` specificati
+00019ad0: 6f6e 2069 6620 7468 6579 2061 7265 206e  on if they are n
+00019ae0: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
+00019af0: 6520 4a53 4f4e 2066 696c 652e 2041 6e20  e JSON file. An 
+00019b00: 6578 616d 706c 6520 4a53 4f4e 2073 7065  example JSON spe
+00019b10: 6369 6669 6361 7469 6f6e 2069 7320 7368  cification is sh
+00019b20: 6f77 6e20 6265 6c6f 773a 0a0a 6060 606a  own below:..```j
+00019b30: 736f 6e0a 7b0a 2020 2269 6d61 6765 7349  son.{.  "imagesI
+00019b40: 6422 3a20 2279 6469 643a 696d 6766 616d  d": "ydid:imgfam
+00019b50: 3a30 3030 3030 303a 3431 3936 3235 3932  :000000:41962592
+00019b60: 2d35 3737 632d 3466 6465 2d61 6230 332d  -577c-4fde-ab03-
+00019b70: 6438 3532 3436 3565 3766 3862 222c 0a20  d852465e7f8b",. 
+00019b80: 2022 696e 7374 616e 6365 5461 6773 223a   "instanceTags":
+00019b90: 207b 2261 3122 3a20 226f 6e65 222c 2022   {"a1": "one", "
+00019ba0: 6132 223a 2022 7477 6f22 7d2c 0a20 2022  a2": "two"},.  "
+00019bb0: 7265 7175 6972 656d 656e 744e 616d 6522  requirementName"
+00019bc0: 3a20 2263 725f 7465 7374 5f7b 7b64 6174  : "cr_test_{{dat
+00019bd0: 6574 696d 657d 7d22 2c0a 2020 2272 6571  etime}}",.  "req
+00019be0: 7569 7265 6d65 6e74 4e61 6d65 7370 6163  uirementNamespac
+00019bf0: 6522 3a20 2270 7965 7861 6d70 6c65 7322  e": "pyexamples"
+00019c00: 2c0a 2020 2272 6571 7569 7265 6d65 6e74  ,.  "requirement
+00019c10: 5461 6722 3a20 2270 7965 7861 6d70 6c65  Tag": "pyexample
+00019c20: 732d 7465 7374 222c 0a20 2022 7465 6d70  s-test",.  "temp
+00019c30: 6c61 7465 4964 223a 2022 7964 6964 3a63  lateId": "ydid:c
+00019c40: 7274 3a30 3030 3030 303a 3233 3065 3961  rt:000000:230e9a
+00019c50: 3432 2d39 3764 622d 3464 3639 2d61 6139  42-97db-4d69-aa9
+00019c60: 312d 3239 6666 3330 3939 3531 6234 222c  1-29ff309951b4",
+00019c70: 0a20 2022 7573 6572 4461 7461 223a 2022  .  "userData": "
+00019c80: 232f 6269 6e2f 6261 7368 5c6e 234f 7468  #/bin/bash\n#Oth
+00019c90: 6572 2073 7475 6666 2e2e 2e22 2c0a 2020  er stuff...",.  
+00019ca0: 2274 6172 6765 7449 6e73 7461 6e63 6543  "targetInstanceC
+00019cb0: 6f75 6e74 223a 2031 2c0a 2020 226d 6169  ount": 1,.  "mai
+00019cc0: 6e74 6169 6e49 6e73 7461 6e63 6543 6f75  ntainInstanceCou
+00019cd0: 6e74 223a 2074 7275 650a 7d0a 6060 600a  nt": true.}.```.
+00019ce0: 0a49 6620 6120 576f 726b 6572 2050 6f6f  .If a Worker Poo
+00019cf0: 6c20 6973 2064 6566 696e 6564 2c20 7573  l is defined, us
+00019d00: 696e 6720 6077 6f72 6b65 7250 6f6f 6c44  ing `workerPoolD
+00019d10: 6174 6160 2069 6e20 7468 6520 636f 6e66  ata` in the conf
+00019d20: 6967 7572 6174 696f 6e20 6669 6c65 206f  iguration file o
+00019d30: 7220 6279 2075 7369 6e67 2074 6865 2060  r by using the `
+00019d40: 2d2d 776f 726b 6572 2d70 6f6f 6c60 2028  --worker-pool` (
+00019d50: 6f72 2060 2d70 6029 206f 7074 696f 6e2c  or `-p`) option,
+00019d60: 2060 7964 2d69 6e73 7461 6e74 6961 7465   `yd-instantiate
+00019d70: 6020 7769 6c6c 2065 7874 7261 6374 2074  ` will extract t
+00019d80: 6865 2043 6f6d 7075 7465 2052 6571 7569  he Compute Requi
+00019d90: 7265 6d65 6e74 2066 726f 6d20 7468 6520  rement from the 
+00019da0: 576f 726b 6572 2050 6f6f 6c20 7370 6563  Worker Pool spec
+00019db0: 6966 6963 6174 696f 6e20 2869 676e 6f72  ification (ignor
+00019dc0: 696e 6720 576f 726b 6572 2d50 6f6f 6c2d  ing Worker-Pool-
+00019dd0: 7370 6563 6966 6963 2064 6174 6129 2c20  specific data), 
+00019de0: 616e 6420 7573 6520 7468 6174 2066 6f72  and use that for
+00019df0: 2069 6e73 7461 6e74 6961 7469 6e67 2074   instantiating t
+00019e00: 6865 2043 6f6d 7075 7465 2052 6571 7569  he Compute Requi
+00019e10: 7265 6d65 6e74 2e0a 0a55 7365 2074 6865  rement...Use the
+00019e20: 2060 2d2d 6472 792d 7275 6e60 206f 7074   `--dry-run` opt
+00019e30: 696f 6e20 746f 2069 6e73 7065 6374 2074  ion to inspect t
+00019e40: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
+00019e50: 6520 436f 6d70 7574 6520 5265 7175 6972  e Compute Requir
+00019e60: 656d 656e 7420 7370 6563 6966 6963 6174  ement specificat
+00019e70: 696f 6e20 7468 6174 2077 696c 6c20 6265  ion that will be
+00019e80: 2073 7562 6d69 7474 6564 2c20 696e 204a   submitted, in J
+00019e90: 534f 4e20 666f 726d 6174 2e20 5468 6520  SON format. The 
+00019ea0: 4a53 4f4e 206f 7574 7075 7420 6f66 2074  JSON output of t
+00019eb0: 6869 7320 636f 6d6d 616e 6420 6361 6e20  his command can 
+00019ec0: 6265 2075 7365 6420 7769 7468 2074 6865  be used with the
+00019ed0: 2060 2d43 6020 6f70 7469 6f6e 2061 626f   `-C` option abo
+00019ee0: 7665 2028 6f72 2077 6974 6820 602d 7060  ve (or with `-p`
+00019ef0: 2066 6f72 2057 6f72 6b65 7220 506f 6f6c   for Worker Pool
+00019f00: 2073 7065 6369 6669 6361 7469 6f6e 7329   specifications)
+00019f10: 2e0a 0a23 2323 2054 6573 742d 5275 6e6e  ...### Test-Runn
+00019f20: 696e 6720 6120 4479 6e61 6d69 6320 5465  ing a Dynamic Te
+00019f30: 6d70 6c61 7465 0a0a 5768 656e 2061 2074  mplate..When a t
+00019f40: 6865 2060 7465 6d70 6c61 7465 4964 6020  he `templateId` 
+00019f50: 6f66 2061 2044 796e 616d 6963 2052 6571  of a Dynamic Req
+00019f60: 7569 7265 6d65 6e74 2069 7320 7573 6564  uirement is used
+00019f70: 2c20 7468 6520 6079 642d 696e 7374 616e  , the `yd-instan
+00019f80: 7469 6174 6560 2063 6f6d 6d61 6e64 2063  tiate` command c
+00019f90: 616e 2062 6520 7573 6564 2074 6f20 7265  an be used to re
+00019fa0: 706f 7274 206f 6e20 6120 7465 7374 2072  port on a test r
+00019fb0: 756e 206f 6620 7468 6520 5465 6d70 6c61  un of the Templa
+00019fc0: 7465 2c20 7573 696e 6720 7468 6520 602d  te, using the `-
+00019fd0: 2d72 6570 6f72 7460 2028 6f72 2060 2d72  -report` (or `-r
+00019fe0: 6029 2063 6f6d 6d61 6e64 206c 696e 6520  `) command line 
+00019ff0: 6f70 7469 6f6e 2e20 5468 6973 2063 616e  option. This can
+0001a000: 2062 6520 7573 6564 2077 6974 6820 544f   be used with TO
+0001a010: 4d4c 2d64 6566 696e 6564 2043 6f6d 7075  ML-defined Compu
+0001a020: 7465 2052 6571 7569 7265 6d65 6e74 2073  te Requirement s
+0001a030: 7065 6369 6669 6361 7469 6f6e 732c 2062  pecifications, b
+0001a040: 7574 206e 6f74 2074 686f 7365 2074 6861  ut not those tha
+0001a050: 7420 6172 6520 4a53 4f4e 2d64 6566 696e  t are JSON-defin
+0001a060: 6564 2e0a 0a4e 6f20 696e 7374 616e 6365  ed...No instance
+0001a070: 7320 7769 6c6c 2062 6520 7072 6f76 6973  s will be provis
+0001a080: 696f 6e65 6420 6475 7269 6e67 2074 6865  ioned during the
+0001a090: 2074 6573 7420 7275 6e2e 0a0a 466f 7220   test run...For 
+0001a0a0: 6578 616d 706c 653a 0a0a 6060 6073 6865  example:..```she
+0001a0b0: 6c6c 0a25 2079 642d 696e 7374 616e 7469  ll.% yd-instanti
+0001a0c0: 6174 6520 2d2d 7265 706f 7274 202d 2d71  ate --report --q
+0001a0d0: 7569 6574 0a0a e294 8ce2 9480 e294 80e2  uiet............
+0001a0e0: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
+0001a0f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a100: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+0001a110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a120: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+0001a130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a160: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+0001a170: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a190: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+0001a1a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a1b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a1c0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
+0001a1d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a1e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a1f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a200: 9490 0ae2 9482 2020 2020 e294 8220 2020  ......    ...   
+0001a210: 5261 6e6b 20e2 9482 2050 726f 7669 6465  Rank ... Provide
+0001a220: 7220 2020 e294 8220 5479 7065 2020 2020  r   ... Type    
+0001a230: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+0001a240: 2052 6567 696f 6e20 2020 20e2 9482 2049   Region    ... I
+0001a250: 6e73 7461 6e63 6554 7970 6520 2020 e294  nstanceType   ..
+0001a260: 8220 536f 7572 6365 204e 616d 6520 2020  . Source Name   
+0001a270: 2020 2020 e294 820a e294 9ce2 9480 e294      ............
+0001a280: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a2a0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a2b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a2c0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a2d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a2e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a2f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a310: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a330: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a340: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a350: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a360: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a370: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a380: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a390: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a3a0: 80e2 94a4 0ae2 9482 2020 3120 e294 8220  ........  1 ... 
+0001a3b0: 2020 2020 2031 20e2 9482 2041 5753 2020       1 ... AWS  
+0001a3c0: 2020 2020 2020 e294 8220 4177 7353 706f        ... AwsSpo
+0001a3d0: 7443 6f6d 7075 7465 536f 7572 6365 20e2  tComputeSource .
+0001a3e0: 9482 2065 752d 7765 7374 2d32 20e2 9482  .. eu-west-2 ...
+0001a3f0: 2074 3361 2e6e 616e 6f20 2020 2020 2020   t3a.nano       
+0001a400: e294 8220 6177 7373 706f 742d 6575 2d77  ... awsspot-eu-w
+0001a410: 6573 742d 3220 e294 820a e294 9ce2 9480  est-2 ..........
+0001a420: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a440: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a460: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a480: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a4a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a4b0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a4c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a4d0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a4e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a4f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a500: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a510: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a520: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a530: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a540: e294 80e2 94a4 0ae2 9482 2020 3220 e294  ..........  2 ..
+0001a550: 8220 2020 2020 2032 20e2 9482 2041 5753  .      2 ... AWS
+0001a560: 2020 2020 2020 2020 e294 8220 4177 7353          ... AwsS
+0001a570: 706f 7443 6f6d 7075 7465 536f 7572 6365  potComputeSource
+0001a580: 20e2 9482 2065 752d 7765 7374 2d32 20e2   ... eu-west-2 .
+0001a590: 9482 2074 3361 2e6d 6963 726f 2020 2020  .. t3a.micro    
+0001a5a0: 2020 e294 8220 6177 7373 706f 742d 6575    ... awsspot-eu
+0001a5b0: 2d77 6573 742d 3220 e294 820a e294 9ce2  -west-2 ........
+0001a5c0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a5d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a5e0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a5f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a600: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a610: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a620: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a630: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a650: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a660: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a670: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a6a0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a6b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a6c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a6d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a6e0: 9480 e294 80e2 94a4 0ae2 9482 2020 3320  ............  3 
+0001a6f0: e294 8220 2020 2020 2033 20e2 9482 2041  ...      3 ... A
+0001a700: 5753 2020 2020 2020 2020 e294 8220 4177  WS        ... Aw
+0001a710: 7353 706f 7443 6f6d 7075 7465 536f 7572  sSpotComputeSour
+0001a720: 6365 20e2 9482 2065 752d 7765 7374 2d32  ce ... eu-west-2
+0001a730: 20e2 9482 2074 3361 2e73 6d61 6c6c 2020   ... t3a.small  
+0001a740: 2020 2020 e294 8220 6177 7373 706f 742d      ... awsspot-
+0001a750: 6575 2d77 6573 742d 3220 e294 820a e294  eu-west-2 ......
+0001a760: 9ce2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a770: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a780: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a7a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a7b0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a7c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a7d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a7e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a7f0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a810: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a830: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a840: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a850: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a860: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a870: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a880: 80e2 9480 e294 80e2 94a4 0ae2 9482 2020  ..............  
+0001a890: 3420 e294 8220 2020 2020 2034 20e2 9482  4 ...      4 ...
+0001a8a0: 2041 5753 2020 2020 2020 2020 e294 8220   AWS        ... 
+0001a8b0: 4177 7353 706f 7443 6f6d 7075 7465 536f  AwsSpotComputeSo
+0001a8c0: 7572 6365 20e2 9482 2065 752d 7765 7374  urce ... eu-west
+0001a8d0: 2d32 20e2 9482 2063 3561 2e6c 6172 6765  -2 ... c5a.large
+0001a8e0: 2020 2020 2020 e294 8220 6177 7373 706f        ... awsspo
+0001a8f0: 742d 6575 2d77 6573 742d 3220 e294 820a  t-eu-west-2 ....
+0001a900: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a910: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a920: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001a930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a950: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001a960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a990: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a9a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a9b0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001a9c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a9d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a9e0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a9f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aa00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aa10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aa20: e294 80e2 9480 e294 80e2 94a4 0ae2 9482  ................
+0001aa30: 2020 3520 e294 8220 2020 2020 2034 20e2    5 ...      4 .
+0001aa40: 9482 2041 5753 2020 2020 2020 2020 e294  .. AWS        ..
+0001aa50: 8220 4177 7353 706f 7443 6f6d 7075 7465  . AwsSpotCompute
+0001aa60: 536f 7572 6365 20e2 9482 2065 752d 7765  Source ... eu-we
+0001aa70: 7374 2d32 20e2 9482 2063 3661 2e6c 6172  st-2 ... c6a.lar
+0001aa80: 6765 2020 2020 2020 e294 8220 6177 7373  ge      ... awss
+0001aa90: 706f 742d 6575 2d77 6573 742d 3220 e294  pot-eu-west-2 ..
+0001aaa0: 820a e294 9ce2 9480 e294 80e2 9480 e294  ................
+0001aab0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001aac0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001aad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aae0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aaf0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001ab00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab30: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001ab40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab50: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001ab60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab90: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aba0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001abb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001abc0: 9480 e294 80e2 9480 e294 80e2 94a4 0ae2  ................
+0001abd0: 9482 2020 3620 e294 8220 2020 2020 2034  ..  6 ...      4
+0001abe0: 20e2 9482 2041 5753 2020 2020 2020 2020   ... AWS        
+0001abf0: e294 8220 4177 7353 706f 7443 6f6d 7075  ... AwsSpotCompu
+0001ac00: 7465 536f 7572 6365 20e2 9482 2065 752d  teSource ... eu-
+0001ac10: 7765 7374 2d32 20e2 9482 2074 3361 2e6d  west-2 ... t3a.m
+0001ac20: 6564 6975 6d20 2020 2020 e294 8220 6177  edium     ... aw
+0001ac30: 7373 706f 742d 6575 2d77 6573 742d 3220  sspot-eu-west-2 
+0001ac40: e294 820a e294 9ce2 9480 e294 80e2 9480  ................
+0001ac50: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001ac60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ac70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ac80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ac90: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001aca0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001acb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001acc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001acd0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001ace0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001acf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ad00: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ad10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ad20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ad30: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001ad40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ad50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ad60: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+0001ad70: 0ae2 9482 2020 3720 e294 8220 2020 2020  ....  7 ...     
+0001ad80: 2035 20e2 9482 2041 5753 2020 2020 2020   5 ... AWS      
+0001ad90: 2020 e294 8220 4177 7353 706f 7443 6f6d    ... AwsSpotCom
+0001ada0: 7075 7465 536f 7572 6365 20e2 9482 2065  puteSource ... e
+0001adb0: 752d 7765 7374 2d32 20e2 9482 206d 3561  u-west-2 ... m5a
+0001adc0: 2e6c 6172 6765 2020 2020 2020 e294 8220  .large      ... 
+0001add0: 6177 7373 706f 742d 6575 2d77 6573 742d  awsspot-eu-west-
+0001ade0: 3220 e294 820a e294 9ce2 9480 e294 80e2  2 ..............
+0001adf0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001ae00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae10: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae30: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001ae40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae70: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001ae80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aea0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001aeb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aec0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aed0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001aee0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aef0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001af00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001af10: 94a4 0ae2 9482 2020 3820 e294 8220 2020  ......  8 ...   
+0001af20: 2020 2035 20e2 9482 2041 5753 2020 2020     5 ... AWS    
+0001af30: 2020 2020 e294 8220 4177 7353 706f 7443      ... AwsSpotC
+0001af40: 6f6d 7075 7465 536f 7572 6365 20e2 9482  omputeSource ...
+0001af50: 2065 752d 7765 7374 2d32 20e2 9482 206d   eu-west-2 ... m
+0001af60: 3561 642e 6c61 7267 6520 2020 2020 e294  5ad.large     ..
+0001af70: 8220 6177 7373 706f 742d 6575 2d77 6573  . awsspot-eu-wes
+0001af80: 742d 3220 e294 820a e294 9ce2 9480 e294  t-2 ............
+0001af90: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001afa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001afb0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001afc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001afd0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001afe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b020: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b040: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001b050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b070: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001b080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b0a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b0b0: 80e2 94a4 0ae2 9482 2020 3920 e294 8220  ........  9 ... 
+0001b0c0: 2020 2020 2035 20e2 9482 2041 5753 2020       5 ... AWS  
+0001b0d0: 2020 2020 2020 e294 8220 4177 7353 706f        ... AwsSpo
+0001b0e0: 7443 6f6d 7075 7465 536f 7572 6365 20e2  tComputeSource .
+0001b0f0: 9482 2065 752d 7765 7374 2d32 20e2 9482  .. eu-west-2 ...
+0001b100: 206d 3661 2e6c 6172 6765 2020 2020 2020   m6a.large      
+0001b110: e294 8220 6177 7373 706f 742d 6575 2d77  ... awsspot-eu-w
+0001b120: 6573 742d 3220 e294 820a e294 9ce2 9480  est-2 ..........
+0001b130: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001b140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b150: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001b160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b170: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001b180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b1a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b1b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b1c0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001b1d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b1e0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001b1f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b200: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b210: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001b220: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b230: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b240: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b250: e294 80e2 94a4 0ae2 9482 2031 3020 e294  .......... 10 ..
+0001b260: 8220 2020 2020 2035 20e2 9482 2041 5753  .      5 ... AWS
+0001b270: 2020 2020 2020 2020 e294 8220 4177 7353          ... AwsS
+0001b280: 706f 7443 6f6d 7075 7465 536f 7572 6365  potComputeSource
+0001b290: 20e2 9482 2065 752d 7765 7374 2d32 20e2   ... eu-west-2 .
+0001b2a0: 9482 2074 3361 2e6c 6172 6765 2020 2020  .. t3a.large    
+0001b2b0: 2020 e294 8220 6177 7373 706f 742d 6575    ... awsspot-eu
+0001b2c0: 2d77 6573 742d 3220 e294 820a e294 94e2  -west-2 ........
+0001b2d0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+0001b2e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b2f0: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
+0001b300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b310: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
+0001b320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b330: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b340: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b350: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b360: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+0001b370: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b380: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
+0001b390: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b3a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b3b0: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
+0001b3c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b3d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b3e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b3f0: 9480 e294 80e2 9498 0a60 6060 0a0a 2323  .........```..##
+0001b400: 2079 642d 7465 726d 696e 6174 650a 0a54   yd-terminate..T
+0001b410: 6865 2060 7964 2d74 6572 6d69 6e61 7465  he `yd-terminate
+0001b420: 6020 636f 6d6d 616e 6420 696d 6d65 6469  ` command immedi
+0001b430: 6174 656c 7920 7465 726d 696e 6174 6573  ately terminates
+0001b440: 2043 6f6d 7075 7465 2052 6571 7569 7265   Compute Require
+0001b450: 6d65 6e74 7320 7468 6174 206d 6174 6368  ments that match
+0001b460: 2074 6865 2060 6e61 6d65 7370 6163 6560   the `namespace`
+0001b470: 2061 6e64 2060 7461 6760 2066 6f75 6e64   and `tag` found
+0001b480: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
+0001b490: 6174 696f 6e20 6669 6c65 2e20 416e 7920  ation file. Any 
+0001b4a0: 6578 6563 7574 696e 6720 5461 736b 7320  executing Tasks 
+0001b4b0: 7769 6c6c 2062 6520 7465 726d 696e 6174  will be terminat
+0001b4c0: 6564 2069 6d6d 6564 6961 7465 6c79 2c20  ed immediately, 
+0001b4d0: 616e 6420 7468 6520 576f 726b 6572 2050  and the Worker P
+0001b4e0: 6f6f 6c20 7769 6c6c 2062 6520 7368 7574  ool will be shut
+0001b4f0: 2064 6f77 6e2e 0a                         down..
```

### Comparing `yellowdog-python-examples-6.0.3/pyproject.toml` & `yellowdog-python-examples-6.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/setup.cfg` & `yellowdog-python-examples-6.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/abort.py` & `yellowdog-python-examples-6.0.4/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/admin.py` & `yellowdog-python-examples-6.0.4/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/args.py` & `yellowdog-python-examples-6.0.4/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.4/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.4/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.4/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/config.py` & `yellowdog-python-examples-6.0.4/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.4/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.4/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/delete.py` & `yellowdog-python-examples-6.0.4/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/download.py` & `yellowdog-python-examples-6.0.4/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.4/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.4/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.4/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/list.py` & `yellowdog-python-examples-6.0.4/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.4/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/printing.py` & `yellowdog-python-examples-6.0.4/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/provision.py` & `yellowdog-python-examples-6.0.4/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.4/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.4/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.4/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/submit.py` & `yellowdog-python-examples-6.0.4/yd_commands/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     CloudProvider,
     DoubleRange,
     FlattenPath,
     RunSpecification,
     Task,
     TaskGroup,
     TaskInput,
+    TaskInputSource,
     TaskInputVerification,
     TaskOutput,
     TaskStatus,
     WorkRequirement,
     WorkRequirementStatus,
 )
 
@@ -582,20 +583,23 @@
             check_for_duplicates_in_file_lists(
                 input_files_list,
                 verify_at_start_files_list,
                 verify_wait_files_list,
                 optional_inputs_list,
             )
 
-            # Upload files in the 'inputs' list
+            # Upload files in the 'inputs' list, applying wildcard expansion.
             # (Duplicates won't be re-added)
+            expanded_files_list: List[str] = []
             for file in input_files_list:
-                UPLOADED_FILES.add_input_file(
+                expanded_files = UPLOADED_FILES.add_input_file(
                     filename=file, flatten_upload_paths=flatten_upload_paths
                 )
+                expanded_files_list += expanded_files
+            input_files_list = expanded_files_list
 
             # Upload files in the 'uploadFiles' list
             upload_files = check_list(
                 task.get(
                     UPLOAD_FILES,
                     task_group_data.get(
                         UPLOAD_FILES,
@@ -629,14 +633,16 @@
             inputs += generate_task_input_list(
                 verify_wait_files_list, TaskInputVerification.VERIFY_WAIT, ID
             )
             inputs += generate_task_input_list(
                 files=optional_inputs_list, verification=None, wr_name=ID
             )
 
+            inputs = deduplicate_inputs(inputs)
+
             # Set up the 'outputs' property
             outputs = [
                 TaskOutput.from_worker_directory(file_pattern=file, required=False)
                 for file in check_list(
                     task.get(
                         OUTPUT_FILES,
                         task_group_data.get(
@@ -811,14 +817,38 @@
     CLIENT.work_client.cancel_work_requirement(work_requirement)
     print_log(f"Cancelled Work Requirement '{work_requirement.name}'")
 
     # Delete uploaded objects
     UPLOADED_FILES.delete()
 
 
+def deduplicate_inputs(task_inputs: List[TaskInput]) -> List[TaskInput]:
+    """
+    Deduplicate a list of TaskInputs. This is useful when wildcards
+    are used. Note that TaskInputs that differ only in their verification
+    type will be caught by 'check_for_duplicates_in_file_lists()'.
+    """
+    deduplicated_task_inputs: List[TaskInput] = []
+    for task_input in task_inputs:
+        if task_input not in deduplicated_task_inputs:
+            deduplicated_task_inputs.append(task_input)
+        else:
+            namespace = (
+                CONFIG_COMMON.namespace
+                if task_input.source == TaskInputSource.TASK_NAMESPACE
+                else task_input.namespace
+            )
+            print_log(
+                f"Removing '{task_input.verification}' duplicate:"
+                f" '{namespace}::{task_input.objectNamePattern}'"
+            )
+
+    return deduplicated_task_inputs
+
+
 def check_for_duplicates_in_file_lists(*args: List[str]):
     """
     Tests for duplicates in file lists. If duplicates found, print an error
     and raise an Exception.
     """
     files_list = []
     for file_list in args:
```

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.4/yd_commands/submit_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utility functions for use with the submit command.
 """
 
 import re
 from dataclasses import dataclass
+from glob import glob
 from typing import List, Optional
 
 from yellowdog_client import PlatformClient
 from yellowdog_client.model import ObjectPath, TaskInput, TaskInputVerification
 
 from yd_commands.config import ConfigCommon
 from yd_commands.printing import print_error, print_log
@@ -36,14 +37,15 @@
 ) -> TaskInput:
     """
     Generate a TaskInput, accommodating files located relative to the root of
     the namespace, relative to the root of a different namespace,
     and relative to the directory specific to this Work Requirement.
     """
     namespace, filepath = get_namespace_and_filepath(file, wr_name)
+    filepath = filepath.lstrip("/")
     if namespace is None:
         return TaskInput.from_task_namespace(
             object_name_pattern=filepath, verification=verification
         )
     else:
         return TaskInput.from_namespace(
             namespace=namespace, object_name_pattern=filepath, verification=verification
@@ -81,15 +83,14 @@
     except:
         raise Exception(f"Malformed file specification: '{file}'")
 
 
 @dataclass
 class UploadedFile:
     local_file_path: str
-    specified_upload_path: str
     upload_namespace: str
     uploaded_file_path: str
 
 
 class UploadedFiles:
     """
     Upload and manage uploaded files from the 'inputs' and
@@ -101,58 +102,99 @@
         self._wr_name = wr_name
         self._config = config
         self._uploaded_files: List[UploadedFile] = []
 
     def add_upload_file(self, upload_file: str, upload_path: str):
         """
         Upload a file if it hasn't already been uploaded to the same location.
+        Handle wildcards.
         """
-        if ARGS_PARSER.dry_run:
-            return
 
-        if upload_file in [
-            f.local_file_path for f in self._uploaded_files
-        ] and upload_path in [f.specified_upload_path for f in self._uploaded_files]:
-            return
-
-        namespace, uploaded_file_path = get_namespace_and_filepath(
-            upload_path, self._wr_name
-        )
-        namespace = self._config.namespace if namespace is None else namespace
-        upload_file_core(
-            client=self._client,
-            url=self._config.url,
-            local_file=upload_file,
-            namespace=namespace,
-            remote_file=uploaded_file_path,
-        )
+        # Handle wildcard expansion
+        expanded_files = glob(pathname=upload_file, recursive=True)
+        if len(expanded_files) > 1:
+            if not upload_path.endswith("*"):
+                raise Exception(
+                    "'uploadPath' must end in '*' when using'uploadFiles' wildcards"
+                )
+
+        for upload_file in expanded_files:
+            namespace, uploaded_file_path = get_namespace_and_filepath(
+                upload_path, self._wr_name
+            )
+            namespace = self._config.namespace if namespace is None else namespace
 
-        self._uploaded_files.append(
-            UploadedFile(
-                local_file_path=upload_file,
-                specified_upload_path=upload_path,
-                upload_namespace=namespace,
-                uploaded_file_path=uploaded_file_path,
+            # Adjust upload file path for a wildcard upload
+            if "*" in uploaded_file_path:
+                uploaded_file_path = uploaded_file_path.replace(
+                    "*", upload_file.split("/")[-1]
+                )
+
+            uploaded_file_path = uploaded_file_path.lstrip("/")
+
+            duplicate = False
+            for uploaded_file in self._uploaded_files:
+                if (
+                    upload_file == uploaded_file.local_file_path
+                    and uploaded_file_path == uploaded_file.uploaded_file_path
+                    and namespace == uploaded_file.upload_namespace
+                ):
+                    print_log(
+                        f"Not uploading duplicate: '{upload_file}' ->"
+                        f" '{namespace}::{uploaded_file_path}'"
+                    )
+                    duplicate = True
+                    break
+            if duplicate:
+                continue
+
+            if not ARGS_PARSER.dry_run:
+                upload_file_core(
+                    client=self._client,
+                    url=self._config.url,
+                    local_file=upload_file,
+                    namespace=namespace,
+                    remote_file=uploaded_file_path,
+                )
+            else:
+                print_log(
+                    f"Dry-run: would upload '{upload_file}' to"
+                    f" '{namespace}::{uploaded_file_path}'"
+                )
+
+            self._uploaded_files.append(
+                UploadedFile(
+                    local_file_path=upload_file,
+                    upload_namespace=namespace,
+                    uploaded_file_path=uploaded_file_path,
+                )
             )
-        )
 
-    def add_input_file(self, filename: str, flatten_upload_paths: bool):
+    def add_input_file(self, filename: str, flatten_upload_paths: bool) -> List[str]:
         """
-        Add a file from the inputs list.
+        Add a filename from the inputs list, processing wildcards if present.
+        Return the expanded list of filenames.
         """
-        # Apply Work Requirement name prefix, etc.
-        upload_file_name = unique_upload_pathname(
-            filename=filename,
-            id=self._wr_name,
-            inputs_folder_name=None,
-            urlencode_forward_slash=False,
-            flatten_upload_paths=flatten_upload_paths,
-        )
-        # Force 'uploaded_file_name' to be at the root of the namespace
-        self.add_upload_file(filename, f"{NAMESPACE_SEPARATOR}{upload_file_name}")
+
+        # Expand wildcards
+        expanded_files = glob(pathname=filename, recursive=True)
+
+        for filename in expanded_files:
+            # Apply Work Requirement name prefix, etc.
+            upload_file_name = unique_upload_pathname(
+                filename=filename,
+                id=self._wr_name,
+                inputs_folder_name=None,
+                urlencode_forward_slash=False,
+                flatten_upload_paths=flatten_upload_paths,
+            )
+            # Force 'uploaded_file_name' to be at the root of the namespace
+            self.add_upload_file(filename, f"{NAMESPACE_SEPARATOR}{upload_file_name}")
+
+        return expanded_files
 
     def delete(self):
         """
         Delete all files that have been uploaded.
         """
         for namespace in {uf.upload_namespace for uf in self._uploaded_files}:
             object_paths = [
```

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.4/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.4/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/upload.py` & `yellowdog-python-examples-6.0.4/yd_commands/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 
 """
 A script to upload files to the YellowDog Object Store.
 """
 
+from glob import glob
 from os import chdir
+from os import name as os_name
 from os import walk as os_walk
 from os.path import join as os_path_join
 from pathlib import Path
 
 from yd_commands.args import ARGS_PARSER
 from yd_commands.printing import print_log
 from yd_commands.upload_utils import upload_file
@@ -25,14 +27,22 @@
 
     print_log(
         f"Using Object Store namespace '{CONFIG_COMMON.namespace}' "
         f"and directory '{ARGS_PARSER.directory}'"
     )
 
     files_set = set(ARGS_PARSER.files)
+    if os_name == "nt":
+        # Windows wildcard expansion (not done natively by the Windows shell)
+        files_set = {f for files in files_set for f in glob(files)}
+
+    if len(files_set) == 0:
+        print_log("No files to upload")
+        return
+
     added_files_set = set()
     removed_dirs_set = set()
 
     for file_or_dir in files_set:
         pathname = Path(file_or_dir)
         if not pathname.exists():
             raise Exception(f"'{file_or_dir}' doesn't exist")
```

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.4/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.4/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/variables.py` & `yellowdog-python-examples-6.0.4/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/version.py` & `yellowdog-python-examples-6.0.4/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.4/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.3
+Version: 6.0.4
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

