# Comparing `tmp/wemp-1.0.2-py3-none-any.whl.zip` & `tmp/wemp-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4808 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     8224 b- defN 23-Jun-27 10:51 wemp/__init__.py
+Zip file size: 4900 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     8636 b- defN 23-Jun-27 10:59 wemp/__init__.py
 -rw-rw-r--  2.0 unx      120 b- defN 23-Jun-12 14:45 wemp/__main__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-12 15:33 wemp/http.py
--rw-rw-r--  2.0 unx      269 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-27 10:51 wemp-1.0.2.dist-info/RECORD
-8 files, 10430 bytes uncompressed, 3784 bytes compressed:  63.7%
+-rw-rw-r--  2.0 unx      269 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/RECORD
+8 files, 10842 bytes uncompressed, 3876 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wemp/__main__.py
 Comment: 
 
 Filename: wemp/http.py
 Comment: 
 
-Filename: wemp-1.0.2.dist-info/METADATA
+Filename: wemp-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: wemp-1.0.2.dist-info/WHEEL
+Filename: wemp-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: wemp-1.0.2.dist-info/entry_points.txt
+Filename: wemp-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: wemp-1.0.2.dist-info/top_level.txt
+Filename: wemp-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: wemp-1.0.2.dist-info/RECORD
+Filename: wemp-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wemp/__init__.py

```diff
@@ -160,21 +160,34 @@
         self.remargs = remargs
         return getattr(self, cmd)(args)
 
     def watch(self, args : argparse.Namespace):
         
         file = args.file
         pid  = args.pid
+        wait_file = args.wait_file
         token = self.cfg.get_cfg("UserName") + "/" + args.token
 
         if pid is not None:
             if not pid_is_live(pid):
                 print(f"This pid[{pid}] is not live")
                 return False
 
+        if wait_file:
+            i = 0
+            while not os.path.isfile(file):
+                i += 1
+
+                if i == 1:
+                    print(f"Wait file: {file}")
+
+                time.sleep(1)
+            
+            print(f"Found watch file: {file}")
+        
         if not os.path.isfile(file):
             print(f"Is not a file: {file}")
             return False
         
         file_size = os.path.getsize(file)
         print(f"Start watching for: {file}, [{file_size} bytes]")
         print(f"You can use [{token}] to view this.")
@@ -244,14 +257,15 @@
             args = ["run", run_name]
 
         cmd = Cmd(self.actions)
         c = cmd.add_cmd("watch", "Get data from server")
         c.add_argument("file", type=str, help="repo name")
         c.add_argument("--token", type=str, default="tmp", help="token")
         c.add_argument("--pid", type=int, help="watch program")
+        c.add_argument("--wait-file", action="store_true", help="wait file")
 
         c = cmd.add_cmd("config", "Config")
         c.add_argument("name", type=str, help="key")
         c.add_argument("value", type=str, help="value")
         return cmd.run(args, remargs)
     
 watch_thread = None
@@ -259,17 +273,17 @@
 def watch(file, token):
 
     cfg     = Config()
     actions = Actions(cfg)
 
     global watch_thread
     def watch_fn(token):
-        actions.watch(argparse.Namespace(file=file, token=token, pid=None))
+        actions.watch(argparse.Namespace(file=file, token=token, pid=None, wait_file=True))
 
-    watch_thread = Thread(target=watch_fn, args=(token)).start()
+    watch_thread = Thread(target=watch_fn, args=(token,)).start()
 
 def stop_watch():
 
     global watch_thread
     if watch_thread is not None:
         watch_thread.join()
```

## Comparing `wemp-1.0.2.dist-info/RECORD` & `wemp-1.0.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-wemp/__init__.py,sha256=j-_k0z98bFqD2LhdaOR76A4CJQOf9fNP7vOTWF1Yc00,8224
+wemp/__init__.py,sha256=ECapc2tbnPDxLAmN3jK4TRztqtSnXVVMD0hSLRLK-yk,8636
 wemp/__main__.py,sha256=C1ICCzLNTtUvY9b_MVidqdvUDufTmVxOAWBxjiSNiQM,120
 wemp/http.py,sha256=0uId3Zj-IqEZUWNjueiYoV3OQFDGNSnGAJDlGvONJ28,1086
-wemp-1.0.2.dist-info/METADATA,sha256=D8gjRJZPJ-UPaC0mQaiHREBJurUxyBbibwq9go_3ue8,269
-wemp-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wemp-1.0.2.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
-wemp-1.0.2.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
-wemp-1.0.2.dist-info/RECORD,,
+wemp-1.0.3.dist-info/METADATA,sha256=bi0VVz8F9fvqbDTv56ngN7vKIJzGANm1Fl6BuVFkkOw,269
+wemp-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+wemp-1.0.3.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
+wemp-1.0.3.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
+wemp-1.0.3.dist-info/RECORD,,
```

