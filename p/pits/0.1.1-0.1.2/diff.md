# Comparing `tmp/pits-0.1.1-py3-none-any.whl.zip` & `tmp/pits-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3775 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3245 b- defN 23-Jun-27 05:49 pits/__init__.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1801 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      443 b- defN 23-Jun-27 06:33 pits-0.1.1.dist-info/RECORD
-6 files, 6654 bytes uncompressed, 2977 bytes compressed:  55.3%
+Zip file size: 3774 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3200 b- defN 23-Jun-27 06:57 pits/__init__.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-27 06:59 pits-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1801 b- defN 23-Jun-27 06:59 pits-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 06:59 pits-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 06:59 pits-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      443 b- defN 23-Jun-27 06:59 pits-0.1.2.dist-info/RECORD
+6 files, 6609 bytes uncompressed, 2976 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pits/__init__.py
 Comment: 
 
-Filename: pits-0.1.1.dist-info/LICENSE
+Filename: pits-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pits-0.1.1.dist-info/METADATA
+Filename: pits-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pits-0.1.1.dist-info/WHEEL
+Filename: pits-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pits-0.1.1.dist-info/top_level.txt
+Filename: pits-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pits-0.1.1.dist-info/RECORD
+Filename: pits-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pits/__init__.py

```diff
@@ -19,47 +19,25 @@
             yield f
         finally:
             return
 
 
 class PointInTimeFile:
     def __init__(self, pit_spec=None):
-        self.pit = self.parse_time_point(pit_spec)
+        self.pit = parse_time_point(pit_spec)
         self.filename = None
 
 
     def is_gzipped(self):
         if not self.filename:
             return False
         with builtins.open(self.filename, 'rb') as f:
             return f.read(2) == b'\x1f\x8b'
 
 
-    @staticmethod
-    def parse_time_point(spec):
-        if spec is None:
-            return dt.datetime.now()
-        if not isinstance(spec, str):
-            raise TypeError('spec should be string')
-        s = re.sub(r'[^0-9]', '', spec)
-        if len(s) < 8:
-            raise ValueError('invalid spec {spec}')
-        year = int(s[:4])
-        mon = int(s[4:6])
-        day = int(s[6:8])
-        
-        if len(s) >= 10:
-            hh = len(s) >= 10 and int(s[ 8:10]) or 0
-            mm = len(s) >= 12 and int(s[10:12]) or 0
-            ss = len(s) >= 14 and int(s[12:14]) or 0
-        else:
-            hh, mm, ss = (23, 59, 59)
-        return dt.datetime(year, mon, day, hh, mm, ss)
-
-
     @property
     def format(self):
         return '%Y.%m.%d-%H:%M:%S'
 
 
     @contextmanager
     def open(self, spec, *args, **kw):
@@ -100,8 +78,31 @@
         with fopen(self.filename, *args, **kwargs) as f:
             try:
                 yield f
             finally:
                 pass
 
 
+def parse_time_point(spec):
+    if spec is None:
+        return dt.datetime.now()
+    if isinstance(spec, dt.datetime):
+        return spec
+    if not isinstance(spec, str):
+        raise TypeError('spec should be string')
+    s = re.sub(r'[^0-9]', '', spec)
+    if len(s) < 8:
+        raise ValueError('invalid spec {spec}')
+    year = int(s[:4])
+    mon = int(s[4:6])
+    day = int(s[6:8])
+
+    if len(s) >= 10:
+        hh = len(s) >= 10 and int(s[ 8:10]) or 0
+        mm = len(s) >= 12 and int(s[10:12]) or 0
+        ss = len(s) >= 14 and int(s[12:14]) or 0
+    else:
+        hh, mm, ss = (23, 59, 59)
+    return dt.datetime(year, mon, day, hh, mm, ss)
+
+
 ### pits/__init__.py ends here
```

## Comparing `pits-0.1.1.dist-info/LICENSE` & `pits-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pits-0.1.1.dist-info/METADATA` & `pits-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pits
-Version: 0.1.1
+Version: 0.1.2
 Summary: Point-in-time Storage.
 Author-email: Sun Yijiang <sunyijiang@gmail.com>
 Project-URL: Homepage, https://github.com/sunyj/pits
 Project-URL: Bug Tracker, https://github.com/sunyj/pits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

