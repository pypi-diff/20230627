# Comparing `tmp/qctrl_visualizer-5.0.1.tar.gz` & `tmp/qctrl_visualizer-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_visualizer-5.0.1.tar", max compression
+gzip compressed data, was "qctrl_visualizer-6.0.0.tar", max compression
```

## Comparing `qctrl_visualizer-5.0.1.tar` & `qctrl_visualizer-6.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    36653 2023-06-05 06:19:46.075615 qctrl_visualizer-5.0.1/LICENSE
--rw-r--r--   0        0        0      755 2023-06-05 06:19:46.075615 qctrl_visualizer-5.0.1/README.md
--rw-r--r--   0        0        0     2841 2023-06-05 06:20:04.463800 qctrl_visualizer-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     2367 2023-06-05 06:20:04.471799 qctrl_visualizer-5.0.1/qctrlvisualizer/__init__.py
--rw-r--r--   0        0        0    23319 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/bloch.py
--rw-r--r--   0        0        0    13992 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/confidence_ellipses.py
--rw-r--r--   0        0        0    19934 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/controls.py
--rw-r--r--   0        0        0     4966 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/cost_histories.py
--rw-r--r--   0        0        0     7355 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/density_matrix.py
--rw-r--r--   0        0        0     8486 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/filter_functions.py
--rw-r--r--   0        0        0     6553 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/histogram.py
--rw-r--r--   0        0        0    12895 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/populations.py
--rw-r--r--   0        0        0     4147 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/style.py
--rw-r--r--   0        0        0     5525 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/utils.py
--rw-r--r--   0        0        0     5858 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/wigner_function.py
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 qctrl_visualizer-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-26 23:47:58.155482 qctrl_visualizer-6.0.0/LICENSE
+-rw-r--r--   0        0        0      755 2023-06-26 23:47:58.155482 qctrl_visualizer-6.0.0/README.md
+-rw-r--r--   0        0        0     2495 2023-06-26 23:48:20.368034 qctrl_visualizer-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2106 2023-06-26 23:48:20.380034 qctrl_visualizer-6.0.0/qctrlvisualizer/__init__.py
+-rw-r--r--   0        0        0    23319 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/bloch.py
+-rw-r--r--   0        0        0    13992 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/confidence_ellipses.py
+-rw-r--r--   0        0        0    17782 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/controls.py
+-rw-r--r--   0        0        0     4555 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/cost_histories.py
+-rw-r--r--   0        0        0     7355 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/density_matrix.py
+-rw-r--r--   0        0        0     8486 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/filter_functions.py
+-rw-r--r--   0        0        0     6553 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/histogram.py
+-rw-r--r--   0        0        0    12487 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/populations.py
+-rw-r--r--   0        0        0     4195 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/style.py
+-rw-r--r--   0        0        0     5525 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/utils.py
+-rw-r--r--   0        0        0     5858 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/wigner_function.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 qctrl_visualizer-6.0.0/PKG-INFO
```

### Comparing `qctrl_visualizer-5.0.1/LICENSE` & `qctrl_visualizer-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/README.md` & `qctrl_visualizer-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/pyproject.toml` & `qctrl_visualizer-6.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-visualizer"
-version = "5.0.1"
+version = "6.0.0"
 description = "Q-CTRL Visualizer"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -61,23 +61,23 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 matplotlib = ">=3.6.3"
 numpy = "^1.23.5"
 scipy = ">=1.9.3"
-qctrl-commons = "^18.0.0"
+qctrl-commons = "^18.1.1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
-mypy = "^1.2.0"
-pytest = "^7.3.1"
-pylint = "^2.17.1"
-pre-commit = "^3.2.2"
+mypy = "^1.3.0"
+pytest = "^7.3.2"
+pylint = "^2.17.4"
+pre-commit = "^3.3.2"
 sphinx = "^5.3.0"
 tomli = "^2.0.1"
 qctrl-sphinx-theme = "~0.1.3"
 docopt = "~0.6.2"
 
 [[tool.poetry.source]]
 name = 'Q-CTRL PyPI'
