# Comparing `tmp/showroom-recorder-0.6.3.tar.gz` & `tmp/showroom-recorder-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.3.tar", last modified: Tue Jun 27 13:00:10 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.4.tar", last modified: Tue Jun 27 13:30:13 2023, max compression
```

## Comparing `showroom-recorder-0.6.3.tar` & `showroom-recorder-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.3/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.552925 showroom-recorder-0.6.3/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.552925 showroom-recorder-0.6.3/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.3/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2698 2023-06-27 12:53:34.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9592 2023-06-27 12:56:05.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 12:48:14.000000 showroom-recorder-0.6.3/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      842 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/zip-safe
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/test/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      461 2023-06-27 11:13:24.000000 showroom-recorder-0.6.3/test/test.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      927 2023-06-27 12:43:33.000000 showroom-recorder-0.6.3/test/test2.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.4/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.4/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2952 2023-06-27 13:27:09.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9597 2023-06-27 13:26:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 13:13:47.000000 showroom-recorder-0.6.4/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      842 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/test/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      461 2023-06-27 11:13:24.000000 showroom-recorder-0.6.4/test/test.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      927 2023-06-27 12:43:33.000000 showroom-recorder-0.6.4/test/test2.py
```

### Comparing `showroom-recorder-0.6.3/LICENSE` & `showroom-recorder-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/PKG-INFO` & `showroom-recorder-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.3
+Version: 0.6.4
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.3/README.md` & `showroom-recorder-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/description.md` & `showroom-recorder-0.6.4/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/setup.py` & `showroom-recorder-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/showroom-recorder.json` & `showroom-recorder-0.6.4/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/common.py` & `showroom-recorder-0.6.4/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.4/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/processor/uploader.py` & `showroom-recorder-0.6.4/src/showroom_recorder/processor/uploader.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,22 +24,26 @@
         video.tid = 137
         video.set_tag(['showroom'])
         video.copyright = 2
         lines = 'AUTO'
         tasks = 3
         dtime = 0
         file_list = [self.file_path]
-        with BiliBili(video) as bili:
-            bili.login("bili.cookie", self.login_cookie)
-            # bili.login_by_password("username", "password")
-            for file in file_list:
-                video_part = bili.upload_file(file, lines=lines, tasks=tasks)
-                video.append(video_part)
-            video.delay_time(dtime)
-            bili.submit()
+        try:
+            with BiliBili(video) as bili:
+                bili.login("bili.cookie", self.login_cookie)
+                # bili.login_by_password("username", "password")
+                for file in file_list:
+                    video_part = bili.upload_file(file, lines=lines, tasks=tasks)
+                    video.append(video_part)
+                video.delay_time(dtime)
+                bili.submit()
+        except Exception as e:
+            logging.error('bilibili upload error: ' + str(e))
+            raise Exception('bilibili upload error.')
 
 
 class UploaderWebDav:
     def __init__(self, from_path, to_path, url, username='', password=''):
         self.from_path = from_path
         self.to_path = to_path
         self.url = url
@@ -52,15 +56,16 @@
 
     def upload(self):
         logging.info('upload by webdav.')
         client = Client(base_url=self.url, auth=(self.username, self.password))
         try:
             client.upload_file(from_path=self.from_path, to_path=self.to_path)
         except Exception as e:
-            logging.error('webdav upload error: ' + e)
+            logging.error('webdav upload error: ' + str(e))
+            raise Exception('webdav upload error.')
         if self.delete_source_file:
             os.remove(self.from_path)
 
 
 class UploaderQueue:
     def __init__(self):
         self.uploader_queue = Queue()
@@ -76,9 +81,9 @@
     def run(self):
         while True:
             if not self.uploader_queue.empty():
                 try:
                     uploader = self.uploader_queue.get()
                     uploader.upload()
                 except Exception as e:
-                    logging.error('upload error:' + e)
+                    logging.error('upload error:' + str(e))
             time.sleep(10)
```

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.4/src/showroom_recorder/processor/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,9 +267,9 @@
                             if room_url_key in self.biliup_list:
                                 r.enable_uploader_bili()
                             r.start()
                             self.recorders[i] = r
                             continue
                         except Exception as e:
                             logging.error('{room_url_key}: {e}'.format(
-                                room_url_key=room_url_key, e=e))
+                                room_url_key=room_url_key, e=str(e)))
             time.sleep(int(self.config['interval']))
```

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.4/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.4/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.4/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.3
+Version: 0.6.4
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.3/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.4/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.3/test/test2.py` & `showroom-recorder-0.6.4/test/test2.py`

 * *Files identical despite different names*

