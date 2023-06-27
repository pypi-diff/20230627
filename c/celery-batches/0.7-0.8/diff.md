# Comparing `tmp/celery-batches-0.7.tar.gz` & `tmp/celery-batches-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-batches-0.7.tar", last modified: Mon May  2 14:19:30 2022, max compression
+gzip compressed data, was "celery-batches-0.8.tar", last modified: Tue Jun 27 14:30:30 2023, max compression
```

## Comparing `celery-batches-0.7.tar` & `celery-batches-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2022-05-02 14:19:30.310991 celery-batches-0.7/
--rw-r--r--   0 clokep     (501) staff       (20)     2770 2022-02-22 19:08:16.000000 celery-batches-0.7/LICENSE
--rw-r--r--   0 clokep     (501) staff       (20)     3498 2022-05-02 14:19:30.311122 celery-batches-0.7/PKG-INFO
--rw-r--r--   0 clokep     (501) staff       (20)     1982 2022-04-26 19:41:03.000000 celery-batches-0.7/README.rst
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2022-05-02 14:19:30.309324 celery-batches-0.7/celery_batches/
--rw-r--r--   0 clokep     (501) staff       (20)    11062 2022-04-27 18:14:02.000000 celery-batches-0.7/celery_batches/__init__.py
--rw-r--r--   0 clokep     (501) staff       (20)     2305 2022-04-08 19:20:36.000000 celery-batches-0.7/celery_batches/trace.py
-drwxr-xr-x   0 clokep     (501) staff       (20)        0 2022-05-02 14:19:30.310804 celery-batches-0.7/celery_batches.egg-info/
--rw-r--r--   0 clokep     (501) staff       (20)     3498 2022-05-02 14:19:29.000000 celery-batches-0.7/celery_batches.egg-info/PKG-INFO
--rw-r--r--   0 clokep     (501) staff       (20)      283 2022-05-02 14:19:30.000000 celery-batches-0.7/celery_batches.egg-info/SOURCES.txt
--rw-r--r--   0 clokep     (501) staff       (20)        1 2022-05-02 14:19:29.000000 celery-batches-0.7/celery_batches.egg-info/dependency_links.txt
--rw-r--r--   0 clokep     (501) staff       (20)       17 2022-05-02 14:19:30.000000 celery-batches-0.7/celery_batches.egg-info/requires.txt
--rw-r--r--   0 clokep     (501) staff       (20)       15 2022-05-02 14:19:30.000000 celery-batches-0.7/celery_batches.egg-info/top_level.txt
--rw-r--r--   0 clokep     (501) staff       (20)      380 2022-04-08 19:20:36.000000 celery-batches-0.7/pyproject.toml
--rw-r--r--   0 clokep     (501) staff       (20)     1689 2022-05-02 14:19:30.311688 celery-batches-0.7/setup.cfg
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.788544 celery-batches-0.8/
+-rw-r--r--   0 clokep     (501) staff       (20)     2770 2022-02-22 19:08:16.000000 celery-batches-0.8/LICENSE
+-rw-r--r--   0 clokep     (501) staff       (20)     3549 2023-06-27 14:30:30.788704 celery-batches-0.8/PKG-INFO
+-rw-r--r--   0 clokep     (501) staff       (20)     2052 2023-06-27 14:29:38.000000 celery-batches-0.8/README.rst
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.785794 celery-batches-0.8/celery_batches/
+-rw-r--r--   0 clokep     (501) staff       (20)    11315 2022-10-24 19:42:02.000000 celery-batches-0.8/celery_batches/__init__.py
+-rw-r--r--   0 clokep     (501) staff       (20)     2305 2022-04-08 19:20:36.000000 celery-batches-0.8/celery_batches/trace.py
+drwxr-xr-x   0 clokep     (501) staff       (20)        0 2023-06-27 14:30:30.788245 celery-batches-0.8/celery_batches.egg-info/
+-rw-r--r--   0 clokep     (501) staff       (20)     3549 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/PKG-INFO
+-rw-r--r--   0 clokep     (501) staff       (20)      283 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/SOURCES.txt
+-rw-r--r--   0 clokep     (501) staff       (20)        1 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/dependency_links.txt
+-rw-r--r--   0 clokep     (501) staff       (20)       17 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/requires.txt
+-rw-r--r--   0 clokep     (501) staff       (20)       15 2023-06-27 14:30:30.000000 celery-batches-0.8/celery_batches.egg-info/top_level.txt
+-rw-r--r--   0 clokep     (501) staff       (20)      380 2022-04-08 19:20:36.000000 celery-batches-0.8/pyproject.toml
+-rw-r--r--   0 clokep     (501) staff       (20)     1690 2023-06-27 14:30:30.789468 celery-batches-0.8/setup.cfg
```

### Comparing `celery-batches-0.7/LICENSE` & `celery-batches-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-batches-0.7/PKG-INFO` & `celery-batches-0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: celery-batches
-Version: 0.7
+Version: 0.8
 Summary: Experimental task class that buffers messages and processes them as a list.
 Home-page: https://github.com/clokep/celery-batches
 Author: Patrick Cloke
 Author-email: clokep@patrick.cloke.us
 License: BSD
 Project-URL: Documentation, https://celery-batches.readthedocs.io
 Project-URL: Release notes, https://github.com/clokep/celery-batches/blob/main/CHANGELOG.rst
 Project-URL: Source, https://github.com/clokep/celery-batches
 Project-URL: Funding, https://github.com/sponsors/clokep
 Project-URL: Tracker, https://github.com/clokep/celery-batches/issues
 Keywords: task,job,queue,distributed,messaging,actor
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Celery Batches
 ==============
 
 .. image:: https://img.shields.io/pypi/v/celery-batches.svg
