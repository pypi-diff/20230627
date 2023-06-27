# Comparing `tmp/configshell-fb-1.1.29.tar.gz` & `tmp/configshell-fb-1.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configshell-fb-1.1.29.tar", last modified: Thu Mar 25 07:42:52 2021, max compression
+gzip compressed data, was "configshell-fb-1.1.30.tar", last modified: Tue Jun 27 15:06:14 2023, max compression
```

## Comparing `configshell-fb-1.1.29.tar` & `configshell-fb-1.1.30.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2021-03-25 07:42:52.511271 configshell-fb-1.1.29/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      444 2021-03-25 07:42:52.511271 configshell-fb-1.1.29/PKG-INFO
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1688 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/README.md
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2021-03-25 07:42:52.507271 configshell-fb-1.1.29/configshell/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1149 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/__init__.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    10940 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/console.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     5498 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/log.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    68890 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/node.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     4558 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/prefs.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    35845 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell/shell.py
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2021-03-25 07:42:52.507271 configshell-fb-1.1.29/configshell_fb/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1149 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/__init__.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    10940 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/console.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     5498 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/log.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    68890 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/node.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     4558 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/prefs.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    35845 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/configshell_fb/shell.py
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2021-03-25 07:42:52.511271 configshell-fb-1.1.29/configshell_fb.egg-info/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      444 2021-03-25 07:42:51.000000 configshell-fb-1.1.29/configshell_fb.egg-info/PKG-INFO
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      481 2021-03-25 07:42:51.000000 configshell-fb-1.1.29/configshell_fb.egg-info/SOURCES.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)        1 2021-03-25 07:42:51.000000 configshell-fb-1.1.29/configshell_fb.egg-info/dependency_links.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       32 2021-03-25 07:42:51.000000 configshell-fb-1.1.29/configshell_fb.egg-info/requires.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       27 2021-03-25 07:42:51.000000 configshell-fb-1.1.29/configshell_fb.egg-info/top_level.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       38 2021-03-25 07:42:52.511271 configshell-fb-1.1.29/setup.cfg
--rwxrwxr-x   0 mlombard  (1000) mlombard  (1000)     1676 2021-03-04 12:59:32.000000 configshell-fb-1.1.29/setup.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 15:06:14.331988 configshell-fb-1.1.30/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    10143 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/COPYING
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      466 2023-06-27 15:06:14.330988 configshell-fb-1.1.30/PKG-INFO
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1688 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/README.md
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 15:06:14.329988 configshell-fb-1.1.30/configshell/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1149 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/__init__.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    10940 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/console.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     5498 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/log.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    68900 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/node.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     4558 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/prefs.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    35845 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell/shell.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 15:06:14.330988 configshell-fb-1.1.30/configshell_fb/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1149 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/__init__.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    10940 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/console.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     5498 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/log.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    68900 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/node.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     4558 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/prefs.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    35845 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/configshell_fb/shell.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 15:06:14.330988 configshell-fb-1.1.30/configshell_fb.egg-info/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      466 2023-06-27 15:06:14.000000 configshell-fb-1.1.30/configshell_fb.egg-info/PKG-INFO
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      489 2023-06-27 15:06:14.000000 configshell-fb-1.1.30/configshell_fb.egg-info/SOURCES.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)        1 2023-06-27 15:06:14.000000 configshell-fb-1.1.30/configshell_fb.egg-info/dependency_links.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       27 2023-06-27 15:06:14.000000 configshell-fb-1.1.30/configshell_fb.egg-info/requires.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       27 2023-06-27 15:06:14.000000 configshell-fb-1.1.30/configshell_fb.egg-info/top_level.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       38 2023-06-27 15:06:14.331988 configshell-fb-1.1.30/setup.cfg
+-rwxr-xr-x   0 mlombard  (1000) mlombard  (1000)     1671 2023-06-27 14:51:06.000000 configshell-fb-1.1.30/setup.py
```

### Comparing `configshell-fb-1.1.29/README.md` & `configshell-fb-1.1.30/README.md`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell/__init__.py` & `configshell-fb-1.1.30/configshell/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
 from .console import Console
 from .log import Log
 from .node import ConfigNode, ExecutionError
 from .prefs import Prefs
 from .shell import ConfigShell
 
-__version__ = '1.1.29'
+__version__ = '1.1.30'
 __url__ = 'http://github.com/open-iscsi/configshell-fb'
 __description__ = 'A framework to implement simple but nice CLIs.'
 __license__ = 'Apache 2.0'
```

