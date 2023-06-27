# Comparing `tmp/flask-allowedhosts-1.0.1.tar.gz` & `tmp/flask-allowedhosts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-allowedhosts-1.0.1.tar", last modified: Sat Jun 24 09:25:53 2023, max compression
+gzip compressed data, was "flask-allowedhosts-1.1.0.tar", last modified: Tue Jun 27 03:11:10 2023, max compression
```

## Comparing `flask-allowedhosts-1.0.1.tar` & `flask-allowedhosts-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.574751 flask-allowedhosts-1.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-24 09:14:27.000000 flask-allowedhosts-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     2953 2023-06-24 09:25:53.573752 flask-allowedhosts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1988 2023-06-24 09:15:11.000000 flask-allowedhosts-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.549752 flask-allowedhosts-1.0.1/flask_allowedhosts/
--rw-rw-rw-   0        0        0       34 2023-06-24 08:29:33.000000 flask-allowedhosts-1.0.1/flask_allowedhosts/__init__.py
--rw-rw-rw-   0        0        0      486 2023-06-24 08:47:48.000000 flask-allowedhosts-1.0.1/flask_allowedhosts/decorators.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.571753 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/
--rw-rw-rw-   0        0        0     2953 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:25:53.574751 flask-allowedhosts-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-06-24 09:25:46.000000 flask-allowedhosts-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:11:10.911111 flask-allowedhosts-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-24 09:14:27.000000 flask-allowedhosts-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     2936 2023-06-27 03:11:10.910111 flask-allowedhosts-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1971 2023-06-27 02:34:52.000000 flask-allowedhosts-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 03:11:10.881110 flask-allowedhosts-1.1.0/flask_allowedhosts/
+-rw-rw-rw-   0        0        0       59 2023-06-27 03:08:35.000000 flask-allowedhosts-1.1.0/flask_allowedhosts/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-06-27 03:02:04.000000 flask-allowedhosts-1.1.0/flask_allowedhosts/decorators.py
+-rw-rw-rw-   0        0        0      265 2023-06-27 03:02:48.000000 flask-allowedhosts-1.1.0/flask_allowedhosts/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:11:10.908111 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/
+-rw-rw-rw-   0        0        0     2936 2023-06-27 03:11:10.000000 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-27 03:11:10.000000 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 03:11:10.000000 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 03:11:10.000000 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 03:11:10.000000 flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 03:11:10.911111 flask-allowedhosts-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-06-27 02:43:43.000000 flask-allowedhosts-1.1.0/setup.py
```

### Comparing `flask-allowedhosts-1.0.1/LICENSE.md` & `flask-allowedhosts-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-allowedhosts-1.0.1/PKG-INFO` & `flask-allowedhosts-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-allowedhosts
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Flask extension to limit access to your routes by using allowed hosts.
 Home-page: https://github.com/riad-azz/flask-allowedhosts
 Author: Riadh Azzoun
 Author-email: riadh.azzoun@hotmail.com
 License: MIT
 Keywords: flask,allowed hosts,web development,security
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,18 +45,18 @@
 ```python
 app = Flask(__name__)
 ```
 
 3. Define the list of allowed hosts:
 
 ```python
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 ```
 
-4. Apply the check_host decorator to the desired endpoint(s):
+4. Apply the `@check_host` decorator to the desired endpoint(s):
 
 ```python
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
@@ -69,15 +69,15 @@
 
 ```python
 from flask import Flask, request, jsonify
 from flask_allowedhosts import check_host
 
 app = Flask(__name__)
 
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
     return jsonify(greeting), 200
```

### Comparing `flask-allowedhosts-1.0.1/README.md` & `flask-allowedhosts-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 ```python
 app = Flask(__name__)
 ```
 
 3. Define the list of allowed hosts:
 
 ```python
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 ```
 
-4. Apply the check_host decorator to the desired endpoint(s):
+4. Apply the `@check_host` decorator to the desired endpoint(s):
 
 ```python
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
@@ -48,15 +48,15 @@
 
 ```python
 from flask import Flask, request, jsonify
 from flask_allowedhosts import check_host
 
 app = Flask(__name__)
 
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
     return jsonify(greeting), 200
```

### Comparing `flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/PKG-INFO` & `flask-allowedhosts-1.1.0/flask_allowedhosts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-allowedhosts
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Flask extension to limit access to your routes by using allowed hosts.
 Home-page: https://github.com/riad-azz/flask-allowedhosts
 Author: Riadh Azzoun
 Author-email: riadh.azzoun@hotmail.com
 License: MIT
 Keywords: flask,allowed hosts,web development,security
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,18 +45,18 @@
 ```python
 app = Flask(__name__)
 ```
 
 3. Define the list of allowed hosts:
 
 ```python
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 ```
 
-4. Apply the check_host decorator to the desired endpoint(s):
+4. Apply the `@check_host` decorator to the desired endpoint(s):
 
 ```python
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
@@ -69,15 +69,15 @@
 
 ```python
 from flask import Flask, request, jsonify
 from flask_allowedhosts import check_host
 
 app = Flask(__name__)
 
-ALLOWED_HOSTS = ['127.0.0.1:5000', 'localhost:5000']
+ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 
 @app.route("/api")
 @check_host(allowed_hosts=ALLOWED_HOSTS)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
     return jsonify(greeting), 200
```

### Comparing `flask-allowedhosts-1.0.1/setup.py` & `flask-allowedhosts-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 long_description = open('README.md').read()
 long_description_content_type = 'text/markdown'
 
 setup(
     name='flask-allowedhosts',
-    version='1.0.1',
+    version='1.1.0',
     packages=['flask_allowedhosts'],
     install_requires=[
         'Flask',
     ],
     url='https://github.com/riad-azz/flask-allowedhosts',
     license='MIT',
     author='Riadh Azzoun',
```

