# Comparing `tmp/bitalign-0.3.0.tar.gz` & `tmp/bitalign-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitalign-0.3.0.tar", last modified: Fri Jun 23 23:16:04 2023, max compression
+gzip compressed data, was "bitalign-0.4.0.tar", last modified: Tue Jun 27 08:30:42 2023, max compression
```

## Comparing `bitalign-0.3.0.tar` & `bitalign-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:16:04.250836 bitalign-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 23:15:55.000000 bitalign-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 23:15:55.000000 bitalign-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-23 23:16:04.250836 bitalign-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-23 23:15:55.000000 bitalign-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:16:04.250836 bitalign-0.3.0/bitalign/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-23 23:15:55.000000 bitalign-0.3.0/bitalign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-23 23:15:55.000000 bitalign-0.3.0/bitalign/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:16:04.250836 bitalign-0.3.0/bitalign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-23 23:16:04.000000 bitalign-0.3.0/bitalign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 23:16:04.000000 bitalign-0.3.0/bitalign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:16:04.000000 bitalign-0.3.0/bitalign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 23:16:04.000000 bitalign-0.3.0/bitalign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-23 23:15:55.000000 bitalign-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:16:04.250836 bitalign-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-23 23:15:55.000000 bitalign-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:16:04.250836 bitalign-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-23 23:15:55.000000 bitalign-0.3.0/src/_bitalign.c
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 23:15:55.000000 bitalign-0.3.0/src/_bitalign.h
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-23 23:15:55.000000 bitalign-0.3.0/src/_bitalign_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-23 23:15:55.000000 bitalign-0.3.0/src/_bitalignmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-23 23:15:55.000000 bitalign-0.3.0/src/_popcount_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:42.831952 bitalign-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 08:30:33.000000 bitalign-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 08:30:33.000000 bitalign-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-27 08:30:42.831952 bitalign-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-27 08:30:33.000000 bitalign-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:42.831952 bitalign-0.4.0/bitalign/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-27 08:30:33.000000 bitalign-0.4.0/bitalign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-27 08:30:33.000000 bitalign-0.4.0/bitalign/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-27 08:30:33.000000 bitalign-0.4.0/bitalign/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:42.831952 bitalign-0.4.0/bitalign.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-27 08:30:42.000000 bitalign-0.4.0/bitalign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 08:30:42.000000 bitalign-0.4.0/bitalign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:30:42.000000 bitalign-0.4.0/bitalign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 08:30:42.000000 bitalign-0.4.0/bitalign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 08:30:33.000000 bitalign-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:30:42.831952 bitalign-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-27 08:30:33.000000 bitalign-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:42.831952 bitalign-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-27 08:30:33.000000 bitalign-0.4.0/src/_bitalign.c
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-27 08:30:33.000000 bitalign-0.4.0/src/_bitalign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-27 08:30:33.000000 bitalign-0.4.0/src/_bitalign_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-27 08:30:33.000000 bitalign-0.4.0/src/_bitalignmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 08:30:33.000000 bitalign-0.4.0/src/_popcount_impl.h
```

### Comparing `bitalign-0.3.0/LICENSE` & `bitalign-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitalign-0.3.0/PKG-INFO` & `bitalign-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitalign
-Version: 0.3.0
+Version: 0.4.0
 Summary: Shift some bits and see how they line up best.
 Home-page: https://github.com/sweeneyde/bitalign
 Author: Dennis Sweeney
 Author-email: Dennis Sweeney <sweeney.427@osu.edu>
 Project-URL: Homepage, https://github.com/sweeneyde/bitalign
 Project-URL: Bug Tracker, https://github.com/sweeneyde/bitalign
 Classifier: Programming Language :: Python :: 3
@@ -85,15 +85,15 @@
     bitalign_16_msb,
     bitalign_32_msb,
     bitalign_64_msb,
 )
 ```
 
 ```
-    bitalign_#_???(arr1, arr2) --> (shift_by, num_common_bits);
+    bitalign_#_?sb(arr1, arr2) --> (shift_by, num_common_bits);
 
     Return a tuple (x, y) such that when arr1 is shifted by x bits,
     the number of bits in common between arr1 and arr2 is y.
 
     Positive shifts indicate that arr1 needs to be shifted toward the back:
 
         arr1 =                    -->  0001001011111111  -->
