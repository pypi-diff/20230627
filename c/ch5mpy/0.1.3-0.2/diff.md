# Comparing `tmp/ch5mpy-0.1.3.tar.gz` & `tmp/ch5mpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch5mpy-0.1.3.tar", last modified: Thu Feb 16 08:28:05 2023, max compression
+gzip compressed data, was "ch5mpy-0.2.tar", last modified: Tue Jun 27 14:06:08 2023, max compression
```

## Comparing `ch5mpy-0.1.3.tar` & `ch5mpy-0.2.tar`

### file list

```diff
@@ -1,46 +1,73 @@
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21392 2023-02-10 13:26:33.000000 ch5mpy-0.1.3/LICENSE
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1181 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5715 2023-02-15 17:24:04.000000 ch5mpy-0.1.3/README.md
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/ch5mpy/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      695 2023-02-06 10:45:34.000000 ch5mpy-0.1.3/ch5mpy/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      477 2023-02-15 15:22:59.000000 ch5mpy-0.1.3/ch5mpy/_typing.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/ch5mpy/h5array/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-02-06 10:45:34.000000 ch5mpy-0.1.3/ch5mpy/h5array/__init__.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/ch5mpy/h5array/functions/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      242 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/functions/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     7880 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/functions/apply.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    15600 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/functions/element_wise.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      877 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/functions/implement.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    13966 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/functions/two_arrays.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9344 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/h5array.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5248 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/inplace.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5073 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/io.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3547 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/repr.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3207 2023-02-13 16:10:02.000000 ch5mpy-0.1.3/ch5mpy/h5array/slice.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4955 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5array/subset.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4848 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/h5dict.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      319 2023-02-01 15:50:09.000000 ch5mpy-0.1.3/ch5mpy/names.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5178 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/objects.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/ch5mpy/pickle/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:50:09.000000 ch5mpy-0.1.3/ch5mpy/pickle/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1337 2023-02-06 10:45:34.000000 ch5mpy-0.1.3/ch5mpy/pickle/wrap.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      612 2023-02-16 08:25:13.000000 ch5mpy-0.1.3/ch5mpy/utils.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3219 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/ch5mpy/write.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/ch5mpy.egg-info/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1181 2023-02-16 08:28:05.000000 ch5mpy-0.1.3/ch5mpy.egg-info/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      903 2023-02-16 08:28:05.000000 ch5mpy-0.1.3/ch5mpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-02-16 08:28:05.000000 ch5mpy-0.1.3/ch5mpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)       11 2023-02-16 08:28:05.000000 ch5mpy-0.1.3/ch5mpy.egg-info/requires.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        7 2023-02-16 08:28:05.000000 ch5mpy-0.1.3/ch5mpy.egg-info/top_level.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)       81 2023-02-15 16:25:40.000000 ch5mpy-0.1.3/pyproject.toml
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1328 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/setup.cfg
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-02-16 08:28:05.766154 ch5mpy-0.1.3/tests/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2169 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_array_repr.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      531 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_full_slice.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6116 2023-02-15 16:02:31.000000 ch5mpy-0.1.3/tests/test_functions.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12219 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_get_chunks.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2941 2023-02-14 09:12:35.000000 ch5mpy-0.1.3/tests/test_h5array.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3901 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_h5dict.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      802 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_pickle.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2431 2023-02-15 17:14:15.000000 ch5mpy-0.1.3/tests/test_write.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.924226 ch5mpy-0.2/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21392 2023-02-10 13:26:33.000000 ch5mpy-0.2/LICENSE
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    39503 2023-06-27 14:06:08.924226 ch5mpy-0.2/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12804 2023-06-27 13:06:46.000000 ch5mpy-0.2/README.md
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.920226 ch5mpy-0.2/ch5mpy/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1111 2023-06-16 14:57:13.000000 ch5mpy-0.2/ch5mpy/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      420 2023-06-11 21:11:04.000000 ch5mpy-0.2/ch5mpy/_typing.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2083 2023-05-24 14:37:45.000000 ch5mpy-0.2/ch5mpy/attributes.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5267 2023-06-21 08:32:43.000000 ch5mpy-0.2/ch5mpy/dict.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.920226 ch5mpy-0.2/ch5mpy/h5array/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)       64 2023-05-30 07:23:40.000000 ch5mpy-0.2/ch5mpy/h5array/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12255 2023-06-22 14:07:39.000000 ch5mpy-0.2/ch5mpy/h5array/array.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.920226 ch5mpy-0.2/ch5mpy/h5array/chunks/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-03-03 16:51:50.000000 ch5mpy-0.2/ch5mpy/h5array/chunks/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5921 2023-05-24 13:08:59.000000 ch5mpy-0.2/ch5mpy/h5array/chunks/iter.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3092 2023-04-17 15:18:01.000000 ch5mpy-0.2/ch5mpy/h5array/chunks/repeated_array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      424 2023-03-03 23:04:08.000000 ch5mpy-0.2/ch5mpy/h5array/chunks/utils.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5181 2023-04-28 12:16:43.000000 ch5mpy-0.2/ch5mpy/h5array/creation_routines.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.924226 ch5mpy-0.2/ch5mpy/h5array/functions/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      242 2023-04-17 14:55:50.000000 ch5mpy-0.2/ch5mpy/h5array/functions/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10050 2023-06-06 14:08:06.000000 ch5mpy-0.2/ch5mpy/h5array/functions/apply.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1216 2023-04-17 14:55:50.000000 ch5mpy-0.2/ch5mpy/h5array/functions/creation_routines.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     7997 2023-04-26 10:00:28.000000 ch5mpy-0.2/ch5mpy/h5array/functions/element_wise.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1150 2023-03-14 10:11:16.000000 ch5mpy-0.2/ch5mpy/h5array/functions/implement.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10474 2023-06-13 09:17:20.000000 ch5mpy-0.2/ch5mpy/h5array/functions/routines.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    16164 2023-04-17 15:18:02.000000 ch5mpy-0.2/ch5mpy/h5array/functions/two_arrays.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2172 2023-06-27 13:11:28.000000 ch5mpy-0.2/ch5mpy/h5array/io.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3776 2023-04-17 15:18:01.000000 ch5mpy-0.2/ch5mpy/h5array/repr.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4629 2023-06-22 09:17:13.000000 ch5mpy-0.2/ch5mpy/h5array/view.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.924226 ch5mpy-0.2/ch5mpy/indexing/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      210 2023-05-04 09:56:15.000000 ch5mpy-0.2/ch5mpy/indexing/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      403 2023-05-04 09:53:30.000000 ch5mpy-0.2/ch5mpy/indexing/_typing.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3193 2023-05-09 13:33:47.000000 ch5mpy-0.2/ch5mpy/indexing/list.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    16101 2023-06-09 16:37:50.000000 ch5mpy-0.2/ch5mpy/indexing/selection.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4565 2023-06-07 09:35:55.000000 ch5mpy-0.2/ch5mpy/indexing/slice.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1385 2023-05-04 09:54:41.000000 ch5mpy-0.2/ch5mpy/indexing/special.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3734 2023-06-16 14:11:05.000000 ch5mpy-0.2/ch5mpy/list.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      725 2023-06-27 13:11:28.000000 ch5mpy-0.2/ch5mpy/names.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      648 2023-04-17 14:55:50.000000 ch5mpy-0.2/ch5mpy/np.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.924226 ch5mpy-0.2/ch5mpy/objects/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      203 2023-05-30 07:23:40.000000 ch5mpy-0.2/ch5mpy/objects/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     8185 2023-06-20 13:23:29.000000 ch5mpy-0.2/ch5mpy/objects/dataset.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6874 2023-06-20 13:23:29.000000 ch5mpy-0.2/ch5mpy/objects/group.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2122 2023-06-06 14:12:48.000000 ch5mpy-0.2/ch5mpy/objects/object.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1144 2023-05-30 07:25:38.000000 ch5mpy-0.2/ch5mpy/objects/pickle.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      740 2023-06-06 12:27:59.000000 ch5mpy-0.2/ch5mpy/options.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2016 2023-05-24 13:11:19.000000 ch5mpy-0.2/ch5mpy/read.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      658 2023-04-17 14:55:50.000000 ch5mpy-0.2/ch5mpy/utils.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5529 2023-05-30 07:34:03.000000 ch5mpy-0.2/ch5mpy/write.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.920226 ch5mpy-0.2/ch5mpy.egg-info/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    39503 2023-06-27 14:06:08.000000 ch5mpy-0.2/ch5mpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1589 2023-06-27 14:06:08.000000 ch5mpy-0.2/ch5mpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-06-27 14:06:08.000000 ch5mpy-0.2/ch5mpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)       93 2023-06-27 14:06:08.000000 ch5mpy-0.2/ch5mpy.egg-info/requires.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        7 2023-06-27 14:06:08.000000 ch5mpy-0.2/ch5mpy.egg-info/top_level.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1828 2023-06-27 14:02:55.000000 ch5mpy-0.2/pyproject.toml
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)       38 2023-06-27 14:06:08.924226 ch5mpy-0.2/setup.cfg
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-06-27 14:06:08.924226 ch5mpy-0.2/tests/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      517 2023-03-15 09:19:15.000000 ch5mpy-0.2/tests/test_array_creation.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2169 2023-02-15 17:14:15.000000 ch5mpy-0.2/tests/test_array_repr.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      556 2023-03-15 09:55:44.000000 ch5mpy-0.2/tests/test_chunked_array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1145 2023-02-16 18:29:12.000000 ch5mpy-0.2/tests/test_complex_object_h5array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      532 2023-05-04 09:54:46.000000 ch5mpy-0.2/tests/test_full_slice.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    11993 2023-05-04 14:27:57.000000 ch5mpy-0.2/tests/test_functions.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12729 2023-05-04 09:56:16.000000 ch5mpy-0.2/tests/test_get_chunks.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1955 2023-06-19 12:44:35.000000 ch5mpy-0.2/tests/test_h5_list.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    13528 2023-06-07 09:35:55.000000 ch5mpy-0.2/tests/test_h5array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4479 2023-05-30 07:36:37.000000 ch5mpy-0.2/tests/test_h5dict.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      802 2023-02-15 17:14:15.000000 ch5mpy-0.2/tests/test_pickle.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      562 2023-03-03 23:51:35.000000 ch5mpy-0.2/tests/test_repeated_array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5051 2023-05-11 14:31:16.000000 ch5mpy-0.2/tests/test_selection.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1418 2023-03-15 16:13:04.000000 ch5mpy-0.2/tests/test_str_h5array.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2230 2023-05-24 09:14:55.000000 ch5mpy-0.2/tests/test_write.py
```

### Comparing `ch5mpy-0.1.3/LICENSE` & `ch5mpy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/functions/implement.py` & `ch5mpy-0.2/ch5mpy/h5array/functions/implement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from __future__ import annotations
 
 import importlib
