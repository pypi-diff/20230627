# Comparing `tmp/ffmpegcv-0.3.3.tar.gz` & `tmp/ffmpegcv-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.3.3.tar", last modified: Sun Jun 25 17:02:33 2023, max compression
+gzip compressed data, was "dist/ffmpegcv-0.3.4.tar", last modified: Tue Jun 27 06:20:09 2023, max compression
```

## Comparing `ffmpegcv-0.3.3.tar` & `ffmpegcv-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12787 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12568 2023-06-23 19:09:37.000000 ffmpegcv-0.3.3/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10529 2023-06-23 17:47:32.000000 ffmpegcv-0.3.3/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2259 2023-06-24 13:18:20.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_noblock.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.3/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.3/ffmpegcv/stream_info.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.3/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12787 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      458 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-25 17:02:33.000000 ffmpegcv-0.3.3/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-25 17:02:06.000000 ffmpegcv-0.3.3/setup.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12930 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12711 2023-06-27 06:12:44.000000 ffmpegcv-0.3.4/README.md
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10510 2023-06-27 05:28:52.000000 ffmpegcv-0.3.4/ffmpegcv/__init__.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_framepick.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      631 2023-06-27 05:41:10.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10257 2023-06-23 19:17:55.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_laggy.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2259 2023-06-24 13:18:20.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     4128 2023-06-26 16:58:44.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2445 2023-06-27 05:43:48.000000 ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer_noblock.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.4/ffmpegcv/stream_info.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3262 2023-06-25 16:44:45.000000 ffmpegcv-0.3.4/ffmpegcv/video_info.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    12930 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      519 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-27 06:20:09.000000 ffmpegcv-0.3.4/setup.cfg
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      656 2023-06-27 06:18:40.000000 ffmpegcv-0.3.4/setup.py
```

### Comparing `ffmpegcv-0.3.3/PKG-INFO` & `ffmpegcv-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.3
+Version: 0.3.4
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
-- `FFmpegReaderNoblock`: Read a video file in background.
+- `noblck`: Read/Write a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -335,26 +335,28 @@
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 ```
 
-## FFmpegReaderNoblock
-A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+## Noblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
+> ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
 #Proxy any VideoCapture args and kargs
-vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
 
 # this is slow
 vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
-for _ in tqdm.trange(2000):
+for _ in tqdm.trange(1000):
     ret, img = vid.read()         #this read will block cpu, take time
     cpu_tense()
 ```
