# Comparing `tmp/lqcv-0.2.0.tar.gz` & `tmp/lqcv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqcv-0.2.0.tar", last modified: Tue Jun 13 09:13:17 2023, max compression
+gzip compressed data, was "lqcv-0.2.1.tar", last modified: Tue Jun 27 03:42:57 2023, max compression
```

## Comparing `lqcv-0.2.0.tar` & `lqcv-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/
--rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-13 09:13:17.405139 lqcv-0.2.0/PKG-INFO
--rw-r--r--   0 laughing  (1000) wheel      (998)      584 2022-07-07 09:32:49.000000 lqcv-0.2.0/README.md
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/
--rw-r--r--   0 laughing  (1000) wheel      (998)       64 2023-06-13 09:12:34.000000 lqcv-0.2.0/lqcv/__init__.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/bbox/
--rw-r--r--   0 laughing  (1000) wheel      (998)       41 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    10031 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/areas.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     5723 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/bbox.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/data/
--rw-r--r--   0 laughing  (1000) wheel      (998)       70 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/__init__.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/data/converter/
--rw-r--r--   0 laughing  (1000) wheel      (998)       94 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    10948 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/base.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3262 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/coco.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4421 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/xml.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4955 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/yolo.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    11718 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/reader.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      407 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/utils.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/simi/
--rw-r--r--   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/simi/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1033 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/simi/hash.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/lqcv/tools/
--rw-r--r--   0 laughing  (1000) wheel      (998)      132 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     2683 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/file.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4034 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/image.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1718 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/video.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/lqcv/utils/
--rw-r--r--   0 laughing  (1000) wheel      (998)       32 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      697 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/log.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     5183 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/ops.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     2122 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/plot.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3570 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/timer.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv.egg-info/
--rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/PKG-INFO
--rw-r--r--   0 laughing  (1000) wheel      (998)      709 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/SOURCES.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)        1 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/dependency_links.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)        5 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/top_level.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)       38 2023-06-13 09:13:17.405139 lqcv-0.2.0/setup.cfg
--rw-r--r--   0 laughing  (1000) wheel      (998)      776 2023-05-30 03:03:32.000000 lqcv-0.2.0/setup.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/test/
--rw-r--r--   0 laughing  (1000) wheel      (998)     2128 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_area.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     2005 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_converter.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1737 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_reader.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      178 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_tool.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.410673 lqcv-0.2.1/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-27 03:42:57.407340 lqcv-0.2.1/PKG-INFO
+-rw-r--r--   0 laughing  (1000) wheel      (998)      584 2022-07-07 09:32:49.000000 lqcv-0.2.1/README.md
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       64 2023-06-27 03:42:05.000000 lqcv-0.2.1/lqcv/__init__.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/bbox/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       41 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/bbox/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    10031 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/bbox/areas.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     5723 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/bbox/bbox.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/data/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       73 2023-06-27 03:41:53.000000 lqcv-0.2.1/lqcv/data/__init__.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/data/converter/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       94 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/data/converter/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    10948 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/data/converter/base.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     3262 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/data/converter/coco.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4421 2023-06-27 03:41:53.000000 lqcv-0.2.1/lqcv/data/converter/xml.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4955 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/data/converter/yolo.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    13871 2023-06-27 03:41:53.000000 lqcv-0.2.1/lqcv/data/reader.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      407 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/data/utils.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/simi/
+-rw-r--r--   0 laughing  (1000) wheel      (998)        0 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/simi/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     1033 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/simi/hash.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/tools/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      132 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/tools/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2683 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/tools/file.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4034 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/tools/image.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     1718 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/tools/video.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv/utils/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       32 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/utils/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      697 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/utils/log.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     5183 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/utils/ops.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2122 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/utils/plot.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     3570 2023-06-27 02:22:45.000000 lqcv-0.2.1/lqcv/utils/timer.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/lqcv.egg-info/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-27 03:42:57.000000 lqcv-0.2.1/lqcv.egg-info/PKG-INFO
+-rw-r--r--   0 laughing  (1000) wheel      (998)      709 2023-06-27 03:42:57.000000 lqcv-0.2.1/lqcv.egg-info/SOURCES.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)        1 2023-06-27 03:42:57.000000 lqcv-0.2.1/lqcv.egg-info/dependency_links.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)        5 2023-06-27 03:42:57.000000 lqcv-0.2.1/lqcv.egg-info/top_level.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)       38 2023-06-27 03:42:57.410673 lqcv-0.2.1/setup.cfg
+-rw-r--r--   0 laughing  (1000) wheel      (998)      776 2023-05-30 03:03:32.000000 lqcv-0.2.1/setup.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-27 03:42:57.407340 lqcv-0.2.1/test/
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2128 2023-06-27 02:22:45.000000 lqcv-0.2.1/test/test_area.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2005 2023-06-27 02:22:45.000000 lqcv-0.2.1/test/test_converter.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2502 2023-06-27 03:41:53.000000 lqcv-0.2.1/test/test_reader.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      178 2023-06-27 02:22:45.000000 lqcv-0.2.1/test/test_tool.py
```

### Comparing `lqcv-0.2.0/PKG-INFO` & `lqcv-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqcv
-Version: 0.2.0
+Version: 0.2.1
 Author: Laughing-q
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 # lqcv
 This is my computer vision lib.
