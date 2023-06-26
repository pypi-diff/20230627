# Comparing `tmp/telexy.sam-1.23.628.tar.gz` & `tmp/telexy.sam-1.23.629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexy.sam-1.23.628.tar", last modified: Mon Jun 26 22:08:24 2023, max compression
+gzip compressed data, was "telexy.sam-1.23.629.tar", last modified: Mon Jun 26 22:37:27 2023, max compression
```

## Comparing `telexy.sam-1.23.628.tar` & `telexy.sam-1.23.629.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 22:08:24.809396 telexy.sam-1.23.628/
--rw-rw-rw-   0        0        0     1076 2023-06-21 03:48:56.000000 telexy.sam-1.23.628/LICENSE.txt
--rw-rw-rw-   0        0        0      416 2023-06-26 22:08:24.808396 telexy.sam-1.23.628/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-06-21 14:45:02.000000 telexy.sam-1.23.628/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 22:08:24.798884 telexy.sam-1.23.628/sam/
--rw-rw-rw-   0        0        0       19 2023-06-26 20:43:53.000000 telexy.sam-1.23.628/sam/__init__.py
--rw-rw-rw-   0        0        0      106 2023-06-26 20:48:13.000000 telexy.sam-1.23.628/sam/sam.py
--rw-rw-rw-   0        0        0       42 2023-06-26 22:08:24.809396 telexy.sam-1.23.628/setup.cfg
--rw-rw-rw-   0        0        0     1855 2023-06-26 22:08:07.000000 telexy.sam-1.23.628/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:08:24.806398 telexy.sam-1.23.628/telexy.sam.egg-info/
--rw-rw-rw-   0        0        0      416 2023-06-26 22:08:24.000000 telexy.sam-1.23.628/telexy.sam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-26 22:08:24.000000 telexy.sam-1.23.628/telexy.sam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 22:08:24.000000 telexy.sam-1.23.628/telexy.sam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-26 22:08:24.000000 telexy.sam-1.23.628/telexy.sam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-26 22:08:24.000000 telexy.sam-1.23.628/telexy.sam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 22:37:27.390371 telexy.sam-1.23.629/
+-rw-rw-rw-   0        0        0     1076 2023-06-21 03:48:56.000000 telexy.sam-1.23.629/LICENSE.txt
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:37:27.389372 telexy.sam-1.23.629/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-06-21 14:45:02.000000 telexy.sam-1.23.629/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 22:37:27.390371 telexy.sam-1.23.629/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-06-26 22:37:10.000000 telexy.sam-1.23.629/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 22:37:27.388372 telexy.sam-1.23.629/telexy.sam.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:37:27.000000 telexy.sam-1.23.629/telexy.sam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-06-26 22:37:27.000000 telexy.sam-1.23.629/telexy.sam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:37:27.000000 telexy.sam-1.23.629/telexy.sam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 22:37:27.000000 telexy.sam-1.23.629/telexy.sam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-26 22:37:27.000000 telexy.sam-1.23.629/telexy.sam.egg-info/top_level.txt
```

### Comparing `telexy.sam-1.23.628/LICENSE.txt` & `telexy.sam-1.23.629/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telexy.sam-1.23.628/setup.py` & `telexy.sam-1.23.629/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,31 @@
 #To build/publish, use following commands
 #python3 setup.py sdist bdist_wheel - for build
 #python3 -m twine upload dist/* - for publish
 import setuptools
-from setuptools.command.install import install
-import importlib
-
-class PostInstallRegisterMars(install):
-    
-    def run(self):
-        install.run(self)
-        print("post installing")
-    #    module = importlib.import_module("mars")
-     #   register = getattr(module, "register")
-     #   plugin = getattr(module, "MarsApplicationRegistryPlugin")
-     #   print("hello")
-     #   register(plugin("SamPlugin", "sam", "sam"))
-
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telexy.sam",                     # This is the name of the package
-    version="1.23.628",                        # The initial release version
+    version="1.23.629",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="SAM Inference service",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.10',                # Minimum version requirement of the package
     py_modules=["sam"],             # Name of the python package
     install_requires=['telexy.mars'],                     # Install other dependencies if any
-    cmdclass={
-        'install': PostInstallRegisterMars
-    }
 )
```

