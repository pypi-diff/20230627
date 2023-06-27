# Comparing `tmp/showroom-recorder-0.6.4.tar.gz` & `tmp/showroom-recorder-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.4.tar", last modified: Tue Jun 27 13:30:13 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.5.tar", last modified: Tue Jun 27 16:06:00 2023, max compression
```

## Comparing `showroom-recorder-0.6.4.tar` & `showroom-recorder-0.6.5.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.4/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.4/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2952 2023-06-27 13:27:09.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9597 2023-06-27 13:26:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.4/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 13:13:47.000000 showroom-recorder-0.6.4/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.026109 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      842 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 13:30:12.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.4/src/showroom_recorder.egg-info/zip-safe
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 13:30:13.030109 showroom-recorder-0.6.4/test/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      461 2023-06-27 11:13:24.000000 showroom-recorder-0.6.4/test/test.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      927 2023-06-27 12:43:33.000000 showroom-recorder-0.6.4/test/test2.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.5/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.293148 showroom-recorder-0.6.5/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-27 14:29:02.000000 showroom-recorder-0.6.5/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3497 2023-06-27 14:25:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2970 2023-06-27 16:03:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9597 2023-06-27 13:26:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 16:05:21.000000 showroom-recorder-0.6.5/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      835 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/test/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      424 2023-06-27 14:26:00.000000 showroom-recorder-0.6.5/test/test_config.py
```

### Comparing `showroom-recorder-0.6.4/LICENSE` & `showroom-recorder-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/PKG-INFO` & `showroom-recorder-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.4
+Version: 0.6.5
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.4/README.md` & `showroom-recorder-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/description.md` & `showroom-recorder-0.6.5/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/setup.py` & `showroom-recorder-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/showroom-recorder.json` & `showroom-recorder-0.6.5/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/common.py` & `showroom-recorder-0.6.5/src/showroom_recorder/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                                     datefmt='%y%m%d %H:%M:%S')
         fileHandler.setFormatter(fileFmt)
         fileHandler.setLevel(logging.DEBUG)
         log.addHandler(fileHandler)
 
     # build ArgumentParser
     parser = argparse.ArgumentParser(
-        description='download showroom video and  comments')
+        description='download showroom video and comments')
     parser.add_argument('-i', '--id', help='Only monitor this one showroom id. \
                 For more rooms, please edit file "romms.ini".', metavar='SHOWROOM_ID', dest='sr_id')
 
     log.debug('program_settings = {}'.format(danmaku_settings['program_settings']))
     log.debug('danmaku_settings = {}'.format(danmaku_settings['danmaku_settings']))
```

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.5/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/processor/uploader.py` & `showroom-recorder-0.6.5/src/showroom_recorder/processor/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         self.room_name = room_name
         self.time_str = time_str
         self.login_cookie = login_cookie
 
     def upload(self):
         logging.info('upload by biliup.')
         video = Data()
-        video.title = self.room_name + ' ' + self.time_str
-        video.desc = self.room_name + ' ' + self.time_str
+        video.title = self.room_name + ' showroom ' + self.time_str
+        video.desc = self.room_name + ' showroom ' + self.time_str
         video.source = 'https://www.showroom-live.com/' + self.room_url_key
         video.tid = 137
         video.set_tag(['showroom'])
         video.copyright = 2
         lines = 'AUTO'
         tasks = 3
         dtime = 0
```

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.5/src/showroom_recorder/processor/video.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.5/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.5/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.5/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.4
+Version: 0.6.5
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.4/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.5/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 src/showroom_recorder/processor/__init__.py
 src/showroom_recorder/processor/danmaku.py
 src/showroom_recorder/processor/uploader.py
 src/showroom_recorder/processor/video.py
 src/showroom_recorder/utils/__init__.py
 src/showroom_recorder/utils/config.py
 src/showroom_recorder/utils/delete_emoji.py
-test/test.py
-test/test2.py
+test/test_config.py
```