@@ -100,18 +100,7 @@
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-#  _______________________________________
-# / If you update this file, please run   \
-# | `poetry update --lock` to update the  |
-# \ file "poetry.lock".                   /
-#  --------------------------------------
-#        \   ^__^
-#         \  (oo)\_______
-#            (__)\       )\/\
-#                ||----w |
-#                ||     ||
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/__init__.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,46 +14,35 @@
 """
 Top-level package for the Q-CTRL Visualizer.
 
 The public API of this package consists only of the objects exposed through this top-level package.
 Direct access to sub-modules is not officially supported, so may be affected by
 backwards-incompatible changes without notice.
 """
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals,
-)
 
 from .bloch import (
     display_bloch_sphere,
     display_bloch_sphere_from_bloch_vectors,
     display_bloch_sphere_from_density_matrices,
 )
 from .confidence_ellipses import (
     confidence_ellipse_matrix,
     plot_confidence_ellipses,
 )
 from .controls import (
     plot_controls,
     plot_sequences,
-    plot_smooth_controls,
-)
-from .cost_histories import (
-    plot_cost_histories,
-    plot_cost_history,
 )
+from .cost_histories import plot_cost_histories
 from .density_matrix import plot_density_matrix
 from .filter_functions import plot_filter_functions
 from .histogram import plot_bitstring_probabilities_histogram
 from .populations import (
     plot_population_distributions,
     plot_population_dynamics,
-    plot_populations,
 )
 from .style import (
     QCTRL_STYLE_COLORS,
     get_qctrl_style,
 )
 from .wigner_function import plot_wigner_function
 
@@ -63,20 +52,17 @@
     "display_bloch_sphere",
     "display_bloch_sphere_from_bloch_vectors",
     "display_bloch_sphere_from_density_matrices",
     "get_qctrl_style",
     "plot_confidence_ellipses",
     "plot_controls",
     "plot_cost_histories",
-    "plot_cost_history",
     "plot_density_matrix",
     "plot_filter_functions",
-    "plot_populations",
     "plot_population_dynamics",
     "plot_population_distributions",
     "plot_bitstring_probabilities_histogram",
     "plot_sequences",
-    "plot_smooth_controls",
     "plot_wigner_function",
 ]
 
-__version__ = "5.0.1"
+__version__ = "6.0.0"
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/bloch.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/bloch.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/confidence_ellipses.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/confidence_ellipses.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/controls.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 """
 Functions for plotting control pulses.
 """
 
 from __future__ import annotations
 
-import warnings
 from collections import namedtuple
 from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 from qctrlcommons.preconditions import check_argument
 
@@ -274,78 +273,14 @@
                 axes.axvline(x=time, linestyle="--", linewidth=1, zorder=-1)
 
             axes.set_ylabel(plot_data.ylabel)
 
     axes_list[-1].set_xlabel(f"Time ({time_prefix}s)")
 
 
