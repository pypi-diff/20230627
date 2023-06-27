# Comparing `tmp/classically-1.0.3.tar.gz` & `tmp/classically-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classically-1.0.3.tar", max compression
+gzip compressed data, was "classically-1.0.4.tar", max compression
```

## Comparing `classically-1.0.3.tar` & `classically-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      169 2023-03-17 19:12:00.676221 classically-1.0.3/classically/__init__.py
--rw-r--r--   0        0        0    11811 2023-03-17 19:12:00.676221 classically-1.0.3/classically/cdd.py
--rw-r--r--   0        0        0    10098 2023-03-17 20:02:32.259495 classically-1.0.3/classically/scatter.py
--rw-r--r--   0        0        0     7800 2023-03-17 19:14:25.104895 classically-1.0.3/classically/score.py
--rw-r--r--   0        0        0      388 2023-03-17 19:12:00.678222 classically-1.0.3/classically/types.py
--rw-r--r--   0        0        0     1088 2022-02-22 11:40:04.285844 classically-1.0.3/LICENSE
--rw-r--r--   0        0        0      632 2023-03-17 20:02:32.260496 classically-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5064 2023-03-17 19:12:00.676221 classically-1.0.3/README.md
--rw-r--r--   0        0        0     5867 2023-03-17 20:03:01.125431 classically-1.0.3/setup.py
--rw-r--r--   0        0        0     5754 2023-03-17 20:03:01.125431 classically-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      169 2022-10-11 09:02:37.605366 classically-1.0.4/classically/__init__.py
+-rw-r--r--   0        0        0    11807 2023-06-27 13:05:18.282032 classically-1.0.4/classically/cdd.py
+-rw-r--r--   0        0        0    12321 2023-06-27 14:08:36.096250 classically-1.0.4/classically/scatter.py
+-rw-r--r--   0        0        0     7800 2022-10-11 09:02:37.608600 classically-1.0.4/classically/score.py
+-rw-r--r--   0        0        0      388 2022-10-11 09:02:37.608600 classically-1.0.4/classically/types.py
+-rw-r--r--   0        0        0     1088 2022-08-11 16:42:59.484024 classically-1.0.4/LICENSE
+-rw-r--r--   0        0        0      632 2023-06-27 14:10:45.076811 classically-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5064 2022-10-11 09:15:32.917066 classically-1.0.4/README.md
+-rw-r--r--   0        0        0     5867 2023-06-27 14:12:13.559193 classically-1.0.4/setup.py
+-rw-r--r--   0        0        0     5754 2023-06-27 14:12:13.559193 classically-1.0.4/PKG-INFO
```

### Comparing `classically-1.0.3/classically/cdd.py` & `classically-1.0.4/classically/cdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, Sequence, overload
 
 import networkx as nx
 import numpy as np
