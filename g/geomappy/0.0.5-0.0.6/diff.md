# Comparing `tmp/geomappy-0.0.5.tar.gz` & `tmp/geomappy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geomappy-0.0.5.tar", last modified: Fri Jun 23 14:22:28 2023, max compression
+gzip compressed data, was "geomappy-0.0.6.tar", last modified: Tue Jun 27 15:10:40 2023, max compression
```

## Comparing `geomappy-0.0.5.tar` & `geomappy-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-23 14:22:28.000000 geomappy-0.0.5/
--rw-r--r--   0 jroebroek   (501) staff       (20)     1072 2021-12-02 09:00:50.000000 geomappy-0.0.5/LICENSE
--rw-r--r--   0 jroebroek   (501) staff       (20)      248 2023-06-23 14:22:28.000000 geomappy-0.0.5/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)      384 2022-01-21 17:42:19.000000 geomappy-0.0.5/README.md
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy/
--rw-r--r--   0 jroebroek   (501) staff       (20)      964 2023-06-22 10:10:42.000000 geomappy-0.0.5/geomappy/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     4929 2023-06-22 13:12:44.000000 geomappy-0.0.5/geomappy/axes_decoration.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     6896 2023-06-23 11:00:00.000000 geomappy-0.0.5/geomappy/basemap.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     1205 2023-06-22 14:35:59.000000 geomappy-0.0.5/geomappy/bounds.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     1585 2023-06-23 09:11:44.000000 geomappy-0.0.5/geomappy/classified.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     9838 2023-06-22 13:12:44.000000 geomappy-0.0.5/geomappy/colors.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     7938 2023-06-22 15:54:39.000000 geomappy-0.0.5/geomappy/geodataframe.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     3030 2023-06-22 13:12:44.000000 geomappy-0.0.5/geomappy/legends.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     7033 2023-06-23 11:11:43.000000 geomappy-0.0.5/geomappy/raster.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     2231 2023-06-23 09:11:44.000000 geomappy-0.0.5/geomappy/scalar.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    17953 2023-06-23 10:48:24.000000 geomappy-0.0.5/geomappy/shapes.py
--rw-r--r--   0 jroebroek   (501) staff       (20)      498 2023-06-22 13:12:44.000000 geomappy-0.0.5/geomappy/types.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     2184 2023-06-22 13:36:54.000000 geomappy-0.0.5/geomappy/utils.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     1993 2023-06-22 15:34:00.000000 geomappy-0.0.5/geomappy/world.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     8269 2023-06-23 13:35:29.000000 geomappy-0.0.5/geomappy/xarray.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/
--rw-r--r--   0 jroebroek   (501) staff       (20)      248 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)      513 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/SOURCES.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        1 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/dependency_links.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       93 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/requires.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        9 2023-06-23 14:22:28.000000 geomappy-0.0.5/geomappy.egg-info/top_level.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       38 2023-06-23 14:22:28.000000 geomappy-0.0.5/setup.cfg
--rw-r--r--   0 jroebroek   (501) staff       (20)      456 2023-06-23 14:21:45.000000 geomappy-0.0.5/setup.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-23 14:22:28.000000 geomappy-0.0.5/tests/
--rw-r--r--   0 jroebroek   (501) staff       (20)     4230 2023-06-23 08:53:00.000000 geomappy-0.0.5/tests/test_plotting.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-27 15:10:40.177931 geomappy-0.0.6/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1072 2021-12-02 09:00:50.000000 geomappy-0.0.6/LICENSE
+-rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-27 15:10:40.177502 geomappy-0.0.6/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      384 2022-01-21 17:42:19.000000 geomappy-0.0.6/README.md
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-27 15:10:40.173639 geomappy-0.0.6/geomappy/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      982 2023-06-24 12:21:19.000000 geomappy-0.0.6/geomappy/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     5060 2023-06-24 13:47:28.000000 geomappy-0.0.6/geomappy/axes_decoration.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     6971 2023-06-24 13:46:09.000000 geomappy-0.0.6/geomappy/basemap.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1243 2023-06-24 13:45:12.000000 geomappy-0.0.6/geomappy/bounds.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1636 2023-06-24 13:54:49.000000 geomappy-0.0.6/geomappy/classified.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     9904 2023-06-24 14:01:48.000000 geomappy-0.0.6/geomappy/colors.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7995 2023-06-24 13:37:53.000000 geomappy-0.0.6/geomappy/geodataframe.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3082 2023-06-24 14:01:37.000000 geomappy-0.0.6/geomappy/legends.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7201 2023-06-24 13:56:28.000000 geomappy-0.0.6/geomappy/raster.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2263 2023-06-24 13:46:26.000000 geomappy-0.0.6/geomappy/scalar.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)    18634 2023-06-24 14:17:18.000000 geomappy-0.0.6/geomappy/shapes.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)      299 2023-06-24 13:03:02.000000 geomappy-0.0.6/geomappy/types.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2174 2023-06-24 13:49:24.000000 geomappy-0.0.6/geomappy/utils.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2014 2023-06-24 13:45:21.000000 geomappy-0.0.6/geomappy/world.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     8339 2023-06-24 14:49:40.000000 geomappy-0.0.6/geomappy/xarray.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-27 15:10:40.175503 geomappy-0.0.6/geomappy.egg-info/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-27 15:10:40.000000 geomappy-0.0.6/geomappy.egg-info/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      573 2023-06-27 15:10:40.000000 geomappy-0.0.6/geomappy.egg-info/SOURCES.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        1 2023-06-27 15:10:40.000000 geomappy-0.0.6/geomappy.egg-info/dependency_links.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       93 2023-06-27 15:10:40.000000 geomappy-0.0.6/geomappy.egg-info/requires.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        9 2023-06-27 15:10:40.000000 geomappy-0.0.6/geomappy.egg-info/top_level.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       38 2023-06-27 15:10:40.178147 geomappy-0.0.6/setup.cfg
+-rw-r--r--   0 jroebroek   (501) staff       (20)      456 2023-06-27 15:09:56.000000 geomappy-0.0.6/setup.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-27 15:10:40.176526 geomappy-0.0.6/tests/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      897 2023-06-24 13:56:28.000000 geomappy-0.0.6/tests/test_classified_params.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     4242 2023-06-24 14:00:04.000000 geomappy-0.0.6/tests/test_plotting.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1350 2023-06-23 08:55:39.000000 geomappy-0.0.6/tests/test_scalar_params.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `geomappy-0.0.5/LICENSE` & `geomappy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geomappy-0.0.5/geomappy/__init__.py` & `geomappy-0.0.6/geomappy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from geomappy.geodataframe import gpd_plot_shapes, gpd_plot_classified_shapes, gpd_plot_world, gpd_plot_file
-from geomappy.xarray import xarray_plot_raster, xarray_plot_classified_raster, xarray_plot_world, xarray_plot_file
+import warnings
+
+import matplotlib  # type: ignore
+
 from geomappy.basemap import basemap, add_ticks, add_gridlines
+from geomappy.geodataframe import gpd_plot_shapes, gpd_plot_classified_shapes, gpd_plot_world, gpd_plot_file
 from geomappy.raster import plot_raster, plot_classified_raster
 from geomappy.shapes import plot_shapes, plot_classified_shapes
-
-import matplotlib
-import warnings
+from geomappy.xarray import xarray_plot_raster, xarray_plot_classified_raster, xarray_plot_world, xarray_plot_file
 
 # Import 'show' and 'savefig' for convenience. This should be avoided in production code.
 show = matplotlib.pyplot.show
 savefig = matplotlib.pyplot.savefig
 
 try:
     from sphinx.ext.autodoc.mock import _MockModule
+
     if not isinstance(matplotlib, _MockModule):
         warnings.filterwarnings("once", category=FutureWarning)
         warnings.filterwarnings("once", category=matplotlib.MatplotlibDeprecationWarning)
         matplotlib.rcParams["image.interpolation"] = 'none'
 except ModuleNotFoundError:
     pass
```

