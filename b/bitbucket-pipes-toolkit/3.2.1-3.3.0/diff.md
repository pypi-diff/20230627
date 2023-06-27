# Comparing `tmp/bitbucket-pipes-toolkit-3.2.1.tar.gz` & `tmp/bitbucket-pipes-toolkit-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitbucket-pipes-toolkit-3.2.1.tar", last modified: Wed Oct 27 10:49:15 2021, max compression
+gzip compressed data, was "dist/bitbucket-pipes-toolkit-3.3.0.tar", last modified: Tue Jun 27 08:33:46 2023, max compression
```

## Comparing `bitbucket-pipes-toolkit-3.2.1.tar` & `bitbucket-pipes-toolkit-3.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/
--rw-r--r--   0 root         (0) root         (0)     1973 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1198 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/
--rw-rw-rw-   0 root         (0) root         (0)      300 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    12620 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1973 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-27 10:49:15.000000 bitbucket-pipes-toolkit-3.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      742 2021-10-27 10:49:02.000000 bitbucket-pipes-toolkit-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6851 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14341 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/setup.py
```

### Comparing `bitbucket-pipes-toolkit-3.2.1/PKG-INFO` & `bitbucket-pipes-toolkit-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.2.1
+Version: 3.3.0
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
 License: UNKNOWN
 Description: Bitbucket Pipes Toolkit
         =========
```

### Comparing `bitbucket-pipes-toolkit-3.2.1/README.md` & `bitbucket-pipes-toolkit-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/annotations.py` & `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/annotations.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/core.py` & `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from collections.abc import MutableSequence
 import re
 from urllib.parse import urlparse
 
 import yaml
 import requests
 from cerberus import Validator
+from requests.auth import HTTPBasicAuth, AuthBase
+from yaml.scanner import ScannerError
 
 from .helpers import fail, success, configure_logger
 
 
 logger = configure_logger()
 
 
@@ -138,14 +140,25 @@
         Purge all shared data
         """
         files = glob.glob(os.path.join(self._path, '_shared_*'))
         for f in files:
             os.remove(f)
 
 
+class TokenAuth(AuthBase):
+    """Attaches auth token to the given Request object."""
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        # modify and return the request
+        r.headers['Authorization'] = 'Bearer ' + self.token
+        return r
+
+
 class Pipe:
     """Base class for all pipes. Provides utilities to work with configuration, validation etc.
 
     Attributes:
         variables (dict): Dictionary containing the pipes variables.
         schema (dict): Dictionary with the pipe parameters schema in the cerberus format.
         env (dict): Dict-like object containing pipe parameters. This is usually the environment variables that
@@ -158,14 +171,39 @@
 
     Pipe variables validation
         Pip variables validation is done at the time of initializing a pipe. The environment variables are
         validated against the schema provided. See https://docs.python-cerberus.org/en/stable/ for more
         details on how to specify schemas.
 
     """
+    def __init__(self, pipe_metadata=None, pipe_metadata_file=None, schema=None,
+                 env=None, logger=logger, check_for_newer_version=False):
+        if pipe_metadata is not None and pipe_metadata_file is not None:
+            self.fail(message="Passing both pipe_metadata and pipe_metadata_file is not allowed. "
+                              "Please use only one of them.")
+        if pipe_metadata_file is not None:
+            self.metadata = self.parse_yaml_file(filepath=pipe_metadata_file)
+        elif pipe_metadata is not None:
+            self.metadata = pipe_metadata
+        else:
+            self.metadata = {}
+
+        if env is None:
+            self.env = os.environ.copy()
+        else:
+            self.env = env
+
+        self.variables = None
+        self.schema = schema
+        self.logger = logger
+        # validate pipe parameters
+        self.variables = self.validate()
+        self.enable_debug_log_level()
+        if check_for_newer_version:
+            self.check_for_newer_version()
 
     def fail(self, message, print_community_link=False):
         """Fail the pipe and exit.
 
         Args:
             message (str): Error message to show.
             print_community_link (bool): print or not.
@@ -240,40 +278,14 @@
             self.fail(message=message)
         except yaml.YAMLError as exc:
             message = f"Failed to parse {filepath} file: {str(exc)}"
             self.fail(message=message)
         else:
             return content
 