-import numpy as np
+from functools import partial
 
 from typing import Callable
 
 from ch5mpy._typing import NP_FUNC
 from ch5mpy._typing import H5_FUNC
 
 
 # ====================================================
 # code
-HANDLED_FUNCTIONS: dict[NP_FUNC | np.ufunc, H5_FUNC] = {}
+HANDLED_FUNCTIONS: dict[NP_FUNC | NP_FUNC, H5_FUNC] = {}
 
 
-def implements(np_function: NP_FUNC | np.ufunc) -> Callable[[H5_FUNC], H5_FUNC]:
-    """Register an __array_function__ implementation for DiagonalArray objects."""
+def implements(*np_functions: NP_FUNC | NP_FUNC) -> Callable[[H5_FUNC], H5_FUNC]:
+    """Register an __array_function__ implementation for H5Array objects."""
 
     def decorator(func: H5_FUNC) -> H5_FUNC:
-        HANDLED_FUNCTIONS[np_function] = func
+        for f in np_functions:
+            HANDLED_FUNCTIONS[f] = func
         return func
 
     return decorator
 
 
+def register(function: partial[H5_FUNC], implements: NP_FUNC) -> None:
+    HANDLED_FUNCTIONS[implements] = function
+
+
 # manually import function implementations otherwise they are never imported
+importlib.__import__("ch5mpy.h5array.functions.routines")
+importlib.__import__("ch5mpy.h5array.functions.creation_routines")
 importlib.__import__("ch5mpy.h5array.functions.two_arrays")
 importlib.__import__("ch5mpy.h5array.functions.element_wise")
```

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/functions/two_arrays.py` & `ch5mpy-0.2/ch5mpy/h5array/functions/two_arrays.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,302 +9,566 @@
 
 import numpy.typing as npt
 from typing import Any
 from typing import Iterable
 from typing import TYPE_CHECKING
 
 import ch5mpy
-from ch5mpy.h5array.inplace import iter_chunks_2
 from ch5mpy.h5array.functions.apply import apply_2
+from ch5mpy.h5array.functions.apply import str_apply_2
 from ch5mpy.h5array.functions.implement import implements
 
 
 if TYPE_CHECKING:
     from ch5mpy import H5Array
 
 
 # ====================================================
 # code
 def _cast_H5Array(obj: Any) -> H5Array[Any]:
-    return obj                                                                             # type: ignore[no-any-return]
+    return obj  # type: ignore[no-any-return]
 
 
-def ensure_h5array_first(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                         x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any]) \
-        -> tuple[H5Array[Any], npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any]]:
+def ensure_h5array_first(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+) -> tuple[H5Array[Any], npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any]]:
     if not isinstance(x1, ch5mpy.H5Array):
         return _cast_H5Array(x2), x1
 
     return _cast_H5Array(x1), x2
 
 
 @implements(np.array_equal)
-def array_equal(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                equal_nan: bool = False) -> bool:
+def array_equal(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    equal_nan: bool = False,
+) -> bool:
     x1, x2 = ensure_h5array_first(x1, x2)
 
     # case 0D
     if isinstance(x2, Number):
         if x1.ndim:
             return False
 
-        return np.array_equal(x1, x2, equal_nan=equal_nan)                                  # type: ignore[arg-type]
+        return np.array_equal(x1, x2, equal_nan=equal_nan)  # type: ignore[arg-type]
 
     # case nD
     if not isinstance(x2, (np.ndarray, ch5mpy.H5Array)):
         x2 = np.array(x2)
 
     if x1.shape != x2.shape:
         return False
 
-    for index, chunk_x1, chunk_x2 in iter_chunks_2(x1, x2):
-        if not np.array_equal(chunk_x1, chunk_x2):                                              # type: ignore[arg-type]
+    for index, chunk_x1, chunk_x2 in x1.iter_chunks_with(x2):
+        if not np.array_equal(chunk_x1, chunk_x2):
             return False
 
     return True
 
 
 @implements(np.greater)
-def greater(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            out: H5Array[Any] | npt.NDArray[Any] | None = None,
-            where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-            dtype: npt.DTypeLike | None = None) -> Any:
+def greater(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.greater, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.greater,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.greater)
+def str_greater(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.greater, x1, x2)
 
 
 @implements(np.greater_equal)
-def greater_equal(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                  x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                  out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                  where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                  dtype: npt.DTypeLike | None = None) -> Any:
+def greater_equal(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.greater_equal, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.greater_equal,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.greater_equal)
+def str_greater_equal(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.greater_equal, x1, x2)
 
 
 @implements(np.less)
-def less(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         out: H5Array[Any] | npt.NDArray[Any] | None = None,
-         where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-         dtype: npt.DTypeLike | None = None) -> Any:
+def less(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.less, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.less,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.less)
+def str_less(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.less, x1, x2)
 
 
 @implements(np.less_equal)
-def less_equal(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-               x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-               out: H5Array[Any] | npt.NDArray[Any] | None = None,
-               where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-               dtype: npt.DTypeLike | None = None) -> Any:
+def less_equal(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.less_equal, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.less_equal,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.less_equal)
+def str_less_equal(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.less_equal, x1, x2)
 
 
 @implements(np.equal)
-def equal(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-          x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-          out: H5Array[Any] | npt.NDArray[Any] | None = None,
-          where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-          dtype: npt.DTypeLike | None = None) -> Any:
+def equal(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.equal, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.equal,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.equal)
+def str_equal(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.equal, x1, x2)
 
 
 @implements(np.not_equal)
-def not_equal(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-              x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-              out: H5Array[Any] | npt.NDArray[Any] | None = None,
-              where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-              dtype: npt.DTypeLike | None = None) -> Any:
+def not_equal(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.not_equal, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=False)
+    return apply_2(
+        np.not_equal,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=False,
+    )
+
+
+@implements(np.char.not_equal)
+def str_not_equal(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.not_equal, x1, x2)
 
 
 @implements(np.add)
-def add(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-        x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-        out: H5Array[Any] | npt.NDArray[Any] | None = None,
-        where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-        dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.add, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def add(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.add,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
+
+
+@implements(np.char.add)
+def str_add(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.add, x1, x2)
 
 
 @implements(np.multiply)
-def multiply(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-             x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-             out: H5Array[Any] | npt.NDArray[Any] | None = None,
-             where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-             dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.multiply, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def multiply(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.multiply,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
+
+
+@implements(np.char.multiply)
+def str_multiply(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.multiply, x1, x2)
 
 
 @implements(np.divide)
-def divide(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-           x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-           out: H5Array[Any] | npt.NDArray[Any] | None = None,
-           where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-           dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.divide, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def divide(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.divide,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.power)
-def power(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-          x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-          out: H5Array[Any] | npt.NDArray[Any] | None = None,
-          where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-          dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.power, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def power(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.power,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.subtract)
-def subtract(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-             x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-             out: H5Array[Any] | npt.NDArray[Any] | None = None,
-             where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-             dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.subtract, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def subtract(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.subtract,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.true_divide)
-def true_divide(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.true_divide, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def true_divide(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.true_divide,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.floor_divide)
-def floor_divide(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                 x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                 out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                 where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                 dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.floor_divide, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def floor_divide(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.floor_divide,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.float_power)
-def float_power(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.float_power, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def float_power(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.float_power,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.fmod)
-def fmod(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         out: H5Array[Any] | npt.NDArray[Any] | None = None,
-         where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-         dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.fmod, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def fmod(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.fmod,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.mod)
-def mod(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-        x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-        out: H5Array[Any] | npt.NDArray[Any] | None = None,
-        where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-        dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.mod, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def mod(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.mod,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
+
+
+@implements(np.char.mod)
+def str_mod(x1: str | npt.NDArray[np.str_] | Iterable[str] | H5Array[np.str_], x2: Any) -> Any:
+    return str_apply_2(np.char.mod, x1, x2)
 
 
 @implements(np.maximum)
-def maximum(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            out: H5Array[Any] | npt.NDArray[Any] | None = None,
-            where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-            dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.maximum, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def maximum(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.maximum,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.fmax)
-def fmax(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         out: H5Array[Any] | npt.NDArray[Any] | None = None,
-         where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-         dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.fmax, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def fmax(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.fmax,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.minimum)
-def minimum(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-            out: H5Array[Any] | npt.NDArray[Any] | None = None,
-            where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-            dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.minimum, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def minimum(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.minimum,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.fmin)
-def fmin(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-         out: H5Array[Any] | npt.NDArray[Any] | None = None,
-         where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-         dtype: npt.DTypeLike | None = None) -> Any:
-    return apply_2(np.fmin, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+def fmin(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
+    return apply_2(
+        np.fmin,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.logical_and)
-def logical_and(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                dtype: npt.DTypeLike | None = None) -> Any:
+def logical_and(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.logical_and, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+    return apply_2(
+        np.logical_and,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.logical_or)
-def logical_or(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-               x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-               out: H5Array[Any] | npt.NDArray[Any] | None = None,
-               where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-               dtype: npt.DTypeLike | None = None) -> Any:
+def logical_or(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.logical_or, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+    return apply_2(
+        np.logical_or,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.logical_not)
-def logical_not(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                dtype: npt.DTypeLike | None = None) -> Any:
+def logical_not(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.logical_not, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+    return apply_2(
+        np.logical_not,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
 
 
 @implements(np.logical_xor)
-def logical_xor(x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
-                out: H5Array[Any] | npt.NDArray[Any] | None = None,
-                where: npt.NDArray[np.bool_] | Iterable[bool] | bool = True,
-                dtype: npt.DTypeLike | None = None) -> Any:
+def logical_xor(
+    x1: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    x2: npt.NDArray[Any] | Iterable[Any] | Number | H5Array[Any],
+    out: H5Array[Any] | npt.NDArray[Any] | None = None,
+    where: npt.NDArray[np.bool_] | Iterable[bool] | bool | int = True,
+    dtype: npt.DTypeLike | None = None,
+) -> Any:
     if dtype is None:
         dtype = bool
 
-    return apply_2(np.logical_xor, *ensure_h5array_first(x1, x2), out=out, dtype=dtype, where=where, default=x1)
+    return apply_2(
+        np.logical_xor,
+        *ensure_h5array_first(x1, x2),
+        out=out,
+        dtype=dtype,
+        where=where,
+        default=x1,
+    )
```

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/h5array.py` & `ch5mpy-0.2/ch5mpy/h5array/array.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,258 +1,371 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from __future__ import annotations
 
