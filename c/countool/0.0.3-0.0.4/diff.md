# Comparing `tmp/countool-0.0.3.tar.gz` & `tmp/countool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\countool-0.0.3.tar", last modified: Sun Jun 25 13:31:39 2023, max compression
+gzip compressed data, was "dist\countool-0.0.4.tar", last modified: Tue Jun 27 13:56:31 2023, max compression
```

## Comparing `countool-0.0.3.tar` & `countool-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 13:31:39.000000 countool-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-25 13:31:38.000000 countool-0.0.3/countool/
--rw-rw-rw-   0        0        0     3498 2023-06-25 13:31:15.000000 countool-0.0.3/countool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/requires.txt
--rw-rw-rw-   0        0        0      210 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 13:31:38.000000 countool-0.0.3/countool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2388 2023-06-25 13:31:39.000000 countool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 13:31:39.000000 countool-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-06-25 13:31:36.000000 countool-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:56:31.000000 countool-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:56:31.000000 countool-0.0.4/countool/
+-rw-rw-rw-   0        0        0     4270 2023-06-27 13:55:16.000000 countool-0.0.4/countool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      210 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 13:56:31.000000 countool-0.0.4/countool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 countool-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2388 2023-06-27 13:56:31.000000 countool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-04-24 08:07:32.000000 countool-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:56:31.000000 countool-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-06-27 13:10:10.000000 countool-0.0.4/setup.py
```

### Comparing `countool-0.0.3/countool/__init__.py` & `countool-0.0.4/countool/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,63 +31,75 @@
                 os.makedirs(p)
                 print({p}, 'is created for saving the results.')
     else:
         if not os.path.exists(path):
             os.makedirs(path)
             print({path}, 'is created for saving the results.')
 
-def calpipe(model: nn.Module,
-                input_shape: tuple,
-                output_path: str,
+def calpipe(
+                onnx_path: str,
+                output_path: str = None,
+                use_model: nn.Module = None,
+                use_onnx_sim: bool = True,
                 use_onnx_tool: bool = True,
-                use_opcounter: bool = True,
+                use_opcounter: bool = False,
                 use_netron: bool = False,
                 sufix:str = '.txt'):
 
-    assert isinstance(model, nn.Module), 'model must be a nn.Module'
+    assert isinstance(use_model, nn.Module), 'model must be a nn.Module'
     assert isinstance(input_shape, tuple), 'input_data must be a torch.tensor'
+    assert isinstance(onnx_path, str), 'onnx_path must be a str'
     assert isinstance(output_path, str), 'output_path must be a str'
     assert isinstance(use_onnx_tool, bool), 'use_onnx_tool must be a bool'
+    assert isinstance(use_opcounter, bool), 'use_opcounter must be a bool'
+    assert isinstance(use_netron, bool), 'use_netron must be a bool'
+    assert isinstance(sufix, str), 'sufix must be a str'
+
     if sufix not in ['.txt', '.csv']:
         raise ValueError('sufix must be txt or csv')
 
-    # mkfolder(output_path)
-    # print(output_path)
-    input_data = torch.randn(input_shape)
-    model.eval()
+    # input_data = torch.randn(input_shape)
+    # model.eval()
 
-    if use_opcounter:
-        flops, params = profile(model, inputs=(input_data, ))
+    if use_opcounter and use_model is not None:
+        input_data = torch.randn(1, 3, 512, 512)
+        print('use opcounter to profile model...')
+        flops, params = profile(use_model, inputs=(input_data, ))
         flops, params = clever_format([flops, params], "%.3f")
-        print("1.torch_Model profile...")
         print(f'Macs: {flops}, Params: {params}')
 
     if use_onnx_tool:
-        with torch.no_grad():
-            torch.onnx.export(
-                model,
-                input_data,
-                output_path,
-                opset_version=11,
-                input_names=['input'],
-                output_names=['output'])
+        if use_onnx_sim:
+            onnx_sim_path = onnx_path[:-5] + '_sim.onnx'
+            sim_onnx, check = simplify(onnx.load(onnx_path))
+            assert check, 'Simplified ONNX model could not be validated'
+            onnx.save(sim_onnx, onnx_sim_path)
+            onnx_tool.model_profile(onnx_sim_path)
+            print('use onnx_sim to simply..')
+        # with torch.no_grad():
+        #     torch.onnx.export(
+        #         model,
+        #         input_data,
+        #         output_path,
+        #         opset_version=11,
+        #         input_names=['input'],
+        #         output_names=['output'])
         # onnx_model = onnx.load(output_path)
         # try:
         #     onnx.checker.check_model(onnx_model)
         # except Exception:
         #     print("×××, Model incorrect, please debug")
         # else:
-            print("2.onnx_Model correct...")
-            print('3.use onnx_tool to profile model...')
-            modelpath = output_path
-            onnx_tool.model_profile(modelpath)  # pass file name
-            onnx_tool.model_profile(modelpath, savenode=f'{output_path[:-5]}' + sufix)  # save profile table to txt file
+        #     print("2.onnx_Model correct...")
+        print('use onnx_tool to profile model...')
+        onnx_tool.model_profile(onnx_path)  # pass file name
+        onnx_tool.model_profile(onnx_path, savenode=f'{output_path[:-5]}' + sufix)  # save profile table to txt file
     if use_netron:
         print('4.use netron to visualize model...')
-        netron.start(output_path)
+        netron.start(onnx_sim_path) if use_onnx_sim else netron.start(onnx_path)
 
 
 
 # if __name__ == "__main__":
 #     from pth2onnx import ControlNetHED_Apache2
 #     model = ControlNetHED_Apache2()
 #     model.eval()
```

### Comparing `countool-0.0.3/countool.egg-info/PKG-INFO` & `countool-0.0.4/countool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.3/LICENSE.txt` & `countool-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countool-0.0.3/PKG-INFO` & `countool-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package of calculator for params/macs 
 Home-page: https://github.com/HuiiJi
 Author: Huii Ji
 Author-email: 752413464@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countool-0.0.3/README.md` & `countool-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `countool-0.0.3/setup.py` & `countool-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="countool",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.3",  # 包版本号，便于pip维护版本
+    version="0.0.4",  # 包版本号，便于pip维护版本
     author="Huii Ji",  # 作者，可以写自己的姓名
     author_email="752413464@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package of calculator for params/macs ",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuiiJi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

