# Comparing `tmp/pic2square2icon-0.10.tar.gz` & `tmp/pic2square2icon-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pic2square2icon-0.10.tar", last modified: Tue Jun 27 03:49:28 2023, max compression
+gzip compressed data, was "pic2square2icon-0.11.tar", last modified: Tue Jun 27 04:26:49 2023, max compression
```

## Comparing `pic2square2icon-0.10.tar` & `pic2square2icon-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 03:49:28.311542 pic2square2icon-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-27 03:49:18.000000 pic2square2icon-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      116 2023-06-27 03:49:15.000000 pic2square2icon-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3694 2023-06-27 03:49:28.311542 pic2square2icon-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2966 2023-06-27 03:47:02.000000 pic2square2icon-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 03:49:28.307552 pic2square2icon-0.10/pic2square2icon/
--rw-rw-rw-   0        0        0     2966 2023-06-27 03:47:02.000000 pic2square2icon-0.10/pic2square2icon/README.MD
--rw-rw-rw-   0        0        0     5210 2023-06-27 03:32:38.000000 pic2square2icon-0.10/pic2square2icon/__init__.py
--rw-rw-rw-   0        0        0       52 2023-06-27 03:49:27.000000 pic2square2icon-0.10/pic2square2icon/requirements.txt
--rw-rw-rw-   0        0        0    60616 2023-06-27 03:49:27.000000 pic2square2icon-0.10/pic2square2icon/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-27 03:49:28.310544 pic2square2icon-0.10/pic2square2icon.egg-info/
--rw-rw-rw-   0        0        0     3694 2023-06-27 03:49:28.000000 pic2square2icon-0.10/pic2square2icon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-06-27 03:49:28.000000 pic2square2icon-0.10/pic2square2icon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 03:49:28.000000 pic2square2icon-0.10/pic2square2icon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-27 03:49:28.000000 pic2square2icon-0.10/pic2square2icon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 03:49:28.000000 pic2square2icon-0.10/pic2square2icon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-27 03:49:28.312539 pic2square2icon-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1489 2023-06-27 03:49:27.000000 pic2square2icon-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:26:49.678609 pic2square2icon-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-27 04:26:43.000000 pic2square2icon-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      116 2023-06-27 04:26:42.000000 pic2square2icon-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4040 2023-06-27 04:26:49.678609 pic2square2icon-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3312 2023-06-27 04:24:13.000000 pic2square2icon-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 04:26:49.676044 pic2square2icon-0.11/pic2square2icon/
+-rw-rw-rw-   0        0        0     3312 2023-06-27 04:24:13.000000 pic2square2icon-0.11/pic2square2icon/README.MD
+-rw-rw-rw-   0        0        0     5541 2023-06-27 04:22:14.000000 pic2square2icon-0.11/pic2square2icon/__init__.py
+-rw-rw-rw-   0        0        0       52 2023-06-27 04:26:48.000000 pic2square2icon-0.11/pic2square2icon/requirements.txt
+-rw-rw-rw-   0        0        0    60616 2023-06-27 04:26:48.000000 pic2square2icon-0.11/pic2square2icon/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-27 04:26:49.678609 pic2square2icon-0.11/pic2square2icon.egg-info/
+-rw-rw-rw-   0        0        0     4040 2023-06-27 04:26:49.000000 pic2square2icon-0.11/pic2square2icon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-06-27 04:26:49.000000 pic2square2icon-0.11/pic2square2icon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 04:26:49.000000 pic2square2icon-0.11/pic2square2icon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-27 04:26:49.000000 pic2square2icon-0.11/pic2square2icon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 04:26:49.000000 pic2square2icon-0.11/pic2square2icon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-27 04:26:49.679608 pic2square2icon-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2023-06-27 04:26:48.000000 pic2square2icon-0.11/setup.py
```

### Comparing `pic2square2icon-0.10/LICENSE.rst` & `pic2square2icon-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pic2square2icon-0.10/PKG-INFO` & `pic2square2icon-0.11/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pic2square2icon
-Version: 0.10
+Version: 0.11
 Summary: 2 functions that provide convenient and efficient ways to resize images to a square with custom backgrounds and convert images to the ICO format
 Home-page: https://github.com/hansalemaos/pic2square2icon
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ico,convert,posts
 Classifier: Development Status :: 4 - Beta