-import numpy as np
-import numpy.lib.mixins
 from numbers import Number
+from typing import TYPE_CHECKING, Any, Collection, Iterator, TypeVar
 
+import numpy as np
+import numpy.lib.mixins
 import numpy.typing as npt
-from typing import Any
-from typing import cast
-from typing import Generic
-from typing import TypeVar
-from typing import Iterator
-from typing import Generator
-from typing import TYPE_CHECKING
-from ch5mpy._typing import NP_FUNC
-from ch5mpy._typing import SELECTOR
 
-from ch5mpy import Dataset
+from ch5mpy._typing import NP_FUNC, SELECTOR
 from ch5mpy.h5array import repr
-from ch5mpy.h5array.inplace import get_chunks
-from ch5mpy.h5array.inplace import get_work_array
+from ch5mpy.h5array.chunks.iter import ChunkIterator, PairedChunkIterator
 from ch5mpy.h5array.functions import HANDLED_FUNCTIONS
-from ch5mpy.h5array.io import parse_selector
-from ch5mpy.h5array.io import write_to_dataset
-from ch5mpy.h5array.slice import FullSlice
-from ch5mpy.h5array.slice import map_slice
+from ch5mpy.h5array.io import read_one_from_dataset, write_to_dataset
+from ch5mpy.indexing import Selection, map_slice
+from ch5mpy.objects.dataset import Dataset, DatasetWrapper
+from ch5mpy.write import write_dataset
 
 if TYPE_CHECKING:
-    from ch5mpy.h5array.subset import H5ArrayView
+    from ch5mpy.h5array.view import H5ArrayView
 
 
 # ====================================================
 # code
-_T = TypeVar("_T", bound=np.generic)
+_T = TypeVar("_T", bound=np.generic, covariant=True)
+SIZES = {"K": 1024, "M": 1024 * 1024, "G": 1024 * 1024 * 1024}
+
+
+def get_size(s: int | str) -> int:
+    value: int | None = None
+
+    if isinstance(s, int):
+        value = s
+
+    elif s[-1] in SIZES and s[:-1].lstrip("-").isdigit():
+        value = int(s[:-1]) * SIZES[s[-1]]
+
+    elif s.isdigit():
+        value = int(s)
+
+    if value is None:
+        raise ValueError(f"Unrecognized size '{s}'")
+
+    if value <= 0:
+        raise ValueError(f"Got invalid size ({value} <= 0).")
+
+    return value
+
+
+def as_array(values: Any, dtype: np.dtype[Any]) -> npt.NDArray[Any]:
+    # FIXME : work on H5Arrays directly instead of converting to np.array
+    if np.issubdtype(dtype, str):
+        return np.array(values, dtype=bytes)
+
+    try:
+        return np.array(values, dtype=dtype)
+
+    except ValueError:
+        raise ValueError(f"Couldn't set value of type {type(values)} in H5Array of type {dtype}.")
 
 
-class H5Array(Generic[_T], numpy.lib.mixins.NDArrayOperatorsMixin):
+def _dtype_repr(dset: Dataset[Any] | DatasetWrapper[Any]) -> str:
+    if np.issubdtype(dset.dtype, np.str_):
+        return f"'{dset.dtype}'"
+
+    return str(dset.dtype)
+
+
+class H5Array(Collection[_T], numpy.lib.mixins.NDArrayOperatorsMixin):
     """Wrapper around Dataset objects to interface with numpy's API."""
 
     MAX_MEM_USAGE: int | str = "250M"
 
     # region magic methods
-    def __init__(self, dset: Dataset[_T]):
-        if not isinstance(dset, Dataset):
-            raise TypeError(
-                f"Object of type '{type(dset)}' is not supported by H5Array."
-            )
+    def __init__(self, dset: Dataset[_T] | DatasetWrapper[_T]):
+        if not isinstance(dset, (Dataset, DatasetWrapper)):
+            raise TypeError(f"Object of type '{type(dset)}' is not supported by H5Array.")
 
-        self._dset = dset
+        if isinstance(dset, Dataset) and np.issubdtype(np.dtype(str(dset.attrs.get("dtype", "O"))), str):
+            self._dset: Dataset[_T] | DatasetWrapper[_T] = dset.asstr()  # type: ignore[assignment]
+
+        else:
+            self._dset = dset
 
     def __repr__(self) -> str:
         return (
             f"H5Array({repr.print_dataset(self, end='', padding=8, padding_skip_first=True)}, "
-            f"shape={self.shape}, dtype={self._dset.dtype})"
+            f"shape={self.shape}, dtype={_dtype_repr(self._dset)})"
         )
 
     def __str__(self) -> str:
         return repr.print_dataset(self, sep="")
 
     def __getitem__(self, index: SELECTOR | tuple[SELECTOR, ...]) -> _T | H5Array[_T] | H5ArrayView[_T]:
-        from ch5mpy.h5array.subset import H5ArrayView
+        from ch5mpy.h5array.view import H5ArrayView
 
-        selection, nb_elements = parse_selector(self.shape, index)
+        selection = Selection.from_selector(index, self.shape)
 
-        if nb_elements == 1:
-            return cast(_T, self._dset[cast(SELECTOR, index)])
-
-        elif selection is None:
+        if selection.is_empty:
             return H5Array(dset=self._dset)
 
+        elif selection.compute_shape(self._dset.shape) == ():
+            return read_one_from_dataset(self._dset, selection, self.dtype)
+
         else:
             return H5ArrayView(dset=self._dset, sel=selection)
 
     def __setitem__(self, index: SELECTOR | tuple[SELECTOR, ...], value: Any) -> None:
-        selection, nb_elements = parse_selector(self.shape, index)
-
-        try:
-            value_arr = np.array(value, dtype=self.dtype)
-
-        except ValueError:
-            raise ValueError(f'Could set value of type {type(value)} in H5Array of type {self.dtype}.')
-
-        if nb_elements != value_arr.size:
-            raise ValueError(f"{' x '.join(map(str, self.shape if selection is None else map(len, selection)))} "
-                             f"values were selected but {' x '.join(map(str, value_arr.shape))} were given.")
-
-        if selection is None:
-            self._dset[()] = value_arr
-
-        else:
-            write_to_dataset(self._dset, value_arr, selection)
+        selection = Selection.from_selector(index, self.shape)
+        write_to_dataset(self._dset, as_array(value, self.dtype), selection)
 
     def __len__(self) -> int:
         return len(self._dset)
 
-    def __iter__(self) -> Iterator[_T | npt.NDArray[_T] | H5Array[_T] | H5ArrayView[_T]]:
+    def __iter__(self) -> Iterator[_T | npt.NDArray[_T] | H5Array[_T] | H5ArrayView[_T]]:  # type: ignore[override]
         for i in range(self.shape[0]):
             yield self[i]
 
     def __contains__(self, item: Any) -> bool:
-        raise NotImplementedError
+        for _, chunk in self.iter_chunks():
+            if item in chunk:
+                return True
+
+        return False
 
-    def _inplace_operation(self, func: NP_FUNC, value: Any) -> H5Array[_T]:
+    def _inplace(self, func: NP_FUNC, value: Any) -> H5Array[_T]:
+        if np.issubdtype(self.dtype, str):
+            raise TypeError("Cannot perform inplace operation on str H5Array.")
+
+        # special case : 0D array
         if self.shape == ():
             self._dset[:] = func(self._dset[:], value)
+            return self
 
-        else:
-            chunks = get_chunks(self.MAX_MEM_USAGE, self.shape, self.dtype.itemsize)
-            work_array = get_work_array(self.shape, chunks[0], dtype=self.dtype)
-
-            for chunk in chunks:
-                work_subset = map_slice(c.shift_to_zero() for c in chunk)
-                dataset_subset = map_slice(chunk)
-
-                self._dset.read_direct(work_array, source_sel=dataset_subset, dest_sel=work_subset)
-                func(work_array, value, out=work_array)
-                self._dset.write_direct(work_array, source_sel=work_subset, dest_sel=dataset_subset)
+        # general case : 1D+ array
+        for index, chunk in self.iter_chunks():
+            func(chunk, value, out=chunk)
+
+            # write back result into array
+            self.dset.write_direct(
+                chunk,
+                source_sel=map_slice(index, shift_to_zero=True),
+                dest_sel=map_slice(index),
+            )
 
         return self
 
     def __add__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] + other                                                      # type: ignore[no-any-return]
+        return np.array(self) + other  # type: ignore[no-any-return]
 
     def __iadd__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.add, other)
+        return self._inplace(np.add, other)
 
     def __sub__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] - other                                                      # type: ignore[no-any-return]
+        return np.array(self) - other  # type: ignore[no-any-return]
 
     def __isub__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.subtract, other)
+        return self._inplace(np.subtract, other)
 
     def __mul__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] * other                                                      # type: ignore[no-any-return]
