# Comparing `tmp/showroom-recorder-0.6.2.tar.gz` & `tmp/showroom-recorder-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.2.tar", last modified: Tue Jun 27 05:49:03 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.3.tar", last modified: Tue Jun 27 13:00:10 2023, max compression
```

## Comparing `showroom-recorder-0.6.2.tar` & `showroom-recorder-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      544 2023-06-27 02:52:25.000000 showroom-recorder-0.6.2/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.151846 showroom-recorder-0.6.2/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.151846 showroom-recorder-0.6.2/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.2/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1304 2023-06-26 13:07:36.000000 showroom-recorder-0.6.2/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     8266 2023-06-27 05:17:39.000000 showroom-recorder-0.6.2/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     4375 2023-06-26 13:35:58.000000 showroom-recorder-0.6.2/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.2/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 05:48:26.000000 showroom-recorder-0.6.2/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 05:49:03.155846 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      815 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       59 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 05:49:03.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.2/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.3/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.552925 showroom-recorder-0.6.3/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.552925 showroom-recorder-0.6.3/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.3/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2698 2023-06-27 12:53:34.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9592 2023-06-27 12:56:05.000000 showroom-recorder-0.6.3/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.3/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 12:48:14.000000 showroom-recorder-0.6.3/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      842 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 13:00:10.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.3/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:00:10.556925 showroom-recorder-0.6.3/test/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      461 2023-06-27 11:13:24.000000 showroom-recorder-0.6.3/test/test.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      927 2023-06-27 12:43:33.000000 showroom-recorder-0.6.3/test/test2.py
```

### Comparing `showroom-recorder-0.6.2/LICENSE` & `showroom-recorder-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/PKG-INFO` & `showroom-recorder-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.2
+Version: 0.6.3
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.2/README.md` & `showroom-recorder-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/description.md` & `showroom-recorder-0.6.3/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/setup.py` & `showroom-recorder-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/showroom-recorder.json` & `showroom-recorder-0.6.3/showroom-recorder.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920634920634921%*

 * *Differences: {"'install_requires'": "{insert: [(6, 'biliup')]}"}*

```diff
@@ -7,14 +7,15 @@
     "description": "Recording Showroom Streaming Video",
     "install_requires": [
         "emoji",
         "pytz",
         "requests",
         "websocket_client",
         "ffmpeg-python",
-        "webdav4"
+        "webdav4",
+        "biliup"
     ],
     "keywords": "video download showroom",
     "license": "GPL",
     "name": "showroom-recorder",
     "url": "https://github.com/vacabun/showroom-recorder"
 }
```

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder/common.py` & `showroom-recorder-0.6.3/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.3/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.3/src/showroom_recorder/processor/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import logging
 import threading
 import ffmpeg
 import json
 import requests
 import datetime
 import pytz
-from .uploader import UploaderQueue, UploaderWebDav
-import random
+from .uploader import UploaderQueue, UploaderWebDav, UploaderBili
+from ..utils.config import get_bili_cookie, get_biliup_list
 import re
 
 fake_headers = {
     'Accept': '*/*',
     'Accept-Encoding': 'gzip, deflate, br',
     'Accept-Language': 'zh,en-US;q=0.9,en;q=0.8,zh-CN;q=0.7,ja;q=0.6',
     'Accept-Charset': 'UTF-8,*;q=0.5',
@@ -39,25 +39,29 @@
         if match:
             room_id = match.group(1)
             return room_id
     except Exception:
         raise Exception('get room_id error.')
 
 
-def get_online_by_roomid(room_id):
+def get_online_by_liveinfo(liveinfo):
+    if liveinfo['live_status'] == 2:
+        return True
+    else:
+        return False
+
+
+def get_liveinfo_by_roomid(room_id):
     url = "https://www.showroom-live.com/api/live/live_info"
     params = {
         "room_id": room_id
     }
     response = requests.get(url=url, headers=fake_headers, params=params)
     response = response.json()
-    if response['live_status'] == 2:
-        return True
-    else:
-        return False
+    return response
 
 
 def get_room_url_key_by_status(status):
     return status['room_url_key']
 
 
 def get_roomid_by_status(status):
@@ -100,37 +104,44 @@
                 stream_url = streaming_url['url']
     except Exception as e:
         raise Exception('get stream url error: ' + e)
     return stream_url
 
 
 class Recorder:
-    def __init__(self, room_url_key, room_id, uploader_queue, config):
+    def __init__(self, room_url_key, live_info, uploader_queue, config):
         self.room_url_key = room_url_key
-        self.room_id = room_id
+        self.live_info = live_info
+        self.room_name = live_info['room_name']
+        self.room_id = live_info['room_id']
         self.uploader_queue = uploader_queue
         self.config = config
         self.is_recording = False
         self._thread = None
         self.ffmpeg_proc = None
         self.output = ''
         self.user_agent = ''
+        self.upload_to_bilibili = False
+        self.time_str = ''
 
     def start(self):
         self._thread = threading.Thread(target=self.record)
         self._thread.daemon = True
         self._thread.start()
 
     def quit(self):
         try:
             self.ffmpeg_proc.stdin.write('q'.encode('utf-8'))
         except Exception:
             pass
         # self._thread.join()
 
+    def enable_uploader_bili(self):
+        self.upload_to_bilibili = True
+
     def record(self):
         self.is_recording = True
         logging.info('{room_url_key}: is on live, start recording video.'.format(
             room_url_key=self.room_url_key))
         try:
             if not os.path.isdir('videos'):
                 os.makedirs('videos')
@@ -142,17 +153,19 @@
 
     def download(self, output_dir='.'):
         try:
             stream_url = get_stream_url_by_roomid(self.room_id)
         except Exception as e:
             raise Exception('get stream url error: ' + e)
 
+        self.time_str = get_time_now().strftime('%Y%m%d_%H%M%S')
+
         title = '{name}_{time}'.format(
             name=self.room_url_key,
-            time=get_time_now().strftime('%Y%m%d_%H%M%S'))
+            time=self.time_str)
 
         self.output = output_dir + '/' + title + '.' + 'mp4'
 
         kwargs_dict = {'c:v': 'copy',
                        'c:a': 'copy',
                        'bsf:a': 'aac_adtstoasc',
                        'loglevel': 'error'}
