# Comparing `tmp/morss-20230625.2341.tar.gz` & `tmp/morss-20230627.2033.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morss-20230625.2341.tar", last modified: Sun Jun 25 23:41:02 2023, max compression
+gzip compressed data, was "morss-20230627.2033.tar", last modified: Tue Jun 27 20:33:22 2023, max compression
```

## Comparing `morss-20230625.2341.tar` & `morss-20230627.2033.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-06-25 23:40:52.000000 morss-20230625.2341/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17665 2023-06-25 23:41:02.696956 morss-20230625.2341/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17228 2023-06-25 23:40:52.000000 morss-20230625.2341/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.692956 morss-20230625.2341/morss/
--rw-r--r--   0 root         (0) root         (0)      869 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/caching.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/cli.py
--rw-r--r--   0 root         (0) root         (0)    22734 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/crawler.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/feedify.ini
--rw-r--r--   0 root         (0) root         (0)    23557 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/feeds.py
--rw-r--r--   0 root         (0) root         (0)    12447 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/morss.py
--rw-r--r--   0 root         (0) root         (0)    11496 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/readabilite.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/util.py
--rw-r--r--   0 root         (0) root         (0)     8484 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/wsgi.py
--rwxr-xr-x   0 root         (0) root         (0)      822 2023-06-25 23:40:52.000000 morss-20230625.2341/morss-helper
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/morss.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17665 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 23:41:02.696956 morss-20230625.2341/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-25 23:40:52.000000 morss-20230625.2341/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/tests/
--rw-r--r--   0 root         (0) root         (0)     3516 2023-06-25 23:40:52.000000 morss-20230625.2341/tests/test_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-25 23:40:52.000000 morss-20230625.2341/tests/test_feeds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/www/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-25 23:40:52.000000 morss-20230625.2341/www/index.html
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-25 23:40:52.000000 morss-20230625.2341/www/logo.svg
--rw-r--r--   0 root         (0) root         (0)     8258 2023-06-25 23:40:52.000000 morss-20230625.2341/www/sheet.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 20:33:22.585931 morss-20230627.2033/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-06-27 20:33:11.000000 morss-20230627.2033/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17665 2023-06-27 20:33:22.585931 morss-20230627.2033/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17228 2023-06-27 20:33:11.000000 morss-20230627.2033/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 20:33:22.581931 morss-20230627.2033/morss/
+-rw-r--r--   0 root         (0) root         (0)      900 2023-06-27 20:33:22.000000 morss-20230627.2033/morss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/caching.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/cli.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/crawler.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/feedify.ini
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/feeds.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/morss.py
+-rw-r--r--   0 root         (0) root         (0)    11496 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/readabilite.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/util.py
+-rw-r--r--   0 root         (0) root         (0)     8484 2023-06-27 20:33:11.000000 morss-20230627.2033/morss/wsgi.py
+-rwxr-xr-x   0 root         (0) root         (0)      822 2023-06-27 20:33:11.000000 morss-20230627.2033/morss-helper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 20:33:22.585931 morss-20230627.2033/morss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17665 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 20:33:22.000000 morss-20230627.2033/morss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 20:33:22.585931 morss-20230627.2033/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-27 20:33:11.000000 morss-20230627.2033/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 20:33:22.585931 morss-20230627.2033/tests/
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-06-27 20:33:11.000000 morss-20230627.2033/tests/test_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-27 20:33:11.000000 morss-20230627.2033/tests/test_feeds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 20:33:22.585931 morss-20230627.2033/www/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-27 20:33:11.000000 morss-20230627.2033/www/index.html
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-27 20:33:11.000000 morss-20230627.2033/www/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-06-27 20:33:11.000000 morss-20230627.2033/www/sheet.xsl
```

### Comparing `morss-20230625.2341/LICENSE` & `morss-20230627.2033/LICENSE`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/PKG-INFO` & `morss-20230627.2033/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20230625.2341
+Version: 20230627.2033
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
```

### Comparing `morss-20230625.2341/README.md` & `morss-20230627.2033/README.md`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/__init__.py` & `morss-20230627.2033/morss/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,9 +15,11 @@
 # You should have received a copy of the GNU Affero General Public License along
 # with this program. If not, see <https://www.gnu.org/licenses/>.
 
 # ran on `import morss`
 
 # pylint: disable=unused-import,unused-variable
 
+__version__ = "20230627.2033"
+
 from .morss import *
 from .wsgi import application
```

### Comparing `morss-20230625.2341/morss/__main__.py` & `morss-20230627.2033/morss/__main__.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/caching.py` & `morss-20230627.2033/morss/caching.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/cli.py` & `morss-20230627.2033/morss/cli.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/crawler.py` & `morss-20230627.2033/morss/crawler.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/feedify.ini` & `morss-20230627.2033/morss/feedify.ini`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/feeds.py` & `morss-20230627.2033/morss/feeds.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/morss.py` & `morss-20230627.2033/morss/morss.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/readabilite.py` & `morss-20230627.2033/morss/readabilite.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/util.py` & `morss-20230627.2033/morss/util.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss/wsgi.py` & `morss-20230627.2033/morss/wsgi.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss-helper` & `morss-20230627.2033/morss-helper`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/morss.egg-info/PKG-INFO` & `morss-20230627.2033/morss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20230625.2341
+Version: 20230627.2033
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
```

### Comparing `morss-20230625.2341/setup.py` & `morss-20230627.2033/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 from datetime import datetime
 from glob import glob
 
 from setuptools import setup
 
+def get_version():
+    with open('morss/__init__.py', 'r+') as file:
+        lines = file.readlines()
+
+        # look for hard coded version number
+        for i in range(len(lines)):
+            if lines[i].startswith('__version__'):
+                version = lines[i].split('"')[1]
+                break
+
+        # create (& save) one if none found
+        if version == '':
+            version = datetime.now().strftime('%Y%m%d.%H%M')
+            lines[i] = '__version__ = "' + version + '"\n'
+
+            file.seek(0)
+            file.writelines(lines)
+
+        # return version number
+        return version
+
 package_name = 'morss'
 
 setup(
     name = package_name,
-    version = datetime.now().strftime('%Y%m%d.%H%M'),
+    version = get_version(),
     description = 'Get full-text RSS feeds',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     author = 'pictuga',
     author_email = 'contact@pictuga.com',
     url = 'http://morss.it/',
     project_urls = {
```

### Comparing `morss-20230625.2341/tests/test_crawler.py` & `morss-20230627.2033/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/tests/test_feeds.py` & `morss-20230627.2033/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/www/index.html` & `morss-20230627.2033/www/index.html`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/www/logo.svg` & `morss-20230627.2033/www/logo.svg`

 * *Files identical despite different names*

### Comparing `morss-20230625.2341/www/sheet.xsl` & `morss-20230627.2033/www/sheet.xsl`

 * *Files identical despite different names*

