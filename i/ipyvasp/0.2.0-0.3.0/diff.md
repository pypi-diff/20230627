# Comparing `tmp/ipyvasp-0.2.0.tar.gz` & `tmp/ipyvasp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.2.0.tar", last modified: Sun Jun 25 19:52:26 2023, max compression
+gzip compressed data, was "ipyvasp-0.3.0.tar", last modified: Tue Jun 27 19:26:57 2023, max compression
```

## Comparing `ipyvasp-0.2.0.tar` & `ipyvasp-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       77 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.305290 ipyvasp-0.2.0/ipyvasp/
--rw-rw-rw-   0        0        0     1803 2023-06-25 19:47:14.000000 ipyvasp-0.2.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0    38537 2023-06-25 03:01:51.000000 ipyvasp-0.2.0/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    87865 2023-06-25 16:38:58.000000 ipyvasp-0.2.0/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.2.0/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.2.0/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.334597 ipyvasp-0.2.0/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.2.0/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37749 2023-06-25 19:45:39.000000 ipyvasp-0.2.0/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34873 2023-06-25 19:28:26.000000 ipyvasp-0.2.0/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    27729 2023-06-25 15:48:45.000000 ipyvasp-0.2.0/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    11584 2023-06-25 16:42:49.000000 ipyvasp-0.2.0/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    20575 2023-06-25 16:39:06.000000 ipyvasp-0.2.0/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.2.0/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11417 2023-06-25 16:39:16.000000 ipyvasp-0.2.0/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    23766 2023-06-25 19:47:03.000000 ipyvasp-0.2.0/ipyvasp/surface.py
--rw-rw-rw-   0        0        0    15028 2023-06-25 16:39:20.000000 ipyvasp-0.2.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44839 2023-06-25 16:39:34.000000 ipyvasp-0.2.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.329406 ipyvasp-0.2.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0       77 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       86 2023-06-25 19:47:34.000000 ipyvasp-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.348920 ipyvasp-0.3.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-06-27 19:26:57.347425 ipyvasp-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.330775 ipyvasp-0.3.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1803 2023-06-27 19:25:12.000000 ipyvasp-0.3.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0    38535 2023-06-26 16:58:40.000000 ipyvasp-0.3.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    88069 2023-06-26 17:49:02.000000 ipyvasp-0.3.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.3.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.3.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.347425 ipyvasp-0.3.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.3.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37749 2023-06-25 19:45:39.000000 ipyvasp-0.3.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34873 2023-06-25 19:28:26.000000 ipyvasp-0.3.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    27729 2023-06-25 15:48:45.000000 ipyvasp-0.3.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    11584 2023-06-25 16:42:49.000000 ipyvasp-0.3.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    25081 2023-06-27 18:35:21.000000 ipyvasp-0.3.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.3.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11416 2023-06-26 16:58:55.000000 ipyvasp-0.3.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    23766 2023-06-25 19:47:03.000000 ipyvasp-0.3.0/ipyvasp/surface.py
+-rw-rw-rw-   0        0        0    15028 2023-06-25 16:39:20.000000 ipyvasp-0.3.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44839 2023-06-25 16:39:34.000000 ipyvasp-0.3.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.343142 ipyvasp-0.3.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0       77 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 19:26:57.348920 ipyvasp-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       86 2023-06-27 19:25:05.000000 ipyvasp-0.3.0/setup.py
```

### Comparing `ipyvasp-0.2.0/LICENSE` & `ipyvasp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/README.md` & `ipyvasp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/__init__.py` & `ipyvasp-0.3.0/ipyvasp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ipyvasp is a processing tool for VASP DFT input/output processing.
 
 It is designed to primarily be used in Jupyter Notebook because it offers
 widgets for interactive visualization and bulk analysis.
 """
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 __all__ = [  # For documentation purpose
     "get_axes",
     "plt2text",
     "plt2html",
     "iplot2html",
     "iplot2widget",
```

### Comparing `ipyvasp-0.2.0/ipyvasp/_enplots.py` & `ipyvasp-0.3.0/ipyvasp/_enplots.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,19 +715,19 @@
             "handlelength": 1,
             "fontsize": "small",
             "frameon": False,
             **legend_kws,
         }
         add_legend(ax, **kwargs)  # Labels are picked from plot
 
-    args = dict(ylim=elim or []) if vertical else dict(xlim=elim or [])
+    kws = dict(ylim=elim or []) if vertical else dict(xlim=elim or [])
     xlabel, ylabel = "Energy (eV)", "DOS"
     if vertical:
         xlabel, ylabel = ylabel, xlabel
-    adjust_axes(ax, xlabel=xlabel, ylabel=ylabel, zeroline=False, **args)
+    adjust_axes(ax, xlabel=xlabel, ylabel=ylabel, zeroline=False, **kws)
     return ax
 
 
 # PLOTLY PLOTS
 
 
 def _format_rgb_data(
```

### Comparing `ipyvasp-0.2.0/ipyvasp/_lattice.py` & `ipyvasp-0.3.0/ipyvasp/_lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import lru_cache
 
 from scipy.spatial import ConvexHull, KDTree
 import plotly.graph_objects as go
 
 import matplotlib.pyplot as plt  # For viewpoint
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
+import matplotlib.colors as mplc
 
 from ipywidgets import interactive
 
 # Inside packages import
 from .core import plot_toolkit as ptk
 from .core import parser as vp, serializer
 from .core.spatial_toolkit import (
@@ -2170,15 +2171,19 @@
         poscar_data = scale_poscar(
             poscar_data, [2, 2, 2], tol=tol
         )  # Repeat in all directions
 
     points = to_basis(
         new_basis, poscar_data.coords
     )  # Transform coordinates to new basis around origin
-    points = points - np.mean(points, axis=0)  # Center around origin, to include all
+
+    # Let's bring the most central point to origin
+    close_to_origin = np.linalg.norm(points - np.mean(points, axis=0), axis=1)
+    nearest_idx = np.argsort(close_to_origin)[0]
+    points = points - points[nearest_idx]  # one point is at origin now
 
     new_poscar = poscar_data.to_dict()  # Update in it
     new_poscar["basis"] = new_basis
     new_poscar["metadata"]["scale"] = np.linalg.norm(new_basis[0])
     new_poscar["metadata"]["comment"] = f"Transformed by ipyvasp"
     new_poscar["metadata"][
         "TM"
```

### Comparing `ipyvasp-0.2.0/ipyvasp/bsdos.py` & `ipyvasp-0.3.0/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/cli.py` & `ipyvasp-0.3.0/ipyvasp/cli.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/core/parser.py` & `ipyvasp-0.3.0/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.3.0/ipyvasp/core/plot_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/core/serializer.py` & `ipyvasp-0.3.0/ipyvasp/core/serializer.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.3.0/ipyvasp/core/spatial_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/lattice.py` & `ipyvasp-0.3.0/ipyvasp/lattice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-__all__ = ["POSCAR", "download_structure", "periodic_table", "get_kpath", "get_kmesh"]
+__all__ = [
+    "POSCAR",
+    "download_structure",
+    "periodic_table",
+    "get_kpath",
+    "get_kmesh",
+    "splot_bz",
+    "iplot_bz",
+]
 
 from pathlib import Path
 from contextlib import redirect_stdout
 from io import StringIO
+from functools import partial
 
 import numpy as np
 from pandas.io.clipboard import clipboard_get, clipboard_set
+import matplotlib.colors as mcolors
 
 
 from .core import serializer
 from .core import spatial_toolkit as stk
 from .utils import _sig_kwargs, _sub_doc
 from . import _lattice as plat
 from ._lattice import (
     periodic_table,
     get_kpath,
     get_kmesh,
+    splot_bz,
+    iplot_bz,
 )  # need these as direct access
 
 
 def download_structure(
     formula, mp_id=None, max_sites=None, min_sites=None, api_key=None, save_key=False
 ):
     """
