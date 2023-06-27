# Comparing `tmp/django-service-urls-1.3.tar.gz` & `tmp/django-service-urls-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-service-urls-1.3.tar", last modified: Tue Mar 28 21:12:23 2023, max compression
+gzip compressed data, was "django-service-urls-1.4.tar", last modified: Tue Jun 27 13:32:07 2023, max compression
```

## Comparing `django-service-urls-1.3.tar` & `django-service-urls-1.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-03-28 21:12:23.885497 django-service-urls-1.3/
--rw-r--r--   0 raf       (1000) raf       (1000)     1338 2023-03-28 20:37:50.000000 django-service-urls-1.3/LICENSE
--rw-r--r--   0 raf       (1000) raf       (1000)      131 2023-03-28 20:37:50.000000 django-service-urls-1.3/MANIFEST.in
--rw-rw-r--   0 raf       (1000) raf       (1000)     9154 2023-03-28 21:12:23.885497 django-service-urls-1.3/PKG-INFO
--rw-r--r--   0 raf       (1000) raf       (1000)     7775 2023-03-28 20:37:50.000000 django-service-urls-1.3/README.md
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-03-28 21:12:23.885497 django-service-urls-1.3/django_service_urls.egg-info/
--rw-rw-r--   0 raf       (1000) raf       (1000)     9154 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/PKG-INFO
--rw-rw-r--   0 raf       (1000) raf       (1000)      440 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/SOURCES.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/dependency_links.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/not-zip-safe
--rw-rw-r--   0 raf       (1000) raf       (1000)        7 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/requires.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)       13 2023-03-28 21:12:23.000000 django-service-urls-1.3/django_service_urls.egg-info/top_level.txt
--rw-r--r--   0 raf       (1000) raf       (1000)     2960 2023-03-28 20:37:50.000000 django-service-urls-1.3/pyproject.toml
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-03-28 21:12:23.885497 django-service-urls-1.3/service_urls/
--rw-r--r--   0 raf       (1000) raf       (1000)     1645 2023-03-28 20:37:50.000000 django-service-urls-1.3/service_urls/__init__.py
--rw-r--r--   0 raf       (1000) raf       (1000)     4435 2023-03-28 20:37:50.000000 django-service-urls-1.3/service_urls/base.py
--rw-r--r--   0 raf       (1000) raf       (1000)     3201 2023-03-28 20:37:50.000000 django-service-urls-1.3/service_urls/patch.py
--rw-r--r--   0 raf       (1000) raf       (1000)     9539 2023-03-28 20:37:50.000000 django-service-urls-1.3/service_urls/services.py
--rw-r--r--   0 raf       (1000) raf       (1000)     2102 2023-03-28 20:37:50.000000 django-service-urls-1.3/service_urls/version.py
--rw-rw-r--   0 raf       (1000) raf       (1000)       38 2023-03-28 21:12:23.885497 django-service-urls-1.3/setup.cfg
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-03-28 21:12:23.885497 django-service-urls-1.3/tests/
--rw-r--r--   0 raf       (1000) raf       (1000)    19880 2023-03-28 20:37:50.000000 django-service-urls-1.3/tests/test_services.py
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.336540 django-service-urls-1.4/
+-rw-r--r--   0 raf       (1000) raf       (1000)     1255 2023-06-17 08:18:52.000000 django-service-urls-1.4/CHANGELOG.md
+-rw-r--r--   0 raf       (1000) raf       (1000)     1388 2023-06-17 08:18:52.000000 django-service-urls-1.4/LICENSE
+-rw-r--r--   0 raf       (1000) raf       (1000)      152 2023-06-17 08:18:52.000000 django-service-urls-1.4/MANIFEST.in
+-rw-rw-r--   0 raf       (1000) raf       (1000)     8479 2023-06-27 13:32:07.336540 django-service-urls-1.4/PKG-INFO
+-rw-r--r--   0 raf       (1000) raf       (1000)     6954 2023-06-17 08:18:52.000000 django-service-urls-1.4/README.md
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/django_service_urls.egg-info/
+-rw-rw-r--   0 raf       (1000) raf       (1000)     8479 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/PKG-INFO
+-rw-rw-r--   0 raf       (1000) raf       (1000)      474 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/SOURCES.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/dependency_links.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:32:06.000000 django-service-urls-1.4/django_service_urls.egg-info/not-zip-safe
+-rw-rw-r--   0 raf       (1000) raf       (1000)        7 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/requires.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)       13 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/top_level.txt
+-rw-r--r--   0 raf       (1000) raf       (1000)     3091 2023-06-17 08:18:52.000000 django-service-urls-1.4/pyproject.toml
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/service_urls/
+-rw-r--r--   0 raf       (1000) raf       (1000)     1696 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/__init__.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     4486 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/base.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     3235 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/patch.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     9938 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/services.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     2152 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/version.py
+-rw-rw-r--   0 raf       (1000) raf       (1000)       38 2023-06-27 13:32:07.336540 django-service-urls-1.4/setup.cfg
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/tests/
+-rw-r--r--   0 raf       (1000) raf       (1000)     3215 2023-06-17 08:18:52.000000 django-service-urls-1.4/tests/test_django.py
+-rw-r--r--   0 raf       (1000) raf       (1000)    21489 2023-06-17 08:18:52.000000 django-service-urls-1.4/tests/test_services.py
```

### Comparing `django-service-urls-1.3/LICENSE` & `django-service-urls-1.4/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 Copyright (C) Tom Forbes
 Copyright (C) Kenneth Reitz