@@ -108,8 +108,10 @@
 
     The number (8, 16, 32, or 64) in the function name the number of bits
     that must be in each array entry.  'lsb'/'msb' indicates whether the
     0th bit of each logical bit-array is to be stored in the least or most
     significant bit of arr[0].
 
     If more than one shift is optimal, the negative-most shift is used.
+    If there are no bits in common (i.e., all zeros with all ones),
+    then (-num_bits, 0) is returned.
 ```
```

### Comparing `bitalign-0.3.0/README.md` & `bitalign-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     bitalign_16_msb,
     bitalign_32_msb,
     bitalign_64_msb,
 )
 ```
 
 ```
-    bitalign_#_???(arr1, arr2) --> (shift_by, num_common_bits);
+    bitalign_#_?sb(arr1, arr2) --> (shift_by, num_common_bits);
 
     Return a tuple (x, y) such that when arr1 is shifted by x bits,
     the number of bits in common between arr1 and arr2 is y.
 
     Positive shifts indicate that arr1 needs to be shifted toward the back:
 
         arr1 =                    -->  0001001011111111  -->
@@ -92,8 +92,10 @@
 
     The number (8, 16, 32, or 64) in the function name the number of bits
     that must be in each array entry.  'lsb'/'msb' indicates whether the
     0th bit of each logical bit-array is to be stored in the least or most
     significant bit of arr[0].
 
     If more than one shift is optimal, the negative-most shift is used.
+    If there are no bits in common (i.e., all zeros with all ones),
+    then (-num_bits, 0) is returned.
 ```
```

### Comparing `bitalign-0.3.0/bitalign/tests.py` & `bitalign-0.4.0/bitalign/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def test_basic_8_msb(self):
         (x, y) = bitalign_8_msb(bytes([0b1111_1111, 0b1111_1111]),
                                 bytes([0b1111_1111, 0b1111_1111]))
         self.assertEqual((x, y), (0, 16))
 
         (x, y) = bitalign_8_msb(bytes([0b1111_1111, 0b1111_1111]),
                                 bytes([0b0000_0000, 0b0000_0000]))
-        self.assertEqual((x, y), (-15, 0))
+        self.assertEqual((x, y), (-16, 0))
 
         (x, y) = bitalign_8_msb(bytes([0b1111_0000, 0b0000_0000]),
                                 bytes([0b0000_1111, 0b0000_0000]))
         self.assertEqual((x, y), (4, 12))
 
         (x, y) = bitalign_8_msb(bytes([0b0000_1111, 0b0000_0000]),
                                 bytes([0b0000_0000, 0b1111_0000]))
@@ -52,40 +52,40 @@
     def test_basic_16_msb(self):
         (x, y) = bitalign_16_msb(array.array('H', [0]),
                                  array.array('H', [0]) )
         self.assertEqual((x, y), (0, 16))
 
         (x, y) = bitalign_16_msb(array.array('H', [0xffff, 0xffff]),
                                  array.array('H', [0x0000, 0x0000]))
-        self.assertEqual((x, y), (-31, 0))
+        self.assertEqual((x, y), (-32, 0))
 
         (x, y) = bitalign_16_msb(array.array('H', [0xffff, 0x0000]),
                                  array.array('H', [0x0000, 0xffff]))
         self.assertEqual((x, y), (-16, 16))
 
     def reference_algorithm(self, A, B):
         N = len(A)
         self.assertEqual(len(B), N)
         self.assertNotEqual(N, 0)
         shift_by, common_bits = None, -1
-        for a_start in reversed(range(N)):
+        for a_start in reversed(range(N+1)):
             c = sum(map(operator.eq, A[a_start:], B))
             if c > common_bits:
                 shift_by, common_bits = -a_start, c
         for b_start in range(1, N):
             c = sum(map(operator.eq, A, B[b_start:]))
             if c > common_bits:
                 shift_by, common_bits = b_start, c
         return (shift_by, common_bits)
 
     def test_reference_algorithm(self):
         # Same test cases as above.
         r = self.reference_algorithm
         self.assertEqual(r("1111111111111111", "1111111111111111"), (0, 16))
