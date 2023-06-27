# Comparing `tmp/probeinterface-0.2.8.tar.gz` & `tmp/probeinterface-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probeinterface-0.2.8.tar", last modified: Wed Mar 23 09:47:19 2022, max compression
+gzip compressed data, was "probeinterface-0.2.9.tar", last modified: Fri Apr 15 07:07:01 2022, max compression
```

## Comparing `probeinterface-0.2.8.tar` & `probeinterface-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:47:19.536601 probeinterface-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-23 09:47:04.000000 probeinterface-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-23 09:47:19.536601 probeinterface-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-03-23 09:47:04.000000 probeinterface-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:47:19.536601 probeinterface-0.2.8/probeinterface/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    32731 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/library.py
--rw-r--r--   0 runner    (1001) docker     (121)    11197 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    33630 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/probe.py
--rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/probegroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/shank.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-03-23 09:47:04.000000 probeinterface-0.2.8/probeinterface/wiring.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:47:19.536601 probeinterface-0.2.8/probeinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-23 09:47:19.000000 probeinterface-0.2.8/probeinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-03-23 09:47:19.000000 probeinterface-0.2.8/probeinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 09:47:19.000000 probeinterface-0.2.8/probeinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-23 09:47:19.000000 probeinterface-0.2.8/probeinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-23 09:47:19.000000 probeinterface-0.2.8/probeinterface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 09:47:19.536601 probeinterface-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-03-23 09:47:04.000000 probeinterface-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 07:07:01.325641 probeinterface-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-15 07:06:53.000000 probeinterface-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-04-15 07:07:01.325641 probeinterface-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-04-15 07:06:53.000000 probeinterface-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 07:07:01.325641 probeinterface-0.2.9/probeinterface/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33103 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/library.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11197 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33630 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/probe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/probegroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/shank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-04-15 07:06:53.000000 probeinterface-0.2.9/probeinterface/wiring.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 07:07:01.325641 probeinterface-0.2.9/probeinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-04-15 07:07:01.000000 probeinterface-0.2.9/probeinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-15 07:07:01.000000 probeinterface-0.2.9/probeinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 07:07:01.000000 probeinterface-0.2.9/probeinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-15 07:07:01.000000 probeinterface-0.2.9/probeinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-15 07:07:01.000000 probeinterface-0.2.9/probeinterface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-15 07:07:01.325641 probeinterface-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-04-15 07:06:53.000000 probeinterface-0.2.9/setup.py
```

### Comparing `probeinterface-0.2.8/LICENSE` & `probeinterface-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/PKG-INFO` & `probeinterface-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probeinterface
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package to handle probe layout, geometry and wiring to device.
 Home-page: https://github.com/SpikeInterface/probeinterface
 Author: Samuel Garcia
 Author-email: sam.garcia.die@gmail.com
 License: UNKNOWN
 Description: # probeinterface
```

### Comparing `probeinterface-0.2.8/README.md` & `probeinterface-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/__init__.py` & `probeinterface-0.2.9/probeinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/generator.py` & `probeinterface-0.2.9/probeinterface/generator.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/io.py` & `probeinterface-0.2.9/probeinterface/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -835,20 +835,27 @@
     """
     import xml.etree.ElementTree as ET
 
     folder = Path(folder).absolute()
     assert folder.is_dir()
 
     # find settings
-    settings_files = [p for p in folder.iterdir() if p.suffix == ".xml" and "setting" in p.name]
+    # settings_files = [p for p in folder.iterdir() if p.suffix == ".xml" and "setting" in p.name]
+    settings_files = [p for p in folder.glob("**/*.xml") if "setting" in p.name]
     if len(settings_files) > 1:
-        assert settings_file is not None, ("More than one settings file found. Specify a settings "
-                                           "file with the 'settings_file' argument")
+        if settings_file is None:
+            if raise_error:
+                raise FileNotFoundError("More than one settings file found. Specify a settings "
+                                           "file with the 'settings_file' argument")    
+            else:
+                return None
     elif len(settings_files) == 0:
-        raise FileNotFoundError("Cannot find settings.xml file!")
+        if raise_error:
+            raise FileNotFoundError("Cannot find settings.xml file!")
+        return None
     else:
         settings_file = settings_files[0]
 
     # parse xml
     tree = ET.parse(str(settings_file))
     root = tree.getroot()
 
@@ -899,14 +906,21 @@
 
     # NP geometry constants
     contact_width = 12
     shank_pitch = 250
 
     # TODO get example of multishank for parsing
     shank_ids = None
+    
+    # x offset
+    if "2.0" in probe_name:
+        x_shift = -8
+    else:
+        x_shift = -11
+    positions[:, 0] += x_shift
 
     probe = Probe(ndim=2, si_units='um')
     probe.set_contacts(positions=positions, shapes='square',
                        shank_ids=shank_ids,
                        shape_params={'width': contact_width})
     probe.set_contact_ids(channels)
     probe.annotate(probe_name=probe_name,
```

### Comparing `probeinterface-0.2.8/probeinterface/library.py` & `probeinterface-0.2.9/probeinterface/library.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/plotting.py` & `probeinterface-0.2.9/probeinterface/plotting.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/probe.py` & `probeinterface-0.2.9/probeinterface/probe.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/probegroup.py` & `probeinterface-0.2.9/probeinterface/probegroup.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/shank.py` & `probeinterface-0.2.9/probeinterface/shank.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/utils.py` & `probeinterface-0.2.9/probeinterface/utils.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface/wiring.py` & `probeinterface-0.2.9/probeinterface/wiring.py`

 * *Files identical despite different names*

### Comparing `probeinterface-0.2.8/probeinterface.egg-info/PKG-INFO` & `probeinterface-0.2.9/probeinterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probeinterface
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package to handle probe layout, geometry and wiring to device.
 Home-page: https://github.com/SpikeInterface/probeinterface
 Author: Samuel Garcia
 Author-email: sam.garcia.die@gmail.com
 License: UNKNOWN
 Description: # probeinterface
```

### Comparing `probeinterface-0.2.8/setup.py` & `probeinterface-0.2.9/setup.py`

 * *Files identical despite different names*

