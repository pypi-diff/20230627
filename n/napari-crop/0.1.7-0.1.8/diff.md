# Comparing `tmp/napari-crop-0.1.7.tar.gz` & `tmp/napari-crop-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-crop-0.1.7.tar", last modified: Fri Feb 17 09:56:24 2023, max compression
+gzip compressed data, was "napari-crop-0.1.8.tar", last modified: Tue Jun 27 15:17:14 2023, max compression
```

## Comparing `napari-crop-0.1.7.tar` & `napari-crop-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 09:56:24.535742 napari-crop-0.1.7/
--rw-rw-rw-   0        0        0     1623 2023-02-17 09:55:20.000000 napari-crop-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      127 2023-02-17 09:55:20.000000 napari-crop-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4591 2023-02-17 09:56:24.536745 napari-crop-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3319 2023-02-17 09:55:20.000000 napari-crop-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 09:56:24.486461 napari-crop-0.1.7/napari_crop/
--rw-rw-rw-   0        0        0      134 2023-02-17 09:55:20.000000 napari-crop-0.1.7/napari_crop/__init__.py
--rw-rw-rw-   0        0        0     5787 2023-02-17 09:55:20.000000 napari-crop-0.1.7/napari_crop/_function.py
-drwxrwxrwx   0        0        0        0 2023-02-17 09:56:24.534740 napari-crop-0.1.7/napari_crop/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-17 09:55:20.000000 napari-crop-0.1.7/napari_crop/_tests/__init__.py
--rw-rw-rw-   0        0        0     4992 2023-02-17 09:55:20.000000 napari-crop-0.1.7/napari_crop/_tests/test_function.py
-drwxrwxrwx   0        0        0        0 2023-02-17 09:56:24.531678 napari-crop-0.1.7/napari_crop.egg-info/
--rw-rw-rw-   0        0        0     4591 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-17 09:56:24.000000 napari-crop-0.1.7/napari_crop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      198 2023-02-17 09:55:20.000000 napari-crop-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0     1382 2023-02-17 09:56:24.550926 napari-crop-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-17 09:55:20.000000 napari-crop-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:17:14.584505 napari-crop-0.1.8/
+-rw-rw-rw-   0        0        0     1623 2022-02-07 14:47:59.000000 napari-crop-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      127 2022-02-07 14:47:59.000000 napari-crop-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4789 2023-06-27 15:17:14.585509 napari-crop-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3517 2023-06-27 08:24:08.000000 napari-crop-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:17:14.503694 napari-crop-0.1.8/napari_crop/
+-rw-rw-rw-   0        0        0      149 2023-06-26 07:09:46.000000 napari-crop-0.1.8/napari_crop/__init__.py
+-rw-rw-rw-   0        0        0    10604 2023-06-27 14:52:20.000000 napari-crop-0.1.8/napari_crop/_dock_widgets.py
+-rw-rw-rw-   0        0        0     7906 2023-06-27 07:10:02.000000 napari-crop-0.1.8/napari_crop/_function.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:17:14.581503 napari-crop-0.1.8/napari_crop/_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-07 14:47:59.000000 napari-crop-0.1.8/napari_crop/_tests/__init__.py
+-rw-rw-rw-   0        0        0     8475 2023-06-26 14:56:20.000000 napari-crop-0.1.8/napari_crop/_tests/test_function.py
+-rw-rw-rw-   0        0        0      917 2023-06-23 14:29:47.000000 napari-crop-0.1.8/napari_crop/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     1272 2023-06-27 06:45:09.000000 napari-crop-0.1.8/napari_crop/_utils.py
+-rw-rw-rw-   0        0        0      610 2023-06-27 06:58:54.000000 napari-crop-0.1.8/napari_crop/bla.py
+-rw-rw-rw-   0        0        0      541 2023-06-27 07:28:49.000000 napari-crop-0.1.8/napari_crop/try_cut_plane.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:17:14.551892 napari-crop-0.1.8/napari_crop.egg-info/
+-rw-rw-rw-   0        0        0     4789 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 15:17:14.000000 napari-crop-0.1.8/napari_crop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      198 2022-02-07 14:47:59.000000 napari-crop-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0     1409 2023-06-27 15:17:14.593052 napari-crop-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       89 2022-02-07 14:47:59.000000 napari-crop-0.1.8/setup.py
```

### Comparing `napari-crop-0.1.7/LICENSE` & `napari-crop-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-crop-0.1.7/PKG-INFO` & `napari-crop-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-crop
-Version: 0.1.7
+Version: 0.1.8
 Summary: Crop regions in napari manually
 Home-page: https://github.com/biapol/napari-crop
 Author: Robert Haase, Tim Morello, Marcelo Leomil Zoccoler, Johannes Muller
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/biapol/napari-crop/issues
 Project-URL: Documentation, https://github.com/biapol/napari-crop#README.md