-        self.assertEqual(r("1111111111111111", "0000000000000000"), (-15, 0))
+        self.assertEqual(r("1111111111111111", "0000000000000000"), (-16, 0))
         self.assertEqual(r("1111000000000000", "0000111100000000"), (4, 12))
         self.assertEqual(r("1001001000100101", "0110001001111100"), (-4, 10))
         self.assertEqual(r("11011110", "10110100"), (-1, 6))
         self.assertEqual(r("00000110", "01100111"), (0, 5))
 
         # From docstring
         self.assertEqual(r("0001001011111111", "1111100010010111"), (5, 11))
```

### Comparing `bitalign-0.3.0/bitalign.egg-info/PKG-INFO` & `bitalign-0.4.0/bitalign.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitalign
-Version: 0.3.0
+Version: 0.4.0
 Summary: Shift some bits and see how they line up best.
 Home-page: https://github.com/sweeneyde/bitalign
 Author: Dennis Sweeney
 Author-email: Dennis Sweeney <sweeney.427@osu.edu>
 Project-URL: Homepage, https://github.com/sweeneyde/bitalign
 Project-URL: Bug Tracker, https://github.com/sweeneyde/bitalign
 Classifier: Programming Language :: Python :: 3
@@ -85,15 +85,15 @@
     bitalign_16_msb,
     bitalign_32_msb,
     bitalign_64_msb,
 )
 ```
 
 ```
-    bitalign_#_???(arr1, arr2) --> (shift_by, num_common_bits);
+    bitalign_#_?sb(arr1, arr2) --> (shift_by, num_common_bits);
 
     Return a tuple (x, y) such that when arr1 is shifted by x bits,
     the number of bits in common between arr1 and arr2 is y.
 
     Positive shifts indicate that arr1 needs to be shifted toward the back:
 
         arr1 =                    -->  0001001011111111  -->
@@ -108,8 +108,10 @@
 
     The number (8, 16, 32, or 64) in the function name the number of bits
     that must be in each array entry.  'lsb'/'msb' indicates whether the
     0th bit of each logical bit-array is to be stored in the least or most
     significant bit of arr[0].
 
     If more than one shift is optimal, the negative-most shift is used.
+    If there are no bits in common (i.e., all zeros with all ones),
+    then (-num_bits, 0) is returned.
 ```
```

### Comparing `bitalign-0.3.0/pyproject.toml` & `bitalign-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.cibuildwheel]
 test-command = "python -m bitalign.tests"
 
 [project]
 name = "bitalign"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Dennis Sweeney", email="sweeney.427@osu.edu" },
 ]
 description = "Shift some bits and see how they line up best."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `bitalign-0.3.0/src/_bitalign.c` & `bitalign-0.4.0/src/_bitalign.c`

 * *Files 22% similar despite different names*