+        return np.array(self) * other  # type: ignore[no-any-return]
 
     def __imul__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.multiply, other)
+        return self._inplace(np.multiply, other)
 
     def __truediv__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] / other                                                      # type: ignore[no-any-return]
+        return np.array(self) / other  # type: ignore[no-any-return]
 
     def __itruediv__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.divide, other)
+        return self._inplace(np.divide, other)
 
     def __mod__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] % other                                                      # type: ignore[no-any-return]
+        return np.array(self) % other  # type: ignore[no-any-return]
 
     def __imod__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.mod, other)
+        return self._inplace(np.mod, other)
 
     def __pow__(self, other: Any) -> Number | str | npt.NDArray[Any]:
-        return self._dset[()] ** other                                                     # type: ignore[no-any-return]
+        return np.array(self) ** other  # type: ignore[no-any-return]
 
     def __ipow__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.power, other)
+        return self._inplace(np.power, other)
 
     def __or__(self, other: Any) -> Number | npt.NDArray[Any]:
-        return self._dset[()] | other                                                      # type: ignore[no-any-return]
+        return np.array(self) | other  # type: ignore[no-any-return]
 
     def __ior__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.logical_or, other)
+        return self._inplace(np.logical_or, other)
 
     def __and__(self, other: Any) -> Number | npt.NDArray[Any]:
-        return self._dset[()] & other                                                      # type: ignore[no-any-return]
+        return np.array(self) & other  # type: ignore[no-any-return]
 
     def __iand__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.logical_and, other)
+        return self._inplace(np.logical_and, other)
 
     def __invert__(self) -> Number | npt.NDArray[Any]:
-        return ~self._dset[()]                                                                  # type: ignore[operator]
+        return ~np.array(self)
 
     def __xor__(self, other: Any) -> Number | npt.NDArray[Any]:
-        return self._dset[()] ^ other                                                      # type: ignore[no-any-return]
+        return np.array(self) ^ other  # type: ignore[no-any-return]
 
     def __ixor__(self, other: Any) -> H5Array[_T]:
-        return self._inplace_operation(np.logical_xor, other)
+        return self._inplace(np.logical_xor, other)
 
     # endregion
 
     # region interface
     def __array__(self, dtype: npt.DTypeLike | None = None) -> npt.NDArray[Any]:
-        return np.array(self._dset).astype(dtype)
+        array = np.array(self._dset)
 
-    def __array_ufunc__(self, ufunc: NP_FUNC, method: str, *inputs: Any, **kwargs: Any) \
-            -> Any:
+        if dtype is None:
+            return array
+
+        return array.astype(dtype)
+
+    def __array_ufunc__(self, ufunc: NP_FUNC, method: str, *inputs: Any, **kwargs: Any) -> Any:
         if method == "__call__":
             if ufunc not in HANDLED_FUNCTIONS:
                 return NotImplemented
 
             return HANDLED_FUNCTIONS[ufunc](*inputs, **kwargs)
 
         else:
-            raise NotImplemented
+            raise NotImplementedError
 
     def __array_function__(
         self,
         func: NP_FUNC,
         types: tuple[type, ...],
         args: tuple[Any, ...],
         kwargs: dict[str, Any],
     ) -> Any:
+        del types
+
         if func not in HANDLED_FUNCTIONS:
             return NotImplemented
 
         return HANDLED_FUNCTIONS[func](*args, **kwargs)
 
     # endregion
 
+    # region predicates
+    @property
+    def is_chunked(self) -> bool:
+        return self._dset.chunks is not None
+
+    # endregion
+
     # region attributes
     @property
-    def dset(self) -> Dataset[_T]:
+    def dset(self) -> Dataset[_T] | DatasetWrapper[_T]:
         return self._dset
 
     @property
+    def chunk_size(self) -> int:
+        """Get the size of a chunk (i.e. the nb of elements that can be read/written at a time)."""
+        return get_size(self.MAX_MEM_USAGE) // self._dset.dtype.itemsize
+
+    @property
     def shape(self) -> tuple[int, ...]:
         return self._dset.shape
 
     @property
     def dtype(self) -> np.dtype[_T]:
         return self._dset.dtype
 
     @property
     def ndim(self) -> int:
         return len(self.shape)
 
+    @property
+    def size(self) -> int:
+        return int(np.prod(self.shape))
+
     # endregion
 
     # region methods
-    def astype(self, dtype: npt.DTypeLike) -> npt.NDArray[Any]:
-        return np.array(self, dtype=dtype)
+    def _resize(self, amount: int, axis: int | tuple[int, ...] | None = None) -> None:
+        if axis is None:
+            axis = 0
 
-    def iter_chunks(self, keepdims: bool = False) \
-            -> Generator[tuple[tuple[FullSlice, ...], npt.NDArray[_T]], None, None]:
-        chunks = get_chunks(self.MAX_MEM_USAGE, self.shape, self.dtype.itemsize)
-        work_array = get_work_array(self.shape, chunks[0], dtype=self.dtype)
-
-        for chunk in chunks:
-            work_subset = map_slice(c.shift_to_zero() for c in chunk)
-            self._dset.read_direct(work_array, source_sel=map_slice(chunk), dest_sel=work_subset)
-
-            if keepdims:
-                res = work_array[work_subset]
-                yield chunk, res.reshape((1,) * (self.ndim - res.ndim) + res.shape)
+        if isinstance(axis, int):
+            self._dset.resize(self.shape[axis] + amount, axis=axis)
+
+        else:
+            self._dset.resize([s + amount if i in axis else s for i, s in enumerate(self.shape)])
+
+    def expand(self, amount: int, axis: int | tuple[int, ...] | None = None) -> None:
+        """
+        Resize an H5Array by adding `amount` elements along the selected axis.
+
+        Raises:
+            TypeError: if the H5Array does not wrap a chunked Dataset.
+        """
+        self._resize(amount, axis)
+
+    def contract(self, amount: int, axis: int | tuple[int, ...] | None = None) -> None:
+        """
+        Resize an H5Array by removing `amount` elements along the selected axis.
+
+        Raises:
+            TypeError: if the H5Array does not wrap a chunked Dataset.
+        """
+        self._resize(-amount, axis)
+
+    def astype(self, dtype: npt.DTypeLike, inplace: bool = False) -> H5Array[Any]:
+        """
+        Cast an H5Array to a specified dtype.
+        This does not perform a copy, it returns a wrapper around the underlying H5 dataset.
+        """
+        if np.issubdtype(dtype, str) and (np.issubdtype(self._dset.dtype, str) or self._dset.dtype == object):
+            new_dset = self._dset.asstr()
+
+        else:
+            new_dset = self._dset.astype(dtype)
+
+        if inplace:
+            file, name = self._dset.file, self._dset.name
+            del file[name]
+
+            # FIXME : conversion to np happens anyway but might be expensive, could we save data without conversion ?
+            write_dataset(file, name, np.array(new_dset), chunks=new_dset.chunks, maxshape=new_dset.maxshape)
+
+            if file[name].dtype == object:
+                self._dset = file[name].asstr()
 
             else:
-                yield chunk, work_array[work_subset]
+                self._dset = file[name]
+
+        return H5Array(new_dset)
+
+    def maptype(self, otype: type[Any]) -> H5Array[Any]:
+        """
+        Cast an H5Array to any object type.
+        This extends H5Array.astype() to any type <T>, where it is required that an object <T> can be constructed as
+        T(v) for any value <v> in the dataset.
+        """
+        return H5Array(self._dset.maptype(otype))
+
+    def iter_chunks(self, keepdims: bool = False) -> ChunkIterator:
+        return ChunkIterator(self, keepdims)
+
+    def iter_chunks_with(self, other: npt.NDArray[Any] | H5Array[Any], keepdims: bool = False) -> PairedChunkIterator:
+        return PairedChunkIterator(self, other, keepdims)
+
+    def read_direct(
+        self,
+        dest: npt.NDArray[_T],
+        source_sel: tuple[slice, ...],
+        dest_sel: tuple[slice, ...],
+    ) -> None:
+        dset = self._dset.asstr() if np.issubdtype(self.dtype, str) else self._dset
+        dset.read_direct(dest, source_sel=source_sel, dest_sel=dest_sel)
+
+    def copy(self) -> npt.NDArray[_T]:
+        return np.copy(self)
+
+    def min(self, axis: int | tuple[int, ...] | None = None) -> _T | npt.NDArray[_T]:
+        return np.min(self, axis=axis)  # type: ignore[no-any-return]
+
+    def max(self, axis: int | tuple[int, ...] | None = None) -> _T | npt.NDArray[_T]:
+        return np.max(self, axis=axis)  # type: ignore[no-any-return]
 
-    def read_direct(self,
-                    dest: npt.NDArray[_T],
-                    source_sel: tuple[FullSlice, ...],
-                    dest_sel: tuple[FullSlice, ...]) -> None:
-        self._dset.read_direct(dest, source_sel=map_slice(source_sel), dest_sel=map_slice(dest_sel))
+    def mean(self, axis: int | tuple[int, ...] | None = None) -> Any | npt.NDArray[Any]:
+        return np.mean(self, axis=axis)
 
     # endregion