-
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
 
-THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django-service-urls-1.3/PKG-INFO` & `django-service-urls-1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: django-service-urls
-Version: 1.3
+Version: 1.4
 Summary: setting helper for django to represent databases, caches and email settings via a single string
 Author-email: Raffaele Salmaso <raffaele.salmaso@gmail.com>
 License: BSD
 Project-URL: GitHub, https://github.com/rsalmaso/django-service-urls
+Project-URL: Changelog, https://github.com/rsalmaso/django-service-urls/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
@@ -21,14 +22,15 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-service-urls
 
 `django-service-urls` is a setting helper for django to represent databases, caches and email settings via a single string.
@@ -228,48 +230,7 @@
 search = SearchService()
 
 
 @search.register(('myengine', 'my_search_engine'))
 def search_config_from_url(backend, engine, scheme, url):
     return backend.config_from_url(engine, scheme, url)
 ```
-
-## Changes
-
-### 1.3.0
-
-* use declarative config in setup.cfg
-* add support for Django 3.2, 4.0, 4.1, and 4.2
-* add support for Python 3.8, 3.9, 3.10, and 3.11
-* drop support for Django < 3.2
-* drop support for Python < 3.8
-* format code with black
-* switch to ruff from flake8/isort
-
-### 1.2.0
-
-* add __lt__ and __gt__ when using Django < 2.2
-* correct settings operations under django > 1.11 (ie: when running tests which override values)
-* add Django 2.2 support
-
-### 1.1.1
-
-* correct sqlite parser
-
-### 1.1.0
-
-* add helper to monkey patch django settings
-* doc cleanup
-
-### 1.0.2
-
-* fix setup.py and MANIFEST.in
-
-### 1.0.1
-
-* fix README typos
-
-### 1.0.0
-
-* Add `service_urls.db` service and default parsers
-* Add `service_urls.cache` service and default parsers
-* Add `service_urls.email` service and default parsers
```