```

### Comparing `lqcv-0.2.0/README.md` & `lqcv-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/bbox/areas.py` & `lqcv-0.2.1/lqcv/bbox/areas.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/bbox/bbox.py` & `lqcv-0.2.1/lqcv/bbox/bbox.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/data/converter/base.py` & `lqcv-0.2.1/lqcv/data/converter/base.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/data/converter/coco.py` & `lqcv-0.2.1/lqcv/data/converter/coco.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/data/converter/xml.py` & `lqcv-0.2.1/lqcv/data/converter/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             if os.path.isfile(xml_file):
                 nf += 1  # label found
                 xml = ET.parse(xml_file).getroot()
                 objects = xml.findall("object")
                 if len(objects):
                     filename = xml.find("filename")
                     assert (filename is not None), f"can't get `filename` info from {xml_file}"
-                    filename = str(filename.text)
-                    # filename = Path(xml_file).name
+                    # filename = str(filename.text)
+                    filename = Path(xml_file).name
                     try:
                         size = xml.find("size")
                         width = size.find("width")
                         height = size.find("height")
                         h = int(height.text)
                         w = int(width.text)
                     except:
```

### Comparing `lqcv-0.2.0/lqcv/data/converter/yolo.py` & `lqcv-0.2.1/lqcv/data/converter/yolo.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/data/reader.py` & `lqcv-0.2.1/lqcv/data/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import cv2
 import time
 from pathlib import Path
 from threading import Thread
 from .utils import IMG_FORMATS, VID_FORMATS
 
 
-class ReadStreams:
+class Streams:
     """Read Streams, modified from yolov5, support multi streams reading, but support one streams saving for now."""
 
     def __init__(self, sources="streams.txt"):
         self.mode = "stream"
 
         if osp.isfile(sources):
             with open(sources, "r") as f:
@@ -94,15 +94,15 @@
             save_path += ".mp4"
             self.vid_writer[i] = cv2.VideoWriter(
                 save_path, cv2.VideoWriter_fourcc(*"mp4v"), int(self.fps[i]), (w, h)
             )
         self.vid_writer[i].write(image)
 
 