```

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/inplace.py` & `ch5mpy-0.2/ch5mpy/h5array/chunks/iter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,163 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from __future__ import annotations
 
 from numbers import Number
-from typing import Generator
-from typing import cast
+from typing import TYPE_CHECKING, Any, Generator, TypeVar, cast
 
 import numpy as np
-
 import numpy.typing as npt
-from typing import Any
-from typing import TypeVar
-from typing import TYPE_CHECKING
 
 import ch5mpy
-from ch5mpy.h5array.slice import FullSlice
+from ch5mpy.h5array.chunks.repeated_array import RepeatedArray
+from ch5mpy.h5array.chunks.utils import _as_valid_dtype
+from ch5mpy.indexing import FullSlice, map_slice
 
 if TYPE_CHECKING:
     from ch5mpy import H5Array
 
+
 # ====================================================
 # code
 _DT = TypeVar("_DT", bound=np.generic)
 INF = np.iinfo(int).max
 
 
-sizes = {"K": 1024, "M": 1024 * 1024, "G": 1024 * 1024 * 1024}
-
-
-def get_size(s: int | str) -> int:
-    value: int | None = None
-
-    if isinstance(s, int):
-        value = s
-
-    elif s[-1] in sizes and s[:-1].lstrip("-").isdigit():
-        value = int(s[:-1]) * sizes[s[-1]]
-
-    elif s.isdigit():
-        value = int(s)
-
-    if value is None:
-        raise ValueError(f"Unrecognized size '{s}'")
-
-    if value <= 0:
-        raise ValueError(f"Got invalid size ({value} <= 0).")
+def get_work_array(shape: tuple[int, ...], slicer: tuple[FullSlice, ...], dtype: np.dtype[_DT]) -> npt.NDArray[_DT]:
+    if len(slicer) == 1 and slicer[0].is_whole_axis():
+        return np.empty(shape, dtype=object if np.issubdtype(dtype, str) else dtype)
 
-    return value
+    slicer_shape = tuple(len(s) for s in slicer)
+    return np.empty(slicer_shape, dtype=object if np.issubdtype(dtype, str) else dtype)
 
 
-def get_chunks(max_memory_usage: int | str,
-               shape: tuple[int, ...],
-               itemsize: int) -> tuple[tuple[FullSlice, ...], ...]:
+def _get_chunk_indices(chunk_size: int, shape: tuple[int, ...]) -> tuple[tuple[FullSlice, ...], ...]:
     # special case of 0D arrays
     if len(shape) == 0:
         raise ValueError("0D array")
 
+    if np.prod(shape) == 0:
+        return (tuple(FullSlice.whole_axis(s) for s in shape),)
+
     rev_shape = tuple(reversed(shape))
-    nb_elements_chunk = int(get_size(max_memory_usage) / itemsize)
 
     # not enough max mem
-    if nb_elements_chunk <= 1:
-        raise ValueError(
-            "Slicing is impossible because of insufficient allowed memory usage."
-        )
+    if chunk_size <= 1:
+        raise ValueError("Slicing is impossible because of insufficient allowed memory usage.")
 
-    block_axes = int(np.argmax(~(np.cumprod(rev_shape + (np.inf,)) <= nb_elements_chunk)))
-    size_block = (
-        nb_elements_chunk // np.cumprod(rev_shape)[block_axes - 1]
-        if block_axes
-        else min(rev_shape[0], nb_elements_chunk)
-    )
+    block_axes = int(np.argmax(~(np.cumprod(rev_shape + (np.inf,)) <= chunk_size)))
+    size_block = chunk_size // np.cumprod(rev_shape)[block_axes - 1] if block_axes else min(rev_shape[0], chunk_size)
 
     if size_block == 0:
         block_axes = max(0, block_axes - 1)
 
     if block_axes == len(shape):
         # all array can be read at once
-        return ((FullSlice.whole_axis(shape[0]),),)
+        return (tuple(FullSlice.whole_axis(s) for s in shape),)
 
     whole_axes = tuple(FullSlice.whole_axis(s) for s in rev_shape[:block_axes][::-1])
     iter_axis = rev_shape[block_axes]
 
     right_chunks = tuple(
         (FullSlice(s, min(s + size_block, iter_axis), 1, iter_axis), *whole_axes)
         for s in range(0, iter_axis, size_block)
     )
 
     if block_axes + 1 == len(shape):
         return right_chunks
 
-    left_shape = shape[:-(block_axes+1)]
-    left_chunks = np.array(np.meshgrid(*map(range, left_shape))).T.reshape(
-        -1, len(left_shape)
-    )
+    left_shape = shape[: -(block_axes + 1)]
+    left_chunks = np.array(np.meshgrid(*map(range, left_shape))).T.reshape(-1, len(left_shape))
 
     return tuple(
         tuple(map(FullSlice.one, left, shape)) + tuple(right) for left in left_chunks for right in right_chunks
     )
 
 
-def _len(obj: int | FullSlice) -> int:
-    if isinstance(obj, FullSlice):
-        return len(obj)
-
-    return 1
+class ChunkIterator:
+    def __init__(self, array: H5Array[Any], keepdims: bool = False):
+        self._array = array
+        self._keepdims = keepdims
+
+        self._chunk_indices = _get_chunk_indices(array.chunk_size, array.shape)
+
+        self._work_array = get_work_array(array.shape, self._chunk_indices[0], dtype=array.dtype)
+
+    def __repr__(self) -> str:
+        return f"<ChunkIterator over {self._array.shape} H5Array>"
+
+    def __iter__(
+        self,
+    ) -> Generator[tuple[tuple[FullSlice, ...], npt.NDArray[Any]], None, None]:
+        for index in self._chunk_indices:
+            work_subset = map_slice(index, shift_to_zero=True)
+            self._array.read_direct(self._work_array, source_sel=map_slice(index), dest_sel=work_subset)
+
+            # cast to str if needed
+            res = _as_valid_dtype(self._work_array, self._array.dtype)[work_subset]
+
+            # reshape to keep dimensions if needed
+            if self._keepdims:
+                res = res.reshape((1,) * (self._array.ndim - res.ndim) + res.shape)
+
+            yield index, res
+
+
+class PairedChunkIterator:
+    def __init__(
+        self,
+        arr_1: H5Array[Any] | npt.NDArray[Any],
+        arr_2: H5Array[Any] | npt.NDArray[Any],
+        keepdims: bool = False,
+    ):
+        broadcasted_shape = np.broadcast_shapes(arr_1.shape, arr_2.shape)
+        self._arr_1 = RepeatedArray(arr_1, broadcasted_shape)
+        self._arr_2 = RepeatedArray(arr_2, broadcasted_shape)
+
+        self._keepdims = keepdims
+
+        chunk_size = min(
+            arr_1.chunk_size if isinstance(arr_1, ch5mpy.H5Array) else INF,
+            arr_2.chunk_size if isinstance(arr_2, ch5mpy.H5Array) else INF,
+        )
 
+        self._chunk_indices = _get_chunk_indices(chunk_size, shape=arr_1.shape)
 
-def get_work_array(shape: tuple[int, ...],
-                   slicer: tuple[FullSlice, ...],
-                   dtype: np.dtype[_DT]) -> npt.NDArray[_DT]:
-    if len(slicer) == 1 and slicer[0].is_whole_axis():
-        return np.empty(shape, dtype=dtype)
+        self._work_array_1 = get_work_array(broadcasted_shape, self._chunk_indices[0], dtype=arr_1.dtype)
+        self._work_array_2 = get_work_array(broadcasted_shape, self._chunk_indices[0], dtype=arr_2.dtype)
 
-    slicer_shape = tuple(_len(s) for s in slicer)
-    return np.empty(slicer_shape, dtype=dtype)
+    def __repr__(self) -> str:
+        return f"<PairedChunkIterator over 2 {self._arr_1.shape} arrays>"
 
+    def __iter__(
+        self,
+    ) -> Generator[tuple[tuple[FullSlice, ...], npt.NDArray[Any], npt.NDArray[Any]], None, None]:
+        for index in self._chunk_indices:
+            work_subset = map_slice(index, shift_to_zero=True)
+            res_1 = self._arr_1.read(self._work_array_1, map_slice(index), work_subset)
+            res_2 = self._arr_2.read(self._work_array_2, map_slice(index), work_subset)
 
-def _read_array(arr: npt.NDArray[Any] | H5Array[Any],
-                out: npt.NDArray[Any],
-                source_sel: tuple[FullSlice, ...],
-                dest_sel: tuple[FullSlice, ...]) -> None:
-    if isinstance(arr, ch5mpy.H5Array):
-        arr.read_direct(out, source_sel=source_sel, dest_sel=dest_sel)
+            if self._keepdims:
+                res_1 = res_1.reshape((1,) * (self._arr_1.ndim - res_1.ndim) + res_1.shape)
+                res_2 = res_2.reshape((1,) * (self._arr_2.ndim - res_2.ndim) + res_2.shape)
 
-    else:
-        out[dest_sel] = arr[source_sel]
+            yield index, res_1, res_2
 
 
-def iter_chunks_2(x1: npt.NDArray[Any] | H5Array[Any],
-                  x2: npt.NDArray[Any] | H5Array[Any]) \
-        -> Generator[tuple[tuple[FullSlice, ...], npt.NDArray[Any], npt.NDArray[Any] | Number], None, None]:
+def iter_chunks_2(
+    x1: npt.NDArray[Any] | H5Array[Any], x2: npt.NDArray[Any] | H5Array[Any]
+) -> Generator[tuple[tuple[FullSlice, ...], npt.NDArray[Any], npt.NDArray[Any] | Number], None, None,]:
     # special case where x2 is a 0D array, iterate through chunks of x1 and always yield x2
     if x2.ndim == 0:
-        max_mem_x1 = get_size(x1.MAX_MEM_USAGE) if isinstance(x1, ch5mpy.H5Array) else INF
+        if isinstance(x1, ch5mpy.H5Array):
+            for chunk, arr in ChunkIterator(x1):
+                yield chunk, arr, cast(Number, x2[()])
 
-        chunks = get_chunks(max_mem_x1, x1.shape, x1.dtype.itemsize)
-        work_array_x1 = get_work_array(x1.shape, chunks[0], dtype=x1.dtype)
-
-        for chunk in chunks:
-            work_subset = tuple(c.shift_to_zero() for c in chunk)
-            _read_array(x1, work_array_x1, chunk, work_subset)
-
-            yield chunk, work_array_x1[work_subset], cast(Number, x2[()])
+        else:
+            yield (FullSlice.whole_axis(x1.shape[0]),), x1, cast(Number, x2[()])
 
     # nD case
     else:
-        if x1.shape != x2.shape:
-            raise ValueError(f'Cannot iterate chunks of arrays with different shapes: {x1.shape} != {x2.shape}')
-
-        max_mem_x1 = get_size(x1.MAX_MEM_USAGE) if isinstance(x1, ch5mpy.H5Array) else INF
-        max_mem_x2 = get_size(x2.MAX_MEM_USAGE) if isinstance(x2, ch5mpy.H5Array) else INF
-
-        chunks = get_chunks(min(max_mem_x1, max_mem_x2), x1.shape, max(x1.dtype.itemsize, x2.dtype.itemsize))
-        work_array_x1 = get_work_array(x1.shape, chunks[0], dtype=x1.dtype)
-        work_array_x2 = get_work_array(x1.shape, chunks[0], dtype=x2.dtype)
-
-        for chunk in chunks:
-            work_subset = tuple(c.shift_to_zero() for c in chunk)
-            _read_array(x1, work_array_x1, chunk, work_subset)
-            _read_array(x2, work_array_x2, chunk, work_subset)
-
-            yield chunk, work_array_x1[work_subset], work_array_x2[work_subset]
+        yield from PairedChunkIterator(x1, x2)
```

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/repr.py` & `ch5mpy-0.2/ch5mpy/h5array/repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from __future__ import annotations
 