@@ -53,14 +65,128 @@
         mp.save_api_key(api_key)
     if mp.success:
         return output
     else:
         raise ConnectionError("Connection was not sccessful. Try again!")
 
 
+def ngl_viewer(
+    poscar,
+    colors=None,
+    sizes=None,
+    plot_cell=True,
+    linewidth=0.05,
+    color=[0, 0, 0.2],
+    bond_color="whitesmoke",
+    width="400px",
+    height="400px",
+    plot_vectors=True,
+):
+    """Display structure in Jupyter notebook using nglview.
+
+    Parameters
+    ----------
+    poscar : ipyvasp.POSCAR
+    colors : list or str
+        List of colors for each atom type. If str, use sames colors for all.
+        If `colors = 'element'`, then element colors from `nglview` will be used.
+        You can use `nglview.color.COLOR_SCHEME` to see available color schemes to use.
+        If colors is None, then default colors from ipyvasp will be used that are same in `[i,s]plot_lattice`.
+    sizes : list
+        List of sizes for each atom type.
+    plot_cell : bool
+        Plot unit cell. Default True.
+    linewidth : float
+        Linewidth of cell edges.
+    color : list or str
+        Color of cell edges. Must be a valid color to support conversion to RGB via matplotlib.
+    bond_color : str
+        Color of bonds. Default "whitesmoke". Can be "element" or any other scheme from `nglview`.
+    width : str
+        Width of viewer. Default "400px".
+    height : str
+        Height of viewer. Default "400px".
+    plot_vectors : bool
+        Plot vectors. Default True. Only works if `plot_cell = True`.
+
+    Returns
+    -------
+    NGLWidget
+        An instance of nglview.NGLWidget object. You can use `.render_image()`, `.download_image()` etc. on it or can add more representations.
+
+    .. note::
+        `nglview` sometimes does not work in Jupyter lab. You can switch to classic notebook in that case.
+    """
+    if not isinstance(poscar, POSCAR):
+        raise TypeError("poscar must be an instance of POSCAR class.")
+
+    try:
+        import nglview as nv
+    except ImportError:
+        raise ImportError("Please install nglview to use this function.")
+
+    if plot_cell:  # Only show equivalent sites if plotting cell
+        poscar = POSCAR(data=plat._fix_sites(poscar.data, eqv_sites=True))
+
+    _types = list(poscar.data.types.keys())
+    _sizes = [0.5 for _ in _types]
+    _colors = [mcolors.to_hex(plat._atom_colors[e]) for e in _types]
+
+    if sizes:
+        if len(sizes) != len(_types):
+            raise ValueError(
+                "sizes must have the same length as the number of atom types."
+            )
+        _sizes = sizes
+
+    if colors:
+        if isinstance(colors, str):
+            _colors = [colors for _ in _types]  # All same color, may be 'element'
+        else:
+            if len(colors) != len(_types):
+                raise ValueError(
+                    "colors must have the same length as the number of atom types."
+                )
+            _colors = [mcolors.to_hex(c) for c in colors]
+
+    view = nv.NGLWidget(
+        nv.ASEStructure(poscar.to_ase()),
+        width=width,
+        height=height,
+        default_representation=False,
+    )
+    view.clear()
+
+    for e, r, c in zip(_types, _sizes, _colors):
+        view.add_spacefill(radius=r, selection=f"#{e}", color=c)
+
+    view.add_ball_and_stick(color=bond_color)
+    view.camera = "orthographic"
+    view.center()
+
+    if plot_cell:
+        shape = nv.shape.Shape(view=view)
+        _color = mcolors.to_rgb(color)  # convert to rgb for nglview
+        cell = poscar.get_cell()
+        for face in cell.faces_coords:
+            for p1, p2 in zip(face[1:], face[:-1]):
+                shape.add_cylinder(p1, p2, _color, linewidth)
+
+        for v in cell.vertices:
+            shape.add_sphere(v, _color, linewidth)
+
+        if plot_vectors:
+            for i, b in enumerate(cell.basis, start=1):
+                tail = b - b / np.linalg.norm(b)
+                shape.add_cone(tail, b, _color, linewidth * 3, f"a{i}")
+                shape.add_text(b / 2, [0.2, 0.15, 0.2], 2, f"a{i}")
+
+    return view
+
+
 class POSCAR:
     _cb_instance = {}  # Loads last clipboard data if not changed
     _mp_instance = {}  # Loads last mp data if not changed
 
     def __init__(self, path=None, content=None, data=None):
         """
         POSCAR class to contain data and related methods, data is PoscarData, json/tuple file/string.
@@ -119,31 +245,39 @@
         >>> reciprocal_lattice.plt_bz() # Plot BZ usinn ase, it also plots suggested band path.
         """
         from ase import Atoms
 
         symbols = [
             lab.split()[0] for lab in self.data.labels
         ]  # Remove numbers from labels
