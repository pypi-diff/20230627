# Comparing `tmp/pywin32-ctypes-0.2.1.tar.gz` & `tmp/pywin32-ctypes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywin32-ctypes-0.2.1.tar", last modified: Mon Jun 19 10:10:25 2023, max compression
+gzip compressed data, was "/home/itziakos/pywin32-ctypes/dist/tmpwppfxdq8/pywin32-ctypes-0.2.2.tar", last modified: Tue Jun 27 11:01:58 2023, max compression
```

## Comparing `pywin32-ctypes-0.2.1.tar` & `pywin32-ctypes-0.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.990797 pywin32-ctypes-0.2.1/
--rw-rw-rw-   0        0        0     2048 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1644 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      126 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3811 2023-06-19 10:10:25.990797 pywin32-ctypes-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1113 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/README.rst
--rw-rw-rw-   0        0        0        7 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/VERSION
--rw-rw-rw-   0        0        0       72 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/doc-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.883091 pywin32-ctypes-0.2.1/docs/
--rw-rw-rw-   0        0        0     7658 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/Makefile
--rwxrwxrwx   0        0        0     7292 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.890606 pywin32-ctypes-0.2.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.901139 pywin32-ctypes-0.2.1/docs/source/_templates/
--rw-rw-rw-   0        0        0     1016 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/source/_templates/module_template.rst
--rw-rw-rw-   0        0        0    12194 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      367 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     2155 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/source/mock_missing.py
--rw-rw-rw-   0        0        0      554 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/docs/source/pywin32.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.916211 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/
--rw-rw-rw-   0        0        0     3811 2023-06-19 10:10:25.000000 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1600 2023-06-19 10:10:25.000000 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:10:25.000000 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 10:09:47.000000 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-06-19 10:10:25.000000 pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      811 2023-06-19 10:10:25.993371 pywin32-ctypes-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      242 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/setup.py
--rw-rw-rw-   0        0        0       48 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/test-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.921805 pywin32-ctypes-0.2.1/win32ctypes/
--rw-rw-rw-   0        0        0      214 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.935830 pywin32-ctypes-0.2.1/win32ctypes/core/
--rw-rw-rw-   0        0        0     1622 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/__init__.py
--rw-rw-rw-   0        0        0      199 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/_winerrors.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.952496 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/
--rw-rw-rw-   0        0        0      270 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/__init__.py
--rw-rw-rw-   0        0        0     5333 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_authentication.py
--rw-rw-rw-   0        0        0      576 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_common.py
--rw-rw-rw-   0        0        0      771 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_dll.py
--rw-rw-rw-   0        0        0      313 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_nl_support.py
--rw-rw-rw-   0        0        0     4555 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_resource.py
--rw-rw-rw-   0        0        0      872 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_system_information.py
--rw-rw-rw-   0        0        0      332 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_time.py
--rw-rw-rw-   0        0        0     2662 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_util.py
--rw-rw-rw-   0        0        0      158 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/compat.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.972537 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/
--rw-rw-rw-   0        0        0      272 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/__init__.py
--rw-rw-rw-   0        0        0     3822 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_authentication.py
--rw-rw-rw-   0        0        0     1223 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_common.py
--rw-rw-rw-   0        0        0      552 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_dll.py
--rw-rw-rw-   0        0        0      315 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_nl_support.py
--rw-rw-rw-   0        0        0     4264 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_resource.py
--rw-rw-rw-   0        0        0      941 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_system_information.py
--rw-rw-rw-   0        0        0      342 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_time.py
--rw-rw-rw-   0        0        0     2005 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_util.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.972537 pywin32-ctypes-0.2.1/win32ctypes/pywin32/
--rw-rw-rw-   0        0        0      354 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/pywin32/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/pywin32/pywintypes.py
--rw-rw-rw-   0        0        0     7724 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/pywin32/win32api.py
--rw-rw-rw-   0        0        0     4801 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/pywin32/win32cred.py
--rw-rw-rw-   0        0        0      350 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/pywintypes.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:10:25.984289 pywin32-ctypes-0.2.1/win32ctypes/tests/
--rw-rw-rw-   0        0        0      693 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/tests/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/tests/test_backends.py
--rw-rw-rw-   0        0        0    11687 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/tests/test_win32api.py
--rw-rw-rw-   0        0        0     7948 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/tests/test_win32cred.py
--rw-rw-rw-   0        0        0       23 2023-06-19 10:10:25.000000 pywin32-ctypes-0.2.1/win32ctypes/version.py
--rw-rw-rw-   0        0        0      346 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/win32api.py
--rw-rw-rw-   0        0        0      348 2023-06-19 10:01:07.000000 pywin32-ctypes-0.2.1/win32ctypes/win32cred.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:58.000000 pywin32-ctypes-0.2.2/
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/win32ctypes/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      206 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      333 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/win32api.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      335 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/win32cred.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      337 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/pywintypes.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:58.000000 pywin32-ctypes-0.2.2/win32ctypes/pywin32/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      342 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/pywin32/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7430 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/pywin32/win32api.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4656 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/pywin32/win32cred.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      967 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/pywin32/pywintypes.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       22 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/win32ctypes/version.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/win32ctypes/core/
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1170 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      261 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      531 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_dll.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1952 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_util.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4116 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_resource.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3700 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_authentication.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      303 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_nl_support.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      327 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_time.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      905 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_system_information.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1564 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      190 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/_winerrors.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      547 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      259 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      741 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_dll.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2557 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_util.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4423 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_resource.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5161 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_authentication.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      295 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_nl_support.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      314 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_time.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      840 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_system_information.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      148 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/core/compat.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:58.000000 pywin32-ctypes-0.2.2/win32ctypes/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      672 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    11383 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/tests/test_win32api.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1017 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/tests/test_backends.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7718 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/win32ctypes/tests/test_win32cred.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       44 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/test-requirements.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      234 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/setup.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       70 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/doc-requirements.txt
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1600 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/SOURCES.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        1 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/dependency_links.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        1 2023-06-27 10:59:08.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/not-zip-safe
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4697 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/PKG-INFO
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       12 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/top_level.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        6 2023-06-27 11:01:47.000000 pywin32-ctypes-0.2.2/VERSION
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1616 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/LICENSE.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      120 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/MANIFEST.in
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      780 2023-06-27 11:01:58.000000 pywin32-ctypes-0.2.2/setup.cfg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4697 2023-06-27 11:01:58.000000 pywin32-ctypes-0.2.2/PKG-INFO
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/docs/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7028 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/make.bat
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/docs/source/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      537 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/source/pywin32.rst
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      337 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/source/index.rst
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-27 11:01:57.000000 pywin32-ctypes-0.2.2/docs/source/_templates/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      955 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/source/_templates/module_template.rst
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2083 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/source/mock_missing.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    11820 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/source/conf.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7465 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/docs/Makefile
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1075 2023-06-27 10:01:34.000000 pywin32-ctypes-0.2.2/README.rst
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2071 2023-06-27 10:14:06.000000 pywin32-ctypes-0.2.2/CHANGELOG.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pywin32-ctypes-0.2.1/CHANGELOG.txt` & `pywin32-ctypes-0.2.2/CHANGELOG.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,72 @@
-Change Log
-==========
-
-Version 0.2.1
--------------
-
-- Use faulthandler when testing and fix discovered errors (#115, #117).
-- Fix support for None username in credentials to be consistent in all backends (#99).
-- Test also on cp38, cp39, cp310, cp311 and use cp38 for linking (#114, #107, #100).
-- Add support for CredEnumerate extending code from @markb-EE (#110, #109, #111)
-- Remove support for older python versions < cp36 (#104, #120).
-
-Version 0.2.0
--------------
-
-- Fix syntax error when installing in python 3.7 (#81).
-- Support testing on python 3.7 (#82).
-- Support testing on python 3.3 and python 3.4 (#77).
-- Do not use 2to3 (#75).
-- Support lazy wrapping of win32 functions (#67).
-- Add CRED_PERSIST constants (#79 contributed by @tivnet).
-
-Version 0.1.2
--------------
-
-(bugfix release)
-
-- Fix implementation for the deprecated api (#64).
-
-Version 0.1.1
--------------
-
-(bugfix release)
-
-- Update Manifest.in entries (#63)
-- fix VERSION path in Manifest.in (#62 contributed by @MinchinWeb)
-
-
-Version 0.1.0
--------------
-
-- Update tests and provide better compatibility with pywin32 for
-  Resource functions
-- Fix: Python 3.5 and 3.6 support (#52).
-- API additions to allow pywin32-ctypes to work with pyinstaller (#46
-  and #57 contributed by @virtuald).
-- Fix: do not update the global copy of the windows dlls (#42)
-- Add documentation and setup automatic builds in ReadTheDocs (#3, #36).
-- Add cffi backend to be used when available (#31).
-- Fix: EnumResourceTypes and EnumResourceNames would only return ints
-  (#21, #30).
-- Restructure package layout to split core wrapping modules from
-  pywin32 emulation (#15, #17).
-
-Version 0.0.1
--------------
-
-7/04/2014
-
-- Python 2.6 support (#13)
-- Python 3 support (#12)
-- Basic maintenance work (#11, #7)
-- Fix error raising to be pywin32 compatible (#8)
-- Package rename mini_pywin32 -> pywin32-ctypes
-- Add travis-ci integration using wine! (#2)
-- Support basic library and resource loading (#1)
-- mini_pywin32 is born
+Change Log
+==========
+
+Version 0.2.2
+-------------
+
+- Use ctypes.set_last_error to avoid race conditions (#122)
+
+Version 0.2.1
+-------------
+
+- Use faulthandler when testing and fix discovered errors (#115, #117).
+- Fix support for None username in credentials to be consistent in all backends (#99).
+- Test also on cp38, cp39, cp310, cp311 and use cp38 for linking (#114, #107, #100).
+- Add support for CredEnumerate extending code from @markb-EE (#110, #109, #111)
+- Remove support for older python versions < cp36 (#104, #120).
+
+Version 0.2.0
+-------------
+
+- Fix syntax error when installing in python 3.7 (#81).
+- Support testing on python 3.7 (#82).
+- Support testing on python 3.3 and python 3.4 (#77).
+- Do not use 2to3 (#75).
+- Support lazy wrapping of win32 functions (#67).
+- Add CRED_PERSIST constants (#79 contributed by @tivnet).
+
+Version 0.1.2
+-------------
+
+(bugfix release)
+
+- Fix implementation for the deprecated api (#64).
+
+Version 0.1.1
+-------------
+
+(bugfix release)
+
+- Update Manifest.in entries (#63)
+- fix VERSION path in Manifest.in (#62 contributed by @MinchinWeb)
+
+
+Version 0.1.0
+-------------
+
+- Update tests and provide better compatibility with pywin32 for
+  Resource functions
+- Fix: Python 3.5 and 3.6 support (#52).
+- API additions to allow pywin32-ctypes to work with pyinstaller (#46
+  and #57 contributed by @virtuald).
+- Fix: do not update the global copy of the windows dlls (#42)
+- Add documentation and setup automatic builds in ReadTheDocs (#3, #36).
+- Add cffi backend to be used when available (#31).
+- Fix: EnumResourceTypes and EnumResourceNames would only return ints
+  (#21, #30).
+- Restructure package layout to split core wrapping modules from
+  pywin32 emulation (#15, #17).
+
+Version 0.0.1
+-------------
+
+7/04/2014
+
+- Python 2.6 support (#13)
+- Python 3 support (#12)
+- Basic maintenance work (#11, #7)
+- Fix error raising to be pywin32 compatible (#8)
+- Package rename mini_pywin32 -> pywin32-ctypes
+- Add travis-ci integration using wine! (#2)
+- Support basic library and resource loading (#1)
+- mini_pywin32 is born
```

### Comparing `pywin32-ctypes-0.2.1/LICENSE.txt` & `pywin32-ctypes-0.2.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-This software is OSI Certified Open Source Software.
-OSI Certified is a certification mark of the Open Source Initiative.
-
-Copyright (c) 2014, Enthought, Inc.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
- * Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
- * Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
- * Neither the name of Enthought, Inc. nor the names of its contributors may
-   be used to endorse or promote products derived from this software without
-   specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+This software is OSI Certified Open Source Software.
+OSI Certified is a certification mark of the Open Source Initiative.
+
+Copyright (c) 2014, Enthought, Inc.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+ * Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+ * Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+ * Neither the name of Enthought, Inc. nor the names of its contributors may
+   be used to endorse or promote products derived from this software without
+   specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pywin32-ctypes-0.2.1/README.rst` & `pywin32-ctypes-0.2.2/README.rst`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-
-.. image:: https://readthedocs.org/projects/pywin32-ctypes/badge/?version=master
-   :target: http://pywin32-ctypes.readthedocs.org/en/latest/?badge=master
-   :alt: Documentation Status
-
-A reimplementation of pywin32 that is pure python. The default
-behaviour will try to use cffi (>= 1.3.0), if available, and fall back
-to using ctypes. Please note that there is no need to have a compiler
-available on installation or at runtime.
-
-Usage
-=====
-
-Example::
-
-  # Equivalent to 'import win32api' from pywin32.
-  from win32ctypes.pywin32 import win32api
-
-  win32api.LoadLibraryEx(sys.executable, 0, win32api.LOAD_LIBRARY_AS_DATAFILE)
-
-.. note::
-
-   Currently pywin32ctypes implements only a very small subset
-   of pywin32, for internal needs at Enthought. We do welcome
-   additional features and PRs, though.
-
-Development setup
-=================
-
-The following should be good enough::
-
-  pip install -r test_requirements.txt
-  python install -e .
-
-.. note::
-
-   - While pywin32-ctypes should regularly be tested on windows, you can also
-     develop/test on unix by using wine
+
+.. image:: https://readthedocs.org/projects/pywin32-ctypes/badge/?version=master
+   :target: http://pywin32-ctypes.readthedocs.org/en/latest/?badge=master
+   :alt: Documentation Status
+
+A reimplementation of pywin32 that is pure python. The default
+behaviour will try to use cffi (>= 1.3.0), if available, and fall back
+to using ctypes. Please note that there is no need to have a compiler
+available on installation or at runtime.
+
+Usage
+=====
+
+Example::
+
+  # Equivalent to 'import win32api' from pywin32.
+  from win32ctypes.pywin32 import win32api
+
+  win32api.LoadLibraryEx(sys.executable, 0, win32api.LOAD_LIBRARY_AS_DATAFILE)
+
+.. note::
+
+   Currently pywin32ctypes implements only a very small subset
+   of pywin32, for internal needs at Enthought. We do welcome
+   additional features and PRs, though.
+
+Development setup
+=================
+
+The following should be good enough::
+
+  pip install -r test_requirements.txt
+  python install -e .
+
+.. note::
+
+   - While pywin32-ctypes should regularly be tested on windows, you can also
+     develop/test on unix by using wine
```

### Comparing `pywin32-ctypes-0.2.1/docs/Makefile` & `pywin32-ctypes-0.2.2/docs/make.bat`

 * *Files 27% similar despite different names*

```diff
@@ -1,193 +1,264 @@
-# Makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = sphinx-build
-PAPER         =
-BUILDDIR      = build
-
-# User-friendly check for sphinx-build
-ifeq ($(shell which $(SPHINXBUILD) >/dev/null 2>&1; echo $$?), 1)
-$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from http://sphinx-doc.org/)
-endif
-
-# Internal variables.
-PAPEROPT_a4     = -D latex_paper_size=a4
-PAPEROPT_letter = -D latex_paper_size=letter
-ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
-# the i18n builder cannot share the environment and doctrees with the others
-I18NSPHINXOPTS  = $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
-
-.PHONY: help clean html dirhtml singlehtml pickle json htmlhelp qthelp devhelp epub latex latexpdf text man changes linkcheck doctest coverage gettext
-
-help:
-	@echo "Please use \`make <target>' where <target> is one of"
-	@echo "  html       to make standalone HTML files"
-	@echo "  dirhtml    to make HTML files named index.html in directories"
-	@echo "  singlehtml to make a single large HTML file"
-	@echo "  pickle     to make pickle files"
-	@echo "  json       to make JSON files"
-	@echo "  htmlhelp   to make HTML files and a HTML help project"
-	@echo "  qthelp     to make HTML files and a qthelp project"
-	@echo "  applehelp  to make an Apple Help Book"
-	@echo "  devhelp    to make HTML files and a Devhelp project"
-	@echo "  epub       to make an epub"
-	@echo "  latex      to make LaTeX files, you can set PAPER=a4 or PAPER=letter"
-	@echo "  latexpdf   to make LaTeX files and run them through pdflatex"
-	@echo "  latexpdfja to make LaTeX files and run them through platex/dvipdfmx"
-	@echo "  text       to make text files"
-	@echo "  man        to make manual pages"
-	@echo "  texinfo    to make Texinfo files"
-	@echo "  info       to make Texinfo files and run them through makeinfo"
-	@echo "  gettext    to make PO message catalogs"
-	@echo "  changes    to make an overview of all changed/added/deprecated items"
-	@echo "  xml        to make Docutils-native XML files"
-	@echo "  pseudoxml  to make pseudoxml-XML files for display purposes"
-	@echo "  linkcheck  to check all external links for integrity"
-	@echo "  doctest    to run all doctests embedded in the documentation (if enabled)"
-	@echo "  coverage   to run coverage check of the documentation (if enabled)"
-
-clean:
-	rm -rf $(BUILDDIR)/*
-	rm -rf source/api
-
-html:
-	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
-	@echo
-	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
-
-dirhtml:
-	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) $(BUILDDIR)/dirhtml
-	@echo
-	@echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
-
-singlehtml:
-	$(SPHINXBUILD) -b singlehtml $(ALLSPHINXOPTS) $(BUILDDIR)/singlehtml
-	@echo
-	@echo "Build finished. The HTML page is in $(BUILDDIR)/singlehtml."
-
-pickle:
-	$(SPHINXBUILD) -b pickle $(ALLSPHINXOPTS) $(BUILDDIR)/pickle
-	@echo
-	@echo "Build finished; now you can process the pickle files."
-
-json:
-	$(SPHINXBUILD) -b json $(ALLSPHINXOPTS) $(BUILDDIR)/json
-	@echo
-	@echo "Build finished; now you can process the JSON files."
-
-htmlhelp:
-	$(SPHINXBUILD) -b htmlhelp $(ALLSPHINXOPTS) $(BUILDDIR)/htmlhelp
-	@echo
-	@echo "Build finished; now you can run HTML Help Workshop with the" \
-	      ".hhp project file in $(BUILDDIR)/htmlhelp."
-
-qthelp:
-	$(SPHINXBUILD) -b qthelp $(ALLSPHINXOPTS) $(BUILDDIR)/qthelp
-	@echo
-	@echo "Build finished; now you can run "qcollectiongenerator" with the" \
-	      ".qhcp project file in $(BUILDDIR)/qthelp, like this:"
-	@echo "# qcollectiongenerator $(BUILDDIR)/qthelp/PyWin32ctypes.qhcp"
-	@echo "To view the help file:"
-	@echo "# assistant -collectionFile $(BUILDDIR)/qthelp/PyWin32ctypes.qhc"
-
-applehelp:
-	$(SPHINXBUILD) -b applehelp $(ALLSPHINXOPTS) $(BUILDDIR)/applehelp
-	@echo
-	@echo "Build finished. The help book is in $(BUILDDIR)/applehelp."
-	@echo "N.B. You won't be able to view it unless you put it in" \
-	      "~/Library/Documentation/Help or install it in your application" \
-	      "bundle."
-
-devhelp:
-	$(SPHINXBUILD) -b devhelp $(ALLSPHINXOPTS) $(BUILDDIR)/devhelp
-	@echo
-	@echo "Build finished."
-	@echo "To view the help file:"
-	@echo "# mkdir -p $$HOME/.local/share/devhelp/PyWin32ctypes"
-	@echo "# ln -s $(BUILDDIR)/devhelp $$HOME/.local/share/devhelp/PyWin32ctypes"
-	@echo "# devhelp"
-
-epub:
-	$(SPHINXBUILD) -b epub $(ALLSPHINXOPTS) $(BUILDDIR)/epub
-	@echo
-	@echo "Build finished. The epub file is in $(BUILDDIR)/epub."
-
-latex:
-	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
-	@echo
-	@echo "Build finished; the LaTeX files are in $(BUILDDIR)/latex."
-	@echo "Run \`make' in that directory to run these through (pdf)latex" \
-	      "(use \`make latexpdf' here to do that automatically)."
-
-latexpdf:
-	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
-	@echo "Running LaTeX files through pdflatex..."
-	$(MAKE) -C $(BUILDDIR)/latex all-pdf
-	@echo "pdflatex finished; the PDF files are in $(BUILDDIR)/latex."
-
-latexpdfja:
-	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
-	@echo "Running LaTeX files through platex and dvipdfmx..."
-	$(MAKE) -C $(BUILDDIR)/latex all-pdf-ja
-	@echo "pdflatex finished; the PDF files are in $(BUILDDIR)/latex."
-
-text:
-	$(SPHINXBUILD) -b text $(ALLSPHINXOPTS) $(BUILDDIR)/text
-	@echo
-	@echo "Build finished. The text files are in $(BUILDDIR)/text."
-
-man:
-	$(SPHINXBUILD) -b man $(ALLSPHINXOPTS) $(BUILDDIR)/man
-	@echo
-	@echo "Build finished. The manual pages are in $(BUILDDIR)/man."
-
-texinfo:
-	$(SPHINXBUILD) -b texinfo $(ALLSPHINXOPTS) $(BUILDDIR)/texinfo
-	@echo
-	@echo "Build finished. The Texinfo files are in $(BUILDDIR)/texinfo."
-	@echo "Run \`make' in that directory to run these through makeinfo" \
-	      "(use \`make info' here to do that automatically)."
-
-info:
-	$(SPHINXBUILD) -b texinfo $(ALLSPHINXOPTS) $(BUILDDIR)/texinfo
-	@echo "Running Texinfo files through makeinfo..."
-	make -C $(BUILDDIR)/texinfo info
-	@echo "makeinfo finished; the Info files are in $(BUILDDIR)/texinfo."
-
-gettext:
-	$(SPHINXBUILD) -b gettext $(I18NSPHINXOPTS) $(BUILDDIR)/locale
-	@echo
-	@echo "Build finished. The message catalogs are in $(BUILDDIR)/locale."
-
-changes:
-	$(SPHINXBUILD) -b changes $(ALLSPHINXOPTS) $(BUILDDIR)/changes
-	@echo
-	@echo "The overview file is in $(BUILDDIR)/changes."
-
-linkcheck:
-	$(SPHINXBUILD) -b linkcheck $(ALLSPHINXOPTS) $(BUILDDIR)/linkcheck
-	@echo
-	@echo "Link check complete; look for any errors in the above output " \
-	      "or in $(BUILDDIR)/linkcheck/output.txt."
-
-doctest:
-	$(SPHINXBUILD) -b doctest $(ALLSPHINXOPTS) $(BUILDDIR)/doctest
-	@echo "Testing of doctests in the sources finished, look at the " \
-	      "results in $(BUILDDIR)/doctest/output.txt."
-
-coverage:
-	$(SPHINXBUILD) -b coverage $(ALLSPHINXOPTS) $(BUILDDIR)/coverage
-	@echo "Testing of coverage in the sources finished, look at the " \
-	      "results in $(BUILDDIR)/coverage/python.txt."
-
-xml:
-	$(SPHINXBUILD) -b xml $(ALLSPHINXOPTS) $(BUILDDIR)/xml
-	@echo
-	@echo "Build finished. The XML files are in $(BUILDDIR)/xml."
-
-pseudoxml:
-	$(SPHINXBUILD) -b pseudoxml $(ALLSPHINXOPTS) $(BUILDDIR)/pseudoxml
-	@echo
-	@echo "Build finished. The pseudo-XML files are in $(BUILDDIR)/pseudoxml."
+@ECHO OFF
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set BUILDDIR=build
+set ALLSPHINXOPTS=-d %BUILDDIR%/doctrees %SPHINXOPTS% source
+set I18NSPHINXOPTS=%SPHINXOPTS% source
+if NOT "%PAPER%" == "" (
+	set ALLSPHINXOPTS=-D latex_paper_size=%PAPER% %ALLSPHINXOPTS%
+	set I18NSPHINXOPTS=-D latex_paper_size=%PAPER% %I18NSPHINXOPTS%
+)
+
+if "%1" == "" goto help
+
+if "%1" == "help" (
+	:help
+	echo.Please use `make ^<target^>` where ^<target^> is one of
+	echo.  html       to make standalone HTML files
+	echo.  dirhtml    to make HTML files named index.html in directories
+	echo.  singlehtml to make a single large HTML file
+	echo.  pickle     to make pickle files
+	echo.  json       to make JSON files
+	echo.  htmlhelp   to make HTML files and a HTML help project
+	echo.  qthelp     to make HTML files and a qthelp project
+	echo.  devhelp    to make HTML files and a Devhelp project
+	echo.  epub       to make an epub
+	echo.  latex      to make LaTeX files, you can set PAPER=a4 or PAPER=letter
+	echo.  text       to make text files
+	echo.  man        to make manual pages
+	echo.  texinfo    to make Texinfo files
+	echo.  gettext    to make PO message catalogs
+	echo.  changes    to make an overview over all changed/added/deprecated items
+	echo.  xml        to make Docutils-native XML files
+	echo.  pseudoxml  to make pseudoxml-XML files for display purposes
+	echo.  linkcheck  to check all external links for integrity
+	echo.  doctest    to run all doctests embedded in the documentation if enabled
+	echo.  coverage   to run coverage check of the documentation if enabled
+	goto end
+)
+
+if "%1" == "clean" (
+	for /d %%i in (%BUILDDIR%\*) do rmdir /q /s %%i
+	del /q /s %BUILDDIR%\*
+	rmdir /q /s source\api
+	goto end
+)
+
+
+REM Check if sphinx-build is available and fallback to Python version if any
+%SPHINXBUILD% 2> nul
+if errorlevel 9009 goto sphinx_python
+goto sphinx_ok
+
+:sphinx_python
+
+set SPHINXBUILD=python -m sphinx.__init__
+%SPHINXBUILD% 2> nul
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.http://sphinx-doc.org/
+	exit /b 1
+)
+
+:sphinx_ok
+
+
+if "%1" == "html" (
+	%SPHINXBUILD% -b html %ALLSPHINXOPTS% %BUILDDIR%/html
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/html.
+	goto end
+)
+
+if "%1" == "dirhtml" (
+	%SPHINXBUILD% -b dirhtml %ALLSPHINXOPTS% %BUILDDIR%/dirhtml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/dirhtml.
+	goto end
+)
+
+if "%1" == "singlehtml" (
+	%SPHINXBUILD% -b singlehtml %ALLSPHINXOPTS% %BUILDDIR%/singlehtml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/singlehtml.
+	goto end
+)
+
+if "%1" == "pickle" (
+	%SPHINXBUILD% -b pickle %ALLSPHINXOPTS% %BUILDDIR%/pickle
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can process the pickle files.
+	goto end
+)
+
+if "%1" == "json" (
+	%SPHINXBUILD% -b json %ALLSPHINXOPTS% %BUILDDIR%/json
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can process the JSON files.
+	goto end
+)
+
+if "%1" == "htmlhelp" (
+	%SPHINXBUILD% -b htmlhelp %ALLSPHINXOPTS% %BUILDDIR%/htmlhelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can run HTML Help Workshop with the ^
+.hhp project file in %BUILDDIR%/htmlhelp.
+	goto end
+)
+
+if "%1" == "qthelp" (
+	%SPHINXBUILD% -b qthelp %ALLSPHINXOPTS% %BUILDDIR%/qthelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can run "qcollectiongenerator" with the ^
+.qhcp project file in %BUILDDIR%/qthelp, like this:
+	echo.^> qcollectiongenerator %BUILDDIR%\qthelp\PyWin32ctypes.qhcp
+	echo.To view the help file:
+	echo.^> assistant -collectionFile %BUILDDIR%\qthelp\PyWin32ctypes.ghc
+	goto end
+)
+
+if "%1" == "devhelp" (
+	%SPHINXBUILD% -b devhelp %ALLSPHINXOPTS% %BUILDDIR%/devhelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished.
+	goto end
+)
+
+if "%1" == "epub" (
+	%SPHINXBUILD% -b epub %ALLSPHINXOPTS% %BUILDDIR%/epub
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The epub file is in %BUILDDIR%/epub.
+	goto end
+)
+
+if "%1" == "latex" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; the LaTeX files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "latexpdf" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	cd %BUILDDIR%/latex
+	make all-pdf
+	cd %~dp0
+	echo.
+	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "latexpdfja" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	cd %BUILDDIR%/latex
+	make all-pdf-ja
+	cd %~dp0
+	echo.
+	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "text" (
+	%SPHINXBUILD% -b text %ALLSPHINXOPTS% %BUILDDIR%/text
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The text files are in %BUILDDIR%/text.
+	goto end
+)
+
+if "%1" == "man" (
+	%SPHINXBUILD% -b man %ALLSPHINXOPTS% %BUILDDIR%/man
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The manual pages are in %BUILDDIR%/man.
+	goto end
+)
+
+if "%1" == "texinfo" (
+	%SPHINXBUILD% -b texinfo %ALLSPHINXOPTS% %BUILDDIR%/texinfo
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The Texinfo files are in %BUILDDIR%/texinfo.
+	goto end
+)
+
+if "%1" == "gettext" (
+	%SPHINXBUILD% -b gettext %I18NSPHINXOPTS% %BUILDDIR%/locale
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The message catalogs are in %BUILDDIR%/locale.
+	goto end
+)
+
+if "%1" == "changes" (
+	%SPHINXBUILD% -b changes %ALLSPHINXOPTS% %BUILDDIR%/changes
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.The overview file is in %BUILDDIR%/changes.
+	goto end
+)
+
+if "%1" == "linkcheck" (
+	%SPHINXBUILD% -b linkcheck %ALLSPHINXOPTS% %BUILDDIR%/linkcheck
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Link check complete; look for any errors in the above output ^
+or in %BUILDDIR%/linkcheck/output.txt.
+	goto end
+)
+
+if "%1" == "doctest" (
+	%SPHINXBUILD% -b doctest %ALLSPHINXOPTS% %BUILDDIR%/doctest
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Testing of doctests in the sources finished, look at the ^
+results in %BUILDDIR%/doctest/output.txt.
+	goto end
+)
+
+if "%1" == "coverage" (
+	%SPHINXBUILD% -b coverage %ALLSPHINXOPTS% %BUILDDIR%/coverage
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Testing of coverage in the sources finished, look at the ^
+results in %BUILDDIR%/coverage/python.txt.
+	goto end
+)
+
+if "%1" == "xml" (
+	%SPHINXBUILD% -b xml %ALLSPHINXOPTS% %BUILDDIR%/xml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The XML files are in %BUILDDIR%/xml.
+	goto end
+)
+
+if "%1" == "pseudoxml" (
+	%SPHINXBUILD% -b pseudoxml %ALLSPHINXOPTS% %BUILDDIR%/pseudoxml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The pseudo-XML files are in %BUILDDIR%/pseudoxml.
+	goto end
+)
+
+:end
```

### Comparing `pywin32-ctypes-0.2.1/docs/source/conf.py` & `pywin32-ctypes-0.2.2/docs/source/conf.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-# -*- coding: utf-8 -*-
-#
-# PyWin32ctypes documentation build configuration file, created by
-# sphinx-quickstart on Sat Nov 14 12:19:38 2015.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-import sys
-import os
-import shlex
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.abspath('.'))
-
-from mock_missing import mock_modules
-mock_modules()
-
-# -- General configuration ------------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.viewcode',
-    'sectiondoc.styles.default',
-]
-
-autosummary_generate = True
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The encoding of source files.
-#source_encoding = 'utf-8-sig'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = u'PyWin32ctypes'
-copyright = u'2015, Enthought Ltd'
-author = u'David Cournapeau, Ioannis Tziakos'
-
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# The full version, including alpha/beta/rc tags.
-release = open(
-    os.path.join(
-        os.path.dirname(__file__),
-        '..', '..', 'VERSION')).read().strip()
-# The short X.Y version.
-version = '.'.join(release.split('.')[:2])
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# There are two options for replacing |today|: either, you set today to some
-# non-false value, then it is used:
-#today = ''
-# Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-exclude_patterns = []
-
-# The reST default role (used for this markup: `text`) to use for all
-# documents.
-#default_role = None
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
-
-# If true, the current module name will be prepended to all description
-# unit titles (such as .. function::).
-#add_module_names = True
-
-# If true, sectionauthor and moduleauthor directives will be shown in the
-# output. They are ignored by default.
-#show_authors = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
-
-# If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = True
-
-
-# -- Options for HTML output ----------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-html_theme = 'alabaster'
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-#html_theme_options = {}
-
-# Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
-
-# The name for this set of Sphinx documents.  If None, it defaults to
-# "<project> v<release> documentation".
-#html_title = None
-
-# A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
-
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-#html_logo = None
-
-# The name of an image file (within the static path) to use as favicon of the
-# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
-# pixels large.
-#html_favicon = None
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-# Add any extra paths that contain custom files (such as robots.txt or
-# .htaccess) here, relative to this directory. These files are copied
-# directly to the root of the documentation.
-#html_extra_path = []
-
-# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
-# using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
-
-# If true, SmartyPants will be used to convert quotes and dashes to
-# typographically correct entities.
-#html_use_smartypants = True
-
-# Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
-
-# Additional templates that should be rendered to pages, maps page names to
-# template names.
-#html_additional_pages = {}
-
-# If false, no module index is generated.
-#html_domain_indices = True
-
-# If false, no index is generated.
-#html_use_index = True
-
-# If true, the index is split into individual pages for each letter.
-#html_split_index = False
-
-# If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
-
-# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
-
-# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
-
-# If true, an OpenSearch description file will be output, and all pages will
-# contain a <link> tag referring to it.  The value of this option must be the
-# base URL from which the finished HTML is served.
-#html_use_opensearch = ''
-
-# This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
-
-# Language to be used for generating the HTML full-text search index.
-# Sphinx supports the following languages:
-#   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
-#   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
-
-# A dictionary with options for the search language support, empty by default.
-# Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
-
-# The name of a javascript file (relative to the configuration directory) that
-# implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'PyWin32ctypesdoc'
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-  (master_doc, 'PyWin32ctypes.tex', u'PyWin32ctypes Documentation',
-   u'David Cournapeau, Ioannis Tziakos', 'manual'),
-]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-#latex_logo = None
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-#latex_use_parts = False
-
-# If true, show page references after internal links.
-#latex_show_pagerefs = False
-
-# If true, show URL addresses after external links.
-#latex_show_urls = False
-
-# Documents to append as an appendix to all manuals.
-#latex_appendices = []
-
-# If false, no module index is generated.
-#latex_domain_indices = True
-
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'pywin32ctypes', u'PyWin32ctypes Documentation',
-     [author], 1)
-]
-
-# If true, show URL addresses after external links.
-#man_show_urls = False
-
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-  (master_doc, 'PyWin32ctypes', u'PyWin32ctypes Documentation',
-   author, 'PyWin32ctypes', 'One line description of project.',
-   'Miscellaneous'),
-]
-
-# Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
-
-# If false, no module index is generated.
-#texinfo_domain_indices = True
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
-
-# If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
-
-
-# -- Options for Epub output ----------------------------------------------
-
-# Bibliographic Dublin Core info.
-epub_title = project
-epub_author = author
-epub_publisher = author
-epub_copyright = copyright
-
-# The basename for the epub file. It defaults to the project name.
-#epub_basename = project
-
-# The HTML theme for the epub output. Since the default themes are not optimized
-# for small screen space, using the same theme for HTML and epub output is
-# usually not wise. This defaults to 'epub', a theme designed to save visual
-# space.
-#epub_theme = 'epub'
-
-# The language of the text. It defaults to the language option
-# or 'en' if the language is not set.
-#epub_language = ''
-
-# The scheme of the identifier. Typical schemes are ISBN or URL.
-#epub_scheme = ''
-
-# The unique identifier of the text. This can be a ISBN number
-# or the project homepage.
-#epub_identifier = ''
-
-# A unique identification for the text.
-#epub_uid = ''
-
-# A tuple containing the cover image and cover page html template filenames.
-#epub_cover = ()
-
-# A sequence of (type, uri, title) tuples for the guide element of content.opf.
-#epub_guide = ()
-
-# HTML files that should be inserted before the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-#epub_pre_files = []
-
-# HTML files shat should be inserted after the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-#epub_post_files = []
-
-# A list of files that should not be packed into the epub file.
-epub_exclude_files = ['search.html']
-
-# The depth of the table of contents in toc.ncx.
-#epub_tocdepth = 3
-
-# Allow duplicate toc entries.
-#epub_tocdup = True
-
-# Choose between 'default' and 'includehidden'.
-#epub_tocscope = 'default'
-
-# Fix unsupported image types using the Pillow.
-#epub_fix_images = False
-
-# Scale large images.
-#epub_max_image_width = 0
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-#epub_show_urls = 'inline'
-
-# If false, no index is generated.
-#epub_use_index = True
-
-
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+# -*- coding: utf-8 -*-
+#
+# PyWin32ctypes documentation build configuration file, created by
+# sphinx-quickstart on Sat Nov 14 12:19:38 2015.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+import sys
+import os
+import shlex
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+sys.path.insert(0, os.path.abspath('.'))
+
+from mock_missing import mock_modules
+mock_modules()
+
+# -- General configuration ------------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.autosummary',
+    'sphinx.ext.intersphinx',
+    'sphinx.ext.todo',
+    'sphinx.ext.coverage',
+    'sphinx.ext.viewcode',
+    'sectiondoc.styles.default',
+]
+
+autosummary_generate = True
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The encoding of source files.
+#source_encoding = 'utf-8-sig'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = u'PyWin32ctypes'
+copyright = u'2015, Enthought Ltd'
+author = u'David Cournapeau, Ioannis Tziakos'
+
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+#
+# The full version, including alpha/beta/rc tags.
+release = open(
+    os.path.join(
+        os.path.dirname(__file__),
+        '..', '..', 'VERSION')).read().strip()
+# The short X.Y version.
+version = '.'.join(release.split('.')[:2])
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# There are two options for replacing |today|: either, you set today to some
+# non-false value, then it is used:
+#today = ''
+# Else, today_fmt is used as the format for a strftime call.
+#today_fmt = '%B %d, %Y'
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+exclude_patterns = []
+
+# The reST default role (used for this markup: `text`) to use for all
+# documents.
+#default_role = None
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+#add_function_parentheses = True
+
+# If true, the current module name will be prepended to all description
+# unit titles (such as .. function::).
+#add_module_names = True
+
+# If true, sectionauthor and moduleauthor directives will be shown in the
+# output. They are ignored by default.
+#show_authors = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# A list of ignored prefixes for module index sorting.
+#modindex_common_prefix = []
+
+# If true, keep warnings as "system message" paragraphs in the built documents.
+#keep_warnings = False
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = True
+
+
+# -- Options for HTML output ----------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+html_theme = 'alabaster'
+
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
+# documentation.
+#html_theme_options = {}
+
+# Add any paths that contain custom themes here, relative to this directory.
+#html_theme_path = []
+
+# The name for this set of Sphinx documents.  If None, it defaults to
+# "<project> v<release> documentation".
+#html_title = None
+
+# A shorter title for the navigation bar.  Default is the same as html_title.
+#html_short_title = None
+
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
+#html_logo = None
+
+# The name of an image file (within the static path) to use as favicon of the
+# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
+# pixels large.
+#html_favicon = None
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+# Add any extra paths that contain custom files (such as robots.txt or
+# .htaccess) here, relative to this directory. These files are copied
+# directly to the root of the documentation.
+#html_extra_path = []
+
+# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
+# using the given strftime format.
+#html_last_updated_fmt = '%b %d, %Y'
+
+# If true, SmartyPants will be used to convert quotes and dashes to
+# typographically correct entities.
+#html_use_smartypants = True
+
+# Custom sidebar templates, maps document names to template names.
+#html_sidebars = {}
+
+# Additional templates that should be rendered to pages, maps page names to
+# template names.
+#html_additional_pages = {}
+
+# If false, no module index is generated.
+#html_domain_indices = True
+
+# If false, no index is generated.
+#html_use_index = True
+
+# If true, the index is split into individual pages for each letter.
+#html_split_index = False
+
+# If true, links to the reST sources are added to the pages.
+#html_show_sourcelink = True
+
+# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
+#html_show_sphinx = True
+
+# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
+#html_show_copyright = True
+
+# If true, an OpenSearch description file will be output, and all pages will
+# contain a <link> tag referring to it.  The value of this option must be the
+# base URL from which the finished HTML is served.
+#html_use_opensearch = ''
+
+# This is the file name suffix for HTML files (e.g. ".xhtml").
+#html_file_suffix = None
+
+# Language to be used for generating the HTML full-text search index.
+# Sphinx supports the following languages:
+#   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
+#   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
+#html_search_language = 'en'
+
+# A dictionary with options for the search language support, empty by default.
+# Now only 'ja' uses this config value
+#html_search_options = {'type': 'default'}
+
+# The name of a javascript file (relative to the configuration directory) that
+# implements a search results scorer. If empty, the default will be used.
+#html_search_scorer = 'scorer.js'
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'PyWin32ctypesdoc'
+
+# -- Options for LaTeX output ---------------------------------------------
+
+latex_elements = {
+# The paper size ('letterpaper' or 'a4paper').
+#'papersize': 'letterpaper',
+
+# The font size ('10pt', '11pt' or '12pt').
+#'pointsize': '10pt',
+
+# Additional stuff for the LaTeX preamble.
+#'preamble': '',
+
+# Latex figure (float) alignment
+#'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title,
+#  author, documentclass [howto, manual, or own class]).
+latex_documents = [
+  (master_doc, 'PyWin32ctypes.tex', u'PyWin32ctypes Documentation',
+   u'David Cournapeau, Ioannis Tziakos', 'manual'),
+]
+
+# The name of an image file (relative to this directory) to place at the top of
+# the title page.
+#latex_logo = None
+
+# For "manual" documents, if this is true, then toplevel headings are parts,
+# not chapters.
+#latex_use_parts = False
+
+# If true, show page references after internal links.
+#latex_show_pagerefs = False
+
+# If true, show URL addresses after external links.
+#latex_show_urls = False
+
+# Documents to append as an appendix to all manuals.
+#latex_appendices = []
+
+# If false, no module index is generated.
+#latex_domain_indices = True
+
+
+# -- Options for manual page output ---------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'pywin32ctypes', u'PyWin32ctypes Documentation',
+     [author], 1)
+]
+
+# If true, show URL addresses after external links.
+#man_show_urls = False
+
+
+# -- Options for Texinfo output -------------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+  (master_doc, 'PyWin32ctypes', u'PyWin32ctypes Documentation',
+   author, 'PyWin32ctypes', 'One line description of project.',
+   'Miscellaneous'),
+]
+
+# Documents to append as an appendix to all manuals.
+#texinfo_appendices = []
+
+# If false, no module index is generated.
+#texinfo_domain_indices = True
+
+# How to display URL addresses: 'footnote', 'no', or 'inline'.
+#texinfo_show_urls = 'footnote'
+
+# If true, do not generate a @detailmenu in the "Top" node's menu.
+#texinfo_no_detailmenu = False
+
+
+# -- Options for Epub output ----------------------------------------------
+
+# Bibliographic Dublin Core info.
+epub_title = project
+epub_author = author
+epub_publisher = author
+epub_copyright = copyright
+
+# The basename for the epub file. It defaults to the project name.
+#epub_basename = project
+
+# The HTML theme for the epub output. Since the default themes are not optimized
+# for small screen space, using the same theme for HTML and epub output is
+# usually not wise. This defaults to 'epub', a theme designed to save visual
+# space.
+#epub_theme = 'epub'
+
+# The language of the text. It defaults to the language option
+# or 'en' if the language is not set.
+#epub_language = ''
+
+# The scheme of the identifier. Typical schemes are ISBN or URL.
+#epub_scheme = ''
+
+# The unique identifier of the text. This can be a ISBN number
+# or the project homepage.
+#epub_identifier = ''
+
+# A unique identification for the text.
+#epub_uid = ''
+
+# A tuple containing the cover image and cover page html template filenames.
+#epub_cover = ()
+
+# A sequence of (type, uri, title) tuples for the guide element of content.opf.
+#epub_guide = ()
+
+# HTML files that should be inserted before the pages created by sphinx.
+# The format is a list of tuples containing the path and title.
+#epub_pre_files = []
+
+# HTML files shat should be inserted after the pages created by sphinx.
+# The format is a list of tuples containing the path and title.
+#epub_post_files = []
+
+# A list of files that should not be packed into the epub file.
+epub_exclude_files = ['search.html']
+
+# The depth of the table of contents in toc.ncx.
+#epub_tocdepth = 3
+
+# Allow duplicate toc entries.
+#epub_tocdup = True
+
+# Choose between 'default' and 'includehidden'.
+#epub_tocscope = 'default'
+
+# Fix unsupported image types using the Pillow.
+#epub_fix_images = False
+
+# Scale large images.
+#epub_max_image_width = 0
+
+# How to display URL addresses: 'footnote', 'no', or 'inline'.
+#epub_show_urls = 'inline'
+
+# If false, no index is generated.
+#epub_use_index = True
+
+
+# Example configuration for intersphinx: refer to the Python standard library.
+intersphinx_mapping = {'https://docs.python.org/': None}
```

### Comparing `pywin32-ctypes-0.2.1/docs/source/mock_missing.py` & `pywin32-ctypes-0.2.2/docs/source/mock_missing.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#------------------------------------------------------------------------------
-#
-#  Copyright (c) 2015, Enthought, Inc.
-#  All rights reserved.
-#
-#  This software is provided without warranty under the terms of the BSD
-#  license included in LICENSE.txt and may be redistributed only
-#  under the conditions described in the aforementioned license.  The license
-#  is also available online at http://www.enthought.com/licenses/BSD.txt
-#
-#  Thanks for using Enthought open source!
-#
-#------------------------------------------------------------------------------
-import sys
-
-
-def mock_modules():
-    """ Mock missing modules if necessary """
-
-    MOCK_MODULES = []
-    MOCK_TYPES = []
-
-    try:
-        import cffi
-    except ImportError:
-        MOCK_MODULES = ['cffi']
-        MOCK_TYPES = []
-    else:
-        del cffi
-
-    TYPES = {
-        mock_type: type(mock_type, bases, {'__module__': path})
-        for path, mock_type, bases in MOCK_TYPES}
-
-    class DocMock(object):
-
-        def __init__(self, *args, **kwds):
-            if '__doc_mocked_name__' in kwds:
-                self.__docmock_name__ = kwds['__docmocked_name__']
-            else:
-                self.__docmock_name__ = 'Unknown'
-
-        def __getattr__(self, name):
-            if name in ('__file__', '__path__'):
-                return '/dev/null'
-            elif name == '__all__':
-                return []
-            else:
-                return TYPES.get(name, DocMock(__docmock_name__=name))
-
-        def __call__(self, *args, **kwards):
-            return DocMock()
-
-        def __iter__(self):
-            return self
-
-        def __next__(self):
-            raise StopIteration()
-
-        def next(self):
-            raise StopIteration()
-
-        @property
-        def __name__(self):
-            return self.__docmock_name__
-
-        def __repr__(self):
-            return '<DocMock.{}>'.format(self.__name__)
-
-    sys.modules.update(
-        (mod_name, DocMock(mocked_name=mod_name)) for mod_name in MOCK_MODULES)
-    print('mocking modules {} and types {}'.format(MOCK_MODULES, MOCK_TYPES))
+#------------------------------------------------------------------------------
+#
+#  Copyright (c) 2015, Enthought, Inc.
+#  All rights reserved.
+#
+#  This software is provided without warranty under the terms of the BSD
+#  license included in LICENSE.txt and may be redistributed only
+#  under the conditions described in the aforementioned license.  The license
+#  is also available online at http://www.enthought.com/licenses/BSD.txt
+#
+#  Thanks for using Enthought open source!
+#
+#------------------------------------------------------------------------------
+import sys
+
+
+def mock_modules():
+    """ Mock missing modules if necessary """
+
+    MOCK_MODULES = []
+    MOCK_TYPES = []
+
+    try:
+        import cffi
+    except ImportError:
+        MOCK_MODULES = ['cffi']
+        MOCK_TYPES = []
+    else:
+        del cffi
+
+    TYPES = {
+        mock_type: type(mock_type, bases, {'__module__': path})
+        for path, mock_type, bases in MOCK_TYPES}
+
+    class DocMock(object):
+
+        def __init__(self, *args, **kwds):
+            if '__doc_mocked_name__' in kwds:
+                self.__docmock_name__ = kwds['__docmocked_name__']
+            else:
+                self.__docmock_name__ = 'Unknown'
+
+        def __getattr__(self, name):
+            if name in ('__file__', '__path__'):
+                return '/dev/null'
+            elif name == '__all__':
+                return []
+            else:
+                return TYPES.get(name, DocMock(__docmock_name__=name))
+
+        def __call__(self, *args, **kwards):
+            return DocMock()
+
+        def __iter__(self):
+            return self
+
+        def __next__(self):
+            raise StopIteration()
+
+        def next(self):
+            raise StopIteration()
+
+        @property
+        def __name__(self):
+            return self.__docmock_name__
+
+        def __repr__(self):
+            return '<DocMock.{}>'.format(self.__name__)
+
+    sys.modules.update(
+        (mod_name, DocMock(mocked_name=mod_name)) for mod_name in MOCK_MODULES)
+    print('mocking modules {} and types {}'.format(MOCK_MODULES, MOCK_TYPES))
```

### Comparing `pywin32-ctypes-0.2.1/docs/source/pywin32.rst` & `pywin32-ctypes-0.2.2/docs/source/pywin32.rst`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-PyWin32 Compatibility Layer
-===========================
-
-The win32ctypes library provides a compatibility layer with
-PyWin32. We attempt to keep the signature of the Functions and their
-behaviour as close as possible to PyWin32. For details and behaviour
-please refer to the Pywin32 documentation and the related
-`MSDN <https://msdn.microsoft.com>`_ reference pages.
-
-
-.. autosummary::
-   :toctree: api
-   :template: module_template.rst
-
-   win32ctypes.pywin32.win32api
-   win32ctypes.pywin32.win32cred
-   win32ctypes.pywin32.pywintypes
+PyWin32 Compatibility Layer
+===========================
+
+The win32ctypes library provides a compatibility layer with
+PyWin32. We attempt to keep the signature of the Functions and their
+behaviour as close as possible to PyWin32. For details and behaviour
+please refer to the Pywin32 documentation and the related
+`MSDN <https://msdn.microsoft.com>`_ reference pages.
+
+
+.. autosummary::
+   :toctree: api
+   :template: module_template.rst
+
+   win32ctypes.pywin32.win32api
+   win32ctypes.pywin32.win32cred
+   win32ctypes.pywin32.pywintypes
```

### Comparing `pywin32-ctypes-0.2.1/pywin32_ctypes.egg-info/SOURCES.txt` & `pywin32-ctypes-0.2.2/pywin32_ctypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_authentication.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_authentication.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-#
-# (C) Copyright 2015 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-from weakref import WeakKeyDictionary
-
-from win32ctypes.core.compat import is_text
-from ._util import ffi, check_false, dlls
-from ._nl_support import _GetACP
-from ._common import _PyBytes_FromStringAndSize
-
-
-ffi.cdef("""
-
-typedef struct _FILETIME {
-  DWORD dwLowDateTime;
-  DWORD dwHighDateTime;
-} FILETIME, *PFILETIME;
-
-typedef struct _CREDENTIAL_ATTRIBUTE {
-  LPWSTR Keyword;
-  DWORD  Flags;
-  DWORD  ValueSize;
-  LPBYTE Value;
-} CREDENTIAL_ATTRIBUTE, *PCREDENTIAL_ATTRIBUTE;
-
-typedef struct _CREDENTIAL {
-  DWORD                 Flags;
-  DWORD                 Type;
-  LPWSTR                TargetName;
-  LPWSTR                Comment;
-  FILETIME              LastWritten;
-  DWORD                 CredentialBlobSize;
-  LPBYTE                CredentialBlob;
-  DWORD                 Persist;
-  DWORD                 AttributeCount;
-  PCREDENTIAL_ATTRIBUTE Attributes;
-  LPWSTR                TargetAlias;
-  LPWSTR                UserName;
-} CREDENTIAL, *PCREDENTIAL;
-
-
-BOOL WINAPI CredReadW(
-    LPCWSTR TargetName, DWORD Type, DWORD Flags, PCREDENTIAL *Credential);
-BOOL WINAPI CredWriteW(PCREDENTIAL Credential, DWORD);
-VOID WINAPI CredFree(PVOID Buffer);
-BOOL WINAPI CredDeleteW(LPCWSTR TargetName, DWORD Type, DWORD Flags);
-BOOL WINAPI CredEnumerateW(
-    LPCWSTR Filter, DWORD Flags, DWORD *Count, PCREDENTIAL **Credential);
-""")
-
-_keep_alive = WeakKeyDictionary()
-
-
-SUPPORTED_CREDKEYS = set((
-    u'Type', u'TargetName', u'Persist',
-    u'UserName', u'Comment', u'CredentialBlob'))
-
-
-def make_unicode(password):
-    """ Convert the input string to unicode.
-
-    """
-    if is_text(password):
-        return password
-    else:
-        code_page = _GetACP()
-        return password.decode(encoding=str(code_page), errors='strict')
-
-
-class _CREDENTIAL(object):
-
-    def __call__(self):
-        return ffi.new("PCREDENTIAL")[0]
-
-    @classmethod
-    def fromdict(cls, credential, flag=0):
-        unsupported = set(credential.keys()) - SUPPORTED_CREDKEYS
-        if len(unsupported):
-            raise ValueError("Unsupported keys: {0}".format(unsupported))
-        if flag != 0:
-            raise ValueError("flag != 0 not yet supported")
-
-        factory = cls()
-        c_creds = factory()
-        # values to ref and make sure that they will not go away
-        values = []
-        for key, value in credential.items():
-            if key == u'CredentialBlob':
-                blob = make_unicode(value)
-                blob_data = ffi.new('wchar_t[]', blob)
-                # new adds a NULL at the end that we do not want.
-                c_creds.CredentialBlobSize = \
-                    ffi.sizeof(blob_data) - ffi.sizeof('wchar_t')
-                c_creds.CredentialBlob = ffi.cast('LPBYTE', blob_data)
-                values.append(blob_data)
-            elif key in (u'Type', u'Persist'):
-                setattr(c_creds, key, value)
-            elif value is None:
-                setattr(c_creds, key, ffi.NULL)
-            else:
-                blob = make_unicode(value)
-                pblob = ffi.new('wchar_t[]', blob)
-                values.append(pblob)
-                setattr(c_creds, key, ffi.cast('LPTSTR', pblob))
-        # keep values alive until c_creds goes away.
-        _keep_alive[c_creds] = tuple(values)
-        return c_creds
-
-
-CREDENTIAL = _CREDENTIAL()
-
-
-def PCREDENTIAL(value=None):
-    return ffi.new("PCREDENTIAL", ffi.NULL if value is None else value)
-
-
-def PPCREDENTIAL(value=None):
-    return ffi.new("PCREDENTIAL*", ffi.NULL if value is None else value)
-
-
-def PPPCREDENTIAL(value=None):
-    return ffi.new("PCREDENTIAL**", ffi.NULL if value is None else value)
-
-
-def credential2dict(pc_creds):
-    credentials = {}
-    for key in SUPPORTED_CREDKEYS:
-        if key == u'CredentialBlob':
-            data = _PyBytes_FromStringAndSize(
-                pc_creds.CredentialBlob, pc_creds.CredentialBlobSize)
-        elif key in (u'Type', u'Persist'):
-            data = int(getattr(pc_creds, key))
-        else:
-            string_pointer = getattr(pc_creds, key)
-            if string_pointer == ffi.NULL:
-                data = None
-            else:
-                data = ffi.string(string_pointer)
-        credentials[key] = data
-    return credentials
-
-
-def _CredRead(TargetName, Type, Flags, ppCredential):
-    target = make_unicode(TargetName)
-    return check_false(
-        dlls.advapi32.CredReadW(target, Type, Flags, ppCredential),
-        u'CredRead')
-
-
-def _CredWrite(Credential, Flags):
-    return check_false(
-        dlls.advapi32.CredWriteW(Credential, Flags), u'CredWrite')
-
-
-def _CredDelete(TargetName, Type, Flags):
-    return check_false(
-        dlls.advapi32.CredDeleteW(
-            make_unicode(TargetName), Type, Flags), u'CredDelete')
-
-
-def _CredEnumerate(Filter, Flags, Count, pppCredential):
-    filter = make_unicode(Filter) if Filter is not None else ffi.NULL
-    return check_false(
-        dlls.advapi32.CredEnumerateW(filter, Flags, Count, pppCredential),
-        u'CredEnumerate')
-
-
-_CredFree = dlls.advapi32.CredFree
+#
+# (C) Copyright 2015 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+from weakref import WeakKeyDictionary
+
+from win32ctypes.core.compat import is_text
+from ._util import ffi, check_false, dlls
+from ._nl_support import _GetACP
+from ._common import _PyBytes_FromStringAndSize
+
+
+ffi.cdef("""
+
+typedef struct _FILETIME {
+  DWORD dwLowDateTime;
+  DWORD dwHighDateTime;
+} FILETIME, *PFILETIME;
+
+typedef struct _CREDENTIAL_ATTRIBUTE {
+  LPWSTR Keyword;
+  DWORD  Flags;
+  DWORD  ValueSize;
+  LPBYTE Value;
+} CREDENTIAL_ATTRIBUTE, *PCREDENTIAL_ATTRIBUTE;
+
+typedef struct _CREDENTIAL {
+  DWORD                 Flags;
+  DWORD                 Type;
+  LPWSTR                TargetName;
+  LPWSTR                Comment;
+  FILETIME              LastWritten;
+  DWORD                 CredentialBlobSize;
+  LPBYTE                CredentialBlob;
+  DWORD                 Persist;
+  DWORD                 AttributeCount;
+  PCREDENTIAL_ATTRIBUTE Attributes;
+  LPWSTR                TargetAlias;
+  LPWSTR                UserName;
+} CREDENTIAL, *PCREDENTIAL;
+
+
+BOOL WINAPI CredReadW(
+    LPCWSTR TargetName, DWORD Type, DWORD Flags, PCREDENTIAL *Credential);
+BOOL WINAPI CredWriteW(PCREDENTIAL Credential, DWORD);
+VOID WINAPI CredFree(PVOID Buffer);
+BOOL WINAPI CredDeleteW(LPCWSTR TargetName, DWORD Type, DWORD Flags);
+BOOL WINAPI CredEnumerateW(
+    LPCWSTR Filter, DWORD Flags, DWORD *Count, PCREDENTIAL **Credential);
+""")
+
+_keep_alive = WeakKeyDictionary()
+
+
+SUPPORTED_CREDKEYS = set((
+    u'Type', u'TargetName', u'Persist',
+    u'UserName', u'Comment', u'CredentialBlob'))
+
+
+def make_unicode(password):
+    """ Convert the input string to unicode.
+
+    """
+    if is_text(password):
+        return password
+    else:
+        code_page = _GetACP()
+        return password.decode(encoding=str(code_page), errors='strict')
+
+
+class _CREDENTIAL(object):
+
+    def __call__(self):
+        return ffi.new("PCREDENTIAL")[0]
+
+    @classmethod
+    def fromdict(cls, credential, flag=0):
+        unsupported = set(credential.keys()) - SUPPORTED_CREDKEYS
+        if len(unsupported):
+            raise ValueError("Unsupported keys: {0}".format(unsupported))
+        if flag != 0:
+            raise ValueError("flag != 0 not yet supported")
+
+        factory = cls()
+        c_creds = factory()
+        # values to ref and make sure that they will not go away
+        values = []
+        for key, value in credential.items():
+            if key == u'CredentialBlob':
+                blob = make_unicode(value)
+                blob_data = ffi.new('wchar_t[]', blob)
+                # new adds a NULL at the end that we do not want.
+                c_creds.CredentialBlobSize = \
+                    ffi.sizeof(blob_data) - ffi.sizeof('wchar_t')
+                c_creds.CredentialBlob = ffi.cast('LPBYTE', blob_data)
+                values.append(blob_data)
+            elif key in (u'Type', u'Persist'):
+                setattr(c_creds, key, value)
+            elif value is None:
+                setattr(c_creds, key, ffi.NULL)
+            else:
+                blob = make_unicode(value)
+                pblob = ffi.new('wchar_t[]', blob)
+                values.append(pblob)
+                setattr(c_creds, key, ffi.cast('LPTSTR', pblob))
+        # keep values alive until c_creds goes away.
+        _keep_alive[c_creds] = tuple(values)
+        return c_creds
+
+
+CREDENTIAL = _CREDENTIAL()
+
+
+def PCREDENTIAL(value=None):
+    return ffi.new("PCREDENTIAL", ffi.NULL if value is None else value)
+
+
+def PPCREDENTIAL(value=None):
+    return ffi.new("PCREDENTIAL*", ffi.NULL if value is None else value)
+
+
+def PPPCREDENTIAL(value=None):
+    return ffi.new("PCREDENTIAL**", ffi.NULL if value is None else value)
+
+
+def credential2dict(pc_creds):
+    credentials = {}
+    for key in SUPPORTED_CREDKEYS:
+        if key == u'CredentialBlob':
+            data = _PyBytes_FromStringAndSize(
+                pc_creds.CredentialBlob, pc_creds.CredentialBlobSize)
+        elif key in (u'Type', u'Persist'):
+            data = int(getattr(pc_creds, key))
+        else:
+            string_pointer = getattr(pc_creds, key)
+            if string_pointer == ffi.NULL:
+                data = None
+            else:
+                data = ffi.string(string_pointer)
+        credentials[key] = data
+    return credentials
+
+
+def _CredRead(TargetName, Type, Flags, ppCredential):
+    target = make_unicode(TargetName)
+    return check_false(
+        dlls.advapi32.CredReadW(target, Type, Flags, ppCredential),
+        u'CredRead')
+
+
+def _CredWrite(Credential, Flags):
+    return check_false(
+        dlls.advapi32.CredWriteW(Credential, Flags), u'CredWrite')
+
+
+def _CredDelete(TargetName, Type, Flags):
+    return check_false(
+        dlls.advapi32.CredDeleteW(
+            make_unicode(TargetName), Type, Flags), u'CredDelete')
+
+
+def _CredEnumerate(Filter, Flags, Count, pppCredential):
+    filter = make_unicode(Filter) if Filter is not None else ffi.NULL
+    return check_false(
+        dlls.advapi32.CredEnumerateW(filter, Flags, Count, pppCredential),
+        u'CredEnumerate')
+
+
+_CredFree = dlls.advapi32.CredFree
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_resource.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_resource.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#
-# (C) Copyright 2015 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-from ._util import (
-    ffi, check_null, check_zero, check_false, HMODULE,
-    PVOID, RESOURCE, resource, dlls)
-
-
-ffi.cdef("""
-
-typedef int WINBOOL;
-typedef WINBOOL (__stdcall *ENUMRESTYPEPROC) (HANDLE, LPTSTR, LONG_PTR);
-typedef WINBOOL (__stdcall *ENUMRESNAMEPROC) (HANDLE, LPCTSTR, LPTSTR, LONG_PTR);
-typedef WINBOOL (__stdcall *ENUMRESLANGPROC) (HANDLE, LPCTSTR, LPCTSTR, WORD, LONG_PTR);
-
-BOOL WINAPI EnumResourceTypesW(
-    HMODULE hModule, ENUMRESTYPEPROC lpEnumFunc, LONG_PTR lParam);
-BOOL WINAPI EnumResourceNamesW(
-    HMODULE hModule, LPCTSTR lpszType,
-    ENUMRESNAMEPROC lpEnumFunc, LONG_PTR lParam);
-BOOL WINAPI EnumResourceLanguagesW(
-    HMODULE hModule, LPCTSTR lpType,
-    LPCTSTR lpName, ENUMRESLANGPROC lpEnumFunc, LONG_PTR lParam);
-HRSRC WINAPI FindResourceExW(
-    HMODULE hModule, LPCTSTR lpType, LPCTSTR lpName, WORD wLanguage);
-DWORD WINAPI SizeofResource(HMODULE hModule, HRSRC hResInfo);
-HGLOBAL WINAPI LoadResource(HMODULE hModule, HRSRC hResInfo);
-LPVOID WINAPI LockResource(HGLOBAL hResData);
-
-HANDLE WINAPI BeginUpdateResourceW(LPCTSTR pFileName, BOOL bDeleteExistingResources);
-BOOL WINAPI EndUpdateResourceW(HANDLE hUpdate, BOOL fDiscard);
-BOOL WINAPI UpdateResourceW(HANDLE hUpdate, LPCTSTR lpType, LPCTSTR lpName, WORD wLanguage, LPVOID lpData, DWORD cbData);
-
-""")  # noqa
-
-
-def ENUMRESTYPEPROC(callback):
-    def wrapped(hModule, lpszType, lParam):
-        return callback(hModule, resource(lpszType), lParam)
-    return wrapped
-
-
-def ENUMRESNAMEPROC(callback):
-    def wrapped(hModule, lpszType, lpszName, lParam):
-        if lpszName == ffi.NULL:
-            return False
-        return callback(
-            hModule, resource(lpszType), resource(lpszName), lParam)
-    return wrapped
-
-
-def ENUMRESLANGPROC(callback):
-    def wrapped(hModule, lpszType, lpszName, wIDLanguage, lParam):
-        return callback(
-            hModule, resource(lpszType), resource(lpszName),
-            wIDLanguage, lParam)
-    return wrapped
-
-
-def _EnumResourceTypes(hModule, lpEnumFunc, lParam):
-    callback = ffi.callback('ENUMRESTYPEPROC', lpEnumFunc)
-    check_false(
-        dlls.kernel32.EnumResourceTypesW(PVOID(hModule), callback, lParam),
-        function_name='EnumResourceTypes')
-
-
-def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
-    callback = ffi.callback('ENUMRESNAMEPROC', lpEnumFunc)
-    check_false(
-        dlls.kernel32.EnumResourceNamesW(
-            PVOID(hModule), RESOURCE(lpszType), callback, lParam),
-        function_name='EnumResourceNames')
-
-
-def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
-    callback = ffi.callback('ENUMRESLANGPROC', lpEnumFunc)
-    check_false(
-        dlls.kernel32.EnumResourceLanguagesW(
-            PVOID(hModule), RESOURCE(lpType),
-            RESOURCE(lpName), callback, lParam),
-        function_name='EnumResourceLanguages')
-
-
-def _FindResourceEx(hModule, lpType, lpName, wLanguage):
-    return check_null(
-        dlls.kernel32.FindResourceExW(
-            PVOID(hModule), RESOURCE(lpType), RESOURCE(lpName), wLanguage),
-        function_name='FindResourceEx')
-
-
-def _SizeofResource(hModule, hResInfo):
-    return check_zero(
-        dlls.kernel32.SizeofResource(PVOID(hModule), hResInfo),
-        function_name='SizeofResource')
-
-
-def _LoadResource(hModule, hResInfo):
-    return check_null(
-        dlls.kernel32.LoadResource(PVOID(hModule), hResInfo),
-        function_name='LoadResource')
-
-
-def _LockResource(hResData):
-    return check_null(
-        dlls.kernel32.LockResource(hResData),
-        function_name='LockResource')
-
-
-def _BeginUpdateResource(pFileName, bDeleteExistingResources):
-    result = check_null(
-        dlls.kernel32.BeginUpdateResourceW(
-            str(pFileName), bDeleteExistingResources))
-    return HMODULE(result)
-
-
-def _EndUpdateResource(hUpdate, fDiscard):
-    check_false(
-        dlls.kernel32.EndUpdateResourceW(PVOID(hUpdate), fDiscard),
-        function_name='EndUpdateResource')
-
-
-def _UpdateResource(hUpdate, lpType, lpName, wLanguage, cData, cbData):
-    lpData = ffi.from_buffer(cData)
-    check_false(
-        dlls.kernel32.UpdateResourceW(
-            PVOID(hUpdate), RESOURCE(lpType), RESOURCE(lpName),
-            wLanguage, PVOID(lpData), cbData),
-        function_name='UpdateResource')
+#
+# (C) Copyright 2015 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+from ._util import (
+    ffi, check_null, check_zero, check_false, HMODULE,
+    PVOID, RESOURCE, resource, dlls)
+
+
+ffi.cdef("""
+
+typedef int WINBOOL;
+typedef WINBOOL (__stdcall *ENUMRESTYPEPROC) (HANDLE, LPTSTR, LONG_PTR);
+typedef WINBOOL (__stdcall *ENUMRESNAMEPROC) (HANDLE, LPCTSTR, LPTSTR, LONG_PTR);
+typedef WINBOOL (__stdcall *ENUMRESLANGPROC) (HANDLE, LPCTSTR, LPCTSTR, WORD, LONG_PTR);
+
+BOOL WINAPI EnumResourceTypesW(
+    HMODULE hModule, ENUMRESTYPEPROC lpEnumFunc, LONG_PTR lParam);
+BOOL WINAPI EnumResourceNamesW(
+    HMODULE hModule, LPCTSTR lpszType,
+    ENUMRESNAMEPROC lpEnumFunc, LONG_PTR lParam);
+BOOL WINAPI EnumResourceLanguagesW(
+    HMODULE hModule, LPCTSTR lpType,
+    LPCTSTR lpName, ENUMRESLANGPROC lpEnumFunc, LONG_PTR lParam);
+HRSRC WINAPI FindResourceExW(
+    HMODULE hModule, LPCTSTR lpType, LPCTSTR lpName, WORD wLanguage);
+DWORD WINAPI SizeofResource(HMODULE hModule, HRSRC hResInfo);
+HGLOBAL WINAPI LoadResource(HMODULE hModule, HRSRC hResInfo);
+LPVOID WINAPI LockResource(HGLOBAL hResData);
+
+HANDLE WINAPI BeginUpdateResourceW(LPCTSTR pFileName, BOOL bDeleteExistingResources);
+BOOL WINAPI EndUpdateResourceW(HANDLE hUpdate, BOOL fDiscard);
+BOOL WINAPI UpdateResourceW(HANDLE hUpdate, LPCTSTR lpType, LPCTSTR lpName, WORD wLanguage, LPVOID lpData, DWORD cbData);
+
+""")  # noqa
+
+
+def ENUMRESTYPEPROC(callback):
+    def wrapped(hModule, lpszType, lParam):
+        return callback(hModule, resource(lpszType), lParam)
+    return wrapped
+
+
+def ENUMRESNAMEPROC(callback):
+    def wrapped(hModule, lpszType, lpszName, lParam):
+        if lpszName == ffi.NULL:
+            return False
+        return callback(
+            hModule, resource(lpszType), resource(lpszName), lParam)
+    return wrapped
+
+
+def ENUMRESLANGPROC(callback):
+    def wrapped(hModule, lpszType, lpszName, wIDLanguage, lParam):
+        return callback(
+            hModule, resource(lpszType), resource(lpszName),
+            wIDLanguage, lParam)
+    return wrapped
+
+
+def _EnumResourceTypes(hModule, lpEnumFunc, lParam):
+    callback = ffi.callback('ENUMRESTYPEPROC', lpEnumFunc)
+    check_false(
+        dlls.kernel32.EnumResourceTypesW(PVOID(hModule), callback, lParam),
+        function_name='EnumResourceTypes')
+
+
+def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
+    callback = ffi.callback('ENUMRESNAMEPROC', lpEnumFunc)
+    check_false(
+        dlls.kernel32.EnumResourceNamesW(
+            PVOID(hModule), RESOURCE(lpszType), callback, lParam),
+        function_name='EnumResourceNames')
+
+
+def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
+    callback = ffi.callback('ENUMRESLANGPROC', lpEnumFunc)
+    check_false(
+        dlls.kernel32.EnumResourceLanguagesW(
+            PVOID(hModule), RESOURCE(lpType),
+            RESOURCE(lpName), callback, lParam),
+        function_name='EnumResourceLanguages')
+
+
+def _FindResourceEx(hModule, lpType, lpName, wLanguage):
+    return check_null(
+        dlls.kernel32.FindResourceExW(
+            PVOID(hModule), RESOURCE(lpType), RESOURCE(lpName), wLanguage),
+        function_name='FindResourceEx')
+
+
+def _SizeofResource(hModule, hResInfo):
+    return check_zero(
+        dlls.kernel32.SizeofResource(PVOID(hModule), hResInfo),
+        function_name='SizeofResource')
+
+
+def _LoadResource(hModule, hResInfo):
+    return check_null(
+        dlls.kernel32.LoadResource(PVOID(hModule), hResInfo),
+        function_name='LoadResource')
+
+
+def _LockResource(hResData):
+    return check_null(
+        dlls.kernel32.LockResource(hResData),
+        function_name='LockResource')
+
+
+def _BeginUpdateResource(pFileName, bDeleteExistingResources):
+    result = check_null(
+        dlls.kernel32.BeginUpdateResourceW(
+            str(pFileName), bDeleteExistingResources))
+    return HMODULE(result)
+
+
+def _EndUpdateResource(hUpdate, fDiscard):
+    check_false(
+        dlls.kernel32.EndUpdateResourceW(PVOID(hUpdate), fDiscard),
+        function_name='EndUpdateResource')
+
+
+def _UpdateResource(hUpdate, lpType, lpName, wLanguage, cData, cbData):
+    lpData = ffi.from_buffer(cData)
+    check_false(
+        dlls.kernel32.UpdateResourceW(
+            PVOID(hUpdate), RESOURCE(lpType), RESOURCE(lpName),
+            wLanguage, PVOID(lpData), cbData),
+        function_name='UpdateResource')
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_system_information.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_system_information.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#
-# (C) Copyright 2018 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-from ._util import ffi, dlls
-
-# TODO: retrieve this value using ffi
-MAX_PATH = 260
-MAX_PATH_BUF = u'wchar_t[{0}]'.format(MAX_PATH)
-
-ffi.cdef("""
-
-BOOL WINAPI Beep(DWORD dwFreq, DWORD dwDuration);
-UINT WINAPI GetWindowsDirectoryW(LPTSTR lpBuffer, UINT uSize);
-UINT WINAPI GetSystemDirectoryW(LPTSTR lpBuffer, UINT uSize);
-
-""")
-
-
-def _GetWindowsDirectory():
-    buffer = ffi.new(MAX_PATH_BUF)
-    directory = dlls.kernel32.GetWindowsDirectoryW(buffer, MAX_PATH)
-    return ffi.unpack(buffer, directory)
-
-
-def _GetSystemDirectory():
-    buffer = ffi.new(MAX_PATH_BUF)
-    directory = dlls.kernel32.GetSystemDirectoryW(buffer, MAX_PATH)
-    return ffi.unpack(buffer, directory)
+#
+# (C) Copyright 2018 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+from ._util import ffi, dlls
+
+# TODO: retrieve this value using ffi
+MAX_PATH = 260
+MAX_PATH_BUF = u'wchar_t[{0}]'.format(MAX_PATH)
+
+ffi.cdef("""
+
+BOOL WINAPI Beep(DWORD dwFreq, DWORD dwDuration);
+UINT WINAPI GetWindowsDirectoryW(LPTSTR lpBuffer, UINT uSize);
+UINT WINAPI GetSystemDirectoryW(LPTSTR lpBuffer, UINT uSize);
+
+""")
+
+
+def _GetWindowsDirectory():
+    buffer = ffi.new(MAX_PATH_BUF)
+    directory = dlls.kernel32.GetWindowsDirectoryW(buffer, MAX_PATH)
+    return ffi.unpack(buffer, directory)
+
+
+def _GetSystemDirectory():
+    buffer = ffi.new(MAX_PATH_BUF)
+    directory = dlls.kernel32.GetSystemDirectoryW(buffer, MAX_PATH)
+    return ffi.unpack(buffer, directory)
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/cffi/_util.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/cffi/_util.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#
-# (C) Copyright 2015 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-""" Utility functions to help with cffi wrapping.
-"""
-from win32ctypes.core.compat import is_bytes, is_integer
-from cffi import FFI
-
-ffi = FFI()
-ffi.set_unicode(True)
-
-
-def HMODULE(cdata):
-    return int(ffi.cast("intptr_t", cdata))
-
-
-def PVOID(x):
-    return ffi.cast("void *", x)
-
-
-def IS_INTRESOURCE(x):
-    """ Check if x is an index into the id list.
-
-    """
-    return int(ffi.cast("uintptr_t", x)) >> 16 == 0
-
-
-def RESOURCE(resource):
-    """ Convert a resource into a compatible input for cffi.
-
-    """
-    if is_integer(resource):
-        resource = ffi.cast('wchar_t *', resource)
-    elif is_bytes(resource):
-        resource = str(resource)
-    return resource
-
-
-def resource(lpRESOURCEID):
-    """ Convert the windows RESOURCE into a python friendly object.
-    """
-    if IS_INTRESOURCE(lpRESOURCEID):
-        resource = int(ffi.cast("uintptr_t", lpRESOURCEID))
-    else:
-        resource = ffi.string(lpRESOURCEID)
-    return resource
-
-
-class ErrorWhen(object):
-    """ Callable factory for raising errors when calling cffi functions.
-
-    """
-
-    def __init__(self, check, raise_on_zero=True):
-        """ Constructor
-
-        Parameters
-        ----------
-        check :
-            The return value that designates that an error has taken place.
-
-        raise_on_zero : bool
-            When set any error will be raised. When false the winerror
-            is checked and only non-zero win errors are raised. Currently
-            this parameters is used to workaround issues with the win32
-            implementation in ``wine``.
-
-        """
-        self._check = check
-        self._raise_on_zero = raise_on_zero
-
-    def __call__(self, value, function_name=''):
-        if value == self._check:
-            self._raise_error(function_name)
-        else:
-            return value
-
-    def _raise_error(self, function_name=''):
-        code, message = ffi.getwinerror()
-        exception = WindowsError()
-        exception.errno = ffi.errno
-        exception.winerror = code
-        exception.strerror = message
-        exception.function = function_name
-        raise exception
-
-
-check_null = ErrorWhen(ffi.NULL)
-check_zero = ErrorWhen(0)
-check_false = ErrorWhen(False)
-
-
-class Libraries(object):
-
-    def __getattr__(self, name):
-        library = ffi.dlopen('{}.dll'.format(name))
-        self.__dict__[name] = library
-        return library
-
-
-dlls = Libraries()
+#
+# (C) Copyright 2015 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+""" Utility functions to help with cffi wrapping.
+"""
+from win32ctypes.core.compat import is_bytes, is_integer
+from cffi import FFI
+
+ffi = FFI()
+ffi.set_unicode(True)
+
+
+def HMODULE(cdata):
+    return int(ffi.cast("intptr_t", cdata))
+
+
+def PVOID(x):
+    return ffi.cast("void *", x)
+
+
+def IS_INTRESOURCE(x):
+    """ Check if x is an index into the id list.
+
+    """
+    return int(ffi.cast("uintptr_t", x)) >> 16 == 0
+
+
+def RESOURCE(resource):
+    """ Convert a resource into a compatible input for cffi.
+
+    """
+    if is_integer(resource):
+        resource = ffi.cast('wchar_t *', resource)
+    elif is_bytes(resource):
+        resource = str(resource)
+    return resource
+
+
+def resource(lpRESOURCEID):
+    """ Convert the windows RESOURCE into a python friendly object.
+    """
+    if IS_INTRESOURCE(lpRESOURCEID):
+        resource = int(ffi.cast("uintptr_t", lpRESOURCEID))
+    else:
+        resource = ffi.string(lpRESOURCEID)
+    return resource
+
+
+class ErrorWhen(object):
+    """ Callable factory for raising errors when calling cffi functions.
+
+    """
+
+    def __init__(self, check, raise_on_zero=True):
+        """ Constructor
+
+        Parameters
+        ----------
+        check :
+            The return value that designates that an error has taken place.
+
+        raise_on_zero : bool
+            When set any error will be raised. When false the winerror
+            is checked and only non-zero win errors are raised. Currently
+            this parameters is used to workaround issues with the win32
+            implementation in ``wine``.
+
+        """
+        self._check = check
+        self._raise_on_zero = raise_on_zero
+
+    def __call__(self, value, function_name=''):
+        if value == self._check:
+            self._raise_error(function_name)
+        else:
+            return value
+
+    def _raise_error(self, function_name=''):
+        code, message = ffi.getwinerror()
+        exception = WindowsError()
+        exception.errno = ffi.errno
+        exception.winerror = code
+        exception.strerror = message
+        exception.function = function_name
+        raise exception
+
+
+check_null = ErrorWhen(ffi.NULL)
+check_zero = ErrorWhen(0)
+check_false = ErrorWhen(False)
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = ffi.dlopen('{}.dll'.format(name))
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_common.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_common.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import ctypes
-import sys
-from ctypes import (
-    pythonapi, POINTER, c_void_p, py_object, c_char_p, c_int, c_long, c_int64,
-    c_longlong)
-from ctypes import cast  # noqa imported here for convenience
-from ctypes.wintypes import BYTE
-
-from ._util import function_factory
-
-PPy_UNICODE = c_void_p
-LPBYTE = POINTER(BYTE)
-is_64bits = sys.maxsize > 2**32
-Py_ssize_t = c_int64 if is_64bits else c_int
-
-if ctypes.sizeof(c_long) == ctypes.sizeof(c_void_p):
-    LONG_PTR = c_long
-elif ctypes.sizeof(c_longlong) == ctypes.sizeof(c_void_p):
-    LONG_PTR = c_longlong
-
-_PyBytes_FromStringAndSize = function_factory(
-    pythonapi.PyBytes_FromStringAndSize,
-    [c_char_p, Py_ssize_t],
-    return_type=py_object)
-
-
-def IS_INTRESOURCE(x):
-    return x >> 16 == 0
-
-
-byreference = ctypes.byref
-
-
-def dereference(x):
-    return x.contents
-
-
-class Libraries(object):
-
-    def __getattr__(self, name):
-        library = ctypes.WinDLL(name)
-        self.__dict__[name] = library
-        return library
-
-
-dlls = Libraries()
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import ctypes
+import sys
+from ctypes import (
+    pythonapi, POINTER, c_void_p, py_object, c_char_p, c_int, c_long, c_int64,
+    c_longlong)
+from ctypes import cast  # noqa imported here for convenience
+from ctypes.wintypes import BYTE
+
+from ._util import function_factory
+
+PPy_UNICODE = c_void_p
+LPBYTE = POINTER(BYTE)
+is_64bits = sys.maxsize > 2**32
+Py_ssize_t = c_int64 if is_64bits else c_int
+
+if ctypes.sizeof(c_long) == ctypes.sizeof(c_void_p):
+    LONG_PTR = c_long
+elif ctypes.sizeof(c_longlong) == ctypes.sizeof(c_void_p):
+    LONG_PTR = c_longlong
+
+_PyBytes_FromStringAndSize = function_factory(
+    pythonapi.PyBytes_FromStringAndSize,
+    [c_char_p, Py_ssize_t],
+    return_type=py_object)
+
+
+def IS_INTRESOURCE(x):
+    return x >> 16 == 0
+
+
+byreference = ctypes.byref
+
+
+def dereference(x):
+    return x.contents
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = ctypes.WinDLL(name)
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_resource.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_resource.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-#
-# (C) Copyright 2018 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import ctypes
-from ctypes.wintypes import (
-    BOOL, DWORD, HANDLE, HMODULE, LPCWSTR, WORD, HRSRC,
-    HGLOBAL, LPVOID)
-
-from ._common import LONG_PTR, IS_INTRESOURCE
-from ._util import check_null, check_zero, check_false, function_factory, dlls
-
-_ENUMRESTYPEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LONG_PTR)
-_ENUMRESNAMEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LPVOID, LONG_PTR)
-_ENUMRESLANGPROC = ctypes.WINFUNCTYPE(
-    BOOL, HMODULE, LPVOID, LPVOID, WORD, LONG_PTR)
-
-
-def ENUMRESTYPEPROC(callback):
-    def wrapped(handle, type_, param):
-        if IS_INTRESOURCE(type_):
-            type_ = int(type_)
-        else:
-            type_ = ctypes.cast(type_, LPCWSTR).value
-        return callback(handle, type_, param)
-
-    return _ENUMRESTYPEPROC(wrapped)
-
-
-def ENUMRESNAMEPROC(callback):
-    def wrapped(handle, type_, name, param):
-        if IS_INTRESOURCE(type_):
-            type_ = int(type_)
-        else:
-            type_ = ctypes.cast(type_, LPCWSTR).value
-        if name is None:
-            return False
-        elif IS_INTRESOURCE(name):
-            name = int(name)
-        else:
-            name = ctypes.cast(name, LPCWSTR).value
-        return callback(handle, type_, name, param)
-
-    return _ENUMRESNAMEPROC(wrapped)
-
-
-def ENUMRESLANGPROC(callback):
-    def wrapped(handle, type_, name, language, param):
-        if IS_INTRESOURCE(type_):
-            type_ = int(type_)
-        else:
-            type_ = ctypes.cast(type_, LPCWSTR).value
-        if IS_INTRESOURCE(name):
-            name = int(name)
-        else:
-            name = ctypes.cast(name, LPCWSTR).value
-        return callback(handle, type_, name, language, param)
-
-    return _ENUMRESLANGPROC(wrapped)
-
-
-def _UpdateResource(hUpdate, lpType, lpName, wLanguage, lpData, cbData):
-    lp_type = LPCWSTR(lpType)
-    lp_name = LPCWSTR(lpName)
-    _BaseUpdateResource(hUpdate, lp_type, lp_name, wLanguage, lpData, cbData)
-
-
-def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
-    resource_type = LPCWSTR(lpszType)
-    _BaseEnumResourceNames(hModule, resource_type, lpEnumFunc, lParam)
-
-
-def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
-    resource_type = LPCWSTR(lpType)
-    resource_name = LPCWSTR(lpName)
-    _BaseEnumResourceLanguages(
-        hModule, resource_type, resource_name, lpEnumFunc, lParam)
-
-
-def _FindResourceEx(hModule, lpType, lpName, wLanguage):
-    resource_type = LPCWSTR(lpType)
-    resource_name = LPCWSTR(lpName)
-    return _BaseFindResourceEx(
-        hModule, resource_type, resource_name, wLanguage)
-
-
-_EnumResourceTypes = function_factory(
-    dlls.kernel32.EnumResourceTypesW,
-    [HMODULE, _ENUMRESTYPEPROC, LONG_PTR],
-    BOOL,
-    check_false)
-
-_LoadResource = function_factory(
-    dlls.kernel32.LoadResource,
-    [HMODULE, HRSRC],
-    HGLOBAL,
-    check_null)
-
-_LockResource = function_factory(
-    dlls.kernel32.LockResource,
-    [HGLOBAL],
-    LPVOID,
-    check_null)
-
-_SizeofResource = function_factory(
-    dlls.kernel32.SizeofResource,
-    [HMODULE, HRSRC],
-    DWORD,
-    check_zero)
-
-_BeginUpdateResource = function_factory(
-    dlls.kernel32.BeginUpdateResourceW,
-    [LPCWSTR, BOOL],
-    HANDLE,
-    check_null)
-
-_EndUpdateResource = function_factory(
-    dlls.kernel32.EndUpdateResourceW,
-    [HANDLE, BOOL],
-    BOOL,
-    check_false)
-
-_BaseEnumResourceNames = function_factory(
-    dlls.kernel32.EnumResourceNamesW,
-    [HMODULE, LPCWSTR, _ENUMRESNAMEPROC, LONG_PTR],
-    BOOL,
-    check_false)
-
-_BaseEnumResourceLanguages = function_factory(
-    dlls.kernel32.EnumResourceLanguagesW,
-    [HMODULE, LPCWSTR, LPCWSTR, _ENUMRESLANGPROC, LONG_PTR],
-    BOOL,
-    check_false)
-
-_BaseFindResourceEx = function_factory(
-    dlls.kernel32.FindResourceExW,
-    [HMODULE, LPCWSTR, LPCWSTR, WORD],
-    HRSRC,
-    check_null)
-
-_BaseUpdateResource = function_factory(
-    dlls.kernel32.UpdateResourceW,
-    [HANDLE, LPCWSTR, LPCWSTR, WORD, LPVOID, DWORD],
-    BOOL,
-    check_false)
+#
+# (C) Copyright 2018 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import ctypes
+from ctypes.wintypes import (
+    BOOL, DWORD, HANDLE, HMODULE, LPCWSTR, WORD, HRSRC,
+    HGLOBAL, LPVOID)
+
+from ._common import LONG_PTR, IS_INTRESOURCE
+from ._util import check_null, check_zero, check_false, function_factory, dlls
+
+_ENUMRESTYPEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LONG_PTR)
+_ENUMRESNAMEPROC = ctypes.WINFUNCTYPE(BOOL, HMODULE, LPVOID, LPVOID, LONG_PTR)
+_ENUMRESLANGPROC = ctypes.WINFUNCTYPE(
+    BOOL, HMODULE, LPVOID, LPVOID, WORD, LONG_PTR)
+
+
+def ENUMRESTYPEPROC(callback):
+    def wrapped(handle, type_, param):
+        if IS_INTRESOURCE(type_):
+            type_ = int(type_)
+        else:
+            type_ = ctypes.cast(type_, LPCWSTR).value
+        return callback(handle, type_, param)
+
+    return _ENUMRESTYPEPROC(wrapped)
+
+
+def ENUMRESNAMEPROC(callback):
+    def wrapped(handle, type_, name, param):
+        if IS_INTRESOURCE(type_):
+            type_ = int(type_)
+        else:
+            type_ = ctypes.cast(type_, LPCWSTR).value
+        if name is None:
+            return False
+        elif IS_INTRESOURCE(name):
+            name = int(name)
+        else:
+            name = ctypes.cast(name, LPCWSTR).value
+        return callback(handle, type_, name, param)
+
+    return _ENUMRESNAMEPROC(wrapped)
+
+
+def ENUMRESLANGPROC(callback):
+    def wrapped(handle, type_, name, language, param):
+        if IS_INTRESOURCE(type_):
+            type_ = int(type_)
+        else:
+            type_ = ctypes.cast(type_, LPCWSTR).value
+        if IS_INTRESOURCE(name):
+            name = int(name)
+        else:
+            name = ctypes.cast(name, LPCWSTR).value
+        return callback(handle, type_, name, language, param)
+
+    return _ENUMRESLANGPROC(wrapped)
+
+
+def _UpdateResource(hUpdate, lpType, lpName, wLanguage, lpData, cbData):
+    lp_type = LPCWSTR(lpType)
+    lp_name = LPCWSTR(lpName)
+    _BaseUpdateResource(hUpdate, lp_type, lp_name, wLanguage, lpData, cbData)
+
+
+def _EnumResourceNames(hModule, lpszType, lpEnumFunc, lParam):
+    resource_type = LPCWSTR(lpszType)
+    _BaseEnumResourceNames(hModule, resource_type, lpEnumFunc, lParam)
+
+
+def _EnumResourceLanguages(hModule, lpType, lpName, lpEnumFunc, lParam):
+    resource_type = LPCWSTR(lpType)
+    resource_name = LPCWSTR(lpName)
+    _BaseEnumResourceLanguages(
+        hModule, resource_type, resource_name, lpEnumFunc, lParam)
+
+
+def _FindResourceEx(hModule, lpType, lpName, wLanguage):
+    resource_type = LPCWSTR(lpType)
+    resource_name = LPCWSTR(lpName)
+    return _BaseFindResourceEx(
+        hModule, resource_type, resource_name, wLanguage)
+
+
+_EnumResourceTypes = function_factory(
+    dlls.kernel32.EnumResourceTypesW,
+    [HMODULE, _ENUMRESTYPEPROC, LONG_PTR],
+    BOOL,
+    check_false)
+
+_LoadResource = function_factory(
+    dlls.kernel32.LoadResource,
+    [HMODULE, HRSRC],
+    HGLOBAL,
+    check_null)
+
+_LockResource = function_factory(
+    dlls.kernel32.LockResource,
+    [HGLOBAL],
+    LPVOID,
+    check_null)
+
+_SizeofResource = function_factory(
+    dlls.kernel32.SizeofResource,
+    [HMODULE, HRSRC],
+    DWORD,
+    check_zero)
+
+_BeginUpdateResource = function_factory(
+    dlls.kernel32.BeginUpdateResourceW,
+    [LPCWSTR, BOOL],
+    HANDLE,
+    check_null)
+
+_EndUpdateResource = function_factory(
+    dlls.kernel32.EndUpdateResourceW,
+    [HANDLE, BOOL],
+    BOOL,
+    check_false)
+
+_BaseEnumResourceNames = function_factory(
+    dlls.kernel32.EnumResourceNamesW,
+    [HMODULE, LPCWSTR, _ENUMRESNAMEPROC, LONG_PTR],
+    BOOL,
+    check_false)
+
+_BaseEnumResourceLanguages = function_factory(
+    dlls.kernel32.EnumResourceLanguagesW,
+    [HMODULE, LPCWSTR, LPCWSTR, _ENUMRESLANGPROC, LONG_PTR],
+    BOOL,
+    check_false)
+
+_BaseFindResourceEx = function_factory(
+    dlls.kernel32.FindResourceExW,
+    [HMODULE, LPCWSTR, LPCWSTR, WORD],
+    HRSRC,
+    check_null)
+
+_BaseUpdateResource = function_factory(
+    dlls.kernel32.UpdateResourceW,
+    [HANDLE, LPCWSTR, LPCWSTR, WORD, LPVOID, DWORD],
+    BOOL,
+    check_false)
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/core/ctypes/_util.py` & `pywin32-ctypes-0.2.2/win32ctypes/core/ctypes/_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-""" Utility functions to help with ctypes wrapping.
-"""
-from ctypes import GetLastError, FormatError, WinDLL
-
-
-def function_factory(
-        function, argument_types=None,
-        return_type=None, error_checking=None):
-    if argument_types is not None:
-        function.argtypes = argument_types
-    function.restype = return_type
-    if error_checking is not None:
-        function.errcheck = error_checking
-    return function
-
-
-def make_error(function, function_name=None):
-    code = GetLastError()
-    description = FormatError(code).strip()
-    if function_name is None:
-        function_name = function.__name__
-    exception = WindowsError()
-    exception.winerror = code
-    exception.function = function_name
-    exception.strerror = description
-    return exception
-
-
-def check_null_factory(function_name=None):
-    def check_null(result, function, arguments, *args):
-        if result is None:
-            raise make_error(function, function_name)
-        return result
-    return check_null
-
-
-check_null = check_null_factory()
-
-
-def check_zero_factory(function_name=None):
-    def check_zero(result, function, arguments, *args):
-        if result == 0:
-            raise make_error(function, function_name)
-        return result
-    return check_zero
-
-
-check_zero = check_zero_factory()
-
-
-def check_false_factory(function_name=None):
-    def check_false(result, function, arguments, *args):
-        if not bool(result):
-            raise make_error(function, function_name)
-        else:
-            return True
-    return check_false
-
-
-check_false = check_false_factory()
-
-
-class Libraries(object):
-
-    def __getattr__(self, name):
-        library = WinDLL(name)
-        self.__dict__[name] = library
-        return library
-
-
-dlls = Libraries()
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+""" Utility functions to help with ctypes wrapping.
+"""
+from ctypes import get_last_error, FormatError, WinDLL
+
+
+def function_factory(
+        function, argument_types=None,
+        return_type=None, error_checking=None):
+    if argument_types is not None:
+        function.argtypes = argument_types
+    function.restype = return_type
+    if error_checking is not None:
+        function.errcheck = error_checking
+    return function
+
+
+def make_error(function, function_name=None):
+    code = get_last_error()
+    description = FormatError(code).strip()
+    if function_name is None:
+        function_name = function.__name__
+    exception = WindowsError()
+    exception.winerror = code
+    exception.function = function_name
+    exception.strerror = description
+    return exception
+
+
+def check_null_factory(function_name=None):
+    def check_null(result, function, arguments, *args):
+        if result is None:
+            raise make_error(function, function_name)
+        return result
+    return check_null
+
+
+check_null = check_null_factory()
+
+
+def check_zero_factory(function_name=None):
+    def check_zero(result, function, arguments, *args):
+        if result == 0:
+            raise make_error(function, function_name)
+        return result
+    return check_zero
+
+
+check_zero = check_zero_factory()
+
+
+def check_false_factory(function_name=None):
+    def check_false(result, function, arguments, *args):
+        if not bool(result):
+            raise make_error(function, function_name)
+        else:
+            return True
+    return check_false
+
+
+check_false = check_false_factory()
+
+
+class Libraries(object):
+
+    def __getattr__(self, name):
+        library = WinDLL(name, use_last_error=True)
+        self.__dict__[name] = library
+        return library
+
+
+dlls = Libraries()
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/pywin32/win32api.py` & `pywin32-ctypes-0.2.2/win32ctypes/pywin32/win32api.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-""" A module, encapsulating the Windows Win32 API. """
-from win32ctypes.core import (
-    _common, _dll, _resource, _system_information, _backend, _time)
-from win32ctypes.pywin32.pywintypes import pywin32error as _pywin32error
-
-LOAD_LIBRARY_AS_DATAFILE = 0x2
-LANG_NEUTRAL = 0x00
-
-
-def LoadLibraryEx(fileName, handle, flags):
-    """ Loads the specified DLL, and returns the handle.
-
-    Parameters
-    ----------
-    fileName : unicode
-        The filename of the module to load.
-
-    handle : int
-        Reserved, always zero.
-
-    flags : int
-        The action to be taken when loading the module.
-
-    Returns
-    -------
-    handle : hModule
-        The handle of the loaded module
-
-    """
-    if not handle == 0:
-        raise ValueError("handle != 0 not supported")
-    with _pywin32error():
-        return _dll._LoadLibraryEx(fileName, 0, flags)
-
-
-def EnumResourceTypes(hModule):
-    """ Enumerates resource types within a module.
-
-    Parameters
-    ----------
-    hModule : handle
-        The handle to the module.
-
-    Returns
-    -------
-    resource_types : list
-       The list of resource types in the module.
-
-    """
-    resource_types = []
-
-    def callback(hModule, type_, param):
-        resource_types.append(type_)
-        return True
-
-    with _pywin32error():
-        _resource._EnumResourceTypes(
-            hModule, _resource.ENUMRESTYPEPROC(callback), 0)
-    return resource_types
-
-
-def EnumResourceNames(hModule, resType):
-    """ Enumerates all the resources of the specified type within a module.
-
-    Parameters
-    ----------
-    hModule : handle
-        The handle to the module.
-    resType : str : int
-        The type or id of resource to enumerate.
-
-    Returns
-    -------
-    resource_names : list
-       The list of resource names (unicode strings) of the specific
-       resource type in the module.
-
-    """
-    resource_names = []
-
-    def callback(hModule, type_, type_name, param):
-        resource_names.append(type_name)
-        return True
-
-    with _pywin32error():
-        _resource._EnumResourceNames(
-            hModule, resType, _resource.ENUMRESNAMEPROC(callback), 0)
-    return resource_names
-
-
-def EnumResourceLanguages(hModule, lpType, lpName):
-    """ List languages of a resource module.
-
-    Parameters
-    ----------
-    hModule : handle
-        Handle to the resource module.
-
-    lpType : str : int
-        The type or id of resource to enumerate.
-
-    lpName : str : int
-        The type or id of resource to enumerate.
-
-    Returns
-    -------
-    resource_languages : list
-        List of the resource language ids.
-
-    """
-    resource_languages = []
-
-    def callback(hModule, type_name, res_name, language_id, param):
-        resource_languages.append(language_id)
-        return True
-
-    with _pywin32error():
-        _resource._EnumResourceLanguages(
-            hModule, lpType, lpName, _resource.ENUMRESLANGPROC(callback), 0)
-    return resource_languages
-
-
-def LoadResource(hModule, type, name, language=LANG_NEUTRAL):
-    """ Find and Load a resource component.
-
-    Parameters
-    ----------
-    handle : hModule
-        The handle of the module containing the resource.
-        Use None for current process executable.
-
-    type : str : int
-        The type of resource to load.
-
-    name : str : int
-        The name or Id of the resource to load.
-
-    language : int
-        Language to use, default is LANG_NEUTRAL.
-
-    Returns
-    -------
-    resource : bytes
-        The byte string blob of the resource
-
-    """
-    with _pywin32error():
-        hrsrc = _resource._FindResourceEx(hModule, type, name, language)
-        size = _resource._SizeofResource(hModule, hrsrc)
-        hglob = _resource._LoadResource(hModule, hrsrc)
-        if _backend == 'ctypes':
-            pointer = _common.cast(
-                _resource._LockResource(hglob), _common.c_char_p)
-        else:
-            pointer = _resource._LockResource(hglob)
-        return _common._PyBytes_FromStringAndSize(pointer, size)
-
-
-def FreeLibrary(hModule):
-    """ Free the loaded dynamic-link library (DLL) module.
-
-    If necessary, decrements its reference count.
-
-    Parameters
-    ----------
-    handle : hModule
-        The handle to the library as returned by the LoadLibrary function.
-
-    """
-    with _pywin32error():
-        return _dll._FreeLibrary(hModule)
-
-
-def GetTickCount():
-    """ The number of milliseconds that have elapsed since startup
-
-    Returns
-    -------
-    counts : int
-        The millisecond counts since system startup.
-    """
-    return _time._GetTickCount()
-
-
-def BeginUpdateResource(filename, delete):
-    """ Get a handle that can be used by the :func:`UpdateResource`.
-
-    Parameters
-    ----------
-    fileName : unicode
-        The filename of the module to load.
-    delete : bool
-        When true all existing resources are deleted
-
-    Returns
-    -------
-    result : hModule
-        Handle of the resource.
-
-    """
-    with _pywin32error():
-        return _resource._BeginUpdateResource(filename, delete)
-
-
-def EndUpdateResource(handle, discard):
-    """ End the update resource of the handle.
-
-    Parameters
-    ----------
-    handle : hModule
-        The handle of the resource as it is returned
-        by :func:`BeginUpdateResource`
-
-    discard : bool
-        When True all writes are discarded.
-
-    """
-    with _pywin32error():
-        _resource._EndUpdateResource(handle, discard)
-
-
-def UpdateResource(handle, type, name, data, language=LANG_NEUTRAL):
-    """ Update a resource.
-
-    Parameters
-    ----------
-    handle : hModule
-        The handle of the resource file as returned by
-        :func:`BeginUpdateResource`.
-
-    type : str : int
-        The type of resource to update.
-
-    name : str : int
-        The name or Id of the resource to update.
-
-    data : bytes
-        A bytes like object is expected.
-
-        .. note::
-          PyWin32 version 219, on Python 2.7, can handle unicode inputs.
-          However, the data are stored as bytes and it is not really
-          possible to convert the information back into the original
-          unicode string. To be consistent with the Python 3 behaviour
-          of PyWin32, we raise an error if the input cannot be
-          converted to `bytes`.
-
-    language : int
-        Language to use, default is LANG_NEUTRAL.
-
-    """
-    with _pywin32error():
-        try:
-            lp_data = bytes(data)
-        except UnicodeEncodeError:
-            raise TypeError(
-                "a bytes-like object is required, not a 'unicode'")
-        _resource._UpdateResource(
-            handle, type, name, language, lp_data, len(lp_data))
-
-
-def GetWindowsDirectory():
-    """ Get the ``Windows`` directory.
-
-    Returns
-    -------
-    result : str
-        The path to the ``Windows`` directory.
-
-    """
-    with _pywin32error():
-        # Note: pywin32 returns str on py27, unicode (which is str) on py3
-        return str(_system_information._GetWindowsDirectory())
-
-
-def GetSystemDirectory():
-    """ Get the ``System`` directory.
-
-    Returns
-    -------
-    result : str
-        The path to the ``System`` directory.
-
-    """
-    with _pywin32error():
-        # Note: pywin32 returns str on py27, unicode (which is str) on py3
-        return str(_system_information._GetSystemDirectory())
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+""" A module, encapsulating the Windows Win32 API. """
+from win32ctypes.core import (
+    _common, _dll, _resource, _system_information, _backend, _time)
+from win32ctypes.pywin32.pywintypes import pywin32error as _pywin32error
+
+LOAD_LIBRARY_AS_DATAFILE = 0x2
+LANG_NEUTRAL = 0x00
+
+
+def LoadLibraryEx(fileName, handle, flags):
+    """ Loads the specified DLL, and returns the handle.
+
+    Parameters
+    ----------
+    fileName : unicode
+        The filename of the module to load.
+
+    handle : int
+        Reserved, always zero.
+
+    flags : int
+        The action to be taken when loading the module.
+
+    Returns
+    -------
+    handle : hModule
+        The handle of the loaded module
+
+    """
+    if not handle == 0:
+        raise ValueError("handle != 0 not supported")
+    with _pywin32error():
+        return _dll._LoadLibraryEx(fileName, 0, flags)
+
+
+def EnumResourceTypes(hModule):
+    """ Enumerates resource types within a module.
+
+    Parameters
+    ----------
+    hModule : handle
+        The handle to the module.
+
+    Returns
+    -------
+    resource_types : list
+       The list of resource types in the module.
+
+    """
+    resource_types = []
+
+    def callback(hModule, type_, param):
+        resource_types.append(type_)
+        return True
+
+    with _pywin32error():
+        _resource._EnumResourceTypes(
+            hModule, _resource.ENUMRESTYPEPROC(callback), 0)
+    return resource_types
+
+
+def EnumResourceNames(hModule, resType):
+    """ Enumerates all the resources of the specified type within a module.
+
+    Parameters
+    ----------
+    hModule : handle
+        The handle to the module.
+    resType : str : int
+        The type or id of resource to enumerate.
+
+    Returns
+    -------
+    resource_names : list
+       The list of resource names (unicode strings) of the specific
+       resource type in the module.
+
+    """
+    resource_names = []
+
+    def callback(hModule, type_, type_name, param):
+        resource_names.append(type_name)
+        return True
+
+    with _pywin32error():
+        _resource._EnumResourceNames(
+            hModule, resType, _resource.ENUMRESNAMEPROC(callback), 0)
+    return resource_names
+
+
+def EnumResourceLanguages(hModule, lpType, lpName):
+    """ List languages of a resource module.
+
+    Parameters
+    ----------
+    hModule : handle
+        Handle to the resource module.
+
+    lpType : str : int
+        The type or id of resource to enumerate.
+
+    lpName : str : int
+        The type or id of resource to enumerate.
+
+    Returns
+    -------
+    resource_languages : list
+        List of the resource language ids.
+
+    """
+    resource_languages = []
+
+    def callback(hModule, type_name, res_name, language_id, param):
+        resource_languages.append(language_id)
+        return True
+
+    with _pywin32error():
+        _resource._EnumResourceLanguages(
+            hModule, lpType, lpName, _resource.ENUMRESLANGPROC(callback), 0)
+    return resource_languages
+
+
+def LoadResource(hModule, type, name, language=LANG_NEUTRAL):
+    """ Find and Load a resource component.
+
+    Parameters
+    ----------
+    handle : hModule
+        The handle of the module containing the resource.
+        Use None for current process executable.
+
+    type : str : int
+        The type of resource to load.
+
+    name : str : int
+        The name or Id of the resource to load.
+
+    language : int
+        Language to use, default is LANG_NEUTRAL.
+
+    Returns
+    -------
+    resource : bytes
+        The byte string blob of the resource
+
+    """
+    with _pywin32error():
+        hrsrc = _resource._FindResourceEx(hModule, type, name, language)
+        size = _resource._SizeofResource(hModule, hrsrc)
+        hglob = _resource._LoadResource(hModule, hrsrc)
+        if _backend == 'ctypes':
+            pointer = _common.cast(
+                _resource._LockResource(hglob), _common.c_char_p)
+        else:
+            pointer = _resource._LockResource(hglob)
+        return _common._PyBytes_FromStringAndSize(pointer, size)
+
+
+def FreeLibrary(hModule):
+    """ Free the loaded dynamic-link library (DLL) module.
+
+    If necessary, decrements its reference count.
+
+    Parameters
+    ----------
+    handle : hModule
+        The handle to the library as returned by the LoadLibrary function.
+
+    """
+    with _pywin32error():
+        return _dll._FreeLibrary(hModule)
+
+
+def GetTickCount():
+    """ The number of milliseconds that have elapsed since startup
+
+    Returns
+    -------
+    counts : int
+        The millisecond counts since system startup.
+    """
+    return _time._GetTickCount()
+
+
+def BeginUpdateResource(filename, delete):
+    """ Get a handle that can be used by the :func:`UpdateResource`.
+
+    Parameters
+    ----------
+    fileName : unicode
+        The filename of the module to load.
+    delete : bool
+        When true all existing resources are deleted
+
+    Returns
+    -------
+    result : hModule
+        Handle of the resource.
+
+    """
+    with _pywin32error():
+        return _resource._BeginUpdateResource(filename, delete)
+
+
+def EndUpdateResource(handle, discard):
+    """ End the update resource of the handle.
+
+    Parameters
+    ----------
+    handle : hModule
+        The handle of the resource as it is returned
+        by :func:`BeginUpdateResource`
+
+    discard : bool
+        When True all writes are discarded.
+
+    """
+    with _pywin32error():
+        _resource._EndUpdateResource(handle, discard)
+
+
+def UpdateResource(handle, type, name, data, language=LANG_NEUTRAL):
+    """ Update a resource.
+
+    Parameters
+    ----------
+    handle : hModule
+        The handle of the resource file as returned by
+        :func:`BeginUpdateResource`.
+
+    type : str : int
+        The type of resource to update.
+
+    name : str : int
+        The name or Id of the resource to update.
+
+    data : bytes
+        A bytes like object is expected.
+
+        .. note::
+          PyWin32 version 219, on Python 2.7, can handle unicode inputs.
+          However, the data are stored as bytes and it is not really
+          possible to convert the information back into the original
+          unicode string. To be consistent with the Python 3 behaviour
+          of PyWin32, we raise an error if the input cannot be
+          converted to `bytes`.
+
+    language : int
+        Language to use, default is LANG_NEUTRAL.
+
+    """
+    with _pywin32error():
+        try:
+            lp_data = bytes(data)
+        except UnicodeEncodeError:
+            raise TypeError(
+                "a bytes-like object is required, not a 'unicode'")
+        _resource._UpdateResource(
+            handle, type, name, language, lp_data, len(lp_data))
+
+
+def GetWindowsDirectory():
+    """ Get the ``Windows`` directory.
+
+    Returns
+    -------
+    result : str
+        The path to the ``Windows`` directory.
+
+    """
+    with _pywin32error():
+        # Note: pywin32 returns str on py27, unicode (which is str) on py3
+        return str(_system_information._GetWindowsDirectory())
+
+
+def GetSystemDirectory():
+    """ Get the ``System`` directory.
+
+    Returns
+    -------
+    result : str
+        The path to the ``System`` directory.
+
+    """
+    with _pywin32error():
+        # Note: pywin32 returns str on py27, unicode (which is str) on py3
+        return str(_system_information._GetSystemDirectory())
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/pywin32/win32cred.py` & `pywin32-ctypes-0.2.2/win32ctypes/pywin32/win32cred.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-""" Interface to credentials management functions. """
-from win32ctypes.core import _authentication, _common, _backend
-from win32ctypes.pywin32.pywintypes import pywin32error as _pywin32error
-
-CRED_TYPE_GENERIC = 0x1
-CRED_PERSIST_SESSION = 0x1
-CRED_PERSIST_LOCAL_MACHINE = 0x2
-CRED_PERSIST_ENTERPRISE = 0x3
-CRED_PRESERVE_CREDENTIAL_BLOB = 0
-CRED_ENUMERATE_ALL_CREDENTIALS = 0x1
-
-
-def CredWrite(Credential, Flags=CRED_PRESERVE_CREDENTIAL_BLOB):
-    """ Creates or updates a stored credential.
-
-    Parameters
-    ----------
-    Credential : dict
-        A dictionary corresponding to the PyWin32 ``PyCREDENTIAL``
-        structure.
-    Flags : int
-        Always pass ``CRED_PRESERVE_CREDENTIAL_BLOB`` (i.e. 0).
-
-    """
-    c_creds = _authentication.CREDENTIAL.fromdict(Credential, Flags)
-    c_pcreds = _authentication.PCREDENTIAL(c_creds)
-    with _pywin32error():
-        _authentication._CredWrite(c_pcreds, 0)
-
-
-def CredRead(TargetName, Type, Flags=0):
-    """ Retrieves a stored credential.
-
-    Parameters
-    ----------
-    TargetName : unicode
-        The target name to fetch from the keyring.
-    Type : int
-        One of the CRED_TYPE_* constants.
-    Flags : int
-        Reserved, always use 0.
-
-    Returns
-    -------
-    credentials : dict
-        ``None`` if the target name was not found or A dictionary
-        corresponding to the PyWin32 ``PyCREDENTIAL`` structure.
-
-    """
-    if Type != CRED_TYPE_GENERIC:
-        raise ValueError("Type != CRED_TYPE_GENERIC not yet supported")
-
-    flag = 0
-    with _pywin32error():
-        if _backend == 'cffi':
-            ppcreds = _authentication.PPCREDENTIAL()
-            _authentication._CredRead(TargetName, Type, flag, ppcreds)
-            pcreds = _common.dereference(ppcreds)
-        else:
-            pcreds = _authentication.PCREDENTIAL()
-            _authentication._CredRead(
-                TargetName, Type, flag, _common.byreference(pcreds))
-    try:
-        return _authentication.credential2dict(_common.dereference(pcreds))
-    finally:
-        _authentication._CredFree(pcreds)
-
-
-def CredDelete(TargetName, Type, Flags=0):
-    """ Remove the given target name from the stored credentials.
-
-    Parameters
-    ----------
-    TargetName : unicode
-        The target name to fetch from the keyring.
-    Type : int
-        One of the CRED_TYPE_* constants.
-    Flags : int
-        Reserved, always use 0.
-
-    """
-    if not Type == CRED_TYPE_GENERIC:
-        raise ValueError("Type != CRED_TYPE_GENERIC not yet supported.")
-    with _pywin32error():
-        _authentication._CredDelete(TargetName, Type, 0)
-
-
-def CredEnumerate(Filter=None, Flags=0):
-    """ Remove the given target name from the stored credentials.
-
-    Parameters
-    ----------
-    Filter : unicode
-        Matches credentials' target names by prefix, can be None.
-    Flags : int
-        When set to CRED_ENUMERATE_ALL_CREDENTIALS enumerates all of
-        the credentials in the user's credential set but in that
-        case the Filter parameter should be NULL, an error is
-        raised otherwise
-
-    Returns
-    -------
-    credentials : list
-        Returns a sequence of CREDENTIAL dictionaries.
-
-    """
-    with _pywin32error():
-        if _backend == 'cffi':
-            pcount = _common.PDWORD()
-            pppcredential = _authentication.PPPCREDENTIAL()
-            _authentication._CredEnumerate(
-                Filter, Flags, pcount, pppcredential)
-            count = pcount[0]
-            data = _common.dereference(
-                _common.ffi.cast(f"PCREDENTIAL*[{count}]", pppcredential))
-            memory = _common.dereference(pppcredential)
-        else:
-            import ctypes
-            count = _authentication.DWORD()
-            pcredential = _authentication.PCREDENTIAL()
-            ppcredential = ctypes.pointer(pcredential)
-            pppcredential = ctypes.pointer(ppcredential)
-            _authentication._CredEnumerate(
-                Filter, Flags, _common.byreference(count), pppcredential)
-            count = count.value
-            data = _common.dereference(
-                _common.cast(
-                    ppcredential,
-                    _common.POINTER(_authentication.PCREDENTIAL*count)))
-            memory = pcredential
-    try:
-        result = []
-        for i in range(count):
-            credential = _common.dereference(data[i])
-            result.append(_authentication.credential2dict(credential))
-        return result
-    finally:
-        _authentication._CredFree(memory)
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+""" Interface to credentials management functions. """
+from win32ctypes.core import _authentication, _common, _backend
+from win32ctypes.pywin32.pywintypes import pywin32error as _pywin32error
+
+CRED_TYPE_GENERIC = 0x1
+CRED_PERSIST_SESSION = 0x1
+CRED_PERSIST_LOCAL_MACHINE = 0x2
+CRED_PERSIST_ENTERPRISE = 0x3
+CRED_PRESERVE_CREDENTIAL_BLOB = 0
+CRED_ENUMERATE_ALL_CREDENTIALS = 0x1
+
+
+def CredWrite(Credential, Flags=CRED_PRESERVE_CREDENTIAL_BLOB):
+    """ Creates or updates a stored credential.
+
+    Parameters
+    ----------
+    Credential : dict
+        A dictionary corresponding to the PyWin32 ``PyCREDENTIAL``
+        structure.
+    Flags : int
+        Always pass ``CRED_PRESERVE_CREDENTIAL_BLOB`` (i.e. 0).
+
+    """
+    c_creds = _authentication.CREDENTIAL.fromdict(Credential, Flags)
+    c_pcreds = _authentication.PCREDENTIAL(c_creds)
+    with _pywin32error():
+        _authentication._CredWrite(c_pcreds, 0)
+
+
+def CredRead(TargetName, Type, Flags=0):
+    """ Retrieves a stored credential.
+
+    Parameters
+    ----------
+    TargetName : unicode
+        The target name to fetch from the keyring.
+    Type : int
+        One of the CRED_TYPE_* constants.
+    Flags : int
+        Reserved, always use 0.
+
+    Returns
+    -------
+    credentials : dict
+        ``None`` if the target name was not found or A dictionary
+        corresponding to the PyWin32 ``PyCREDENTIAL`` structure.
+
+    """
+    if Type != CRED_TYPE_GENERIC:
+        raise ValueError("Type != CRED_TYPE_GENERIC not yet supported")
+
+    flag = 0
+    with _pywin32error():
+        if _backend == 'cffi':
+            ppcreds = _authentication.PPCREDENTIAL()
+            _authentication._CredRead(TargetName, Type, flag, ppcreds)
+            pcreds = _common.dereference(ppcreds)
+        else:
+            pcreds = _authentication.PCREDENTIAL()
+            _authentication._CredRead(
+                TargetName, Type, flag, _common.byreference(pcreds))
+    try:
+        return _authentication.credential2dict(_common.dereference(pcreds))
+    finally:
+        _authentication._CredFree(pcreds)
+
+
+def CredDelete(TargetName, Type, Flags=0):
+    """ Remove the given target name from the stored credentials.
+
+    Parameters
+    ----------
+    TargetName : unicode
+        The target name to fetch from the keyring.
+    Type : int
+        One of the CRED_TYPE_* constants.
+    Flags : int
+        Reserved, always use 0.
+
+    """
+    if not Type == CRED_TYPE_GENERIC:
+        raise ValueError("Type != CRED_TYPE_GENERIC not yet supported.")
+    with _pywin32error():
+        _authentication._CredDelete(TargetName, Type, 0)
+
+
+def CredEnumerate(Filter=None, Flags=0):
+    """ Remove the given target name from the stored credentials.
+
+    Parameters
+    ----------
+    Filter : unicode
+        Matches credentials' target names by prefix, can be None.
+    Flags : int
+        When set to CRED_ENUMERATE_ALL_CREDENTIALS enumerates all of
+        the credentials in the user's credential set but in that
+        case the Filter parameter should be NULL, an error is
+        raised otherwise
+
+    Returns
+    -------
+    credentials : list
+        Returns a sequence of CREDENTIAL dictionaries.
+
+    """
+    with _pywin32error():
+        if _backend == 'cffi':
+            pcount = _common.PDWORD()
+            pppcredential = _authentication.PPPCREDENTIAL()
+            _authentication._CredEnumerate(
+                Filter, Flags, pcount, pppcredential)
+            count = pcount[0]
+            data = _common.dereference(
+                _common.ffi.cast(f"PCREDENTIAL*[{count}]", pppcredential))
+            memory = _common.dereference(pppcredential)
+        else:
+            import ctypes
+            count = _authentication.DWORD()
+            pcredential = _authentication.PCREDENTIAL()
+            ppcredential = ctypes.pointer(pcredential)
+            pppcredential = ctypes.pointer(ppcredential)
+            _authentication._CredEnumerate(
+                Filter, Flags, _common.byreference(count), pppcredential)
+            count = count.value
+            data = _common.dereference(
+                _common.cast(
+                    ppcredential,
+                    _common.POINTER(_authentication.PCREDENTIAL*count)))
+            memory = pcredential
+    try:
+        result = []
+        for i in range(count):
+            credential = _common.dereference(data[i])
+            result.append(_authentication.credential2dict(credential))
+        return result
+    finally:
+        _authentication._CredFree(memory)
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/tests/__init__.py` & `pywin32-ctypes-0.2.2/win32ctypes/tests/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import os
-
-if 'SHOW_TEST_ENV' in os.environ:
-    import sys
-    from win32ctypes.core import _backend
-    is_64bits = sys.maxsize > 2**32
-    print('=' * 30, file=sys.stderr)
-    print(
-        'Running on python: {} {}'.format(
-            sys.version, '64bit' if is_64bits else '32bit'),
-        file=sys.stderr)
-    print('The executable is: {}'.format(sys.executable), file=sys.stderr)
-    print('Using the {} backend'.format(_backend), file=sys.stderr)
-    print('=' * 30, file=sys.stderr, flush=True)
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import os
+
+if 'SHOW_TEST_ENV' in os.environ:
+    import sys
+    from win32ctypes.core import _backend
+    is_64bits = sys.maxsize > 2**32
+    print('=' * 30, file=sys.stderr)
+    print(
+        'Running on python: {} {}'.format(
+            sys.version, '64bit' if is_64bits else '32bit'),
+        file=sys.stderr)
+    print('The executable is: {}'.format(sys.executable), file=sys.stderr)
+    print('Using the {} backend'.format(_backend), file=sys.stderr)
+    print('=' * 30, file=sys.stderr, flush=True)
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/tests/test_backends.py` & `pywin32-ctypes-0.2.2/win32ctypes/tests/test_backends.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#
-# (C) Copyright 2023 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import importlib
-import unittest
-
-from win32ctypes.core import _backend
-
-_modules = [
-    '_dll', '_authentication', '_time', '_common',
-    '_resource',  '_nl_support', '_system_information']
-
-
-class TestBackends(unittest.TestCase):
-
-    @unittest.skipIf(_backend != 'cffi', 'cffi backend not enabled')
-    def test_backend_cffi_load(self):
-        # when/then
-        for name in _modules:
-            module = importlib.import_module(f'win32ctypes.core.{name}')
-            self.assertTrue(module.__file__.endswith(f'cffi\\{name}.py'))
-
-    @unittest.skipIf(_backend != 'ctypes', 'ctypes backend not enabled')
-    def test_backend_ctypes_load(self):
-        # when/then
-        for name in _modules:
-            module = importlib.import_module(f'win32ctypes.core.{name}')
-            self.assertTrue(module.__file__.endswith(f'ctypes\\{name}.py'))
+#
+# (C) Copyright 2023 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import importlib
+import unittest
+
+from win32ctypes.core import _backend
+
+_modules = [
+    '_dll', '_authentication', '_time', '_common',
+    '_resource',  '_nl_support', '_system_information']
+
+
+class TestBackends(unittest.TestCase):
+
+    @unittest.skipIf(_backend != 'cffi', 'cffi backend not enabled')
+    def test_backend_cffi_load(self):
+        # when/then
+        for name in _modules:
+            module = importlib.import_module(f'win32ctypes.core.{name}')
+            self.assertTrue(module.__file__.endswith(f'cffi\\{name}.py'))
+
+    @unittest.skipIf(_backend != 'ctypes', 'ctypes backend not enabled')
+    def test_backend_ctypes_load(self):
+        # when/then
+        for name in _modules:
+            module = importlib.import_module(f'win32ctypes.core.{name}')
+            self.assertTrue(module.__file__.endswith(f'ctypes\\{name}.py'))
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/tests/test_win32api.py` & `pywin32-ctypes-0.2.2/win32ctypes/tests/test_win32api.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import os
-import sys
-import unittest
-import contextlib
-import tempfile
-import shutil
-import faulthandler
-
-import win32api
-
-
-from win32ctypes import pywin32
-from win32ctypes.pywin32.pywintypes import error
-
-
-skip_on_wine = 'SKIP_WINE_KNOWN_FAILURES' in os.environ
-
-
-class TestWin32API(unittest.TestCase):
-
-    # the pywin32ctypes implementation
-    module = pywin32.win32api
-
-    def setUp(self):
-        self.tempdir = tempfile.mkdtemp()
-        shutil.copy(sys.executable, self.tempdir)
-
-    def tearDown(self):
-        shutil.rmtree(self.tempdir)
-
-    @contextlib.contextmanager
-    def load_library(self, module, library=sys.executable, flags=0x2):
-        handle = module.LoadLibraryEx(library, 0, flags)
-        try:
-            yield handle
-        finally:
-            module.FreeLibrary(handle)
-
-    @contextlib.contextmanager
-    def resource_update(self, module, library=sys.executable):
-        handle = module.BeginUpdateResource(library, False)
-        try:
-            yield handle
-        finally:
-            module.EndUpdateResource(handle, False)
-
-    @contextlib.contextmanager
-    def nofaulthandler(self):
-        """ Disable the faulthander
-
-            Use this function to avoid poluting the output with errors
-            When it is known that an access violation is expected.
-
-        """
-        enabled = faulthandler.is_enabled()
-        faulthandler.disable()
-        try:
-            yield
-        finally:
-            if enabled:
-                faulthandler.enable()
-
-    def test_load_library_ex(self):
-        with self.load_library(win32api) as expected:
-            with self.load_library(self.module) as handle:
-                self.assertEqual(handle, expected)
-
-        with self.assertRaises(error):
-            self.module.LoadLibraryEx(u'ttt.dll', 0, 0x2)
-
-    def test_free_library(self):
-        with self.load_library(win32api) as handle:
-            self.assertTrue(win32api.FreeLibrary(handle) is None)
-            self.assertNotEqual(self.module.FreeLibrary(handle), 0)
-
-        with self.assertRaises(error):
-            with self.nofaulthandler():
-                self.module.FreeLibrary(-3)
-
-    def test_enum_resource_types(self):
-        with self.load_library(win32api, u'shell32.dll') as handle:
-            expected = win32api.EnumResourceTypes(handle)
-
-        with self.load_library(pywin32.win32api, u'shell32.dll') as handle:
-            resource_types = self.module.EnumResourceTypes(handle)
-
-        self.assertEqual(resource_types, expected)
-
-        with self.assertRaises(error):
-            with self.nofaulthandler():
-                self.module.EnumResourceTypes(-3)
-
-    def test_enum_resource_names(self):
-        with self.load_library(win32api, u'shell32.dll') as handle:
-            resource_types = win32api.EnumResourceTypes(handle)
-            for resource_type in resource_types:
-                expected = win32api.EnumResourceNames(handle, resource_type)
-                resource_names = self.module.EnumResourceNames(
-                    handle, resource_type)
-                self.assertEqual(resource_names, expected)
-                # check that the #<index> format works
-                resource_names = self.module.EnumResourceNames(
-                    handle, self._id2str(resource_type))
-                self.assertEqual(resource_names, expected)
-
-        with self.assertRaises(error):
-            self.module.EnumResourceNames(2, 3)
-
-    def test_enum_resource_languages(self):
-        with self.load_library(win32api, u'shell32.dll') as handle:
-            resource_types = win32api.EnumResourceTypes(handle)
-            for resource_type in resource_types:
-                resource_names = win32api.EnumResourceNames(
-                    handle, resource_type)
-                for resource_name in resource_names:
-                    expected = win32api.EnumResourceLanguages(
-                        handle, resource_type, resource_name)
-                    resource_languages = self.module.EnumResourceLanguages(
-                        handle, resource_type, resource_name)
-                    self.assertEqual(resource_languages, expected)
-                    # check that the #<index> format works
-                    resource_languages = self.module.EnumResourceLanguages(
-                        handle, self._id2str(resource_type),
-                        self._id2str(resource_name))
-                    self.assertEqual(resource_languages, expected)
-
-        with self.assertRaises(error):
-            self.module.EnumResourceLanguages(handle, resource_type, 2235)
-
-    def test_load_resource(self):
-        with self.load_library(win32api, u'explorer.exe') as handle:
-            resource_types = win32api.EnumResourceTypes(handle)
-            for resource_type in resource_types:
-                resource_names = win32api.EnumResourceNames(
-                    handle, resource_type)
-                for resource_name in resource_names:
-                    resource_languages = win32api.EnumResourceLanguages(
-                        handle, resource_type, resource_name)
-                    for resource_language in resource_languages:
-                        expected = win32api.LoadResource(
-                            handle, resource_type, resource_name,
-                            resource_language)
-                        resource = self.module.LoadResource(
-                            handle, resource_type, resource_name,
-                            resource_language)
-                        # check that the #<index> format works
-                        resource = self.module.LoadResource(
-                            handle, self._id2str(resource_type),
-                            self._id2str(resource_name),
-                            resource_language)
-                        self.assertEqual(resource, expected)
-
-        with self.assertRaises(error):
-            with self.nofaulthandler():
-                self.module.LoadResource(
-                    handle, resource_type, resource_name, 12435)
-
-    def test_get_tick_count(self):
-        self.assertGreater(self.module.GetTickCount(), 0.0)
-
-    def test_begin_and_end_update_resource(self):
-        # given
-        module = self.module
-        filename = os.path.join(self.tempdir, 'python.exe')
-        with self.load_library(module, filename) as handle:
-            count = len(module.EnumResourceTypes(handle))
-
-        # when
-        handle = module.BeginUpdateResource(filename, False)
-        module.EndUpdateResource(handle, False)
-
-        # then
-        with self.load_library(module, filename) as handle:
-            self.assertEqual(len(module.EnumResourceTypes(handle)), count)
-
-        # when
-        handle = module.BeginUpdateResource(filename, True)
-        module.EndUpdateResource(handle, True)
-
-        # then
-        with self.load_library(module, filename) as handle:
-            self.assertEqual(len(module.EnumResourceTypes(handle)), count)
-
-    def test_begin_removing_all_resources(self):
-        if skip_on_wine:
-            self.skipTest('EnumResourceTypes known failure on wine, see #59')
-
-        # given
-        module = self.module
-        filename = os.path.join(self.tempdir, 'python.exe')
-
-        # when
-        handle = module.BeginUpdateResource(filename, True)
-        module.EndUpdateResource(handle, False)
-
-        # then
-        with self.load_library(module, filename) as handle:
-            self.assertEqual(len(module.EnumResourceTypes(handle)), 0)
-
-    def test_begin_update_resource_with_invalid(self):
-        if skip_on_wine:
-            self.skipTest('BeginUpdateResource known failure on wine, see #59')
-
-            # when/then
-        with self.assertRaises(error) as context:
-            self.module.BeginUpdateResource('invalid', False)
-        # the errno cannot be 0 (i.e. success)
-        self.assertNotEqual(context.exception.winerror, 0)
-
-    def test_end_update_resource_with_invalid(self):
-        if skip_on_wine:
-            self.skipTest('EndUpdateResource known failure on wine, see #59')
-
-        # when/then
-        with self.assertRaises(error) as context:
-            self.module.EndUpdateResource(-3, False)
-        # the errno cannot be 0 (i.e. success)
-        self.assertNotEqual(context.exception.winerror, 0)
-
-    def test_update_resource(self):
-        # given
-        module = self.module
-        filename = os.path.join(self.tempdir, 'python.exe')
-        with self.load_library(self.module, filename) as handle:
-            resource_type = module.EnumResourceTypes(handle)[-1]
-            resource_name = module.EnumResourceNames(handle, resource_type)[-1]
-            resource_language = module.EnumResourceLanguages(
-                handle, resource_type, resource_name)[-1]
-            resource = module.LoadResource(
-                handle, resource_type, resource_name, resource_language)
-
-        # when
-        with self.resource_update(self.module, filename) as handle:
-            module.UpdateResource(
-                handle, resource_type, resource_name, resource[:-2],
-                resource_language)
-
-        # then
-        with self.load_library(self.module, filename) as handle:
-            updated = module.LoadResource(
-                handle, resource_type, resource_name, resource_language)
-        self.assertEqual(len(updated), len(resource) - 2)
-        self.assertEqual(updated, resource[:-2])
-
-    def test_update_resource_with_unicode(self):
-        # given
-        module = self.module
-        filename = os.path.join(self.tempdir, 'python.exe')
-        with self.load_library(module, filename) as handle:
-            resource_type = module.EnumResourceTypes(handle)[-1]
-            resource_name = module.EnumResourceNames(handle, resource_type)[-1]
-            resource_language = module.EnumResourceLanguages(
-                handle, resource_type, resource_name)[-1]
-        resource = u"\N{GREEK CAPITAL LETTER DELTA}"
-
-        # when
-        with self.resource_update(module, filename) as handle:
-            with self.assertRaises(TypeError):
-                module.UpdateResource(
-                    handle, resource_type, resource_name, resource,
-                    resource_language)
-
-    def test_get_windows_directory(self):
-        # given
-        expected = win32api.GetWindowsDirectory()
-
-        # when
-        result = self.module.GetWindowsDirectory()
-
-        # then
-        # note: pywin32 returns str on py27, unicode (which is str) on py3
-        self.assertIsInstance(result, str)
-        self.assertEqual(result.lower(), r"c:\windows")
-        self.assertEqual(result, expected)
-
-    def test_get_system_directory(self):
-        # given
-        expected = win32api.GetSystemDirectory()
-
-        # when
-        result = self.module.GetSystemDirectory()
-
-        # then
-        # note: pywin32 returns str on py27, unicode (which is str) on py3
-        self.assertIsInstance(result, str)
-        self.assertEqual(result.lower(), r"c:\windows\system32")
-        self.assertEqual(result, expected)
-
-    def _id2str(self, type_id):
-        if hasattr(type_id, 'index'):
-            return type_id
-        else:
-            return u'#{0}'.format(type_id)
-
-
-if __name__ == '__main__':
-    unittest.main()
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import os
+import sys
+import unittest
+import contextlib
+import tempfile
+import shutil
+import faulthandler
+
+import win32api
+
+
+from win32ctypes import pywin32
+from win32ctypes.pywin32.pywintypes import error
+
+
+skip_on_wine = 'SKIP_WINE_KNOWN_FAILURES' in os.environ
+
+
+class TestWin32API(unittest.TestCase):
+
+    # the pywin32ctypes implementation
+    module = pywin32.win32api
+
+    def setUp(self):
+        self.tempdir = tempfile.mkdtemp()
+        shutil.copy(sys.executable, self.tempdir)
+
+    def tearDown(self):
+        shutil.rmtree(self.tempdir)
+
+    @contextlib.contextmanager
+    def load_library(self, module, library=sys.executable, flags=0x2):
+        handle = module.LoadLibraryEx(library, 0, flags)
+        try:
+            yield handle
+        finally:
+            module.FreeLibrary(handle)
+
+    @contextlib.contextmanager
+    def resource_update(self, module, library=sys.executable):
+        handle = module.BeginUpdateResource(library, False)
+        try:
+            yield handle
+        finally:
+            module.EndUpdateResource(handle, False)
+
+    @contextlib.contextmanager
+    def nofaulthandler(self):
+        """ Disable the faulthander
+
+            Use this function to avoid poluting the output with errors
+            When it is known that an access violation is expected.
+
+        """
+        enabled = faulthandler.is_enabled()
+        faulthandler.disable()
+        try:
+            yield
+        finally:
+            if enabled:
+                faulthandler.enable()
+
+    def test_load_library_ex(self):
+        with self.load_library(win32api) as expected:
+            with self.load_library(self.module) as handle:
+                self.assertEqual(handle, expected)
+
+        with self.assertRaises(error):
+            self.module.LoadLibraryEx(u'ttt.dll', 0, 0x2)
+
+    def test_free_library(self):
+        with self.load_library(win32api) as handle:
+            self.assertTrue(win32api.FreeLibrary(handle) is None)
+            self.assertNotEqual(self.module.FreeLibrary(handle), 0)
+
+        with self.assertRaises(error):
+            with self.nofaulthandler():
+                self.module.FreeLibrary(-3)
+
+    def test_enum_resource_types(self):
+        with self.load_library(win32api, u'shell32.dll') as handle:
+            expected = win32api.EnumResourceTypes(handle)
+
+        with self.load_library(pywin32.win32api, u'shell32.dll') as handle:
+            resource_types = self.module.EnumResourceTypes(handle)
+
+        self.assertEqual(resource_types, expected)
+
+        with self.assertRaises(error):
+            with self.nofaulthandler():
+                self.module.EnumResourceTypes(-3)
+
+    def test_enum_resource_names(self):
+        with self.load_library(win32api, u'shell32.dll') as handle:
+            resource_types = win32api.EnumResourceTypes(handle)
+            for resource_type in resource_types:
+                expected = win32api.EnumResourceNames(handle, resource_type)
+                resource_names = self.module.EnumResourceNames(
+                    handle, resource_type)
+                self.assertEqual(resource_names, expected)
+                # check that the #<index> format works
+                resource_names = self.module.EnumResourceNames(
+                    handle, self._id2str(resource_type))
+                self.assertEqual(resource_names, expected)
+
+        with self.assertRaises(error):
+            self.module.EnumResourceNames(2, 3)
+
+    def test_enum_resource_languages(self):
+        with self.load_library(win32api, u'shell32.dll') as handle:
+            resource_types = win32api.EnumResourceTypes(handle)
+            for resource_type in resource_types:
+                resource_names = win32api.EnumResourceNames(
+                    handle, resource_type)
+                for resource_name in resource_names:
+                    expected = win32api.EnumResourceLanguages(
+                        handle, resource_type, resource_name)
+                    resource_languages = self.module.EnumResourceLanguages(
+                        handle, resource_type, resource_name)
+                    self.assertEqual(resource_languages, expected)
+                    # check that the #<index> format works
+                    resource_languages = self.module.EnumResourceLanguages(
+                        handle, self._id2str(resource_type),
+                        self._id2str(resource_name))
+                    self.assertEqual(resource_languages, expected)
+
+        with self.assertRaises(error):
+            self.module.EnumResourceLanguages(handle, resource_type, 2235)
+
+    def test_load_resource(self):
+        with self.load_library(win32api, u'explorer.exe') as handle:
+            resource_types = win32api.EnumResourceTypes(handle)
+            for resource_type in resource_types:
+                resource_names = win32api.EnumResourceNames(
+                    handle, resource_type)
+                for resource_name in resource_names:
+                    resource_languages = win32api.EnumResourceLanguages(
+                        handle, resource_type, resource_name)
+                    for resource_language in resource_languages:
+                        expected = win32api.LoadResource(
+                            handle, resource_type, resource_name,
+                            resource_language)
+                        resource = self.module.LoadResource(
+                            handle, resource_type, resource_name,
+                            resource_language)
+                        # check that the #<index> format works
+                        resource = self.module.LoadResource(
+                            handle, self._id2str(resource_type),
+                            self._id2str(resource_name),
+                            resource_language)
+                        self.assertEqual(resource, expected)
+
+        with self.assertRaises(error):
+            with self.nofaulthandler():
+                self.module.LoadResource(
+                    handle, resource_type, resource_name, 12435)
+
+    def test_get_tick_count(self):
+        self.assertGreater(self.module.GetTickCount(), 0.0)
+
+    def test_begin_and_end_update_resource(self):
+        # given
+        module = self.module
+        filename = os.path.join(self.tempdir, 'python.exe')
+        with self.load_library(module, filename) as handle:
+            count = len(module.EnumResourceTypes(handle))
+
+        # when
+        handle = module.BeginUpdateResource(filename, False)
+        module.EndUpdateResource(handle, False)
+
+        # then
+        with self.load_library(module, filename) as handle:
+            self.assertEqual(len(module.EnumResourceTypes(handle)), count)
+
+        # when
+        handle = module.BeginUpdateResource(filename, True)
+        module.EndUpdateResource(handle, True)
+
+        # then
+        with self.load_library(module, filename) as handle:
+            self.assertEqual(len(module.EnumResourceTypes(handle)), count)
+
+    def test_begin_removing_all_resources(self):
+        if skip_on_wine:
+            self.skipTest('EnumResourceTypes known failure on wine, see #59')
+
+        # given
+        module = self.module
+        filename = os.path.join(self.tempdir, 'python.exe')
+
+        # when
+        handle = module.BeginUpdateResource(filename, True)
+        module.EndUpdateResource(handle, False)
+
+        # then
+        with self.load_library(module, filename) as handle:
+            self.assertEqual(len(module.EnumResourceTypes(handle)), 0)
+
+    def test_begin_update_resource_with_invalid(self):
+        if skip_on_wine:
+            self.skipTest('BeginUpdateResource known failure on wine, see #59')
+
+            # when/then
+        with self.assertRaises(error) as context:
+            self.module.BeginUpdateResource('invalid', False)
+        # the errno cannot be 0 (i.e. success)
+        self.assertNotEqual(context.exception.winerror, 0)
+
+    def test_end_update_resource_with_invalid(self):
+        if skip_on_wine:
+            self.skipTest('EndUpdateResource known failure on wine, see #59')
+
+        # when/then
+        with self.assertRaises(error) as context:
+            self.module.EndUpdateResource(-3, False)
+        # the errno cannot be 0 (i.e. success)
+        self.assertNotEqual(context.exception.winerror, 0)
+
+    def test_update_resource(self):
+        # given
+        module = self.module
+        filename = os.path.join(self.tempdir, 'python.exe')
+        with self.load_library(self.module, filename) as handle:
+            resource_type = module.EnumResourceTypes(handle)[-1]
+            resource_name = module.EnumResourceNames(handle, resource_type)[-1]
+            resource_language = module.EnumResourceLanguages(
+                handle, resource_type, resource_name)[-1]
+            resource = module.LoadResource(
+                handle, resource_type, resource_name, resource_language)
+
+        # when
+        with self.resource_update(self.module, filename) as handle:
+            module.UpdateResource(
+                handle, resource_type, resource_name, resource[:-2],
+                resource_language)
+
+        # then
+        with self.load_library(self.module, filename) as handle:
+            updated = module.LoadResource(
+                handle, resource_type, resource_name, resource_language)
+        self.assertEqual(len(updated), len(resource) - 2)
+        self.assertEqual(updated, resource[:-2])
+
+    def test_update_resource_with_unicode(self):
+        # given
+        module = self.module
+        filename = os.path.join(self.tempdir, 'python.exe')
+        with self.load_library(module, filename) as handle:
+            resource_type = module.EnumResourceTypes(handle)[-1]
+            resource_name = module.EnumResourceNames(handle, resource_type)[-1]
+            resource_language = module.EnumResourceLanguages(
+                handle, resource_type, resource_name)[-1]
+        resource = u"\N{GREEK CAPITAL LETTER DELTA}"
+
+        # when
+        with self.resource_update(module, filename) as handle:
+            with self.assertRaises(TypeError):
+                module.UpdateResource(
+                    handle, resource_type, resource_name, resource,
+                    resource_language)
+
+    def test_get_windows_directory(self):
+        # given
+        expected = win32api.GetWindowsDirectory()
+
+        # when
+        result = self.module.GetWindowsDirectory()
+
+        # then
+        # note: pywin32 returns str on py27, unicode (which is str) on py3
+        self.assertIsInstance(result, str)
+        self.assertEqual(result.lower(), r"c:\windows")
+        self.assertEqual(result, expected)
+
+    def test_get_system_directory(self):
+        # given
+        expected = win32api.GetSystemDirectory()
+
+        # when
+        result = self.module.GetSystemDirectory()
+
+        # then
+        # note: pywin32 returns str on py27, unicode (which is str) on py3
+        self.assertIsInstance(result, str)
+        self.assertEqual(result.lower(), r"c:\windows\system32")
+        self.assertEqual(result, expected)
+
+    def _id2str(self, type_id):
+        if hasattr(type_id, 'index'):
+            return type_id
+        else:
+            return u'#{0}'.format(type_id)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `pywin32-ctypes-0.2.1/win32ctypes/tests/test_win32cred.py` & `pywin32-ctypes-0.2.2/win32ctypes/tests/test_win32cred.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-#
-# (C) Copyright 2014 Enthought, Inc., Austin, TX
-# All right reserved.
-#
-# This file is open source software distributed according to the terms in
-# LICENSE.txt
-#
-import os
-import sys
-import unittest
-
-import win32cred
-
-from win32ctypes.core._winerrors import ERROR_NOT_FOUND
-from win32ctypes.pywin32.pywintypes import error
-from win32ctypes.pywin32.win32cred import (
-    CredDelete, CredRead, CredWrite, CredEnumerate,
-    CRED_PERSIST_ENTERPRISE, CRED_TYPE_GENERIC,
-    CRED_ENUMERATE_ALL_CREDENTIALS)
-
-# find the pywin32 version
-version_file = os.path.join(
-    os.path.dirname(
-        os.path.dirname(win32cred.__file__)), 'pywin32.version.txt')
-if os.path.exists(version_file):
-    with open(version_file) as handle:
-        pywin32_build = handle.read().strip()
-else:
-    pywin32_build = None
-
-
-class TestCred(unittest.TestCase):
-
-    def setUp(self):
-        from pywintypes import error
-        try:
-            win32cred.CredDelete(u'jone@doe', CRED_TYPE_GENERIC)
-        except error:
-            pass
-
-    def _demo_credentials(self, UserName=u'jone'):
-        return {
-            "Type": CRED_TYPE_GENERIC,
-            "TargetName": u'jone@doe',
-            "UserName": UserName,
-            "CredentialBlob": u"doefsajfsakfj",
-            "Comment": u"Created by MiniPyWin32Cred test suite",
-            "Persist": CRED_PERSIST_ENTERPRISE}
-
-    @unittest.skipIf(
-        pywin32_build == "223" and sys.version_info[:2] == (3, 7),
-        "pywin32 version 223 bug with CredRead (mhammond/pywin32#1232)")
-    def test_write_to_pywin32(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials()
-        CredWrite(r_credentials)
-
-        # when
-        credentials = win32cred.CredRead(
-            TargetName=target, Type=CRED_TYPE_GENERIC)
-
-        # then
-        self.assertEqual(credentials["Type"], CRED_TYPE_GENERIC)
-        self.assertEqual(credentials["UserName"], u"jone")
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        # XXX: the fact that we have to decode the password when reading, but
-        # not encode when writing is a bit strange, but that's what pywin32
-        # seems to do and we try to be backward compatible here.
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_read_from_pywin32(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials()
-        win32cred.CredWrite(r_credentials)
-
-        # when
-        credentials = CredRead(target, CRED_TYPE_GENERIC)
-
-        # then
-        self.assertEqual(credentials["UserName"], u"jone")
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_read_from_pywin32_with_none_usename(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials(None)
-        win32cred.CredWrite(r_credentials)
-
-        # when
-        credentials = CredRead(target, CRED_TYPE_GENERIC)
-
-        self.assertEqual(credentials["UserName"], None)
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_write_to_pywin32_with_none_usename(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials(None)
-        CredWrite(r_credentials)
-
-        # when
-        credentials = win32cred.CredRead(target, CRED_TYPE_GENERIC)
-
-        self.assertEqual(credentials["UserName"], None)
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_read_write(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials()
-
-        # when
-        CredWrite(r_credentials)
-        credentials = CredRead(target, CRED_TYPE_GENERIC)
-
-        self.assertEqual(credentials["UserName"], u"jone")
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_read_write_with_none_username(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials(None)
-
-        # when
-        CredWrite(r_credentials)
-        credentials = CredRead(target, CRED_TYPE_GENERIC)
-
-        # then
-        self.assertEqual(credentials["UserName"], None)
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_enumerate_filter(self):
-        # given
-        r_credentials = self._demo_credentials()
-        CredWrite(r_credentials)
-
-        # when
-        credentials = CredEnumerate('jone*')[0]
-
-        # then
-        self.assertEqual(credentials["UserName"], u"jone")
-        self.assertEqual(credentials["TargetName"], u'jone@doe')
-        self.assertEqual(
-            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
-        self.assertEqual(
-            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
-
-    def test_enumerate_no_filter(self):
-        # given
-        r_credentials = self._demo_credentials()
-        CredWrite(r_credentials)
-
-        # when
-        pywin32_result = win32cred.CredEnumerate()
-        credentials = CredEnumerate()
-
-        # then
-        self.assertEqual(len(credentials), len(pywin32_result))
-
-    def test_enumerate_all(self):
-        # when
-        credentials = CredEnumerate(Flags=CRED_ENUMERATE_ALL_CREDENTIALS)
-
-        # then
-        self.assertGreater(len(credentials), 1)
-
-    def test_read_doesnt_exists(self):
-        # given
-        target = "Floupi_dont_exists@MiniPyWin"
-
-        # when/then
-        with self.assertRaises(error) as ctx:
-            CredRead(target, CRED_TYPE_GENERIC)
-        self.assertTrue(ctx.exception.winerror, ERROR_NOT_FOUND)
-
-    def test_delete_simple(self):
-        # given
-        target = u'jone@doe'
-        r_credentials = self._demo_credentials()
-        CredWrite(r_credentials, 0)
-        credentials = CredRead(target, CRED_TYPE_GENERIC)
-        self.assertTrue(credentials is not None)
-
-        # when
-        CredDelete(target, CRED_TYPE_GENERIC)
-
-        # then
-        with self.assertRaises(error) as ctx:
-            CredRead(target, CRED_TYPE_GENERIC)
-        self.assertEqual(ctx.exception.winerror, ERROR_NOT_FOUND)
-        self.assertEqual(ctx.exception.funcname, "CredRead")
-
-    def test_delete_doesnt_exists(self):
-        # given
-        target = u"Floupi_doesnt_exists@MiniPyWin32"
-
-        # when/then
-        with self.assertRaises(error) as ctx:
-            CredDelete(target, CRED_TYPE_GENERIC)
-        self.assertEqual(ctx.exception.winerror, ERROR_NOT_FOUND)
-        self.assertEqual(ctx.exception.funcname, "CredDelete")
-
-
-if __name__ == '__main__':
-    unittest.main()
+#
+# (C) Copyright 2014 Enthought, Inc., Austin, TX
+# All right reserved.
+#
+# This file is open source software distributed according to the terms in
+# LICENSE.txt
+#
+import os
+import sys
+import unittest
+
+import win32cred
+
+from win32ctypes.core._winerrors import ERROR_NOT_FOUND
+from win32ctypes.pywin32.pywintypes import error
+from win32ctypes.pywin32.win32cred import (
+    CredDelete, CredRead, CredWrite, CredEnumerate,
+    CRED_PERSIST_ENTERPRISE, CRED_TYPE_GENERIC,
+    CRED_ENUMERATE_ALL_CREDENTIALS)
+
+# find the pywin32 version
+version_file = os.path.join(
+    os.path.dirname(
+        os.path.dirname(win32cred.__file__)), 'pywin32.version.txt')
+if os.path.exists(version_file):
+    with open(version_file) as handle:
+        pywin32_build = handle.read().strip()
+else:
+    pywin32_build = None
+
+
+class TestCred(unittest.TestCase):
+
+    def setUp(self):
+        from pywintypes import error
+        try:
+            win32cred.CredDelete(u'jone@doe', CRED_TYPE_GENERIC)
+        except error:
+            pass
+
+    def _demo_credentials(self, UserName=u'jone'):
+        return {
+            "Type": CRED_TYPE_GENERIC,
+            "TargetName": u'jone@doe',
+            "UserName": UserName,
+            "CredentialBlob": u"doefsajfsakfj",
+            "Comment": u"Created by MiniPyWin32Cred test suite",
+            "Persist": CRED_PERSIST_ENTERPRISE}
+
+    @unittest.skipIf(
+        pywin32_build == "223" and sys.version_info[:2] == (3, 7),
+        "pywin32 version 223 bug with CredRead (mhammond/pywin32#1232)")
+    def test_write_to_pywin32(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials()
+        CredWrite(r_credentials)
+
+        # when
+        credentials = win32cred.CredRead(
+            TargetName=target, Type=CRED_TYPE_GENERIC)
+
+        # then
+        self.assertEqual(credentials["Type"], CRED_TYPE_GENERIC)
+        self.assertEqual(credentials["UserName"], u"jone")
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        # XXX: the fact that we have to decode the password when reading, but
+        # not encode when writing is a bit strange, but that's what pywin32
+        # seems to do and we try to be backward compatible here.
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_read_from_pywin32(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials()
+        win32cred.CredWrite(r_credentials)
+
+        # when
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+
+        # then
+        self.assertEqual(credentials["UserName"], u"jone")
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_read_from_pywin32_with_none_usename(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials(None)
+        win32cred.CredWrite(r_credentials)
+
+        # when
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+
+        self.assertEqual(credentials["UserName"], None)
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_write_to_pywin32_with_none_usename(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials(None)
+        CredWrite(r_credentials)
+
+        # when
+        credentials = win32cred.CredRead(target, CRED_TYPE_GENERIC)
+
+        self.assertEqual(credentials["UserName"], None)
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_read_write(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials()
+
+        # when
+        CredWrite(r_credentials)
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+
+        self.assertEqual(credentials["UserName"], u"jone")
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_read_write_with_none_username(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials(None)
+
+        # when
+        CredWrite(r_credentials)
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+
+        # then
+        self.assertEqual(credentials["UserName"], None)
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_enumerate_filter(self):
+        # given
+        r_credentials = self._demo_credentials()
+        CredWrite(r_credentials)
+
+        # when
+        credentials = CredEnumerate('jone*')[0]
+
+        # then
+        self.assertEqual(credentials["UserName"], u"jone")
+        self.assertEqual(credentials["TargetName"], u'jone@doe')
+        self.assertEqual(
+            credentials["Comment"], u"Created by MiniPyWin32Cred test suite")
+        self.assertEqual(
+            credentials["CredentialBlob"].decode('utf-16'), u"doefsajfsakfj")
+
+    def test_enumerate_no_filter(self):
+        # given
+        r_credentials = self._demo_credentials()
+        CredWrite(r_credentials)
+
+        # when
+        pywin32_result = win32cred.CredEnumerate()
+        credentials = CredEnumerate()
+
+        # then
+        self.assertEqual(len(credentials), len(pywin32_result))
+
+    def test_enumerate_all(self):
+        # when
+        credentials = CredEnumerate(Flags=CRED_ENUMERATE_ALL_CREDENTIALS)
+
+        # then
+        self.assertGreater(len(credentials), 1)
+
+    def test_read_doesnt_exists(self):
+        # given
+        target = "Floupi_dont_exists@MiniPyWin"
+
+        # when/then
+        with self.assertRaises(error) as ctx:
+            CredRead(target, CRED_TYPE_GENERIC)
+        self.assertTrue(ctx.exception.winerror, ERROR_NOT_FOUND)
+
+    def test_delete_simple(self):
+        # given
+        target = u'jone@doe'
+        r_credentials = self._demo_credentials()
+        CredWrite(r_credentials, 0)
+        credentials = CredRead(target, CRED_TYPE_GENERIC)
+        self.assertTrue(credentials is not None)
+
+        # when
+        CredDelete(target, CRED_TYPE_GENERIC)
+
+        # then
+        with self.assertRaises(error) as ctx:
+            CredRead(target, CRED_TYPE_GENERIC)
+        self.assertEqual(ctx.exception.winerror, ERROR_NOT_FOUND)
+        self.assertEqual(ctx.exception.funcname, "CredRead")
+
+    def test_delete_doesnt_exists(self):
+        # given
+        target = u"Floupi_doesnt_exists@MiniPyWin32"
+
+        # when/then
+        with self.assertRaises(error) as ctx:
+            CredDelete(target, CRED_TYPE_GENERIC)
+        self.assertEqual(ctx.exception.winerror, ERROR_NOT_FOUND)
+        self.assertEqual(ctx.exception.funcname, "CredDelete")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