+from numbers import Number
+
 from typing import Any
 from typing import overload
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ch5mpy import H5Array
 
 
 # ====================================================
 # code
 @overload
-def _get3(arr: H5Array[Any]) -> list[Any | None]:
+def _get3(arr: None) -> None:
     ...
 
 
 @overload
-def _get3(arr: None) -> None:
+def _get3(arr: H5Array[Any] | Number | str) -> list[Any]:
     ...
 
 
-def _get3(arr: H5Array[Any] | None) -> list[Any | None] | None:
+def _get3(arr: H5Array[Any] | Number | str | None) -> list[Any] | None:
     """Get the first (and last) 3 elements in a set <arr>."""
     if arr is None:
         return None
 
-    if len(arr) <= 6:
-        return list(arr[:])
+    elif isinstance(arr, (Number, str)):
+        return [arr]
+
+    elif len(arr) <= 6:
+        return list(arr)
 
     return list(arr[:3]) + [None] + list(arr[-3:])
 
 
-def _print3(
-    lst: list[Any | None] | None, end: str = "\n", before: str = "", sep: str = ","
-) -> str:
+def _print3(lst: list[Any | None] | None, end: str = "\n", before: str = "", sep: str = ",") -> str:
     """Print the first (and last) 3 elements in"""
     if lst is None:
         return f"{before}...{end}"
 
-    return f"{before}[{(sep + ' ').join(['...' if e is None else str(e) for e in lst])}]{end}"
+    return f"{before}[{(sep + ' ').join(['...' if e is None else repr(e) for e in lst])}]{end}"
 
 
-def _get_padding(
-    padding: int, before: str | None = None, padding_skip_first: bool = False
-) -> str:
+def _get_padding(padding: int, before: str | None = None, padding_skip_first: bool = False) -> str:
     """Get the actual needed amount of padding, given that head strings might have been pasted before."""
     if padding_skip_first:
         return ""
 
     if before is None:
         return " " * padding
 
@@ -63,32 +64,29 @@
     padding: int,
     padding_skip_first: bool,
     before: str,
     end: str,
     sep: str,
 ) -> str:
     # exit condition : array is 1D and can be printed
-    if arr is None or arr.ndim == 1:
+    if arr is None or arr.ndim <= 1:
         return _print3(_get3(arr), before=before, end=end, sep=sep)
 
     # recursive calls
     rows = _get3(arr)
-
     spacer = "," + "\n" * (arr.ndim - 1)
 
     return (
         spacer.join(
             [
                 _print_dataset_core(
                     rows[0],
                     padding=padding,
-                    padding_skip_first=False,
-                    before=_get_padding(padding, before, padding_skip_first)
-                    + before
-                    + "[",
+                    padding_skip_first=True,
+                    before=_get_padding(padding, before, padding_skip_first) + before + "[",
                     end="",
                     sep=sep,
                 )
             ]
             + [
                 _print_dataset_core(
                     sub_arr,
@@ -96,39 +94,46 @@
                     padding_skip_first=False,
                     before=_get_padding(padding + len(before) + 1),
                     end="",
                     sep=sep,
                 )
                 for sub_arr in rows[1:-1]
             ]
-            + [
-                _print_dataset_core(
-                    rows[-1],
-                    padding=padding,
-                    padding_skip_first=False,
-                    before=_get_padding(padding + len(before) + 1),
-                    end="",
-                    sep=sep,
-                )
-            ]
+            + (
+                [
+                    _print_dataset_core(
+                        rows[-1],
+                        padding=padding,
+                        padding_skip_first=False,
+                        before=_get_padding(padding + len(before) + 1),
+                        end="",
+                        sep=sep,
+                    )
+                ]
+                if len(rows) > 1
+                else []
+            )
         )
         + "]"
     )
 
 
 def print_dataset(
     arr: H5Array[Any],
     padding: int = 0,
     padding_skip_first: bool = False,
     before: str | None = None,
     after: str | None = None,
     end: str = "\n",
     sep: str = ",",
 ) -> str:
