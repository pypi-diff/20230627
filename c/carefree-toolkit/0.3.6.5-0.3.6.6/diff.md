# Comparing `tmp/carefree-toolkit-0.3.6.5.tar.gz` & `tmp/carefree-toolkit-0.3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-toolkit-0.3.6.5.tar", last modified: Sat Jun 17 13:29:45 2023, max compression
+gzip compressed data, was "carefree-toolkit-0.3.6.6.tar", last modified: Tue Jun 27 15:22:14 2023, max compression
```

## Comparing `carefree-toolkit-0.3.6.5.tar` & `carefree-toolkit-0.3.6.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/
--rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/LICENSE
--rw-rw-rw-   0        0        0     9010 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.246160 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/
--rw-rw-rw-   0        0        0     9010 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.251636 carefree-toolkit-0.3.6.5/cftool/
--rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/__init__.py
--rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.6.5/cftool/array.py
--rw-rw-rw-   0        0        0       58 2023-05-17 12:47:47.000000 carefree-toolkit-0.3.6.5/cftool/constants.py
--rw-rw-rw-   0        0        0     8445 2023-03-28 02:09:18.000000 carefree-toolkit-0.3.6.5/cftool/cv.py
--rw-rw-rw-   0        0        0    17747 2023-06-17 08:20:53.000000 carefree-toolkit-0.3.6.5/cftool/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.251636 carefree-toolkit-0.3.6.5/cftool/dist/
--rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.6.5/cftool/dist/__init__.py
--rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/dist/core.py
--rw-rw-rw-   0        0        0     9983 2023-05-31 06:56:25.000000 carefree-toolkit-0.3.6.5/cftool/geometry.py
--rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/manage.py
--rw-rw-rw-   0        0        0    85225 2023-06-17 13:29:03.000000 carefree-toolkit-0.3.6.5/cftool/misc.py
--rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.6.5/cftool/pipeline.py
--rw-rw-rw-   0        0        0     1004 2023-03-28 02:09:02.000000 carefree-toolkit-0.3.6.5/cftool/types.py
--rw-rw-rw-   0        0        0     2237 2023-05-17 12:54:11.000000 carefree-toolkit-0.3.6.5/cftool/web.py
--rw-rw-rw-   0        0        0       42 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-06-17 13:29:43.000000 carefree-toolkit-0.3.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.398146 carefree-toolkit-0.3.6.6/
+-rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/LICENSE
+-rw-rw-rw-   0        0        0     9010 2023-06-27 15:22:14.397149 carefree-toolkit-0.3.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.388178 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     9010 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.395155 carefree-toolkit-0.3.6.6/cftool/
+-rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/__init__.py
+-rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.6.6/cftool/array.py
+-rw-rw-rw-   0        0        0       58 2023-05-17 12:47:47.000000 carefree-toolkit-0.3.6.6/cftool/constants.py
+-rw-rw-rw-   0        0        0    10833 2023-06-27 13:19:40.000000 carefree-toolkit-0.3.6.6/cftool/cv.py
+-rw-rw-rw-   0        0        0    17757 2023-06-27 12:49:06.000000 carefree-toolkit-0.3.6.6/cftool/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.396189 carefree-toolkit-0.3.6.6/cftool/dist/
+-rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.6.6/cftool/dist/__init__.py
+-rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/dist/core.py
+-rw-rw-rw-   0        0        0     9983 2023-05-31 06:56:25.000000 carefree-toolkit-0.3.6.6/cftool/geometry.py
+-rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/manage.py
+-rw-rw-rw-   0        0        0    85225 2023-06-17 13:29:03.000000 carefree-toolkit-0.3.6.6/cftool/misc.py
+-rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.6.6/cftool/pipeline.py
+-rw-rw-rw-   0        0        0     1085 2023-06-27 13:01:32.000000 carefree-toolkit-0.3.6.6/cftool/types.py
+-rw-rw-rw-   0        0        0     2237 2023-05-17 12:54:11.000000 carefree-toolkit-0.3.6.6/cftool/web.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:22:14.398146 carefree-toolkit-0.3.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      905 2023-06-27 15:21:39.000000 carefree-toolkit-0.3.6.6/setup.py
```

### Comparing `carefree-toolkit-0.3.6.5/LICENSE` & `carefree-toolkit-0.3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/PKG-INFO` & `carefree-toolkit-0.3.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.5
+Version: 0.3.6.6
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.5.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.6.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.5/README.md` & `carefree-toolkit-0.3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/PKG-INFO` & `carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.5
+Version: 0.3.6.6
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.5.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.6.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.5/cftool/array.py` & `carefree-toolkit-0.3.6.6/cftool/array.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/cv.py` & `carefree-toolkit-0.3.6.6/cftool/cv.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from typing import Any
 from typing import Dict
 from typing import Type
 from typing import Tuple
 from typing import Union
 from typing import Optional
 from typing import NamedTuple
+from dataclasses import dataclass
 
 from .misc import safe_execute
 from .misc import shallow_copy_dict
 from .misc import WithRegister
-from .array import torch
 from .array import to_torch
-from .types import arr_type
+from .types import torch
 from .types import torchvision
+from .types import arr_type
+from .types import TNumberPair
 
 try:
     from PIL import Image
 
     TImage = Image.Image
 except:
     Image = None