```diff
@@ -7,116 +7,116 @@
 #include "./_bitalign.h"
 #include "./_popcount_impl.h"
 
 // LSB Stored first --------------------------------------------------
 
 #define SHIFT_FORWARD(w, i) ((w) << (i))
 #define LAST_BIT_AND_SHIFTED_REST(prev, rest) \
-    (((prev) >> (WORD_BIT - 1)) | (rest << 1))
+    (((prev) >> (BA_WORD_BIT - 1)) | (rest << 1))
 
 #define MANGLE(name)   name##_8lsb
-#define WORD           uint8_t
-#define WORD_BIT       8
+#define BA_WORD           uint8_t
+#define BA_WORD_BIT       8
 #define POPCNT(x)      popcount8(x)
-#define WORD_MAX       UINT8_MAX
+#define BA_WORD_MAX       UINT8_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_16lsb
-#define WORD           uint16_t
-#define WORD_BIT       16
+#define BA_WORD           uint16_t
+#define BA_WORD_BIT       16
 #define POPCNT(x)      popcount16(x)
-#define WORD_MAX       UINT16_MAX
+#define BA_WORD_MAX       UINT16_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_32lsb
-#define WORD           uint32_t
-#define WORD_BIT       32
+#define BA_WORD           uint32_t
+#define BA_WORD_BIT       32
 #define POPCNT(x)      popcount32(x)
-#define WORD_MAX       UINT32_MAX
+#define BA_WORD_MAX       UINT32_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_64lsb
-#define WORD           uint64_t
-#define WORD_BIT       64
+#define BA_WORD           uint64_t
+#define BA_WORD_BIT       64
 #define POPCNT(x)      popcount64(x)
-#define WORD_MAX       UINT64_MAX
+#define BA_WORD_MAX       UINT64_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #undef SHIFT_FORWARD
 #undef LAST_BIT_AND_SHIFTED_REST
 
 // MSB Stored first --------------------------------------------------
 
 #define SHIFT_FORWARD(w, i) ((w) >> (i))
 #define LAST_BIT_AND_SHIFTED_REST(prev, rest) \
-    (((prev) << (WORD_BIT - 1)) | (rest >> 1))
+    (((prev) << (BA_WORD_BIT - 1)) | (rest >> 1))
 
 #define MANGLE(name)   name##_8msb
-#define WORD           uint8_t
-#define WORD_BIT       8
+#define BA_WORD           uint8_t
+#define BA_WORD_BIT       8
 #define POPCNT(x)      popcount8(x)
-#define WORD_MAX       UINT8_MAX
+#define BA_WORD_MAX       UINT8_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_16msb
-#define WORD           uint16_t
-#define WORD_BIT       16
+#define BA_WORD           uint16_t
+#define BA_WORD_BIT       16
 #define POPCNT(x)      popcount16(x)
-#define WORD_MAX       UINT16_MAX
+#define BA_WORD_MAX       UINT16_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_32msb
-#define WORD           uint32_t
-#define WORD_BIT       32
+#define BA_WORD           uint32_t
+#define BA_WORD_BIT       32
 #define POPCNT(x)      popcount32(x)
-#define WORD_MAX       UINT32_MAX
+#define BA_WORD_MAX       UINT32_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #define MANGLE(name)   name##_64msb
-#define WORD           uint64_t
-#define WORD_BIT       64
+#define BA_WORD           uint64_t
+#define BA_WORD_BIT       64
 #define POPCNT(x)      popcount64(x)
-#define WORD_MAX       UINT64_MAX
+#define BA_WORD_MAX       UINT64_MAX
 #include "./_bitalign_impl.h"
 #undef MANGLE
-#undef WORD
-#undef WORD_BIT
+#undef BA_WORD
+#undef BA_WORD_BIT
 #undef POPCNT
-#undef WORD_MAX
+#undef BA_WORD_MAX
 
 #undef SHIFT_FORWARD
 #undef LAST_BIT_AND_SHIFTED_REST
```

### Comparing `bitalign-0.3.0/src/_bitalignmodule.c` & `bitalign-0.4.0/src/_bitalignmodule.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,15 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include "./_bitalign.h"
 
