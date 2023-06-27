# Comparing `tmp/databricks_session-0.0.2.tar.gz` & `tmp/databricks_session-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_session-0.0.2.tar", last modified: Tue Jun 27 00:47:22 2023, max compression
+gzip compressed data, was "databricks_session-0.1.8.tar", last modified: Tue Jun 27 03:08:02 2023, max compression
```

## Comparing `databricks_session-0.0.2.tar` & `databricks_session-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:47:22.738523 databricks_session-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 00:47:12.000000 databricks_session-0.0.2/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-27 00:47:12.000000 databricks_session-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 00:47:12.000000 databricks_session-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-27 00:47:12.000000 databricks_session-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-27 00:47:12.000000 databricks_session-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 00:47:12.000000 databricks_session-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 00:47:12.000000 databricks_session-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 00:47:12.000000 databricks_session-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-27 00:47:22.738523 databricks_session-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-27 00:47:12.000000 databricks_session-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 00:47:12.000000 databricks_session-0.0.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:47:22.738523 databricks_session-0.0.2/databricks_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 00:47:22.000000 databricks_session-0.0.2/databricks_session.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 00:47:12.000000 databricks_session-0.0.2/databricks_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 00:47:12.000000 databricks_session-0.0.2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 00:47:12.000000 databricks_session-0.0.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 00:47:12.000000 databricks_session-0.0.2/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 00:47:12.000000 databricks_session-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 00:47:12.000000 databricks_session-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 00:47:22.738523 databricks_session-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-27 00:47:12.000000 databricks_session-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:08:02.505553 databricks_session-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 03:07:46.000000 databricks_session-0.1.8/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-27 03:07:46.000000 databricks_session-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-27 03:07:46.000000 databricks_session-0.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 03:07:46.000000 databricks_session-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 03:07:46.000000 databricks_session-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 03:07:46.000000 databricks_session-0.1.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 03:08:02.505553 databricks_session-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-27 03:07:46.000000 databricks_session-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 03:07:46.000000 databricks_session-0.1.8/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:08:02.505553 databricks_session-0.1.8/databricks_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 03:08:02.000000 databricks_session-0.1.8/databricks_session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 03:07:46.000000 databricks_session-0.1.8/databricks_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 03:07:46.000000 databricks_session-0.1.8/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 03:07:46.000000 databricks_session-0.1.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:07:46.000000 databricks_session-0.1.8/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 03:07:46.000000 databricks_session-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 03:07:46.000000 databricks_session-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 03:08:02.505553 databricks_session-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 03:07:46.000000 databricks_session-0.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 03:07:46.000000 databricks_session-0.1.8/version.py
```

### Comparing `databricks_session-0.0.2/.gitignore` & `databricks_session-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/CODE_OF_CONDUCT.md` & `databricks_session-0.1.8/CODE_OF_CONDUCT.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 the behavior directly with those involved. Many issues can be resolved quickly
 and easily, and this gives people more control over the outcome of their
 dispute. If you are unable to resolve the matter for any reason, or if the
 behavior is threatening or harassing, report it. We are dedicated to providing
 an environment where participants feel welcome and safe.
 
 
-Reports should be directed to *support@occlusion.solutions*, the
-Project Steward(s) for *Occlusion LLM Explorer*. It is the Project Steward’s duty to
+Reports should be directed to *carlosdavidescobar@gmail.com*, the
+Project Steward(s) for *Databricks Session*. It is the Project Steward’s duty to
 receive and address reported violations of the code of conduct. If for any reason you
 are uncomfortable reaching out to the Project Steward, please email
-carlos@occlusion.solutions
+carlosdavidescobar@gmail.com
 
 We will investigate every complaint, but you may not receive a direct response.
 We will use our discretion in determining when and how to follow up on reported
 incidents, which may range from not taking action to permanent expulsion from
 the project and project-sponsored spaces. We will notify the accused of the
 report and provide them an opportunity to discuss it before any action is taken.
 The identity of the reporter will be omitted from the details of the report
```

### Comparing `databricks_session-0.0.2/CONTRIBUTING.rst` & `databricks_session-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/LICENSE` & `databricks_session-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/PKG-INFO` & `databricks_session-0.1.8/databricks_session.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: databricks_session
-Version: 0.0.2
+Name: databricks-session
+Version: 0.1.8
 Summary: A simple util to get a spark and mlflow session objects from an .env file
-Home-page: https://github.com/Occlusion-Solutions/databricks_session.git
+Home-page: https://github.com/Broomva/databricks_session
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
-Classifier: Programming Language :: Python :: 3
+License: MIT
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: protobuf
 License-File: LICENSE
 
 # Databricks Session Util
 **A simple utility for spark and mlflow session objects**
 
 
 ## Setup
```

### Comparing `databricks_session-0.0.2/README.md` & `databricks_session-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/SECURITY.md` & `databricks_session-0.1.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/databricks_session.egg-info/PKG-INFO` & `databricks_session-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: databricks-session
-Version: 0.0.2
+Name: databricks_session
+Version: 0.1.8
 Summary: A simple util to get a spark and mlflow session objects from an .env file
-Home-page: https://github.com/Occlusion-Solutions/databricks_session.git
+Home-page: https://github.com/Broomva/databricks_session
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
-Classifier: Programming Language :: Python :: 3
+License: MIT
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: protobuf
 License-File: LICENSE
 
 # Databricks Session Util
 **A simple utility for spark and mlflow session objects**
 
 
 ## Setup