### Comparing `geomappy-0.0.5/geomappy/axes_decoration.py` & `geomappy-0.0.6/geomappy/axes_decoration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import Tuple, Optional, Union
 
-from matplotlib import pyplot as plt
-from matplotlib.cm import ScalarMappable
-from matplotlib.image import AxesImage
-from matplotlib.lines import Line2D
-from matplotlib.patches import Patch
-from mpl_toolkits import axes_grid1
-from mpl_toolkits.axes_grid1.inset_locator import InsetPosition
+from matplotlib import pyplot as plt  # type: ignore
+from matplotlib.cm import ScalarMappable  # type: ignore
+from matplotlib.image import AxesImage  # type: ignore
+from matplotlib.lines import Line2D  # type: ignore
+from matplotlib.patches import Patch  # type: ignore
+from mpl_toolkits import axes_grid1  # type: ignore
+from mpl_toolkits.axes_grid1.inset_locator import InsetPosition  # type: ignore
 
-from geomappy.types import Number
 
+def prepare_axes(ax: Optional[plt.Axes] = None, figsize: Optional[Tuple[int, int]] = None) -> plt.Axes:
+    if figsize is None:
+        figsize = (8, 8)
 
-def prepare_axes(ax: Optional[plt.Axes] = None, figsize: Tuple[int, int] = (10, 10)) -> plt.Axes:
     if ax is None:
         f, ax = plt.subplots(figsize=figsize)
 
     return ax
 
 
-def create_colorbar_axes(ax: plt.Axes, aspect: Number = 30, pad_fraction: float = 0.6, position="right"):
+def create_colorbar_axes(ax: plt.Axes, aspect: float = 30, pad_fraction: float = 0.6, position="right"):
     """
     Create an axes for the colorbar to be drawn on that has the same size as the figure
 
     Parameters
     ----------
     ax : Axes, optional
         The Axes that the colorbar will added to.
@@ -41,15 +42,15 @@
     width = axes_grid1.axes_size.AxesY(ax, aspect=1. / aspect)
     pad = axes_grid1.axes_size.Fraction(pad_fraction, width)
     ax = divider.append_axes(position=position, size=width, pad=pad, axes_class=plt.Axes)
     return ax
 
 
 def add_colorbar(im: Optional[Union[ScalarMappable, AxesImage]] = None, ax: Optional[plt.Axes] = None,
-                 legend_ax: Optional[plt.Axes] = None, aspect: Number = 25, pad_fraction: float = 0.7,
+                 legend_ax: Optional[plt.Axes] = None, aspect: float = 25, pad_fraction: float = 0.7,
                  position: str = "right", shrink=1, **kwargs):
     """
     Add colorbar to a plot
 
     Parameters
     ----------
     im : ScalarMappable, optional
```

### Comparing `geomappy-0.0.5/geomappy/basemap.py` & `geomappy-0.0.6/geomappy/basemap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from numbers import Number
 from typing import Union, Tuple
 
-import cartopy
-import cartopy.crs as ccrs
-import matplotlib.pyplot as plt
-import matplotlib.ticker as mticker
+import cartopy  # type: ignore
+import cartopy.crs as ccrs  # type: ignore
+import matplotlib.pyplot as plt  # type: ignore
+import matplotlib.ticker as mticker  # type: ignore
 import numpy as np
-from cartopy.mpl.geoaxes import GeoAxes
-from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
+from cartopy.mpl.geoaxes import GeoAxes  # type: ignore
+from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter  # type: ignore
 
 
 class ProjectCustomExtent(ccrs.Projection):
     """
     Creating a custom extent for a given epsg code, if the hardcoded values do not suffice
     """
+
     def __init__(self, epsg: Union[str, int], extent: Tuple[int, int, int, int], *args, **kwargs):
         super(ccrs.Projection, self).__init__(f"EPSG:{epsg}")
         xmin, xmax, ymin, ymax = extent
         self.xmin = xmin
         self.xmax = xmax
         self.ymin = ymin
         self.ymax = ymax
@@ -46,27 +46,27 @@
         return self.xmin, self.xmax
 
     @property
     def y_limits(self):
         return self.ymin, self.ymax
 
 
-def calculate_horizontal_locations(v: Union[Number, Tuple[Number]]):
+def calculate_horizontal_locations(v: Union[float, Tuple[float]]):
     if isinstance(v, (float, int)):
         return np.linspace(-180, 180, int(360 / v + 1))
     return np.asarray(v)
 
 
-def calculate_vertical_locations(v: Union[Number, Tuple[Number]]):
+def calculate_vertical_locations(v: Union[float, Tuple[float]]):
     if isinstance(v, (float, int)):
         return np.linspace(-90, 90, int(180 / v + 1))
     return np.asarray(v)
 
 
-def add_gridlines(ax: GeoAxes, lines: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]], *,
+def add_gridlines(ax: GeoAxes, lines: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]], *,
                   color: str = "grey", linestyle: str = "--", alpha: float = 0.5, n_steps: int = 300,
                   linewidth: float = 1, crs: ccrs.Projection = ccrs.PlateCarree(), **kwargs) -> None:
     """Add gridlines to a basemap. Return a Gridliner object that can be further modified
 
     Parameters
     ----------
     ax: GeoAxes
@@ -100,15 +100,16 @@
                      linewidth=linewidth, **kwargs)
     g.xlocator = mticker.FixedLocator(xlines)
     g.ylocator = mticker.FixedLocator(ylines)
     g.n_steps = n_steps
     return g
 
 
-def add_ticks(ax: GeoAxes, ticks: Union[int, Tuple[int, int], Tuple[Tuple[int, int], Tuple[int, int]]], *,
+def add_ticks(ax: GeoAxes,
+              ticks: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]], *,
               formatter: Union[mticker.Formatter, Tuple[mticker.Formatter, mticker.Formatter], None] = None,
               fontsize: int = 10, crs: ccrs.Projection = ccrs.PlateCarree(), **kwargs) -> None:
     """Helper function creating labels. Returns a Gridliner object that can be further modified for styling
 
     Parameters
     ----------
     ax: GeoAxes
```

### Comparing `geomappy-0.0.5/geomappy/bounds.py` & `geomappy-0.0.6/geomappy/bounds.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Optional, Tuple
+from typing import Tuple
 