-typedef struct {
-    void *freeblock;
-    size_t size;
-} bitalign_module_state;
-
-
-static void *
-allocate_buffer(bitalign_module_state *state, size_t size)
-{
-    void *block = state->freeblock;
-    if (block != NULL && state->size == size) {
-        state->freeblock = NULL;
-        return block;
-    }
-    return PyMem_Malloc(size);
-}
-
-static void
-free_buffer(bitalign_module_state *state, void *block, size_t size)
-{
-    assert(block != NULL);
-    void *oldblock = state->freeblock;
-    state->freeblock = block;
-    state->size = size;
-    if (oldblock) {
-        PyMem_Free(oldblock);
-    }
-}
-
-static int
-bitalign_clear(PyObject *module)
-{
-    bitalign_module_state *state = PyModule_GetState(module);
-    assert(state != NULL);
-    void *block = state->freeblock;
-    if (block) {
-        state->freeblock = NULL;
-        PyMem_Free(block);
-    }
-    return 0;
-}
-
-typedef struct bitalign_result (*implfunc)(void *, void *, int, void *);
-
 static PyObject *
 bitalign_helper(PyObject *self, PyObject *const *args, Py_ssize_t nargs,
                 int itemsize, implfunc func)
 {
-    bitalign_module_state *state = PyModule_GetState(self);
-    assert(state != NULL);
     if (nargs != 2) {
         PyErr_SetString(PyExc_TypeError,
                         "bitalign_#_xxx expected 2 arguments.");
         return NULL;
     }
     Py_buffer a, b;
     if (PyObject_GetBuffer(args[0], &a, PyBUF_ND) < 0) {
@@ -82,26 +36,25 @@
     if (msg) {
         PyBuffer_Release(&a);
         PyBuffer_Release(&b);
         PyErr_SetString(PyExc_ValueError, msg);
         return NULL;
     }
     int N = (int)(a.len / itemsize);
-    void *buffer = allocate_buffer(state, (N + 1) * itemsize);
+    void *buffer = PyMem_Malloc((N + 1) * itemsize);
     if (buffer == NULL) {
         PyBuffer_Release(&a);
         PyBuffer_Release(&b);
         return PyErr_NoMemory();
     }
     struct bitalign_result res = func(a.buf, b.buf, N, buffer);
     PyBuffer_Release(&a);
     PyBuffer_Release(&b);
-    free_buffer(state, buffer, N + 1);
+    PyMem_Free(buffer);
     return Py_BuildValue("(ii)", res.shift_by, res.common_bits);
-
 }
 
 static PyObject *
 bitalign_8_lsb(PyObject *self, PyObject *const *args, Py_ssize_t nargs)
 {
     return bitalign_helper(self, args, nargs,
                            sizeof(uint8_t), bitalign_impl_8lsb);
@@ -152,22 +105,16 @@
 static PyObject *
 bitalign_64_msb(PyObject *self, PyObject *const *args, Py_ssize_t nargs)
 {
     return bitalign_helper(self, args, nargs,
                            sizeof(uint64_t), bitalign_impl_64msb);
 }
 
-static void
-bitalign_free(void *module)
-{
-    (void)bitalign_clear((PyObject *)module);
-}
-
 PyDoc_STRVAR(bitalign_doc,"\
-bitalign_#_???(arr1, arr2) --> (shift_by, num_common_bits);\n\
+bitalign_#_?sb(arr1, arr2) --> (shift_by, num_common_bits);\n\
 \n\
 Return a tuple (x, y) such that when arr1 is shifted by x bits,\n\
 the number of bits in common between arr1 and arr2 is y.\n\
 \n\
 Positive shifts indicate that arr1 needs to be shifted toward the back:\n\
 \n\
     arr1 =                    -->  0001001011111111  -->\n\
@@ -181,39 +128,35 @@
     gives (shift_by=-5, num_common_bits=11)\n\
 \n\
 The number (8, 16, 32, or 64) in the function name the number of bits\n\
 that must be in each array entry.  'lsb'/'msb' indicates whether the\n\
 0th bit of each logical bit-array is to be stored in the least or most\n\
 significant bit of arr[0].\n\
 \n\
-If more than one shift is optimal, the negative-most shift is used.\
+If more than one shift is optimal, the negative-most shift is used.\n\
+If there are no bits in common (i.e., all zeros with all ones),\n\
+then (-num_bits, 0) is returned.\
 ");
 
 static PyMethodDef bitalign_methods[] = {
     {"bitalign_8_lsb",  (PyCFunction)bitalign_8_lsb,  METH_FASTCALL, bitalign_doc},
     {"bitalign_16_lsb", (PyCFunction)bitalign_16_lsb, METH_FASTCALL, bitalign_doc},
     {"bitalign_32_lsb", (PyCFunction)bitalign_32_lsb, METH_FASTCALL, bitalign_doc},
     {"bitalign_64_lsb", (PyCFunction)bitalign_64_lsb, METH_FASTCALL, bitalign_doc},
     {"bitalign_8_msb",  (PyCFunction)bitalign_8_msb,  METH_FASTCALL, bitalign_doc},
     {"bitalign_16_msb", (PyCFunction)bitalign_16_msb, METH_FASTCALL, bitalign_doc},
     {"bitalign_32_msb", (PyCFunction)bitalign_32_msb, METH_FASTCALL, bitalign_doc},
     {"bitalign_64_msb", (PyCFunction)bitalign_64_msb, METH_FASTCALL, bitalign_doc},
     {NULL, NULL}
 };
 
-PyDoc_STRVAR(module_doc, "some kind of module");
-
 static struct PyModuleDef _bitalignmodule = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "bitalign",
-    .m_doc = module_doc,
-    .m_size = sizeof(bitalign_module_state),
+    .m_name = "_bitalign",
     .m_methods = bitalign_methods,
-    .m_clear = bitalign_clear,
-    .m_free = bitalign_free,
 };
 
 PyMODINIT_FUNC
 PyInit__bitalign(void)
 {
     return PyModuleDef_Init(&_bitalignmodule);
 }
```

### Comparing `bitalign-0.3.0/src/_popcount_impl.h` & `bitalign-0.4.0/src/_popcount_impl.h`

 * *Files identical despite different names*

