# Comparing `tmp/django-service-urls-1.4.tar.gz` & `tmp/django-service-urls-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-service-urls-1.4.tar", last modified: Tue Jun 27 13:32:07 2023, max compression
+gzip compressed data, was "django-service-urls-1.4.1.tar", last modified: Tue Jun 27 13:45:59 2023, max compression
```

## Comparing `django-service-urls-1.4.tar` & `django-service-urls-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.336540 django-service-urls-1.4/
--rw-r--r--   0 raf       (1000) raf       (1000)     1255 2023-06-17 08:18:52.000000 django-service-urls-1.4/CHANGELOG.md
--rw-r--r--   0 raf       (1000) raf       (1000)     1388 2023-06-17 08:18:52.000000 django-service-urls-1.4/LICENSE
--rw-r--r--   0 raf       (1000) raf       (1000)      152 2023-06-17 08:18:52.000000 django-service-urls-1.4/MANIFEST.in
--rw-rw-r--   0 raf       (1000) raf       (1000)     8479 2023-06-27 13:32:07.336540 django-service-urls-1.4/PKG-INFO
--rw-r--r--   0 raf       (1000) raf       (1000)     6954 2023-06-17 08:18:52.000000 django-service-urls-1.4/README.md
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/django_service_urls.egg-info/
--rw-rw-r--   0 raf       (1000) raf       (1000)     8479 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/PKG-INFO
--rw-rw-r--   0 raf       (1000) raf       (1000)      474 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/SOURCES.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/dependency_links.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:32:06.000000 django-service-urls-1.4/django_service_urls.egg-info/not-zip-safe
--rw-rw-r--   0 raf       (1000) raf       (1000)        7 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/requires.txt
--rw-rw-r--   0 raf       (1000) raf       (1000)       13 2023-06-27 13:32:07.000000 django-service-urls-1.4/django_service_urls.egg-info/top_level.txt
--rw-r--r--   0 raf       (1000) raf       (1000)     3091 2023-06-17 08:18:52.000000 django-service-urls-1.4/pyproject.toml
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/service_urls/
--rw-r--r--   0 raf       (1000) raf       (1000)     1696 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/__init__.py
--rw-r--r--   0 raf       (1000) raf       (1000)     4486 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/base.py
--rw-r--r--   0 raf       (1000) raf       (1000)     3235 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/patch.py
--rw-r--r--   0 raf       (1000) raf       (1000)     9938 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/services.py
--rw-r--r--   0 raf       (1000) raf       (1000)     2152 2023-06-17 08:18:52.000000 django-service-urls-1.4/service_urls/version.py
--rw-rw-r--   0 raf       (1000) raf       (1000)       38 2023-06-27 13:32:07.336540 django-service-urls-1.4/setup.cfg
-drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:32:07.332540 django-service-urls-1.4/tests/
--rw-r--r--   0 raf       (1000) raf       (1000)     3215 2023-06-17 08:18:52.000000 django-service-urls-1.4/tests/test_django.py
--rw-r--r--   0 raf       (1000) raf       (1000)    21489 2023-06-17 08:18:52.000000 django-service-urls-1.4/tests/test_services.py
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:45:59.014716 django-service-urls-1.4.1/
+-rw-r--r--   0 raf       (1000) raf       (1000)     1317 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/CHANGELOG.md
+-rw-r--r--   0 raf       (1000) raf       (1000)     1388 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/LICENSE
+-rw-r--r--   0 raf       (1000) raf       (1000)      152 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/MANIFEST.in
+-rw-rw-r--   0 raf       (1000) raf       (1000)     8848 2023-06-27 13:45:59.014716 django-service-urls-1.4.1/PKG-INFO
+-rw-r--r--   0 raf       (1000) raf       (1000)     7321 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/README.md
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:45:59.010716 django-service-urls-1.4.1/django_service_urls.egg-info/
+-rw-rw-r--   0 raf       (1000) raf       (1000)     8848 2023-06-27 13:45:58.000000 django-service-urls-1.4.1/django_service_urls.egg-info/PKG-INFO
+-rw-rw-r--   0 raf       (1000) raf       (1000)      474 2023-06-27 13:45:59.000000 django-service-urls-1.4.1/django_service_urls.egg-info/SOURCES.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:45:58.000000 django-service-urls-1.4.1/django_service_urls.egg-info/dependency_links.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)        1 2023-06-27 13:45:58.000000 django-service-urls-1.4.1/django_service_urls.egg-info/not-zip-safe
+-rw-rw-r--   0 raf       (1000) raf       (1000)        7 2023-06-27 13:45:58.000000 django-service-urls-1.4.1/django_service_urls.egg-info/requires.txt
+-rw-rw-r--   0 raf       (1000) raf       (1000)       13 2023-06-27 13:45:58.000000 django-service-urls-1.4.1/django_service_urls.egg-info/top_level.txt
+-rw-r--r--   0 raf       (1000) raf       (1000)     3091 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/pyproject.toml
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:45:59.010716 django-service-urls-1.4.1/service_urls/
+-rw-r--r--   0 raf       (1000) raf       (1000)     1696 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/service_urls/__init__.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     4486 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/service_urls/base.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     3235 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/service_urls/patch.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     9938 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/service_urls/services.py
+-rw-r--r--   0 raf       (1000) raf       (1000)     2152 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/service_urls/version.py
+-rw-rw-r--   0 raf       (1000) raf       (1000)       38 2023-06-27 13:45:59.014716 django-service-urls-1.4.1/setup.cfg
+drwxrwxr-x   0 raf       (1000) raf       (1000)        0 2023-06-27 13:45:59.014716 django-service-urls-1.4.1/tests/
+-rw-r--r--   0 raf       (1000) raf       (1000)     3215 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/tests/test_django.py
+-rw-r--r--   0 raf       (1000) raf       (1000)    21489 2023-06-27 13:45:15.000000 django-service-urls-1.4.1/tests/test_services.py
```

### Comparing `django-service-urls-1.4/CHANGELOG.md` & `django-service-urls-1.4.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 
-## dev
+## 1.4.1
+
+* update memcache service protocols in README.md
+
+## 1.4.0
 
 * add support for `django.core.cache.backends.memcached.PyMemcacheCache` as `pymemcached:` protocol
 * rename `memcached+pylibmccache` protocol to `pylibmccache`
 * fix parsing of `pylibmccache` service
 * add support for Python 3.12
 * add nox support
 * test `service_urls.patch` (monkeypatch django settings)
