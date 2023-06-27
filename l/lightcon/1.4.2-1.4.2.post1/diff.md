# Comparing `tmp/lightcon-1.4.2.tar.gz` & `tmp/lightcon-1.4.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.4.2.tar", last modified: Tue Jun 27 11:40:38 2023, max compression
+gzip compressed data, was "lightcon-1.4.2.post1.tar", last modified: Tue Jun 27 11:54:42 2023, max compression
```

## Comparing `lightcon-1.4.2.tar` & `lightcon-1.4.2.post1.tar`

### file list

```diff
@@ -1,21 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/
--rw-rw-rw-   0        0        0     1082 2023-06-27 11:38:49.000000 lightcon-1.4.2/LICENCE
--rw-rw-rw-   0        0        0      249 2023-06-27 11:38:49.000000 lightcon-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6252 2023-06-27 11:40:38.856850 lightcon-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-06-27 11:38:49.000000 lightcon-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/
--rw-rw-rw-   0        0        0        0 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/__config__.py
--rw-rw-rw-   0        0        0      715 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-27 11:38:49.000000 lightcon-1.4.2/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/datasets/
-drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon/datasets/data/
--rw-rw-rw-   0        0        0    11968 2023-06-27 11:39:53.000000 lightcon-1.4.2/lightcon/datasets/data/motor_parameters.json
--rw-rw-rw-   0        0        0     4990 2023-06-27 11:39:53.000000 lightcon-1.4.2/lightcon/datasets/data/stage_parameters.json
-drwxrwxrwx   0        0        0        0 2023-06-27 11:40:38.856850 lightcon-1.4.2/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 11:40:38.000000 lightcon-1.4.2/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 11:40:38.856850 lightcon-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1744 2023-06-27 11:38:49.000000 lightcon-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/
+-rw-rw-rw-   0        0        0     1082 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/LICENCE
+-rw-rw-rw-   0        0        0      249 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6258 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.892080 lightcon-1.4.2.post1/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/__config__.py
+-rw-rw-rw-   0        0        0      717 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/beam_alignment/
+-rw-rw-rw-   0        0        0       93 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/beam_alignment/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/beam_alignment/_beam_alignment.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/calculate/
+-rw-rw-rw-   0        0        0      190 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_gauss.py
+-rw-rw-rw-   0        0        0     3393 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_iso.py
+-rw-rw-rw-   0        0        0     1407 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_calculate_motor_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/camera_app_client/
+-rw-rw-rw-   0        0        0       76 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/camera_app_client/__init__.py
+-rw-rw-rw-   0        0        0     2965 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/camera_app_client/_camera_app_client.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/common/
+-rw-rw-rw-   0        0        0      614 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_converters.py
+-rw-rw-rw-   0        0        0     3155 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_http_methods.py
+-rw-rw-rw-   0        0        0     5607 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_leprecan_provider.py
+-rw-rw-rw-   0        0        0      336 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_load_motor_and_stage_parameters.py
+-rw-rw-rw-   0        0        0     1042 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_serial_tools.py
+-rw-rw-rw-   0        0        0     5151 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_udp_locator.py
+-rw-rw-rw-   0        0        0      506 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/stage_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/datasets/
+-rw-rw-rw-   0        0        0      159 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3055 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/_base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/datasets/data/
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0    11968 2023-06-27 11:53:57.000000 lightcon-1.4.2.post1/lightcon/datasets/data/motor_parameters.json
+-rw-rw-rw-   0        0        0     4990 2023-06-27 11:53:57.000000 lightcon-1.4.2.post1/lightcon/datasets/data/stage_parameters.json
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/eth_motor_board/
+-rw-rw-rw-   0        0        0      204 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/__init__.py
+-rw-rw-rw-   0        0        0    15177 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board.py
+-rw-rw-rw-   0        0        0     1920 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/fast_daq/
+-rw-rw-rw-   0        0        0      130 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/fast_daq/__init__.py
+-rw-rw-rw-   0        0        0     5442 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/fast_daq/_fast_daq.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/harpia/
+-rw-rw-rw-   0        0        0      237 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/__init__.py
+-rw-rw-rw-   0        0        0    24803 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia.py
+-rw-rw-rw-   0        0        0     2222 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia_leprecan_provider.py
+-rw-rw-rw-   0        0        0     8813 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia_model_decoder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/harpia_daq/
+-rw-rw-rw-   0        0        0       84 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia_daq/__init__.py
+-rw-rw-rw-   0        0        0     5744 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia_daq/_harpia_daq.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/laser_clients/
+-rw-rw-rw-   0        0        0       91 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/laser_clients/__init__.py
+-rw-rw-rw-   0        0        0     8634 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/laser_clients/_laser_clients.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/style/
+-rw-rw-rw-   0        0        0      229 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/__init__.py
+-rw-rw-rw-   0        0        0     7848 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/_plotstyle_1d.py
+-rw-rw-rw-   0        0        0     7839 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/plotstyle_1d.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/timing_controller/
+-rw-rw-rw-   0        0        0      172 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/__init__.py
+-rw-rw-rw-   0        0        0     6326 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller.py
+-rw-rw-rw-   0        0        0     7234 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller_v2.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/utils/
+-rw-rw-rw-   0        0        0       50 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/utils/__init__.py
+-rw-rw-rw-   0        0        0      591 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/utils/_fixes.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/wintopas/
+-rw-rw-rw-   0        0        0       65 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/wintopas/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/wintopas/_wintopas.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6258 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1894 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/setup.py
```

### Comparing `lightcon-1.4.2/LICENCE` & `lightcon-1.4.2.post1/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2/PKG-INFO` & `lightcon-1.4.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2
+Version: 1.4.2.post1
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2/README.md` & `lightcon-1.4.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2/lightcon/__init__.py` & `lightcon-1.4.2.post1/lightcon/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.2"
+__version__ = "1.4.2-1"
 
 from . import wintopas
 from . import timing_controller
 from . import style
 from . import laser_clients
 from . import harpia
 from . import harpia_daq
```

### Comparing `lightcon-1.4.2/lightcon/datasets/data/motor_parameters.json` & `lightcon-1.4.2.post1/lightcon/datasets/data/motor_parameters.json`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2/lightcon/datasets/data/stage_parameters.json` & `lightcon-1.4.2.post1/lightcon/datasets/data/stage_parameters.json`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2/lightcon.egg-info/PKG-INFO` & `lightcon-1.4.2.post1/lightcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2
+Version: 1.4.2.post1
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2/setup.py` & `lightcon-1.4.2.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     author='Vytautas Butkus',
     author_email='vytautas.butkus@lightcon.com',
     description='A set of APIs to Light Conversion devices',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/harpiasoftware/light-conversion-apis.git',
     install_requires = install_requires,
-    packages=setuptools.find_packages(include=["lightcon"]),
+    packages=setuptools.find_packages(include=["lightcon*"]),
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Development Status :: 1 - Planning',
     ],
```