@@ -47,47 +46,47 @@
 Celery Batches provides a ``Task`` class that allows processing of multiple
 Celery task calls together as a list. The buffer of tasks calls is flushed on a
 timer and based on the number of queued tasks.
 
 Some potential use-cases for batching of task calls include:
 
 * De-duplicating tasks.
-* Accumlating / only handling the latest task with similar arguments.
+* Accumulating / only handling the latest task with similar arguments.
 * Bulk inserting / updating of data.
 * Tasks with expensive setup that can run across a range of arguments.
 
 What do I need?
 ===============
 
 celery-batches version runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3 (7.6)
 
-And is tested with Celery >= 4.4.
+And is tested with Celery >= 5.0.
 
 If you're running an older version of Python, you need to be running
 an older version of celery-batches:
 
 - Python 2.7: celery-batches 0.3.
 - Python 3.4: celery-batches 0.2.
 - Python 3.5: celery-batches 0.3.
 - Python 3.6: celery-batches 0.5.
+- Python 3.7: celery-batches 0.7.
 
 If you're running an older version of Celery, you need to be running
 an older version of celery-batches:
 
 - Celery < 4.0: Use `celery.contrib.batches` instead.
 - Celery 4.0 - 4.3: celery-batches 0.3.
+- Celery 4.4: celery-batches 0.7.
 
 History
 =======
 
 Celery Batches was distributed as part of Celery (as ``celery.contrib.batches``)
 until Celery 4.0. This project updates the Batches code to maintain compatiblity
 with newer versions of Celery and other fixes. See the Changelog for details.
 
 Additionally, this repository includes the full history of the code from
 ``celery.contrib.batches``, but rewritten to the ``celery_batches/__init__.py``
 file.
-
-
```

### Comparing `celery-batches-0.7/README.rst` & `celery-batches-0.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,41 +14,43 @@
 Celery Batches provides a ``Task`` class that allows processing of multiple
 Celery task calls together as a list. The buffer of tasks calls is flushed on a
 timer and based on the number of queued tasks.
 
 Some potential use-cases for batching of task calls include:
 
 * De-duplicating tasks.
-* Accumlating / only handling the latest task with similar arguments.
+* Accumulating / only handling the latest task with similar arguments.
 * Bulk inserting / updating of data.
 * Tasks with expensive setup that can run across a range of arguments.
 
 What do I need?
 ===============
 
 celery-batches version runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3 (7.6)
 
-And is tested with Celery >= 4.4.
+And is tested with Celery >= 5.0.
 
 If you're running an older version of Python, you need to be running
 an older version of celery-batches:
 
 - Python 2.7: celery-batches 0.3.
 - Python 3.4: celery-batches 0.2.
 - Python 3.5: celery-batches 0.3.
 - Python 3.6: celery-batches 0.5.
+- Python 3.7: celery-batches 0.7.
 
 If you're running an older version of Celery, you need to be running
 an older version of celery-batches:
 
 - Celery < 4.0: Use `celery.contrib.batches` instead.
 - Celery 4.0 - 4.3: celery-batches 0.3.
+- Celery 4.4: celery-batches 0.7.
 
 History
 =======
 
 Celery Batches was distributed as part of Celery (as ``celery.contrib.batches``)
 until Celery 4.0. This project updates the Batches code to maintain compatiblity
 with newer versions of Celery and other fixes. See the Changelog for details.
```

### Comparing `celery-batches-0.7/celery_batches/__init__.py` & `celery-batches-0.8/celery_batches/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,38 +106,43 @@
 
     #: used by rpc backend when failures reported by parent process
     reply_to = None
 
     #: used similarly to reply_to
     correlation_id = None
 
+    #: includes all of the original request headers
+    request_dict: Optional[Dict[str, Any]] = {}
+
     #: TODO
     chord = None
 
     def __init__(
         self,
         id: str,
         name: str,
         args: Tuple[Any, ...],
         kwargs: Dict[Any, Any],
         delivery_info: dict,
         hostname: str,
         ignore_result: bool,
         reply_to: Optional[str],
         correlation_id: Optional[str],
+        request_dict: Optional[Dict[str, Any]],
     ):
         self.id = id
         self.name = name
         self.args = args
         self.kwargs = kwargs
         self.delivery_info = delivery_info
         self.hostname = hostname
         self.ignore_result = ignore_result
         self.reply_to = reply_to
         self.correlation_id = correlation_id