@@ -37,15 +37,21 @@
 
 Crop regions in napari manually
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/screencast.gif)
 
 Crop in any dimension
 
-![](https://github.com/haesleinhuepf/napari-crop/blob/main/images/side_crop.gif)
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/side_crop.gif)
+
+Cut a volume using a plane
+
+*Note: this functionality currently only works with 3D data*
+
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/napari_crop_cut_with_plane_demo.gif)
 
 ## Usage
 Create a new shapes layer to annotate the region you would like to crop:
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/shapes.png)
 
 Use the rectangle tool to annotate a region. Start the `crop` tool from the `Tools > Utilities > Crop region` menu.
```

### Comparing `napari-crop-0.1.7/README.md` & `napari-crop-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 
 Crop regions in napari manually
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/screencast.gif)
 
 Crop in any dimension
 
-![](https://github.com/haesleinhuepf/napari-crop/blob/main/images/side_crop.gif)
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/side_crop.gif)
+
+Cut a volume using a plane
+
+*Note: this functionality currently only works with 3D data*
+
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/napari_crop_cut_with_plane_demo.gif)
 
 ## Usage
 Create a new shapes layer to annotate the region you would like to crop:
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/shapes.png)
 
 Use the rectangle tool to annotate a region. Start the `crop` tool from the `Tools > Utilities > Crop region` menu.
```

### Comparing `napari-crop-0.1.7/napari_crop/_function.py` & `napari-crop-0.1.8/napari_crop/_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import warnings
 
 import numpy as np
-from napari_plugin_engine import napari_hook_implementation
+from magicgui import magic_factory
 from napari_tools_menu import register_function
 import napari
 from napari.types import LayerDataTuple
 from typing import List
-
+from ._utils import compute_combined_slices
 
 # This is the actual plugin function, where we export our function
 # (The functions themselves are defined below)
-@napari_hook_implementation
-def napari_experimental_provide_function():
-    return [crop_region]
 
 
-@register_function(menu="Utilities > Crop region(s)")
+@register_function(menu="Utilities > Crop region(s) (napari-crop)")
 def crop_region(
     layer: napari.layers.Layer,
     shapes_layer: napari.layers.Shapes,
-    viewer: 'napari.viewer.Viewer' = None, 
+    viewer: 'napari.viewer.Viewer' = None,
 ) -> List[LayerDataTuple]:
     """Crop regions in napari defined by shapes."""
     if shapes_layer is None:
         shapes_layer.mode = "add_rectangle"
         warnings.warn("Please annotate a region to crop.")
         return
 
