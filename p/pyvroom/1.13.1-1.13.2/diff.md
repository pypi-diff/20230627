# Comparing `tmp/pyvroom-1.13.1.tar.gz` & `tmp/pyvroom-1.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvroom-1.13.1.tar", last modified: Sat May  6 08:14:25 2023, max compression
+gzip compressed data, was "pyvroom-1.13.2.tar", last modified: Tue Jun 27 20:01:15 2023, max compression
```

## Comparing `pyvroom-1.13.1.tar` & `pyvroom-1.13.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.701874 pyvroom-1.13.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.685874 pyvroom-1.13.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.693874 pyvroom-1.13.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-06 08:14:17.000000 pyvroom-1.13.1/.github/workflows/main_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-06 08:14:17.000000 pyvroom-1.13.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-06 08:14:17.000000 pyvroom-1.13.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-06 08:14:17.000000 pyvroom-1.13.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 08:14:17.000000 pyvroom-1.13.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-06 08:14:17.000000 pyvroom-1.13.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 08:14:17.000000 pyvroom-1.13.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-06 08:14:17.000000 pyvroom-1.13.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-06 08:14:25.701874 pyvroom-1.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-06 08:14:17.000000 pyvroom-1.13.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 08:14:17.000000 pyvroom-1.13.1/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-06 08:14:17.000000 pyvroom-1.13.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 08:14:17.000000 pyvroom-1.13.1/conanfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 08:14:17.000000 pyvroom-1.13.1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-06 08:14:17.000000 pyvroom-1.13.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-06 08:14:25.701874 pyvroom-1.13.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-06 08:14:17.000000 pyvroom-1.13.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.693874 pyvroom-1.13.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/_vroom.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.693874 pyvroom-1.13.1/src/bind/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/amount.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/break.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/exception.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.693874 pyvroom-1.13.1/src/bind/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/generic/matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.693874 pyvroom-1.13.1/src/bind/input/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/input/input.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/input/vehicle_step.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/job.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/location.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.697874 pyvroom-1.13.1/src/bind/solution/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/solution/route.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/solution/solution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/solution/step.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/solution/summary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/time_window.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/bind/vehicle.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.697874 pyvroom-1.13.1/src/pyvroom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 08:14:25.000000 pyvroom-1.13.1/src/pyvroom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.697874 pyvroom-1.13.1/src/vroom/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/break_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.701874 pyvroom-1.13.1/src/vroom/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/input/forced_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/input/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/input/vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.701874 pyvroom-1.13.1/src/vroom/solution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/solution/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-06 08:14:17.000000 pyvroom-1.13.1/src/vroom/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.701874 pyvroom-1.13.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:14:25.701874 pyvroom-1.13.1/test/input/
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/input/test_vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_file_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_libvroom_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-06 08:14:17.000000 pyvroom-1.13.1/test/test_vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.004866 pyvroom-1.13.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.008866 pyvroom-1.13.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/main_push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 20:01:05.000000 pyvroom-1.13.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 20:01:05.000000 pyvroom-1.13.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-27 20:01:05.000000 pyvroom-1.13.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 20:01:15.016867 pyvroom-1.13.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-27 20:01:05.000000 pyvroom-1.13.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 20:01:05.000000 pyvroom-1.13.2/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 20:01:05.000000 pyvroom-1.13.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 20:01:05.000000 pyvroom-1.13.2/conanfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-27 20:01:05.000000 pyvroom-1.13.2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 20:01:05.000000 pyvroom-1.13.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-27 20:01:15.020866 pyvroom-1.13.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-27 20:01:05.000000 pyvroom-1.13.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.008866 pyvroom-1.13.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/_vroom.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/amount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/break.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/exception.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/generic/matrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/input/input.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/input/vehicle_step.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/location.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/route.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/step.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/summary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/time_window.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/vehicle.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/pyvroom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 20:01:15.000000 pyvroom-1.13.2/src/pyvroom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/break_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/forced_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/solution/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/test/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/input/test_vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_libvroom_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_vehicle.py
```

### Comparing `pyvroom-1.13.1/.github/workflows/main_push.yml` & `pyvroom-1.13.2/.github/workflows/main_push.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/.github/workflows/pull_request.yml` & `pyvroom-1.13.2/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/.github/workflows/release.yml` & `pyvroom-1.13.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/.gitignore` & `pyvroom-1.13.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/LICENSE` & `pyvroom-1.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/Makefile` & `pyvroom-1.13.2/Makefile`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/PKG-INFO` & `pyvroom-1.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvroom
-Version: 1.13.1
+Version: 1.13.2
 Summary: Vehicle routing open-source optimization machine (VROOM)
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyvroom-1.13.1/README.rst` & `pyvroom-1.13.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/pyproject.toml` & `pyvroom-1.13.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/setup.cfg` & `pyvroom-1.13.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/setup.py` & `pyvroom-1.13.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 if platform.system() == "Windows":
     extra_compile_args = [
         "-DNOGDI",
         "-DNOMINMAX",
         "-DWIN32_LEAN_AND_MEAN",
         "-DASIO_STANDALONE",
         "-DUSE_PYTHON_BINDINGS",
+        "-DUSE_ROUTING=true"
     ]
     extra_link_args = []
 
 else:  # anything *nix
     extra_compile_args = [
         "-MMD",
         "-MP",
         "-Wextra",
         "-Wpedantic",
         "-Wall",
         "-O3",
         "-DASIO_STANDALONE",
         "-DNDEBUG",
         "-DUSE_PYTHON_BINDINGS",
+        "-DUSE_ROUTING=true"
     ]
     extra_link_args = [
         "-lpthread",
         "-lssl",
         "-lcrypto",
     ]
```