-    def __init__(self, pipe_metadata=None, pipe_metadata_file=None, schema=None,
-                 env=None, logger=logger, check_for_newer_version=False):
-        if pipe_metadata is not None and pipe_metadata_file is not None:
-            self.fail(message="Passing both pipe_metadata and pipe_metadata_file is not allowed. "
-                              "Please use only one of them.")
-        if pipe_metadata_file is not None:
-            self.metadata = self.parse_yaml_file(filepath=pipe_metadata_file)
-        elif pipe_metadata is not None:
-            self.metadata = pipe_metadata
-        else:
-            self.metadata = {}
-
-        if env is None:
-            self.env = os.environ.copy()
-        else:
-            self.env = env
-
-        self.variables = None
-        self.schema = schema
-        self.logger = logger
-        # validate pipe parameters
-        self.variables = self.validate()
-        self.enable_debug_log_level()
-        if check_for_newer_version:
-            self.check_for_newer_version()
-
     def check_for_newer_version(self):
         """Check if a newer version is available and show a warning message
 
         >>> metadata = {'image': 'bitbucketpipelines/aws-ecs-deploy:0.0.3',
         ...             'repository': 'https://bitbucket.org/atlassian/aws-ecs-deploy'}
         >>> pipe = Pipe(pipe_metadata=metadata, schema={})
         >>> pipe.check_for_newer_version()
@@ -344,15 +356,15 @@
                 # NOTE: we accept string as this
                 if schema[key].get('type', '') == 'string':
                     env[key] = value
                     continue
 
                 try:
                     env[key] = yaml.safe_load(value)
-                except yaml.scanner.ScannerError:
+                except ScannerError:
                     # keep a string value
                     env[key] = value
 
         for key, key_schema in schema.items():
             if key_schema.get('type') == 'list':
                 env[key] = ArrayVariable(key, self.env)
 
@@ -379,14 +391,54 @@
         """
         tags = self.metadata.get("tags")
         tags_string = ",".join(tags) if tags else ""
         community_link = f"https://community.atlassian.com/t5/forums/postpage/board-id/bitbucket-pipelines-questions?" \
                          f"add-tags=pipes,{tags_string}"
         return community_link
 
+    def resolve_auth(self):
+        """Resolve authorization.
+        Currently supported:
+        - BITBUCKET_USERNAME and BITBUCKET_APP_PASSWORD
+        or
+        - BITBUCKET_ACCESS_TOKEN
+
+        Returns
+        <HTTPBasicAuth object> or <TokenAuth object>
+
+        Raises
+        Authentication missing ... SystemExit: 1
+
+        >>> pipe = Pipe(schema={})
+        >>> pipe.resolve_auth()
+        Traceback (most recent call last):
+        SystemExit: 1
+
+        >>> pipe = Pipe(schema={})
+        >>> pipe.variables = {'BITBUCKET_USERNAME': 'test', 'BITBUCKET_APP_PASSWORD': 'test-pass'}
+        >>> pipe.resolve_auth() # doctest: +ELLIPSIS
+        <...HTTPBasicAuth object at 0x...>
+
+        >>> pipe = Pipe(schema={})
+        >>> pipe.variables = {'BITBUCKET_ACCESS_TOKEN': 'test-token'}
+        >>> pipe.resolve_auth() # doctest: +ELLIPSIS
+        <...TokenAuth object at 0x...>
+
+        """
+        username = self.get_variable('BITBUCKET_USERNAME')
+        password = self.get_variable('BITBUCKET_APP_PASSWORD')
+        token = self.get_variable('BITBUCKET_ACCESS_TOKEN')
+
+        if username and password:
+            return HTTPBasicAuth(username, password)
+        elif token:
+            return TokenAuth(token)
+        else:
+            self.fail('Authentication missing. You must provide an access token or a username and app password.')
+
     def run(self):
         """Run the pipe.
 
         The main entry point for a pipe execution. This will do
         all the setup steps, like enabling debug mode if configure etc.
         """
         self.enable_debug_log_level()
```

### Comparing `bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/helpers.py` & `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit/test.py` & `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/test.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.2.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO` & `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.2.1
+Version: 3.3.0
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
 License: UNKNOWN
 Description: Bitbucket Pipes Toolkit
         =========
```

### Comparing `bitbucket-pipes-toolkit-3.2.1/setup.py` & `bitbucket-pipes-toolkit-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bitbucket-pipes-toolkit',
-    version='3.2.1',
+    version='3.3.0',
     packages=['bitbucket_pipes_toolkit', ],
     url='https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit',
     author='Atlassian',
     author_email='bitbucketci-team@atlassian.com',
     description='This package contains various helpers for developing bitbucket pipelines pipes',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