@@ -83,16 +80,16 @@
                 .squeeze()
             )
             # match cropped_data (x,y) shape with mask_2D shape
             cropped_data_shape = cropped_data.shape
             # Adjust cropped_data axes order in case axes were swapped in napari
             if viewer is not None:
                 cropped_data_shape = np.moveaxis(cropped_data,
-                                                  viewer.dims.order,
-                                                  np.arange(len(cropped_data_shape))).shape
+                                                 viewer.dims.order,
+                                                 np.arange(len(layer_shape))).shape
             if rgb:
                 shape_dif_2D = np.array(cropped_data_shape[-3:-1]) \
                     - np.array(mask_2D.shape)
             else:
                 shape_dif_2D = np.array(cropped_data_shape[-2:]) \
                     - np.array(mask_2D.shape)
             shape_dif_2D = [None if i == 0 else i
@@ -105,35 +102,104 @@
             mask_nD = mask_2D.reshape(mask_nD_shape)
             # broadcast the mask to the shape of the cropped image
             mask = np.broadcast_to(mask_nD, cropped_data.shape)
             # erase pixels outside drawn shape
             cropped_data[~mask] = 0
 
             # trim zeros
-            non_zero = np.where(cropped_data != 0)
-            slices = [slice(min(i_nz), max(i_nz) + 1) for i_nz in non_zero]
-            if rgb:
-                slices[-1] = slice(None)
-            cropped_data = cropped_data[tuple(slices)]
+            inner_slices = get_nonzero_slices(cropped_data)
+            cropped_data = trim_zeros(cropped_data, rgb=rgb)
+            slices = compute_combined_slices(layer_shape, slices, inner_slices)
 
         new_layer_props = layer_props.copy()
         # Update start and stop values for bbox
         start = [slc.start for slc in slices if slc is not None]
-        stop = [slc.stop for slc in slices if slc is not None]
+        stop = []
+        for slc in slices:
+            if slc is not None:
+                if slc.stop is None:
+                    stop.append(layer_shape[slices.index(slc)])
+                else:
+                    stop.append(slc.stop)
+        # stop = [slc.stop for slc in slices if slc is not None]
         # Add cropped coordinates as metadata
-        # bounding box: (min_row, max_row, min_col, max_col)
+        # bounding box: ([min_z,] min_row, min_col, [max_z,] max_row, max_col)
         # Pixels belonging to the bounding box are in the half-open interval [min_row; max_row) and [min_col; max_col).
-        new_layer_props['metadata'] = {'bbox': (start[0], stop[0], start[1], stop[1])}
+        new_layer_props['metadata'] = {'bbox': tuple(start + stop)}
+        # apply layer translation scaled by layer scaling factor
+        new_layer_props['translate'] = tuple(np.asarray(tuple(start)) * np.asarray(layer_props['scale']))
 
         # If layer name is in viewer or is about to be added,
         # increment layer name until it has a different name
         while True:
             new_name = layer_props["name"] \
                 + f" cropped [{shape_count+new_layer_index}]"
             if new_name not in names_list:
                 break
             else:
                 new_layer_index += 1
         new_layer_props["name"] = new_name
         names_list.append(new_name)
         cropped_list.append((cropped_data, new_layer_props, layer_type))
     return cropped_list
+
+
+def get_nonzero_slices(array):
+    non_zero = np.where(array != 0)
+    return [slice(min(i_nz), max(i_nz) + 1) for i_nz in non_zero]
+
+
+def trim_zeros(image, rgb=False):
+    slices = get_nonzero_slices(image)
+    if rgb:
+        slices[-1] = slice(None)
+    return image[tuple(slices)]
+
+
+def cut_with_plane(image_to_be_cut, plane_normal, plane_position, positive_cut=True, crop=False):
+    """Cut a 3D volume with a plane
+
+    Parameters
+    ----------
+    image_to_be_cut : array_like (3D)
+        3D image to be cut
+    plane_normal : tuple (3)
+        Normal vector of the plane
+    plane_position : tuple (3)
+        Position of the plane center
+    positive_cut : bool, optional
+        If True, the positive side of the plane is kept.
+        If False, the negative side of the plane is kept. By default True
+
+    Returns
+    -------
+    array_like (3D)
+        Cut image with the same shape as the input image
+    """
+    import numpy as np
+    if len(image_to_be_cut.shape) != 3:
+        print('Input image to be cut must be 3D')
+        return
+    image_to_be_cut = np.asarray(image_to_be_cut)
+
+    x = np.arange(image_to_be_cut.shape[2])
+    y = np.arange(image_to_be_cut.shape[1])
+    z = np.arange(image_to_be_cut.shape[0])
+
+    zmesh, ymesh, xmesh = np.meshgrid(z, y, x, indexing='ij')
+
+    xm = xmesh - plane_position[2]
+    ym = ymesh - plane_position[1]
+    zm = zmesh - plane_position[0]
+
+    p = xm * plane_normal[2] + ym * plane_normal[1] + zm * plane_normal[0]
+
+    if positive_cut:
+        mask = np.where(p >= 0, 1, 0).astype(bool)
+    else:
+        mask = np.where(p < 0, 1, 0).astype(bool)
+
+    image_cut = image_to_be_cut.copy()
+    image_cut[~mask] = 0
+    if crop:
+        image_cut = trim_zeros(image_cut)
+    return image_cut
```

### Comparing `napari-crop-0.1.7/napari_crop.egg-info/PKG-INFO` & `napari-crop-0.1.8/napari_crop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-crop
-Version: 0.1.7
+Version: 0.1.8
 Summary: Crop regions in napari manually
 Home-page: https://github.com/biapol/napari-crop
 Author: Robert Haase, Tim Morello, Marcelo Leomil Zoccoler, Johannes Muller
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/biapol/napari-crop/issues
 Project-URL: Documentation, https://github.com/biapol/napari-crop#README.md
@@ -37,15 +37,21 @@
 
 Crop regions in napari manually
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/screencast.gif)
 
 Crop in any dimension
 
