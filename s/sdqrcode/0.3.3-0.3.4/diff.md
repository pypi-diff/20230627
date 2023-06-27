# Comparing `tmp/sdqrcode-0.3.3.tar.gz` & `tmp/sdqrcode-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.3.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.4.tar", max compression
```

## Comparing `sdqrcode-0.3.3.tar` & `sdqrcode-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-06-26 20:10:18.146164 sdqrcode-0.3.3/LICENSE
--rw-r--r--   0        0        0     9268 2023-06-26 20:10:18.146164 sdqrcode-0.3.3/README.md
--rw-r--r--   0        0        0      495 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     7900 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      719 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      777 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    12834 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    10101 1970-01-01 00:00:00.000000 sdqrcode-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-27 13:35:26.136620 sdqrcode-0.3.4/LICENSE
+-rw-r--r--   0        0        0    10370 2023-06-27 13:35:26.136620 sdqrcode-0.3.4/README.md
+-rw-r--r--   0        0        0      495 2023-06-27 13:35:26.188620 sdqrcode-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-06-27 13:35:26.188620 sdqrcode-0.3.4/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     7900 2023-06-27 13:35:26.188620 sdqrcode-0.3.4/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-27 13:35:26.188620 sdqrcode-0.3.4/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-27 13:35:26.188620 sdqrcode-0.3.4/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      719 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    12834 2023-06-27 13:35:26.192620 sdqrcode-0.3.4/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    11203 1970-01-01 00:00:00.000000 sdqrcode-0.3.4/PKG-INFO
```

### Comparing `sdqrcode-0.3.3/LICENSE` & `sdqrcode-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/README.md` & `sdqrcode-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # Stable Diffusion QR Code
 alpha version, expect breaking changes
 
-call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770) is released
 
 # tldr
 
 ```python
 import sdqrcode
 sd_qr_images, generator = sdqrcode.init_and_generate_sd_qrcode(config="default_diffusers")
 ```
@@ -18,15 +18,27 @@
 
 # Updates
 - **June 25:** The diffusers version has been added to the package
 - **June 23:** a colab with a pure diffusers version without automatic1111 dependencie is now available. It will be added to the package soon
 
 # Motivation
 There is multiple methodes availables to generate ai qr code with differents controlnets models and params. Some parameters might works better with some stable diffusion checkpoints and it's a pain to find somethings that works consistanly.
-This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file 
+This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file
+
+# How it works
+The idea is to use controlnet to guide the generation: 
+- an image is generated  based on the prompt for a few steps
+- controlnet is activated for some steps to add the qrcode on the generating image
+- controlnet is deactivated to blend the qrcode and the image
+
+With this method, small modifications of the ``weight``, ``start`` and ``end`` parameters can have huge impacts on the generation.
+
+
+ 
+
 
 # Exemple
 click to expand, cherry picked, will add more results later
 
 | ![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323) | ![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305) |
 | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
 
