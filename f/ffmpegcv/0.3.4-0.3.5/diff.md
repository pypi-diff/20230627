# Comparing `tmp/ffmpegcv-0.3.4.tar.gz` & `tmp/ffmpegcv-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.3.4.tar", last modified: Tue Jun 27 06:20:09 2023, max compression
+gzip compressed data, was "dist/ffmpegcv-0.3.5.tar", last modified: Tue Jun 27 10:33:37 2023, max compression
```

## Comparing `ffmpegcv-0.3.4.tar` & `ffmpegcv-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12930 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12711 2023-06-27 06:12:44.000000 ffmpegcv-0.3.4/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10510 2023-06-27 05:28:52.000000 ffmpegcv-0.3.4/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      631 2023-06-27 05:41:10.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2259 2023-06-24 13:18:20.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     4128 2023-06-26 16:58:44.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2445 2023-06-27 05:43:48.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.4/ffmpegcv/stream_info.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.4/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12930 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      519 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-27 06:18:40.000000 ffmpegcv-0.3.4/setup.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12966 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12747 2023-06-27 06:23:38.000000 ffmpegcv-0.3.5/README.md
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10510 2023-06-27 05:28:52.000000 ffmpegcv-0.3.5/ffmpegcv/__init__.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_framepick.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      631 2023-06-27 05:41:10.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_laggy.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2513 2023-06-27 10:16:24.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     4128 2023-06-26 16:58:44.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2606 2023-06-27 09:58:14.000000 ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.5/ffmpegcv/stream_info.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.5/ffmpegcv/video_info.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12966 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      519 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-27 10:33:37.000000 ffmpegcv-0.3.5/setup.cfg
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-27 10:29:42.000000 ffmpegcv-0.3.5/setup.py
```

### Comparing `ffmpegcv-0.3.4/PKG-INFO` & `ffmpegcv-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
@@ -29,15 +29,15 @@
 
 ## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
 - `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
-- `noblck`: Read/Write a video file in background.
+- `noblck`: Read/Write a video file in background using mulitprocssing.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -339,17 +339,18 @@
     pass
 ```
 
 ## Noblock
 A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
 > ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> 
 > ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
-#Proxy any VideoCapture args and kargs
+#Proxy any VideoCapture&VideoWriter args and kargs
 vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
```

### Comparing `ffmpegcv-0.3.4/README.md` & `ffmpegcv-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
 - `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
-- `noblck`: Read/Write a video file in background.
+- `noblck`: Read/Write a video file in background using mulitprocssing.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -330,17 +330,18 @@
     pass
 ```
 
 ## Noblock
 A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
 > ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> 
 > ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
-#Proxy any VideoCapture args and kargs
+#Proxy any VideoCapture&VideoWriter args and kargs
 vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
```

### Comparing `ffmpegcv-0.3.4/ffmpegcv/__init__.py` & `ffmpegcv-0.3.5/ffmpegcv/__init__.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_framepick.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_framepick.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_noblock.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_noblock.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_laggy.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_laggy.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_noblock.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_noblock.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,39 +23,43 @@
 
         # 将共享内存的NumPy数组转换为NumPy数组
         self.np_array = np.frombuffer(shared_array.get_obj(), dtype=np.uint8).reshape((NFRAME,*self.out_numpy_shape))
         
         self.shared_array = shared_array
         self.vcap_args = vcap_args
         self.vcap_kwargs = vcap_kwargs
-        self.q = Queue(maxsize=NFRAME-1)
+        self.q = Queue(maxsize=(NFRAME-1)*2)
         self.vcap_fun = vcap_fun
         self.has_init = False
         self.process = None
 
     def read(self):
         if not self.has_init:
             self.has_init = True
             process = multiprocessing.Process(target=child_process, 
                                               args=(self.shared_array, self.q, self.vcap_fun,
                                                     self.vcap_args, self.vcap_kwargs))
             process.start()
             self.process = process
         