-import scipy.stats as stats
 from matplotlib import pyplot as plt
 from matplotlib import ticker
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
+from scipy import stats
 
 
 def critical_difference_graph(
     data: np.ndarray,
     labels: Optional[Sequence[str]] = None,
     alpha: float = 0.05,
     holm_bonferroni: bool = True,
```

### Comparing `classically-1.0.3/classically/scatter.py` & `classically-1.0.4/classically/scatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,26 +24,31 @@
     axis.text(x=0.02, y=0.98, s=label, size="large", ha="left", va="top")
 
 
 def _scattercomp(
     data: np.ndarray,
     axis: Axes,
     labels: tuple[str, str],
-    color_points: tuple[
-        tuple[float, float, float], tuple[float, float, float]
+    color: Union[
+        tuple[tuple[float, float, float], tuple[float, float, float]],
+        Sequence[tuple[float, float, float]]
     ],
     color_default: tuple[float, float, float],
     color_dl: tuple[float, float, float],
+    display_numbers: bool,
     opacity: Optional[np.ndarray] = None,
 ) -> None:
     n_datasets = data.shape[1]
     colors = np.zeros((n_datasets, 4))
-    colors[data[0] > data[1], :3] = color_points[0]
-    colors[data[0] < data[1], :3] = color_points[1]
-    colors[data[0] == data[1], :3] = color_default
+    if len(color) > 2:
+        colors[:, :3] = color
+    else:
+        colors[data[0] > data[1], :3] = color[0]
+        colors[data[0] < data[1], :3] = color[1]
+        colors[data[0] == data[1], :3] = color_default
     colors[:, 3] = opacity if opacity is not None else 1.0
 
     # draw scatterplot
     axis.scatter(data[0, :], data[1, :], c=colors)
 
     # draw diagonal auxiliary lines
     axis.plot(
@@ -61,127 +66,171 @@
     )
 
     # draw lines for the mean values on each axis
     mean1 = data[0].mean()
     mean2 = data[1].mean()
     opacity1, ls1 = (0.8, "-") if mean1 > mean2 else (0.5, "--")
     opacity2, ls2 = (0.8, "-") if mean2 > mean1 else (0.5, "--")
+    color1 = (0, 0, 0) if len(color) > 2 else color[0]
+    color2 = (0, 0, 0) if len(color) > 2 else color[1]
     axis.axhline(
         mean2,
         xmin=0,
         xmax=mean2,
-        color=color_points[1]+(opacity2, ),
+        color=color2+(opacity2, ),
         ls=ls2,
     )
     axis.axvline(
         mean1,
         ymin=0,
         ymax=mean1,
-        color=color_points[0]+(opacity1, ),
+        color=color1+(opacity1, ),
         ls=ls1,
     )
     axis.axhline(
         0,
         xmin=0,
         xmax=1,
-        color=color_points[0]+(0.5, ),
+        color=color1+(0.5, ),
         lw=4,
     )
     axis.axvline(
         0,
         ymin=0,
         ymax=1,
-        color=color_points[1]+(0.5, ),
+        color=color2+(0.5, ),
         lw=4,
     )
+    if display_numbers:
+        axis.annotate(
+            f"${mean2:.2f}$ | ${np.sum(data[0] < data[1])}$", size="large",
+            xy=(0.08, mean2),
+            ha="left", va="top",
+            color=color2,
+        )
+        axis.annotate(
+            f"${mean1:.2f}$ | ${np.sum(data[0] > data[1])}$", size="large",
+            xy=(mean1, 0.08),
+            ha="right", va="bottom",
+            color=color1,
+            rotation=270,
+        )
+        # axis.text(
+        #     0.05, 0.02,
+        #     s=str(np.sum(data[0] > data[1])), size="large",
+        #     ha="left", va="top",
+        #     color=color1,
+        # )
     axis.text(0.02, 0.98, s=labels[1], size="large", ha="left", va="top")
     axis.text(0.98, 0.02, s=labels[0], size="large", ha="right", va="bottom")
 
 
 @overload
 def scatter_comparison(
     data: np.ndarray,
-    opacity: Optional[np.ndarray] = ...,
     labels: Optional[Sequence[str]] = ...,
-    axes: None = ...,
+    pairs: Optional[Sequence[tuple[int, int]]] = ...,
+    color: Optional[Union[
+        tuple[tuple[float, float, float], tuple[float, float, float]],
+        Sequence[tuple[float, float, float]]
+    ]] = ...,
+    opacity: Optional[np.ndarray] = ...,
+    axes: Union[Axes, np.ndarray] = ...,
     max_cols: int = ...,
     draw_hist: bool = ...,
-    color_points: Optional[
-        tuple[tuple[float, float, float], tuple[float, float, float]]
-    ] = ...,
+    display_numbers: bool = ...,
     color_hist: Optional[tuple[float, float, float]] = ...,
     color_dl: Optional[tuple[float, float, float]] = ...,
+    **kwargs,
 ) -> tuple[Figure, Axes]:
     ...
 
 
 @overload
 def scatter_comparison(
     data: np.ndarray,
-    opacity: Optional[np.ndarray] = ...,
     labels: Optional[Sequence[str]] = ...,
+    pairs: Optional[Sequence[tuple[int, int]]] = ...,
+    color: Optional[Union[
+        tuple[tuple[float, float, float], tuple[float, float, float]],
+        Sequence[tuple[float, float, float]]
+    ]] = ...,
+    opacity: Optional[np.ndarray] = ...,
     axes: Union[Axes, np.ndarray] = ...,
     max_cols: int = ...,
     draw_hist: bool = ...,
-    color_points: Optional[
-        tuple[tuple[float, float, float], tuple[float, float, float]]
-    ] = ...,
+    display_numbers: bool = ...,
     color_hist: Optional[tuple[float, float, float]] = ...,
     color_dl: Optional[tuple[float, float, float]] = ...,
+    **kwargs,
 ) -> None:
     ...
 
 
 def scatter_comparison(
     data: np.ndarray,
-    opacity: Optional[np.ndarray] = None,
     labels: Optional[Sequence[str]] = None,
+    pairs: Optional[Sequence[tuple[int, int]]] = None,
+    color: Optional[Union[
+        tuple[tuple[float, float, float], tuple[float, float, float]],
+        Sequence[tuple[float, float, float]]
+    ]] = None,
+    opacity: Optional[np.ndarray] = None,
     axes: Optional[Union[Axes, np.ndarray]] = None,
     max_cols: int = 4,
     draw_hist: bool = False,
-    color_points: Optional[
-        tuple[tuple[float, float, float], tuple[float, float, float]]
-    ] = None,
+    display_numbers: bool = True,
     color_hist: Optional[tuple[float, float, float]] = None,
     color_dl: Optional[tuple[float, float, float]] = None,
+    **kwargs,
 ) -> Optional[tuple[Figure, Union[Axes, np.ndarray]]]:
     """Creates scatterplots comparing the data of different categories.
     This produces plots for each combination of rows in the given
     ``data`` array.
     The plots also contain a vertical and horizontal line indicating the
     mean accuracy values of the classifiers. The line corresponding to
     the lower mean is dashed.
 
     Args:
         data (np.ndarray): A two dimensional array, e.g. consisting of
             accuracy values from different classifiers.
-        opacity (np.ndarray, optional): Opacity values that are used to
-            set alpha color values to the points in the scatter plot.
-            The length of this array has to be the same as the size of
-            the second dimension in ``data``.
         labels (Sequence[str], optional): A number of strings matching
             names of the categories or classifiers that are being
             compared. The length of this sequence has to match
             ``data.shape[0]``.
+        pairs (sequence of 2-tuples of int, optional): Which pairs of
+            classifiers to compare against one another. Defaults to all
+            possible combinations of two classifiers.
+        color (sequence of 3-tuples of floats, optional): Colors of
+            points in the scatterplots. The first color is used for
+            points below the diagonal line, the second for points above.
+            Points exactly on the diagonal use `color_hist`. The colors
+            are also used for the lines marking the mean values.
+            If a number of float tuples equal to the size of the second
+            dimension in ``data`` is given, the points in the scatter
+            plot will be colored accordingly.
+        opacity (np.ndarray, optional): Opacity values that are used to
+            set alpha color values to the points in the scatter plot.
+            The length of this array has to be the same as the size of
+            the second dimension in ``data``.
         axes (Axes | np.ndarray, optional): One or multiple axes in
             a numpy array. The plots will be drawn on these axes.
         max_cols (int, optional): If ``axes`` is not specified, this
             integer is the number of columns in a figure to fill before
             starting a new row of scatterplots. Defaults to 4.
         draw_hist (bool, optional): If True, also draws a histogram
             for each category. Defaults to False.
-        color_points (two 3-tuples of floats, optional): Colors of
-            points in the scatterplots. The first color is used for
-            points below the diagonal line, the second for points above.
-            Points exactly on the diagonal use `color_hist`. The colors
-            are also used for the lines marking the mean values.
+        display_numbers (bool, optional): Whether to display the number
+            of datasets where one classifier exceeds the other.
         color_hist (3-tuple of floats, optional): Color of the bars in
             histograms.
         color_dl (3-tuple of floats, optional): Color of the diagonal
             lines.
+        kwargs: Other keyword arguments directly passed to the figure
+            initialization method ``plt.subplots(n, m, **kwargs)``.
 
     Returns:
         Pyplot figure and axes containing all plots or None if ``axes``
         is specified.
     """
     fig = None
     if data.ndim != 2:
@@ -192,55 +241,61 @@
         raise ValueError(f"length of 'opacity' ({len(opacity)}) does not match"
                          f" data shape; should be {n_datasets}")
     if labels is not None and len(labels) != n_classifiers:
         raise ValueError(f"length of 'labels' ({len(labels)}) does not match"
                          f" data shape; should be {n_classifiers}")
 
     color_hist = color_hist if color_hist is not None else (0.7, 0.7, 0.1)
-    color_points = color_points if color_points is not None else (
+    color_points = color if color is not None else (
         (0.55, 0.1, 0.1), (0.1, 0.55, 0.1)
     )
     labels = labels if labels is not None else (
         [f"{i+1}" for i in range(n_classifiers)]
     )
     if n_classifiers == 1:
         if axes is not None:
             if not isinstance(axes, Axes):
                 raise ValueError(f"Expected a single axes, got {type(axes)}")
             return _hist(data, axis=axes, label=labels[0], color=color_hist)
         else:
-            fig, axs = plt.subplots(1, 1)
+            fig, axs = plt.subplots(1, 1, **kwargs)
             _hist(data, axis=axs, label=labels[0], color=color_hist)
             return fig, axs
 
     color_dl = color_dl if color_dl is not None else (0.2, 0.1, 0.7)
     if axes is None:
-        cols = n_plots = int(n_classifiers * (n_classifiers-1) / 2)
+        if pairs is None:
+            cols = n_plots = int(n_classifiers * (n_classifiers-1) / 2)
+        else:
+            cols = n_plots = len(pairs)
         if draw_hist:
             cols += n_classifiers
             n_plots = cols
         rows = 1
         if n_plots > max_cols:
             cols = max_cols
             rows = n_plots // max_cols
             if n_plots % max_cols != 0:
                 rows += 1
-        fig, axs = plt.subplots(rows, cols)
+        fig, axs = plt.subplots(rows, cols, **kwargs)
         axs = np.array(axs).reshape((rows, cols))
     else:
         if isinstance(axes, Axes):
             if n_classifiers > 2:
                 raise ValueError("Expected an array of axes")
             axes = np.array([[axes]])
         axs = axes
 
-    if draw_hist:
-        indices = combinations_with_replacement(range(n_classifiers), r=2)
+    if pairs is None:
+        if draw_hist:
+            indices = combinations_with_replacement(range(n_classifiers), r=2)
+        else:
+            indices = combinations(range(n_classifiers), r=2)
     else:
-        indices = combinations(range(n_classifiers), r=2)
+        indices = pairs
     i = j = 0
     for ii, jj in indices:
         if j == axs.shape[1]:
             j = 0
             i += 1
         axs[i, j].axis('square')
         axs[i, j].set_xlim([0, 1])
@@ -273,15 +328,16 @@
             )
         else:
             _scattercomp(
                 data[np.array([ii, jj]), :],
                 axis=axs[i, j],
                 opacity=opacity,
                 labels=(labels[ii], labels[jj]),
-                color_points=color_points,
+                color=color_points,
+                display_numbers=display_numbers,
                 color_default=color_hist,
                 color_dl=color_dl,
             )
         j += 1
     while j < axs.shape[1]:
         axs[i, j].axis('off')
         j += 1
```

### Comparing `classically-1.0.3/classically/score.py` & `classically-1.0.4/classically/score.py`

 * *Files identical despite different names*

### Comparing `classically-1.0.3/LICENSE` & `classically-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `classically-1.0.3/pyproject.toml` & `classically-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classically"
-version = "1.0.3"
+version = "1.0.4"
 description = "Classifier Comparison and Feature Analysis Tools in Python"
 authors = ["alienkrieg <alienkrieg@gmail.com>"]
 keywords = ["machine learning", "classification", "analysis"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/alienkrieg/classically"
```

### Comparing `classically-1.0.3/README.md` & `classically-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `classically-1.0.3/setup.py` & `classically-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'networkx>=2.6.3,<3.0.0',
  'numpy>=1.22.2,<2.0.0',
  'scikit-learn>=1.1.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'classically',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Classifier Comparison and Feature Analysis Tools in Python',
     'long_description': '# CLASSICALLY\nClassifier Comparison and Feature Analysis Tools in Python\n\nA python package for the evaluation of classification performance.\n\n## Installation\n\n__Classically__ is published on PyPi so you can install it with `pip`.\n\n    >>> python -m pip install classically\n\n## Applications\n\n### Critical Difference Diagram\n\nA main application is the comparison of categorized paired metric data, e.g. accuracy results of\ndifferent classification methods in machine learning.\nTherefore __Classically__ implements the *critical difference diagram* (described in [[1]](#1)).\n\n<a id="2"><u>Example</u></a>\n\nImagine that we have five different classification methods tested on 14 different datasets.\nEvery classifiers returns an accuracy result on each test set in the corresponding dataset.\nWe collect the results in a table like this:\n\nClassifier |      |      |      |      |      |      |      |      |      |      |      |      |      |      |\n-----------|------|------|------|------|------|------|------|------|------|------|------|------|------|------|\nA          | 0.60 | 0.81 | 0.62 | 0.19 | 0.93 | 0.54 | 0.53 | 0.41 | 0.21 | 0.97 | 0.32 | 0.82 | 0.38 | 0.75 |\nB          | 0.33 | 0.68 | 0.43 | 0.23 | 0.90 | 0.43 | 0.32 | 0.20 | 0.22 | 0.86 | 0.21 | 0.82 | 0.41 | 0.73 |\nC          | 0.25 | 0.64 | 0.40 | 0.10 | 0.85 | 0.39 | 0.31 | 0.19 | 0.18 | 0.90 | 0.23 | 0.78 | 0.43 | 0.71 |\nD          | 0.64 | 0.84 | 0.60 | 0.26 | 0.95 | 0.60 | 0.36 | 0.37 | 0.19 | 0.95 | 0.44 | 0.84 | 0.41 | 0.84 |\nE          | 0.37 | 0.68 | 0.47 | 0.18 | 0.88 | 0.37 | 0.27 | 0.25 | 0.24 | 0.79 | 0.25 | 0.83 | 0.36 | 0.64 |\n\nWe load this table in a `numpy array` of shape `(5, 14)` and call the function\n`classically.critical_difference_diagram`. The resulting plot can be seen below.\n\n![critical difference diagram](example/cdd_example.png)\n\nMarkings on this number line represent the average ranks of one classifier based on his accuracy\nover all datasets. The lowest rank corresponds to the highest accuracy. Classifiers are connected\nby a horizontal line if they do not have a significant difference. This significance is based on\npost-hoc Wilcoxon signed rank tests for each pair of classifiers.\n\nTherefore, it seems like classifier D is the best choice for the overall classification task.\nIt works best on the 14 chosen datasets, altough it\'s not the best classfier for every single\ndataset on its own. But we can also see, that there is no significant (`alpha=0.05`) difference in\nthe accuracy results of classifier D and A. If D would be much more computationally expensive than\nA, then we should consider choosing A as the better classifier.\n\n### Scatter Matrix\n\nFor an in-depth comparison of the classifiers on single datasets a special type of scatter matrix\nthat is designed to compare multiple categories of data can be found in __Classically__.\n\n<u>Example</u>\n\nFor a more elaborate decision in the [example above](#2) we could directly compare the best three\nclassifiers A, B and D using the function `classically.scatter_comparison.`\n\n![scatter comparison](example/scatter_example.png)\n\nPoints above the diagonal line represent datasets that are better classified by the method in the\nupper left corner. A horizontal and vertical line indicates the mean accuracy of the corresponding\nclassifier. A solid line marks the higher mean.\nA choice can now be easily made for the comparison of classifier A and B as well as B and D.\nWe also see that D is better than A in mean accuracy but that A has a big advantage on one dataset\nthat is well beyond the diagonal line for five percent difference.\nThe datasets could now be further analyzed by, for example, looking at the number of training and\ntest instances. An option for setting the opacity value of points in the scatterplots accordingly\nis available.\n\n### Feature Score\n\nEvaluating the importance of features in data can be very helpful in reducing the dimensionality of\nthe feature space. While principal component analysis transforms original features into new ones,\nit can also be used to creating a ranking of those features. __Classically__ is able to compute the\nfeature score for a given dataset.\n\n<u>Example</u>\n\nWe can analyze the importance of the four features in the well-known IRIS dataset by using the\nmethod `classically.plot_feature_score`.\n\n<p align="center"> <img width=512 src="example/score_example.png"> </align>\n\nThe plot shows the normalized feature score. The \'most important\' feature based on that score is\n\'petal length (cm)\'. All other features then have a relatively low score, e.g. sepal length\'s score\nis about 80% lower. The red markings show the accuracy results of a ridge classifier where only the\nfirst `n` features (in descending score order) are used (`n` gets incremented with each step on the\nx-axis).\n\n## References\n\n<a id="1">[1]</a>\nDemšar, Janez (2006).\n"Statistical comparisons of classifiers over multiple data sets."\nThe Journal of Machine learning research 7, 1-30.\n',
     'author': 'alienkrieg',
     'author_email': 'alienkrieg@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alienkrieg/classically',
```

### Comparing `classically-1.0.3/PKG-INFO` & `classically-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classically
-Version: 1.0.3
+Version: 1.0.4
 Summary: Classifier Comparison and Feature Analysis Tools in Python
 Home-page: https://github.com/alienkrieg/classically
 License: MIT
 Keywords: machine learning,classification,analysis
 Author: alienkrieg
 Author-email: alienkrieg@gmail.com
 Requires-Python: >=3.9,<3.10
```

