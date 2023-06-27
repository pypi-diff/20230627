# Comparing `tmp/selenium_profiles-2.2.7.tar.gz` & `tmp/selenium_profiles-2.2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_profiles-2.2.7.tar", last modified: Tue Jun 27 08:21:01 2023, max compression
+gzip compressed data, was "dist\selenium_profiles-2.2.7.1.tar", last modified: Tue Jun 27 11:43:17 2023, max compression
```

## Comparing `selenium_profiles-2.2.7.tar` & `selenium_profiles-2.2.7.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7/LICENSE.md
--rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0    14202 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    12856 2023-06-27 07:02:11.000000 selenium_profiles-2.2.7/README.md
--rw-rw-rw-   0        0        0     1695 2022-11-30 14:03:19.000000 selenium_profiles-2.2.7/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2083 2023-06-27 08:10:20.000000 selenium_profiles-2.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/
--rw-rw-rw-   0        0        0       23 2023-06-27 08:07:14.000000 selenium_profiles-2.2.7/src/selenium_profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/export_profile.js
--rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/fetch.js
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/__init.py
--rw-rw-rw-   0        0        0     2334 2023-06-20 18:15:50.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/devtools_anti_detector.js
--rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/
--rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/
--rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
--rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/default.json
--rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/example.json
--rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7/src/selenium_profiles/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/__init__.py
--rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    24904 2023-06-27 06:39:28.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/profiles.py
--rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/proxy.py
--rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7/src/selenium_profiles/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles/utils/
--rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7/src/selenium_profiles/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7/src/selenium_profiles/utils/colab_utils.py
--rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7/src/selenium_profiles/utils/utils.py
--rw-rw-rw-   0        0        0    11075 2023-06-27 07:46:17.000000 selenium_profiles-2.2.7/src/selenium_profiles/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/
--rw-rw-rw-   0        0        0    14202 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1931 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/src/selenium_profiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 08:21:01.000000 selenium_profiles-2.2.7/tests/
--rw-rw-rw-   0        0        0     1617 2023-06-20 18:05:33.000000 selenium_profiles-2.2.7/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.1/LICENSE.md
+-rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    14204 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12856 2023-06-27 07:02:11.000000 selenium_profiles-2.2.7.1/README.md
+-rw-rw-rw-   0        0        0     1730 2023-06-27 08:22:38.000000 selenium_profiles-2.2.7.1/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2083 2023-06-27 08:10:20.000000 selenium_profiles-2.2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/
+-rw-rw-rw-   0        0        0       25 2023-06-27 11:42:48.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/proxy_extension/
+-rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/proxy_extension/
+-rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/__init.py
+-rw-rw-rw-   0        0        0     2334 2023-06-20 18:15:50.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/devtools_anti_detector.js
+-rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/
+-rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/
+-rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/default.json
+-rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/example.json
+-rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24902 2023-06-27 09:54:03.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/profiles.py
+-rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/proxy.py
+-rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/utils/colab_utils.py
+-rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/utils/utils.py
+-rw-rw-rw-   0        0        0    11075 2023-06-27 07:46:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/
+-rw-rw-rw-   0        0        0    14204 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1931 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:43:17.000000 selenium_profiles-2.2.7.1/tests/
+-rw-rw-rw-   0        0        0     1617 2023-06-20 18:05:33.000000 selenium_profiles-2.2.7.1/tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.7/LICENSE.md` & `selenium_profiles-2.2.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/PKG-INFO` & `selenium_profiles-2.2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_profiles
-Version: 2.2.7
+Version: 2.2.7.1
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
```

### Comparing `selenium_profiles-2.2.7/README.md` & `selenium_profiles-2.2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/build_upload.md` & `selenium_profiles-2.2.7.1/build_upload.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 # 3.11
 C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install C:\Users\aurin\PycharmProjects\selenium_profiles
 ```
 
 ## install all python versions from pypi
 ```shell
 # 3.7
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles==2.2.7
 # 3.8
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7
 # 3.9
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles==2.2.7
 # 3.10
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7
 # 3.11
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7
 ```
 
 ## install from GitHub
 ```shell
 pip install https://github.com/kaliiiiiiiiii/Selenium-Profiles/archive/refs/heads/master.zip
 ```
```

### Comparing `selenium_profiles-2.2.7/setup.py` & `selenium_profiles-2.2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/files/proxy_extension/background.js` & `selenium_profiles-2.2.7.1/src/selenium_profiles/files/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/files/tmp/proxy_extension/background.js` & `selenium_profiles-2.2.7.1/src/selenium_profiles/files/tmp/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/js/export_profile.js` & `selenium_profiles-2.2.7.1/src/selenium_profiles/js/export_profile.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/js/fetch.js` & `selenium_profiles-2.2.7.1/src/selenium_profiles/js/fetch.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/js/undetected/devtools_anti_detector.js` & `selenium_profiles-2.2.7.1/src/selenium_profiles/js/undetected/devtools_anti_detector.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/default.json` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/default.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/example.json` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/example.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/profiles.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/profiles/scratch.json` & `selenium_profiles-2.2.7.1/src/selenium_profiles/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/scripts/driver_utils.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/scripts/profiles.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 useragent = driver.execute_cdp_cmd("Browser.getVersion",{})["product"]
                 import re
                 version = re.findall(r'(?<=Chrome/)\d+(?:\.\d+)+|(?<=Chromium/)\d+(?:\.\d+)+', useragent)
                 version = version[0]
             else:
                 raise ValueError("driver or version needs to be specified")
 
-        elif type(version) == str:
+        if type(version) == str:
             if profile["userAgent"]:
                 import re
                 # noinspection PyTypeChecker
                 profile["userAgent"] = re.sub(r"(?<=Chrome/)\d+(?:\.\d+)+|(?<=Chromium/)\d+(?:\.\d+)+",
                                               version.split(".")[0] + ".0.0.0", profile["userAgent"])
 
             if profile["userAgentMetadata"]:
```

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/scripts/proxy.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/scripts/undetected.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/scripts/undetected.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/utils/colab_utils.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/utils/utils.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles/webdriver.py` & `selenium_profiles-2.2.7.1/src/selenium_profiles/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles.egg-info/PKG-INFO` & `selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-profiles
-Version: 2.2.7
+Version: 2.2.7.1
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
```

### Comparing `selenium_profiles-2.2.7/src/selenium_profiles.egg-info/SOURCES.txt` & `selenium_profiles-2.2.7.1/src/selenium_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7/tests/test_driver.py` & `selenium_profiles-2.2.7.1/tests/test_driver.py`

 * *Files identical despite different names*

