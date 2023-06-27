# Comparing `tmp/torchhandy-0.0.0.tar.gz` & `tmp/torchhandy-0.0.1.tar.gz`

## Comparing `torchhandy-0.0.0.tar` & `torchhandy-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 torchhandy-0.0.0/.pypirc
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 torchhandy-0.0.0/torchhandy/Block.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 torchhandy-0.0.0/torchhandy/Conv.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 torchhandy-0.0.0/torchhandy/FC.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchhandy-0.0.0/torchhandy/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 torchhandy-0.0.0/torchhandy/utils.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 torchhandy-0.0.0/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 torchhandy-0.0.0/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 torchhandy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 torchhandy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 torchhandy-0.0.1/.pypirc
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 torchhandy-0.0.1/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 torchhandy-0.0.1/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 torchhandy-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 torchhandy-0.0.1/torchhandy/Block.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 torchhandy-0.0.1/torchhandy/Conv.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 torchhandy-0.0.1/torchhandy/FC.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 torchhandy-0.0.1/torchhandy/utils.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 torchhandy-0.0.1/PKG-INFO
```

### Comparing `torchhandy-0.0.0/torchhandy/Block.py` & `torchhandy-0.0.1/torchhandy/Block.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.0/torchhandy/Conv.py` & `torchhandy-0.0.1/torchhandy/Conv.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             output = self.act(output)
         return output
     
 '''
     This is a conv module with self-attention layers.
 '''
 class Att_Conv(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size, num_heads, dropout,
+    def __init__(self, in_channels, out_channels, kernel_size, siz, num_heads, dropout,
                 normalization = None, activation = 'relu', res_connection = True):
         nn.Module.__init__(self)
         
-        self.conv1 = Res_Conv(in_channels, out_channels, kernel_size, 
+        self.conv1 = SConv(in_channels, out_channels, kernel_size, 
                            normalization, activation, res_connection)
-        self.conv2 = Res_Conv(out_channels, out_channels, kernel_size, 
+        self.conv2 = SConv(out_channels, out_channels, kernel_size, 
                            normalization, activation, res_connection)
-        self.norm = select_normalization(normalization)
+        self.norm = nn.LayerNorm((siz * siz, out_channels))
         self.att = nn.MultiheadAttention(out_channels, num_heads, dropout, batch_first = True)
         
     def forward(self, x):
         fea = self.conv1(x)
         a_fea = cha2fea(fea)
         att_out, _ = self.att(a_fea, a_fea, a_fea)
-        att_out = fea2cha(att_out)
-        fea = fea + att_out
+        fea = a_fea + att_out
         if self.norm:
             fea = self.norm(fea)
+        fea = fea2cha(fea)
         return self.conv2(fea)
```

### Comparing `torchhandy-0.0.0/torchhandy/FC.py` & `torchhandy-0.0.1/torchhandy/FC.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.0/torchhandy/utils.py` & `torchhandy-0.0.1/torchhandy/utils.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.0/LICENSE` & `torchhandy-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.0/pyproject.toml` & `torchhandy-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 746f 7263 6868 616e 6479 220d 0a76   "torchhandy"..v
-00000070: 6572 7369 6f6e 203d 2022 302e 302e 3022  ersion = "0.0.0"
+00000070: 6572 7369 6f6e 203d 2022 302e 302e 3122  ersion = "0.0.1"
 00000080: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
 00000090: 207b 206e 616d 653d 22e5 bca0 e88d 9fe8   { name=".......
 000000a0: 90b1 222c 2065 6d61 696c 3d22 706b 756c  ..", email="pkul
 000000b0: 656f 7a68 616e 6740 676d 6169 6c2e 636f  eozhang@gmail.co
 000000c0: 6d22 7d2c 0d0a 5d0d 0a0d 0a64 6573 6372  m"},..]....descr
 000000d0: 6970 7469 6f6e 203d 2022 746f 7263 6868  iption = "torchh
 000000e0: 616e 6479 2069 7320 6120 6861 6e64 7920  andy is a handy
```

### Comparing `torchhandy-0.0.0/PKG-INFO` & `torchhandy-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchhandy
-Version: 0.0.0
+Version: 0.0.1
 Summary: torchhandy is a handy package that implements some commonly used modules and function.
 Project-URL: Homepage, https://github.com/NickYi1990/juans
 Author-email: 张荟萱 <pkuleozhang@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Huixuan Zhang]
         
@@ -21,15 +21,14 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: torch>=1.6.0
 Description-Content-Type: text/markdown
```