@@ -193,14 +205,26 @@
 ## default
 This method seem to be the best for me, I use it with the model [realistic_visionV2](https://civitai.com/models/4201/realistic-vision-v20).
 It uses [Controlnet Brightness](https://huggingface.co/ioclab/control_v1p_sd15_brightness) and [Controlnet Tile](https://huggingface.co/lllyasviel/control_v11f1e_sd15_tile)
 Here are my firsts thoughts:
 * CN brightness should be left as is
 * You can play with CN tile parameters to get an image more or less "grid like"
 
+# Controlnet models
+There are multiple controlnet models that can be used:
+- [Controlnet Tile](https://huggingface.co/ControlNet-1-1-preview/control_v11f1e_sd15_tile): This CN takes an image as input and guide the generation toward this image and to increase the details. We can use a qr code as input.
+- Controlnet Brightness: 
+  - https://huggingface.co/ioclab/control_v1p_sd15_brightness
+  - https://huggingface.co/ViscoseBean/control_v1p_sd15_brightness
+- Controlnet QR code
+  - https://huggingface.co/DionTimmer/controlnet_qrcode-control_v1p_sd15
+  - https://huggingface.co/DionTimmer/controlnet_qrcode-control_v11p_sd21
+  - https://huggingface.co/models?search=qrcode
+
+
 # Todos
 - [ ] add img2img for diffusers 
 - [x] allow to set the sampler (diffusers)
 - [ ] allow to set the seed (diffusers)
 - [ ] allow to set the model in the config (auto)
 - [ ] add more configs
 - [x] allow to set the config without having the file in local path
```

### Comparing `sdqrcode-0.3.3/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.4/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.4/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
             )
         
         if self.config["global"]["mode"] == "img2img":
             self.pipeline = StableDiffusionControlNetImg2ImgPipeline.from_pretrained(
                 self.config["global"]["model_name_or_path"],
                 controlnet=self.controlnet_units,
             )
-        self.pipeline = self.pipeline.to("cuda")
         self.pipeline.enable_xformers_memory_efficient_attention()
+        self.pipeline = self.pipeline.to("cuda")
 
 
     def generate_sd_qrcode(
         self,
         input_image: PIL.Image.Image = None,
         controlnet_input_images: PIL.Image.Image = None,
     ) -> list[PIL.Image.Image]:
```

### Comparing `sdqrcode-0.3.3/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.4/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.4/src/sdqrcode/configs/default_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.4/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.4/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_diffusers.yaml` & `sdqrcode-0.3.4/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.4/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.3/PKG-INFO` & `sdqrcode-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Requires-Dist: xformers (>=0.0.20,<0.0.21)
 Description-Content-Type: text/markdown
 
 
 # Stable Diffusion QR Code
 alpha version, expect breaking changes
 
-call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
+call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770) is released
 
 # tldr
 
 ```python
 import sdqrcode
 sd_qr_images, generator = sdqrcode.init_and_generate_sd_qrcode(config="default_diffusers")
 ```
@@ -40,15 +40,27 @@
 
 # Updates
 - **June 25:** The diffusers version has been added to the package
 - **June 23:** a colab with a pure diffusers version without automatic1111 dependencie is now available. It will be added to the package soon
 
 # Motivation
 There is multiple methodes availables to generate ai qr code with differents controlnets models and params. Some parameters might works better with some stable diffusion checkpoints and it's a pain to find somethings that works consistanly.
-This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file 
+This repo aims to easily try and evaluate differents methods, models, params and share them with a simple config file
+
+# How it works
+The idea is to use controlnet to guide the generation: 
+- an image is generated  based on the prompt for a few steps
+- controlnet is activated for some steps to add the qrcode on the generating image
+- controlnet is deactivated to blend the qrcode and the image
+
+With this method, small modifications of the ``weight``, ``start`` and ``end`` parameters can have huge impacts on the generation.
+
+
+ 
+
 
 # Exemple
 click to expand, cherry picked, will add more results later
 
 | ![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323) | ![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305) |
 | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
 
@@ -215,14 +227,26 @@
 ## default
 This method seem to be the best for me, I use it with the model [realistic_visionV2](https://civitai.com/models/4201/realistic-vision-v20).
 It uses [Controlnet Brightness](https://huggingface.co/ioclab/control_v1p_sd15_brightness) and [Controlnet Tile](https://huggingface.co/lllyasviel/control_v11f1e_sd15_tile)
 Here are my firsts thoughts:
 * CN brightness should be left as is
 * You can play with CN tile parameters to get an image more or less "grid like"
 
+# Controlnet models
+There are multiple controlnet models that can be used:
+- [Controlnet Tile](https://huggingface.co/ControlNet-1-1-preview/control_v11f1e_sd15_tile): This CN takes an image as input and guide the generation toward this image and to increase the details. We can use a qr code as input.
+- Controlnet Brightness: 
+  - https://huggingface.co/ioclab/control_v1p_sd15_brightness
+  - https://huggingface.co/ViscoseBean/control_v1p_sd15_brightness
+- Controlnet QR code
+  - https://huggingface.co/DionTimmer/controlnet_qrcode-control_v1p_sd15
+  - https://huggingface.co/DionTimmer/controlnet_qrcode-control_v11p_sd21
+  - https://huggingface.co/models?search=qrcode
+
+
 # Todos
 - [ ] add img2img for diffusers 
 - [x] allow to set the sampler (diffusers)
 - [ ] allow to set the seed (diffusers)
 - [ ] allow to set the model in the config (auto)
 - [ ] add more configs
 - [x] allow to set the config without having the file in local path
```