```

### Comparing `django-service-urls-1.4/LICENSE` & `django-service-urls-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/PKG-INFO` & `django-service-urls-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-service-urls
-Version: 1.4
+Version: 1.4.1
 Summary: setting helper for django to represent databases, caches and email settings via a single string
 Author-email: Raffaele Salmaso <raffaele.salmaso@gmail.com>
 License: BSD
 Project-URL: GitHub, https://github.com/rsalmaso/django-service-urls
 Project-URL: Changelog, https://github.com/rsalmaso/django-service-urls/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -114,22 +114,26 @@
 Service | Backend | URLString
 --------|---------|-----------
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://abc
 Database | django.core.cache.backends.db.DatabaseCache | db://table-name
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://abc
+PyMemcached: single ip | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567
+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567
 Memcached: single ip | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567
-Memcached+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567
+PyMemcached multiple ips | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567,1.2.3.5:1568
+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567,1.2.3.5:1568
 Memcached multiple ips | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567,1.2.3.5:1568
-Memcached+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567,1.2.3.5:1568
+PyMemcached no port | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4
+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4
 Memcached no port | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4
-Memcached+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4
+PyMemcached unix socket | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached:///tmp/memcached.sock
+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache:///tmp/memcached.sock
 Memcached unix socket | django.core.cache.backends.memcached.MemcachedCache | memcached:///tmp/memcached.sock
-Memcached+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache:///tmp/memcached.sock
 File | django.core.cache.backends.filebased.FileBasedCache | file://C:/abc/def/xyz
 File | django.core.cache.backends.filebased.FileBasedCache | file:///abc/def/xyz
 
 ### EMAIL (``service_urls.email``)
 
 Service | Backend | URLString
 --------|---------|-----------
```

### Comparing `django-service-urls-1.4/README.md` & `django-service-urls-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -81,22 +81,26 @@
 Service | Backend | URLString
 --------|---------|-----------
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://abc
 Database | django.core.cache.backends.db.DatabaseCache | db://table-name
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://abc
+PyMemcached: single ip | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567
+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567
 Memcached: single ip | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567
-Memcached+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567
+PyMemcached multiple ips | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567,1.2.3.5:1568
+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567,1.2.3.5:1568
 Memcached multiple ips | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567,1.2.3.5:1568