-import geopandas as gpd
+import geopandas as gpd  # type: ignore
 import numpy as np
 from pyproj import Proj
-from rasterio.coords import BoundingBox
-from shapely.geometry import Polygon
+from rasterio.coords import BoundingBox  # type: ignore
+from shapely.geometry import Polygon  # type: ignore
 
 PROJ_LAT_LON = Proj(4326, preserve_units=False)
 
 
 def bounds_to_polygons(bounds_list: Tuple[BoundingBox]):
     """
     Creating a geodataframe with polygons based on a list of bounds.
```

### Comparing `geomappy-0.0.5/geomappy/classified.py` & `geomappy-0.0.6/geomappy/classified.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Optional, Tuple, Iterable
 
 import numpy as np
-from matplotlib import pyplot as plt
-from matplotlib.colors import Colormap, BoundaryNorm, ListedColormap
+from matplotlib import pyplot as plt  # type: ignore
+from matplotlib.colors import Colormap, BoundaryNorm, ListedColormap  # type: ignore
 
 from geomappy.colors import colors_discrete
 from geomappy.types import Color
 from geomappy.utils import check_increasing_and_unique
 
 
 def parse_classified_plot_params(m: np.ma.MaskedArray, *, levels: Optional[Iterable] = None,
                                  colors: Optional[Iterable] = None,
                                  cmap: Colormap = "Set1", nan_color: Optional[Color] = None,
-                                 suppress_warnings: bool = False) -> Tuple[ListedColormap, BoundaryNorm]:
+                                 suppress_warnings: bool = False) -> Tuple[ListedColormap, BoundaryNorm, np.ndarray]:
     unique_values = np.unique(m)
 
     if levels is None:
         levels = unique_values
     levels = np.asarray(levels)
 
     check_increasing_and_unique(levels)
 
     if levels.size > 9 and not suppress_warnings:
-        raise ValueError("Number of levels above 9, this creates issues with visibility. This error can be suppressed"
+        raise ValueError("float of levels above 9, this creates issues with visibility. This error can be suppressed"
                          "by setting suppress_warnings to True. Be aware that the default colormap will cause "
                          "issues")
 
     if cmap is None:
         cmap = plt.get_cmap()
     else:
         cmap = plt.get_cmap(cmap)
@@ -37,8 +37,8 @@
     boundaries = np.hstack((levels[0] - 1, (levels[1:] + levels[:-1]) / 2, levels[-1] + 1))
     norm = BoundaryNorm(boundaries, len(levels))
     cmap = ListedColormap(colors)
 
     if nan_color is not None:
         cmap.set_bad(nan_color)
 
-    return cmap, norm
+    return cmap, norm, levels
```

### Comparing `geomappy-0.0.5/geomappy/colors.py` & `geomappy-0.0.6/geomappy/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 """
 The functions here implement shortcuts to create different sort of colors/cmap instances for different scenarios. It
 also contains a convenient function to add a colorbar that has the right size for the plots.
 """
 import colorsys
 from typing import Iterable, Union, Optional
 
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
-from matplotlib.colorbar import ColorbarBase
-from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap, to_rgba_array, BoundaryNorm, to_rgba
-
-from geomappy.types import ColorOrMap, Color
+from matplotlib.colorbar import ColorbarBase  # type: ignore
+from matplotlib.colors import (  # type: ignore
+    Colormap, LinearSegmentedColormap, ListedColormap, to_rgba_array, BoundaryNorm, to_rgba
+)  # type: ignore
+from geomappy.types import Color
 from geomappy.utils import _grid_from_corners
 
 
-def plot_colors(c: ColorOrMap, ticks: bool = False):
+def plot_colors(c: Union[Color, Colormap], ticks: bool = False):
     """
     Plot a horizontal colorbar to inspect colors
 
     Parameters
     ----------
     c : array-like or Colormap instance
         Iterable containing matplotlib interpretable colors, matplotlib cmap, or str indicating the cmap.
@@ -70,15 +71,15 @@
     alpha : float, optional
         Value between 0 and 1. Default is 0.
     plotting : bool, optional
         Plotting cmap. Default is False
     diverging : bool, optional
         Apply whitening kernel causing the centre of the cmap to be white if v is left to None. Default is False.
     diverging_alpha : float, optional
-        The central RGB components are raised with this number. The default is 0.5, which is also the maximum, and will
+        The central RGB components are raised with this float. The default is 0.5, which is also the maximum, and will
         lead to white as the central colors. The minimum is -0.5 which will lead to black as the central color.
     rotate : int, optional
         Rotate the created array clockwise. The default is zero. Options are 1, 2 or 3 which will lead to 90, 180 or 270
         degrees rotation.
     flip : bool, optional
         Flip the array left to right. Default is False.
     ax : `plt.Axes`, optional
@@ -156,15 +157,15 @@
     Returns n sampled colors from Colormap
 
     Parameters
     ----------
     cmap : str or Colormap, optional
         Name of cmap (or cmap itself). If `cmap` is a string it needs to be available in the matplotlib namespace
     n : int
-        Number of colors
+        float of colors
     """
     if isinstance(cmap, str):
         cmap = plt.get_cmap(cmap)
 
     return cmap(np.linspace(0, 1, n))
 
 
@@ -173,15 +174,15 @@
     Returns a resampled colormap
 
     Parameters
     ----------
     cmap : str or Colormap, optional
         Name of cmap (or cmap itself). If `cmap` is a string it needs to be available in the matplotlib namespace
     n : int
-        Number of colors
+        float of colors
     """
     if isinstance(cmap, str):
         cmap = plt.get_cmap(cmap)
 
     return cmap.resampled(n)
 
 
@@ -206,15 +207,15 @@
                   last_color: Optional[Color] = None) -> np.ndarray:
     """
     Creates random RGBA colors
 
     Parameters
     ----------
     n : int
-        Number of labels (size of colormap)
+        float of labels (size of colormap)
     color_type : {"bright","pastel"}
         'bright' for strong colors, 'soft' for pastel colors, which is the default behaviour
     first_color : str, optional
         Option to set first color if necessary
     last_color : str, optional
         Option to set last color if necessary
 
@@ -260,15 +261,15 @@
                 last_color: Optional[Color] = None) -> Colormap:
     """
     Creates a random Colormap object
 
     Parameters
     ----------
     n : int
-        Number of labels (size of colormap)
+        float of labels (size of colormap)
     color_type : {"bright","pastel"}
         'bright' for strong colors, 'soft' for pastel colors, which is the default behaviour
     first_color : str, optional
         Option to set first color if necessary
     last_color : str, optional
         Option to set last color if necessary
```

### Comparing `geomappy-0.0.5/geomappy/geodataframe.py` & `geomappy-0.0.6/geomappy/geodataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Optional, Union, Tuple
 
-import cartopy.crs as ccrs
-import geopandas as gpd
-from cartopy.mpl.geoaxes import GeoAxes
-from matplotlib import pyplot as plt
+import cartopy.crs as ccrs  # type: ignore
+import geopandas as gpd  # type: ignore
+from cartopy.mpl.geoaxes import GeoAxes  # type: ignore
+from matplotlib import pyplot as plt  # type: ignore
 
 from geomappy.basemap import basemap as basemap_function, add_gridlines, add_ticks
 from geomappy.shapes import plot_shapes, plot_classified_shapes