@@ -43,56 +43,65 @@
 
 ```python
 
 from pic2square2icon import resize_with_background, pic2ico
 import cv2
 
 test = 1
-fg = r"C:\testim\fg.png"
-bg = r"C:\testim\bg.png"
+fg = r"C:\test\fg.png"
+bg = r"C:\test\bg.png"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 
 test = 2
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = "orange"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 3
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = (255, 255, 0)
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 4
-fg = r"C:\testim\bg.png"
-bg = cv2.imread(r"C:\testim\fg.png")
+fg = r"C:\test\bg.png"
+bg = cv2.imread(r"C:\test\fg.png")
 target_size = 512
-resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
+
+test = 5
+fg = r"C:\test\fg.png"
+bg = None
+target_size = 512
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+resized_image.save(rf"C:\test\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+
 ```
 
 
 
-#### g.png
+#### bg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/bg.png?raw=true)
 
 
 
-#### g.png
+#### fg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/fg.png?raw=true)
 
 
 
 #### 1.png
 
@@ -111,7 +120,12 @@
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/3.png?raw=true)
 
 
 
 #### 4.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/4.png?raw=true)
+
+
+#### 5.png
+
+![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/5.png?raw=true)
```

### Comparing `pic2square2icon-0.10/README.md` & `pic2square2icon-0.11/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,56 +25,65 @@
 
 ```python
 
 from pic2square2icon import resize_with_background, pic2ico
 import cv2
 
 test = 1
-fg = r"C:\testim\fg.png"
-bg = r"C:\testim\bg.png"
+fg = r"C:\test\fg.png"
+bg = r"C:\test\bg.png"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 
 test = 2
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = "orange"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 3
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = (255, 255, 0)
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 4
-fg = r"C:\testim\bg.png"
-bg = cv2.imread(r"C:\testim\fg.png")
+fg = r"C:\test\bg.png"
+bg = cv2.imread(r"C:\test\fg.png")
 target_size = 512
-resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
+
+test = 5
+fg = r"C:\test\fg.png"
+bg = None
+target_size = 512
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+resized_image.save(rf"C:\test\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+
 ```
 
 
 
-#### g.png
+#### bg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/bg.png?raw=true)
 
 
 
-#### g.png
+#### fg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/fg.png?raw=true)
 
 
 
 #### 1.png
 
@@ -93,7 +102,12 @@
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/3.png?raw=true)
 
 
 
 #### 4.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/4.png?raw=true)
+
+
+#### 5.png
+
+![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/5.png?raw=true)
```

### Comparing `pic2square2icon-0.10/pic2square2icon/README.MD` & `pic2square2icon-0.11/pic2square2icon/README.MD`

 * *Files 10% similar despite different names*

```diff
@@ -25,56 +25,65 @@
 
 ```python
 
 from pic2square2icon import resize_with_background, pic2ico
 import cv2
 
 test = 1
-fg = r"C:\testim\fg.png"
-bg = r"C:\testim\bg.png"
+fg = r"C:\test\fg.png"
+bg = r"C:\test\bg.png"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 
 test = 2
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = "orange"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 3
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = (255, 255, 0)
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 4
-fg = r"C:\testim\bg.png"
-bg = cv2.imread(r"C:\testim\fg.png")
+fg = r"C:\test\bg.png"
+bg = cv2.imread(r"C:\test\fg.png")
 target_size = 512
-resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
+
+test = 5
+fg = r"C:\test\fg.png"
+bg = None
+target_size = 512
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+resized_image.save(rf"C:\test\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+
 ```
 
 
 
-#### g.png
+#### bg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/bg.png?raw=true)
 
 
 
-#### g.png
+#### fg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/fg.png?raw=true)
 
 
 
 #### 1.png
 
@@ -93,7 +102,12 @@
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/3.png?raw=true)
 
 
 
 #### 4.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/4.png?raw=true)
+
+
+#### 5.png
+
+![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/5.png?raw=true)
```

### Comparing `pic2square2icon-0.10/pic2square2icon/__init__.py` & `pic2square2icon-0.11/pic2square2icon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from PIL import Image
 from fabisschomagut import to_rgb_tuple
 from touchtouch import touch
 from ignoreexceptions import ignore_Exception
 from typing import Any
 
 
-def resize_with_background(image, target_size: int = 512, background=None) -> Image:
+def resize_with_background(
+    image, target_size: int = 512, background=None, background_ratio: int = 1
+) -> Image:
     """
     Resize an image to the specified target size with a background.
 
     Args:
         image (Image, np.array or str (file path)): The input image.
         target_size (int, optional): The target size for the resized image. Defaults to 512.
         background (None, Image, np.array, str (file path/hex color/color name), RGB tuple, optional): The background. Defaults to None (image is also used as background).
+        background_ratio (int): Zoom on background pic
 
     Returns:
         Image: The resized image with the background.
     """
     image = image2rgb(image)
     width, height = fit_pic_to_size(target_size, *image.size)
     resized_image = image.resize((width, height))