@@ -173,33 +186,44 @@
             raise Exception(e)
         return True
 
     def __download_finish(self):
         if os.path.exists(self.output):
             logging.info('{room_url_key}: video recording finished, saved to {output}.'.format(
                 room_url_key=self.room_url_key, output=self.output))
-            if self.config['upload_webdav']:
-                uploader = UploaderWebDav(self.output,
-                                          self.output,
-                                          self.config['webdav_url'],
-                                          self.config['webdav_username'],
-                                          self.config['webdav_password'])
-                self.uploader_queue.put(uploader)
 
+            if self.upload_to_bilibili:
+                uploader_bili = UploaderBili(file_path=self.output,
+                                             room_url_key=self.room_url_key,
+                                             room_name=self.room_name,
+                                             time_str=self.time_str,
+                                             login_cookie=get_bili_cookie('bili_cookie.json'))
+                self.uploader_queue.put(uploader_bili)
+
+            if self.config['upload_webdav']:
+                uploader_webdav = UploaderWebDav(self.output,
+                                                 self.output,
+                                                 self.config['webdav_url'],
+                                                 self.config['webdav_username'],
+                                                 self.config['webdav_password'])
+                if(self.config['webdav_delete_source_file']):
+                    uploader_webdav.enable_delete_source_file()
+                self.uploader_queue.put(uploader_webdav)
 
 class RecroderManager:
     def __init__(self, room_url_key_list, config):
         self.room_url_key_list = room_url_key_list
         self.room_id_list = self.__get_room_id_list()
         self.rooms_num = len(self.room_url_key_list)
         self.recorders = [None] * self.rooms_num
         self.t = None
         self._isQuit = False
         self.config = config
         self.uploader_queue = UploaderQueue()
+        self.biliup_list = get_biliup_list('biliup.list')
 
     def quit(self):
         self._isQuit = True
         self.t.join()
 
     def start(self):
         self.t = threading.Thread(target=self.manager)
@@ -226,23 +250,26 @@
                         continue
                     else:
                         self.recorders[i] = None
                         logging.info('{room_url_key}: delete recorder.'.format(
                             room_url_key=room_url_key))
                 if self.recorders[i] is None:
                     try:
-                        is_live = get_online_by_roomid(room_id)
+                        live_info = get_liveinfo_by_roomid(room_id)
+                        is_live = get_online_by_liveinfo(live_info)
                     except Exception:
                         logging.error('{room_url_key}: get online error wait 30s....'.format(
                             room_url_key=room_url_key))
                         time.sleep(30)
                     if is_live:
                         try:
-                            r = Recorder(room_url_key, room_id,
+                            r = Recorder(room_url_key, live_info,
                                          self.uploader_queue, self.config)
+                            if room_url_key in self.biliup_list:
+                                r.enable_uploader_bili()
                             r.start()
                             self.recorders[i] = r
                             continue
                         except Exception as e:
                             logging.error('{room_url_key}: {e}'.format(
                                 room_url_key=room_url_key, e=e))
-            time.sleep(10)
+            time.sleep(int(self.config['interval']))
```

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.3/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.3/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.2
+Version: 0.6.3
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.2/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.3/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 src/showroom_recorder.egg-info/zip-safe
 src/showroom_recorder/processor/__init__.py
 src/showroom_recorder/processor/danmaku.py
 src/showroom_recorder/processor/uploader.py
 src/showroom_recorder/processor/video.py
 src/showroom_recorder/utils/__init__.py
 src/showroom_recorder/utils/config.py
-src/showroom_recorder/utils/delete_emoji.py
+src/showroom_recorder/utils/delete_emoji.py
+test/test.py
+test/test2.py
```