```

### Comparing `ffmpegcv-0.3.3/README.md` & `ffmpegcv-0.3.4/ffmpegcv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: ffmpegcv
+Version: 0.3.4
+Home-page: https://github.com/chenxinfeng4/ffmpegcv
+Author: chenxf
+Author-email: cxf529125853@163.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # FFMPEGCV is an alternative to OPENCV for video read and write.
 ![Python versions](https://img.shields.io/badge/Python-3.6%2B-blue.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ffmpegcv.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ffmpegcv/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/ffmpegcv.svg)](https://pypistats.org/packages/ffmpegcv)
 ![Code size](https://shields.io/github/languages/code-size/chenxinfeng4/ffmpegcv
 )
 ![Last Commit](https://shields.io/github/last-commit/chenxinfeng4/ffmpegcv)
@@ -20,15 +29,15 @@
 
 ## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
 - `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
-- `FFmpegReaderNoblock`: Read a video file in background.
+- `noblck`: Read/Write a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -326,26 +335,28 @@
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 ```
 
-## FFmpegReaderNoblock
-A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+## Noblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
+> ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
 #Proxy any VideoCapture args and kargs
-vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
 
 # this is slow
 vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
-for _ in tqdm.trange(2000):
+for _ in tqdm.trange(1000):
     ret, img = vid.read()         #this read will block cpu, take time
     cpu_tense()
-```
+```
```

### Comparing `ffmpegcv-0.3.3/ffmpegcv/__init__.py` & `ffmpegcv-0.3.4/ffmpegcv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .ffmpeg_reader import FFmpegReader, FFmpegReaderNV
 from .ffmpeg_writer import FFmpegWriter, FFmpegWriterNV
 from .ffmpeg_reader_camera import FFmpegReaderCAM
 from .ffmpeg_reader_stream import FFmpegReaderStream
-from .ffmpeg_reader_noblock import FFmpegReaderNoblock
+from .ffmpeg_noblock import noblock
 from .video_info import get_num_NVIDIA_GPUs
 import shutil
 from subprocess import DEVNULL, check_output
 
 
 def _check():
     if not shutil.which("ffmpeg") or not shutil.which("ffprobe"):
```

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_framepick.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_framepick.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_laggy.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_laggy.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_noblock.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_noblock.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_reader_stream.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_reader_stream.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.4/ffmpegcv/ffmpeg_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         vid.codec, vid.pix_fmt, vid.filename = codec, pix_fmt, filename
         vid.waitInit = True
         vid.bitrate = bitrate
         return vid
 
     def _init_video_stream(self):
         bitrate_str = f'-b:v {self.bitrate} ' if self.bitrate else ''
-        args = (f'ffmpeg -y -loglevel warning ' 
+        self.ffmpeg_cmd = (f'ffmpeg -y -loglevel warning ' 
                 f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
                 f'{bitrate_str} '
                 f'-r {self.fps} -c:v {self.codec} -pix_fmt yuv420p "{self.filename}"')
-        self.process = run_async(args)
+        self.process = run_async(self.ffmpeg_cmd)
 
-    def write(self, img):
+    def write(self, img:np.ndarray):
         if self.waitInit:
             if self.size is None:
                 self.size = (img.shape[1], img.shape[0])
             self.width, self.height = self.size
             self._init_video_stream()
             self.waitInit = False
 
@@ -106,14 +106,15 @@
         vid.codec, vid.pix_fmt, vid.filename = codec, pix_fmt, filename
         vid.gpu = gpu
         vid.waitInit = True
         vid.bitrate = bitrate
         return vid
 
     def _init_video_stream(self):
+        bitrate_str = f'-b:v {self.bitrate} ' if self.bitrate else ''
         default_preset = 'default' if IN_COLAB else 'p2'
         self.preset = getattr(self, 'preset', default_preset)
-        args = (f'ffmpeg -y -loglevel warning '
+        self.ffmpeg_cmd = (f'ffmpeg -y -loglevel warning '
             f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
-            f'-preset {self.preset} '
+            f'-preset {self.preset} {bitrate_str} '
             f'-r {self.fps} -gpu {self.gpu} -c:v {self.codec} -pix_fmt yuv420p "{self.filename}"')
-        self.process = run_async(args)
+        self.process = run_async(self.ffmpeg_cmd)
```

### Comparing `ffmpegcv-0.3.3/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.4/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv/video_info.py` & `ffmpegcv-0.3.4/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.3/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: ffmpegcv
-Version: 0.3.3
-Home-page: https://github.com/chenxinfeng4/ffmpegcv
-Author: chenxf
-Author-email: cxf529125853@163.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # FFMPEGCV is an alternative to OPENCV for video read and write.
 ![Python versions](https://img.shields.io/badge/Python-3.6%2B-blue.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ffmpegcv.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ffmpegcv/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/ffmpegcv.svg)](https://pypistats.org/packages/ffmpegcv)
 ![Code size](https://shields.io/github/languages/code-size/chenxinfeng4/ffmpegcv
 )
 ![Last Commit](https://shields.io/github/last-commit/chenxinfeng4/ffmpegcv)
@@ -29,15 +20,15 @@
 
 ## Functions:
 - `VideoWriter`: Write a video file.
 - `VideoCapture`: Read a video file.
 - `VideoCaptureNV`: Read a video file by NVIDIA GPU.
 - `VideoCaptureCAM`: Read a camera.
 - `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
-- `FFmpegReaderNoblock`: Read a video file in background.
+- `noblck`: Read/Write a video file in background.
 
 ## Install
 You need to download ffmpeg before you can use ffmpegcv.
 ```
  #1A. LINUX: sudo apt install ffmpeg
  #1B. MAC: brew install ffmpeg
  #1C. WINDOWS: download ffmpeg and add to the path
@@ -335,26 +326,28 @@
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 ```
 
-## FFmpegReaderNoblock
-A proxy to automatic prepare frames in backgroud, which does not block when reading current frame. This make your python program more efficient in CPU usage. Benifit from multicore CPU.
+## Noblock
+A proxy to automatic prepare frames in backgroud, which does not block when reading&writing current frame (multiprocessing). This make your python program more efficient in CPU usage. Up to 2x boost.
 
+> ffmpegcv.VideoCapture(*args) -> ffmpegcv.noblock(ffmpegcv.VideoCapture, *args)
+> ffmpegcv.VideoWriter(*args) -> ffmpegcv.noblock(ffmpegcv.VideoWriter, *args)
 ```python
 #Proxy any VideoCapture args and kargs
-vid_noblock = ffmpegcv.FFmpegReaderNoblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
+vid_noblock = ffmpegcv.noblock(ffmpegcv.VideoCapture, vfile, pix_fmt='rbg24')
 
 # this is fast
 def cpu_tense(): time.sleep(0.01)
 for _ in tqdm.trange(1000):
     ret, img = vid_noblock.read() #current img is already buffered, take no time
     cpu_tense()                   #meanwhile, the next img is buffering in background
 
 # this is slow
 vid = ffmpegcv.VideoCapture(vfile, pix_fmt='rbg24')
-for _ in tqdm.trange(2000):
+for _ in tqdm.trange(1000):
     ret, img = vid.read()         #this read will block cpu, take time
     cpu_tense()
-```
+```
```

### Comparing `ffmpegcv-0.3.3/setup.py` & `ffmpegcv-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.3', # 版本号
+    version='0.3.4', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://github.com/chenxinfeng4/ffmpegcv',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

