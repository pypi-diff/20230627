# Comparing `tmp/django-localized-recurrence-4.0.0.tar.gz` & `tmp/django-localized-recurrence-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-localized-recurrence-4.0.0.tar", last modified: Tue Dec 29 07:54:05 2020, max compression
+gzip compressed data, was "django-localized-recurrence-4.1.0.tar", last modified: Tue Jun 27 20:01:29 2023, max compression
```

## Comparing `django-localized-recurrence-4.0.0.tar` & `django-localized-recurrence-4.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)        1 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/not-zip-safe
--rwxr-xr-x   0 root         (0) root         (0)     2139 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       86 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)      987 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)       21 2020-12-29 07:54:04.000000 django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     1093 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/localized_recurrence/
--rwxr-xr-x   0 root         (0) root         (0)      392 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/admin.py
--rwxr-xr-x   0 root         (0) root         (0)      169 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/apps.py
--rwxr-xr-x   0 root         (0) root         (0)     4976 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/fields.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/
--rwxr-xr-x   0 root         (0) root         (0)     1175 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)      522 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/0002_localizedrecurrence_offset2.py
--rwxr-xr-x   0 root         (0) root         (0)      705 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/0003_offset_data_migration.py
--rwxr-xr-x   0 root         (0) root         (0)      623 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/0004_auto_20161108_2151.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10526 2020-12-29 07:46:22.000000 django-localized-recurrence-4.0.0/localized_recurrence/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/localized_recurrence/tests/
--rwxr-xr-x   0 root         (0) root         (0)      828 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/tests/admin_tests.py
--rwxr-xr-x   0 root         (0) root         (0)     7527 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/tests/fields_tests.py
--rwxr-xr-x   0 root         (0) root         (0)    23785 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/tests/models_tests.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       23 2020-12-29 07:27:03.000000 django-localized-recurrence-4.0.0/localized_recurrence/version.py
--rwxr-xr-x   0 root         (0) root         (0)      128 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/localized_recurrence/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       37 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)     2139 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1033 2020-12-29 07:25:28.000000 django-localized-recurrence-4.0.0/README.rst
--rwxr-xr-x   0 root         (0) root         (0)      269 2020-12-29 07:54:05.000000 django-localized-recurrence-4.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1870 2020-12-29 07:27:40.000000 django-localized-recurrence-4.0.0/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1074 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       35 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1902 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1002 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1902 2023-06-27 20:01:29.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      987 2023-06-27 20:01:29.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-27 20:01:29.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-27 20:01:28.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       70 2023-06-27 20:01:29.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       21 2023-06-27 20:01:29.000000 django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/localized_recurrence/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      124 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      375 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/admin.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      163 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3872 2023-06-27 19:50:08.000000 django-localized-recurrence-4.1.0/localized_recurrence/fields.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/localized_recurrence/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1145 2023-06-27 19:34:08.000000 django-localized-recurrence-4.1.0/localized_recurrence/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      501 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/migrations/0002_localizedrecurrence_offset2.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      681 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/migrations/0003_offset_data_migration.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      598 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/migrations/0004_auto_20161108_2151.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    10268 2023-06-27 19:33:31.000000 django-localized-recurrence-4.1.0/localized_recurrence/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/localized_recurrence/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      801 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/tests/admin_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7304 2023-06-27 19:41:12.000000 django-localized-recurrence-4.1.0/localized_recurrence/tests/fields_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    23235 2023-01-09 15:25:59.000000 django-localized-recurrence-4.1.0/localized_recurrence/tests/models_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-27 19:55:24.000000 django-localized-recurrence-4.1.0/localized_recurrence/version.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      269 2023-06-27 20:01:29.113021 django-localized-recurrence-4.1.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1854 2023-06-27 19:30:36.000000 django-localized-recurrence-4.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/PKG-INFO` & `django-localized-recurrence-4.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-localized-recurrence
-Version: 4.0.0
+Version: 4.1.0
 Summary: Store events that recur in users' local times.
-Home-page: UNKNOWN
 Author: Erik Swanson
 Author-email: theerikswanson@gmail.com
 License: MIT License