-Memcached+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567,1.2.3.5:1568
+PyMemcached no port | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4
+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4
 Memcached no port | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4
-Memcached+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4
+PyMemcached unix socket | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached:///tmp/memcached.sock
+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache:///tmp/memcached.sock
 Memcached unix socket | django.core.cache.backends.memcached.MemcachedCache | memcached:///tmp/memcached.sock
-Memcached+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache:///tmp/memcached.sock
 File | django.core.cache.backends.filebased.FileBasedCache | file://C:/abc/def/xyz
 File | django.core.cache.backends.filebased.FileBasedCache | file:///abc/def/xyz
 
 ### EMAIL (``service_urls.email``)
 
 Service | Backend | URLString
 --------|---------|-----------
```

### Comparing `django-service-urls-1.4/django_service_urls.egg-info/PKG-INFO` & `django-service-urls-1.4.1/django_service_urls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-service-urls
-Version: 1.4
+Version: 1.4.1
 Summary: setting helper for django to represent databases, caches and email settings via a single string
 Author-email: Raffaele Salmaso <raffaele.salmaso@gmail.com>
 License: BSD
 Project-URL: GitHub, https://github.com/rsalmaso/django-service-urls
 Project-URL: Changelog, https://github.com/rsalmaso/django-service-urls/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -114,22 +114,26 @@
 Service | Backend | URLString
 --------|---------|-----------
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://
 Memory | django.core.cache.backends.locmem.LocMemCache | memory://abc
 Database | django.core.cache.backends.db.DatabaseCache | db://table-name
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://
 Dummy | django.core.cache.backends.dummy.DummyCache | dummy://abc
+PyMemcached: single ip | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567
+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567
 Memcached: single ip | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567
-Memcached+PyLibMCCache: single ip | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567
+PyMemcached multiple ips | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4:1567,1.2.3.5:1568
+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4:1567,1.2.3.5:1568
 Memcached multiple ips | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4:1567,1.2.3.5:1568
-Memcached+PyLibMCCache multiple ips | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4:1567,1.2.3.5:1568
+PyMemcached no port | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached://1.2.3.4
+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache://1.2.3.4
 Memcached no port | django.core.cache.backends.memcached.MemcachedCache | memcached://1.2.3.4
-Memcached+PyLibMCCache no port | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache://1.2.3.4
+PyMemcached unix socket | django.core.cache.backends.memcached.PyMemcachedCache | pymemcached:///tmp/memcached.sock
+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | pylibmccache:///tmp/memcached.sock
 Memcached unix socket | django.core.cache.backends.memcached.MemcachedCache | memcached:///tmp/memcached.sock
-Memcached+PyLibMCCache unix socket | django.core.cache.backends.memcached.PyLibMCCache | memcached+pylibmccache:///tmp/memcached.sock
 File | django.core.cache.backends.filebased.FileBasedCache | file://C:/abc/def/xyz
 File | django.core.cache.backends.filebased.FileBasedCache | file:///abc/def/xyz
 
 ### EMAIL (``service_urls.email``)
 
 Service | Backend | URLString
 --------|---------|-----------
```

### Comparing `django-service-urls-1.4/pyproject.toml` & `django-service-urls-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/service_urls/__init__.py` & `django-service-urls-1.4.1/service_urls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
 # THE POSSIBILITY OF SUCH DAMAGE.
 
 from .base import Service  # noqa: F401
 from .services import cache, db, email  # noqa: F401
 from .version import get_version
 
-VERSION = (1, 4, 0, "final", 0)
+VERSION = (1, 4, 1, "final", 0)
 
 __version__ = get_version(VERSION)
 __author__ = "Raffaele Salmaso"
 __email__ = "raffele@salmaso.org"
```

### Comparing `django-service-urls-1.4/service_urls/base.py` & `django-service-urls-1.4.1/service_urls/base.py`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/service_urls/patch.py` & `django-service-urls-1.4.1/service_urls/patch.py`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/service_urls/services.py` & `django-service-urls-1.4.1/service_urls/services.py`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/service_urls/version.py` & `django-service-urls-1.4.1/service_urls/version.py`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/tests/test_django.py` & `django-service-urls-1.4.1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `django-service-urls-1.4/tests/test_services.py` & `django-service-urls-1.4.1/tests/test_services.py`

 * *Files identical despite different names*

