# Comparing `tmp/wemp-1.0.1-py3-none-any.whl.zip` & `tmp/wemp-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4712 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     7824 b- defN 23-Jun-13 06:46 wemp/__init__.py
+Zip file size: 4808 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     8224 b- defN 23-Jun-27 10:51 wemp/__init__.py
 -rw-rw-r--  2.0 unx      120 b- defN 23-Jun-12 14:45 wemp/__main__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-12 15:33 wemp/http.py
--rw-rw-r--  2.0 unx      269 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/RECORD
-8 files, 10030 bytes uncompressed, 3688 bytes compressed:  63.2%
+-rw-rw-r--  2.0 unx      269 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/RECORD
+8 files, 10430 bytes uncompressed, 3784 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wemp/__main__.py
 Comment: 
 
 Filename: wemp/http.py
 Comment: 
 
-Filename: wemp-1.0.1.dist-info/METADATA
+Filename: wemp-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: wemp-1.0.1.dist-info/WHEEL
+Filename: wemp-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: wemp-1.0.1.dist-info/entry_points.txt
+Filename: wemp-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: wemp-1.0.1.dist-info/top_level.txt
+Filename: wemp-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wemp-1.0.1.dist-info/RECORD
+Filename: wemp-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wemp/__init__.py

```diff
@@ -143,17 +143,16 @@
     try:
         os.kill(pid, 0)
         return True
     except:
         return False
 
 class Actions:
-    def __init__(self, app):
-        self.app = app
-        self.cfg : Config = app.cfg
+    def __init__(self, cfg):
+        self.cfg : Config = cfg
 
     def private_run_cmd(self, args, remargs):
         
         cmd = args.cmd
         if not hasattr(self, cmd):
             return False
 
@@ -249,8 +248,29 @@
         c.add_argument("file", type=str, help="repo name")
         c.add_argument("--token", type=str, default="tmp", help="token")
         c.add_argument("--pid", type=int, help="watch program")
 
         c = cmd.add_cmd("config", "Config")
         c.add_argument("name", type=str, help="key")
         c.add_argument("value", type=str, help="value")
-        return cmd.run(args, remargs)
+        return cmd.run(args, remargs)
+    
+watch_thread = None
+
+def watch(file, token):
+
+    cfg     = Config()
+    actions = Actions(cfg)
+
+    global watch_thread
+    def watch_fn(token):
+        actions.watch(argparse.Namespace(file=file, token=token, pid=None))
+
+    watch_thread = Thread(target=watch_fn, args=(token)).start()
+
+def stop_watch():
+
+    global watch_thread
+    if watch_thread is not None:
+        watch_thread.join()
+    
+    watch_thread = None
```

## Comparing `wemp-1.0.1.dist-info/RECORD` & `wemp-1.0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-wemp/__init__.py,sha256=t5TjXw-_7m-9DKnLy9K65uK92X9Ab9W35i4Gi0RWvn0,7824
+wemp/__init__.py,sha256=j-_k0z98bFqD2LhdaOR76A4CJQOf9fNP7vOTWF1Yc00,8224
 wemp/__main__.py,sha256=C1ICCzLNTtUvY9b_MVidqdvUDufTmVxOAWBxjiSNiQM,120
 wemp/http.py,sha256=0uId3Zj-IqEZUWNjueiYoV3OQFDGNSnGAJDlGvONJ28,1086
-wemp-1.0.1.dist-info/METADATA,sha256=Tm_VtSZJUKF7dCCy9npiP970SczmSM2eWYS3KU1S01E,269
-wemp-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wemp-1.0.1.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
-wemp-1.0.1.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
-wemp-1.0.1.dist-info/RECORD,,
+wemp-1.0.2.dist-info/METADATA,sha256=D8gjRJZPJ-UPaC0mQaiHREBJurUxyBbibwq9go_3ue8,269
+wemp-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+wemp-1.0.2.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
+wemp-1.0.2.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
+wemp-1.0.2.dist-info/RECORD,,
```

