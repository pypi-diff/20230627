# Comparing `tmp/wemp-1.0.3-py3-none-any.whl.zip` & `tmp/wemp-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4900 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     8636 b- defN 23-Jun-27 10:59 wemp/__init__.py
+Zip file size: 4938 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     8829 b- defN 23-Jun-27 11:07 wemp/__init__.py
 -rw-rw-r--  2.0 unx      120 b- defN 23-Jun-12 14:45 wemp/__main__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-12 15:33 wemp/http.py
--rw-rw-r--  2.0 unx      269 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-27 10:59 wemp-1.0.3.dist-info/RECORD
-8 files, 10842 bytes uncompressed, 3876 bytes compressed:  64.3%
+-rw-rw-r--  2.0 unx      269 b- defN 23-Jun-27 11:07 wemp-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 11:07 wemp-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jun-27 11:07 wemp-1.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 11:07 wemp-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-27 11:07 wemp-1.0.5.dist-info/RECORD
+8 files, 11035 bytes uncompressed, 3914 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wemp/__main__.py
 Comment: 
 
 Filename: wemp/http.py
 Comment: 
 
-Filename: wemp-1.0.3.dist-info/METADATA
+Filename: wemp-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: wemp-1.0.3.dist-info/WHEEL
+Filename: wemp-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: wemp-1.0.3.dist-info/entry_points.txt
+Filename: wemp-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: wemp-1.0.3.dist-info/top_level.txt
+Filename: wemp-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: wemp-1.0.3.dist-info/RECORD
+Filename: wemp-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wemp/__init__.py

```diff
@@ -161,14 +161,15 @@
         return getattr(self, cmd)(args)
 
     def watch(self, args : argparse.Namespace):
         
         file = args.file
         pid  = args.pid
         wait_file = args.wait_file
+        noprint = args.noprint
         token = self.cfg.get_cfg("UserName") + "/" + args.token
 
         if pid is not None:
             if not pid_is_live(pid):
                 print(f"This pid[{pid}] is not live")
                 return False
 
@@ -225,15 +226,17 @@
                         last_line = line
                     else:
                         break
                 
                 if last_line:
                     last_line = last_line.strip().replace("\n", "").replace("\r", "")
                     if last_line:
-                        print(f"Send: {last_line}")
+                        if not noprint:
+                            print(f"Send: {last_line}")
+                            
                         last_message = last_line
                         http.update(update_url, token, last_line)
 
                 time.sleep(1)
 
         heart_thread.join()
         return True
@@ -258,14 +261,15 @@
 
         cmd = Cmd(self.actions)
         c = cmd.add_cmd("watch", "Get data from server")
         c.add_argument("file", type=str, help="repo name")
         c.add_argument("--token", type=str, default="tmp", help="token")
         c.add_argument("--pid", type=int, help="watch program")
         c.add_argument("--wait-file", action="store_true", help="wait file")
+        c.add_argument("--noprint", action="store_true", help="wait file")
 
         c = cmd.add_cmd("config", "Config")
         c.add_argument("name", type=str, help="key")
         c.add_argument("value", type=str, help="value")
         return cmd.run(args, remargs)
     
 watch_thread = None
@@ -273,15 +277,15 @@
 def watch(file, token):
 
     cfg     = Config()
     actions = Actions(cfg)
 
     global watch_thread
     def watch_fn(token):
-        actions.watch(argparse.Namespace(file=file, token=token, pid=None, wait_file=True))
+        actions.watch(argparse.Namespace(file=file, token=token, pid=None, wait_file=True, noprint=True))
 
     watch_thread = Thread(target=watch_fn, args=(token,)).start()
 
 def stop_watch():
 
     global watch_thread
     if watch_thread is not None:
```

## Comparing `wemp-1.0.3.dist-info/RECORD` & `wemp-1.0.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-wemp/__init__.py,sha256=ECapc2tbnPDxLAmN3jK4TRztqtSnXVVMD0hSLRLK-yk,8636
+wemp/__init__.py,sha256=iq8SkO4OzQiHRbaNtP3dlXoZjabu85tzfwGz42zA8Js,8829
 wemp/__main__.py,sha256=C1ICCzLNTtUvY9b_MVidqdvUDufTmVxOAWBxjiSNiQM,120
 wemp/http.py,sha256=0uId3Zj-IqEZUWNjueiYoV3OQFDGNSnGAJDlGvONJ28,1086
-wemp-1.0.3.dist-info/METADATA,sha256=bi0VVz8F9fvqbDTv56ngN7vKIJzGANm1Fl6BuVFkkOw,269
-wemp-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wemp-1.0.3.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
-wemp-1.0.3.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
-wemp-1.0.3.dist-info/RECORD,,
+wemp-1.0.5.dist-info/METADATA,sha256=Fzsy3we_rHUeZVaue_3UsdyjTvN1iOKXuK6mOiMGoWU,269
+wemp-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+wemp-1.0.5.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
+wemp-1.0.5.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
+wemp-1.0.5.dist-info/RECORD,,
```