```

### Comparing `databricks_session-0.0.2/databricks_session.egg-info/SOURCES.txt` & `databricks_session-0.1.8/databricks_session.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 main.py
 package.json
 pip.conf
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
+version.py
 databricks_session.egg-info/PKG-INFO
 databricks_session.egg-info/SOURCES.txt
 databricks_session.egg-info/dependency_links.txt
 databricks_session.egg-info/entry_points.txt
 databricks_session.egg-info/not-zip-safe
 databricks_session.egg-info/requires.txt
 databricks_session.egg-info/top_level.txt
```

### Comparing `databricks_session-0.0.2/databricks_session.egg-info/requires.txt` & `databricks_session-0.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/databricks_session.py` & `databricks_session-0.1.8/databricks_session.py`

 * *Files identical despite different names*

### Comparing `databricks_session-0.0.2/requirements.txt` & `databricks_session-0.1.8/databricks_session.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -68,7 +68,10 @@
 threadpoolctl==3.1.0
 typing_extensions==4.6.3
 tzdata==2023.3
 urllib3==1.26.16
 websocket-client==1.6.1
 Werkzeug==2.3.6
 zipp==3.15.0
+
+[protobuf]
+protobuf<5.0.0dev
```

### Comparing `databricks_session-0.0.2/setup.py` & `databricks_session-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,20 @@
+import io
+import os
+import setuptools
 import glob
-import re
 import sys
+from setuptools import find_packages, find_namespace_packages
 
-from setuptools import find_packages, setup
-
-if sys.version_info < (3, 10):
-    print("Error: databricks_session does not support this version of Python.")
-    print("Please upgrade to Python 3.10 or higher.")
-    sys.exit(1)
-
-try:
-    from setuptools import find_namespace_packages
-
+if sys.version_info < (3, 8):
     find_namespace_packages()
-except ImportError:
-    # the user has a downlevel version of setuptools.
-    print("Error: databricks_session requires setuptools v40.1.0 or higher.")
-    print(
-        'Please upgrade setuptools with "pip install --upgrade setuptools" '
-        "and try again"
-    )
+    print("Error: databricks_session does not support this version of Python.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
-version = "#{PKG_VAR_SETUP}#"
-package_name = "databricks_session"
-
-package_env = re.sub(r"[^a-zA-Z]", "", version)
-
-if "PKGVARSETUP" in package_env:
-    version = "0.0.2"
-
-package_env = re.sub(r"[^a-zA-Z]", "", version)
-
-# Check if any letters were found
-if len(package_env) > 0:
-    package_name += f"_{package_env}"
-
-
-with open("requirements.txt") as f:
-    required = f.read().splitlines()
-
 
 def prepare_data_files(directory, extensions):
     files = []
     for ext in extensions:
         files.extend(glob.glob(f"{directory}/*.{ext}"))
     return files
 
@@ -54,42 +25,73 @@
         prepare_data_files(
             "databricks_session",
             ["csv", "sql", "txt", "md", "html", "css", "json", "yaml", "faiss", "pkl"],
         ),
     ),
 ]
 
-print(package_name, version)
-setup(
-    name=package_name,
+# Package metadata.
+name = "databricks_session"
+description = (
+    "A simple util to get a spark and mlflow session objects from an .env file"
+)
+# Should be one of:
+# 'Development Status :: 3 - Alpha'
+# 'Development Status :: 4 - Beta'
+# 'Development Status :: 5 - Production/Stable'
+release_status = "Development Status :: 3 - Alpha"
+
+with open("requirements.txt") as f:
+    required = f.read().splitlines()
+extras = {"protobuf": ["protobuf<5.0.0dev"]}
+
+# Setup boilerplate below this line.
+
+package_root = os.path.abspath(os.path.dirname(__file__))
+
+version = {}
+with open(os.path.join(package_root, "version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+readme_filename = os.path.join(package_root, "README.md")
+with io.open(readme_filename, encoding="utf-8") as readme_file:
+    readme = readme_file.read()
+
+setuptools.setup(
+    name=name,
     version=version,
+    description=description,
+    long_description=readme,
+    long_description_content_type="text/markdown",
     author="Carlos D. Escobar-Valbuena",
     author_email="carlosdavidescobar@gmail.com",
-    description="A simple util to get a spark and mlflow session objects from an .env file",
-    long_description=open("README.md", "r").read(),
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    include_package_data=True,
-    setup_requires=["setuptools", "wheel"],
-    tests_require=["pytest"],
-    python_requires=">=3.10",
-    nstall_requires=required,
-    test_suite="tests",
-    zip_safe=False,
-    url="https://github.com/Occlusion-Solutions/databricks_session.git",
+    license="MIT",
     classifiers=[
-        "Programming Language :: Python :: 3",
+        release_status,
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    packages=find_packages(),
     install_requires=required,
+    extras_require=extras,
+    python_requires=">=3.8",
+    include_package_data=True,
+    setup_requires=["setuptools", "wheel"],
+    tests_require=["pytest"],
+    test_suite="tests",
+    zip_safe=False,
+    url="https://github.com/Broomva/databricks_session",
     package_data={
         "databricks_session": [
             "*.json",
             "*.yaml",
             "*.sql",
             "*.csv",
             "*.txt",
```

