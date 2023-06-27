# Comparing `tmp/bkapi-plugins-py-0.625.tar.gz` & `tmp/bkapi-plugins-py-0.627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.625.tar", last modified: Sun Jun 25 03:06:45 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.627.tar", last modified: Tue Jun 27 11:50:53 2023, max compression
```

## Comparing `bkapi-plugins-py-0.625.tar` & `bkapi-plugins-py-0.627.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.417015 bkapi-plugins-py-0.625/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-06-13 13:44:28.000000 bkapi-plugins-py-0.625/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      181 2023-06-25 03:06:45.417015 bkapi-plugins-py-0.625/PKG-INFO
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.397015 bkapi-plugins-py-0.625/bkapi_plugins/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      169 2023-06-13 13:44:28.000000 bkapi-plugins-py-0.625/bkapi_plugins/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.401015 bkapi-plugins-py-0.625/bkapi_plugins/files/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  8943406 2023-06-25 03:05:22.000000 bkapi-plugins-py-0.625/bkapi_plugins/files/grafana-mongodb-datasource-1.8.3.linux_amd64.zip
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.417015 bkapi-plugins-py-0.625/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      181 2023-06-25 03:06:45.000000 bkapi-plugins-py-0.625/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      357 2023-06-25 03:06:45.000000 bkapi-plugins-py-0.625/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-25 03:06:45.000000 bkapi-plugins-py-0.625/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2023-06-25 03:06:45.000000 bkapi-plugins-py-0.625/bkapi_plugins_py.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.393015 bkapi-plugins-py-0.625/build/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.397015 bkapi-plugins-py-0.625/build/lib/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-25 03:06:45.397015 bkapi-plugins-py-0.625/build/lib/bkapi_plugins/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      169 2023-06-13 13:44:28.000000 bkapi-plugins-py-0.625/build/lib/bkapi_plugins/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      867 2023-06-13 13:44:28.000000 bkapi-plugins-py-0.625/build/lib/setup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-25 03:06:45.421015 bkapi-plugins-py-0.625/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      863 2023-06-25 03:06:11.000000 bkapi-plugins-py-0.625/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:50:53.259227 bkapi-plugins-py-0.627/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.627/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-06-27 11:50:53.259723 bkapi-plugins-py-0.627/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 11:50:53.242477 bkapi-plugins-py-0.627/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:50:53.250336 bkapi-plugins-py-0.627/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0   336586 2023-06-27 11:45:52.000000 bkapi-plugins-py-0.627/bkapi_plugins/files/mychart.tgz
+drwxrwxrwx   0        0        0        0 2023-06-27 11:50:53.257734 bkapi-plugins-py-0.627/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-06-27 11:50:53.000000 bkapi-plugins-py-0.627/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-27 11:50:53.000000 bkapi-plugins-py-0.627/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:50:53.000000 bkapi-plugins-py-0.627/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:50:53.000000 bkapi-plugins-py-0.627/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:50:53.260712 bkapi-plugins-py-0.627/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-27 11:50:46.000000 bkapi-plugins-py-0.627/setup.py
```

### Comparing `bkapi-plugins-py-0.625/build/lib/setup.py` & `bkapi-plugins-py-0.627/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_namespace_packages
-
-
-readme = ''
-
-setup(
-    description='',
-    long_description=readme,
-    name='bkapi-plugins-py', # 包的名字
-    version='0.5121714', # 版本号每次打包完要改一下
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
-    author='fadewalk',
-    license='Apach License 2.0',
-    # packages=find_packages(),
-    # namespace_packages=['bkapi_plugins'],
-    package_dir={'': '.'},
-    include_package_data=True,
-    package_data={ # 包的数据，可以不写
-        # 'bkapi_plugins': ['data.zip','generator1.0.tar.gz'],
-        # 'bkapi_plugins': ['generator1.0.tar.gz'],
-    },
-    #  packages= find_namespace_packages(
-    #             include=["bkapi_plugins", "bkapi_plugins.*"], ),
-    # install_requires=[
-    #     'bkapi-client-core>=1.1.0,<2.0.0',
-    # ],
-)
+from setuptools import setup, find_namespace_packages
+
+
+readme = ''
+
+setup(
+    description='',
+    long_description=readme,
+    name='bkapi-plugins-py', # 包的名字
+    version='0.627', # 版本号每次打包完要改一下
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
+    author='fadewalk',
+    license='Apach License 2.0',
+    # packages=find_packages(),
+    # namespace_packages=['bkapi_plugins'],
+    package_dir={'': '.'},
+    include_package_data=True,
+    package_data={ # 包的数据，可以不写
+        # 'bkapi_plugins': ['data.zip','generator1.0.tar.gz'],
+        # 'bkapi_plugins': ['generator1.0.tar.gz'],
+    },
+    #  packages= find_namespace_packages(
+    #             include=["bkapi_plugins", "bkapi_plugins.*"], ),
+    # install_requires=[
+    #     'bkapi-client-core>=1.1.0,<2.0.0',
+    # ],
+)
```

