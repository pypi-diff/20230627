# Comparing `tmp/otel_tracer-0.0.9-py3-none-any.whl.zip` & `tmp/otel_tracer-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4884 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 07:33 otel_tracer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 07:33 otel_tracer/tracing/__init__.py
--rw-r--r--  2.0 unx     1744 b- defN 23-Jun-27 07:33 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx     1969 b- defN 23-Jun-27 07:33 otel_tracer/tracing/queue_instrumentor/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-27 07:33 otel_tracer/tracing/queue_instrumentor/package.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-27 07:33 otel_tracer/tracing/queue_instrumentor/version.py
--rw-r--r--  2.0 unx     2311 b- defN 23-Jun-27 07:33 otel_tracer/tracing/threading_instrumentor/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-27 07:33 otel_tracer/tracing/threading_instrumentor/package.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-27 07:33 otel_tracer/tracing/threading_instrumentor/version.py
--rw-r--r--  2.0 unx      670 b- defN 23-Jun-27 07:33 otel_tracer-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 07:33 otel_tracer-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-27 07:33 otel_tracer-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-27 07:33 otel_tracer-0.0.9.dist-info/RECORD
-13 files, 8143 bytes uncompressed, 2804 bytes compressed:  65.6%
+Zip file size: 4889 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 08:10 otel_tracer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 08:10 otel_tracer/tracing/__init__.py
+-rw-r--r--  2.0 unx     1744 b- defN 23-Jun-27 08:10 otel_tracer/tracing/tracer.py
+-rw-r--r--  2.0 unx     1956 b- defN 23-Jun-27 08:10 otel_tracer/tracing/queue_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-27 08:10 otel_tracer/tracing/queue_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-27 08:10 otel_tracer/tracing/queue_instrumentor/version.py
+-rw-r--r--  2.0 unx     2311 b- defN 23-Jun-27 08:10 otel_tracer/tracing/threading_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-27 08:10 otel_tracer/tracing/threading_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-27 08:10 otel_tracer/tracing/threading_instrumentor/version.py
+-rw-r--r--  2.0 unx      670 b- defN 23-Jun-27 08:11 otel_tracer-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 08:11 otel_tracer-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-27 08:11 otel_tracer-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-27 08:11 otel_tracer-0.1.0.dist-info/RECORD
+13 files, 8130 bytes uncompressed, 2809 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: otel_tracer/tracing/threading_instrumentor/package.py
 Comment: 
 
 Filename: otel_tracer/tracing/threading_instrumentor/version.py
 Comment: 
 
-Filename: otel_tracer-0.0.9.dist-info/METADATA
+Filename: otel_tracer-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: otel_tracer-0.0.9.dist-info/WHEEL
+Filename: otel_tracer-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: otel_tracer-0.0.9.dist-info/top_level.txt
+Filename: otel_tracer-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_tracer-0.0.9.dist-info/RECORD
+Filename: otel_tracer-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otel_tracer/tracing/queue_instrumentor/__init__.py

```diff
@@ -23,17 +23,17 @@
         with self.tracer.start_as_current_span("queue_put_event", context=ctx):
             event_span = trace.get_current_span()
             super().put(EventWithSpan(item, event_span), block=block, timeout=timeout)
 
     def get(self, block=True, timeout=None, *args, **kwargs):
         event_with_span = super().get(block=block, timeout=timeout)
         parent_span = event_with_span.span
-        ctx = trace.set_span_in_context(parent_span)
-        with self.tracer.start_as_current_span("queue_get_event", context=ctx):
-            return event_with_span.event, trace.get_current_span()
+        # ctx = trace.set_span_in_context(parent_span)
+        # with self.tracer.start_as_current_span("queue_get_event", context=ctx):
+        return event_with_span.event, parent_span
 
 
 class QueueInstrumentor(BaseInstrumentor):
     original_queuecls = queue.Queue
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
```

## Comparing `otel_tracer-0.0.9.dist-info/METADATA` & `otel_tracer-0.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-tracer
-Version: 0.0.9
+Version: 0.1.0
 Summary: common python utilities for VxRail
 Home-page: UNKNOWN
 Author: VxRail
 Author-email: UNKNOWN
 License: ToBeDone
 Platform: python3
 Requires-Dist: flask
```

## Comparing `otel_tracer-0.0.9.dist-info/RECORD` & `otel_tracer-0.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 otel_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/tracer.py,sha256=NdPjLbjRFKpsTgQX0u2OgeiCjLmfiyYzZ_5NI5KyKWE,1744
-otel_tracer/tracing/queue_instrumentor/__init__.py,sha256=JuDYZMkRhoRKDhlSiZ1zvkgGpU90hgRyBaUHlDAs9nQ,1969
+otel_tracer/tracing/queue_instrumentor/__init__.py,sha256=D13BHg0W09DFZY62wF1R-trfcxkn92-j0V664vBu5KM,1956
 otel_tracer/tracing/queue_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
 otel_tracer/tracing/queue_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
 otel_tracer/tracing/threading_instrumentor/__init__.py,sha256=WiDsbWKvP43CJ8H8Q6SrUV4fofZqF7qfLlHbs0fYyMY,2311
 otel_tracer/tracing/threading_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
 otel_tracer/tracing/threading_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
-otel_tracer-0.0.9.dist-info/METADATA,sha256=Y9xA1Avw840aSbLr_NzAtilp3GjZ00pxVbsvtCbvzOI,670
-otel_tracer-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-otel_tracer-0.0.9.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
-otel_tracer-0.0.9.dist-info/RECORD,,
+otel_tracer-0.1.0.dist-info/METADATA,sha256=4Qj74NIH36BXd0PEkW18gc0bl8CYvEAGE-4d9oJwtPI,670
+otel_tracer-0.1.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+otel_tracer-0.1.0.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
+otel_tracer-0.1.0.dist-info/RECORD,,
```