-# Deprecated 2023/02/09.
-@qctrl_style()
-@figure_as_kwarg_only
-def plot_smooth_controls(
-    controls: dict,
-    polar: bool = True,
-    unit_symbol: str = "Hz",
-    two_pi_factor: bool = True,
-    *,
-    figure: plt.Figure,
-):
-    """
-    This function will be removed in the future. Please use `plot_controls` instead.
-    """
-
-    warnings.warn(
-        "The function `plot_smooth_controls` will be removed in the future. "
-        "Please use `plot_controls` instead.",
-        FutureWarning,
-    )
-
-    plots_data: list[Any] = []
-    for name, control in controls.items():
-        # Process each control depending whether it's passed as a list of samples...
-        if isinstance(control, list):
-            times = []
-            values = []
-            for sample in control:
-                times.append(sample["time"])
-                values.append(sample["value"])
-        # ...or a times/values dictionary.
-        else:
-            times = control["times"]
-            values = control["values"]
-        # Create plot data for the control.
-        plots_data = plots_data + _create_plots_data_from_control(
-            name, times, np.array(values), polar, unit_symbol, two_pi_factor
-        )
-
-    # Get the appropriate scaling for the time axis based on the total durations of all controls.
-    time_scaling, time_prefix = get_units(
-        [max(plot_data.xdata) for plot_data in plots_data]
-    )
-
-    axes_list = create_axes(
-        figure, 1, len(plots_data), width=FIG_WIDTH, height=FIG_WIDTH / 4, share_x=True
-    ).flatten()
-
-    for axes, plot_data in zip(axes_list, plots_data):
-        # Pad with leading and trailing zeros, to indicate that the pulse is zero outside the plot
-        # domain.
-        plot_times = np.pad(plot_data.xdata, ((1, 1)), "edge") / time_scaling
-        values_arr = np.pad(np.asarray(plot_data.values), ((1, 1)), "constant")
-
-        axes.plot(plot_times, values_arr, linewidth=2)
-        axes.fill(plot_times, values_arr, alpha=0.3)
-
-        axes.axhline(y=0, linewidth=1, zorder=-1)
-
-        axes.set_ylabel(plot_data.ylabel)
-
-    axes_list[-1].set_xlabel(f"Time ({time_prefix}s)")
-
-
 # Internal named tuple containing data required to draw a single plot. Note that xdata can represent
 # either durations (of segments) or times (of samples), depending on whether the plot is for a
 # piecewise-constant or smooth pulse.
 _PlotData = namedtuple("_PlotData", ["ylabel", "xdata", "values"])
 
 
 def _create_plots_data_from_control(
@@ -405,15 +340,15 @@
     ]
 
 
 @qctrl_style()
 @figure_as_kwarg_only
 def plot_sequences(sequences: dict, *, figure: plt.Figure):
     """
-    Create plot of dynamical decoupling sequences.
+    Create a plot of dynamical decoupling sequences.
 
     Parameters
     ----------
     sequences : dict
         The dictionary of sequences to plot. Works the same as the dictionary for
         plot_controls, but takes 'offset' instead of 'duration' and 'rotation'
         instead of 'value'. Rotations can be around any axis in the XY plane.
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/cost_histories.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/cost_histories.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 """
 Functions for plotting cost vs iterations.
 """
 
 from __future__ import annotations
 
-import warnings
 from typing import Optional
 
 import matplotlib.pyplot as plt
 from qctrlcommons.preconditions import check_argument
 
 from .style import qctrl_style
 from .utils import figure_as_kwarg_only
@@ -130,21 +129,7 @@
             )
 
     axs.set_xlabel("Iteration")
     axs.set_ylabel("Cost")
 
     if y_axis_log:
         axs.set_yscale("log")
-
-
-# Deprecated 2023/01/24.
-def plot_cost_history(*args, **kwargs):
-    """
-    This function will be removed in the future.
-    Please use `plot_cost_histories` instead.
-    """
-    warnings.warn(
-        "The function `plot_cost_history` will be removed in the future. "
-        "Please use `plot_cost_histories` instead.",
-        FutureWarning,
-    )
-    plot_cost_histories(*args, **kwargs)
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/density_matrix.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/density_matrix.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/filter_functions.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/filter_functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/histogram.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/histogram.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/populations.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/populations.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,28 +129,14 @@
 
     axes.set_xlabel(f"Time ({prefix}s)")
     axes.set_ylabel("Probability")
 
     axes.legend()
 
 
-# Deprecated 2023/02/28.
-def plot_populations(*args, **kwargs):
-    """
-    This function will be removed in the future.
-    Please use `plot_population_dynamics` instead.
-    """
-    warnings.warn(
-        "The function `plot_populations` will be removed in the future. "
-        "Please use `plot_population_dynamics` instead.",
-        FutureWarning,
-    )
-    plot_population_dynamics(*args, **kwargs)
-
-
 _PopulationData = namedtuple("_PopulationData", ["values", "label"])
 
 
 def _create_population_data(
     sample_times: np.ndarray, populations: dict
 ) -> list[_PopulationData]:
     """
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/style.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/style.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 BORDER_COLOR = "#D8E0E9"
 TEXT_COLOR = "#6C5C71"
 
 DPI = 72
 FIG_WIDTH = 10.0
 FIG_HEIGHT = 5.0
 
+#: A list of colors defined in the Q-CTRL style.
 QCTRL_STYLE_COLORS = [
     "#680CE9",
     "#D84144",
     "#32A4A8",
     "#A2A933",
     "#D84190",
     "#4177D8",
     "#D6722F",
     "#D543ED",
     "#32A857",
 ]
 
-
 QCTRL_SEQUENTIAL_COLORMAP = LinearSegmentedColormap.from_list(
     "QCTRL_SEQUENTIAL_COLORMAP",
     ["#EDE0FE", "#B482FA", "#680CE9", "#440087", "#1E0033"],
     N=200,
 )
```

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/utils.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/qctrlvisualizer/wigner_function.py` & `qctrl_visualizer-6.0.0/qctrlvisualizer/wigner_function.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.1/PKG-INFO` & `qctrl_visualizer-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-visualizer
-Version: 5.0.1
+Version: 6.0.0
 Summary: Q-CTRL Visualizer
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -30,15 +30,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: matplotlib (>=3.6.3)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: qctrl-commons (>=18.1.1,<19.0.0)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-visualizer/
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Description-Content-Type: text/markdown
 
 # Q-CTRL Visualizer
```

