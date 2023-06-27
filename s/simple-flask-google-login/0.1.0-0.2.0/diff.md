# Comparing `tmp/simple-flask-google-login-0.1.0.tar.gz` & `tmp/simple-flask-google-login-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-flask-google-login-0.1.0.tar", last modified: Tue Jun 27 08:39:07 2023, max compression
+gzip compressed data, was "simple-flask-google-login-0.2.0.tar", last modified: Tue Jun 27 09:09:50 2023, max compression
```

## Comparing `simple-flask-google-login-0.1.0.tar` & `simple-flask-google-login-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 08:39:07.087971 simple-flask-google-login-0.1.0/
--rw-r--r--   0 alvinwan   (501) staff       (20)    11357 2023-06-27 07:42:50.000000 simple-flask-google-login-0.1.0/LICENSE
--rw-r--r--   0 alvinwan   (501) staff       (20)    18523 2023-06-27 08:39:07.087566 simple-flask-google-login-0.1.0/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)     5074 2023-06-27 08:38:35.000000 simple-flask-google-login-0.1.0/README.md
--rw-r--r--   0 alvinwan   (501) staff       (20)      674 2023-06-27 08:38:35.000000 simple-flask-google-login-0.1.0/pyproject.toml
--rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-06-27 08:39:07.088104 simple-flask-google-login-0.1.0/setup.cfg
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 08:39:07.085676 simple-flask-google-login-0.1.0/simple_flask_google_login/
--rw-r--r--   0 alvinwan   (501) staff       (20)     5135 2023-06-27 08:37:05.000000 simple-flask-google-login-0.1.0/simple_flask_google_login/__init__.py
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 08:39:07.087030 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/
--rw-r--r--   0 alvinwan   (501) staff       (20)    18523 2023-06-27 08:39:07.000000 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)      314 2023-06-27 08:39:07.000000 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/SOURCES.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-06-27 08:39:07.000000 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/dependency_links.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)       27 2023-06-27 08:39:07.000000 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/requires.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)       26 2023-06-27 08:39:07.000000 simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/top_level.txt
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 09:09:50.463594 simple-flask-google-login-0.2.0/
+-rw-r--r--   0 alvinwan   (501) staff       (20)    11357 2023-06-27 07:42:50.000000 simple-flask-google-login-0.2.0/LICENSE
+-rw-r--r--   0 alvinwan   (501) staff       (20)    18523 2023-06-27 09:09:50.463199 simple-flask-google-login-0.2.0/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)     5074 2023-06-27 08:38:35.000000 simple-flask-google-login-0.2.0/README.md
+-rw-r--r--   0 alvinwan   (501) staff       (20)      674 2023-06-27 09:02:32.000000 simple-flask-google-login-0.2.0/pyproject.toml
+-rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-06-27 09:09:50.463673 simple-flask-google-login-0.2.0/setup.cfg
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 09:09:50.460975 simple-flask-google-login-0.2.0/simple_flask_google_login/
+-rw-r--r--   0 alvinwan   (501) staff       (20)     5521 2023-06-27 09:07:40.000000 simple-flask-google-login-0.2.0/simple_flask_google_login/__init__.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-06-27 09:09:50.462668 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/
+-rw-r--r--   0 alvinwan   (501) staff       (20)    18523 2023-06-27 09:09:50.000000 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)      314 2023-06-27 09:09:50.000000 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/SOURCES.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-06-27 09:09:50.000000 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/dependency_links.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)       27 2023-06-27 09:09:50.000000 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/requires.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)       26 2023-06-27 09:09:50.000000 simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/top_level.txt
```

### Comparing `simple-flask-google-login-0.1.0/LICENSE` & `simple-flask-google-login-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-flask-google-login-0.1.0/PKG-INFO` & `simple-flask-google-login-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-flask-google-login
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convenience utility for implementing Google login with Flask.
 Author-email: Alvin Wan <hi@alvinwan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-flask-google-login-0.1.0/README.md` & `simple-flask-google-login-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple-flask-google-login-0.1.0/pyproject.toml` & `simple-flask-google-login-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-flask-google-login"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convenience utility for implementing Google login with Flask."
 readme = "README.md"
 authors = [{ name = "Alvin Wan", email = "hi@alvinwan.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `simple-flask-google-login-0.1.0/simple_flask_google_login/__init__.py` & `simple-flask-google-login-0.2.0/simple_flask_google_login/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     def init_app(
         self,
         app,
         login_endpoint: Union[str, None] = '/login',
         callback_endpoint: Union[str, None] = '/login/callback',
         logout_endpoint: Union[str, None] = '/logout',
+        force_https: bool = True,
     ):
         """
         Register views with the Flask app.
 
         :param login_endpoint: Path to send users to, to login
         :param callback_endpoint: Path to send users to, to finish authorization
             using the Google-provided token
@@ -73,14 +74,16 @@
         assert app is not None, 'Flask application must not be None'
         if login_endpoint is not None:
             app.add_url_rule(login_endpoint, view_func=self.login)
         if callback_endpoint is not None:
             app.add_url_rule(callback_endpoint, view_func=self.callback)
         if logout_endpoint is not None:
             app.add_url_rule(logout_endpoint, view_func=self.logout)
+        if force_https:
+            app.before_request(self.before_request)
 
     @property
     def flow(self):
         """
         Get or create a new flow instance for this client.
         """
         if not hasattr(self, '_flow'):
@@ -134,7 +137,15 @@
         return self.logout_handler()
     
     def default_logout_handler(self):
         """
         By default, after logout, simply redirect back to the homepage.
         """
         return redirect('/')
+    
+    def before_request(self):
+        """
+        NOTE: Hacking this in as we're forcing SSL below. Without this, all
+        request.{url,base_url} calls will use http incorrectly when assembling
+        oauth redirect URLs.
+        """
+        request.scheme = 'https'
```

### Comparing `simple-flask-google-login-0.1.0/simple_flask_google_login.egg-info/PKG-INFO` & `simple-flask-google-login-0.2.0/simple_flask_google_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-flask-google-login
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convenience utility for implementing Google login with Flask.
 Author-email: Alvin Wan <hi@alvinwan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