+        self.request_dict = request_dict
 
     @classmethod
     def from_request(cls, request: Request) -> "SimpleRequest":
         # Support both protocol v1 and v2.
         args, kwargs, embed = request._payload
         # Celery 5.1.0 added an ignore_result option.
         ignore_result = getattr(request, "ignore_result", False)
@@ -147,14 +152,15 @@
             args,
             kwargs,
             request.delivery_info,
             request.hostname,
             ignore_result,
             request.reply_to,
             request.correlation_id,
+            request.request_dict,
         )
 
 
 class Batches(Task):
     abstract = True
 
     # Disable typing since the signature of batch tasks take only a single item
@@ -281,14 +287,15 @@
                 "routing_key": options.get("routing_key"),
                 "priority": options.get("priority"),
             },
             hostname=gethostname(),
             ignore_result=options.get("ignore_result", False),
             reply_to=None,
             correlation_id=None,
+            request_dict={},
         )
 
         return super().apply(([request],), {}, *_args, **options)
 
     def _do_flush(self) -> None:
         logger.debug("Batches: Wake-up to flush buffers...")
```

### Comparing `celery-batches-0.7/celery_batches/trace.py` & `celery-batches-0.8/celery_batches/trace.py`

 * *Files identical despite different names*

### Comparing `celery-batches-0.7/celery_batches.egg-info/PKG-INFO` & `celery-batches-0.8/celery_batches.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: celery-batches
-Version: 0.7
+Version: 0.8
 Summary: Experimental task class that buffers messages and processes them as a list.
 Home-page: https://github.com/clokep/celery-batches
 Author: Patrick Cloke
 Author-email: clokep@patrick.cloke.us
 License: BSD
 Project-URL: Documentation, https://celery-batches.readthedocs.io
 Project-URL: Release notes, https://github.com/clokep/celery-batches/blob/main/CHANGELOG.rst
 Project-URL: Source, https://github.com/clokep/celery-batches
 Project-URL: Funding, https://github.com/sponsors/clokep
 Project-URL: Tracker, https://github.com/clokep/celery-batches/issues
 Keywords: task,job,queue,distributed,messaging,actor
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Celery Batches
 ==============
 
 .. image:: https://img.shields.io/pypi/v/celery-batches.svg
@@ -47,47 +46,47 @@
 Celery Batches provides a ``Task`` class that allows processing of multiple
 Celery task calls together as a list. The buffer of tasks calls is flushed on a
 timer and based on the number of queued tasks.
 
 Some potential use-cases for batching of task calls include:
 
 * De-duplicating tasks.
-* Accumlating / only handling the latest task with similar arguments.
+* Accumulating / only handling the latest task with similar arguments.
 * Bulk inserting / updating of data.
 * Tasks with expensive setup that can run across a range of arguments.
 
 What do I need?
 ===============
 
 celery-batches version runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3 (7.6)
 
-And is tested with Celery >= 4.4.
+And is tested with Celery >= 5.0.
 
 If you're running an older version of Python, you need to be running
 an older version of celery-batches:
 
 - Python 2.7: celery-batches 0.3.
 - Python 3.4: celery-batches 0.2.
 - Python 3.5: celery-batches 0.3.
 - Python 3.6: celery-batches 0.5.
+- Python 3.7: celery-batches 0.7.
 
 If you're running an older version of Celery, you need to be running
 an older version of celery-batches:
 
 - Celery < 4.0: Use `celery.contrib.batches` instead.
 - Celery 4.0 - 4.3: celery-batches 0.3.
+- Celery 4.4: celery-batches 0.7.
 
 History
 =======
 
 Celery Batches was distributed as part of Celery (as ``celery.contrib.batches``)
 until Celery 4.0. This project updates the Batches code to maintain compatiblity
 with newer versions of Celery and other fixes. See the Changelog for details.
 
 Additionally, this repository includes the full history of the code from
 ``celery.contrib.batches``, but rewritten to the ``celery_batches/__init__.py``
 file.
-
-
```

### Comparing `celery-batches-0.7/setup.cfg` & `celery-batches-0.8/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = celery-batches
-version = 0.7
+version = 0.8
 description = Experimental task class that buffers messages and processes them as a list.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Patrick Cloke
 author_email = clokep@patrick.cloke.us
 url = https://github.com/clokep/celery-batches
 keywords = task, job, queue, distributed, messaging, actor
@@ -14,33 +14,33 @@
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: BSD License
 	Topic :: System :: Distributed Computing
 	Topic :: Software Development :: Object Brokering
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Operating System :: OS Independent
 project_urls = 
 	Documentation = https://celery-batches.readthedocs.io
 	Release notes = https://github.com/clokep/celery-batches/blob/main/CHANGELOG.rst
 	Source = https://github.com/clokep/celery-batches
 	Funding = https://github.com/sponsors/clokep
 	Tracker = https://github.com/clokep/celery-batches/issues
 
 [options]
 packages = 
 	celery_batches
-install_requires = celery>=4.4,<5.3
-python_requires = >=3.7
+install_requires = celery>=5.0,<5.3
+python_requires = >=3.8
 
 [flake8]
 extend-ignore = E203
 max-line-length = 88
 
 [isort]
 profile = black
```