### Comparing `pyvroom-1.13.1/src/_vroom.cpp` & `pyvroom-1.13.2/src/_vroom.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/_main.cpp` & `pyvroom-1.13.2/src/bind/_main.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/amount.cpp` & `pyvroom-1.13.2/src/bind/amount.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/break.cpp` & `pyvroom-1.13.2/src/bind/break.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/enums.cpp` & `pyvroom-1.13.2/src/bind/enums.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/generic/matrix.cpp` & `pyvroom-1.13.2/src/bind/generic/matrix.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/input/input.cpp` & `pyvroom-1.13.2/src/bind/input/input.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/input/vehicle_step.cpp` & `pyvroom-1.13.2/src/bind/input/vehicle_step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/job.cpp` & `pyvroom-1.13.2/src/bind/job.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/location.cpp` & `pyvroom-1.13.2/src/bind/location.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/solution/route.cpp` & `pyvroom-1.13.2/src/bind/solution/route.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/solution/solution.cpp` & `pyvroom-1.13.2/src/bind/solution/solution.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
   char type[9];
   int64_t arrival;
   int64_t duration;
   int64_t setup;
   int64_t service;
   int64_t waiting_time;
   int64_t distance;
-  int64_t longitude;
-  int64_t latitude;
+  double longitude;
+  double latitude;
   int64_t location_index;
   int64_t id;
 
   char description[40];
 };
 
 void init_solution(py::module_ &m) {
```

### Comparing `pyvroom-1.13.1/src/bind/solution/step.cpp` & `pyvroom-1.13.2/src/bind/solution/step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/solution/summary.cpp` & `pyvroom-1.13.2/src/bind/solution/summary.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/time_window.cpp` & `pyvroom-1.13.2/src/bind/time_window.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/bind/vehicle.cpp` & `pyvroom-1.13.2/src/bind/vehicle.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/pyvroom.egg-info/PKG-INFO` & `pyvroom-1.13.2/src/pyvroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvroom
-Version: 1.13.1
+Version: 1.13.2
 Summary: Vehicle routing open-source optimization machine (VROOM)
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyvroom-1.13.1/src/pyvroom.egg-info/SOURCES.txt` & `pyvroom-1.13.2/src/pyvroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/__init__.py` & `pyvroom-1.13.2/src/vroom/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/amount.py` & `pyvroom-1.13.2/src/vroom/amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/break_.py` & `pyvroom-1.13.2/src/vroom/break_.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/input/forced_service.py` & `pyvroom-1.13.2/src/vroom/input/forced_service.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/input/input.py` & `pyvroom-1.13.2/src/vroom/input/input.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/input/vehicle_step.py` & `pyvroom-1.13.2/src/vroom/input/vehicle_step.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/job.py` & `pyvroom-1.13.2/src/vroom/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,16 @@
             pickup:
                 The amount of how much is being carried back from customer.
             skills:
                 Skills required to perform job. Only vehicles which satisfies
                 all required skills (i.e. has at minimum all skills values
                 required) are allowed to perform this job.
             priority:
-                The job priority level, where 0 is the most
-                important and 100 is the least important.
+                The job priority level, where 0 is the lowest priority
+                and 100 is the highest priority.
             time_windows:
                 Windows for where service is allowed to begin.
                 Defaults to have not restraints.
             description:
                 Optional string descriping the job.
         """
         if not pickup:
@@ -273,16 +273,16 @@
                 An interger representation of how much is being carried back
                 from customer.
             skills:
                 Skills required to perform job. Only vehicles which satisfies
                 all required skills (i.e. has at minimum all skills values
                 required) are allowed to perform this job.
             priority:
-                The job priority level, where 0 is the most
-                important and 100 is the least important.
+                The job priority level, where 0 is the lowest priority
+                and 100 is the highest priority.
         """
         self.pickup = pickup
         self.delivery = delivery
         self.amount = Amount(amount)
         self.skills = skills or set()
         self.priority = int(priority)
```

### Comparing `pyvroom-1.13.1/src/vroom/location.py` & `pyvroom-1.13.2/src/vroom/location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/solution/solution.py` & `pyvroom-1.13.2/src/vroom/solution/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
                 ),
                 "arrival": array["arrival"],
                 "duration": array["duration"],
                 "setup": array["setup"],
                 "service": array["service"],
                 "waiting_time": array["waiting_time"],
                 "location_index": array["location_index"],
