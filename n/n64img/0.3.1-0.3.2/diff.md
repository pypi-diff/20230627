# Comparing `tmp/n64img-0.3.1.tar.gz` & `tmp/n64img-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n64img-0.3.1.tar", last modified: Thu May  4 15:48:19 2023, max compression
+gzip compressed data, was "n64img-0.3.2.tar", last modified: Tue Jun 27 04:29:15 2023, max compression
```

## Comparing `n64img-0.3.1.tar` & `n64img-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 15:48:08.000000 n64img-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 15:48:19.910780 n64img-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 15:48:08.000000 n64img-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.906780 n64img-0.3.1/n64img/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/n64img.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 15:48:08.000000 n64img-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 15:48:19.910780 n64img-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:08.000000 n64img-0.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-04 15:48:08.000000 n64img-0.3.1/test/test_endian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 15:48:08.000000 n64img-0.3.1/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 04:29:07.000000 n64img-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 04:29:15.200862 n64img-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 04:29:07.000000 n64img-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/n64img/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/n64img.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 04:29:07.000000 n64img-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 04:29:15.200862 n64img-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:07.000000 n64img-0.3.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-27 04:29:07.000000 n64img-0.3.2/test/test_endian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-27 04:29:07.000000 n64img-0.3.2/test/test_image.py
```

### Comparing `n64img-0.3.1/LICENSE` & `n64img-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `n64img-0.3.1/n64img/image.py` & `n64img-0.3.2/n64img/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,52 +6,53 @@
 
 from n64img import iter
 
 Palette = List[Tuple[int, int, int, int]]
 
 
 class Image:
-    def __init__(self, data: bytes, width: int, height: int):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         self.data: bytes = data
         self.width: int = width
         self.height: int = height
         self.depth: float = 1
         self.greyscale: bool = False
         self.alpha: bool = False
         self.flip_h: bool = False
         self.flip_v: bool = False
         self.little_endian: bool = False
         self.palette: Optional[Palette] = None
 
-    def __str__(self):
-        return "Image(width={}, height={}, data={})".format(
+    def __str__(self) -> str:
+        return "Image(width={}, height={}, data={!r})".format(
             self.width, self.height, self.data
         )
 
     def set_palette(
         self, palette_bytes: bytes, endian: Literal["little", "big"] = "big"
     ) -> None:
-        def unpack_color(data):
-            s = int.from_bytes(data[0:2], endian)
+        def unpack_color(data: bytes) -> Tuple[int, int, int, int]:
+            s = int.from_bytes(data, endian)
 
             r = (s >> 11) & 0x1F
             g = (s >> 6) & 0x1F
             b = (s >> 1) & 0x1F
             a = (s & 1) * 0xFF
 
             r = ceil(0xFF * (r / 31))
             g = ceil(0xFF * (g / 31))
             b = ceil(0xFF * (b / 31))
 
             return r, g, b, a
 
         palette = []
 
-        for a, b in iter.iter_in_groups(palette_bytes, 2):
-            palette.append(unpack_color([a, b]))
+        assert len(palette_bytes) % 2 == 0
+        for i in range(0, len(palette_bytes), 2):
+            palette.append(unpack_color(palette_bytes[i : i + 2]))
 
         self.palette = palette
 
     def get_writer(self) -> png.Writer:
         return png.Writer(
             self.width,
             self.height,
@@ -63,21 +64,21 @@
     def parse(self) -> bytes:
         if not self.flip_h and not self.flip_v:
             return self.data
 
         img = bytearray()
 
         for x, y, i in iter.iter_image_indexes(
-            self.width, self.height, 1, self.flip_h, self.flip_v
+            self.width, self.height, self.depth, self.flip_h, self.flip_v
         ):
             img.append(self.data[i])
 
         return bytes(img)
 
-    def write(self, outpath: Path):
+    def write(self, outpath: Path) -> None:
         with open(outpath, "wb") as f:
             pixels = self.parse()
             self.get_writer().write_array(f, pixels)
 
     def mipmap_size(self) -> int:
         size = 0
         width = self.width
@@ -92,15 +93,15 @@
         return size
 
     def size(self) -> int:
         return ceil(self.width * self.height * self.depth)
 
 
 class CI4(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 0.5
 
     def parse(self) -> bytes:
         img = bytearray()
 
         if self.little_endian:
@@ -122,15 +123,15 @@
 class CI8(Image):
     pass
 
 
 # I1, a very primitive type where each bit represents one pixel.
 # Generally, only used for debug fonts and rendered using the cpu instead of the rdp.
 class I1(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 0.125
         self.greyscale = True
 
     def parse(self) -> bytes:
         if self.flip_h:
             raise Exception("I1 images cannot be flipped horizontally.")
@@ -149,15 +150,15 @@
 
                 img.append(p)
 
         return bytes(img)
 
 
 class I4(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 0.5
         self.greyscale = True
 
     def parse(self) -> bytes:
         img = bytearray()
 
@@ -188,21 +189,21 @@
 
                 img += bytes((i1, i2))
 
         return bytes(img)
 
 
 class I8(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.greyscale = True
 
 
 class IA4(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 0.5
         self.greyscale = True
         self.alpha = True
 
     def parse(self) -> bytes:
         img = bytearray()
@@ -229,15 +230,15 @@
 
             img += bytes((i1, a1, i2, a2))
 
         return bytes(img)
 
 
 class IA8(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.greyscale = True
         self.alpha = True
 
     def parse(self) -> bytes:
         img = bytearray()
 
@@ -254,23 +255,36 @@
 
             img += bytes((i, a))
 
         return bytes(img)
 
 
 class IA16(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 2
         self.greyscale = True
         self.alpha = True
 
+    def parse(self) -> bytes:
+        if not self.flip_h and not self.flip_v:
+            return self.data
+
+        img = bytearray()
+
+        for x, y, i in iter.iter_image_indexes(
+            self.width, self.height, self.depth, self.flip_h, self.flip_v
+        ):
+            img += bytes((self.data[i + 1], self.data[i]))
+
+        return bytes(img)
+
 
 class RGBA16(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 2
         self.greyscale = False
         self.alpha = True
 
     def parse(self) -> bytes:
         img = bytearray()
@@ -292,12 +306,27 @@
 
             img += bytes((r, g, b, a))
 
         return bytes(img)
 
 
 class RGBA32(Image):
-    def __init__(self, data, width, height):
+    def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
         self.depth = 4
         self.greyscale = False
         self.alpha = True
+
+    def parse(self) -> bytes:
+        if not self.flip_h and not self.flip_v:
+            return self.data
+
+        img = bytearray()
+
+        for x, y, i in iter.iter_image_indexes(
+            self.width, self.height, self.depth, self.flip_h, self.flip_v
+        ):
+            img += bytes(
+                (self.data[i], self.data[i + 1], self.data[i + 2], self.data[i + 3])
+            )
+
+        return bytes(img)
```

### Comparing `n64img-0.3.1/test/test_endian.py` & `n64img-0.3.2/test/test_endian.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.1/test/test_image.py` & `n64img-0.3.2/test/test_image.py`

 * *Files identical despite different names*