### Comparing `configshell-fb-1.1.29/configshell/console.py` & `configshell-fb-1.1.30/configshell/console.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell/log.py` & `configshell-fb-1.1.30/configshell/log.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell/node.py` & `configshell-fb-1.1.30/configshell/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1413,18 +1413,18 @@
         @type method: method
         @param pparams: The positional parameters.
         @type pparams: list
         @param kparams: The keyword parameters.
         @type kparams: dict
         @raise ExecutionError: When the check fails.
         '''
-        spec = inspect.getargspec(method)
+        spec = inspect.getfullargspec(method)
         args = spec.args[1:]
         pp = spec.varargs
-        kw = spec.keywords
+        kw = spec.varkw
 
         if spec.defaults is None:
             nb_opt_params = 0
         else:
             nb_opt_params = len(spec.defaults)
         nb_max_params = len(args)
         nb_min_params = nb_max_params - nb_opt_params
@@ -1456,15 +1456,15 @@
                 "Missing required parameter %s"
                 % missing_params[0])
         elif missing_params:
             raise ExecutionError(
                 "Missing required parameters %s"
                 % ", ".join("'%s'" % missing for missing in missing_params))
 
-        if spec.keywords is None:
+        if kw is None:
             if len(unexpected_keywords) == 1:
                 raise ExecutionError(
                     "Unexpected keyword parameter '%s'."
                     % unexpected_keywords[0])
             elif unexpected_keywords:
                 raise ExecutionError(
                     "Unexpected keyword parameters %s."
@@ -1571,20 +1571,20 @@
             - comments is a list of additionnal comments about the syntax.
             - default_values is a string with the default parameters values.
         @rtype: (str, [str...], str)
         @param command: The command to document.
         @type command: str
         '''
         method = self.get_command_method(command)
-        parameters, args, kwargs, default = inspect.getargspec(method)
-        parameters = parameters[1:]
-        if default is None:
+        spec = inspect.getfullargspec(method)
+        parameters = spec.args[1:]
+        if spec.defaults is None:
             num_defaults = 0
         else:
-            num_defaults = len(default)
+            num_defaults = len(spec.defaults)
 
         if num_defaults != 0:
             required_parameters = parameters[:-num_defaults]
             optional_parameters = parameters[-num_defaults:]
         else:
             required_parameters = parameters
             optional_parameters = []
@@ -1601,24 +1601,24 @@
 
         optional_parameters_str = ''
         for param in optional_parameters:
             optional_parameters_str += "[%s] " % param
         syntax += optional_parameters_str
 
         comments = []
-        if args is not None:
-            syntax += "[%s...] " % args
-        if kwargs is not None:
-            syntax += "[%s=value...] " % (kwargs)
+        if spec.varargs is not None:
+            syntax += "[%s...] " % spec.varargs
+        if spec.varkw is not None:
+            syntax += "[%s=value...] " % (spec.varkw)
 
         default_values = ''
         if num_defaults > 0:
             for index, param in enumerate(optional_parameters):
-                if default[index] is not None:
-                    default_values += "%s=%s " % (param, str(default[index]))
+                if spec.defaults[index] is not None:
+                    default_values += "%s=%s " % (param, str(spec.defaults[index]))
 
         return syntax, comments, default_values
 
     def get_command_signature(self, command):
         '''
         Get a command's signature.
         @param command: The command to get the signature of.
@@ -1626,22 +1626,22 @@
         @return: (parameters, free_pparams, free_kparams) where parameters is a
         list of all the command's parameters and free_pparams and free_kparams
         booleans set to True is the command accepts an arbitrary number of,
         respectively, pparams and kparams.
         @rtype: ([str...], bool, bool)
         '''
         method = self.get_command_method(command)
-        parameters, args, kwargs, default = inspect.getargspec(method)
-        parameters = parameters[1:]
-        if args is not None:
-            free_pparams = args
+        spec = inspect.getfullargspec(method)
+        parameters = spec.args[1:]
+        if spec.varargs is not None:
+            free_pparams = spec.varargs
         else:
             free_pparams = False
-        if kwargs is not None:
-            free_kparams = kwargs
+        if spec.varkw is not None:
+            free_kparams = spec.varkw
         else:
             free_kparams = False
         self.shell.log.debug("Signature is %s, %s, %s."
                              % (str(parameters),
                                 str(free_pparams),
                                 str(free_kparams)))
         return parameters, free_pparams, free_kparams
```

### Comparing `configshell-fb-1.1.29/configshell/prefs.py` & `configshell-fb-1.1.30/configshell/prefs.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell/shell.py` & `configshell-fb-1.1.30/configshell/shell.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell_fb/__init__.py` & `configshell-fb-1.1.30/configshell_fb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
 from .console import Console
 from .log import Log
 from .node import ConfigNode, ExecutionError
 from .prefs import Prefs
 from .shell import ConfigShell
 
-__version__ = '1.1.29'
+__version__ = '1.1.30'
 __url__ = 'http://github.com/open-iscsi/configshell-fb'
 __description__ = 'A framework to implement simple but nice CLIs.'
 __license__ = 'Apache 2.0'