-class ReadOneStream:
+class Stream:
     """Read one Stream, modified from yolov5, support one streams reading and saving."""
 
     def __init__(self, source, vid_stride=1, imgsz=None, im_only=False):
         """ReadOneStream
 
         Args:
             source (str): Source, could be a folder or a direct file.
@@ -290,19 +290,83 @@
                 self.vid_writer = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*"mp4v"), self.fps, (w, h))
             self.vid_writer.write(image)
 
     def __len__(self):
         return self.nf  # number of files
 
 
-def create_reader(source: str):
-    """This is for data(video, webcam, image, image_path) reading in inference.
-    Args:
-        source(str): data source, could be a video,image,dir or webcam.
-    Return:
-        reader(ReadVideosAndImages | ReadStreams): data reader.
-        webcam(bool): the source is webcam or not.
-    """
-    is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
-    is_url = source.lower().startswith(("rtsp://", "rtmp://", "http://", "https://"))
-    webcam = source.isnumeric() or source.endswith(".txt") or (is_url and not is_file)
-    return ReadOneStream(source) if webcam else ReadVideosAndImages(source), webcam
+class Images(ReadVideosAndImages):
+    """Read Images."""
+    def __init__(self, source: str, imgsz=None, im_only=False):
+        """Images
+
+        Args:
+            source (str): Source, could be a folder or a direct file.
+            imgsz (tuple | optional): Image size, (height, width)
+            im_only (bool | optional): Whether to return image only, or it'll return
+                image, path and description.
+        """
+        p = str(Path(source).resolve())  # os-agnostic absolute path
+        if "*" in p:
+            files = sorted(glob.glob(p, recursive=True))  # glob
+        elif osp.isdir(p):
+            files = sorted(glob.glob(osp.join(p, "*.*")))  # dir
+        elif osp.isfile(p):
+            files = [p]  # files
+        else:
+            raise Exception(f"ERROR: {p} does not exist")
+
+        # random.shuffle(files)
+        images = [x for x in files if x.split(".")[-1].lower() in IMG_FORMATS]
+        ni = len(images)
+
+        self.files = images
+        self.nf = ni  # number of files
+        self.video_flag = [False] * ni
+        self.mode = "image"
+        self.imgsz = imgsz
+        self.im_only = im_only
+        assert self.nf > 0, (
+            f"No images or videos found in {p}. "
+            f"Supported formats are:\nimages: {IMG_FORMATS}"
+        )
+
+
+class Videos(ReadVideosAndImages):
+    """Read Images."""
+    def __init__(self, source: str, vid_stride=1, imgsz=None, im_only=False):
+        """Images
+
+        Args:
+            source (str): Source, could be a folder or a direct file.
+            vid_stride (int | optional): Video stride.
+            imgsz (tuple | optional): Image size, (height, width)
+            im_only (bool | optional): Whether to return image only, or it'll return
+                image, path and description.
+        """
+        p = str(Path(source).resolve())  # os-agnostic absolute path
+        if "*" in p:
+            files = sorted(glob.glob(p, recursive=True))  # glob
+        elif osp.isdir(p):
+            files = sorted(glob.glob(osp.join(p, "*.*")))  # dir
+        elif osp.isfile(p):
+            files = [p]  # files
+        else:
+            raise Exception(f"ERROR: {p} does not exist")
+
+        # random.shuffle(files)
+        videos = [x for x in files if x.split(".")[-1].lower() in VID_FORMATS]
+        nv = len(videos)
+
+        self.vid_path, self.vid_writer = None, None
+        self.files = videos
+        self.nf = nv  # number of files
+        self.video_flag = [True] * nv
+        self.vid_stride = vid_stride
+        self.mode = "video"
+        self.imgsz = imgsz
+        self.im_only = im_only
+        self.new_video(videos[0])  # new video
+        assert self.nf > 0, (
+            f"No images or videos found in {p}. "
+            f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
+        )
```

### Comparing `lqcv-0.2.0/lqcv/simi/hash.py` & `lqcv-0.2.1/lqcv/simi/hash.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/tools/file.py` & `lqcv-0.2.1/lqcv/tools/file.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/tools/image.py` & `lqcv-0.2.1/lqcv/tools/image.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/tools/video.py` & `lqcv-0.2.1/lqcv/tools/video.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/utils/log.py` & `lqcv-0.2.1/lqcv/utils/log.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/utils/ops.py` & `lqcv-0.2.1/lqcv/utils/ops.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/utils/plot.py` & `lqcv-0.2.1/lqcv/utils/plot.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv/utils/timer.py` & `lqcv-0.2.1/lqcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/lqcv.egg-info/PKG-INFO` & `lqcv-0.2.1/lqcv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqcv
-Version: 0.2.0
+Version: 0.2.1
 Author: Laughing-q
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 # lqcv
 This is my computer vision lib.
```

### Comparing `lqcv-0.2.0/lqcv.egg-info/SOURCES.txt` & `lqcv-0.2.1/lqcv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/setup.py` & `lqcv-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/test/test_area.py` & `lqcv-0.2.1/test/test_area.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/test/test_converter.py` & `lqcv-0.2.1/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `lqcv-0.2.0/test/test_reader.py` & `lqcv-0.2.1/test/test_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lqcv.data import ReadVideosAndImages, ReadOneStream
+from lqcv.data import ReadVideosAndImages, Stream, Images, Videos
 from lqcv.utils.plot import waitKey
 import cv2
 
 def test_img_video(source):
     reader = ReadVideosAndImages(source)
     # reader = ReadVideosAndImages(source, vid_stride=3)
     for img, p, s in reader:
@@ -10,16 +10,40 @@
             continue
         print(s)
         reader.save("sample", img)   # save to sample.jpg
         cv2.imshow('p', img)
         if cv2.waitKey(1) == ord('q'):
             break
 
+def test_img(source):
+    reader = Images(source)
+    # reader = ReadVideosAndImages(source, vid_stride=3)
+    for img, p, s in reader:
+        if img is None:
+            continue
+        print(s)
+        reader.save("sample", img)   # save to sample.jpg
+        cv2.imshow('p', img)
+        if cv2.waitKey(1) == ord('q'):
+            break
+
+def test_video(source):
+    reader = Videos(source)
+    # reader = ReadVideosAndImages(source, vid_stride=3)
+    for img, p, s in reader:
+        if img is None:
+            continue
+        print(s)
+        reader.save("sample", img)   # save to sample.jpg
+        cv2.imshow('p', img)
+        if cv2.waitKey(1) == ord('q'):
+            break
+
 def test_stream(source):
-    reader = ReadOneStream(source, vid_stride=3)
+    reader = Stream(source, vid_stride=3)
     for img, p, _ in reader:
         reader.save("sample", img)   # save to sample.jpg
         cv2.imshow('p', img)
         if cv2.waitKey(1) == ord('q'):
             break
 
 def test_img_video2(source):
@@ -28,15 +52,15 @@
         if img is None:
             continue
         cv2.imshow('p', img)
         if waitKey(1) == ord('q'):
             break
 
 def test_stream2(source):
-    reader = ReadOneStream(source, imgsz=(640, 640), im_only=True)
+    reader = Stream(source, imgsz=(640, 640), im_only=True)
     for img in reader:
         if img is None:
             continue
         cv2.imshow('p', img)
         if waitKey(1) == ord('q'):
             break
 
@@ -44,9 +68,12 @@
 if __name__ == "__main__":
     # test_img_video("lqcv/assets/")
     # test_img_video("lqcv/assets/bus.jpg")
     # test_img_video("/home/laughing/Videos/test.mp4")
     # test_stream("rtsp://admin:allcam123@172.16.11.133:554/Steaming/Channels/101")
     # test_img_video("/d/dataset/长沙/videos/advertise_0104/佳欣小学保家村委会门口（四期）_南_20230104141959_001.mp4")
 
-    test_img_video2("/home/laughing/Videos/test.mp4")
+    # test_img_video2("/home/laughing/Videos/test.mp4")
     # test_stream2("rtsp://admin:allcam123@172.16.11.133:554/Steaming/Channels/101")
+
+    # test_img("lqcv/assets")
+    test_video("/home/laughing/Videos/test.mp4")
```