-![](https://github.com/haesleinhuepf/napari-crop/blob/main/images/side_crop.gif)
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/side_crop.gif)
+
+Cut a volume using a plane
+
+*Note: this functionality currently only works with 3D data*
+
+![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/napari_crop_cut_with_plane_demo.gif)
 
 ## Usage
 Create a new shapes layer to annotate the region you would like to crop:
 
 ![](https://github.com/haesleinhuepf/napari-crop/raw/main/images/shapes.png)
 
 Use the rectangle tool to annotate a region. Start the `crop` tool from the `Tools > Utilities > Crop region` menu.
```

### Comparing `napari-crop-0.1.7/setup.cfg` & `napari-crop-0.1.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 6372 6f70 0d0a   = napari-crop..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 370d  version = 0.1.7.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 380d  version = 0.1.8.
 00000030: 0a61 7574 686f 7220 3d20 526f 6265 7274  .author = Robert
 00000040: 2048 6161 7365 2c20 5469 6d20 4d6f 7265   Haase, Tim More
 00000050: 6c6c 6f2c 204d 6172 6365 6c6f 204c 656f  llo, Marcelo Leo
 00000060: 6d69 6c20 5a6f 6363 6f6c 6572 2c20 4a6f  mil Zoccoler, Jo
 00000070: 6861 6e6e 6573 204d 756c 6c65 720d 0a61  hannes Muller..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 726f  uthor_email = ro
 00000090: 6265 7274 2e68 6161 7365 4074 752d 6472  bert.haase@tu-dr
@@ -73,15 +73,17 @@
 00000480: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
 00000490: 2e37 0d0a 696e 7374 616c 6c5f 7265 7175  .7..install_requ
 000004a0: 6972 6573 203d 200d 0a09 6e61 7061 7269  ires = ...napari
 000004b0: 2d70 6c75 6769 6e2d 656e 6769 6e65 3e3d  -plugin-engine>=
 000004c0: 302e 312e 340d 0a09 6e75 6d70 790d 0a09  0.1.4...numpy...
 000004d0: 7363 696b 6974 2d69 6d61 6765 0d0a 096e  scikit-image...n
 000004e0: 6170 6172 692d 746f 6f6c 732d 6d65 6e75  apari-tools-menu
-000004f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000500: 7279 5f70 6f69 6e74 735d 0d0a 6e61 7061  ry_points]..napa
-00000510: 7269 2e70 6c75 6769 6e20 3d20 0d0a 096e  ri.plugin = ...n
-00000520: 6170 6172 692d 6372 6f70 203d 206e 6170  apari-crop = nap
-00000530: 6172 695f 6372 6f70 0d0a 0d0a 5b65 6767  ari_crop....[egg
-00000540: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000550: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000560: 2030 0d0a 0d0a                            0....
+000004f0: 3e3d 302e 312e 3137 0d0a 096e 6170 6172  >=0.1.17...napar
+00000500: 692d 776f 726b 666c 6f77 730d 0a0d 0a5b  i-workflows....[
+00000510: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+00000520: 696e 7473 5d0d 0a6e 6170 6172 692e 706c  ints]..napari.pl
+00000530: 7567 696e 203d 200d 0a09 6e61 7061 7269  ugin = ...napari
+00000540: 2d63 726f 7020 3d20 6e61 7061 7269 5f63  -crop = napari_c
+00000550: 726f 700d 0a0d 0a5b 6567 675f 696e 666f  rop....[egg_info
+00000560: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000570: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000580: 0a                                       .
```

