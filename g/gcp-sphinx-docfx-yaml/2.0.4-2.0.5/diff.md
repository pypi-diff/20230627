# Comparing `tmp/gcp-sphinx-docfx-yaml-2.0.4.tar.gz` & `tmp/gcp-sphinx-docfx-yaml-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-sphinx-docfx-yaml-2.0.4.tar", last modified: Sat Jun  3 00:55:07 2023, max compression
+gzip compressed data, was "gcp-sphinx-docfx-yaml-2.0.5.tar", last modified: Tue Jun 27 06:58:08 2023, max compression
```

## Comparing `gcp-sphinx-docfx-yaml-2.0.4.tar` & `gcp-sphinx-docfx-yaml-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-03 00:55:07.150530 gcp-sphinx-docfx-yaml-2.0.4/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/LICENSE
--rw-r--r--   0 root         (0)     1003      296 2023-06-03 00:55:07.150530 gcp-sphinx-docfx-yaml-2.0.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2625 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-03 00:55:07.150530 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/
--rw-rw-r--   0 root         (0)     1003      576 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/__init__.py
--rw-rw-r--   0 root         (0)     1003     1262 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/directives.py
--rw-rw-r--   0 root         (0)     1003    75619 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/extension.py
--rw-rw-r--   0 root         (0)     1003     5154 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/extract_nodes.py
--rw-rw-r--   0 root         (0)     1003    14975 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/markdown_utils.py
--rw-rw-r--   0 root         (0)     1003    20734 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/monkeypatch.py
--rw-rw-r--   0 root         (0)     1003      988 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/nodes.py
--rw-rw-r--   0 root         (0)     1003      727 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/settings.py
--rw-rw-r--   0 root         (0)     1003     1731 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/utils.py
--rw-rw-r--   0 root         (0)     1003    33366 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-03 00:55:07.150530 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/
--rw-r--r--   0 root         (0)     1003      296 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      554 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      127 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       11 2023-06-03 00:55:07.000000 gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-03 00:55:07.150530 gcp-sphinx-docfx-yaml-2.0.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     1553 2023-06-03 00:52:47.000000 gcp-sphinx-docfx-yaml-2.0.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 06:58:08.650907 gcp-sphinx-docfx-yaml-2.0.5/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/LICENSE
+-rw-r--r--   0 root         (0)     1003      296 2023-06-27 06:58:08.650907 gcp-sphinx-docfx-yaml-2.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2625 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 06:58:08.650907 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/
+-rw-rw-r--   0 root         (0)     1003      576 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1262 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/directives.py
+-rw-rw-r--   0 root         (0)     1003    75619 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/extension.py
+-rw-rw-r--   0 root         (0)     1003     5154 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/extract_nodes.py
+-rw-rw-r--   0 root         (0)     1003    14975 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/markdown_utils.py
+-rw-rw-r--   0 root         (0)     1003    20734 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/monkeypatch.py
+-rw-rw-r--   0 root         (0)     1003      988 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/nodes.py
+-rw-rw-r--   0 root         (0)     1003      727 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/settings.py
+-rw-rw-r--   0 root         (0)     1003     1731 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/utils.py
+-rw-rw-r--   0 root         (0)     1003    33366 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 06:58:08.650907 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/
+-rw-r--r--   0 root         (0)     1003      296 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      554 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      134 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       11 2023-06-27 06:58:08.000000 gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-27 06:58:08.650907 gcp-sphinx-docfx-yaml-2.0.5/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     1560 2023-06-27 06:55:43.000000 gcp-sphinx-docfx-yaml-2.0.5/setup.py
```

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/LICENSE` & `gcp-sphinx-docfx-yaml-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/README.rst` & `gcp-sphinx-docfx-yaml-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/__init__.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/directives.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/directives.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/extension.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/extension.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/extract_nodes.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/markdown_utils.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/monkeypatch.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/nodes.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/settings.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/settings.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/utils.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/docfx_yaml/writer.py` & `gcp-sphinx-docfx-yaml-2.0.5/docfx_yaml/writer.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt` & `gcp-sphinx-docfx-yaml-2.0.5/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-2.0.4/setup.py` & `gcp-sphinx-docfx-yaml-2.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 
 import codecs
 import setuptools
 
 name = 'gcp-sphinx-docfx-yaml'
 description = 'Sphinx Python Domain to DocFX YAML Generator'
-version = '2.0.4'
+version = '2.0.5'
 dependencies = [
     'black',
     'gcp-docuploader',
     'PyYAML',
     'recommonmark',
     'sphinx==4.5.0',
-    'sphinx-markdown-builder',
+    'sphinx-markdown-builder==0.5.5',
     'sphinxcontrib.napoleon',
     'unidecode',
     'wheel>=0.24.0'
 ]
 
 packages = setuptools.find_packages('.', exclude=['tests'])
```