@@ -153,14 +155,97 @@
     if isinstance(arr, np.ndarray):
         arr = to_torch(arr)
     if n_row is None:
         n_row = math.ceil(math.sqrt(len(arr)))
     torchvision.utils.save_image(arr, path, normalize=True, nrow=n_row)
 
 
+@dataclass
+class ImageBox:
+    l: int
+    t: int
+    r: int
+    b: int
+
+    @property
+    def tuple(self) -> Tuple[int, int, int, int]:
+        return self.l, self.t, self.r, self.b
+
+    def copy(self) -> "ImageBox":
+        return ImageBox(*self.tuple)
+
+    def crop(self, image: ndarray) -> ndarray:
+        return image[self.t : self.b, self.l : self.r]
+
+    def crop_tensor(self, image: torch.Tensor) -> torch.Tensor:
+        return image[..., self.t : self.b, self.l : self.r]
+
+    def pad(
+        self,
+        padding: int,
+        *,
+        w: Optional[int] = None,
+        h: Optional[int] = None,
+    ) -> "ImageBox":
+        l, t, r, b = self.tuple
+        l = max(0, l - padding)
+        r += padding
+        if w is not None:
+            r = min(r, w)
+        t = max(0, t - padding)
+        b += padding
+        if h is not None:
+            b = min(b, h)
+        return ImageBox(l, t, r, b)
+
+    def to_square(
+        self,
+        *,
+        w: Optional[int] = None,
+        h: Optional[int] = None,
+        expand: bool = True,
+    ) -> "ImageBox":
+        l, t, r, b = self.tuple
+        bw, bh = r - l, b - t
+        diff = abs(bw - bh)
+        if diff == 0:
+            return self.copy()
+        if expand:
+            if bw > bh:
+                t = max(0, t - diff // 2)
+                b = t + bw
+                if h is not None:
+                    b = min(b, h)
+            else:
+                l = max(0, l - diff // 2)
+                r = l + bh
+                if w is not None:
+                    r = min(r, w)
+        else:
+            if bw > bh:
+                l += diff // 2
+                r = l + bh
+                if w is not None:
+                    r = min(r, w)
+            else:
+                t += diff // 2
+                b = t + bw
+                if h is not None:
+                    b = min(b, h)
+        return ImageBox(l, t, r, b)
+
+    @classmethod
+    def from_mask(cls, uint8_mask: ndarray, threshold: Optional[int]) -> "ImageBox":
+        ys, xs = np.where(uint8_mask > (threshold or 0))
+        ys, xs = np.where(uint8_mask)
+        if len(ys) == 0:
+            return cls(0, 0, 0, 0)
+        return cls(xs.min().item(), ys.min().item(), xs.max().item(), ys.max().item())
+
+
 class ImageProcessor:
     @staticmethod
     def _calculate_cdf(histogram: ndarray) -> ndarray:
         cdf = histogram.cumsum()
         normalized_cdf = cdf / float(cdf.max())
         return normalized_cdf
```

### Comparing `carefree-toolkit-0.3.6.5/cftool/data_structures.py` & `carefree-toolkit-0.3.6.6/cftool/data_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             f"'{earliest_key}' is unloaded to make room for '{key}' "
             f"(last updated: {time.strftime(time_format, time.localtime(loadable_item.load_time))})"
         )
         return item
 
 
 class InjectionPack(BaseModel):
-    index: int
+    index: Optional[int]
     field: str
 
 
 class WorkNode(BaseModel):
     key: str = Field(
         ...,
         description="Key of the node, should be identical within the same workflow",
```

### Comparing `carefree-toolkit-0.3.6.5/cftool/dist/core.py` & `carefree-toolkit-0.3.6.6/cftool/dist/core.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/geometry.py` & `carefree-toolkit-0.3.6.6/cftool/geometry.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/manage.py` & `carefree-toolkit-0.3.6.6/cftool/manage.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/misc.py` & `carefree-toolkit-0.3.6.6/cftool/misc.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/pipeline.py` & `carefree-toolkit-0.3.6.6/cftool/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/cftool/types.py` & `carefree-toolkit-0.3.6.6/cftool/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import Tuple
 from typing import Union
 from typing import Callable
 from typing import Optional
 from typing import NamedTuple
 
 try:
     import torch
@@ -33,7 +34,9 @@
 
 general_config_type = Optional[Union[str, Dict[str, Any]]]
 configs_type = Optional[Union[List[Dict[str, Any]], Dict[str, Any]]]
 
 arr_type = Union[np.ndarray, torch.Tensor]
 np_dict_type = Dict[str, Union[np.ndarray, Any]]
 tensor_dict_type = Dict[str, Union[torch.Tensor, Any]]
+
+TNumberPair = Optional[Union[int, Tuple[int, int]]]
```

### Comparing `carefree-toolkit-0.3.6.5/cftool/web.py` & `carefree-toolkit-0.3.6.6/cftool/web.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.5/setup.py` & `carefree-toolkit-0.3.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.3.6.5"
+VERSION = "0.3.6.6"
 
 DESCRIPTION = "Some commonly used functions and modules"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 INSTALL_REQUIRES = [
     "dill",
```