### Comparing `django-service-urls-1.3/README.md` & `django-service-urls-1.4/django_service_urls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: django-service-urls
+Version: 1.4
+Summary: setting helper for django to represent databases, caches and email settings via a single string
+Author-email: Raffaele Salmaso <raffaele.salmaso@gmail.com>
+License: BSD
+Project-URL: GitHub, https://github.com/rsalmaso/django-service-urls
+Project-URL: Changelog, https://github.com/rsalmaso/django-service-urls/blob/main/CHANGELOG.md
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # django-service-urls
 
 `django-service-urls` is a setting helper for django to represent databases, caches and email settings via a single string.
 
 This work is based on [dj-database-url](https://github.com/jazzband/dj-database-url) and [https://github.com/django/django/pull/8562](https://github.com/django/django/pull/8562).
 
 ### Example
@@ -197,48 +230,7 @@
 search = SearchService()
 
 
 @search.register(('myengine', 'my_search_engine'))
 def search_config_from_url(backend, engine, scheme, url):
     return backend.config_from_url(engine, scheme, url)
 ```
-
-## Changes
-
-### 1.3.0
-
-* use declarative config in setup.cfg
-* add support for Django 3.2, 4.0, 4.1, and 4.2
-* add support for Python 3.8, 3.9, 3.10, and 3.11
-* drop support for Django < 3.2
-* drop support for Python < 3.8
-* format code with black
-* switch to ruff from flake8/isort
-
-### 1.2.0
-
-* add __lt__ and __gt__ when using Django < 2.2
-* correct settings operations under django > 1.11 (ie: when running tests which override values)
-* add Django 2.2 support
-
-### 1.1.1
-
-* correct sqlite parser
-
-### 1.1.0
-
-* add helper to monkey patch django settings
-* doc cleanup
-
-### 1.0.2
-
-* fix setup.py and MANIFEST.in
-
-### 1.0.1
-
-* fix README typos
-
-### 1.0.0
-
-* Add `service_urls.db` service and default parsers
-* Add `service_urls.cache` service and default parsers
-* Add `service_urls.email` service and default parsers
```

### Comparing `django-service-urls-1.3/pyproject.toml` & `django-service-urls-1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,26 @@
     "Framework :: Django :: 4.2",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
     "django",
 ]
 
 [project.urls]
 GitHub = "https://github.com/rsalmaso/django-service-urls"
+Changelog = "https://github.com/rsalmaso/django-service-urls/blob/main/CHANGELOG.md"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.dynamic]
 version = {attr = "service_urls.__version__"}
```

### Comparing `django-service-urls-1.3/service_urls/__init__.py` & `django-service-urls-1.4/service_urls/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 from .base import Service  # noqa: F401
 from .services import cache, db, email  # noqa: F401
 from .version import get_version
 
-VERSION = (1, 3, 0, "final", 0)
+VERSION = (1, 4, 0, "final", 0)
 
 __version__ = get_version(VERSION)
 __author__ = "Raffaele Salmaso"
 __email__ = "raffele@salmaso.org"
```

### Comparing `django-service-urls-1.3/service_urls/base.py` & `django-service-urls-1.4/service_urls/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 import re
 from urllib import parse
 
 
 class Service:
     validation = re.compile(r"^(?P<scheme>\S+)://\S*")
```

### Comparing `django-service-urls-1.3/service_urls/patch.py` & `django-service-urls-1.4/service_urls/patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 
 from django import conf
-from django.conf import (
-    ENVIRONMENT_VARIABLE,
-    LazySettings as DjangoLazySettings,
-    Settings as DjangoSettings,
-)
+from django.conf import ENVIRONMENT_VARIABLE, LazySettings as DjangoLazySettings, Settings as DjangoSettings
 from django.core.exceptions import ImproperlyConfigured
 
 from .services import cache, db, email
 
 
 class Settings(DjangoSettings):
     def __init__(self, settings_module):
```

### Comparing `django-service-urls-1.3/service_urls/services.py` & `django-service-urls-1.4/service_urls/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 from urllib import parse
 
 from .base import Service
 
 
 class DatabaseService(Service):
@@ -119,15 +119,15 @@
         }
         if multiple_netloc and parsed["location"]:
             config["LOCATION"] = parsed["location"]
         else:
             if parsed["hostname"]:
                 config["LOCATION"] = parsed["hostname"]
                 if parsed["port"]:
-                    config["LOCATION"] = f"{config['LOCATION']}:parsed['port']"
+                    config["LOCATION"] = f"{config['LOCATION']}:{parsed['port']}"
         for key in ("timeout", "key_prefix", "version"):
             if key in parsed["options"]:
                 option = parsed["options"].pop(key)
                 config[key.upper()] = option
         config["OPTIONS"] = parsed["options"]
         return config
 
@@ -153,35 +153,39 @@
     ("dummy", "django.core.cache.backends.dummy.DummyCache"),
 )
 def dummy_config_from_url(backend, engine, scheme, url):
     return backend.config_from_url(engine, scheme, url)
 
 
 @cache.register(
-    ("memcached", "django.core.cache.backends.memcached.MemcachedCache"),
+    ("pymemcached", "django.core.cache.backends.memcached.PyMemcachedCache"),
+    ("memcached", "django.core.cache.backends.memcached.MemcachedCache"),  # for django <= 4.2
 )