-        return Atoms(
-            symbols=symbols, positions=self.data.positions, cell=self.data.basis
+        return Atoms(  # ASE positions are cartesian, not fractional
+            symbols=symbols, positions=self.data.coords, cell=self.data.basis
         )
 
     def view(self, viewer=None, **kwargs):
         """View POSCAR in notebook. If viewer is given it will be passed ase.visualize.view. You need to have ase installed.
 
         kwargs are passed to self.splot_lattice if viewer is None, otherwise a  single keyword argument `data` is passed to ase viewer.
         data should be volumetric data for ase.visualize.view, such as charge density, spin density, etc.
+
+        .. tip::
+            Use ``self.view_ngl()`` if you don't want to pass ``viewer = 'nglview'`` to ASE viewer or not showing volumetric data.
         """
         if viewer is None:
             return plat.view_poscar(self.data, **kwargs)
         else:
             from ase.visualize import view
 
             return view(self.to_ase(), viewer=viewer, data=kwargs.get("data", None))
 
+    @_sub_doc(ngl_viewer, {"poscar :.*colors :": "colors :"})
+    @_sig_kwargs(ngl_viewer, ("poscar",))
+    def view_ngl(self, **kwargs):
+        return ngl_viewer(self, **kwargs)
+
     def view_kpath(self):
         "Initialize a KpathWidget instance to view kpath for current POSCAR, and you can select others too."
         from .widgets import KpathWidget
 
         return KpathWidget(path=str(self.path.parent), glob=self.path.name)
 
     @classmethod
@@ -384,15 +518,15 @@
         if not labels:
             labels = [
                 "[{0:5.2f}, {1:5.2f}, {2:5.2f}]".format(x, y, z) for x, y, z in kpoints
             ]
 
         plat._validate_label_func(fmt_label, labels[0])
 
-        coords = self.to_R3(kpoints, reciprocal=True)
+        coords = self.bz.to_cartesian(kpoints)
         if _zoffset and self._plane:
             normal = (
                 [0, 0, 1]
                 if self._plane in "xyx"
                 else [0, 1, 0]
                 if self._plane in "xzx"
                 else [1, 0, 0]
```

### Comparing `ipyvasp-0.2.0/ipyvasp/misc.py` & `ipyvasp-0.3.0/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/potential.py` & `ipyvasp-0.3.0/ipyvasp/potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 value=0.125,
                 step=_step,
                 readout_format=".4f",
                 continuous_update=False,
             ),
         )
 
-    def view_slice(self, *argse, **kwargs):
+    def view_slice(self, *args, **kwargs):
         # Use interactive here to select the slice, digonal slices and so on..., tell user to get output results back
         raise NotImplementedError("Coming soon...")
 
 
 class CHG(LOCPOT):
     __doc__ = LOCPOT.__doc__.replace("LOCPOT", "CHG")
```

### Comparing `ipyvasp-0.2.0/ipyvasp/surface.py` & `ipyvasp-0.3.0/ipyvasp/surface.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/utils.py` & `ipyvasp-0.3.0/ipyvasp/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.2.0/ipyvasp/widgets.py` & `ipyvasp-0.3.0/ipyvasp/widgets.py`

 * *Files identical despite different names*

