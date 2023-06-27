# Comparing `tmp/pineworkslabs-0.1.0.tar.gz` & `tmp/pineworkslabs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/pineworkslabs/rp-2040-gpio-board/Pine/dist/tmpwo_vl6sk/pineworkslabs-0.1.0.tar", last modified: Tue Jun  7 15:52:51 2022, max compression
+gzip compressed data, was "/builds/pineworkslabs/rp-2040-gpio-board/Pine/dist/.tmp-8nqo_xyb/pineworkslabs-0.2.0.tar", last modified: Tue Jun 27 01:51:05 2023, max compression
```

## Comparing `pineworkslabs-0.1.0.tar` & `pineworkslabs-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    34282 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1299 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      731 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      916 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs/
--rw-rw-rw-   0 root         (0) root         (0)     2298 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/src/pineworkslabs/GPIO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 15:52:32.000000 pineworkslabs-0.1.0/src/pineworkslabs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1299 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-06-07 15:52:51.000000 pineworkslabs-0.1.0/src/pineworkslabs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34282 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs/
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/src/pineworkslabs/GPIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/src/pineworkslabs/RPi.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 01:50:51.000000 pineworkslabs-0.2.0/src/pineworkslabs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 01:51:05.000000 pineworkslabs-0.2.0/src/pineworkslabs.egg-info/top_level.txt
```

### Comparing `pineworkslabs-0.1.0/LICENSE` & `pineworkslabs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pineworkslabs-0.1.0/setup.py` & `pineworkslabs-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pineworkslabs",
-    version="0.1.0",
+    version="0.2.0",
     author="Pineworks Labs",
     author_email="shelby@pineworkslabs.com",
     description="An access layer for the Pineworks Labs RP2040 GPIO board",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/pineworkslabs/rp-2040-gpio-board",
     project_urls={
@@ -19,9 +19,8 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
-    install_requires="telemetrix_rpi_pico == 1.1"
 )
```

### Comparing `pineworkslabs-0.1.0/src/pineworkslabs/GPIO.py` & `pineworkslabs-0.2.0/src/pineworkslabs/GPIO.py`

 * *Files identical despite different names*