-def memcached_config_from_url(backend, engine, scheme, url):
+def pymemcached_config_from_url(backend, engine, scheme, url):
     parsed = backend.parse_url(url, multiple_netloc=True)
     config = backend.config_from_url(engine, scheme, parsed, multiple_netloc=True)
     if parsed["path"]:
-        # We are dealing with a URI like memcached:///socket/path
+        # We are dealing with a URI like pymemcached:///socket/path
         config["LOCATION"] = f"unix:/{parsed['path']}"
     return config
 
 
 @cache.register(
-    ("memcached+pylibmccache", "django.core.cache.backends.memcached.PyLibMCCache"),
+    ("pylibmccache", "django.core.cache.backends.memcached.PyLibMCCache"),
+    ("memcached+pylibmccache", "django.core.cache.backends.memcached.PyLibMCCache"),  # deprecated protocol
 )
 def pylibmccache_config_from_url(backend, engine, scheme, url):
+    # django >= 5.0 remove the "unix:" prefix from unix location
+    # keep a different converter until we support old django versions
     parsed = backend.parse_url(url, multiple_netloc=True)
-    # We are dealing with a URI like memcached://unix:/abc
-    # Set the hostname to be the unix path
-    parsed["hostname"] = f"/{parsed['path']}"
-    parsed["path"] = None
-    return backend.config_from_url(engine, scheme, parsed)
+    config = backend.config_from_url(engine, scheme, parsed, multiple_netloc=True)
+    if parsed["path"]:
+        # We are dealing with a URI like pylibmccache:///socket/path
+        config["LOCATION"] = f"/{parsed['path']}"
+    return config
 
 
 @cache.register(
     ("file", "django.core.cache.backends.filebased.FileBasedCache"),
 )
 def file_config_from_url(backend, engine, scheme, url):
     parsed = backend.parse_url(url)
```

### Comparing `django-service-urls-1.3/service_urls/version.py` & `django-service-urls-1.4/service_urls/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 def get_version(version=None):
     """Returns a PEP 386-compliant version number from VERSION."""
     if version is None:
         from . import VERSION as version
     else:
         assert len(version) == 5
```

### Comparing `django-service-urls-1.3/tests/test_services.py` & `django-service-urls-1.4/tests/test_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Copyright (C) Raffaele Salmaso <raffaele@salmaso.org>
 # Copyright (C) Tom Forbes
 # Copyright (C) Kenneth Reitz