-                "longitude": pandas.array(array["longitude"], dtype="Int64"),
-                "latitude": pandas.array(array["latitude"], dtype="Int64"),
+                "longitude": pandas.array(array["longitude"]),
+                "latitude": pandas.array(array["latitude"]),
                 "id": pandas.array(array["id"], dtype="Int64"),
                 "description": array["description"].astype("U40"),
             }
         )
         for column in ["longitude", "latitude", "id"]:
             if (frame[column] == NA_SUBSTITUTE).all():
                 del frame[column]
```

### Comparing `pyvroom-1.13.1/src/vroom/time_window.py` & `pyvroom-1.13.2/src/vroom/time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/src/vroom/vehicle.py` & `pyvroom-1.13.2/src/vroom/vehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             args.append(f"costs={self.costs}")
 
         for name, default in [
             ("breaks", []),
             ("description", ""),
             ("speed_factor", 1.0),
             ("max_tasks", MAX_UINT),
-            ("max_travel_time", MAX_INT),
+            ("max_travel_time", _vroom.scale_to_user_duration(MAX_INT)),
             ("steps", []),
         ]:
             attribute = getattr(self, name)
             if attribute != default:
                 args.append(f"{name}={attribute!r}")
 
         return f"vroom.{self.__class__.__name__}({', '.join(args)})"
@@ -231,15 +231,15 @@
 
     @property
     def max_tasks(self) -> str:
         return self._max_tasks
 
     @property
     def max_travel_time(self) -> str:
-        return self._max_travel_time
+        return _vroom.scale_to_user_duration(self._max_travel_time)
 
     @property
     def steps(self) -> List[VehicleStep]:
         return [VehicleStep(step) for step in self._steps]
 
     def has_same_locations(self, vehicle: Vehicle) -> bool:
         return self._has_same_locations(vehicle)
```

### Comparing `pyvroom-1.13.1/test/input/test_vehicle_step.py` & `pyvroom-1.13.2/test/input/test_vehicle_step.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_amount.py` & `pyvroom-1.13.2/test/test_amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_break.py` & `pyvroom-1.13.2/test/test_break.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_file_handle.py` & `pyvroom-1.13.2/test/test_file_handle.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_job.py` & `pyvroom-1.13.2/test/test_job.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_libvroom_examples.py` & `pyvroom-1.13.2/test/test_libvroom_examples.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_location.py` & `pyvroom-1.13.2/test/test_location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_time_window.py` & `pyvroom-1.13.2/test/test_time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.1/test/test_vehicle.py` & `pyvroom-1.13.2/test/test_vehicle.py`

 * *Files identical despite different names*

