# Comparing `tmp/bmw-lobster-0.9.7.tar.gz` & `tmp/bmw-lobster-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-0.9.7.tar", last modified: Thu Jun 22 14:54:05 2023, max compression
+gzip compressed data, was "bmw-lobster-0.9.8.tar", last modified: Tue Jun 27 13:44:47 2023, max compression
```

## Comparing `bmw-lobster-0.9.7.tar` & `bmw-lobster-0.9.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.965278 bmw-lobster-0.9.7/
--rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-22 14:54:05.965278 bmw-lobster-0.9.7/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1142 2023-06-13 09:17:37.000000 bmw-lobster-0.9.7/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.965278 bmw-lobster-0.9.7/bmw_lobster.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-22 14:54:05.000000 bmw-lobster-0.9.7/bmw_lobster.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-22 14:54:05.000000 bmw-lobster-0.9.7/bmw_lobster.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:05.000000 bmw-lobster-0.9.7/bmw_lobster.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-22 14:54:05.000000 bmw-lobster-0.9.7/bmw_lobster.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:05.000000 bmw-lobster-0.9.7/bmw_lobster.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-22 14:54:05.965278 bmw-lobster-0.9.7/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-06-13 09:17:37.000000 bmw-lobster-0.9.7/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1379 2023-06-27 13:44:26.000000 bmw-lobster-0.9.8/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/bmw_lobster.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2316 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:47.000000 bmw-lobster-0.9.8/bmw_lobster.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:47.062434 bmw-lobster-0.9.8/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2511 2023-06-27 13:44:26.000000 bmw-lobster-0.9.8/setup.py
```

### Comparing `bmw-lobster-0.9.7/PKG-INFO` & `bmw-lobster-0.9.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.7
+Version: 0.9.8
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -33,12 +33,17 @@
 * [bmw-lobster-tool-cpp](https://pypi.org/project/bmw-lobster-tool-cpp)
 * [bmw-lobster-tool-gtest](https://pypi.org/project/bmw-lobster-tool-gtest)
 * [bmw-lobster-tool-json](https://pypi.org/project/bmw-lobster-tool-json)
 * [bmw-lobster-tool-python](https://pypi.org/project/bmw-lobster-tool-python)
 * [bmw-lobster-tool-trlc](https://pypi.org/project/bmw-lobster-tool-trlc)
 * [miss_hit](https://pypi.org/project/miss_hit)
 
+Note there is also a monolithic wheel
+[bmw-lobster-monolithic](https://pypi.org/project/bmw-lobster-monolithic),
+which may be interesting for people who wish to integrate into bazel,
+as `py_wheel` cannot deal with overlapping installs.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
```

### Comparing `bmw-lobster-0.9.7/README.md` & `bmw-lobster-0.9.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -13,12 +13,17 @@
 * [bmw-lobster-tool-cpp](https://pypi.org/project/bmw-lobster-tool-cpp)
 * [bmw-lobster-tool-gtest](https://pypi.org/project/bmw-lobster-tool-gtest)
 * [bmw-lobster-tool-json](https://pypi.org/project/bmw-lobster-tool-json)
 * [bmw-lobster-tool-python](https://pypi.org/project/bmw-lobster-tool-python)
 * [bmw-lobster-tool-trlc](https://pypi.org/project/bmw-lobster-tool-trlc)
 * [miss_hit](https://pypi.org/project/miss_hit)
 
+Note there is also a monolithic wheel
+[bmw-lobster-monolithic](https://pypi.org/project/bmw-lobster-monolithic),
+which may be interesting for people who wish to integrate into bazel,
+as `py_wheel` cannot deal with overlapping installs.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
```

### Comparing `bmw-lobster-0.9.7/bmw_lobster.egg-info/PKG-INFO` & `bmw-lobster-0.9.8/bmw_lobster.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.7
+Version: 0.9.8
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -33,12 +33,17 @@
 * [bmw-lobster-tool-cpp](https://pypi.org/project/bmw-lobster-tool-cpp)
 * [bmw-lobster-tool-gtest](https://pypi.org/project/bmw-lobster-tool-gtest)
 * [bmw-lobster-tool-json](https://pypi.org/project/bmw-lobster-tool-json)
 * [bmw-lobster-tool-python](https://pypi.org/project/bmw-lobster-tool-python)
 * [bmw-lobster-tool-trlc](https://pypi.org/project/bmw-lobster-tool-trlc)
 * [miss_hit](https://pypi.org/project/miss_hit)
 
+Note there is also a monolithic wheel
+[bmw-lobster-monolithic](https://pypi.org/project/bmw-lobster-monolithic),
+which may be interesting for people who wish to integrate into bazel,
+as `py_wheel` cannot deal with overlapping installs.
+
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
```

### Comparing `bmw-lobster-0.9.7/setup.py` & `bmw-lobster-0.9.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
 gh_root = "https://github.com"
 gh_project = "bmw-software-engineering/lobster"
 
 with open("README.md", "r") as fd:
     long_description = fd.read()
 
+with open("requirements", "r") as fd:
+    package_requirements = [line
+                            for line in fd.read().splitlines()
+                            if line.strip()]
+
 # For the readme to look right on PyPI we need to translate any
 # relative links to absolute links to github.
 fixes = []
 for match in re.finditer(r"\[(.*)\]\((.*)\)", long_description):
     if not match.group(2).startswith("http"):
         fixes.append((match.span(0)[0], match.span(0)[1],
                       "[%s](%s/%s/blob/main/%s)" % (match.group(1),
@@ -36,15 +41,15 @@
     "Source Code"   : "%s/%s"        % (gh_root, gh_project),
 }
 
 packages = ["bmw-lobster-core>=%s" % version.LOBSTER_VERSION]
 for dirname in glob.glob("../lobster-tool-*"):
     packages.append("bmw-%s>=%s" % (os.path.basename(dirname),
                                     version.LOBSTER_VERSION))
-packages.append("miss-hit>=0.9.41")
+packages += package_requirements
 
 setuptools.setup(
     name="bmw-lobster",
     version=version.LOBSTER_VERSION,
     author="Bayerische Motoren Werke Aktiengesellschaft (BMW AG)",
     author_email="florian.schanda@bmw.de",
     description="Metapackage to install all LOBSTER Tools",
```