-Description: .. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
-            :target: https://travis-ci.org/Wilduck/django-localized-recurrence
-        
-        Django Localized Recurrence
-        ===========================
-        Django Localized Recurrence allowes you to store events that recur in
-        users' local times, and not have to worry about things like
-        
-        This django app provides a model, ``LocalizedRecurrence``, with
-        methods to help store recurring events, check if the events are due,
-        and update their next scheduled time.
-        
-        Installation
-        ------------
-        This packages is currently available through Pypi and github. To
-        install from Pypi using ``pip`` (recommended)::
-        
-            pip install django-localized-recurrence
-        
-        
-        To install the development version from github::
-        
-            pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
-        
-        Documentation
-        -------------
-        Full documentation is available at http://django-localized-recurrence.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
+    :target: https://travis-ci.org/Wilduck/django-localized-recurrence
+
+Django Localized Recurrence
+===========================
+Django Localized Recurrence allowes you to store events that recur in
+users' local times, and not have to worry about things like
+
+This django app provides a model, ``LocalizedRecurrence``, with
+methods to help store recurring events, check if the events are due,
+and update their next scheduled time.
+
+Installation
+------------
+This packages is currently available through Pypi and github. To
+install from Pypi using ``pip`` (recommended)::
+
+    pip install django-localized-recurrence
+
+
+To install the development version from github::
+
+    pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
+
+Documentation
+-------------
+Full documentation is available at http://django-localized-recurrence.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-localized-recurrence-4.0.0/django_localized_recurrence.egg-info/SOURCES.txt` & `django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-localized-recurrence-4.0.0/LICENSE` & `django-localized-recurrence-4.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2014 Ambition
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+The MIT License (MIT)
+
+Copyright (c) 2014 Ambition
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/fields.py` & `django-localized-recurrence-4.1.0/localized_recurrence/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,105 @@
-from datetime import timedelta
-import re
-
-from django.db.models.fields import IntegerField
-import six
-
-
-class CastOnAssignDescriptor(object):
-    """
-    A property descriptor which ensures that `field.to_python()` is called on _every_ assignment to the field.
-    This used to be provided by the `django.db.models.subclassing.Creator` class, which in turn
-    was used by the deprecated-in-Django-1.10 `SubfieldBase` class, hence the reimplementation here.
-    https://stackoverflow.com/questions/39392343/
-    how-do-i-make-a-custom-model-field-call-to-python-when-the-field-is-accessed-imm
-    """
-
-    def __init__(self, field):
-        self.field = field
-
-    def __get__(self, obj, type=None):  # pragma: no cover
-        if obj is None:
-            return self
-        return obj.__dict__[self.field.name]
-
-    def __set__(self, obj, value):  # pragma: no cover
-        obj.__dict__[self.field.name] = self.field.to_python(value)
-
-
-class DurationField(IntegerField):
-    """A field to store durations of time with accuracy to the second.
-
-    A Duration Field will automatically convert between python
-    timedelta objects and database integers.
-
-    Duration fields can be used to define fields in a django model
-
-    .. code-block:: python
-
-        class Presentations(models.Model):
-            length = DurationField()
-            speaker = models.ForeignKey(User)
-            location = models.ForeignKey(Location)
-
-    Given such a model, storing a duration in the database is as
-    simple as passing in a ``timedelta`` object
-
-    .. code-block:: python
-
-        >>> Presentations.objects.create(
-        ...     length=datetime.timedelta(minutes=45),
-        ...     speaker=User.objects.get(email='MrT@example.com'),
-        ...     location=wrestle_mania_ring,
-        ... )
-
-    The timedeltas are stored as seconds in the backend, so sub-second
-    accuracy is lost with this field.
-
-    """
-    description = "A duration of time."
-
-    def __init__(self, *args, **kwargs):
-        """Call out to the super. Makes docs cleaner."""
-        return super(DurationField, self).__init__(*args, **kwargs)
-
-    def contribute_to_class(self, cls, name):
-        super(DurationField, self).contribute_to_class(cls, name)
-        setattr(cls, name, CastOnAssignDescriptor(self))
-
-    def to_python(self, value):
-        """Convert a stored duration into a python datetime.timedelta object.
-
-        Need to handle three cases:
-            - An instance of the correct type (timedelta).
-            - A string (e.g., from a deserializer).
-            - What the database returns (integer).
-        """
-        if isinstance(value, timedelta):
-            v = value
-        elif isinstance(value, (six.binary_type, six.text_type)):
-            # The string should be in the form "[D day[s],][H]H:MM:SS[.UUUUUU]"
-            try:
-                v = parse_timedelta_string(value)
-            except ValueError:
-                raise ValueError("Duration string must be in the form '[D day[s],][H]H:MM:SS[.UUUUUU]'")
-        elif isinstance(value, int):
-            v = timedelta(seconds=value)
-        elif value is None:
-            v = None
-        else:
-            raise ValueError("Not a valid Duration object")
-        return v
-
-    def deconstruct(self):
-        name, path, args, kwargs = super(DurationField, self).deconstruct()
-        if 'default' in kwargs.keys():
-            kwargs['default'] = self.get_prep_value(kwargs['default'])
-        return name, 'localized_recurrence.fields.DurationField', args, kwargs
-
-    def get_prep_value(self, value):
-        """Convert a timedelta to integer for storage.
-        """
-        value = self.to_python(value)
-        return int(value.total_seconds())
-
-    def value_to_string(self, obj):
-        """Used by serializers to get a string representation.
-        """
-        time_delta_value = self._get_val_from_obj(obj)
-        return str(time_delta_value)
-
-
-def parse_timedelta_string(string):
-    """Parses strings from datetime.timedelta.__str__.
-
-    Usefull because django's force_text uses .__str__ instead of
-    .__repr__
-
-    datetime.timedelta.__str__ returns a string in the form [D day[s],
-    ][H]H:MM:SS[.UUUUUU], where D is negative for negative t.
-    """
-    days_re = r"(?P<days>-?[0-9]*) days?, (?P<hours>[0-9]+):(?P<minutes>[0-9]+):(?P<seconds>[0-9]+\.?[0-9]*)"
-    no_days_re = r"(?P<hours>[0-9]+):(?P<minutes>[0-9]+):(?P<seconds>[0-9]+\.?[0-9]*)"
-    match_days = re.match(days_re, string)
-    match_no_days = re.match(no_days_re, string)
-    if match_days:
-        return timedelta(**{k: float(v) for k, v in match_days.groupdict().items()})
-    elif match_no_days:
-        return timedelta(**{k: float(v) for k, v in match_no_days.groupdict().items()})
-    else:
-        raise ValueError("'%s' is not in the form [D day[s],][H]H:MM:SS[.UUUUUU]" % string)
+from datetime import timedelta
+import re
+
+from django.db.models.fields import IntegerField
+from ambition_utils.fields import CastOnAssignFieldMixin
+
+
+class DurationField(CastOnAssignFieldMixin, IntegerField):
+    """A field to store durations of time with accuracy to the second.
+
+    A Duration Field will automatically convert between python
+    timedelta objects and database integers.
+
+    Duration fields can be used to define fields in a django model
+
+    .. code-block:: python
+
+        class Presentations(models.Model):
+            length = DurationField()
+            speaker = models.ForeignKey(User)
+            location = models.ForeignKey(Location)
+
+    Given such a model, storing a duration in the database is as
+    simple as passing in a ``timedelta`` object
+
+    .. code-block:: python
+
+        >>> Presentations.objects.create(
+        ...     length=datetime.timedelta(minutes=45),
+        ...     speaker=User.objects.get(email='MrT@example.com'),
+        ...     location=wrestle_mania_ring,
+        ... )
+
+    The timedeltas are stored as seconds in the backend, so sub-second
+    accuracy is lost with this field.
+
+    """
+    description = "A duration of time."
+
+    def __init__(self, *args, **kwargs):
+        """Call out to the super. Makes docs cleaner."""
+        return super().__init__(*args, **kwargs)
+
+    def to_python(self, value):
+        """Convert a stored duration into a python datetime.timedelta object.
+
+        Need to handle three cases:
+            - An instance of the correct type (timedelta).
+            - A string (e.g., from a deserializer).
+            - What the database returns (integer).
+        """
+        if isinstance(value, timedelta):
+            v = value
+        elif isinstance(value, (bytes, str)):
+            # The string should be in the form "[D day[s],][H]H:MM:SS[.UUUUUU]"
+            try:
+                v = parse_timedelta_string(value)
+            except ValueError:
+                raise ValueError("Duration string must be in the form '[D day[s],][H]H:MM:SS[.UUUUUU]'")
+        elif isinstance(value, int):
+            v = timedelta(seconds=value)
+        elif value is None:
+            v = None
+        else:
+            raise ValueError("Not a valid Duration object")
+        return v
+
+    def deconstruct(self):
+        name, path, args, kwargs = super(DurationField, self).deconstruct()
+        if 'default' in kwargs.keys():
+            kwargs['default'] = self.get_prep_value(kwargs['default'])
+        return name, 'localized_recurrence.fields.DurationField', args, kwargs
+
+    def get_prep_value(self, value):
+        """Convert a timedelta to integer for storage.
+        """
+        value = self.to_python(value)
+        return int(value.total_seconds())
+
+    def value_to_string(self, obj):
+        """Used by serializers to get a string representation.
+        """
+        time_delta_value = self._get_val_from_obj(obj)
+        return str(time_delta_value)
+
+
+def parse_timedelta_string(string):
+    """Parses strings from datetime.timedelta.__str__.
+
+    Usefull because django's force_text uses .__str__ instead of
+    .__repr__
+
+    datetime.timedelta.__str__ returns a string in the form [D day[s],
+    ][H]H:MM:SS[.UUUUUU], where D is negative for negative t.
+    """
+    days_re = r"(?P<days>-?[0-9]*) days?, (?P<hours>[0-9]+):(?P<minutes>[0-9]+):(?P<seconds>[0-9]+\.?[0-9]*)"
+    no_days_re = r"(?P<hours>[0-9]+):(?P<minutes>[0-9]+):(?P<seconds>[0-9]+\.?[0-9]*)"
+    match_days = re.match(days_re, string)
+    match_no_days = re.match(no_days_re, string)
+    if match_days:
+        return timedelta(**{k: float(v) for k, v in match_days.groupdict().items()})
+    elif match_no_days:
+        return timedelta(**{k: float(v) for k, v in match_no_days.groupdict().items()})
+    else:
+        raise ValueError("'%s' is not in the form [D day[s],][H]H:MM:SS[.UUUUUU]" % string)
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/migrations/0001_initial.py` & `django-localized-recurrence-4.1.0/localized_recurrence/migrations/0001_initial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-
-from django.db import models, migrations
-import timezone_field.fields
-import localized_recurrence.fields
-import datetime
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='LocalizedRecurrence',
-            fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('interval', models.CharField(default='DAY', choices=[('DAY', 'Day'), ('WEEK', 'Week'), ('MONTH', 'Month'), ('QUARTER', 'Quarter'), ('YEAR', 'Year')], max_length=18)),
-                ('offset', localized_recurrence.fields.DurationField(default=0)),
-                ('timezone', timezone_field.fields.TimeZoneField(default='UTC')),
-                ('previous_scheduled', models.DateTimeField(default=datetime.datetime(1970, 1, 1, 0, 0))),
-                ('next_scheduled', models.DateTimeField(default=datetime.datetime(1970, 1, 1, 0, 0))),
-            ],
-            options={
-            },
-            bases=(models.Model,),
-        ),
-    ]
+# -*- coding: utf-8 -*-
+from __future__ import unicode_literals
+
+from django.db import models, migrations
+import ambition_utils.fields
+import localized_recurrence.fields
+import datetime
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='LocalizedRecurrence',
+            fields=[
+                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
+                ('interval', models.CharField(default='DAY', choices=[('DAY', 'Day'), ('WEEK', 'Week'), ('MONTH', 'Month'), ('QUARTER', 'Quarter'), ('YEAR', 'Year')], max_length=18)),
+                ('offset', localized_recurrence.fields.DurationField(default=0)),
+                ('timezone', ambition_utils.fields.TimeZoneField(default='UTC')),
+                ('previous_scheduled', models.DateTimeField(default=datetime.datetime(1970, 1, 1, 0, 0))),
+                ('next_scheduled', models.DateTimeField(default=datetime.datetime(1970, 1, 1, 0, 0))),
+            ],
+            options={
+            },
+            bases=(models.Model,),
+        ),
+    ]
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/migrations/0003_offset_data_migration.py` & `django-localized-recurrence-4.1.0/localized_recurrence/migrations/0003_offset_data_migration.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# -*- coding: utf-8 -*-
-
-from __future__ import unicode_literals
-
-from datetime import timedelta
-from django.db import migrations
-
-
-def migrate_integers_to_intervals(apps, schema_editor):
-    # Migrate custom DurationField values to Django's Native DurationField values
-    LocalizedRecurrence = apps.get_model('localized_recurrence', 'LocalizedRecurrence')
-    for lr in LocalizedRecurrence.objects.all():
-        lr.offset2 = lr.offset
-        lr.save()
-
-
-class Migration(migrations.Migration):
-    dependencies = [
-        ('localized_recurrence', '0002_localizedrecurrence_offset2'),
-    ]
-
-    operations = [
-        migrations.RunPython(migrate_integers_to_intervals),
-    ]
+# -*- coding: utf-8 -*-
+
+from __future__ import unicode_literals
+
+from datetime import timedelta
+from django.db import migrations
+
+
+def migrate_integers_to_intervals(apps, schema_editor):
+    # Migrate custom DurationField values to Django's Native DurationField values
+    LocalizedRecurrence = apps.get_model('localized_recurrence', 'LocalizedRecurrence')
+    for lr in LocalizedRecurrence.objects.all():
+        lr.offset2 = lr.offset
+        lr.save()
+
+
+class Migration(migrations.Migration):
+    dependencies = [
+        ('localized_recurrence', '0002_localizedrecurrence_offset2'),
+    ]
+
+    operations = [
+        migrations.RunPython(migrate_integers_to_intervals),
+    ]
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/models.py` & `django-localized-recurrence-4.1.0/localized_recurrence/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-from datetime import datetime, timedelta
-import calendar
-
-from dateutil.relativedelta import relativedelta
-from django.db import models
-from timezone_field import TimeZoneField
-import fleming
-import pytz
-
-
-INTERVAL_CHOICES = (
-    ('DAY', 'Day'),
-    ('WEEK', 'Week'),
-    ('MONTH', 'Month'),
-    ('QUARTER', 'Quarter'),
-    ('YEAR', 'Year'),
-)
-
-
-class LocalizedRecurrenceQuerySet(models.query.QuerySet):
-    def update_schedule(self, time=None):
-        """
-        Update the schedule times for all the provided recurrences.
-
-        :type time: :py:class:`datetime.datetime`
-        :param time: The time the schedule was checked. If ``None``,
-            defaults to ``datetime.utcnow()``.
-
-        In the common case, this can be called without any arguments.
-
-        .. code-block:: python
-
-            >>> past_due = LocalizedRecurrence.objects.filter(
-            ...     next_scheduled__lte=datetime.utcnow()
-            ... )
-            >>> # Do something with past_due recurrences
-            >>> past_due.update_schedule()
-
-        The code above will ensure that all the processed recurrences
-        are re-scheduled for their next recurrence.
-
-        Calling this function has the side effect that the
-        ``next_scheduled`` attribute of every recurrence in the
-        queryset will be updated to the new time in utc.
-        """
-        _update_schedule(self, time=time)
-
-
-class LocalizedRecurrenceManager(models.Manager):
-    def get_queryset(self):
-        return LocalizedRecurrenceQuerySet(self.model)
-
-    def update_schedule(self, time=None):
-        """
-        Update the schedule times for all recurrences.
-
-        Functions exactly the same as the method on the querysets. The
-        following to calls are equivalent:
-
-        .. code-block:: python
-
-            >>> LocalizedRecurrence.objects.all().update_schedule()
-            >>> LocalizedRecurrence.objects.update_schedule()
-
-        Calling this function has the side effect that the
-        ``next_scheduled`` attribute of every recurrence will be
-        updated to the new time in utc.
-        """
-        self.get_queryset().update_schedule(time=time)
-
-
-class LocalizedRecurrence(models.Model):
-    """The information necessary to act on events in users local
-    times. Can be instantiated with ``LocalizedRecurrence.objects.create``
-
-    :type interval: str
-    :param interval: The interval at which the event recurs.
-        One of ``'DAY'``, ``'WEEK'``, ``'MONTH'``, ``'QUARTER'``, ``'YEAR'``.
-
-    :type offset: :py:class:`datetime.timedelta`
-    :param offset: The amount of time into the interval that the event
-        occurs at.
-
-        If the interval is monthly, quarterly, or yearly, the number
-        of days in the interval are variable. In the case of offsets
-        with more days than the number of days in the interval,
-        updating the schedule will not raise an error, but will update
-        to the last day in the interval if necessary.
-
-    :type timezone: pytz.timezone
-    :param timezone: The local timezone for the user.
-
-    Localized recurrences are simply objects in the database. They can
-    be created with standard django ORM tools:
-
-    .. code-block:: python
-
-        >>> from datetime import datetime, timedelta
-        >>> my_lr = LocalizedRecurrence.objects.create(
-        ...     interval='DAY',
-        ...     offset=timedela(hours=15),
-        ...     timezone=pytz.timedelta('US/Eastern'),
-        ... )
-
-    Once instantiated it is simple to check if a localized recurrence
-    is due to be acted upon.
-
-    .. code-block:: python
-
-        >>> my_lr.next_scheduled < datetime.utcnow()
-        True
-
-    After a recurrence has been acted upon, it's schedule can be
-    simply reset to occur at the prescribed time in the next interval.
-
-    .. code-block:: python
-
-        >>> my_lr.update_schedule()
-        >>> my_lr.next_scheduled < datetime.utcnow()
-        False
-
-    """
-    interval = models.CharField(max_length=18, default='DAY', choices=INTERVAL_CHOICES)
-    offset = models.DurationField(default=timedelta(0))
-    timezone = TimeZoneField(default='UTC')
-    previous_scheduled = models.DateTimeField(default=datetime(1970, 1, 1))
-    next_scheduled = models.DateTimeField(default=datetime(1970, 1, 1))
-
-    objects = LocalizedRecurrenceManager()
-
-    def __str__(self):
-        return 'ID: {0}, Interval: {1}, Next Scheduled: {2}'.format(self.id, self.interval, self.next_scheduled)
-
-    def update(self, **updates):
-        """Updates fields in the localized recurrence."""
-        for update in updates:
-            setattr(self, update, updates[update])
-
-        return self.save()
-
-    def update_schedule(self, time=None):
-        """
-        Update the schedule for this recurrence or an object it tracks.
-
-        :type time: :py:class:`datetime.datetime`
-        :param time: The time the schedule was checked. If ``None``,
-            defaults to ``datetime.utcnow()``.
-
-        Calling this function has the side effect that the
-        ``next_scheduled`` attribute will be updated to the new time
-        in utc.
-        """
-        _update_schedule([self], time)
-
-    def utc_of_next_schedule(self, current_time):
-        """
-        Generates the next recurrence time in utc after the current time
-
-        :type current_time: :py:class:`datetime.datetime`
-        :param current_time: The current time in utc.
-
-        Usually this function does not need to be called directly, but
-        will be used by ``update_schedule``. If however, you need to
-        check when the next recurrence of a instance would happen,
-        without persisting an update to the schedule, this function
-        can be called without side-effect.
-        """
-        # Make a copy of the next scheduled datetime
-        next_scheduled_utc = datetime(
-            self.next_scheduled.year, self.next_scheduled.month, self.next_scheduled.day,
-            self.next_scheduled.hour, self.next_scheduled.minute, self.next_scheduled.second
-        )
-
-        additional_time = {
-            'DAY': timedelta(days=1),
-            'WEEK': timedelta(weeks=1),
-            'MONTH': relativedelta(months=1),
-            'QUARTER': relativedelta(months=3),
-            'YEAR': relativedelta(years=1),
-        }
-
-        # Keep updating next scheduled to the next recurrence until it is greater than current time
-        while next_scheduled_utc <= current_time:
-            # Convert to local time
-            next_scheduled_local = fleming.convert_to_tz(next_scheduled_utc, self.timezone)
-
-            # Replace with the offset data
-            replaced_with_offset = _replace_with_offset(next_scheduled_local, self.offset, self.interval)
-
-            # Normalize to handle dst
-            local_scheduled_time = fleming.fleming.dst_normalize(replaced_with_offset)
-
-            # Add the time delta
-            next_local_scheduled_time = fleming.add_timedelta(
-                local_scheduled_time,
-                additional_time[self.interval],
-                within_tz=self.timezone
-            )
-
-            # Check if last day of month
-            is_last_day = self.interval == 'MONTH' and self.offset.days >= 28
-
-            # Check if we need to manually set the day to the next month's last day rather than apply the offset info
-            if self.interval == 'MONTH' and is_last_day:
-                _, last_day_of_next_month = calendar.monthrange(
-                    next_local_scheduled_time.year,
-                    next_local_scheduled_time.month
-                )
-
-                # Replace day with last day of month
-                next_local_scheduled_time = next_local_scheduled_time.replace(day=last_day_of_next_month)
-            else:
-                # Apply the offset info for all cases that are not end of month
-                next_local_scheduled_time = _replace_with_offset(next_local_scheduled_time, self.offset, self.interval)
-
-            # Convert back to utc
-            next_scheduled_utc = fleming.convert_to_tz(next_local_scheduled_time, pytz.utc, return_naive=True)
-
-        return next_scheduled_utc
-
-
-def _update_schedule(recurrences, time=None):
-    """
-    Update the schedule times for all the provided recurrences.
-    """
-    time = time or datetime.utcnow()
-    for recurrence in recurrences:
-        recurrence.next_scheduled = recurrence.utc_of_next_schedule(time)
-        recurrence.previous_scheduled = time
-        recurrence.save()
-
-
-def _replace_with_offset(dt, offset, interval):
-    """
-    Replace components of a datetime with those of a timedelta.
-
-    This replacement is done within the given interval. This means the
-    the final result, will the be a datetime, at the desired offset
-    given the interval.
-    """
-    hours, minutes, seconds = offset.seconds // 3600, (offset.seconds // 60) % 60, offset.seconds % 60
-    interval = interval.lower()
-    if interval == 'day':
-        dt_out = dt.replace(hour=hours, minute=minutes, second=seconds)
-    elif interval == 'week':
-        dt_out = dt + timedelta(days=offset.days - dt.weekday())
-        dt_out = dt_out.replace(hour=hours, minute=minutes, second=seconds)
-    elif interval == 'month':
-        _, last_day = calendar.monthrange(dt.year, dt.month)
-        day = (offset.days + 1) if (offset.days + 1) <= last_day else last_day
-        dt_out = dt.replace(day=day, hour=hours, minute=minutes, second=seconds)
-    elif interval == 'quarter':
-        month_range = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]][int((dt.month - 1) / 3)]
-        quarter_days = sum(calendar.monthrange(dt.year, month)[1] for month in month_range)
-        days = offset.days if offset.days <= (quarter_days - 1) else (quarter_days - 1)
-        dt_out = fleming.floor(dt, month=3).replace(hour=hours, minute=minutes, second=seconds)
-        dt_out += timedelta(days)
-    elif interval == 'year':
-        leap_year_extra_days = 1 if calendar.isleap(dt.year) else 0
-        days = offset.days if offset.days <= 364 + leap_year_extra_days else 364 + leap_year_extra_days
-        dt_out = fleming.floor(dt, year=1).replace(hour=hours, minute=minutes, second=seconds)
-        dt_out += timedelta(days)
-    else:
-        raise ValueError('{i} is not a proper interval value'.format(i=interval))
-    return dt_out
+from datetime import datetime, timedelta
+import calendar
+
+from dateutil.relativedelta import relativedelta
+from django.db import models
+from ambition_utils.fields import TimeZoneField
+import fleming
+import pytz
+
+
+INTERVAL_CHOICES = (
+    ('DAY', 'Day'),
+    ('WEEK', 'Week'),
+    ('MONTH', 'Month'),
+    ('QUARTER', 'Quarter'),
+    ('YEAR', 'Year'),
+)
+
+
+class LocalizedRecurrenceQuerySet(models.query.QuerySet):
+    def update_schedule(self, time=None):
+        """
+        Update the schedule times for all the provided recurrences.
+
+        :type time: :py:class:`datetime.datetime`
+        :param time: The time the schedule was checked. If ``None``,
+            defaults to ``datetime.utcnow()``.
+
+        In the common case, this can be called without any arguments.
+
+        .. code-block:: python
+
+            >>> past_due = LocalizedRecurrence.objects.filter(
+            ...     next_scheduled__lte=datetime.utcnow()
+            ... )
+            >>> # Do something with past_due recurrences
+            >>> past_due.update_schedule()
+
+        The code above will ensure that all the processed recurrences
+        are re-scheduled for their next recurrence.
+
+        Calling this function has the side effect that the
+        ``next_scheduled`` attribute of every recurrence in the
+        queryset will be updated to the new time in utc.
+        """
+        _update_schedule(self, time=time)
+
+
+class LocalizedRecurrenceManager(models.Manager):
+    def get_queryset(self):
+        return LocalizedRecurrenceQuerySet(self.model)
+
+    def update_schedule(self, time=None):
+        """
+        Update the schedule times for all recurrences.
+
+        Functions exactly the same as the method on the querysets. The
+        following to calls are equivalent:
+
+        .. code-block:: python
+
+            >>> LocalizedRecurrence.objects.all().update_schedule()
+            >>> LocalizedRecurrence.objects.update_schedule()
+
+        Calling this function has the side effect that the
+        ``next_scheduled`` attribute of every recurrence will be
+        updated to the new time in utc.
+        """
+        self.get_queryset().update_schedule(time=time)
+
+
+class LocalizedRecurrence(models.Model):
+    """The information necessary to act on events in users local
+    times. Can be instantiated with ``LocalizedRecurrence.objects.create``
+
+    :type interval: str
+    :param interval: The interval at which the event recurs.
+        One of ``'DAY'``, ``'WEEK'``, ``'MONTH'``, ``'QUARTER'``, ``'YEAR'``.
+
+    :type offset: :py:class:`datetime.timedelta`
+    :param offset: The amount of time into the interval that the event
+        occurs at.
+
+        If the interval is monthly, quarterly, or yearly, the number
+        of days in the interval are variable. In the case of offsets
+        with more days than the number of days in the interval,
+        updating the schedule will not raise an error, but will update
+        to the last day in the interval if necessary.
+
+    :type timezone: pytz.timezone
+    :param timezone: The local timezone for the user.
+
+    Localized recurrences are simply objects in the database. They can
+    be created with standard django ORM tools:
+
+    .. code-block:: python
+
+        >>> from datetime import datetime, timedelta
+        >>> my_lr = LocalizedRecurrence.objects.create(
+        ...     interval='DAY',
+        ...     offset=timedela(hours=15),
+        ...     timezone=pytz.timedelta('US/Eastern'),
+        ... )
+
+    Once instantiated it is simple to check if a localized recurrence
+    is due to be acted upon.
+
+    .. code-block:: python
+
+        >>> my_lr.next_scheduled < datetime.utcnow()
+        True
+
+    After a recurrence has been acted upon, it's schedule can be
+    simply reset to occur at the prescribed time in the next interval.
+
+    .. code-block:: python
+
+        >>> my_lr.update_schedule()
+        >>> my_lr.next_scheduled < datetime.utcnow()
+        False
+
+    """
+    interval = models.CharField(max_length=18, default='DAY', choices=INTERVAL_CHOICES)
+    offset = models.DurationField(default=timedelta(0))
+    timezone = TimeZoneField(default='UTC')
+    previous_scheduled = models.DateTimeField(default=datetime(1970, 1, 1))
+    next_scheduled = models.DateTimeField(default=datetime(1970, 1, 1))
+
+    objects = LocalizedRecurrenceManager()
+
+    def __str__(self):
+        return 'ID: {0}, Interval: {1}, Next Scheduled: {2}'.format(self.id, self.interval, self.next_scheduled)
+
+    def update(self, **updates):
+        """Updates fields in the localized recurrence."""
+        for update in updates:
+            setattr(self, update, updates[update])
+
+        return self.save()
+
+    def update_schedule(self, time=None):
+        """
+        Update the schedule for this recurrence or an object it tracks.
+
+        :type time: :py:class:`datetime.datetime`
+        :param time: The time the schedule was checked. If ``None``,
+            defaults to ``datetime.utcnow()``.
+
+        Calling this function has the side effect that the
+        ``next_scheduled`` attribute will be updated to the new time
+        in utc.
+        """
+        _update_schedule([self], time)
+
+    def utc_of_next_schedule(self, current_time):
+        """
+        Generates the next recurrence time in utc after the current time
+
+        :type current_time: :py:class:`datetime.datetime`
+        :param current_time: The current time in utc.
+
+        Usually this function does not need to be called directly, but
+        will be used by ``update_schedule``. If however, you need to
+        check when the next recurrence of a instance would happen,
+        without persisting an update to the schedule, this function
+        can be called without side-effect.
+        """
+        # Make a copy of the next scheduled datetime
+        next_scheduled_utc = datetime(
+            self.next_scheduled.year, self.next_scheduled.month, self.next_scheduled.day,
+            self.next_scheduled.hour, self.next_scheduled.minute, self.next_scheduled.second
+        )
+
+        additional_time = {
+            'DAY': timedelta(days=1),
+            'WEEK': timedelta(weeks=1),
+            'MONTH': relativedelta(months=1),
+            'QUARTER': relativedelta(months=3),
+            'YEAR': relativedelta(years=1),
+        }
+
+        # Keep updating next scheduled to the next recurrence until it is greater than current time
+        while next_scheduled_utc <= current_time:
+            # Convert to local time
+            next_scheduled_local = fleming.convert_to_tz(next_scheduled_utc, self.timezone)
+
+            # Replace with the offset data
+            replaced_with_offset = _replace_with_offset(next_scheduled_local, self.offset, self.interval)
+
+            # Normalize to handle dst
+            local_scheduled_time = fleming.fleming.dst_normalize(replaced_with_offset)
+
+            # Add the time delta
+            next_local_scheduled_time = fleming.add_timedelta(
+                local_scheduled_time,
+                additional_time[self.interval],
+                within_tz=self.timezone
+            )
+
+            # Check if last day of month
+            is_last_day = self.interval == 'MONTH' and self.offset.days >= 28
+
+            # Check if we need to manually set the day to the next month's last day rather than apply the offset info
+            if self.interval == 'MONTH' and is_last_day:
+                _, last_day_of_next_month = calendar.monthrange(
+                    next_local_scheduled_time.year,
+                    next_local_scheduled_time.month
+                )
+
+                # Replace day with last day of month
+                next_local_scheduled_time = next_local_scheduled_time.replace(day=last_day_of_next_month)
+            else:
+                # Apply the offset info for all cases that are not end of month
+                next_local_scheduled_time = _replace_with_offset(next_local_scheduled_time, self.offset, self.interval)
+
+            # Convert back to utc
+            next_scheduled_utc = fleming.convert_to_tz(next_local_scheduled_time, pytz.utc, return_naive=True)
+
+        return next_scheduled_utc
+
+
+def _update_schedule(recurrences, time=None):
+    """
+    Update the schedule times for all the provided recurrences.
+    """
+    time = time or datetime.utcnow()
+    for recurrence in recurrences:
+        recurrence.next_scheduled = recurrence.utc_of_next_schedule(time)
+        recurrence.previous_scheduled = time
+        recurrence.save()
+
+
+def _replace_with_offset(dt, offset, interval):
+    """
+    Replace components of a datetime with those of a timedelta.
+
+    This replacement is done within the given interval. This means the
+    the final result, will the be a datetime, at the desired offset
+    given the interval.
+    """
+    hours, minutes, seconds = offset.seconds // 3600, (offset.seconds // 60) % 60, offset.seconds % 60
+    interval = interval.lower()
+    if interval == 'day':
+        dt_out = dt.replace(hour=hours, minute=minutes, second=seconds)
+    elif interval == 'week':
+        dt_out = dt + timedelta(days=offset.days - dt.weekday())
+        dt_out = dt_out.replace(hour=hours, minute=minutes, second=seconds)
+    elif interval == 'month':
+        _, last_day = calendar.monthrange(dt.year, dt.month)
+        day = (offset.days + 1) if (offset.days + 1) <= last_day else last_day
+        dt_out = dt.replace(day=day, hour=hours, minute=minutes, second=seconds)
+    elif interval == 'quarter':
+        month_range = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]][int((dt.month - 1) / 3)]
+        quarter_days = sum(calendar.monthrange(dt.year, month)[1] for month in month_range)
+        days = offset.days if offset.days <= (quarter_days - 1) else (quarter_days - 1)
+        dt_out = fleming.floor(dt, month=3).replace(hour=hours, minute=minutes, second=seconds)
+        dt_out += timedelta(days)
+    elif interval == 'year':
+        leap_year_extra_days = 1 if calendar.isleap(dt.year) else 0
+        days = offset.days if offset.days <= 364 + leap_year_extra_days else 364 + leap_year_extra_days
+        dt_out = fleming.floor(dt, year=1).replace(hour=hours, minute=minutes, second=seconds)
+        dt_out += timedelta(days)
+    else:
+        raise ValueError('{i} is not a proper interval value'.format(i=interval))
+    return dt_out
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/tests/admin_tests.py` & `django-localized-recurrence-4.1.0/localized_recurrence/tests/admin_tests.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from django.contrib.admin.sites import AdminSite
-from django.test import TestCase
-
-from localized_recurrence.admin import LocalizedRecurrenceAdmin
-from localized_recurrence.models import LocalizedRecurrence
-
-
-class LocalizedRecurrenceAdminTest(TestCase):
-    """Verify that the admin can load.
-    """
-    def setUp(self):
-        super(LocalizedRecurrenceAdminTest, self).setUp()
-        self.site = AdminSite()
-
-    def test_model_admin_load(self):
-        lr_admin = LocalizedRecurrenceAdmin(LocalizedRecurrence, self.site)
-        self.assertEqual(
-            lr_admin.list_display,
-            [
-                'id',
-                'interval',
-                'timezone',
-                'offset',
-                'previous_scheduled',
-                'next_scheduled'
-            ]
-        )
+from django.contrib.admin.sites import AdminSite
+from django.test import TestCase
+
+from localized_recurrence.admin import LocalizedRecurrenceAdmin
+from localized_recurrence.models import LocalizedRecurrence
+
+
+class LocalizedRecurrenceAdminTest(TestCase):
+    """Verify that the admin can load.
+    """
+    def setUp(self):
+        super(LocalizedRecurrenceAdminTest, self).setUp()
+        self.site = AdminSite()
+
+    def test_model_admin_load(self):
+        lr_admin = LocalizedRecurrenceAdmin(LocalizedRecurrence, self.site)
+        self.assertEqual(
+            lr_admin.list_display,
+            [
+                'id',
+                'interval',
+                'timezone',
+                'offset',
+                'previous_scheduled',
+                'next_scheduled'
+            ]
+        )
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/tests/fields_tests.py` & `django-localized-recurrence-4.1.0/localized_recurrence/tests/fields_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,202 +1,199 @@
-import unittest
-from datetime import timedelta
-
-import django
-import six
-if six.PY3:  # pragma: no cover
-    from importlib import reload
-
-from mock import MagicMock, patch
-
-from .. import fields
-
-
-class DurationFieldToPythonTest(unittest.TestCase):
-    def setUp(self):
-        """Create a mock of the DurationField class and pin to_python to it.
-        """
-        self.df = fields.DurationField()
-        self.df_with_default = fields.DurationField(default=60)
-
-    def test_deconstruct_with_default(self):
-        """
-        Test .deconstruct() with a default
-        """
-        if django.VERSION[1] >= 7:  # pragma: no cover
-            name, path, args, kwargs = self.df_with_default.deconstruct()
-
-            self.assertEqual(kwargs['default'], 60)
-        else:  # pragma: no cover
-            with patch('localized_recurrence.fields.IntegerField.deconstruct', create=True) as mock_deconstruct:
-                mock_deconstruct.return_value = (
-                    'duration', 'django.db.models.IntegerField', [], {'default': timedelta(seconds=60)}
-                )
-                name, path, args, kwargs = self.df_with_default.deconstruct()
-                self.assertEqual(kwargs['default'], 60)
-
-    def test_deconstruct_without_default(self):
-        """
-        Test .deconstruct() without a default
-        """
-        if django.VERSION[1] >= 7:  # pragma: no cover
-            name, path, args, kwargs = self.df.deconstruct()
-            self.assertFalse('default' in kwargs.keys())
-        else:  # pragma: no cover
-            with patch('localized_recurrence.fields.IntegerField.deconstruct', create=True) as mock_deconstruct:
-                mock_deconstruct.return_value = (
-                    'duration', 'django.db.models.IntegerField', [], {}
-                )
-                name, path, args, kwargs = self.df_with_default.deconstruct()
-                self.assertNotIn('default', kwargs.keys())
-
-    def test_timedelta(self):
-        """A timedelta should just get returned.
-        """
-        td_in = timedelta(days=1, hours=3)
-        td_out = self.df.to_python(td_in)
-        self.assertEqual(td_out, td_in)
-
-    def test_string(self):
-        """A string should be properly converted.
-        """
-        td_expected = timedelta(days=3, hours=5, minutes=10)
-        str_in = str(td_expected)
-        td_out = self.df.to_python(str_in)
-        self.assertEqual(td_out, td_expected)
-
-    def test_bad_string(self):
-        """Malformed strings should raise an error.
-        """
-        str_in = "3:5"
-        with self.assertRaises(ValueError):
-            self.df.to_python(str_in)
-
-    def test_int(self):
-        """Int inputs should give timedelta outputs
-        """
-        int_in = 176400
-        td_expected = timedelta(days=2, hours=1)
-        td_out = self.df.to_python(int_in)
-        self.assertEqual(td_out, td_expected)
-
-    def test_none(self):
-        """Null input -> None output
-        """
-        td_in = None
-        td_out = self.df.to_python(td_in)
-        self.assertEqual(td_in, td_out)
-
-    def test_invalid(self):
-        """Unsupported objects raise ValueError
-        """
-        td_in = self
-        with self.assertRaises(ValueError):
-            self.df.to_python(td_in)
-
-
-class DurationFieldGetPrepValueTest(unittest.TestCase):
-    def setUp(self):
-        """Create a mock of the DurationField class and pin get_prep_value.
-        """
-        self.df = fields.DurationField()
-
-    def test_returns_int(self):
-        """Type should be `int`.
-        """
-        td_in = timedelta(hours=14)
-        int_out = self.df.get_prep_value(td_in)
-        self.assertTrue(isinstance(int_out, int))
-
-    def test_returns_int2(self):
-        """Type should be `int`.
-        """
-        td_in = timedelta(hours=14, seconds=3.5)
-        int_out = self.df.get_prep_value(td_in)
-        self.assertTrue(isinstance(int_out, int))
-
-    def test_round_trip(self):
-        """A trip through get_prep_value and to_python.
-        """
-        td_in = timedelta(hours=14)
-        int_out = self.df.get_prep_value(td_in)
-        td_out = self.df.to_python(int_out)
-        self.assertEqual(td_out, td_in)
-
-
-class DurationFieldValueToStringTest(unittest.TestCase):
-    def setUp(self):
-        """Create a mock of the DurationField class and pin value_to_string to it.
-
-        We also mock out the _get_val_from_obj, to just return what is
-        passed in. Allows us to pass in a timedelta for testing intead
-        of the expected object.
-        """
-        self.mock_DurationField = MagicMock()
-        self.mock_DurationField.value_to_string = fields.DurationField.__dict__['value_to_string']
-        self.mock_DurationField.to_python = fields.DurationField.__dict__['to_python']
-        self.mock_DurationField._get_val_from_obj.side_effect = lambda x: x
-
-    def test_simple_string(self):
-        """
-        """
-        in_td = timedelta(days=1, hours=1, minutes=1, seconds=1)
-        expected_str = "1 day, 1:01:01"
-        out_str = self.mock_DurationField.value_to_string(self.mock_DurationField, in_td)
-        self.assertEqual(out_str, expected_str)
-
-    def test_loop_to_python(self):
-        """A roundtrip through value_to_string and to_python.
-
-        We expect the value to be unchanged after the trip.
-        """
-        in_td = timedelta(days=1, hours=1, minutes=1, seconds=1)
-        out_str = self.mock_DurationField.value_to_string(self.mock_DurationField, in_td)
-        out_td = self.mock_DurationField.to_python(self.mock_DurationField, out_str)
-        self.assertEqual(out_td, in_td)
-
-
-class ParseTimedeltaStringTest(unittest.TestCase):
-    """Test some round trips between timedelta, string, timedelta.
-    """
-    def test_works(self):
-        """Test a bunch of cases for the regular expressions.
-
-        We test so many things in this test because regular
-        expressions represent a lot of effective branching.
-        """
-        td1_in = timedelta(days=1)
-        td2_in = timedelta(seconds=1)
-        td3_in = timedelta(hours=1, minutes=1, seconds=1)
-        td4_in = timedelta(days=1, seconds=10000.001)
-        td5_in = timedelta(hours=12)
-        td6_in = timedelta(hours=-12)
-        str1_out = str(td1_in)
-        str2_out = str(td2_in)
-        str3_out = str(td3_in)
-        str4_out = str(td4_in)
-        str5_out = str(td5_in)
-        str6_out = str(td6_in)
-        td1_out = fields.parse_timedelta_string(str1_out)
-        td2_out = fields.parse_timedelta_string(str2_out)
-        td3_out = fields.parse_timedelta_string(str3_out)
-        td4_out = fields.parse_timedelta_string(str4_out)
-        td5_out = fields.parse_timedelta_string(str5_out)
-        td6_out = fields.parse_timedelta_string(str6_out)
-        self.assertEqual(td1_in, td1_out)
-        self.assertEqual(td2_in, td2_out)
-        self.assertEqual(td3_in, td3_out)
-        self.assertEqual(td4_in, td4_out)
-        self.assertEqual(td5_in, td5_out)
-        self.assertEqual(td6_in, td6_out)
-
-
-class SetupSouthTest(unittest.TestCase):
-    def test_no_south(self):
-        """This test is meant to hit the branch handleing the ImportError for
-        south.
-
-        Some users may not have south, so if it is not available, we
-        just pass.
-        """
-        with patch.dict('sys.modules', {'south.modelsinspector': {}}):
-            reload(fields)
+import unittest
+from datetime import timedelta
+
+import django
+from importlib import reload
+from unittest.mock import MagicMock, patch
+
+from localized_recurrence import fields
+
+
+class DurationFieldToPythonTest(unittest.TestCase):
+    def setUp(self):
+        """Create a mock of the DurationField class and pin to_python to it.
+        """
+        self.df = fields.DurationField()
+        self.df_with_default = fields.DurationField(default=60)
+
+    def test_deconstruct_with_default(self):
+        """
+        Test .deconstruct() with a default
+        """
+        if django.VERSION[1] >= 7:  # pragma: no cover
+            name, path, args, kwargs = self.df_with_default.deconstruct()
+
+            self.assertEqual(kwargs['default'], 60)
+        else:  # pragma: no cover
+            with patch('localized_recurrence.fields.IntegerField.deconstruct', create=True) as mock_deconstruct:
+                mock_deconstruct.return_value = (
+                    'duration', 'django.db.models.IntegerField', [], {'default': timedelta(seconds=60)}
+                )
+                name, path, args, kwargs = self.df_with_default.deconstruct()
+                self.assertEqual(kwargs['default'], 60)
+
+    def test_deconstruct_without_default(self):
+        """
+        Test .deconstruct() without a default
+        """
+        if django.VERSION[1] >= 7:  # pragma: no cover
+            name, path, args, kwargs = self.df.deconstruct()
+            self.assertFalse('default' in kwargs.keys())
+        else:  # pragma: no cover
+            with patch('localized_recurrence.fields.IntegerField.deconstruct', create=True) as mock_deconstruct:
+                mock_deconstruct.return_value = (
+                    'duration', 'django.db.models.IntegerField', [], {}
+                )
+                name, path, args, kwargs = self.df_with_default.deconstruct()
+                self.assertNotIn('default', kwargs.keys())
+
+    def test_timedelta(self):
+        """A timedelta should just get returned.
+        """
+        td_in = timedelta(days=1, hours=3)
+        td_out = self.df.to_python(td_in)
+        self.assertEqual(td_out, td_in)
+
+    def test_string(self):
+        """A string should be properly converted.
+        """
+        td_expected = timedelta(days=3, hours=5, minutes=10)
+        str_in = str(td_expected)
+        td_out = self.df.to_python(str_in)
+        self.assertEqual(td_out, td_expected)
+
+    def test_bad_string(self):
+        """Malformed strings should raise an error.
+        """
+        str_in = "3:5"
+        with self.assertRaises(ValueError):
+            self.df.to_python(str_in)
+
+    def test_int(self):
+        """Int inputs should give timedelta outputs
+        """
+        int_in = 176400
+        td_expected = timedelta(days=2, hours=1)
+        td_out = self.df.to_python(int_in)
+        self.assertEqual(td_out, td_expected)
+
+    def test_none(self):
+        """Null input -> None output
+        """
+        td_in = None
+        td_out = self.df.to_python(td_in)
+        self.assertEqual(td_in, td_out)
+
+    def test_invalid(self):
+        """Unsupported objects raise ValueError
+        """
+        td_in = self
+        with self.assertRaises(ValueError):
+            self.df.to_python(td_in)
+
+
+class DurationFieldGetPrepValueTest(unittest.TestCase):
+    def setUp(self):
+        """Create a mock of the DurationField class and pin get_prep_value.
+        """
+        self.df = fields.DurationField()
+
+    def test_returns_int(self):
+        """Type should be `int`.
+        """
+        td_in = timedelta(hours=14)
+        int_out = self.df.get_prep_value(td_in)
+        self.assertTrue(isinstance(int_out, int))
+
+    def test_returns_int2(self):
+        """Type should be `int`.
+        """
+        td_in = timedelta(hours=14, seconds=3.5)
+        int_out = self.df.get_prep_value(td_in)
+        self.assertTrue(isinstance(int_out, int))
+
+    def test_round_trip(self):
+        """A trip through get_prep_value and to_python.
+        """
+        td_in = timedelta(hours=14)
+        int_out = self.df.get_prep_value(td_in)
+        td_out = self.df.to_python(int_out)
+        self.assertEqual(td_out, td_in)
+
+
+class DurationFieldValueToStringTest(unittest.TestCase):
+    def setUp(self):
+        """Create a mock of the DurationField class and pin value_to_string to it.
+
+        We also mock out the _get_val_from_obj, to just return what is
+        passed in. Allows us to pass in a timedelta for testing intead
+        of the expected object.
+        """
+        self.mock_DurationField = MagicMock()
+        self.mock_DurationField.value_to_string = fields.DurationField.__dict__['value_to_string']
+        self.mock_DurationField.to_python = fields.DurationField.__dict__['to_python']
+        self.mock_DurationField._get_val_from_obj.side_effect = lambda x: x
+
+    def test_simple_string(self):
+        """
+        """
+        in_td = timedelta(days=1, hours=1, minutes=1, seconds=1)
+        expected_str = "1 day, 1:01:01"
+        out_str = self.mock_DurationField.value_to_string(self.mock_DurationField, in_td)
+        self.assertEqual(out_str, expected_str)
+
+    def test_loop_to_python(self):
+        """A roundtrip through value_to_string and to_python.
+
+        We expect the value to be unchanged after the trip.
+        """
+        in_td = timedelta(days=1, hours=1, minutes=1, seconds=1)
+        out_str = self.mock_DurationField.value_to_string(self.mock_DurationField, in_td)
+        out_td = self.mock_DurationField.to_python(self.mock_DurationField, out_str)
+        self.assertEqual(out_td, in_td)
+
+
+class ParseTimedeltaStringTest(unittest.TestCase):
+    """Test some round trips between timedelta, string, timedelta.
+    """
+    def test_works(self):
+        """Test a bunch of cases for the regular expressions.
+
+        We test so many things in this test because regular
+        expressions represent a lot of effective branching.
+        """
+        td1_in = timedelta(days=1)
+        td2_in = timedelta(seconds=1)
+        td3_in = timedelta(hours=1, minutes=1, seconds=1)
+        td4_in = timedelta(days=1, seconds=10000.001)
+        td5_in = timedelta(hours=12)
+        td6_in = timedelta(hours=-12)
+        str1_out = str(td1_in)
+        str2_out = str(td2_in)
+        str3_out = str(td3_in)
+        str4_out = str(td4_in)
+        str5_out = str(td5_in)
+        str6_out = str(td6_in)
+        td1_out = fields.parse_timedelta_string(str1_out)
+        td2_out = fields.parse_timedelta_string(str2_out)
+        td3_out = fields.parse_timedelta_string(str3_out)
+        td4_out = fields.parse_timedelta_string(str4_out)
+        td5_out = fields.parse_timedelta_string(str5_out)
+        td6_out = fields.parse_timedelta_string(str6_out)
+        self.assertEqual(td1_in, td1_out)
+        self.assertEqual(td2_in, td2_out)
+        self.assertEqual(td3_in, td3_out)
+        self.assertEqual(td4_in, td4_out)
+        self.assertEqual(td5_in, td5_out)
+        self.assertEqual(td6_in, td6_out)
+
+
+class SetupSouthTest(unittest.TestCase):
+    def test_no_south(self):
+        """This test is meant to hit the branch handleing the ImportError for
+        south.
+
+        Some users may not have south, so if it is not available, we
+        just pass.
+        """
+        with patch.dict('sys.modules', {'south.modelsinspector': {}}):
+            reload(fields)
```

### Comparing `django-localized-recurrence-4.0.0/localized_recurrence/tests/models_tests.py` & `django-localized-recurrence-4.1.0/localized_recurrence/tests/models_tests.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,550 +1,550 @@
-from datetime import datetime, timedelta
-
-from django.test import TestCase
-from django_dynamic_fixture import G
-import pytz
-
-from ..models import LocalizedRecurrence, LocalizedRecurrenceQuerySet
-from ..models import _replace_with_offset, _update_schedule
-
-
-class LocalizedRecurrenceUpdateTest(TestCase):
-    """
-    Tests calling 'update' on a localized recurrence.
-    """
-    def test_update_creation(self):
-        lr = LocalizedRecurrence()
-        lr.update()
-        self.assertIsNotNone(lr.id)
-
-    def test_update_timezone(self):
-        lr = G(LocalizedRecurrence)
-        lr.update(timezone='US/Eastern')
-        lr = LocalizedRecurrence.objects.get(id=lr.id)
-        self.assertEqual(lr.timezone, pytz.timezone('US/Eastern'))
-
-    def test_update_offset(self):
-        lr = G(LocalizedRecurrence)
-        lr.update(offset=timedelta(seconds=1))
-        lr = LocalizedRecurrence.objects.get(id=lr.id)
-        self.assertEqual(lr.offset, timedelta(seconds=1))
-
-
-class LocalizedRecurrenceQuerySetTest(TestCase):
-    """Simple test to ensure the custom query set is being used.
-    """
-    def test_isinstance(self):
-        G(LocalizedRecurrence)
-        recurrences = LocalizedRecurrence.objects.all()
-        self.assertIsInstance(recurrences, LocalizedRecurrenceQuerySet)
-
-
-class LocalizedRecurrenceQuerySetUpdateScheduleTest(TestCase):
-    """Test that updates to recurrences are reflected in the DB.
-    """
-    def setUp(self):
-        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
-        G(LocalizedRecurrence, interval='MONTH', offset=timedelta(hours=15), timezone=pytz.timezone('US/Eastern'))
-
-    def test_update_from_1970(self):
-        """Start with next_scheduled of 1970, after update should be new.
-        """
-        time = datetime(year=2013, month=5, day=20, hour=12, minute=3)
-        LocalizedRecurrence.objects.filter(interval='DAY').update_schedule(time=time)
-        lr_day = LocalizedRecurrence.objects.filter(interval='DAY').first()
-        self.assertGreater(lr_day.next_scheduled, time)
-
-
-class LocalizedRecurrenceManagerUpdateScheduleTest(TestCase):
-    def setUp(self):
-        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
-        G(LocalizedRecurrence, interval='MONTH', offset=timedelta(hours=15), timezone=pytz.timezone('US/Eastern'))
-
-    def test_update_all(self):
-        """Calls to the model manager to update should be passed through.
-        """
-        time = datetime(year=2013, month=5, day=20, hour=15, minute=3)
-        LocalizedRecurrence.objects.update_schedule(time=time)
-        self.assertTrue(all(r.next_scheduled > time for r in LocalizedRecurrence.objects.all()))
-
-
-class LocalizedRecurrenceTest(TestCase):
-    """Test the creation and querying of LocalizedRecurrence records.
-    """
-    def setUp(self):
-        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
-
-    def test_timedelta_returned(self):
-        """Test that the Duration field is correctly returning timedeltas.
-        """
-        lr = LocalizedRecurrence.objects.first()
-        self.assertTrue(isinstance(lr.offset, timedelta))
-
-    def test_string_representation(self):
-        lr = LocalizedRecurrence.objects.first()
-        self.assertEqual(
-            str(lr),
-            'ID: {0}, Interval: {1}, Next Scheduled: {2}'.format(lr.id, lr.interval, lr.next_scheduled),
-        )
-
-
-class LocalizedRecurrenceUpdateScheduleTest(TestCase):
-    def setUp(self):
-        self.lr_day = G(LocalizedRecurrence,
-                        interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
-
-    def test_update_passes_through(self):
-        time = datetime(year=2013, month=5, day=20, hour=15, minute=3)
-        self.lr_day.update_schedule(time)
-        self.assertGreater(self.lr_day.next_scheduled, time)
-
-
-class LocalizedRecurrenceUtcOfNextScheduleTest(TestCase):
-    def setUp(self):
-        self.lr_day = G(
-            LocalizedRecurrence,
-            interval='DAY', offset=timedelta(hours=12),
-            timezone=pytz.timezone('US/Eastern'))
-        self.lr_week = G(
-            LocalizedRecurrence,
-            interval='WEEK', offset=timedelta(days=3, hours=17, minutes=30),
-            timezone=pytz.timezone('US/Central'))
-        self.lr_month = G(
-            LocalizedRecurrence,
-            interval='MONTH', offset=timedelta(days=21, hours=19, minutes=15, seconds=10),
-            timezone=pytz.timezone('US/Central'))
-        self.lr_quarter = G(
-            LocalizedRecurrence,
-            interval='QUARTER', offset=timedelta(days=68, hours=16, minutes=30),
-            timezone=pytz.timezone('Asia/Hong_Kong'))
-        self.lr_year = G(
-            LocalizedRecurrence,
-            interval='YEAR', offset=timedelta(days=31, hours=16, minutes=30),
-            timezone=pytz.timezone('Asia/Hong_Kong'))
-
-    def test_basic_works(self):
-        """
-        Test a simple case of utc_of_next_schedule.
-
-        - The given recurrence is scheduled daily for Eastern Time at noon.
-        - The given current date in UTC is 2013/1/15::17:05:22
-        - We then expect the next schedule in UTC to be 2013/1/16::17:0:0
-        """
-        current_time = datetime(2013, 1, 15, 17, 5, 22)
-        expected_next_schedule = datetime(2013, 1, 16, 17)
-        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_dst_cross_monthly(self):
-        """The case when a monthly recurrence goes past daylight savings time"""
-        self.lr_month.offset = timedelta(hours=0)
-        self.lr_month.previous_scheduled = datetime(2015, 2, 1, 6)
-        scheduled_out = self.lr_month.utc_of_next_schedule(datetime(2015, 3, 31))
-        self.assertEqual(scheduled_out, datetime(2015, 4, 1, 5))
-
-    def test_before_midnight(self):
-        """The case when the scheduled and current time cross midnight.
-
-        - The given recurrence is scheduled daily for Eastern Time at 11:59PM.
-        - The given current date in UTC is 2013/1/15::05:05:22 -> 12:05AM EST
-        - We then expect the next schedule in UTC to be 2013/1/16::05:0:0
-        """
-        self.lr_day.offset = timedelta(hours=23, minutes=59)
-        self.lr_day.save()
-        current_time = datetime(2013, 1, 15, 5, 5, 22)
-        expected_next_schedule = datetime(2013, 1, 16, 4, 59)
-        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_after_midnight(self):
-        """
-        The case when the scheduled and current time are after midnight.
-
-        - The given recurrence is scheduled daily for Eastern Time at 12:01 AM.
-        - The given current date in UTC is 2013/1/15::05:05:22 -> 12:05AM EST
-        - We then expect the next schedule in UTC to be 2013/1/16::05:01:0
-        """
-        self.lr_day.offset = timedelta(minutes=1)
-        self.lr_day.save()
-        current_time = datetime(2013, 1, 15, 5, 5, 22)
-        expected_next_schedule = datetime(2013, 1, 16, 5, 1)
-        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_week_update_full_week(self):
-        """
-        Weekly Recurrences should be able to add a full week.
-
-        - Thursday August 8th at 10:34 PM UTC is 5:34 PM CDT.
-        - Scheduled for weekly, Thursday at 5:30
-        - Expect next schedule to be Thursday August 15th at 10:30 PM UTC
-        """
-        current_time = datetime(2013, 8, 8, 22, 34)
-        expected_next_schedule = datetime(2013, 8, 15, 22, 30)
-        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_weekly_update_current_week(self):
-        """
-        Weekly Recurrences should be able to work in the current week.
-
-        - Tuesday August 6th at 10:34 PM UTC is 5:34 PM CDT.
-        - Scheduled for weekly, Thursday at 5:30
-        - Expect next schedule to be Thursday August 8th at 10:30 PM UTC
-        """
-        current_time = datetime(2013, 8, 6, 22, 34)
-        expected_next_schedule = datetime(2013, 8, 8, 22, 30)
-        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_month_update_full_month(self):
-        """
-        Monthly Recurrences should work as expected moving forward a full month.
-
-        - Friday August 23rd at 12:34 AM UTC is Thursday August 22nd at 7:34 PM CDT.
-        - Scheduled for Monthly, on the 21st day at 7:15.10 PM
-        - Expect next schedule to be September 23 at 12:15.10 AM UTC
-        """
-        current_time = datetime(2013, 8, 23, 0, 34, 55)
-        expected_next_schedule = datetime(2013, 9, 23, 0, 15, 10)
-        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_month_update_current_month(self):
-        """
-        Monthly Recurrences should work as expected moving forward in the
-        current month.
-
-        - Friday August 16th at 12:34 AM UTC is Thursday August 15th at 7:34 PM CDT.
-        - Scheduled for Monthly, on the 21st day at 7:15.10 PM
-        - Expect next schedule to be August 23 at 12:15.10 AM UTC
-
-        """
-        current_time = datetime(2013, 8, 16, 0, 34, 55)
-        expected_next_schedule = datetime(2013, 8, 23, 0, 15, 10)
-        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_month_year_end_update(self):
-        """
-        Monthly Recurrences should transition over years correctly
-
-        - Monday December 23 at 2:34 AM UTC is Sunday August 22nd at 9:34 PM CDT.
-        - Scheduled for Monthly, on the 21st day at 7:15.10 PM CDT
-        - Expect next schedule to be January 23 at 1:15.10 AM UCT
-        """
-        current_time = datetime(2013, 12, 23, 2, 34, 55)
-        expected_next_schedule = datetime(2014, 1, 23, 1, 15, 10)
-        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_quarterly_full_quarter(self):
-        """
-        Quarterly Recurrences should be able to update a full quarter.
-
-        - June 23rd at 12:34 AM UTC is June 22nd at 10:34 PM HKT.
-        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
-        - Expect next schedule to be September 7th at 8:30 AM UTC
-        """
-        current_time = datetime(2013, 6, 23, 0, 34, 55)
-        expected_next_schedule = datetime(2013, 9, 7, 8, 30)
-        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
-        self.lr_quarter = G(
-            LocalizedRecurrence,
-            interval='QUARTER',
-            offset=timedelta(days=68, hours=16, minutes=30),
-            timezone=pytz.timezone('Asia/Hong_Kong')
-        )
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_quarterly_current_quarter(self):
-        """
-        Quarterly Recurrences should be able to update in the current quarter.
-
-        - April 23rd at 12:34 AM UTC is April 22nd at 10:34 PM HKT.
-        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
-        - Expect next schedule to be June 8th at 8:30 AM UTC
-        """
-        current_time = datetime(2013, 4, 23, 0, 34, 55)
-        expected_next_schedule = datetime(2013, 6, 8, 8, 30)
-        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
-
-        self.lr_quarter = G(
-            LocalizedRecurrence,
-            interval='QUARTER',
-            offset=timedelta(days=68, hours=16, minutes=30),
-            timezone=pytz.timezone('Asia/Hong_Kong')
-        )
-
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_quarterly_end_year(self):
-        """
-        Quarterly Recurrences should be able to update through year end.
-
-        - December 23rd at 12:34 AM UTC is April 22nd at 10:34 PM HKT.
-        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
-        - Expect next schedule to be March 10th at 8:30 AM UTC
-        """
-        current_time = datetime(2013, 12, 23, 0, 34, 55)
-        expected_next_schedule = datetime(2014, 3, 10, 8, 30)
-        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
-        self.lr_quarter = G(
-            LocalizedRecurrence,
-            interval='QUARTER',
-            offset=timedelta(days=68, hours=16, minutes=30),
-            timezone=pytz.timezone('Asia/Hong_Kong')
-        )
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_yearly(self):
-        """
-        Yearly Recurrences should work as expected.
-
-        - June 23rd at 12:34 AM UTC is June 22nd at 10:34 PM HKT.
-        - Scheduled for Yearly, on the 31st day at 4:30 PM HKT
-        - Expect next schedule to be February 1st at 8:30 AM UTC
-        """
-        current_time = datetime(2013, 6, 23, 0, 34, 55)
-        expected_next_schedule = datetime(2014, 2, 1, 8, 30)
-        schedule_out = self.lr_year.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_into_dst_boundary(self):
-        """
-        Recurrences happen at the correct local time after going into DST.
-
-        Going into daylight savings time should mean the UTC time is
-        an hour less on the next recurrence.
-
-        - 2013 US DST began: Sunday March 10th.
-        - Weekly recurence, every Thursday at Noon EST.
-        """
-        self.lr_week.offset = timedelta(days=3, hours=12)
-        self.lr_week.save()
-        current_time = datetime(2013, 3, 7, 18)
-        expected_next_schedule = datetime(2013, 3, 14, 17)
-        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_out_of_dst_boundary(self):
-        """
-        Recurrences at the correct local time after going out of UTC.
-
-        Going into daylight savings time should mean the UTC time is
-        an hour greater on the next recurrence.
-
-        - 2013 US DST ended: Sunday November 3rd.
-        - Weekly recurence, every Thursday at Noon EST.
-        """
-        self.lr_week.offset = timedelta(days=3, hours=12)
-        self.lr_week.save()
-        current_time = datetime(2013, 10, 31, 17)
-        expected_next_schedule = datetime(2013, 11, 7, 18)
-        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-    def test_utc_plus(self):
-        """
-        Test a timezone that is UTC + 2.
-
-        - Europe/Berlin DST is UTC + 2
-        """
-        self.lr_day.timezone = pytz.timezone('Europe/Berlin')
-        self.lr_day.save()
-        current_time = datetime(2013, 5, 5, 10, 10)
-        expected_next_schedule = datetime(2013, 5, 6, 10)
-        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
-        self.assertEqual(schedule_out, expected_next_schedule)
-
-
-class UpdateScheduleTest(TestCase):
-    def setUp(self):
-        self.lr_week = G(
-            LocalizedRecurrence,
-            interval='WEEK', offset=timedelta(hours=12),
-            timezone=pytz.timezone('US/Eastern'))
-        self.lr_day = G(
-            LocalizedRecurrence,
-            interval='DAY',
-            offset=timedelta(hours=12),
-            timezone=pytz.timezone('US/Eastern'))
-
-    def test_updates_localized_recurrences(self):
-        time = datetime(year=2013, month=5, day=20, hour=12, minute=3)
-        _update_schedule([self.lr_week], time)
-        self.assertGreater(self.lr_week.next_scheduled, time)
-        self.assertEqual(self.lr_week.previous_scheduled, time)
-
-
-class ReplaceWithOffsetTest(TestCase):
-    def test_day(self):
-        """
-        _replace_with_offset works as expected with a 'DAY' interval.
-        """
-        dt_in = datetime(2013, 1, 20, 12, 45, 48)
-        td_in = timedelta(hours=3, minutes=3, seconds=3)
-        interval_in = 'DAY'
-        dt_expected = datetime(2013, 1, 20, 3, 3, 3)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_out, dt_expected)
-
-    def test_week(self):
-        """
-        _replace_with_offset works as expected with a 'WEEK' interval.
-        """
-        dt_in = datetime(2013, 1, 20, 12, 45, 48)
-        td_in = timedelta(days=4, hours=3, minutes=3, seconds=3)
-        interval_in = 'WEEK'
-        dt_expected = datetime(2013, 1, 18, 3, 3, 3)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_out, dt_expected)
-
-    def test_week_on_month_boundary(self):
-        """
-        _replace_with_offset using interval 'WEEK' should roll over months
-        correctly.
-        """
-        dt_in = datetime(2013, 7, 30, 12, 45, 48)
-        td_in = timedelta(days=4, hours=3, minutes=3, seconds=3)
-        interval_in = 'WEEK'
-        dt_expected = datetime(2013, 8, 2, 3, 3, 3)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_out, dt_expected)
-
-    def test_month(self):
-        """
-        _replace_with_offset works as expected with a 'MONTH' interval.
-        """
-        dt_in = datetime(2013, 1, 20, 12, 45, 48)
-        td_in = timedelta(days=15, hours=3, minutes=3, seconds=3)
-        interval_in = 'MONTH'
-        dt_expected = datetime(2013, 1, 16, 3, 3, 3)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_out, dt_expected)
-
-    def test_last_day_of_month(self):
-        """
-        Check dates for a full year where the utc time is the first and the time zone is the previous day
-        """
-        time_delta = timedelta(days=30, hours=23, minutes=3, seconds=3)
-        dt_start = datetime(2013, 2, 20, 23, 45, 48)
-        interval_name = 'MONTH'
-        timezone_name = 'US/Central'
-        recurrence = LocalizedRecurrence.objects.create(
-            interval=interval_name,
-            offset=time_delta,
-            timezone=timezone_name,
-            next_scheduled=dt_start,
-        )
-
-        # Check a full year of dates. The first next recurrence should be the month after it starts because
-        # The start time is weird because it should be set correctly to begin with. Setting it to 2-20 should not
-        # be happening. The app should initially set it to the correct first fire date
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 2, 20, 23, 45, 48))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 4, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 5, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 6, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 7, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 8, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 9, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 10, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 11, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2013, 12, 1, 5, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2014, 1, 1, 5, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2014, 2, 1, 5, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2014, 3, 1, 5, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-        self.assertEqual(recurrence.next_scheduled, datetime(2014, 4, 1, 4, 3, 3))
-        recurrence.update_schedule(recurrence.next_scheduled)
-
-    def test_quarter(self):
-        dt_in = datetime(2013, 4, 20, 12, 45, 48)
-        td_in = timedelta(days=65, hours=3, minutes=3, seconds=3)
-        interval_in = 'QUARTER'
-        dt_expected = datetime(2013, 6, 5, 3, 3, 3)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_out, dt_expected)
-
-    def test_quarterly_past(self):
-        dt_in = datetime(2013, 6, 23, 0, 34, 55)
-        td_in = timedelta(days=68, hours=16, minutes=30)
-        interval_in = 'QUARTER'
-        dt_expected = datetime(2013, 6, 8, 16, 30)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_quarterly_overshoot(self):
-        dt_in = datetime(2013, 1, 1, 0)
-        td_in = timedelta(days=90, hours=12)
-        interval_in = 'QUARTER'
-        dt_expected = datetime(2013, 3, 31, 12)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_quarterly_undershoot(self):
-        dt_in = datetime(2013, 7, 1, 0)
-        td_in = timedelta(days=90, hours=12)
-        interval_in = 'QUARTER'
-        dt_expected = datetime(2013, 9, 29, 12)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_year(self):
-        dt_in = datetime(2013, 6, 23, 0, 34, 55)
-        td_in = timedelta(days=5, hours=16, minutes=30)
-        interval_in = 'YEAR'
-        dt_expected = datetime(2013, 1, 6, 16, 30)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_year_end_leap_year(self):
-        dt_in = datetime(2016, 6, 23, 0, 34, 55)
-        td_in = timedelta(days=365, hours=16, minutes=30)
-        interval_in = 'YEAR'
-        dt_expected = datetime(2016, 12, 31, 16, 30)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_year_end_non_leap_year(self):
-        dt_in = datetime(2015, 6, 23, 0, 34, 55)
-        td_in = timedelta(days=365, hours=16, minutes=30)
-        interval_in = 'YEAR'
-        dt_expected = datetime(2015, 12, 31, 16, 30)
-        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
-        self.assertEqual(dt_expected, dt_out)
-
-    def test_bad_interval(self):
-        """
-        A missformed interval should raise a value error
-        """
-        dt_in = datetime(2013, 1, 20, 12, 45, 48)
-        td_in = timedelta(days=15, hours=3, minutes=3, seconds=3)
-        interval_in = 'blah'
-        with self.assertRaises(ValueError):
-            _replace_with_offset(dt_in, td_in, interval_in)
+from datetime import datetime, timedelta
+
+from django.test import TestCase
+from django_dynamic_fixture import G
+import pytz
+
+from ..models import LocalizedRecurrence, LocalizedRecurrenceQuerySet
+from ..models import _replace_with_offset, _update_schedule
+
+
+class LocalizedRecurrenceUpdateTest(TestCase):
+    """
+    Tests calling 'update' on a localized recurrence.
+    """
+    def test_update_creation(self):
+        lr = LocalizedRecurrence()
+        lr.update()
+        self.assertIsNotNone(lr.id)
+
+    def test_update_timezone(self):
+        lr = G(LocalizedRecurrence)
+        lr.update(timezone='US/Eastern')
+        lr = LocalizedRecurrence.objects.get(id=lr.id)
+        self.assertEqual(lr.timezone, pytz.timezone('US/Eastern'))
+
+    def test_update_offset(self):
+        lr = G(LocalizedRecurrence)
+        lr.update(offset=timedelta(seconds=1))
+        lr = LocalizedRecurrence.objects.get(id=lr.id)
+        self.assertEqual(lr.offset, timedelta(seconds=1))
+
+
+class LocalizedRecurrenceQuerySetTest(TestCase):
+    """Simple test to ensure the custom query set is being used.
+    """
+    def test_isinstance(self):
+        G(LocalizedRecurrence)
+        recurrences = LocalizedRecurrence.objects.all()
+        self.assertIsInstance(recurrences, LocalizedRecurrenceQuerySet)
+
+
+class LocalizedRecurrenceQuerySetUpdateScheduleTest(TestCase):
+    """Test that updates to recurrences are reflected in the DB.
+    """
+    def setUp(self):
+        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
+        G(LocalizedRecurrence, interval='MONTH', offset=timedelta(hours=15), timezone=pytz.timezone('US/Eastern'))
+
+    def test_update_from_1970(self):
+        """Start with next_scheduled of 1970, after update should be new.
+        """
+        time = datetime(year=2013, month=5, day=20, hour=12, minute=3)
+        LocalizedRecurrence.objects.filter(interval='DAY').update_schedule(time=time)
+        lr_day = LocalizedRecurrence.objects.filter(interval='DAY').first()
+        self.assertGreater(lr_day.next_scheduled, time)
+
+
+class LocalizedRecurrenceManagerUpdateScheduleTest(TestCase):
+    def setUp(self):
+        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
+        G(LocalizedRecurrence, interval='MONTH', offset=timedelta(hours=15), timezone=pytz.timezone('US/Eastern'))
+
+    def test_update_all(self):
+        """Calls to the model manager to update should be passed through.
+        """
+        time = datetime(year=2013, month=5, day=20, hour=15, minute=3)
+        LocalizedRecurrence.objects.update_schedule(time=time)
+        self.assertTrue(all(r.next_scheduled > time for r in LocalizedRecurrence.objects.all()))
+
+
+class LocalizedRecurrenceTest(TestCase):
+    """Test the creation and querying of LocalizedRecurrence records.
+    """
+    def setUp(self):
+        G(LocalizedRecurrence, interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
+
+    def test_timedelta_returned(self):
+        """Test that the Duration field is correctly returning timedeltas.
+        """
+        lr = LocalizedRecurrence.objects.first()
+        self.assertTrue(isinstance(lr.offset, timedelta))
+
+    def test_string_representation(self):
+        lr = LocalizedRecurrence.objects.first()
+        self.assertEqual(
+            str(lr),
+            'ID: {0}, Interval: {1}, Next Scheduled: {2}'.format(lr.id, lr.interval, lr.next_scheduled),
+        )
+
+
+class LocalizedRecurrenceUpdateScheduleTest(TestCase):
+    def setUp(self):
+        self.lr_day = G(LocalizedRecurrence,
+                        interval='DAY', offset=timedelta(hours=12), timezone=pytz.timezone('US/Eastern'))
+
+    def test_update_passes_through(self):
+        time = datetime(year=2013, month=5, day=20, hour=15, minute=3)
+        self.lr_day.update_schedule(time)
+        self.assertGreater(self.lr_day.next_scheduled, time)
+
+
+class LocalizedRecurrenceUtcOfNextScheduleTest(TestCase):
+    def setUp(self):
+        self.lr_day = G(
+            LocalizedRecurrence,
+            interval='DAY', offset=timedelta(hours=12),
+            timezone=pytz.timezone('US/Eastern'))
+        self.lr_week = G(
+            LocalizedRecurrence,
+            interval='WEEK', offset=timedelta(days=3, hours=17, minutes=30),
+            timezone=pytz.timezone('US/Central'))
+        self.lr_month = G(
+            LocalizedRecurrence,
+            interval='MONTH', offset=timedelta(days=21, hours=19, minutes=15, seconds=10),
+            timezone=pytz.timezone('US/Central'))
+        self.lr_quarter = G(
+            LocalizedRecurrence,
+            interval='QUARTER', offset=timedelta(days=68, hours=16, minutes=30),
+            timezone=pytz.timezone('Asia/Hong_Kong'))
+        self.lr_year = G(
+            LocalizedRecurrence,
+            interval='YEAR', offset=timedelta(days=31, hours=16, minutes=30),
+            timezone=pytz.timezone('Asia/Hong_Kong'))
+
+    def test_basic_works(self):
+        """
+        Test a simple case of utc_of_next_schedule.
+
+        - The given recurrence is scheduled daily for Eastern Time at noon.
+        - The given current date in UTC is 2013/1/15::17:05:22
+        - We then expect the next schedule in UTC to be 2013/1/16::17:0:0
+        """
+        current_time = datetime(2013, 1, 15, 17, 5, 22)
+        expected_next_schedule = datetime(2013, 1, 16, 17)
+        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_dst_cross_monthly(self):
+        """The case when a monthly recurrence goes past daylight savings time"""
+        self.lr_month.offset = timedelta(hours=0)
+        self.lr_month.previous_scheduled = datetime(2015, 2, 1, 6)
+        scheduled_out = self.lr_month.utc_of_next_schedule(datetime(2015, 3, 31))
+        self.assertEqual(scheduled_out, datetime(2015, 4, 1, 5))
+
+    def test_before_midnight(self):
+        """The case when the scheduled and current time cross midnight.
+
+        - The given recurrence is scheduled daily for Eastern Time at 11:59PM.
+        - The given current date in UTC is 2013/1/15::05:05:22 -> 12:05AM EST
+        - We then expect the next schedule in UTC to be 2013/1/16::05:0:0
+        """
+        self.lr_day.offset = timedelta(hours=23, minutes=59)
+        self.lr_day.save()
+        current_time = datetime(2013, 1, 15, 5, 5, 22)
+        expected_next_schedule = datetime(2013, 1, 16, 4, 59)
+        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_after_midnight(self):
+        """
+        The case when the scheduled and current time are after midnight.
+
+        - The given recurrence is scheduled daily for Eastern Time at 12:01 AM.
+        - The given current date in UTC is 2013/1/15::05:05:22 -> 12:05AM EST
+        - We then expect the next schedule in UTC to be 2013/1/16::05:01:0
+        """
+        self.lr_day.offset = timedelta(minutes=1)
+        self.lr_day.save()
+        current_time = datetime(2013, 1, 15, 5, 5, 22)
+        expected_next_schedule = datetime(2013, 1, 16, 5, 1)
+        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_week_update_full_week(self):
+        """
+        Weekly Recurrences should be able to add a full week.
+
+        - Thursday August 8th at 10:34 PM UTC is 5:34 PM CDT.
+        - Scheduled for weekly, Thursday at 5:30
+        - Expect next schedule to be Thursday August 15th at 10:30 PM UTC
+        """
+        current_time = datetime(2013, 8, 8, 22, 34)
+        expected_next_schedule = datetime(2013, 8, 15, 22, 30)
+        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_weekly_update_current_week(self):
+        """
+        Weekly Recurrences should be able to work in the current week.
+
+        - Tuesday August 6th at 10:34 PM UTC is 5:34 PM CDT.
+        - Scheduled for weekly, Thursday at 5:30
+        - Expect next schedule to be Thursday August 8th at 10:30 PM UTC
+        """
+        current_time = datetime(2013, 8, 6, 22, 34)
+        expected_next_schedule = datetime(2013, 8, 8, 22, 30)
+        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_month_update_full_month(self):
+        """
+        Monthly Recurrences should work as expected moving forward a full month.
+
+        - Friday August 23rd at 12:34 AM UTC is Thursday August 22nd at 7:34 PM CDT.
+        - Scheduled for Monthly, on the 21st day at 7:15.10 PM
+        - Expect next schedule to be September 23 at 12:15.10 AM UTC
+        """
+        current_time = datetime(2013, 8, 23, 0, 34, 55)
+        expected_next_schedule = datetime(2013, 9, 23, 0, 15, 10)
+        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_month_update_current_month(self):
+        """
+        Monthly Recurrences should work as expected moving forward in the
+        current month.
+
+        - Friday August 16th at 12:34 AM UTC is Thursday August 15th at 7:34 PM CDT.
+        - Scheduled for Monthly, on the 21st day at 7:15.10 PM
+        - Expect next schedule to be August 23 at 12:15.10 AM UTC
+
+        """
+        current_time = datetime(2013, 8, 16, 0, 34, 55)
+        expected_next_schedule = datetime(2013, 8, 23, 0, 15, 10)
+        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_month_year_end_update(self):
+        """
+        Monthly Recurrences should transition over years correctly
+
+        - Monday December 23 at 2:34 AM UTC is Sunday August 22nd at 9:34 PM CDT.
+        - Scheduled for Monthly, on the 21st day at 7:15.10 PM CDT
+        - Expect next schedule to be January 23 at 1:15.10 AM UCT
+        """
+        current_time = datetime(2013, 12, 23, 2, 34, 55)
+        expected_next_schedule = datetime(2014, 1, 23, 1, 15, 10)
+        schedule_out = self.lr_month.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_quarterly_full_quarter(self):
+        """
+        Quarterly Recurrences should be able to update a full quarter.
+
+        - June 23rd at 12:34 AM UTC is June 22nd at 10:34 PM HKT.
+        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
+        - Expect next schedule to be September 7th at 8:30 AM UTC
+        """
+        current_time = datetime(2013, 6, 23, 0, 34, 55)
+        expected_next_schedule = datetime(2013, 9, 7, 8, 30)
+        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
+        self.lr_quarter = G(
+            LocalizedRecurrence,
+            interval='QUARTER',
+            offset=timedelta(days=68, hours=16, minutes=30),
+            timezone=pytz.timezone('Asia/Hong_Kong')
+        )
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_quarterly_current_quarter(self):
+        """
+        Quarterly Recurrences should be able to update in the current quarter.
+
+        - April 23rd at 12:34 AM UTC is April 22nd at 10:34 PM HKT.
+        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
+        - Expect next schedule to be June 8th at 8:30 AM UTC
+        """
+        current_time = datetime(2013, 4, 23, 0, 34, 55)
+        expected_next_schedule = datetime(2013, 6, 8, 8, 30)
+        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
+
+        self.lr_quarter = G(
+            LocalizedRecurrence,
+            interval='QUARTER',
+            offset=timedelta(days=68, hours=16, minutes=30),
+            timezone=pytz.timezone('Asia/Hong_Kong')
+        )
+
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_quarterly_end_year(self):
+        """
+        Quarterly Recurrences should be able to update through year end.
+
+        - December 23rd at 12:34 AM UTC is April 22nd at 10:34 PM HKT.
+        - Scheduled for Quarterly, on the 68th day at 4:30 PM HKT
+        - Expect next schedule to be March 10th at 8:30 AM UTC
+        """
+        current_time = datetime(2013, 12, 23, 0, 34, 55)
+        expected_next_schedule = datetime(2014, 3, 10, 8, 30)
+        schedule_out = self.lr_quarter.utc_of_next_schedule(current_time)
+        self.lr_quarter = G(
+            LocalizedRecurrence,
+            interval='QUARTER',
+            offset=timedelta(days=68, hours=16, minutes=30),
+            timezone=pytz.timezone('Asia/Hong_Kong')
+        )
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_yearly(self):
+        """
+        Yearly Recurrences should work as expected.
+
+        - June 23rd at 12:34 AM UTC is June 22nd at 10:34 PM HKT.
+        - Scheduled for Yearly, on the 31st day at 4:30 PM HKT
+        - Expect next schedule to be February 1st at 8:30 AM UTC
+        """
+        current_time = datetime(2013, 6, 23, 0, 34, 55)
+        expected_next_schedule = datetime(2014, 2, 1, 8, 30)
+        schedule_out = self.lr_year.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_into_dst_boundary(self):
+        """
+        Recurrences happen at the correct local time after going into DST.
+
+        Going into daylight savings time should mean the UTC time is
+        an hour less on the next recurrence.
+
+        - 2013 US DST began: Sunday March 10th.
+        - Weekly recurence, every Thursday at Noon EST.
+        """
+        self.lr_week.offset = timedelta(days=3, hours=12)
+        self.lr_week.save()
+        current_time = datetime(2013, 3, 7, 18)
+        expected_next_schedule = datetime(2013, 3, 14, 17)
+        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_out_of_dst_boundary(self):
+        """
+        Recurrences at the correct local time after going out of UTC.
+
+        Going into daylight savings time should mean the UTC time is
+        an hour greater on the next recurrence.
+
+        - 2013 US DST ended: Sunday November 3rd.
+        - Weekly recurence, every Thursday at Noon EST.
+        """
+        self.lr_week.offset = timedelta(days=3, hours=12)
+        self.lr_week.save()
+        current_time = datetime(2013, 10, 31, 17)
+        expected_next_schedule = datetime(2013, 11, 7, 18)
+        schedule_out = self.lr_week.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+    def test_utc_plus(self):
+        """
+        Test a timezone that is UTC + 2.
+
+        - Europe/Berlin DST is UTC + 2
+        """
+        self.lr_day.timezone = pytz.timezone('Europe/Berlin')
+        self.lr_day.save()
+        current_time = datetime(2013, 5, 5, 10, 10)
+        expected_next_schedule = datetime(2013, 5, 6, 10)
+        schedule_out = self.lr_day.utc_of_next_schedule(current_time)
+        self.assertEqual(schedule_out, expected_next_schedule)
+
+
+class UpdateScheduleTest(TestCase):
+    def setUp(self):
+        self.lr_week = G(
+            LocalizedRecurrence,
+            interval='WEEK', offset=timedelta(hours=12),
+            timezone=pytz.timezone('US/Eastern'))
+        self.lr_day = G(
+            LocalizedRecurrence,
+            interval='DAY',
+            offset=timedelta(hours=12),
+            timezone=pytz.timezone('US/Eastern'))
+
+    def test_updates_localized_recurrences(self):
+        time = datetime(year=2013, month=5, day=20, hour=12, minute=3)
+        _update_schedule([self.lr_week], time)
+        self.assertGreater(self.lr_week.next_scheduled, time)
+        self.assertEqual(self.lr_week.previous_scheduled, time)
+
+
+class ReplaceWithOffsetTest(TestCase):
+    def test_day(self):
+        """
+        _replace_with_offset works as expected with a 'DAY' interval.
+        """
+        dt_in = datetime(2013, 1, 20, 12, 45, 48)
+        td_in = timedelta(hours=3, minutes=3, seconds=3)
+        interval_in = 'DAY'
+        dt_expected = datetime(2013, 1, 20, 3, 3, 3)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_out, dt_expected)
+
+    def test_week(self):
+        """
+        _replace_with_offset works as expected with a 'WEEK' interval.
+        """
+        dt_in = datetime(2013, 1, 20, 12, 45, 48)
+        td_in = timedelta(days=4, hours=3, minutes=3, seconds=3)
+        interval_in = 'WEEK'
+        dt_expected = datetime(2013, 1, 18, 3, 3, 3)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_out, dt_expected)
+
+    def test_week_on_month_boundary(self):
+        """
+        _replace_with_offset using interval 'WEEK' should roll over months
+        correctly.
+        """
+        dt_in = datetime(2013, 7, 30, 12, 45, 48)
+        td_in = timedelta(days=4, hours=3, minutes=3, seconds=3)
+        interval_in = 'WEEK'
+        dt_expected = datetime(2013, 8, 2, 3, 3, 3)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_out, dt_expected)
+
+    def test_month(self):
+        """
+        _replace_with_offset works as expected with a 'MONTH' interval.
+        """
+        dt_in = datetime(2013, 1, 20, 12, 45, 48)
+        td_in = timedelta(days=15, hours=3, minutes=3, seconds=3)
+        interval_in = 'MONTH'
+        dt_expected = datetime(2013, 1, 16, 3, 3, 3)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_out, dt_expected)
+
+    def test_last_day_of_month(self):
+        """
+        Check dates for a full year where the utc time is the first and the time zone is the previous day
+        """
+        time_delta = timedelta(days=30, hours=23, minutes=3, seconds=3)
+        dt_start = datetime(2013, 2, 20, 23, 45, 48)
+        interval_name = 'MONTH'
+        timezone_name = 'US/Central'
+        recurrence = LocalizedRecurrence.objects.create(
+            interval=interval_name,
+            offset=time_delta,
+            timezone=timezone_name,
+            next_scheduled=dt_start,
+        )
+
+        # Check a full year of dates. The first next recurrence should be the month after it starts because
+        # The start time is weird because it should be set correctly to begin with. Setting it to 2-20 should not
+        # be happening. The app should initially set it to the correct first fire date
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 2, 20, 23, 45, 48))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 4, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 5, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 6, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 7, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 8, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 9, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 10, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 11, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2013, 12, 1, 5, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2014, 1, 1, 5, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2014, 2, 1, 5, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2014, 3, 1, 5, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+        self.assertEqual(recurrence.next_scheduled, datetime(2014, 4, 1, 4, 3, 3))
+        recurrence.update_schedule(recurrence.next_scheduled)
+
+    def test_quarter(self):
+        dt_in = datetime(2013, 4, 20, 12, 45, 48)
+        td_in = timedelta(days=65, hours=3, minutes=3, seconds=3)
+        interval_in = 'QUARTER'
+        dt_expected = datetime(2013, 6, 5, 3, 3, 3)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_out, dt_expected)
+
+    def test_quarterly_past(self):
+        dt_in = datetime(2013, 6, 23, 0, 34, 55)
+        td_in = timedelta(days=68, hours=16, minutes=30)
+        interval_in = 'QUARTER'
+        dt_expected = datetime(2013, 6, 8, 16, 30)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_quarterly_overshoot(self):
+        dt_in = datetime(2013, 1, 1, 0)
+        td_in = timedelta(days=90, hours=12)
+        interval_in = 'QUARTER'
+        dt_expected = datetime(2013, 3, 31, 12)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_quarterly_undershoot(self):
+        dt_in = datetime(2013, 7, 1, 0)
+        td_in = timedelta(days=90, hours=12)
+        interval_in = 'QUARTER'
+        dt_expected = datetime(2013, 9, 29, 12)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_year(self):
+        dt_in = datetime(2013, 6, 23, 0, 34, 55)
+        td_in = timedelta(days=5, hours=16, minutes=30)
+        interval_in = 'YEAR'
+        dt_expected = datetime(2013, 1, 6, 16, 30)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_year_end_leap_year(self):
+        dt_in = datetime(2016, 6, 23, 0, 34, 55)
+        td_in = timedelta(days=365, hours=16, minutes=30)
+        interval_in = 'YEAR'
+        dt_expected = datetime(2016, 12, 31, 16, 30)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_year_end_non_leap_year(self):
+        dt_in = datetime(2015, 6, 23, 0, 34, 55)
+        td_in = timedelta(days=365, hours=16, minutes=30)
+        interval_in = 'YEAR'
+        dt_expected = datetime(2015, 12, 31, 16, 30)
+        dt_out = _replace_with_offset(dt_in, td_in, interval_in)
+        self.assertEqual(dt_expected, dt_out)
+
+    def test_bad_interval(self):
+        """
+        A missformed interval should raise a value error
+        """
+        dt_in = datetime(2013, 1, 20, 12, 45, 48)
+        td_in = timedelta(days=15, hours=3, minutes=3, seconds=3)
+        interval_in = 'blah'
+        with self.assertRaises(ValueError):
+            _replace_with_offset(dt_in, td_in, interval_in)
```

### Comparing `django-localized-recurrence-4.0.0/PKG-INFO` & `django-localized-recurrence-4.1.0/django_localized_recurrence.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-localized-recurrence
-Version: 4.0.0
+Version: 4.1.0
 Summary: Store events that recur in users' local times.
