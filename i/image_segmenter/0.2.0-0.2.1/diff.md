# Comparing `tmp/image_segmenter-0.2.0.tar.gz` & `tmp/image_segmenter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_segmenter-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "image_segmenter-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `image_segmenter-0.2.0.tar` & `image_segmenter-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.2.0/LICENSE
--rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.2.0/README.md
--rw-r--r--   0        0        0      104 2023-06-27 18:30:42.025604 image_segmenter-0.2.0/image_segmenter/__init__.py
--rw-r--r--   0        0        0    10020 2023-06-27 18:29:21.725604 image_segmenter-0.2.0/image_segmenter/image_segmenter.py
--rw-r--r--   0        0        0     6343 2023-06-27 18:29:25.975604 image_segmenter-0.2.0/image_segmenter/voc_writer.py
--rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.2.0/requirements.txt
--rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 image_segmenter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-06-27 17:46:52.551846 image_segmenter-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-27 17:49:01.418964 image_segmenter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2450 2023-06-27 17:18:02.552909 image_segmenter-0.2.1/README.md
+-rw-r--r--   0        0        0      104 2023-06-27 18:43:15.715605 image_segmenter-0.2.1/image_segmenter/__init__.py
+-rw-r--r--   0        0        0    10209 2023-06-27 18:43:05.385604 image_segmenter-0.2.1/image_segmenter/image_segmenter.py
+-rw-r--r--   0        0        0     6343 2023-06-27 18:29:25.975604 image_segmenter-0.2.1/image_segmenter/voc_writer.py
+-rw-r--r--   0        0        0      613 2023-06-27 17:50:24.835137 image_segmenter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-09 00:01:47.107516 image_segmenter-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 image_segmenter-0.2.1/PKG-INFO
```

### Comparing `image_segmenter-0.2.0/.gitignore` & `image_segmenter-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.2.0/LICENSE` & `image_segmenter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.2.0/README.md` & `image_segmenter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.2.0/image_segmenter/image_segmenter.py` & `image_segmenter-0.2.1/image_segmenter/image_segmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,20 @@
             img (np.array): The image in BGR format.
             colorsp (str): The color space to return. Options are 'gray', 'red', 'green', 'blue', 'hue', 'sat', 'val'.
 
         Returns:
             channels[colorsp] (np.array): The selected color space.
         """
         # Convert to grayscale.
-        gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        if img.ndim == 3:
+            gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        elif img.ndim == 1:
+            gray = img
+        else:
+            raise ValueError(f'Image must be 1 or 3 channels. Got {img.ndim} channels.')
         # Split BGR.
         red, green, blue = cv2.split(img)
         # Convert to HSV.
         im_hsv = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
         # Split HSV.
         hue, sat, val = cv2.split(im_hsv)
         # Store channels in a dict.
```

### Comparing `image_segmenter-0.2.0/image_segmenter/voc_writer.py` & `image_segmenter-0.2.1/image_segmenter/voc_writer.py`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.2.0/pyproject.toml` & `image_segmenter-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_segmenter-0.2.0/PKG-INFO` & `image_segmenter-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_segmenter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Image Segmenter
 Author-email: Rich Baird <rich@rbaird.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/richbai90/image_segmenter.git
 Project-URL: Repository, https://github.com/richbai90/image_segmenter.git
```

