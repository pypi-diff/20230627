# Comparing `tmp/bmw-lobster-core-0.9.7.tar.gz` & `tmp/bmw-lobster-core-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.7.tar", last modified: Thu Jun 22 14:54:03 2023, max compression
+gzip compressed data, was "bmw-lobster-core-0.9.8.tar", last modified: Tue Jun 27 13:44:44 2023, max compression
```

## Comparing `bmw-lobster-core-0.9.7.tar` & `bmw-lobster-core-0.9.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.813240 bmw-lobster-core-0.9.7/
--rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-22 14:54:03.813240 bmw-lobster-core-0.9.7/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1735 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.7/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.809239 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      705 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.809239 bmw-lobster-core-0.9.7/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.809239 bmw-lobster-core-0.9.7/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.809239 bmw-lobster-core-0.9.7/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4448 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7684 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.809239 bmw-lobster-core-0.9.7/lobster/tools/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.813240 bmw-lobster-core-0.9.7/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     2142 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/tools/core/report.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-22 14:54:03.000000 bmw-lobster-core-0.9.7/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-22 14:54:03.813240 bmw-lobster-core-0.9.7/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2545 2023-06-22 14:53:06.000000 bmw-lobster-core-0.9.7/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1735 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.8/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.966397 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      705 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.966397 bmw-lobster-core-0.9.8/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.966397 bmw-lobster-core-0.9.8/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4448 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7684 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/lobster/tools/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     2142 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/tools/core/report.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-27 13:44:44.000000 bmw-lobster-core-0.9.8/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-27 13:44:44.970397 bmw-lobster-core-0.9.8/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2611 2023-06-27 13:44:26.000000 bmw-lobster-core-0.9.8/setup.py
```

### Comparing `bmw-lobster-core-0.9.7/PKG-INFO` & `bmw-lobster-core-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.7
+Version: 0.9.8
 Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.7/README.md` & `bmw-lobster-core-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/PKG-INFO` & `bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.7
+Version: 0.9.8
 Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.7/bmw_lobster_core.egg-info/SOURCES.txt` & `bmw-lobster-core-0.9.8/bmw_lobster_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/config/lexer.py` & `bmw-lobster-core-0.9.8/lobster/config/lexer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/config/parser.py` & `bmw-lobster-core-0.9.8/lobster/config/parser.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/errors.py` & `bmw-lobster-core-0.9.8/lobster/errors.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/exceptions.py` & `bmw-lobster-core-0.9.8/lobster/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/html/assets.py` & `bmw-lobster-core-0.9.8/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/html/htmldoc.py` & `bmw-lobster-core-0.9.8/lobster/html/htmldoc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/io.py` & `bmw-lobster-core-0.9.8/lobster/io.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/items.py` & `bmw-lobster-core-0.9.8/lobster/items.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/location.py` & `bmw-lobster-core-0.9.8/lobster/location.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/report.py` & `bmw-lobster-core-0.9.8/lobster/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/tools/core/ci_report.py` & `bmw-lobster-core-0.9.8/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/tools/core/html_report.py` & `bmw-lobster-core-0.9.8/lobster/tools/core/html_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/tools/core/online_report.py` & `bmw-lobster-core-0.9.8/lobster/tools/core/online_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/tools/core/report.py` & `bmw-lobster-core-0.9.8/lobster/tools/core/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.7/lobster/version.py` & `bmw-lobster-core-0.9.8/lobster/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 7)
+VERSION_TUPLE = (0, 9, 8)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-core-0.9.7/setup.py` & `bmw-lobster-core-0.9.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 
 gh_root = "https://github.com"
 gh_project = "bmw-software-engineering/lobster"
 
 with open("README.md", "r") as fd:
     long_description = fd.read()
 
+with open("requirements", "r") as fd:
+    package_requirements = [line
+                            for line in fd.read().splitlines()
+                            if line.strip()]
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
@@ -46,26 +55,21 @@
     project_urls=project_urls,
     license="GNU Affero General Public License v3",
     packages=["lobster",
               "lobster.config",
               "lobster.html",
               "lobster.tools",
               "lobster.tools.core"],
-    install_requires=[],
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
-            "lobster-report = lobster.tools.core.report:main",
-            "lobster-html-report = lobster.tools.core.html_report:main",
-            "lobster-online-report = lobster.tools.core.online_report:main",
-            "lobster-ci-report = lobster.tools.core.ci_report:main",
-        ],
+        "console_scripts": entrypoints
     },
 )
```