-Home-page: UNKNOWN
 Author: Erik Swanson
 Author-email: theerikswanson@gmail.com
 License: MIT License
-Description: .. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
-            :target: https://travis-ci.org/Wilduck/django-localized-recurrence
-        
-        Django Localized Recurrence
-        ===========================
-        Django Localized Recurrence allowes you to store events that recur in
-        users' local times, and not have to worry about things like
-        
-        This django app provides a model, ``LocalizedRecurrence``, with
-        methods to help store recurring events, check if the events are due,
-        and update their next scheduled time.
-        
-        Installation
-        ------------
-        This packages is currently available through Pypi and github. To
-        install from Pypi using ``pip`` (recommended)::
-        
-            pip install django-localized-recurrence
-        
-        
-        To install the development version from github::
-        
-            pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
-        
-        Documentation
-        -------------
-        Full documentation is available at http://django-localized-recurrence.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
+    :target: https://travis-ci.org/Wilduck/django-localized-recurrence
+
+Django Localized Recurrence
+===========================
+Django Localized Recurrence allowes you to store events that recur in
+users' local times, and not have to worry about things like
+
+This django app provides a model, ``LocalizedRecurrence``, with
+methods to help store recurring events, check if the events are due,
+and update their next scheduled time.
+
+Installation
+------------
+This packages is currently available through Pypi and github. To
+install from Pypi using ``pip`` (recommended)::
+
+    pip install django-localized-recurrence
+
+
+To install the development version from github::
+
+    pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
+
+Documentation
+-------------
+Full documentation is available at http://django-localized-recurrence.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-localized-recurrence-4.0.0/README.rst` & `django-localized-recurrence-4.1.0/README.rst`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-.. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
-    :target: https://travis-ci.org/Wilduck/django-localized-recurrence
-
-Django Localized Recurrence
-===========================
-Django Localized Recurrence allowes you to store events that recur in
-users' local times, and not have to worry about things like
-
-This django app provides a model, ``LocalizedRecurrence``, with
-methods to help store recurring events, check if the events are due,
-and update their next scheduled time.
-
-Installation
-------------
-This packages is currently available through Pypi and github. To
-install from Pypi using ``pip`` (recommended)::
-
-    pip install django-localized-recurrence
-
-
-To install the development version from github::
-
-    pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
-
-Documentation
--------------
-Full documentation is available at http://django-localized-recurrence.readthedocs.org
-
-License
--------
-MIT License (see LICENSE)
+.. image:: https://travis-ci.org/Wilduck/django-localized-recurrence.svg?branch=develop
+    :target: https://travis-ci.org/Wilduck/django-localized-recurrence
+
+Django Localized Recurrence
+===========================
+Django Localized Recurrence allowes you to store events that recur in
+users' local times, and not have to worry about things like
+
+This django app provides a model, ``LocalizedRecurrence``, with
+methods to help store recurring events, check if the events are due,
+and update their next scheduled time.
+
+Installation
+------------
+This packages is currently available through Pypi and github. To
+install from Pypi using ``pip`` (recommended)::
+
+    pip install django-localized-recurrence
+
+
+To install the development version from github::
+
+    pip install git+git://github.com/ambitioninc/django-localized-recurrence.git@develop
+
+Documentation
+-------------
+Full documentation is available at http://django-localized-recurrence.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-localized-recurrence-4.0.0/setup.py` & `django-localized-recurrence-4.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-import re
-from setuptools import setup, find_packages
-
-import multiprocessing
-assert multiprocessing
-
-
-def get_version():
-    """
-    Extracts the version number from the version.py file.
-    """
-    VERSION_FILE = 'localized_recurrence/version.py'
-    mo = re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', open(VERSION_FILE, 'rt').read(), re.M)
-    if mo:
-        return mo.group(1)
-    else:
-        raise RuntimeError('Unable to find version string in {0}.'.format(VERSION_FILE))
-
-
-setup(
-    name='django-localized-recurrence',
-    version=get_version(),
-    packages=find_packages(),
-    include_package_data=True,
-    zip_safe=False,
-    license='MIT License',
-    description='Store events that recur in users\' local times.',
-    long_description=open('README.rst').read(),
-    author='Erik Swanson',
-    author_email='theerikswanson@gmail.com',
-    classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
-    ],
-    install_requires=[
-        'Django>=2.2',
-        'ambition-django-timezone-field>=2.0.4',
-        'fleming>=0.6.0',
-        'python-dateutil',
-        'pytz',
-    ],
-    tests_require=[
-        'django-nose>=1.4',
-        'django-dynamic-fixture',
-        'mock',
-    ],
-    test_suite='run_tests.run_tests'
-)
+import re
+from setuptools import setup, find_packages
+
+import multiprocessing
+assert multiprocessing
+
+
+def get_version():
+    """
+    Extracts the version number from the version.py file.
+    """
+    VERSION_FILE = 'localized_recurrence/version.py'
+    mo = re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', open(VERSION_FILE, 'rt').read(), re.M)
+    if mo:
+        return mo.group(1)
+    else:
+        raise RuntimeError('Unable to find version string in {0}.'.format(VERSION_FILE))
+
+
+def get_lines(file_path):
+    return open(file_path, 'r').read().split('\n')
+
+
+install_requires = get_lines('requirements/requirements.txt')
+tests_require = get_lines('requirements/requirements-testing.txt')
+
+
+setup(
+    name='django-localized-recurrence',
+    version=get_version(),
+    packages=find_packages(),
+    include_package_data=True,
+    zip_safe=False,
+    license='MIT License',
+    description='Store events that recur in users\' local times.',
+    long_description=open('README.rst').read(),
+    author='Erik Swanson',
+    author_email='theerikswanson@gmail.com',
+    classifiers=[
+        'Environment :: Web Environment',
+        'Framework :: Django',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Internet :: WWW/HTTP',
+        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+    ],
+    install_requires=install_requires,
+    tests_require=tests_require,
+    test_suite='run_tests.run_tests'
+)
```