-from geomappy.types import Number, OptionalLegend
+from geomappy.types import LegendOrColorbar
 from geomappy.utils import add_method, change_between_bounds_and_extent
 from geomappy.world import plot_world
 
 
 def _plot_combined_shapes(classified, df, *,
                           figsize: Tuple[int, int] = (8, 8), ax: Optional[plt.Axes] = None, basemap: bool = True,
-                          lines: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
-                          ticks: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
-                          fontsize: int = 10, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                          lines: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]] = 30,
+                          ticks: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]] = 30,
+                          fontsize: int = 10, **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     if isinstance(ax, GeoAxes):
         basemap = True
 
     if basemap:
         projection = df.get_cartopy_projection()
         ax = basemap_function(ax=ax, projection=projection, figsize=figsize)
         ax.set_extent(df.get_extent(), crs=projection)
@@ -74,15 +74,15 @@
     lines : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two gridlines in lat-lon terms. The default 30
         means that every 30 degrees a gridline gets drawn. See add_gridlines
     ticks : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two tick labels in lat-lon terms. The default 30
         means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
-        fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
+        fontsize for both the lon/lat ticks and the ticks on the colorbar if one float, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
     kwargs
         kwargs going to the plot_classified_shapes() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
@@ -115,15 +115,15 @@
     lines : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two gridlines in lat-lon terms. The default 30
         means that every 30 degrees a gridline gets drawn. See add_gridlines
     ticks : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two tick labels in lat-lon terms. The default 30
         means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
-        fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
+        fontsize for both the lon/lat ticks and the ticks on the colorbar if one float, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
     kwargs
         kwargs going to the plot_classified_shapes() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
@@ -147,15 +147,15 @@
     Plots the outer bounds of a GeoDataFrame on a world map.
 
     Parameters
     ----------
     ax : :obj:`~matplotlib.axes.Axes`, optional
         Axes on which to plot the figure
     extent : list, optional
-        Takes a four number list, or rasterio bounds object. It constrains the world view
+        Takes a four float list, or rasterio bounds object. It constrains the world view
         to a specific view. If not lat-lon, the extent_projection needs to be specified
     extent_projection: cartopy.CRS
         Projection of the extent. The default ccrs.PlateCarree().
     projection : cartopy.CRS
         Projection of the plot. The default ccrs.PlateCarree().
     kwargs
         arguments for the Basemap function
```

### Comparing `geomappy-0.0.5/geomappy/legends.py` & `geomappy-0.0.6/geomappy/legends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Optional, Tuple, Union
+from typing import Optional, Tuple, TypeVar
 
+import matplotlib  # type: ignore
 import numpy as np
-import matplotlib
-from matplotlib import pyplot as plt
-from matplotlib.cm import ScalarMappable
-from matplotlib.colorbar import Colorbar
-from matplotlib.colors import BoundaryNorm, Normalize, Colormap
+from matplotlib import pyplot as plt  # type: ignore
+from matplotlib.cm import ScalarMappable  # type: ignore
+from matplotlib.colorbar import Colorbar  # type: ignore
+from matplotlib.colors import BoundaryNorm, Normalize, Colormap  # type: ignore
 
 from geomappy.axes_decoration import legend_patches, add_colorbar
-from geomappy.types import Number
+
+Labels = TypeVar("Labels", Tuple[float, ...], Tuple[str, ...], np.ndarray)
 
 
 def no_legend(*args, **kwargs) -> None:
     pass
 
 
 def add_legend_patches_scalar(ax: plt.Axes, norm: Normalize, cmap: Colormap, **kwargs) -> matplotlib.legend.Legend:
@@ -37,53 +38,54 @@
 
 
 def add_colorbar_scalar(ax: plt.Axes, norm: Normalize, cmap: Colormap, **kwargs) -> Colorbar:
     im = ScalarMappable(norm, cmap)
     return add_colorbar(ax=ax, im=im, **kwargs)
 
 
-def add_legend_patches_classified(ax: plt.Axes, labels: Optional[Tuple[Union[Number, str]]], norm: BoundaryNorm,
-                                  cmap: Colormap, **kwargs) -> matplotlib.legend.Legend:
+def add_legend_patches_classified(ax: plt.Axes, labels: Optional[Labels], norm: BoundaryNorm, cmap: Colormap,
+                                  **kwargs) -> matplotlib.legend.Legend:
     if not isinstance(norm, BoundaryNorm):
         TypeError("Can only plot classified patches with BoundaryNorm")
 
     bins = norm.boundaries[:-1]
     if labels is None:
         labels = bins
     colors = cmap(norm(bins))
     handles = legend_patches(colors, labels)
     return ax.legend(handles=handles, **kwargs)
 
 
-def add_colorbar_classified(ax: plt.Axes, labels: Optional[Tuple[Union[Number, str]]], norm: BoundaryNorm,
-                            cmap: Colormap, **kwargs) -> Colorbar:
+def add_colorbar_classified(ax: plt.Axes, labels: Optional[Labels],
+                            norm: BoundaryNorm, cmap: Colormap, **kwargs) -> Colorbar:
     if not isinstance(norm, BoundaryNorm):
         TypeError("Can only plot classified colorbar with BoundaryNorm")
 
     im = ScalarMappable(norm, cmap)
 
     l = add_colorbar(ax=ax, im=im, extend='neither', **kwargs)
     xs = (norm.boundaries[:-1] + norm.boundaries[1:]) / 2
     if labels is None:
         labels = norm.boundaries[:-1]
     l.set_ticks(xs, labels=labels)
     return l
 
 
