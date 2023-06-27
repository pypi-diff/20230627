# Comparing `tmp/webcam-1.4.tar.gz` & `tmp/webcam-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.4.tar", last modified: Fri Jun 23 12:39:54 2023, max compression
+gzip compressed data, was "webcam-1.5.tar", last modified: Tue Jun 27 11:42:40 2023, max compression
```

## Comparing `webcam-1.4.tar` & `webcam-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.080841 webcam-1.4/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.4/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-06-23 12:39:54.079793 webcam-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 12:39:54.081807 webcam-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-06-23 12:39:51.000000 webcam-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.057762 webcam-1.4/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.4/webcam/__init__.py
--rw-rw-rw-   0        0        0    10127 2023-06-23 12:36:27.000000 webcam-1.4/webcam/_perspective_manager.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.4/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.4/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    18641 2023-06-23 12:38:38.000000 webcam-1.4/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.078558 webcam-1.4/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:42:40.465687 webcam-1.5/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.5/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-27 11:42:40.464687 webcam-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:42:40.465687 webcam-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-27 11:42:34.000000 webcam-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:42:40.431361 webcam-1.5/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.5/webcam/__init__.py
+-rw-rw-rw-   0        0        0    12272 2023-06-27 11:38:18.000000 webcam-1.5/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.5/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.5/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    20189 2023-06-27 11:29:06.000000 webcam-1.5/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:42:40.462678 webcam-1.5/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-27 11:42:40.000000 webcam-1.5/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-27 11:42:40.000000 webcam-1.5/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:42:40.000000 webcam-1.5/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-27 11:42:40.000000 webcam-1.5/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 11:42:40.000000 webcam-1.5/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.4/LICENSE` & `webcam-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.4/PKG-INFO` & `webcam-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.4
+Version: 1.5
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.4/README.md` & `webcam-1.5/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.4/setup.py` & `webcam-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.4',
+    version='1.5',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.4/webcam/_perspective_manager.py` & `webcam-1.5/webcam/_perspective_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Author: Eric Canas
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 20-06-2023
 """
 from __future__ import annotations
-from functools import lru_cache, cache
+from functools import lru_cache
 import cv2
 import numpy as np
 
 
 class _PerspectiveManager:
     def __init__(self, homography_matrix: np.ndarray|list[list[float], ...], default_w: int, default_h: int,
                  crop_boundaries: bool = False,
@@ -171,21 +171,47 @@
         vec_y_transformed /= vec_y_transformed[2]
 
         # Compute the lengths of the transformed vectors
         length_transformed_x = np.linalg.norm(vec_x_transformed[:, -1] - vec_x_transformed[:, 0])
         length_transformed_y = np.linalg.norm(vec_y_transformed[:, -1] - vec_y_transformed[:, 0])
 
         # The magnification in x and y directions is the ratio of transformed length to original length
-        homography_magnification_w = length_transformed_x / (vec_x[0, -1] - vec_x[0, 0])
-        homography_magnification_h = length_transformed_y / (vec_y[1, -1] - vec_y[1, 0])
+        homography_magnification_w = length_transformed_x / (vec_x[0, -1] - vec_x[0, 0]) if (vec_x[0, -1] - vec_x[
+            0, 0]) != 0 else 1.0
+        homography_magnification_h = length_transformed_y / (vec_y[1, -1] - vec_y[1, 0]) if (vec_y[1, -1] - vec_y[
+            1, 0]) != 0 else 1.0
 
         return homography_magnification_w, homography_magnification_h
 
-class _DummyPerspectiveManager:
-    def __init__(self, *args, **kwargs):
-        pass
+    def get_hw_magnification_for_line(self, xyxy_line: np.ndarray | tuple[int | float, int | float, int | float, int | float]) \
+            -> tuple[float, float]:
+        """
+        Get the magnification factor for the given line. It is calculated by transforming the two endpoints of the line
+        and calculating the ratio between the length of the transformed line and the original one.
+        :param xyxy_line: np.ndarray or tuple[int|float, int|float, int|float, int|float]. The line to which the magnification
+        factor must be calculated. It can be either a tuple with the coordinates of the two endpoints of the line or a
+        numpy array with shape (2, 2) containing the coordinates of the two endpoints of the line.
+        :return: tuple[float, float]. The magnification factor for the given line. In the form (h_magnification, w_magnification).
+        """
+        assert self.homography_matrix is not None, "Homography matrix must be set before calling this method."
+        assert self.homography_matrix.shape == (
+        3, 3), f"Homography matrix must be a 3x3 matrix. Got {'x'.join(map(str, self.homography_matrix.shape))}"
 
-    def after_warp_image_shape(self, w: int, h: int) -> tuple[int, int]:
-        return w, h
+        if isinstance(xyxy_line, tuple):
+            assert len(xyxy_line) == 4, f"Expected tuple of length 4, but got length {len(xyxy_line)}."
+            xyxy_line = np.array(xyxy_line, dtype=np.float32)
+        assert isinstance(xyxy_line, np.ndarray), "Line must be either a tuple or a numpy array."
+        xyxy_line = xyxy_line.reshape(2, 2)
+
+        # Transform the line using homography matrix
+        line_transformed = np.dot(self.homography_matrix, np.c_[xyxy_line, np.ones(2)].T)
+        line_transformed /= line_transformed[2]
+
+        # Calculate the lengths in x and y directions separately for the original and transformed lines
+        dx_original, dy_original = np.abs(xyxy_line[1] - xyxy_line[0])
+        dx_transformed, dy_transformed = np.abs(np.diff(line_transformed[:2], axis=1).squeeze())
+
+        # Calculate the magnification in x and y directions separately
+        magnification_w = dx_transformed / dx_original if dx_original != 0 else 1.0
+        magnification_h = dy_transformed / dy_original if dy_original != 0 else 1.0
 
-    def warp(self, image: np.ndarray) -> np.ndarray:
-        return image
+        return magnification_w, magnification_h
```

### Comparing `webcam-1.4/webcam/_video_webcam.py` & `webcam-1.5/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.4/webcam/_webcam_background.py` & `webcam-1.5/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.4/webcam/webcam.py` & `webcam-1.5/webcam/webcam.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import time
 from typing import Tuple
 
 import os
 
 from webcam._video_webcam import _VideoWebcam
 from webcam._webcam_background import _WebcamBackground
-from webcam._perspective_manager import _PerspectiveManager, _DummyPerspectiveManager
+from webcam._perspective_manager import _PerspectiveManager
 
 CROP, RESIZE = 'crop', 'resize'
 
 class Webcam:
     def __init__(
         self,
         src: int | str = 0,
@@ -314,28 +314,14 @@
 
     def release(self):
         self.cap.release()
 
     def isOpened(self):
         return self.cap.isOpened()
 
-    @lru_cache(maxsize=8)
-    def _get_pixel_magnification_one_axis(self, length:int, axis: str) -> float:
-        """
-        Calculate the pixel magnification factor for one axis (height or width) of the frame.
-        Pixel magnification factor is the ratio between the length of the axis in the original video and the length
-        of the axis in the output frame.
-
-        :param length: int. The length of the axis (height or width) of the frame.
-        :param axis: str. The axis to calculate the pixel magnification factor for.
-        Valid values are 'h' and 'w'.
-
-        :return: float. The pixel magnification factor for the given axis.
-        """
-        assert axis in ('h', 'w'), f"Invalid value for 'axis' parameter: {axis}. Valid values are 'h' and 'w'."
 
     @lru_cache(maxsize=64)
     def get_magnification_hw(self, x: int | float | None = None, y: int | float | None = None) -> float:
         """
         Calculate the magnification of the pixel at (x, y). If x and y are not given, the magnification of the
         center pixel is calculated. (x, y) coordinates are only relevant if the perspective is adjusted.
 
