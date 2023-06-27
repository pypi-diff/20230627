# Comparing `tmp/WIDscript-1.1.2.tar.gz` & `tmp/WIDscript-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WIDscript-1.1.2.tar", last modified: Sun Jun 25 22:29:11 2023, max compression
+gzip compressed data, was "WIDscript-1.2.0.tar", last modified: Tue Jun 27 21:20:56 2023, max compression
```

## Comparing `WIDscript-1.1.2.tar` & `WIDscript-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.666245 WIDscript-1.1.2/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      520 2023-06-25 22:29:11.666245 WIDscript-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.1.2/README.md
--rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      661 2023-06-25 22:29:11.668248 WIDscript-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.648248 WIDscript-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.653246 WIDscript-1.1.2/src/WIDscript/
--rw-rw-rw-   0        0        0    26393 2023-06-25 22:28:10.000000 WIDscript-1.1.2/src/WIDscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.665243 WIDscript-1.1.2/src/WIDscript.egg-info/
--rw-rw-rw-   0        0        0      520 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 21:20:56.367304 WIDscript-1.2.0/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-06-27 21:20:56.367304 WIDscript-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.2.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      661 2023-06-27 21:20:56.368809 WIDscript-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 21:20:56.339265 WIDscript-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 21:20:56.353788 WIDscript-1.2.0/src/WIDscript/
+-rw-rw-rw-   0        0        0     3512 2023-06-27 21:18:06.000000 WIDscript-1.2.0/src/WIDscript/WIDscript_dpir.py
+-rw-rw-rw-   0        0        0     3516 2023-06-27 21:17:58.000000 WIDscript-1.2.0/src/WIDscript/WIDscript_dpirNCNN.py
+-rw-rw-rw-   0        0        0    26342 2023-06-27 21:19:51.000000 WIDscript-1.2.0/src/WIDscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 21:20:56.366302 WIDscript-1.2.0/src/WIDscript.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-06-27 21:20:56.000000 WIDscript-1.2.0/src/WIDscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-27 21:20:56.000000 WIDscript-1.2.0/src/WIDscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 21:20:56.000000 WIDscript-1.2.0/src/WIDscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 21:20:56.000000 WIDscript-1.2.0/src/WIDscript.egg-info/top_level.txt
```

### Comparing `WIDscript-1.1.2/PKG-INFO` & `WIDscript-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.1.2
+Version: 1.2.0
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WIDscript-1.1.2/setup.cfg` & `WIDscript-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 4944 7363 7269 7074 0d0a 7665   = WIDscript..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 320d 0a61  rsion = 1.1.2..a
+00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
 00000030: 7574 686f 7220 3d20 5749 444f 574e 0d0a  uthor = WIDOWN..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2077  author_email = w
 00000050: 6964 6f77 6e2e 6d61 4067 6d61 696c 2e63  idown.ma@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7072 6976 6174 6520 7772 6170  = A private wrap
 00000080: 7065 7220 6d61 6465 2066 6f72 2057 4944  per made for WID
 00000090: 4f57 4e20 7265 6c65 6173 6573 2e0d 0a6c  OWN releases...l
```

### Comparing `WIDscript-1.1.2/src/WIDscript/__init__.py` & `WIDscript-1.2.0/src/WIDscript/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 core = vs.core
 
 from    vskernels      import Hermite, BSpline, Mitchell
 from    dfttest2       import DFTTest
 from    havsfunc       import DeHalo_alpha, HQDeringmod
 from    kagefunc       import retinex_edgemask
 from    vsmasktools    import retinex
-from    vsdpir_ncnn    import DPIR
 from    vsTAAmbk       import TAAmbk
 from    vsscale        import SSIM
 from    vstools        import finalize_clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 class cFormatEnum(str, Enum):
@@ -250,31 +249,27 @@
     clip = format(clip)
     clip = TAAmbk(clip, aatype='Nnedi3UpscaleSangNom', opencl=True) if (useUsAA == True) else TAAmbk(clip, aatype='Eedi3', opencl=True)
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def dpir(clip                   : vs.VideoNode,
+         enableNCNN             : bool = True,
          dpirTileDenominator    : int  = 2,
          dpirDeblocking         : bool = True,
          dpirDenoising          : bool = True,
          dpirDeblockingStrength : int  = 15,
          dpirDenoisingStrength  : int  = 1) :
     
-    clip = format(clip, cFormatEnum.RGBS)
-
-    # Divide frames by tiles to save on VRAM.
-    dpirTileW = int(clip.width  / dpirTileDenominator)
-    dpirTileH = int(clip.height / dpirTileDenominator)
-
-    # AI Assisted deblocking & denoising.
-    if (dpirDeblocking == True) : clip = DPIR(task='deblock').run(clip, strength=dpirDeblockingStrength, tile_w=dpirTileW, tile_h=dpirTileH)
-    if (dpirDenoising  == True) : clip = DPIR(task='denoise').run(clip, strength=dpirDenoisingStrength,  tile_w=dpirTileW, tile_h=dpirTileH)
-    
-    return clip
+    if (enableNCNN == False) :
+        from . import WIDscript_dpir as dpir
+        clip = dpir.dpir(clip, enableNCNN, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
+    else :
+        from . import WIDscript_dpirNCNN as dpir
+        clip = dpir.dpir(clip, enableNCNN, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def deband(clip          : vs.VideoNode,
            dbRemBinarize : int = 1500) :
 
     clip_edge = format(clip)
@@ -327,14 +322,15 @@
                #
                useDehaloing           : bool  = True,
                useDeringing           : bool  = True,
                useAA                  : bool  = True,
                useUsAA                : bool  = True,
                #
                useDPIR                : bool  = False,
+               enableNCNN             : bool  = True,
                dpirTileDenominator    : int   = 2,
                dpirDeblocking         : bool  = True,
                dpirDenoising          : bool  = True,
                dpirDeblockingStrength : int   = 15,
                dpirDenoisingStrength  : int   = 1,
                #
                useDebanding           : bool  = False,
@@ -346,12 +342,12 @@
     if (useHDR2SDR     == True) : clip = hdr2SDR(clip, dst_max, src_max, src_min)
     if (useDownscaling == True) : clip = downscale(clip, dsWidth, dsHeight)
     if (useMAGE        == True) : clip = mage(clip, thsxdxMultiplier)
     if (useUpscaling   == True) : clip = upscale(clip, isAnime, fsrcnnxPath, fsrcnnxLaPath, usWidth, usHeight)
     if (useDehaloing   == True) : clip = dehalo(clip)
     if (useDeringing   == True) : clip = dering(clip)
     if (useAA          == True) : clip = aa(clip, useUsAA)
-    if (useDPIR        == True) : clip = dpir(clip, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
+    if (useDPIR        == True) : clip = dpir(clip, enableNCNN, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
     if (useDebanding   == True) : clip = deband(clip, dbRemBinarize)
     if (useFinalizing  == True) : clip = finalize(clip)
     
     return clip
```

### Comparing `WIDscript-1.1.2/src/WIDscript.egg-info/PKG-INFO` & `WIDscript-1.2.0/src/WIDscript.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.1.2
+Version: 1.2.0
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