-SCALAR_LEGENDS = {None: no_legend,
-                  "legend": add_legend_patches_scalar,
+SCALAR_LEGENDS = {"legend": add_legend_patches_scalar,
                   "colorbar": add_colorbar_scalar}
 
-CLASSIFIED_LEGENDS = {None: no_legend,
-                      "legend": add_legend_patches_classified,
+CLASSIFIED_LEGENDS = {"legend": add_legend_patches_classified,
                       "colorbar": add_colorbar_classified}
 
+LEGENDS = {
+    'scalar': SCALAR_LEGENDS,
+    'classified': CLASSIFIED_LEGENDS,
+}
+EMPTY_DICT = {None: no_legend}
 
-def add_legend(t: str, legend: Optional[str], *, ax: plt.Axes, **kwargs):
-    if t == 'scalar':
-        d = SCALAR_LEGENDS
-    elif t == 'classified':
-        d = CLASSIFIED_LEGENDS
-    else:
-        raise ValueError
 
-    return d.get(legend)(ax=ax, **kwargs)
+def add_legend(t: str, legend: Optional[str], *, ax: plt.Axes, **kwargs):
+    return (
+        LEGENDS
+        .get(t, EMPTY_DICT)
+        .get(legend, no_legend)(ax=ax, **kwargs)
+    )
```

### Comparing `geomappy-0.0.5/geomappy/raster.py` & `geomappy-0.0.6/geomappy/raster.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import Tuple, Optional, Dict, Union, Iterable
+from typing import Tuple, Optional, Dict, Union, Sequence
 
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
-from matplotlib.colors import Colormap, Normalize
+from matplotlib.colors import Colormap, Normalize  # type: ignore
 
 from geomappy.axes_decoration import prepare_axes
 from geomappy.classified import parse_classified_plot_params
 from geomappy.legends import add_legend
 from geomappy.scalar import parse_scalar_plot_params
-from geomappy.types import Color, Number, OptionalLegend
+from geomappy.types import Color, LegendOrColorbar
 
 
-def plot_classified_raster(m: np.ndarray, *, levels: Optional[Tuple[Number]] = None,
-                           colors: Optional[Tuple[Color]] = None, labels: Optional[Tuple[Union[Number, str]]] = None,
+def plot_classified_raster(m: np.ndarray, *, levels: Optional[Union[Tuple[float, ...], np.ndarray]] = None,
+                           colors: Optional[Union[Tuple[Color, ...], np.ndarray]] = None,
+                           labels: Optional[Union[Tuple[float, ...], Tuple[str, ...], np.ndarray]] = None,
                            cmap: Union[str, Colormap] = "Set1", nan_color: Optional[Color] = None,
                            suppress_warnings: bool = False, ax: Optional[plt.Axes] = None,
                            figsize: Optional[Tuple[int, int]] = None, legend: Optional[str] = "colorbar",
-                           legend_kw: Optional[Dict] = None, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                           legend_kw: Optional[Dict] = None, **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     """"Plot a classified raster
 
     Parameters
     ----------
 
     m : array-like
         Input array. Needs to be 2D
@@ -57,42 +58,41 @@
     Returns
     -------
 
     """
     if m.ndim != 2:
         raise ValueError("Input data needs to be 2D if plotting classified data")
 
-    if not isinstance(m, np.ma.MaskedArray):
-        m = np.ma.fix_invalid(m)
+    m_masked = np.ma.fix_invalid(m)
 
-    cmap, norm = parse_classified_plot_params(m, levels=levels, colors=colors, cmap=cmap, nan_color=nan_color,
-                                              suppress_warnings=suppress_warnings)
+    cmap, norm, levels_parsed = parse_classified_plot_params(m_masked, levels=levels, colors=colors, cmap=cmap,
+                                                             nan_color=nan_color, suppress_warnings=suppress_warnings)
 
     ax = prepare_axes(ax, figsize)
-    ax.imshow(m, cmap=cmap, norm=norm, **kwargs)
+    ax.imshow(m_masked, cmap=cmap, norm=norm, **kwargs)
 
     if legend_kw is None:
         legend_kw = {}
 
     if labels is None and levels is None:
         labels = np.unique(m)
     elif labels is None:
-        labels = levels
+        labels = levels_parsed
 
     l = add_legend('classified', legend, ax=ax, labels=labels, norm=norm, cmap=cmap, **legend_kw)
 
     return ax, l
 
 
-def plot_raster(m: np.ndarray, *, bins: Optional[Union[Iterable, np.ndarray]] = None,
+def plot_raster(m: np.ndarray, *, bins: Optional[Union[Sequence, np.ndarray]] = None,
                 cmap: Optional[Union[str, Colormap]] = None, norm: Optional[Normalize] = None,
                 ax: Optional[plt.Axes] = None, vmin: Optional[float] = None, vmax: Optional[float] = None,
                 figsize: Optional[Tuple[int, int]] = None, nan_color: Optional[Color] = None,
                 legend: Optional[str] = "colorbar", legend_kw: Optional[Dict] = None,
-                **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     """
     Plot a scalar raster
 
     Parameters
     ----------
     m : array-like
         Input array. Needs to be either 2D or 3D if the third axis contains RGB(A) information
@@ -131,32 +131,31 @@
     """
     if m.ndim not in (2, 3):
         raise ValueError("Input data needs to be 2D or present RGB(A) values on the third axis.")
     if m.ndim == 3 and (m.shape[-1] not in (3, 4) or np.issubdtype(m.dtype, np.bool_)):
         raise ValueError(f"3D arrays are only acceptable if presenting RGB(A) information. It does not work with "
                          f"boolean variables.\nShape: {m.shape} \ndtype: {m.dtype}")
 
-    if not isinstance(m, np.ma.MaskedArray):
-        m = np.ma.fix_invalid(m)
+    m_masked = np.ma.fix_invalid(m)
 
     if bins is not None and len(bins) == 1:
-        m = m > bins[0]
+        m_masked = m_masked > bins[0]
 
-    if np.issubdtype(m.dtype, np.bool_):
-        return plot_classified_raster(m, colors=("Lightgrey", "Red"), legend=legend, labels=["False", "True"], ax=ax,
-                                      figsize=figsize, legend_kw=legend_kw, nan_color=nan_color, **kwargs)
+    if np.issubdtype(m_masked.dtype, np.bool_):
+        return plot_classified_raster(m_masked, colors=("Lightgrey", "Red"), legend=legend, labels=("False", "True"),
+                                      ax=ax, figsize=figsize, legend_kw=legend_kw, nan_color=nan_color, **kwargs)
 
-    if m.ndim == 3:
+    if m_masked.ndim == 3:
         cmap = None
         norm = None
     else:
-        cmap, norm = parse_scalar_plot_params(m, cmap=cmap, bins=bins, vmin=vmin, vmax=vmax, norm=norm,
+        cmap, norm = parse_scalar_plot_params(m_masked, cmap=cmap, bins=bins, vmin=vmin, vmax=vmax, norm=norm,
                                               nan_color=nan_color)
 
     ax = prepare_axes(ax, figsize)
-    ax.imshow(m, cmap=cmap, norm=norm, **kwargs)
+    ax.imshow(m_masked, cmap=cmap, norm=norm, **kwargs)
 
     if legend_kw is None:
         legend_kw = {}
     l = add_legend('scalar', legend, ax=ax, norm=norm, cmap=cmap, **legend_kw)
 
     return ax, l
```

### Comparing `geomappy-0.0.5/geomappy/scalar.py` & `geomappy-0.0.6/geomappy/scalar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple, Iterable
 
 import numpy as np
-from matplotlib import pyplot as plt
-from matplotlib.colors import Colormap, Normalize, BoundaryNorm
+from matplotlib import pyplot as plt  # type: ignore
+from matplotlib.colors import Colormap, Normalize, BoundaryNorm  # type: ignore
 from numpy.ma.core import MaskedConstant
 
 from geomappy.types import Color
 from geomappy.utils import check_increasing_and_unique
 
 
 def _define_extend(vmin: float, minimum: float, vmax: float, maximum: float) -> str:
```

### Comparing `geomappy-0.0.5/geomappy/shapes.py` & `geomappy-0.0.6/geomappy/shapes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,85 @@
 from typing import Union, Optional, Tuple, Dict
 
-import cartopy.crs as ccrs
-import geopandas as gpd
+import cartopy.crs as ccrs  # type: ignore
+import geopandas as gpd  # type: ignore
 import numpy as np
-from cartopy.mpl.geoaxes import GeoAxes
+from cartopy.mpl.geoaxes import GeoAxes  # type: ignore
 from geopandas import GeoDataFrame, GeoSeries
-from geopandas.plotting import _plot_polygon_collection, _plot_linestring_collection, _plot_point_collection
-from matplotlib import pyplot as plt
-from matplotlib.colors import Normalize, Colormap
-from shapely.geometry import Point
+from geopandas.plotting import (  # type: ignore
+    _plot_polygon_collection, _plot_linestring_collection, _plot_point_collection
+)
+from matplotlib import pyplot as plt  # type: ignore
+from matplotlib.colors import Normalize, Colormap  # type: ignore
+from shapely.geometry import Point  # type: ignore
 
 from geomappy.axes_decoration import prepare_axes
 from geomappy.classified import parse_classified_plot_params
 from geomappy.legends import add_legend
 from geomappy.scalar import parse_scalar_plot_params
-from geomappy.types import Number, Color, OptionalLegend
+from geomappy.types import Color, LegendOrColorbar
 
 
 def _create_geometries_and_values_from_lat_lon(lat: Optional[np.ndarray] = None,
                                                lon: Optional[np.ndarray] = None,
-                                               values: Optional[np.ndarray] = None,
-                                               s: Optional[Union[Number, np.ndarray]] = None) \
+                                               values: Optional[Union[np.ndarray, str, float]] = None,
+                                               s: Optional[Union[float, np.ndarray]] = None) \
         -> Tuple[GeoSeries, np.ndarray, Optional[np.ndarray]]:
     lon = np.asarray(lon)
     lat = np.asarray(lat)
+
+    if isinstance(values, str):
+        raise TypeError("When no dataframe is provided, values need to be either numeric or an array")
+
     values = np.asarray(values)
 
     if lon.size != lat.size:
         raise IndexError("Mismatch in length of `lat` and `lon`")
 
     if s is None:
         markersize = None
     else:
         markersize = np.asarray(s)
 
     geometry = gpd.GeoSeries([Point(lon[i], lat[i]) for i in range(len(lon))])
     return geometry, values, markersize
 
 
-def _create_geometries_and_values_from_gdf(values: Optional[Union[str, Number, np.ndarray]] = None,
-                                           s: Optional[Union[Number, np.ndarray]] = None,
-                                           df: Optional[Union[GeoDataFrame, GeoSeries]] = None) \
+def _create_geometries_and_values_from_gdf(values: Optional[Union[str, float, np.ndarray]] = None,
+                                           s: Optional[Union[float, np.ndarray]] = None,
+                                           df: Union[GeoDataFrame, GeoSeries] = None) \
         -> Tuple[GeoSeries, np.ndarray, Optional[np.ndarray]]:
     geometry = df['geometry']
     if isinstance(values, str):
+        if df is None:
+            raise ValueError("Values str refers to dataframe, which is not provided")
         if values not in df.columns:
             raise ValueError("values are not present in dataframe")
         values = df.loc[:, values].values
     else:
-        values = np.array(values).flatten()
+        values = np.asarray(values).flatten()
+
+    markersize: Optional[np.ndarray]
 
     if s is None:
         markersize = None
     elif isinstance(s, str):
         markersize = None
         if s in df.columns:
             markersize = df.loc[:, s].values
     else:
         markersize = np.array(s).flatten()
 
-    return geometry, values, markersize
+    return geometry, np.ma.fix_invalid(values), markersize
 
 
 def _create_geometry_values_and_sizes(lat: Optional[np.ndarray] = None,
                                       lon: Optional[np.ndarray] = None,
-                                      values: Optional[Union[str, Number, np.ndarray]] = None,
-                                      s: Optional[Union[Number, np.ndarray]] = None,
+                                      values: Optional[Union[str, float, np.ndarray]] = None,
+                                      s: Optional[Union[float, np.ndarray]] = None,
                                       df: Optional[Union[GeoDataFrame, GeoSeries]] = None) \
         -> Tuple[GeoSeries, np.ma.MaskedArray, Optional[np.ndarray]]:
     """
     Function that deals with the input data for `plot_shapes` and `plot_classified_shapes`. Lat and Lon will be used
     if `df` is not given. `Values` and `s` will be cast to the length of the geometries, or set to 1 and None
     respectively if not provided.
 
@@ -100,31 +110,31 @@
         if values[0] is None or values[0] == np.nan:
             values = np.array(1)
         values = values.repeat(geometry.size)
 
     if values.size != geometry.size:
         raise IndexError("Mismatch length sizes and geometries")
 
+    markersize_parsed: Optional[np.ndarray] = None
     if markersize is not None:
         if markersize.size == 1:
             if markersize[0] is None:
-                markersize = None
+                markersize_parsed = None
             else:
-                markersize = markersize.repeat(geometry.size)
+                markersize_parsed = markersize.repeat(geometry.size)
 
-        if markersize.size != geometry.size:
+        elif markersize.size != geometry.size:
             raise IndexError("Mismatch length of `s` and coordindates")
 
-    values = np.ma.fix_invalid(values)
-
-    return geometry, values, markersize
+    return geometry, np.ma.fix_invalid(values), markersize_parsed
 
 
-def _plot_geometries(ax: plt.Axes, geometries: GeoSeries, colors: np.ndarray, linewidth: float,
-                     markersize: Union[float, np.ndarray], **kwargs) -> None:
+def _plot_geometries(ax: plt.Axes, geometries: GeoSeries, colors: Union[np.ndarray, Tuple[Color, ...]],
+                     linewidth: float,
+                     markersize: Optional[Union[float, np.ndarray]], **kwargs) -> None:
     """
     internal plotting function for geometries, called by plot_shapes and plot_classified_shapes
 
     Parameters
     ----------
     ax : matplotlib.Axes
         axes to plot on
@@ -177,28 +187,28 @@
             markersize = markersize[point_idx]
         _plot_point_collection(ax, points, facecolor=facecolor[point_idx], edgecolor=edgecolor[point_idx],
                                markersize=markersize, linewidth=linewidth, **kwargs)
 
 
 def plot_classified_shapes(lat: Optional[np.ndarray] = None,
                            lon: Optional[np.ndarray] = None,
-                           values: Optional[Union[str, Number, np.ndarray]] = None,
-                           s: Optional[Union[Number, np.ndarray]] = None,
+                           values: Optional[Union[str, float, np.ndarray]] = None,
+                           s: Optional[Union[float, np.ndarray]] = None,
                            df: Optional[Union[GeoDataFrame, GeoSeries]] = None,
-                           levels: Optional[Tuple[Number]] = None,
-                           colors: Optional[Tuple[Color]] = None,
+                           levels: Optional[Tuple[float, ...]] = None,
+                           colors: Optional[Tuple[Color, ...]] = None,
                            cmap: Union[str, Colormap] = "Set1",
-                           labels: Optional[Tuple[str]] = None,
+                           labels: Optional[Tuple[str, ...]] = None,
                            legend: Optional[str] = "colorbar",
                            ax: Optional[plt.Axes] = None,
                            figsize: Optional[Tuple[int, int]] = None,
                            suppress_warnings: bool = False,
                            legend_kw: Optional[Dict] = None,
-                           linewidth: Number = 1,
-                           nan_color: Optional[Color] = None, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                           linewidth: float = 1,
+                           nan_color: Optional[Color] = None, **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     """
     Plot shapes with discrete classes or index
 
     Parameters
     ----------
     lat, lon : array-like
         Latitude and Longitude
@@ -259,50 +269,50 @@
         legend = None
 
     if isinstance(ax, GeoAxes):
         if 'transform' not in kwargs:
             kwargs["transform"] = ccrs.PlateCarree()
 
     geometry, values, markersize = _create_geometry_values_and_sizes(lat, lon, values, s, df)
-    cmap, norm = parse_classified_plot_params(values, levels=levels, colors=colors, cmap=cmap, nan_color=nan_color,
-                                              suppress_warnings=suppress_warnings)
+    cmap, norm, parsed_levels = parse_classified_plot_params(values, levels=levels, colors=colors, cmap=cmap,
+                                                             nan_color=nan_color, suppress_warnings=suppress_warnings)
 
-    colors = cmap(norm(values))
+    colors_parsed = cmap(norm(values))
     ax = prepare_axes(ax, figsize)
-    _plot_geometries(ax, geometry, colors, linewidth, markersize, **kwargs)
+    _plot_geometries(ax, geometry, colors_parsed, linewidth, markersize, **kwargs)
 
     if legend_kw is None:
         legend_kw = {}
 
     if labels is None and levels is None:
         labels = np.unique(values)
     elif labels is None:
-        labels = levels
+        labels = tuple(str(l) for l in parsed_levels)
 
     l = add_legend('classified', legend, ax=ax, labels=labels, norm=norm, cmap=cmap, **legend_kw)
 
     return ax, l
 
 
 def plot_shapes(lat: Optional[np.ndarray] = None,
                 lon: Optional[np.ndarray] = None,
-                values: Optional[Union[str, Number, np.ndarray]] = None,
-                s: Optional[Union[Number, np.ndarray]] = None,
+                values: Optional[Union[str, float, np.ndarray]] = None,
+                s: Optional[Union[float, np.ndarray]] = None,
                 df: Optional[Union[GeoDataFrame, GeoSeries]] = None,
-                bins: Optional[Tuple[Number]] = None,
+                bins: Optional[Tuple[float]] = None,
                 cmap: Optional[Colormap] = None,
                 norm: Optional[Normalize] = None,
                 vmin: Optional[float] = None,
                 vmax: Optional[float] = None,
                 ax: Optional[plt.Axes] = None,
                 legend: Optional[str] = "colorbar",
                 figsize: Optional[Tuple[int, int]] = None,
                 legend_kw: Optional[Dict] = None,
                 linewidth: float = 1,
-                nan_color: Optional[Color] = None, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                nan_color: Optional[Color] = None, **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     """
     Plot shapes in a continuous fashion
 
     Parameters
     ----------
     lat, lon : array-like
         Latitude and Longitude
@@ -363,28 +373,28 @@
             kwargs['edgecolor'] = "black"
         legend = None
 
     if isinstance(ax, GeoAxes):
         if 'transform' not in kwargs:
             kwargs["transform"] = ccrs.PlateCarree()
 
-    geometry, values, markersize = _create_geometry_values_and_sizes(lat, lon, values, s, df)
+    geometry, values_parsed, markersize = _create_geometry_values_and_sizes(lat, lon, values, s, df)
 
     if bins is not None and len(bins) == 1:
         # If only one bin is present the data will be converted to a boolean array
-        values = values > bins[0]
+        values_parsed = values_parsed > bins[0]
 
-    if np.issubdtype(values.dtype, np.bool_):
+    if np.issubdtype(values_parsed.dtype, np.bool_):
         plot_classified_shapes(lat, lon, values, s, df, labels=("False", "True"), colors=("Lightgrey", "Red"), ax=ax,
                                figsize=figsize, legend=legend, legend_kw=legend_kw, linewidth=linewidth,
                                nan_color=nan_color, **kwargs)
 
-    cmap, norm = parse_scalar_plot_params(values, cmap=cmap, bins=bins, vmin=vmin, vmax=vmax, norm=norm,
+    cmap, norm = parse_scalar_plot_params(values_parsed, cmap=cmap, bins=bins, vmin=vmin, vmax=vmax, norm=norm,
                                           nan_color=nan_color)
-    colors = cmap(norm(values))
+    colors = cmap(norm(values_parsed))
     ax = prepare_axes(ax, figsize)
     _plot_geometries(ax, geometry, colors, linewidth, markersize, **kwargs)
 
     if legend_kw is None:
         legend_kw = {}
     l = add_legend('scalar', legend, ax=ax, norm=norm, cmap=cmap, **legend_kw)
```

### Comparing `geomappy-0.0.5/geomappy/utils.py` & `geomappy-0.0.6/geomappy/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Utilities used in geomappy. Interesting functions to use outside the internal scope are
 progress_bar and reproject_map_like
 """
 from functools import wraps
-from numbers import Number
 from typing import Tuple, Union
 
 import numpy as np
 from numpy import ndarray
-from rasterio.coords import BoundingBox
+from rasterio.coords import BoundingBox  # type: ignore
 
 
-def _grid_from_corners(v: Tuple[Union[Number, ndarray]], shape: Tuple[int, int]):
+def _grid_from_corners(v: Tuple[Union[float, ndarray], ...], shape: Tuple[int, int]):
     """
     function returns an linearly interpolated grid from values at the corners
 
     Parameters
     ----------
     v : tuple
         List of four numeric values that will be interpolated. Order of the values is clockwise; starting from the upper
@@ -65,9 +64,9 @@
 
 def check_increasing_and_unique(v: np.ndarray) -> None:
     vs = np.sort(np.unique(v))
     if not np.array_equal(v, vs):
         raise ValueError("Levels are not sorted or contain double entries")
 
 
-def change_between_bounds_and_extent(x: Union[BoundingBox, Tuple[Number, Number, Number, Number]]):
-    return x[0], x[2], x[1], x[3]
+def change_between_bounds_and_extent(x: Union[BoundingBox, Tuple[float, float, float, float]]):
+    return x[0], x[2], x[1], x[3]
```

### Comparing `geomappy-0.0.5/geomappy/world.py` & `geomappy-0.0.6/geomappy/world.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from typing import Tuple, Optional, Union
 
-import cartopy.crs as ccrs
-from cartopy.mpl.geoaxes import GeoAxes
-from matplotlib import pyplot as plt
-from rasterio.coords import BoundingBox
+import cartopy.crs as ccrs  # type: ignore
+from cartopy.mpl.geoaxes import GeoAxes  # type: ignore
+from matplotlib import pyplot as plt  # type: ignore
+from rasterio.coords import BoundingBox  # type: ignore
 
 from geomappy.basemap import basemap, add_gridlines, add_ticks
 from geomappy.bounds import bounds_to_polygons
-from geomappy.types import Number
 
 
-def plot_world(bounds: Union[Tuple[Number, Number, Number, Number]], ax: Optional[plt.Axes] = None,
-               extent: Union[Tuple[Number, Number, Number, Number], str] = 'global',
+def plot_world(bounds: Union[Tuple[float, float, float, float]], ax: Optional[plt.Axes] = None,
+               extent: Union[Tuple[float, float, float, float], str] = 'global',
                projection: ccrs.Projection = ccrs.PlateCarree(),
                extent_projection: ccrs.Projection = ccrs.PlateCarree(),
                bounds_projection: ccrs.Projection = ccrs.PlateCarree(),
                **kwargs) -> GeoAxes:
     """
     Plots the outer bounds on a world map
 
     Parameters
     ----------
     bounds: list of int
         Bounds to be plotted on the map
     ax : :obj:`~matplotlib.axes.Axes`, optional
         Axes on which to plot the figure
     extent : list, optional
-        Takes a four number list, or rasterio bounds object. It constrains the world view
+        Takes a four float list, or rasterio bounds object. It constrains the world view
         to a specific view. If not lat-lon, the extent_projection needs to be specified
     extent_projection: cartopy.CRS
         Projection of the extent and bounds. The default ccrs.PlateCarree().
     projection : cartopy.CRS
         Projection of the plot. The default ccrs.PlateCarree().
     kwargs
         Arguments for the Basemap function
```

### Comparing `geomappy-0.0.5/geomappy/xarray.py` & `geomappy-0.0.6/geomappy/xarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Optional, Union, Tuple
 
-import cartopy.crs as ccrs
+import cartopy.crs as ccrs  # type: ignore
 import xarray as xr
-from cartopy.mpl.geoaxes import GeoAxes
-from matplotlib import pyplot as plt
+from cartopy.mpl.geoaxes import GeoAxes  # type: ignore
+from matplotlib import pyplot as plt  # type: ignore
 
 from geomappy.basemap import basemap as basemap_function, add_gridlines, add_ticks
 from geomappy.raster import plot_classified_raster, plot_raster
-from geomappy.types import Number, OptionalLegend
+from geomappy.types import LegendOrColorbar
 from geomappy.utils import add_method, change_between_bounds_and_extent
 from geomappy.world import plot_world
 
 
 def _plot_combined_raster(classified: bool, *, da: xr.DataArray, basemap: bool = True,
                           figsize: Tuple[int, int] = (8, 8), ax: Optional[plt.Axes] = None,
-                          lines: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
-                          ticks: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
-                          coastlines: bool = True, fontsize: int = 10, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+                          lines: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]] = 30,
+                          ticks: Union[float, Tuple[float, float], Tuple[Tuple[float], Tuple[float]]] = 30,
+                          decorate_basemap: bool = True, fontsize: int = 10,
+                          **kwargs) -> Tuple[plt.Axes, Optional[LegendOrColorbar]]:
     if da.ndim == 3 and da.shape[0] == 1:
         da = da[0]
 
     if da.ndim != 2:
         raise IndexError("Only 2 or 3 dimensional DataArrays are accepted")
 
     if isinstance(ax, GeoAxes):
@@ -29,21 +30,21 @@
     if basemap:
         if isinstance(ax, GeoAxes):
             projection = ax.projection
         else:
             projection = da.get_cartopy_projection()
 
         ax = basemap_function(ax=ax, projection=projection, figsize=figsize)
-        ax.set_extent(da.get_extent(), crs=da.get_cartopy_projection())
+        ax.set_extent(da.get_extent(), crs=projection)
 
-        if coastlines:
+        if decorate_basemap:
             ax.coastlines()
+            add_gridlines(ax, lines)
+            add_ticks(ax, ticks, fontsize=fontsize)
 
-        add_gridlines(ax, lines)
-        add_ticks(ax, ticks, fontsize=fontsize)
         kwargs['extent'] = da.get_extent()
         kwargs['transform'] = projection
 
     a = da.to_masked_array()
 
     if classified:
         return plot_classified_raster(a, ax=ax, figsize=figsize, **kwargs)
@@ -92,15 +93,15 @@
     lines : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two gridlines in lat-lon terms. The default 30
         means that every 30 degrees a gridline gets drawn. See add_gridlines
     ticks : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two tick labels in lat-lon terms. The default 30
         means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
-        fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
+        fontsize for both the lon/lat ticks and the ticks on the colorbar if one float, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
     kwargs
         kwargs going to the plot_classified_raster() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
@@ -133,15 +134,15 @@
     lines : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two gridlines in lat-lon terms. The default 30
         means that every 30 degrees a gridline gets drawn. See add_gridlines
     ticks : int, tuple of ints, or tuple of tuples of ints, optional
         parameter that describes the distance between two tick labels in lat-lon terms. The default 30
         means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
-        fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
+        fontsize for both the lon/lat ticks and the ticks on the colorbar if one float, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
     kwargs
         kwargs going to the plot_classified_raster() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
@@ -163,15 +164,15 @@
     Plots the outer bounds of a DataArray on a world map.
 
     Parameters
     ----------
     ax : :obj:`~matplotlib.axes.Axes`, optional
         Axes on which to plot the figure
     extent : list, optional
-        Takes a four number list, or rasterio bounds object. It constrains the world view
+        Takes a four float list, or rasterio bounds object. It constrains the world view
         to a specific view. If not lat-lon, the extent_projection needs to be specified
     extent_projection: cartopy.CRS
         Projection of the extent. The default ccrs.PlateCarree().
     projection : cartopy.CRS
         Projection of the plot. The default ccrs.PlateCarree().
     kwargs
         arguments for the Basemap function
```

### Comparing `geomappy-0.0.5/geomappy.egg-info/SOURCES.txt` & `geomappy-0.0.6/geomappy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 geomappy/world.py
 geomappy/xarray.py
 geomappy.egg-info/PKG-INFO
 geomappy.egg-info/SOURCES.txt
 geomappy.egg-info/dependency_links.txt
 geomappy.egg-info/requires.txt
 geomappy.egg-info/top_level.txt
-tests/test_plotting.py
+tests/test_classified_params.py
+tests/test_plotting.py
+tests/test_scalar_params.py
```

### Comparing `geomappy-0.0.5/tests/test_plotting.py` & `geomappy-0.0.6/tests/test_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pytest
 from matplotlib.colors import ListedColormap, from_levels_and_colors
 
 import geomappy as mp
 
 
 def imshow(*args, **kwargs):
-    f, ax = plt.subplots()
+    f, ax = plt.subplots(figsize=(8, 8))
     ax.imshow(*args, **kwargs)
     return ax
 
 
 def compare_images(ax1, ax2, tol=0):
     try:
         os.mkdir("_test_figures")
@@ -112,15 +112,15 @@
     # plt.show()
 
     # get discrete colormap
     cmap = plt.get_cmap('jet', m)
     ax2 = imshow(x, cmap=cmap, vmin=0, vmax=m - 1)
     # plt.show()
 
-    assert compare_images(ax1, ax2, tol=0.8)
+    assert compare_images(ax1, ax2, tol=1)
 
 
 def test_figure_legend_patches():
     # 3D image data
     # no legend should be plotted
     x = np.random.rand(10, 10, 3)
     with pytest.raises(TypeError):
```