@@ -353,31 +339,44 @@
             input_h, input_w = self.perspective_manager.output_h, self.perspective_manager.output_w
         # Or use the default magnification
         else:
             magnification_h, magnification_w = 1.0, 1.0
             input_h, input_w = self._h, self._w
 
         # Calculate the pixel magnification for each axis when adjusting size
-        if self.on_aspect_ratio_lost == RESIZE:
-            magnification_h *= self.h / input_h
-            magnification_w *= self.w / input_w
+        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h, input_w, magnification_h,
+                                                                                      magnification_w)
 
-        elif self.on_aspect_ratio_lost == CROP:
-            resize_ratio = self.h / input_h if input_h < input_w else self.w / input_w
-            magnification_h *= resize_ratio
-            magnification_w *= resize_ratio
+        # Return the magnification of the pixel at (x, y)
+        return magnification_h, magnification_w
+
+    def get_line_hw_magnification(self, line_xyxy: np.ndarray | tuple[int|float, int|float, int|float, int|float]) \
+            -> tuple[float, float]:
+        """
+        Get the magnification factor for the given line. It allows to take precise measurements on the image, without
+        having to worry about the perspective distortion, aspect ratio modifications or resizing.
+        :param line_xyxy: tuple. The line to measure, in the format (x1, y1, x2, y2).
+        :return: tuple. The magnification factor for the line.
+        """
+        # Calculate the homography magnification if appliable
+        if self.perspective_manager is not None:
+            magnification_h, magnification_w = self.perspective_manager.get_hw_magnification_for_line(xyxy_line=line_xyxy)
+            input_h, input_w = self.perspective_manager.output_h, self.perspective_manager.output_w
+        # Or use the default magnification
         else:
-            raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}."
-                             f" Valid values are '{RESIZE}' and '{CROP}'.")
+            magnification_h, magnification_w = 1.0, 1.0
+            input_h, input_w = self._h, self._w
 
+        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h, input_w, magnification_h,
+                                                                                      magnification_w)
 
-        # Return the magnification of the pixel at (x, y)
         return magnification_h, magnification_w
 
 
+
     # --------------- AUXILIARY METHODS ---------------
     def calculate_frame_size_keeping_aspect_ratio(self, h:int | None, w:int|None) -> tuple[int, int]:
         """
         When only one of the frame size dimensions is given, the other one is calculated keeping the
         aspect ratio with the original video.
 
         :param h: int or None. Height of the frame. If None, _w must be provided.
@@ -391,14 +390,39 @@
             w = int(round(self._w * h / self._h))
         else:
             raise ValueError(f'Only one of the frame size dimensions must be provided.'
                              f' Got _h={h} and _w={w}.')
         assert h is not None and w is not None, f'Both _h and _w should have been calculated. Got _h={h} and _w={w}.'
         return h, w
 
+    @lru_cache(maxsize=64)
+    def __calculate_resizing_magnification_hw(self, input_h: int, input_w: int, pre_magnification_h: float = 1.0,
+                                              pre_magnification_w: float = 1.0) -> tuple[float, float]:
+        """
+        Calculate the pixel magnification for each axis when adjusting size
+        :param input_h: int. The input height.
+        :param input_w: int. The input width.
+        :param pre_magnification_h: float. The previous magnification in height. Default is 1.0.
+        :param pre_magnification_w: float. The previous magnification in width. Default is 1.0.
+        :return: tuple[float, float]. The updated magnification in height and width.
+        """
+        if self.on_aspect_ratio_lost == RESIZE:
+            pre_magnification_h *= self.h / input_h
+            pre_magnification_w *= self.w / input_w
+
+        elif self.on_aspect_ratio_lost == CROP:
+            resize_ratio = self.h / input_h if input_h < input_w else self.w / input_w
+            pre_magnification_h *= resize_ratio
+            pre_magnification_w *= resize_ratio
+        else:
+            raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}."
+                             f" Valid values are '{RESIZE}' and '{CROP}'.")
+
+        return pre_magnification_h, pre_magnification_w
+
     def __iter__(self):
         return self
 
     def __next__(self):
         return self.read_next_frame()
 
     def __del__(self):
```

### Comparing `webcam-1.4/webcam.egg-info/PKG-INFO` & `webcam-1.5/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.4
+Version: 1.5
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