@@ -24,15 +27,17 @@
         if not background:
             background = image.copy()
     except ValueError:
         pass
     background_image = create_new_image_with_color(target_size, background)
     if not background_image:
         background_image = resize_image_at_least_size(background, target_size)
-        background_image = crop_image(background_image, (target_size, target_size))
+        background_image = crop_image(
+            background_image, (target_size, target_size), background_ratio
+        )
     x = (target_size - width) // 2
     y = (target_size - height) // 2
     background_image.paste(resized_image, (x, y))
     return background_image
 
 
 def pic2ico(src: Any, dst=None) -> str:
@@ -108,32 +113,36 @@
     Returns:
         Image: The new image with the specified background color.
     """
     background_color = to_rgb_tuple(color=background_color, invert=False)
     return Image.new("RGB", (target_size, target_size), background_color)
 
 
-def crop_image(image, crop_size: tuple | list) -> Image:
+def crop_image(image, crop_size: tuple | list, background_ratio: int = 1) -> Image:
     """
     Crop an image to the specified size.
 
     Args:
         image (Image, np.array or str (file path)): The input image.
         crop_size (tuple or list): The size of the cropped image.
+        background_ratio (int): Zoom on background pic
 
     Returns:
         Image: The cropped image.
     """
     image = image2rgb(image)
-    width, height = image.size
+    imagex = image.resize(
+        (image.size[0] * background_ratio, image.size[1] * background_ratio)
+    )
+    width, height = imagex.size
     x1 = (width - crop_size[0]) // 2
     y1 = (height - crop_size[1]) // 2
     x2 = x1 + crop_size[0]
     y2 = y1 + crop_size[1]
-    cropped_image = image.crop((x1, y1, x2, y2))
+    cropped_image = imagex.crop((x1, y1, x2, y2))
     return cropped_image
 
 
 def resize_image_at_least_size(image, target_size: int) -> Image:
     """
     Resize an image to at least the specified target size while maintaining the aspect ratio.
```

### Comparing `pic2square2icon-0.10/pic2square2icon/thirdparty.json` & `pic2square2icon-0.11/pic2square2icon/thirdparty.json`

 * *Files identical despite different names*

### Comparing `pic2square2icon-0.10/pic2square2icon.egg-info/PKG-INFO` & `pic2square2icon-0.11/pic2square2icon.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pic2square2icon
-Version: 0.10
+Version: 0.11
 Summary: 2 functions that provide convenient and efficient ways to resize images to a square with custom backgrounds and convert images to the ICO format
 Home-page: https://github.com/hansalemaos/pic2square2icon
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ico,convert,posts
 Classifier: Development Status :: 4 - Beta
@@ -43,56 +43,65 @@
 
 ```python
 
 from pic2square2icon import resize_with_background, pic2ico
 import cv2
 
 test = 1
-fg = r"C:\testim\fg.png"
-bg = r"C:\testim\bg.png"
+fg = r"C:\test\fg.png"
+bg = r"C:\test\bg.png"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 
 test = 2
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = "orange"
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 3
-fg = r"C:\testim\fg.png"
+fg = r"C:\test\fg.png"
 bg = (255, 255, 0)
 target_size = 512
 resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
 
 test = 4
-fg = r"C:\testim\bg.png"
-bg = cv2.imread(r"C:\testim\fg.png")
+fg = r"C:\test\bg.png"
+bg = cv2.imread(r"C:\test\fg.png")
 target_size = 512
-resized_image = resize_with_background(fg, target_size, bg)
-pic2ico(src=resized_image, dst=rf"C:\testim\{test}.ico")
-resized_image.save(rf"C:\testim\{test}.png")
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+resized_image.save(rf"C:\test\{test}.png")
+
+test = 5
+fg = r"C:\test\fg.png"
+bg = None
+target_size = 512
+resized_image = resize_with_background(fg, target_size, bg, background_ratio=2)
+resized_image.save(rf"C:\test\{test}.png")
+pic2ico(src=resized_image, dst=rf"C:\test\{test}.ico")
+
 ```
 
 
 
-#### g.png
+#### bg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/bg.png?raw=true)
 
 
 
-#### g.png
+#### fg.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/fg.png?raw=true)
 
 
 
 #### 1.png
 
@@ -111,7 +120,12 @@
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/3.png?raw=true)
 
 
 
 #### 4.png
 
 ![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/4.png?raw=true)
+
+
+#### 5.png
+
+![](https://github.com/hansalemaos/screenshots/blob/main/create_ico/5.png?raw=true)
```

### Comparing `pic2square2icon-0.10/setup.py` & `pic2square2icon-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''2 functions that provide convenient and efficient ways to resize images to a square with custom backgrounds and convert images to the ICO format'''
 
 # Setting up
 setup(
     name="pic2square2icon",
     version=VERSION,
     license='MIT',
```

