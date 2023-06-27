# Comparing `tmp/django-lazy-srcset-0.1.0.tar.gz` & `tmp/django-lazy-srcset-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-0.1.0.tar", last modified: Mon Jun 26 19:29:43 2023, max compression
+gzip compressed data, was "django-lazy-srcset-0.2.0.tar", last modified: Tue Jun 27 21:15:42 2023, max compression
```

## Comparing `django-lazy-srcset-0.1.0.tar` & `django-lazy-srcset-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-26 19:29:43.280536 django-lazy-srcset-0.1.0/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.1.0/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)      155 2023-06-26 19:06:22.000000 django-lazy-srcset-0.1.0/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     4340 2023-06-26 19:29:43.280614 django-lazy-srcset-0.1.0/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     2863 2023-06-26 19:27:12.000000 django-lazy-srcset-0.1.0/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-26 19:29:43.278282 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     4340 2023-06-26 19:29:43.000000 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      445 2023-06-26 19:29:43.000000 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-26 19:29:43.000000 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-06-26 19:29:43.000000 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-06-26 19:29:43.000000 django-lazy-srcset-0.1.0/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-26 19:29:43.279584 django-lazy-srcset-0.1.0/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.1.0/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.1.0/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.1.0/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.1.0/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-26 19:29:43.280405 django-lazy-srcset-0.1.0/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.1.0/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     8358 2023-06-26 19:18:24.000000 django-lazy-srcset-0.1.0/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.1.0/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-06-26 19:29:43.283994 django-lazy-srcset-0.1.0/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.1.0/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.566515 django-lazy-srcset-0.2.0/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.0/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       49 2023-06-27 17:54:23.000000 django-lazy-srcset-0.2.0/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-27 21:15:42.566631 django-lazy-srcset-0.2.0/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.0/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.560594 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      445 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.562817 django-lazy-srcset-0.2.0/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.0/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.0/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.0/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.0/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.566002 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8879 2023-06-27 16:04:10.000000 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.0/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-06-27 21:15:42.570431 django-lazy-srcset-0.2.0/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.0/setup.py
```

### Comparing `django-lazy-srcset-0.1.0/LICENSE` & `django-lazy-srcset-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.1.0/lazy_srcset/conf.py` & `django-lazy-srcset-0.2.0/lazy_srcset/conf.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.1.0/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-0.2.0/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.1.0/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-0.2.0/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import re
 from pathlib import Path
 from xml.etree import ElementTree
 
 from django import template
 from django.contrib.staticfiles import finders
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.core.files.images import ImageFile
@@ -61,14 +62,18 @@
         if width is None or height is None:
             viewbox = root.get("viewBox")
             try:
                 _, _, width, height = viewbox.split(" ")
             except (AttributeError, ValueError):
                 pass
 
+        # These could include units eg px or pt so strip them out.
+        width = re.sub("\\D", "", width) if width is not None else None
+        height = re.sub("\\D", "", height) if height is not None else None
+
     return width, height
 
 
 def svg_srcset(svg_file):
     """
     Returns attrs string containing src and width and height if possible. Will also add role="img" attr.
     """
@@ -97,42 +102,45 @@
 @register.simple_tag
 def srcset(*args, **kwargs):
     """
     The srcset template tag will create srcset, sizes, src, width and height attributes for an <img> tag.
 
     The first arg must be an ImageField or subclass or a path to an image discoverable by static files.
 
-    args can provide image sizes in vw for each breakpoint, if not provided 100vw is assumed.  These are integers
-    which are used to calculate generated image sizes.  They must be in vw.  Sorry no calc() etc. allowed.  Don't try
-    too hard here! Close is good enough.
+    args can provide relative image sizes in vw for each breakpoint, if not provided 100vw is assumed.  These are
+    integers which are used to calculate generated image sizes.  They must be in vw.  Sorry no calc() etc. allowed.
+    Don't try too hard here! Close is good enough.
+
+    kwargs can be used to provide breakpoints and the relative width for each breakpoint directly (ignoring the
+    config breakpoints and args if you set them for some reason).
 
-    kwargs can be used to provide this and breakpoints to use.
+    The config with the key ``default`` is used unless you provide the config kwarg to specify another config to use.
 
-    If the second arg is a key from ``settings.LAZY_SRCSET`` this will be used otherwise the default config will be
-    used.
+    You can use the ``max_width`` and ``qualtiy`` kwargs to override the config on a per-use basis.
 
     Example usage (where image is a file-like e.g. ImageField or a string representing a path to a static file):
 
-    {% srcset image %}
+    <img {% srcset image %} />
 
-    {% srcset image 25 50 %}
+    <img {% srcset image 25 50 %} />
 
-    {% srcset image 25 50 quality=50 %}
+    <img {% srcset image 25 50 quality=50 %} />
 
-    {% srcset image "custom_breakpoints" %}
+    <img {% srcset image config="custom_breakpoints" %} />
 
-    {% srcset image "custom_breakpoints" 25 50 %}
+    <img {% srcset image 25 50 config="custom_breakpoints" %} />
 
-    {% srcset image "custom_breakpoints" 25 50 quality=50 %}
+    <img {% srcset image 25 50 config="custom_breakpoints" quality=50 %} />
 
-    {% srcset image "custom_breakpoints" 25 50 max_width=1920 quality=50 %}
+    <img {% srcset image 25 50 config="custom_breakpoints" max_width=1920 quality=50 %} />
 
-    {% srcset image 1920=25 1024=50 %}
+    <img {% srcset image 1920=25 1024=50 %} />
+
+    <img {% srcset image 1920=25 1024=50 max_width=1920 quality=50 %} />
 
-    {% srcset image 1920=25 1024=50 max_width=1920 quality=50 %}
 
     """
     args = list(args)
 
     # If the image has an open method we should be good to go.  If not assume it's a string and get it from
     # staticfiles wrapped up in ImageFile. Set the url attribute, so we can use it later.
     image = args.pop(0)
@@ -143,17 +151,16 @@
 
     # If the image is an SVG return now with src="whatever.svg" and width and height if possible. SVG is lazy king!
     if Path(image.name).suffix.lower() == ".svg":
         return svg_srcset(image)
 
     # Get the conf from the first arg or default
     try:
-        conf = settings.LAZY_SRCSET[args[0]]
-        args.pop(0)
-    except (KeyError, IndexError):
+        conf = settings.LAZY_SRCSET[kwargs.pop("config")]
+    except KeyError:
         conf = settings.LAZY_SRCSET["default"]
 
     # Get the max_width from kwargs or conf.
     max_width = get_from_kwargs_or_conf("max_width", kwargs, conf)
 
     # Set the maximum width image in our srcset.
     if max_width is None or max_width > image.width:
```

### Comparing `django-lazy-srcset-0.1.0/setup.cfg` & `django-lazy-srcset-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-lazy-srcset
-version = 0.1.0
+version = 0.2.0
 description = Lazy srcset and image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