-#
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #
-# THIS SOFTWARE IS PROVIDED BY KYLE FULLER ''AS IS'' AND ANY
-# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL KYLE FULLER BE LIABLE FOR ANY
-# DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+# THE POSSIBILITY OF SUCH DAMAGE.
 
 import unittest
 
 from service_urls import cache, db, email, Service
 
 GENERIC_TESTS = [
     ("username:password@domain/database", ("username", "password", "domain", "", "database", {})),
@@ -238,53 +238,93 @@
         self.assertNotIn("LOCATION", result)
 
     def test_dummy_caching_with_location(self):
         result = cache.parse("dummy://abc")
         self.assertEqual(result["BACKEND"], "django.core.cache.backends.dummy.DummyCache")
         self.assertEqual(result["LOCATION"], "abc")
 
-    def test_memcached_with_single_ip(self):
-        result = cache.parse("memcached://1.2.3.4:1567")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.MemcachedCache")
-        self.assertEqual(result["LOCATION"], "1.2.3.4:1567")
-
-    def test_memcached_with_multiple_ips(self):
-        result = cache.parse("memcached://1.2.3.4:1567,1.2.3.5:1568")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.MemcachedCache")
-        self.assertEqual(result["LOCATION"], ["1.2.3.4:1567", "1.2.3.5:1568"])
-
-    def test_memcached_without_port(self):
-        result = cache.parse("memcached://1.2.3.4")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.MemcachedCache")
-        self.assertEqual(result["LOCATION"], "1.2.3.4")
-
-    def test_memcached_with_unix_socket(self):
-        result = cache.parse("memcached:///tmp/memcached.sock")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.MemcachedCache")
-        self.assertEqual(result["LOCATION"], "unix:/tmp/memcached.sock")
-
-    def test_pylibmccache_memcached_with_single_ip(self):
-        result = cache.parse("memcached+pylibmccache://1.2.3.4:1567")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
-        self.assertEqual(result["LOCATION"], "1.2.3.4:1567")
-
-    def test_pylibmccache_memcached_with_multiple_ips(self):
-        result = cache.parse("memcached+pylibmccache://1.2.3.4:1567,1.2.3.5:1568")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
-        self.assertEqual(result["LOCATION"], ["1.2.3.4:1567", "1.2.3.5:1568"])
-
-    def test_pylibmccache_memcached_without_port(self):
-        result = cache.parse("memcached+pylibmccache://1.2.3.4")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
-        self.assertEqual(result["LOCATION"], "1.2.3.4")
-
-    def test_pylibmccache_memcached_with_unix_socket(self):
-        result = cache.parse("memcached+pylibmccache:///tmp/memcached.sock")
-        self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
-        self.assertEqual(result["LOCATION"], "/tmp/memcached.sock")
+    def test_pymemcached_with_single_ip(self):
+        for url, backend in [
+            ("pymemcached://1.2.3.4:1567", "django.core.cache.backends.memcached.PyMemcachedCache"),
+            ("memcached://1.2.3.4:1567", "django.core.cache.backends.memcached.MemcachedCache"),
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], backend)
+                self.assertEqual(result["LOCATION"], "1.2.3.4:1567")
+
+    def test_pymemcached_with_multiple_ips(self):
+        for url, backend in [
+            ("pymemcached://1.2.3.4:1567,1.2.3.5:1568", "django.core.cache.backends.memcached.PyMemcachedCache"),
+            ("memcached://1.2.3.4:1567,1.2.3.5:1568", "django.core.cache.backends.memcached.MemcachedCache"),
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], backend)
+                self.assertEqual(result["LOCATION"], ["1.2.3.4:1567", "1.2.3.5:1568"])
+
+    def test_pymemcached_without_port(self):
+        for url, backend in [
+            ("pymemcached://1.2.3.4", "django.core.cache.backends.memcached.PyMemcachedCache"),
+            ("memcached://1.2.3.4", "django.core.cache.backends.memcached.MemcachedCache"),
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], backend)
+                self.assertEqual(result["LOCATION"], "1.2.3.4")
+
+    def test_pymemcached_with_unix_socket(self):
+        for url, backend in [
+            ("pymemcached:///tmp/memcached.sock", "django.core.cache.backends.memcached.PyMemcachedCache"),
+            ("memcached:///tmp/memcached.sock", "django.core.cache.backends.memcached.MemcachedCache"),
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], backend)
+                self.assertEqual(result["LOCATION"], "unix:/tmp/memcached.sock")
+
+    def test_pylibmccache_with_single_ip(self):
+        for url in [
+            "pylibmccache://1.2.3.4:1567",
+            "memcached+pylibmccache://1.2.3.4:1567",
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
+                self.assertEqual(result["LOCATION"], "1.2.3.4:1567")
+
+    def test_pylibmccache_with_multiple_ips(self):
+        for url in [
+            "pylibmccache://1.2.3.4:1567,1.2.3.5:1568",
+            "memcached+pylibmccache://1.2.3.4:1567,1.2.3.5:1568",
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
+                self.assertEqual(result["LOCATION"], ["1.2.3.4:1567", "1.2.3.5:1568"])
+
+    def test_pylibmccache_without_port(self):
+        for url in [
+            "pylibmccache://1.2.3.4",
+            "memcached+pylibmccache://1.2.3.4",
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
+                self.assertEqual(result["LOCATION"], "1.2.3.4")
+
+    def test_pylibmccache_with_unix_socket(self):
+        for url in [
+            "pylibmccache:///tmp/memcached.sock",
+            "memcached+pylibmccache:///tmp/memcached.sock",
+        ]:
+            with self.subTest(url=url):
+                result = cache.parse(url)
+                self.assertEqual(result["BACKEND"], "django.core.cache.backends.memcached.PyLibMCCache")
+                self.assertEqual(result["LOCATION"], "/tmp/memcached.sock")
 
     def test_file_cache_windows_path(self):
         result = cache.parse("file://C:/abc/def/xyz")
         self.assertEqual(result["BACKEND"], "django.core.cache.backends.filebased.FileBasedCache")
         self.assertEqual(result["LOCATION"], "C:/abc/def/xyz")
 
     def test_file_cache_unix_path(self):
```