-    if arr.ndim == 0:
+    if arr.size == 0:
+        array_repr = "[]"
+
+    elif arr.ndim == 0:
         array_repr = f"{arr[()]}"
 
     else:
         array_repr = _print_dataset_core(
             arr,
             padding=padding,
             padding_skip_first=padding_skip_first,
```

### Comparing `ch5mpy-0.1.3/ch5mpy/h5array/subset.py` & `ch5mpy-0.2/ch5mpy/h5array/view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,141 +1,130 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from __future__ import annotations
 
-import numpy as np
+from typing import Any, TypeVar
 
+import numpy as np
 import numpy.typing as npt
-from typing import Any
-from typing import cast
-from typing import TypeVar
-from typing import Sequence
-from ch5mpy._typing import SELECTOR
-from ch5mpy._typing import NP_FUNC
 
-import ch5mpy.h5array.h5array as h5array
+import ch5mpy
 from ch5mpy import Dataset
-from ch5mpy.h5array.io import parse_selector
-from ch5mpy.h5array.io import read_from_dataset
-from ch5mpy.h5array.io import write_to_dataset
-from ch5mpy.h5array.slice import FullSlice
-from ch5mpy.h5array.slice import map_slice
+from ch5mpy._typing import NP_FUNC, SELECTOR
+from ch5mpy.h5array.array import as_array
+from ch5mpy.h5array.io import read_from_dataset, read_one_from_dataset, write_to_dataset
+from ch5mpy.indexing import FullSlice, Selection
+from ch5mpy.objects.dataset import DatasetWrapper
 
 # ====================================================
 # code
 _T = TypeVar("_T", bound=np.generic)
-_DT = TypeVar("_DT", bound=np.generic)
-
-
-def _cast_selection(
-        selection: tuple[Sequence[int] | FullSlice, ...],
-        on: tuple[Sequence[int] | FullSlice, ...],
-) -> tuple[Sequence[int] | FullSlice, ...]:
-    casted_indices: tuple[Sequence[int] | FullSlice, ...] = ()
-
-    for s, o in zip(selection, on):
-        if isinstance(s, FullSlice) and \
-                s.is_whole_axis(o.max if isinstance(o, FullSlice) else s.max):
-            casted_indices += (o,)
 
-        elif isinstance(o, FullSlice) and o.is_whole_axis():
-            casted_indices += (s,)
 
-        else:
-            casted_indices += (np.array(o)[np.array(s)],)
-
-    return casted_indices
-
-
-class H5ArrayView(h5array.H5Array[_T]):
+class H5ArrayView(ch5mpy.H5Array[_T]):
     """A view on a H5Array."""
 
     # region magic methods
-    def __init__(self, dset: Dataset[_T], sel: tuple[Sequence[int] | FullSlice, ...]):
+    def __init__(self, dset: Dataset[_T] | DatasetWrapper[_T], sel: Selection):
         super().__init__(dset)
         self._selection = sel
 
     def __getitem__(self, index: SELECTOR | tuple[SELECTOR, ...]) -> _T | H5ArrayView[_T]:
-        selection, nb_elements = parse_selector(self.shape_selection, index)
+        selection = Selection.from_selector(index, self.shape)
 
-        if selection is None:
+        if selection.is_empty:
             return H5ArrayView(dset=self._dset, sel=self._selection)
 
-        elif nb_elements == 1:
-            loading_array = np.empty(1, dtype=self.dtype)
-            read_from_dataset(self._dset, _cast_selection(selection, on=self._selection), loading_array)
+        selection = selection.cast_on(self._selection)
 
-            return cast(_T, loading_array[0])
+        if selection.compute_shape(self._dset.shape) == ():
+            return read_one_from_dataset(self._dset, selection, self.dtype)
 
-        return H5ArrayView(dset=self._dset, sel=_cast_selection(selection, on=self._selection))
+        return H5ArrayView(dset=self._dset, sel=selection)
 
     def __setitem__(self, index: SELECTOR | tuple[SELECTOR, ...], value: Any) -> None:
-        selection, nb_elements = parse_selector(self.shape_selection, index)
-
-        try:
-            value_arr = np.array(value, dtype=self.dtype)
-
-        except ValueError:
-            raise ValueError(f'Could set value of type {type(value)} in H5Array of type {self.dtype}.')
-
-        if nb_elements != value_arr.size:
-            raise ValueError(f"{' x '.join(map(str, self.shape if selection is None else map(len, selection)))} "
-                             f"values were selected but {' x '.join(map(str, value_arr.shape))} were given.")
-
-        if selection is None:
-            selection_as_slices: tuple[Sequence[int] | slice, ...] = \
-                tuple(e.as_slice() if isinstance(e, FullSlice) else e for e in self._selection)
-            self._dset[selection_as_slices] = value_arr
-
-        else:
-            write_to_dataset(self._dset, value_arr,  _cast_selection(selection, on=self._selection))
+        selection = Selection.from_selector(index, self.shape)
+        write_to_dataset(self._dset, as_array(value, self.dtype), selection.cast_on(self._selection))
 
     def __len__(self) -> int:
         return self.shape[0]
 
-    def __contains__(self, item: Any) -> bool:
-        raise NotImplementedError
+    def _inplace(self, func: NP_FUNC, value: Any) -> H5ArrayView[_T]:
+        if np.issubdtype(self.dtype, str):
+            raise TypeError("Cannot perform inplace operation on str H5Array.")
+
+        # special case : 0D array
+        if self.shape == ():
+            self._dset[:] = func(self._dset[:], value)
+            return self
+
+        # general case : 1D+ array
+        for index, chunk in self.iter_chunks():
+            func(chunk, value, out=chunk)
+
+            for dest_sel, source_sel in Selection(index).cast_on(self._selection).iter_h5(self.shape):
+                # FIXME : can be slow in some cases (e.g. index is [column vector, 0] --> we loop over all pairs
+                #  (c, 0) for c in column vector / instead we could flatten the column vector and pass it as is)
+                # write back result into array
+                self._dset.write_direct(chunk, source_sel=source_sel, dest_sel=dest_sel)
 
-    def _inplace_operation(self, func: NP_FUNC, value: Any) -> H5ArrayView[_T]:
-        raise NotImplementedError
+        return self
 
     # endregion
 
     # region interface
     def __array__(self, dtype: npt.DTypeLike | None = None) -> npt.NDArray[Any]:
-        if dtype is None:
-            dtype = self.dtype
-
-        loading_array = np.empty(self.shape, dtype)
+        loading_array = np.empty(
+            self._selection.compute_shape(self._dset.shape, new_axes=False),
+            dtype or self.dtype,
+        )
         read_from_dataset(self._dset, self._selection, loading_array)
 
-        return loading_array
+        return loading_array.reshape(self.shape)
 
     # endregion
 
     # region attributes
     @property
-    def shape_selection(self) -> tuple[int, ...]:
-        return tuple(len(axis_sel) for axis_sel in self._selection)
-
-    @property
     def shape(self) -> tuple[int, ...]:
-        return tuple(len(axis_sel) for axis_sel in self._selection if len(axis_sel) > 1)
+        return self._selection.compute_shape(self._dset.shape)
 
     # endregion
 
     # region methods
-    def read_direct(self,
-                    dest: npt.NDArray[_T],
-                    source_sel: tuple[FullSlice, ...],
-                    dest_sel: tuple[FullSlice, ...]) -> None:
-        nb_whole_axes_before = (self._dset.ndim - len(source_sel))
-        whole_axes_before = tuple(FullSlice.whole_axis(s) for s in self.shape[:nb_whole_axes_before])
-        nb_whole_axes_after = (len(whole_axes_before) + len(source_sel))
-        whole_axes_after = tuple(FullSlice.whole_axis(s) for s in self.shape[nb_whole_axes_after:])
-
-        source_sel_casted = _cast_selection(whole_axes_before + source_sel + whole_axes_after, on=self._selection)
-        read_from_dataset(self._dset, source_sel_casted, dest[map_slice(dest_sel)])
+    def astype(self, dtype: npt.DTypeLike, inplace: bool = False) -> H5ArrayView[Any]:
+        """
+        Cast an H5Array to a specified dtype.
+        This does not perform a copy, it returns a wrapper around the underlying H5 dataset.
+        """
+        if inplace:
+            raise TypeError("Cannot cast inplace a view of an H5Array.")
+
+        if np.issubdtype(dtype, str) and (np.issubdtype(self._dset.dtype, str) or self._dset.dtype == object):
+            return H5ArrayView(self._dset.asstr(), sel=self._selection)
+
+        return H5ArrayView(self._dset.astype(dtype), sel=self._selection)
+
+    def maptype(self, otype: type[Any]) -> H5ArrayView[Any]:
+        """
+        Cast an H5Array to any object type.
+        This extends H5Array.astype() to any type <T>, where it is required that an object <T> can be constructed as
+        T(v) for any value <v> in the dataset.
+        """
+        return H5ArrayView(self._dset.maptype(otype), sel=self._selection)
+
+    def read_direct(
+        self,
+        dest: npt.NDArray[_T],
+        source_sel: tuple[slice, ...],
+        dest_sel: tuple[slice, ...],
+    ) -> None:
+        dset = self._dset.asstr() if np.issubdtype(self.dtype, str) else self._dset
+        read_from_dataset(
+            dset,
+            Selection((FullSlice.from_slice(s) for s in source_sel)).cast_on(self._selection),
+            dest[dest_sel],
+        )
 
     # endregion
```

### Comparing `ch5mpy-0.1.3/ch5mpy/pickle/wrap.py` & `ch5mpy-0.2/ch5mpy/objects/pickle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-# coding: utf-8
-
 """
 Modify h5 File, Group and Dataset objects to allow pickling.
 
 Modified from https://github.com/DaanVanVugt/h5pickle/blob/master/h5pickle
 """
-
-# ====================================================
-# imports
 from __future__ import annotations
 
-import h5py
-
 from typing import Any
-from typing import TypeVar
-
 
-# ====================================================
-# code
-X = TypeVar("X")
+import h5py
 
 
-class PickleableH5PyObject(h5py.HLObject):
+class PickleableH5Object(h5py.HLObject):
     """Save state required to pickle and unpickle h5py objects and groups.
     This class should not be used directly, but is here as a base for inheritance
     for Group and Dataset"""
 
     def __getstate__(self) -> dict[str, Any] | None:
         """Save the current name and a reference to the root file object."""
         return {"name": self.name, "file": self.file_info}
```

### Comparing `ch5mpy-0.1.3/ch5mpy/utils.py` & `ch5mpy-0.2/ch5mpy/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # coding: utf-8
 
 # ====================================================
 # imports
 from typing import Any
-from typing import Sequence
+from typing import Sequence  # noqa: F401
 from typing import Collection
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing_extensions import TypeGuard
+    from typing_extensions import TypeGuard  # noqa: F401
 
 
 # ====================================================
 # code
-def is_sequence(obj: Any) -> 'TypeGuard[Sequence[Any]]':
+def is_sequence(obj: Any) -> "TypeGuard[Sequence[Any]]":
     """Is the object a sequence of objects ? (excluding strings and byte objects.)"""
-    return isinstance(obj, Collection) and hasattr(obj, '__getitem__') and not isinstance(
-        obj, (str, bytes, bytearray, memoryview)
+    return (
+        isinstance(obj, Collection)
+        and hasattr(obj, "__getitem__")
+        and not isinstance(obj, (str, bytes, bytearray, memoryview))
     )
```

### Comparing `ch5mpy-0.1.3/tests/test_array_repr.py` & `ch5mpy-0.2/tests/test_array_repr.py`

 * *Files identical despite different names*

### Comparing `ch5mpy-0.1.3/tests/test_full_slice.py` & `ch5mpy-0.2/tests/test_full_slice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # ====================================================
 # imports
-from ch5mpy.h5array.slice import FullSlice
+from ch5mpy.indexing.slice import FullSlice
 
 
 # ====================================================
 # code
 def test_true_stop_step1():
     f = FullSlice(0, 3, 1, 10)
     assert f.true_stop == 2
```

### Comparing `ch5mpy-0.1.3/tests/test_get_chunks.py` & `ch5mpy-0.2/tests/test_get_chunks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,97 @@
 # coding: utf-8
 
 # ====================================================
 # imports
-from ch5mpy.h5array.inplace import get_chunks
-from ch5mpy.h5array.slice import FullSlice
+from ch5mpy.h5array.chunks.iter import _get_chunk_indices
+from ch5mpy.indexing.slice import FullSlice
 
 
 # ====================================================
 # code
 def test_1d_smaller_than_nb_elements():
-    assert get_chunks(10, (5,), 1) == ((FullSlice.whole_axis(5),),)
+    assert _get_chunk_indices(10, (5,)) == ((FullSlice.whole_axis(5),),)
 
 
 def test_1d_greater_than_nb_elements():
-    assert get_chunks(10, (15,), 1) == ((FullSlice(0, 10, 1, 15),),
-                                        (FullSlice(10, 15, 1, 15),))
+    assert _get_chunk_indices(10, (15,)) == ((FullSlice(0, 10, 1, 15),), (FullSlice(10, 15, 1, 15),))
 
 
 def test_1d_greater_than_nb_elements_multiple():
-    assert get_chunks(10, (30,), 1) == (
+    assert _get_chunk_indices(10, (30,)) == (
         (FullSlice(0, 10, 1, 30),),
         (FullSlice(10, 20, 1, 30),),
         (FullSlice(20, 30, 1, 30),),
     )
 
 
 def test_2d_array_smaller_than_nb_elements():
-    assert get_chunks(100, (2, 10), 1) == (
-        (FullSlice.whole_axis(2),),
-    )
+    assert _get_chunk_indices(100, (2, 10)) == ((FullSlice.whole_axis(2), FullSlice.whole_axis(10)),)
 
 
 def test_2d_array_1row():
-    assert get_chunks(10, (8, 10), 1) == (
-        (FullSlice.one(0, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(1, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(2, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(3, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(4, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(5, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(6, 8), FullSlice.whole_axis(10),),
-        (FullSlice.one(7, 8), FullSlice.whole_axis(10),),
+    assert _get_chunk_indices(10, (8, 10)) == (
+        (
+            FullSlice.one(0, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(1, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(2, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(3, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(4, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(5, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(6, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice.one(7, 8),
+            FullSlice.whole_axis(10),
+        ),
     )
 
 
 def test_2d_array_2rows():
-    assert get_chunks(20, (8, 10), 1) == (
-        (FullSlice(0, 2, 1, 8), FullSlice.whole_axis(10),),
-        (FullSlice(2, 4, 1, 8), FullSlice.whole_axis(10),),
-        (FullSlice(4, 6, 1, 8), FullSlice.whole_axis(10),),
-        (FullSlice(6, 8, 1, 8), FullSlice.whole_axis(10),),
+    assert _get_chunk_indices(20, (8, 10)) == (
+        (
+            FullSlice(0, 2, 1, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice(2, 4, 1, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice(4, 6, 1, 8),
+            FullSlice.whole_axis(10),
+        ),
+        (
+            FullSlice(6, 8, 1, 8),
+            FullSlice.whole_axis(10),
+        ),
     )
 
 
 def test_2d_array_0rows():
-    assert get_chunks(6, (8, 10), 1) == (
+    assert _get_chunk_indices(6, (8, 10)) == (
         (FullSlice.one(0, 8), FullSlice(0, 6, 1, 10)),
         (FullSlice.one(0, 8), FullSlice(6, 10, 1, 10)),
         (FullSlice.one(1, 8), FullSlice(0, 6, 1, 10)),
         (FullSlice.one(1, 8), FullSlice(6, 10, 1, 10)),
         (FullSlice.one(2, 8), FullSlice(0, 6, 1, 10)),
         (FullSlice.one(2, 8), FullSlice(6, 10, 1, 10)),
         (FullSlice.one(3, 8), FullSlice(0, 6, 1, 10)),
@@ -71,54 +104,54 @@
         (FullSlice.one(6, 8), FullSlice(6, 10, 1, 10)),
         (FullSlice.one(7, 8), FullSlice(0, 6, 1, 10)),
         (FullSlice.one(7, 8), FullSlice(6, 10, 1, 10)),
     )
 
 
 def test_3d_array_smaller_than_nb_elements():
-    assert get_chunks(200, (5, 5, 5), 1) == (
-        (FullSlice.whole_axis(5),),
+    assert _get_chunk_indices(200, (5, 5, 5)) == (
+        (FullSlice.whole_axis(5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
     )
 
 
 def test_3d_array_1_array():
-    assert get_chunks(30, (5, 5, 5), 1) == (
+    assert _get_chunk_indices(30, (5, 5, 5)) == (
         (FullSlice.one(0, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice.one(1, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice.one(2, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice.one(3, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice.one(4, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
     )
 
 
 def test_3d_array_2_arrays():
-    assert get_chunks(60, (5, 5, 5), 1) == (
+    assert _get_chunk_indices(60, (5, 5, 5)) == (
         (FullSlice(0, 2, 1, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice(2, 4, 1, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
         (FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5), FullSlice.whole_axis(5)),
     )
 
 
 def test_3d_array_2rows():
-    assert get_chunks(20, (5, 5, 5), 1) == (
+    assert _get_chunk_indices(20, (5, 5, 5)) == (
         (FullSlice.one(0, 5), FullSlice(0, 4, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(0, 5), FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(1, 5), FullSlice(0, 4, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(1, 5), FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(2, 5), FullSlice(0, 4, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(2, 5), FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(3, 5), FullSlice(0, 4, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(3, 5), FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(4, 5), FullSlice(0, 4, 1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(4, 5), FullSlice(4, 5, 1, 5), FullSlice.whole_axis(5)),
     )
 
 
 def test_3d_array_1row():
-    assert get_chunks(6, (5, 5, 5), 1) == (
+    assert _get_chunk_indices(6, (5, 5, 5)) == (
         (FullSlice.one(0, 5), FullSlice.one(0, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(0, 5), FullSlice.one(1, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(0, 5), FullSlice.one(2, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(0, 5), FullSlice.one(3, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(0, 5), FullSlice.one(4, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(1, 5), FullSlice.one(0, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(1, 5), FullSlice.one(1, 5), FullSlice.whole_axis(5)),
@@ -140,15 +173,15 @@
         (FullSlice.one(4, 5), FullSlice.one(2, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(4, 5), FullSlice.one(3, 5), FullSlice.whole_axis(5)),
         (FullSlice.one(4, 5), FullSlice.one(4, 5), FullSlice.whole_axis(5)),
     )
 
 
 def test_3d_array_0rows():
-    assert get_chunks(3, (5, 5, 5), 1) == (
+    assert _get_chunk_indices(3, (5, 5, 5)) == (
         (FullSlice.one(0, 5), FullSlice.one(0, 5), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(0, 5), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(1, 5), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(1, 5), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(2, 5), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(2, 5), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 5), FullSlice.one(3, 5), FullSlice(0, 3, 1, 5)),
@@ -195,15 +228,15 @@
         (FullSlice.one(4, 5), FullSlice.one(3, 5), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(4, 5), FullSlice.one(4, 5), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(4, 5), FullSlice.one(4, 5), FullSlice(3, 5, 1, 5)),
     )
 
 
 def test_3d_array():
-    assert get_chunks(24, (3, 4, 5), 8) == (
+    assert _get_chunk_indices(3, (3, 4, 5)) == (
         (FullSlice.one(0, 3), FullSlice.one(0, 4), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(0, 4), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(1, 4), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(1, 4), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(2, 4), FullSlice(0, 3, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(2, 4), FullSlice(3, 5, 1, 5)),
         (FullSlice.one(0, 3), FullSlice.one(3, 4), FullSlice(0, 3, 1, 5)),
```

### Comparing `ch5mpy-0.1.3/tests/test_h5dict.py` & `ch5mpy-0.2/tests/test_h5dict.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding: utf-8
 
 # ====================================================
 # imports
-import pytest
-import numpy as np
+from __future__ import annotations
+
 from pathlib import Path
+from typing import Generator
 
-from ch5mpy import File
-from ch5mpy import H5Dict
-from ch5mpy import H5Mode
-from ch5mpy import H5Array
-from ch5mpy import write_object
+import numpy as np
+import pytest
+
+from ch5mpy import File, H5Array, H5Dict, H5Mode, write_object
 
 
 # ====================================================
 # code
 @pytest.fixture
-def backed_dict() -> H5Dict:
+def backed_dict() -> Generator[H5Dict, None, None]:
     data = {
         "a": 1,
         "b": [1, 2, 3],
         "c": {"d": "test", "e": np.arange(100)},
         "f": np.zeros((10, 10, 10)),
     }
 
@@ -64,28 +64,26 @@
     assert isinstance(backed_dict["c"], H5Dict)
 
 
 def test_backed_dict_has_correct_values(backed_dict):
     values_list = list(backed_dict.values())
 
     assert (
-        values_list[0] == 1
-        and np.array_equal(values_list[1], [1, 2, 3])
-        and list(values_list[2].keys()) == ["d", "e"]
+        values_list[0] == 1 and np.array_equal(values_list[1], [1, 2, 3]) and list(values_list[2].keys()) == ["d", "e"]
     )
 
 
 def test_backed_dict_has_correct_items(backed_dict):
     assert list(backed_dict.items())[0] == ("a", 1)
 
 
 def test_backed_dict_can_set_regular_value(backed_dict):
     backed_dict["a"] = 5
 
-    assert np.all(backed_dict["a"] == 5)
+    assert backed_dict["a"] == 5
 
 
 def test_backed_dict_can_set_array_value(backed_dict):
     backed_dict["b"][1] = 6
 
     assert np.all(backed_dict["b"] == [1, 6, 3])
 
@@ -156,8 +154,29 @@
 
     assert isinstance(c["c"], dict)
 
 
 def test_backed_dict_copy_dataset_proxy_should_be_array(backed_dict):
     c = backed_dict.copy()
 
-    assert isinstance(c["b"], H5Array)
+    assert isinstance(c["b"], np.ndarray)
+
+
+class ComplexObject:
+    def __init__(self, value: int):
+        self.value = value
+
+    def __repr__(self) -> str:
+        return f"CO({self.value})"
+
+    def __h5_write__(self, values: H5Dict) -> None:
+        values.attributes["value"] = self.value
+
+    @classmethod
+    def __h5_read__(cls, values: H5Dict) -> ComplexObject:
+        return ComplexObject(values.attributes["value"])
+
+
+def test_backed_dict_can_store_complex_objects(backed_dict):
+    backed_dict["g"] = {"a": ComplexObject(1), "b": ComplexObject(2)}
+
+    assert isinstance(backed_dict["g"]["a"], ComplexObject)
```

### Comparing `ch5mpy-0.1.3/tests/test_pickle.py` & `ch5mpy-0.2/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `ch5mpy-0.1.3/tests/test_write.py` & `ch5mpy-0.2/tests/test_write.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,56 +2,50 @@
 # Created on 13/12/2022 14:52
 # Author : matteo
 
 # ====================================================
 # imports
 from __future__ import annotations
 
-import pickle
-import pytest
-import numpy as np
 from enum import Enum
-
 from typing import Any
 
-from ch5mpy.write import write_attribute
-from ch5mpy.write import write_dataset
-from ch5mpy.write import write_object
-from ch5mpy import File
-from ch5mpy import Group
+import numpy as np
+import pytest
+
+from ch5mpy import File, Group
+from ch5mpy.write import write_dataset, write_object
 
 
 # ====================================================
 # code
 class State(Enum):
     RNA = "RNA"
 
 
-@pytest.mark.parametrize("obj, expected", [(1, 1), ("abc", "abc"), (None, "None")])
+@pytest.mark.parametrize("obj, expected", [(1, 1), ("abc", "abc"), (None, None)])
 def test_should_write_simple_attribute(obj, expected, group):
-    write_attribute(group, "something", obj)
+    group.attrs["something"] = obj
 
     assert "something" in group.attrs.keys()
     assert group.attrs["something"] == expected
 
 
 def test_should_write_list_attribute(group):
-    write_attribute(group, "something", [1, 2, 3])
+    group.attrs["something"] = [1, 2, 3]
 
     assert "something" in group.attrs.keys()
     assert np.all(group.attrs["something"] == [1, 2, 3])
 
 
 def test_should_write_complex_objects_as_strings_in_attributes(group):
-    write_attribute(group, "something", State.RNA)
+    group.attrs["something"] = State.RNA
 
     assert "something" in group.attrs.keys()
-    assert group.attrs["something"].tobytes() == pickle.dumps(
-        State.RNA, protocol=pickle.HIGHEST_PROTOCOL
-    )
+    assert group.attrs["something"] == State.RNA
 
 
 @pytest.mark.parametrize(
     "array, expected",
     [
         (np.array([1, 2, 3]), [1, 2, 3]),
         ([1, 2, 3], [1, 2, 3]),
```