-        data_id = self.q.get()
+        self.q.get() # 等待子进程写入
+        data_id = self.q.get() # 读取子进程写入的数据
         if data_id is None:
             return False, None
         else:
             self.iframe += 1
             return True, self.np_array[data_id]
 
 
 def child_process(shared_array, q:Queue, vcap_fun, vcap_args, vcap_kwargs):
     vid = vcap_fun(*vcap_args, **vcap_kwargs)
     np_array = np.frombuffer(shared_array.get_obj(), dtype=np.uint8).reshape((NFRAME,*vid.out_numpy_shape))
+    anything = True
     with vid:
         for i, img in enumerate(vid):
             iloop = i % NFRAME
-            q.put(iloop)
             # 在子进程中修改共享内存的NumPy数组
+            q.put(anything) # 通知主进程可以读取了
             np_array[iloop] = img
+            q.put(iloop)  # 通知主进程已经写入了
+        q.put(anything) # 通知主进程可以读取了
         q.put(None)
```

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_stream.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_reader_stream.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer_noblock.py` & `ffmpegcv-0.3.5/ffmpegcv/ffmpeg_writer_noblock.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,18 @@
                       'filename', 'size', 'bitrate']
         for name in props_name:
             setattr(self, name, getattr(vid, name, None))
 
         self.vwriter_fun = vwriter_fun
         self.vwriter_args = vwriter_args
         self.vwriter_kwargs = vwriter_kwargs
-        self.q = Queue(maxsize=NFRAME-1)
+        self.q = Queue(maxsize=(NFRAME-1)*2)
         self.waitInit = True
         self.process = None
+        self._anything = True
 
     def write(self, img:np.ndarray):
         if self.waitInit:
             if self.size is None:
                 self.size = (img.shape[1], img.shape[0])
                 self.in_numpy_shape = img.shape
                 self._init_share_array()
@@ -36,31 +37,34 @@
                 process.start()
                 self.process = process
             self.width, self.height = self.size
             self.waitInit = False
 
         self.iframe += 1
         data_id = self.iframe % NFRAME
-        self.q.put(data_id)
+        self.q.put(self._anything) # 排队
         self.np_array[data_id] = img
+        self.q.put(data_id)
 
     def _init_share_array(self):
         self.shared_array = Array('b', int(NFRAME*np.prod(self.in_numpy_shape)))
         self.np_array = np.frombuffer(self.shared_array.get_obj(), dtype=np.uint8).reshape((NFRAME,*self.in_numpy_shape))
 
     def release(self):
         if self.process is not None and self.process.is_alive():
+            self.q.put(self._anything)
             self.q.put(None)
             self.process.join()
 
 
 def child_process(shared_array, q:Queue, in_numpy_shape, vwriter_fun, vwriter_args, vwriter_kwargs):
     vid = vwriter_fun(*vwriter_args, **vwriter_kwargs)
     np_array = np.frombuffer(shared_array.get_obj(), dtype=np.uint8).reshape((NFRAME,*in_numpy_shape))
     with vid:
         while True:
+            q.get() # 等待写入的信号
             data_id = q.get()
             if data_id is None:
                 break
             else:
                 img = np_array[data_id]
                 vid.write(img)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ffmpegcv-0.3.4/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.5/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv/video_info.py` & `ffmpegcv-0.3.5/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.5/ffmpegcv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
@@ -29,15 +29,15 @@
 
 ## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
 - `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
-- `noblck`: Read/Write a video file in background.
+- `noblck`: Read/Write a video file in background using mulitprocssing.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -339,17 +339,18 @@
     pass
 ```
 
 ## Noblock
 A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
 > ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> 
 > ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
-#Proxy any VideoCapture args and kargs
+#Proxy any VideoCapture&VideoWriter args and kargs
 vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
```

### Comparing `ffmpegcv-0.3.4/ffmpegcv.egg-info/SOURCES.txt` & `ffmpegcv-0.3.5/ffmpegcv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.4/setup.py` & `ffmpegcv-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.4', # 版本号
+    version='0.3.5', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://github.com/chenxinfeng4/ffmpegcv',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

