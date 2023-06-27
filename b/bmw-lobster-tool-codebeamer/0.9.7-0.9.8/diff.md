# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.7.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.7.tar", last modified: Thu Jun 22 14:54:04 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.8.tar", last modified: Tue Jun 27 13:44:45 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.7.tar` & `bmw-lobster-tool-codebeamer-0.9.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.7/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    10398 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.7/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.8/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    10398 2023-06-27 13:44:45.000000 bmw-lobster-tool-codebeamer-0.9.8/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:45.590408 bmw-lobster-tool-codebeamer-0.9.8/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2558 2023-06-27 13:44:26.000000 bmw-lobster-tool-codebeamer-0.9.8/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.7/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.7
+Version: 0.9.8
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.7/README.md` & `bmw-lobster-tool-codebeamer-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.8/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.7
+Version: 0.9.8
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.8/lobster/tools/codebeamer/codebeamer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.7/setup.py` & `bmw-lobster-tool-codebeamer-0.9.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 
 gh_root = "https://github.com"
 gh_project = "bmw-software-engineering/lobster"
 
 with open("README.md", "r") as fd:
     long_description = fd.read()
 
+with open("requirements", "r") as fd:
+    package_requirements = [line
+                            for line in fd.read().splitlines()
+                            if line.strip()]
+package_requirements.append("bmw-lobster-core>=%s" % version.LOBSTER_VERSION)
+with open("entrypoints", "r") as fd:
+    entrypoints = [line
+                   for line in fd.read().splitlines()
+                   if line.strip()]
+
 # For the readme to look right on PyPI we need to translate any
 # relative links to absolute links to github.
 fixes = []
 for match in re.finditer(r"\[(.*)\]\((.*)\)", long_description):
     if not match.group(2).startswith("http"):
         fixes.append((match.span(0)[0], match.span(0)[1],
                       "[%s](%s/%s/blob/main/%s)" % (match.group(1),
@@ -42,26 +52,21 @@
     description="LOBSTER Tool for Codebeamer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=project_urls["Source Code"],
     project_urls=project_urls,
     license="GNU Affero General Public License v3",
     packages=["lobster.tools.codebeamer"],
-    install_requires=[
-        "bmw-lobster-core>=%s" % version.LOBSTER_VERSION,
-        "requests>=2.22"
-    ],
+    install_requires=package_requirements,
     python_requires=">=3.7, <4",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Topic :: Documentation",
         "Topic :: Software Development",
     ],
     entry_points={
-        "console_scripts": [
-            "lobster-codebeamer = lobster.tools.codebeamer.codebeamer:main",
-        ],
+        "console_scripts": entrypoints,
     },
 )
```