```

### Comparing `configshell-fb-1.1.29/configshell_fb/console.py` & `configshell-fb-1.1.30/configshell_fb/console.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell_fb/log.py` & `configshell-fb-1.1.30/configshell_fb/log.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell_fb/node.py` & `configshell-fb-1.1.30/configshell_fb/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1413,18 +1413,18 @@
         @type method: method
         @param pparams: The positional parameters.
         @type pparams: list
         @param kparams: The keyword parameters.
         @type kparams: dict
         @raise ExecutionError: When the check fails.
         '''
-        spec = inspect.getargspec(method)
+        spec = inspect.getfullargspec(method)
         args = spec.args[1:]
         pp = spec.varargs
-        kw = spec.keywords
+        kw = spec.varkw
 
         if spec.defaults is None:
             nb_opt_params = 0
         else:
             nb_opt_params = len(spec.defaults)
         nb_max_params = len(args)
         nb_min_params = nb_max_params - nb_opt_params
@@ -1456,15 +1456,15 @@
                 "Missing required parameter %s"
                 % missing_params[0])
         elif missing_params:
             raise ExecutionError(
                 "Missing required parameters %s"
                 % ", ".join("'%s'" % missing for missing in missing_params))
 
-        if spec.keywords is None:
+        if kw is None:
             if len(unexpected_keywords) == 1:
                 raise ExecutionError(
                     "Unexpected keyword parameter '%s'."
                     % unexpected_keywords[0])
             elif unexpected_keywords:
                 raise ExecutionError(
                     "Unexpected keyword parameters %s."
@@ -1571,20 +1571,20 @@
             - comments is a list of additionnal comments about the syntax.
             - default_values is a string with the default parameters values.
         @rtype: (str, [str...], str)
         @param command: The command to document.
         @type command: str
         '''
         method = self.get_command_method(command)
-        parameters, args, kwargs, default = inspect.getargspec(method)
-        parameters = parameters[1:]
-        if default is None:
+        spec = inspect.getfullargspec(method)
+        parameters = spec.args[1:]
+        if spec.defaults is None:
             num_defaults = 0
         else:
-            num_defaults = len(default)
+            num_defaults = len(spec.defaults)
 
         if num_defaults != 0:
             required_parameters = parameters[:-num_defaults]
             optional_parameters = parameters[-num_defaults:]
         else:
             required_parameters = parameters
             optional_parameters = []
@@ -1601,24 +1601,24 @@
 
         optional_parameters_str = ''
         for param in optional_parameters:
             optional_parameters_str += "[%s] " % param
         syntax += optional_parameters_str
 
         comments = []
-        if args is not None:
-            syntax += "[%s...] " % args
-        if kwargs is not None:
-            syntax += "[%s=value...] " % (kwargs)
+        if spec.varargs is not None:
+            syntax += "[%s...] " % spec.varargs
+        if spec.varkw is not None:
+            syntax += "[%s=value...] " % (spec.varkw)
 
         default_values = ''
         if num_defaults > 0:
             for index, param in enumerate(optional_parameters):
-                if default[index] is not None:
-                    default_values += "%s=%s " % (param, str(default[index]))
+                if spec.defaults[index] is not None:
+                    default_values += "%s=%s " % (param, str(spec.defaults[index]))
 
         return syntax, comments, default_values
 
     def get_command_signature(self, command):
         '''
         Get a command's signature.
         @param command: The command to get the signature of.
@@ -1626,22 +1626,22 @@
         @return: (parameters, free_pparams, free_kparams) where parameters is a
         list of all the command's parameters and free_pparams and free_kparams
         booleans set to True is the command accepts an arbitrary number of,
         respectively, pparams and kparams.
         @rtype: ([str...], bool, bool)
         '''
         method = self.get_command_method(command)
-        parameters, args, kwargs, default = inspect.getargspec(method)
-        parameters = parameters[1:]
-        if args is not None:
-            free_pparams = args
+        spec = inspect.getfullargspec(method)
+        parameters = spec.args[1:]
+        if spec.varargs is not None:
+            free_pparams = spec.varargs
         else:
             free_pparams = False
-        if kwargs is not None:
-            free_kparams = kwargs
+        if spec.varkw is not None:
+            free_kparams = spec.varkw
         else:
             free_kparams = False
         self.shell.log.debug("Signature is %s, %s, %s."
                              % (str(parameters),
                                 str(free_pparams),
                                 str(free_kparams)))
         return parameters, free_pparams, free_kparams
```

### Comparing `configshell-fb-1.1.29/configshell_fb/prefs.py` & `configshell-fb-1.1.30/configshell_fb/prefs.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/configshell_fb/shell.py` & `configshell-fb-1.1.30/configshell_fb/shell.py`

 * *Files identical despite different names*

### Comparing `configshell-fb-1.1.29/setup.py` & `configshell-fb-1.1.30/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,23 +30,23 @@
             version = match.group(1)
             break
     else:
         raise Exception("Couldn't find version in setup.py")
 
 setup(
     name = 'configshell-fb',
-    version = '1.1.29',
+    version = '1.1.30',
     description = 'A framework to implement simple but nice CLIs.',
     license = 'Apache 2.0',
     maintainer = 'Andy Grover',
     maintainer_email = 'agrover@redhat.com',
     url = 'http://github.com/open-iscsi/configshell-fb',
     packages = ['configshell', 'configshell_fb'],
     install_requires = [
-        'pyparsing >=2.0.2,<3.0',
+        'pyparsing >=2.0.2',
         'six',
         'urwid',
     ],
     classifiers = [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

