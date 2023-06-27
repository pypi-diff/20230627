# Comparing `tmp/centerline-width-0.3.0.tar.gz` & `tmp/centerline-width-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.3.0.tar", last modified: Fri Jun 23 06:25:52 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.4.0.tar", last modified: Tue Jun 27 20:55:34 2023, max compression
```

## Comparing `centerline-width-0.3.0.tar` & `centerline-width-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.216256 centerline-width-0.3.0/
--rw-rw-r--   0 user      (1000) user      (1000)    41251 2023-06-23 06:25:52.216256 centerline-width-0.3.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    35625 2023-06-23 06:21:40.000000 centerline-width-0.3.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.208256 centerline-width-0.3.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-0.3.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    27096 2023-06-23 05:59:37.000000 centerline-width-0.3.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    15761 2023-06-23 06:16:11.000000 centerline-width-0.3.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.3.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     7691 2023-06-22 22:02:51.000000 centerline-width-0.3.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.3.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.216256 centerline-width-0.3.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)    14666 2023-06-23 06:16:37.000000 centerline-width-0.3.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.3.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.3.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.3.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     4107 2023-06-23 05:49:19.000000 centerline-width-0.3.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     6131 2023-06-23 05:40:55.000000 centerline-width-0.3.0/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.208256 centerline-width-0.3.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    41251 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-23 06:25:52.216256 centerline-width-0.3.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1850 2023-06-23 06:24:04.000000 centerline-width-0.3.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.398051 centerline-width-0.4.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    42076 2023-06-27 20:55:34.398051 centerline-width-0.4.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    36442 2023-06-27 20:52:49.000000 centerline-width-0.4.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-0.4.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-0.4.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-0.4.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.4.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8526 2023-06-24 01:42:25.000000 centerline-width-0.4.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.4.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-0.4.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.4.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-0.4.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.4.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-0.4.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-0.4.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    42076 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-27 20:55:34.398051 centerline-width-0.4.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1850 2023-06-27 20:52:28.000000 centerline-width-0.4.0/setup.py
```

### Comparing `centerline-width-0.3.0/PKG-INFO` & `centerline-width-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.4.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -21,30 +21,29 @@
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
-        	* saveCenterlineCSV()
-        	* saveCenterlineMAT()
         	* centerlineVoronoi
         	* centerlineEqualDistance 
         	* centerlineEvenlySpaced
         	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
+        * **Export centerline to .CSV and .MAT files**
+        	* saveCenterlineCSV()
+        	* saveCenterlineMAT()
         
         | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
         
-        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
-        
         NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
         
         ## Install
         PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
         
         ```
         pip install centerline-width
@@ -167,22 +166,24 @@
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
         				interpolate_data=False,
         				interpolate_n=5,
         				interpolate_n_centerpoints=None,
-        				equal_distance=10)
+        				equal_distance=10,
+        				ellipsoid="WGS84")
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
+        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
         **Solutions for sparse data:**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
@@ -203,27 +204,27 @@
         **Object (class) additional atttributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
+        * ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
         * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
         * interpolate_data (bool): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
-        
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
@@ -271,36 +272,36 @@
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
-        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+        * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
+        * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
         saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
         ```
-        * **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
-        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
+        * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -318,19 +319,25 @@
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
-        plotCenterline(display_all_possible_paths=False, 
+        plotCenterline(centerline_type="Voronoi",
+        		marker_type="line",
+        		centerline_color="black",
+        		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False)
         ```
+        * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
+        * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
         
         ```python
         import centerline_width
@@ -394,37 +401,34 @@
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         ### Return Width of River
         
-        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
+        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
-        			units="km",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
-        							units="km",
         							remove_intersections=True)
         ```
         Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
         
         ## Documentation and Algorithm to Determine Centerline
         
         The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
@@ -527,24 +531,21 @@
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
         * option to turn off verbose (no logs printed)
-        * option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
         
         ## Citations
-        Based on work written in R (Golly et al. 2017):
+        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) with modification (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
         
-        [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
-        
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
```

### Comparing `centerline-width-0.3.0/README.md` & `centerline-width-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,29 @@
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
 	* plotCenterline()
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
-	* saveCenterlineCSV()
-	* saveCenterlineMAT()
 	* centerlineVoronoi
 	* centerlineEqualDistance 
 	* centerlineEvenlySpaced
 	* centerlineSmoothed
 	* centerlineLength
 	* rightBankLength
 	* leftBankLength
+* **Export centerline to .CSV and .MAT files**
+	* saveCenterlineCSV()
+	* saveCenterlineMAT()
 
 | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
 
-Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
-
 NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
 
 ## Install
 PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
 
 ```
 pip install centerline-width
@@ -159,22 +158,24 @@
 First, generate a river object to contain river data and available transformations
 ```
 centerline_width.riverCenterline(csv_data=None,
 				optional_cutoff=None,
 				interpolate_data=False,
 				interpolate_n=5,
 				interpolate_n_centerpoints=None,
-				equal_distance=10)
+				equal_distance=10,
+				ellipsoid="WGS84")
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
+* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
 **Solutions for sparse data:**
 
 `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
 
 `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
 
@@ -195,27 +196,27 @@
 **Object (class) additional atttributes:**
 
 * river_name (string): name of object, set to the csv_data string
 * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
 * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
 * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
 * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
+* ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
 * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
 * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
 * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
 * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
 * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
 * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
 * interpolate_data (bool): if interpolating between existing data, defaults to False
 * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
 * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
 
-
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
 Return the latitude/longitude coordinates of the centerline based on the left and right banks
@@ -263,36 +264,36 @@
 
 ### Save Centerline Coordinates to a .CSV File
 Save the centerline coordinates to a csv file with columns for latitude and longitude
 
 ```
 saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
 ```
-* **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-* [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-* [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+* **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
+* [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
 ```
 Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
 
 ### Save Centerline Coordinates to a .MAT File
 Save the centerline coordinates to a .mat file with columns for latitude and longitude
 
 ```
 saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
 ```
-* **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
-* [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-* [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
-* [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+* **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
+* [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+* [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
+* [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
 ```
 Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -310,19 +311,25 @@
 ```
 The length of the river centerline returns `215.34700589636674` km
 
 ## Plot Centerline in Matplotlib
 Plot the centerline created from a list of right and left banks with Voronoi vertices
 
 ```
-plotCenterline(display_all_possible_paths=False, 
+plotCenterline(centerline_type="Voronoi",
+		marker_type="line",
+		centerline_color="black",
+		display_all_possible_paths=False, 
 		plot_title=None, 
 		save_plot_name=None, 
 		display_voronoi=False)
 ```
+* [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+* [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
+* [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
 
 ```python
 import centerline_width
@@ -386,37 +393,34 @@
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
 
 ### Return Width of River
 
-Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
+Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			apply_smoothing=True,
 			remove_intersections=False,
-			units="km",
 			save_to_csv=None)
 ```
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
 * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-* [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
 * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
 
 Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
 							apply_smoothing=True,
-							units="km",
 							remove_intersections=True)
 ```
 Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
 
 ## Documentation and Algorithm to Determine Centerline
 
 The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
@@ -519,24 +523,21 @@
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
 
 The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
 ## Developer Notes: Tech Debt and Bug Fixes
 * option to turn off verbose (no logs printed)
-* option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
 * Fix legend overlapping on graph, replace doc_examples that have an overlapping
 
 ## Citations
-Based on work written in R (Golly et al. 2017):
+Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) with modification (Golly et al. 2017):
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
 
-[Github - CMGO](https://github.com/AntoniusGolly/cmgo)
-
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
 </p>
 
 This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
```

### Comparing `centerline-width-0.3.0/centerline_width/__init__.py` & `centerline-width-0.4.0/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/centerline_width/centerline.py` & `centerline-width-0.4.0/centerline_width/centerline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Built in Python functions
 import math
 import logging
 import csv
 
 # External Python libraries (installed via pip install)
-from haversine import haversine
 import numpy as np
 import networkx as nx
 from scipy import interpolate
 from scipy.io import savemat
 from shapely.geometry import Point, LineString
+from shapely.ops import split
 import pyproj
 import geopy.distance
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 ## Logging set up for .INFO
@@ -109,23 +109,23 @@
 		logger.critical("\nCRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.")
 		shortest_path_points = None
 	else:
 		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
 
 	return starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_points
 
-def equalDistanceCenterline(centerline_coordinates=None, equal_distance=None):
+def equalDistanceCenterline(centerline_coordinates=None, equal_distance=None, ellipsoid="WGS84"):
 	# Interpolate centerline to space out coordinates an equal physical distance from the next (in meters)
 	if centerline_coordinates is None:
 		return None
 
 	centerline_line = LineString(centerline_coordinates)
 	equal_distance_between_centerline_coordinates=[]
 
-	geodesic = pyproj.Geod(ellps='WGS84')
+	geodesic = pyproj.Geod(ellps=ellipsoid)
 
 	# Iterate through coordinates based on a set distance (distance_m)
 	lon_start, lat_start = centerline_coordinates[0]
 	equal_distance_between_centerline_coordinates.append((lon_start, lat_start))
 	for i, centerline_coord in enumerate(centerline_coordinates):
 		if i+1 < len(centerline_coordinates):
 			lon_end, lat_end = centerline_coordinates[i+1]
@@ -237,14 +237,15 @@
 		if river_object.top_bank.distance(point1) < 1e-8 or river_object.bottom_bank.distance(point1) < 1e-8:
 			points_intersect_false_edges = True
 		if river_object.top_bank.distance(point2) < 1e-8 or river_object.bottom_bank.distance(point2) < 1e-8:
 			points_intersect_false_edges = True
 		return points_intersect_false_edges
 
 	# Generate a list of lines from the centerline point with its normal
+	logger.info("[PROCESSING] Calculating and positioning width lines, may takes a few minutes...")
 	min_x, min_y, max_x, max_y = river_object.bank_polygon.bounds
 	for centerline_point, slope in centerline_slope.items():
 		# draw a max line that extends the entire distance of the available space, will be trimmed below to just within polygon
 		left_y = slope * (min_x - centerline_point[0]) + centerline_point[1]
 		right_y = slope * (max_x - centerline_point[0]) + centerline_point[1]
 
 		# Save the points where they intersect the polygon
@@ -253,44 +254,32 @@
 		# if the line only intersects in two places (does not intersect polygon any additional times)
 		if len(line_intersection_points.geoms) == 2:
 			 # only save width lines that do not touch the artifical top/bottom
 			if not intersectsTopOrBottomOfBank(line_intersection_points.geoms[0], line_intersection_points.geoms[1]):
 				left_width_coordinates[centerline_point] = (line_intersection_points.geoms[0].x, line_intersection_points.geoms[0].y)
 				right_width_coordinates[centerline_point] = (line_intersection_points.geoms[1].x, line_intersection_points.geoms[1].y)
 		else:
-			# line intersects to polygon at multiple points, by default, find the closest two points to chart
-			distances_between_centerline_and_point = []
-			for i in range(len(line_intersection_points.geoms)):
-				point_intersection = Point(line_intersection_points.geoms[i].x, line_intersection_points.geoms[i].y)
-				distance_between = Point(centerline_point).distance(point_intersection)
-				distances_between_centerline_and_point.append(distance_between)
-
-			# collect the two closest points
-			index_of_sorted_list = sorted(range(len(distances_between_centerline_and_point)),key=distances_between_centerline_and_point.__getitem__)
-			smallest_point = line_intersection_points.geoms[index_of_sorted_list[0]]
-			second_smallest_point = line_intersection_points.geoms[index_of_sorted_list[1]]
-			if not intersectsTopOrBottomOfBank(smallest_point, second_smallest_point): # only save width lines that do not touch the artifical top/bottom
-
-				# Verify linestring contains the centerline (avoid making connections outside of polygon)
-				linestring_generated = LineString([Point(smallest_point.x, smallest_point.y), Point(second_smallest_point.x, second_smallest_point.y)])
-				if not linestring_generated.distance(Point(centerline_point)) < 1e-8: 
-					# linestring does not contains the centerline
-					# find a new second_smallest_point that falls on the centerline
-					for i in index_of_sorted_list: # search for new point in order of distance (smallest -> greatest)
-						second_smallest_point = line_intersection_points.geoms[index_of_sorted_list[i]]
-						linestring_generated = LineString([Point(smallest_point.x, smallest_point.y), Point(second_smallest_point.x, second_smallest_point.y)])
-						if smallest_point != second_smallest_point: # ignore current smallest_point (make a unique pair)
-							if linestring_generated.distance(Point(centerline_point)) < 1e-8: # if point is within a small distance of a line it is considered to intersect
-								break # once a linestring is found that lies within polygon, break out of search early
+			# line intersects to polygon at multiple points
+			if river_object.bank_polygon.contains(Point(centerline_point)): # width line made by centering centerline point, skip this width line if the centerline is outside of the polygon due to smoothing
+				all_linestring = split(sloped_line, river_object.bank_polygon) # split linestring where it intersects the polygon
+				left_point = None
+				right_point = None
+				for i, possible_linestring in enumerate(all_linestring.geoms): # iterate through all linestrings
+					if possible_linestring.distance(Point(centerline_point)) < 1e-8: # select linestring that contains the centerline point
+						left_point = Point(possible_linestring.coords[0])
+						right_point = Point(possible_linestring.coords[1])
 
 				# linestring contains the centerline, save coordinates
-				left_width_coordinates[centerline_point] = (smallest_point.x, smallest_point.y)
-				right_width_coordinates[centerline_point] = (second_smallest_point.x, second_smallest_point.y)
+				if left_point is not None and right_point is not None:
+					 # only save width lines that do not touch the artifical top/bottom
+					if not intersectsTopOrBottomOfBank(left_point, right_point):
+						left_width_coordinates[centerline_point] = (left_point.x, left_point.y)
+						right_width_coordinates[centerline_point] = (right_point.x, right_point.y)
 
-	# Determine lines that intersect with other lines in mulitple places to flag/remove
+	# Determine lines that intersect with other lines in multiple places to flag/remove
 	all_linestrings = []
 	linestring_with_centerlines = {} # linestring with associated centerline: {linestring : centerline coordinate}
 	linestring_with_linestrings_that_intersect = {} # dictionary of all the linestrings that a linestring intersects with
 	# Generate a list of linestrings
 	for centerline_coord in right_width_coordinates.keys():
 		linestring_generated = LineString([Point(left_width_coordinates[centerline_coord][0], left_width_coordinates[centerline_coord][1]),
 											Point(right_width_coordinates[centerline_coord][0], right_width_coordinates[centerline_coord][1])])
@@ -354,25 +343,23 @@
 
 	return right_width_coordinates, left_width_coordinates, num_intersection_coordinates
 
 def riverWidthFromCenterline(river_object=None,
 							transect_span_distance=3,
 							apply_smoothing=True,
 							remove_intersections=False,
-							units="km",
 							save_to_csv=None):
 	# Return river width: centerline and width at centerline
 	# Width is measured to the bank, relative to the center point (normal of the centerline)
 	# { [centerline latitude, centerline longitude] : widthValue }
 
 	centerline_width.errorHandlingRiverWidthFromCenterline(river_object=river_object,
 															transect_span_distance=transect_span_distance,
 															apply_smoothing=apply_smoothing,
 															remove_intersections=remove_intersections,
-															units=units,
 															save_to_csv=save_to_csv)
 
 	if river_object.centerlineVoronoi is None:
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
 	# recreate the centerline with evenly spaced points
@@ -385,47 +372,52 @@
 	# if using smoothing, replace left/right coordinates with the smoothed variation
 	right_width_coord, left_width_coord, _ = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																								centerline_coordinates=defined_centerline_coordinates,
 																								transect_span_distance=transect_span_distance,
 																								remove_intersections=remove_intersections)
 
 	width_dict = {}
+
+	geodesic = pyproj.Geod(ellps=river_object.ellipsoid)
+
 	for centerline_coord, _ in right_width_coord.items():
-		# store the haversine distance between the lat/lon position of the right/left bank
+		# store the distance between the lat/lon position of the right/left bank
 		lon1, lat1 = right_width_coord[centerline_coord]
 		lon2, lat2 = left_width_coord[centerline_coord]
-		haversine_distance_between_right_and_left = haversine((lat1, lon1), (lat2, lon2), unit=units)
-		width_dict[centerline_coord] = haversine_distance_between_right_and_left
+		_, _, distance_between_right_and_left_m = geodesic.inv(lon1, lat1, lon2, lat2)
+		width_dict[centerline_coord] = distance_between_right_and_left_m/1000
 
 	# Save width dictionary to a csv file (Latitude, Longtiude, Width)
 	if save_to_csv:
 		with open(save_to_csv, "w") as csv_file_output:
 			writer = csv.writer(csv_file_output)
-			writer.writerow(["Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width ({0})".format(units)])
+			writer.writerow(["Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)"])
 			for coordinate_key, width_value in width_dict.items():
 				writer.writerow([coordinate_key[1], coordinate_key[0], width_value])
 
 	return width_dict
 
-def centerlineLength(centerline_coordinates=None):
-	# Return the length/distance for all the centerline coordaintes in km
+def centerlineLength(centerline_coordinates=None, ellipsoid="WGS84"):
+	# Return the length/distance for all the centerline coordinates in km
 	total_length = 0
 	previous_pair = None
 	if centerline_coordinates is None:
 		return 0
 
+	geodesic = pyproj.Geod(ellps=ellipsoid)
+
 	for xy_pair in centerline_coordinates:
 		if previous_pair is None:
 			previous_pair = xy_pair
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
-			distance_to_add = haversine((lat1, lon1), (lat2, lon2), unit="km")
-			total_length += distance_to_add
-	return total_length
+			_, _, distance_between_meters = geodesic.inv(lon1, lat1, lon2, lat2)
+			total_length += distance_between_meters
+	return total_length/1000
 
 def saveCenterlineCSV(river_object=None, save_to_csv=None, latitude_header=None, longitude_header=None, centerline_type="Voronoi"):
 	# Save Centerline Coordinates generated by Voronoi Diagram to .CSV
 	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object,
 													save_to_csv=save_to_csv, 
 													latitude_header=latitude_header,
 													longitude_header=longitude_header,
```

### Comparing `centerline-width-0.3.0/centerline_width/error_handling.py` & `centerline-width-0.4.0/centerline_width/error_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 ## Logging set up for .CRITICAL
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.CRITICAL)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
+centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"]
+
 ## Error Handling: preprocessing.py
 def errrorHandlingConvertColumnsToCSV(text_file=None,
 									flipBankDirection=None):
 	# Error handling for convertColumnsToCSV()
 	if text_file is None:
 		logger.critical("\nCRITICAL ERROR, [text_file]: Requires text file")
 		exit()
@@ -33,27 +35,51 @@
 
 	if type(flipBankDirection) != bool:
 		logger.critical("\nCRITICAL ERROR, [flipBankDirection]: Must be a bool, current type = '{0}'".format(type(flipBankDirection)))
 		exit()
 
 ## Error Handling: plotDiagrams.py
 def errorHandlingPlotCenterline(river_object=None,
+								centerline_type=None,
+								marker_type=None,
+								centerline_color=None,
 								display_all_possible_paths=None,
 								plot_title=None,
 								save_plot_name=None,
 								display_voronoi=None):
 	# Error handling for plotCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
 			exit()
 
+	if type(centerline_type) != str:
+		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
+		exit()
+	else:
+		if centerline_type.title() not in centerline_type_options:
+			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
+			exit()
+
+	if type(marker_type) != str:
+		logger.critical("\nCRITICAL ERROR, [marker_type]: Must be a str, current type = '{0}'".format(type(marker_type)))
+		exit()
+	else:
+		marker_type_options = ["Line", "Scatter"]
+		if marker_type.title() not in marker_type_options:
+			logger.critical("\nCRITICAL ERROR, [marker_type]: Must be an available option in {0}, current option = '{1}'".format(marker_type_options, marker_type))
+			exit()
+
+	if type(centerline_color) != str:
+		logger.critical("\nCRITICAL ERROR, [centerline_color]: Must be a str, current type = '{0}'".format(type(centerline_color)))
+		exit()
+
 	if type(display_all_possible_paths) != bool:
 		logger.critical("\nCRITICAL ERROR, [display_all_possible_paths]: Must be a bool, current type = '{0}'".format(type(display_all_possible_paths)))
 		exit()
 
 	if plot_title is not None and type(plot_title) != str:
 		logger.critical("\nCRITICAL ERROR, [plot_title]: Must be a str, current type = '{0}'".format(type(plot_title)))
 		exit()
@@ -117,15 +143,14 @@
 		exit()
 
 ## Error Handling: centerline.py
 def errorHandlingRiverWidthFromCenterline(river_object=None,
 										transect_span_distance=None,
 										apply_smoothing=None,
 										remove_intersections=None,
-										units=None,
 										save_to_csv=None):
 	# Error Handling for riverWidthFromCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
@@ -145,23 +170,14 @@
 		logger.critical("\nCRITICAL ERROR, [apply_smoothing]: Must be a bool, current type = '{0}'".format(type(apply_smoothing)))
 		exit()
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
-	units_options = ["km","m","mi","nmi","ft","in","rad","deg"]
-	if units is not None and type(units) != str:
-			logger.critical("\nCRITICAL ERROR, [units]: Must be a str, current type = '{0}'".format(type(units)))
-			exit()
-	else:
-		if units not in units_options:
-			logger.critical("\nCRITICAL ERROR, [units]: Must be an option available ({0}), current given option = '{1}'".format(units_options, units))
-			exit()
-
 	if save_to_csv is not None:
 		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		if not save_to_csv.lower().endswith(".csv"):
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
 			exit()
@@ -192,15 +208,14 @@
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		else:
 			if not save_to_csv.lower().endswith(".csv"):
 				logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
 				exit()
 
-	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"]
 	if type(centerline_type) != str:
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
@@ -239,15 +254,14 @@
 			logger.critical("\nCRITICAL ERROR, [save_to_mat]: Must be a str, current type = '{0}'".format(type(save_to_mat)))
 			exit()
 		else:
 			if not save_to_mat.lower().endswith(".mat"):
 				logger.critical("\nCRITICAL ERROR, [save_to_mat]: Extension must be a .mat file, current extension = '{0}'".format(save_to_mat.split(".")[1]))
 				exit()
 
-	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"]
 	if type(centerline_type) != str:
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
@@ -291,15 +305,16 @@
 
 ## Error Handling: riverCenterlineClass.py
 def errorHandlingRiverCenterlineClass(csv_data=None,
 									optional_cutoff=None,
 									interpolate_data=None,
 									interpolate_n=None,
 									interpolate_n_centerpoints=None,
-									equal_distance=None):
+									equal_distance=None,
+									ellipsoid=None):
 	# Error Handling for riverCenterlineClass()
 	if csv_data is None:
 		logger.critical("\nCRITICAL ERROR, [csv_data]: Requires csv_data location")
 		exit()
 	else:
 		if type(csv_data) != str and not isinstance(csv_data, StringIO): 
 			# StringIO accounts for testing against a StringIO instead of a CSV (used in pytests)
@@ -332,7 +347,16 @@
 
 	if type(equal_distance) != int and type(equal_distance) != float:
 		logger.critical("\nCRITICAL ERROR, [equal_distance]: Must be a int or float, current type = '{0}'".format(type(equal_distance)))
 		exit()
 		if equal_distance <= 0:
 			logger.critical("WARNING, [equal_distance]: Must be a postive value, greater than 0, currently = '{0}'".format(equal_distance))
 			exit()
+
+	ellipsoid_options = ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"]
+	if type(ellipsoid) != str:
+		logger.critical("\nCRITICAL ERROR, [ellipsoid]: Must be a str, current type = '{0}'".format(type(ellipsoid)))
+		exit()
+	else:
+		if ellipsoid not in ellipsoid_options:
+			logger.critical("\nCRITICAL ERROR, [ellipsoid]: Must be an available option in {0}, current option = '{1}'".format(ellipsoid_options, ellipsoid))
+			exit()
```

### Comparing `centerline-width-0.3.0/centerline_width/getCoordinatesKML.py` & `centerline-width-0.4.0/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/centerline_width/plotDiagrams.py` & `centerline-width-0.4.0/centerline_width/plotDiagrams.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def plotCenterlineBackend(river_object=None, display_true_centerline=True):
+def plotCenterlineBackend(river_object=None,
+						display_true_centerline=True,
+						centerline_type="Voronoi",
+						marker_type="line",
+						centerline_color="black"):
 	# Shared components between plotCenterline and plotCenterlineWidth
 	fig = plt.figure(figsize=(10,10))
 	ax = fig.add_subplot(111)
 	
 	# Plot River as a Polygon
 	plt.plot(*river_object.bank_polygon.exterior.xy, c="gainsboro")
 	plt.plot(*river_object.top_bank.xy, c="forestgreen")
@@ -37,63 +41,84 @@
 	for i in river_object.left_bank_coordinates:
 		x.append(i[0])
 		y.append(i[1])
 	plt.scatter(x, y, c="orange", s=scatter_plot_size, label="Left Bank")
 
 	# Plot centerline found from NetworkX
 	valid_path_through = False
-	if river_object.centerlineVoronoi: # shortest path through points
+
+	centerline_type = centerline_type.title()
+	marker_type = marker_type.title()
+
+	if centerline_type == "Voronoi": 
+		centerline_coordinates_by_type = river_object.centerlineVoronoi
+		centerline_legend = "Voronoi Centerline Coordinates"
+	if centerline_type == "Equal Distance": 
+		centerline_coordinates_by_type = river_object.centerlineEqualDistance
+		centerline_legend = "Equal Distance Centerline Coordinates"
+	if centerline_type == "Evenly Spaced": 
+		centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+		centerline_legend = "Evenly Spaced Centerline Coordiantes"
+	if centerline_type == "Smoothed": 
+		centerline_coordinates_by_type = river_object.centerlineSmoothed
+		centerline_legend = "Smoothed Centerlined Coordiantes"
+
+	if centerline_coordinates_by_type:
 		valid_path_through = True
-		x = []
-		y = []
-		for k, v in river_object.centerlineVoronoi:
-			x.append(k)
-			y.append(v)
-		#plt.scatter(x, y, c="black", label="Centerline Coordinates", s=8)
 		if display_true_centerline:
-			plt.plot(*zip(*river_object.centerlineVoronoi), c="black", label="Centerline")
+			if marker_type == "Line":
+				plt.plot(*zip(*centerline_coordinates_by_type), c=centerline_color, label=centerline_legend)
+			if marker_type == "Scatter":
+				x = []
+				y = []
+				for k, v in centerline_coordinates_by_type:
+					x.append(k)
+					y.append(v)
+				plt.scatter(x, y, c=centerline_color, label=centerline_legend, s=8)
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 		plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
 		plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
 
 	return fig, ax, valid_path_through
 
 def plotCenterline(river_object=None,
+					centerline_type="Voronoi",
+					marker_type="line",
+					centerline_color="black",
 					display_all_possible_paths=False, 
 					plot_title=None, 
 					save_plot_name=None, 
 					display_voronoi=False):
 	# Plot Centerline of River
 	centerline_width.errorHandlingPlotCenterline(river_object=river_object,
+												centerline_type=centerline_type,
+												marker_type=marker_type,
+												centerline_color=centerline_color,
 												display_all_possible_paths=display_all_possible_paths,
 												plot_title=plot_title,
 												save_plot_name=save_plot_name,
 												display_voronoi=display_voronoi)
 
-	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, display_true_centerline=True)
+	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object,
+														display_true_centerline=True,
+														centerline_type=centerline_type,
+														marker_type=marker_type,
+														centerline_color=centerline_color)
 
 	# Display the Voronoi Diagram
 	if display_voronoi:
 		voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
 	if display_all_possible_paths:
 		for i in range(len(river_object.x_voronoi_ridge_point)):
 			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1)
 
-	# Plot Equally Spaced Points
-	x = []
-	y = []
-	for k, v in river_object.centerlineEqualDistance:
-			x.append(k)
-			y.append(v)
-	#plt.scatter(x, y, c="darkorchid", label="Equal Distance Centerline Coordinates", s=8)
-
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
 	plt.ylabel("Latitude (°)")
@@ -115,15 +140,19 @@
 													save_plot_name=save_plot_name, 
 													display_true_centerline=display_true_centerline,
 													transect_span_distance=transect_span_distance,
 													apply_smoothing=apply_smoothing,
 													flag_intersections=flag_intersections,
 													remove_intersections=remove_intersections)
 
-	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, display_true_centerline=display_true_centerline)
+	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, 
+														display_true_centerline=display_true_centerline,
+														centerline_type="Voronoi",
+														marker_type="line",
+														centerline_color="black")
 
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
 
 	if river_object.centerlineVoronoi is not None:
 		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(river_object.interpolate_n_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
@@ -142,23 +171,14 @@
 			else:
 				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
 																														remove_intersections=remove_intersections)
 
-			# Display the evenly spaced centerline
-			#x = []
-			#y = []
-			#for k, v in river_object.centerlineEvenlySpaced:
-			#	x.append(k)
-			#	y.append(v)
-			#plt.scatter(x, y, c="plum", label="Evenly Spaced Centerline Coordinates", s=8)
-			#plt.plot(*zip(*evenly_spaced_centerline_coordinates), "--", c="thistle", label="Evenly Spaced Centerline")
-
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
 				y_points = (right_width_coordinates[center_coord][1], left_width_coordinates[center_coord][1])
 				if flag_intersections:
 					if num_intersection_coordinates[center_coord] > 0:
 						if remove_intersections:
 							logger.error("\nERROR: Unable to completely resolve all intersections lines to be removed")
```

### Comparing `centerline-width-0.3.0/centerline_width/preprocessing.py` & `centerline-width-0.4.0/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/centerline_width/pytests/test_centerline.py` & `centerline-width-0.4.0/centerline_width/pytests/test_centerline.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,31 +80,14 @@
 	with pytest.raises(SystemExit):
 		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
 											remove_intersections=remove_intersections_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(remove_intersections_error_output)
 
-@pytest.mark.parametrize("units_invalid, units_error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_unitsInvalidTypes(caplog, units_invalid, units_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											units=units_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [units]: Must be a str, current type = '{0}'".format(units_error_output)
-
-def test_riverWidthFromCenterline_unitsInvalidOption(caplog):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											units="un")
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [units]: Must be an option available (['km', 'm', 'mi', 'nmi', 'ft', 'in', 'rad', 'deg']), current given option = 'un'"
-
 @pytest.mark.parametrize("save_to_csv_invalid, save_to_csv_error_output", invalid_non_str_options)
 def test_riverWidthFromCenterline_saveToCSVInvalidTypes(caplog, save_to_csv_invalid, save_to_csv_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
 											save_to_csv=save_to_csv_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
```

### Comparing `centerline-width-0.3.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.4.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.4.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,14 +54,57 @@
 def test_plotCenterline_riverObjectInvalidTypes(caplog, river_object_invalid, river_object_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_object_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(river_object_error_output)
 
+@pytest.mark.parametrize("centerline_type_invalid, centerline_type_error_output", invalid_non_str_options)
+def test_plotCenterline_centerlineTypeInvalidTypes(caplog, centerline_type_invalid, centerline_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										centerline_type=centerline_type_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(centerline_type_error_output)
+
+def test_plotCenterline_centerlineTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										centerline_type="invalid centerline")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'invalid centerline'"
+
+@pytest.mark.parametrize("marker_type_invalid, marker_type_error_output", invalid_non_str_options)
+def test_plotCenterline_markerTypeInvalidTypes(caplog, marker_type_invalid, marker_type_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										marker_type=marker_type_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [marker_type]: Must be a str, current type = '{0}'".format(marker_type_error_output)
+
+def test_plotCenterline_markerTypeInvalidOption(caplog):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										marker_type="invalid marker")
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [marker_type]: Must be an available option in ['Line', 'Scatter'], current option = 'invalid marker'"
+
+@pytest.mark.parametrize("centerline_color_invalid, centerline_color_error_output", invalid_non_str_options)
+def test_plotCenterline_centerlineColorInvalidTypes(caplog, centerline_color_invalid, centerline_color_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.plotCenterline(river_object=river_class_example,
+										centerline_color=centerline_color_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [centerline_color]: Must be a str, current type = '{0}'".format(centerline_color_error_output)
+
 @pytest.mark.parametrize("display_all_possible_paths_invalid, display_all_possible_paths_error_output", invalid_non_bool_options)
 def test_plotCenterline_displayAllPossiblePathsInvalidTypes(caplog, display_all_possible_paths_invalid, display_all_possible_paths_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_class_example,
 											display_all_possible_paths=display_all_possible_paths_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
```

### Comparing `centerline-width-0.3.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.4.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/centerline_width/riverCenterlineClass.py` & `centerline-width-0.4.0/centerline_width/riverCenterlineClass.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,43 +9,46 @@
 class riverCenterline:
 	def __init__(self,
 				csv_data=None,
 				optional_cutoff=None,
 				interpolate_data=False,
 				interpolate_n=5,
 				interpolate_n_centerpoints=None, 
-				equal_distance=10):
+				equal_distance=10,
+				ellipsoid="WGS84"):
 		centerline_width.errorHandlingRiverCenterlineClass(csv_data=csv_data,
 															optional_cutoff=optional_cutoff,
 															interpolate_data=interpolate_data,
 															interpolate_n=interpolate_n,
 															interpolate_n_centerpoints=interpolate_n_centerpoints,
-															equal_distance=equal_distance)
+															equal_distance=equal_distance,
+															ellipsoid=ellipsoid)
 
 		# Description and dataframe
 		self.river_name = csv_data
 		self.interpolate_data = interpolate_data
 		self.interpolate_n = interpolate_n
 		df = pd.read_csv(csv_data)
 		if optional_cutoff:
 			df = df.head(optional_cutoff)
 		self.df_len = len(df)
 		self.interpolate_n_centerpoints = interpolate_n_centerpoints
 		if self.interpolate_n_centerpoints is None: self.interpolate_n_centerpoints = self.df_len
+		self.ellipsoid = ellipsoid
 
 		# Left and Right Coordinates from the given csv data and data cutoff
 		left_bank_coordinates, right_bank_coordinates = centerline_width.leftRightCoordinates(df)
 		if interpolate_data:
 			right_bank_coordinates, left_bank_coordinates = centerline_width.interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n)
 		self.left_bank_coordinates = left_bank_coordinates
 		self.right_bank_coordinates = right_bank_coordinates
 
 		# Right/Length Bank Length
-		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
-		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
+		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates, ellipsoid=self.ellipsoid)
+		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates, ellipsoid=self.ellipsoid)
 
 		# River polygon, position of the top/bottom polygon
 		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(self.left_bank_coordinates, self.right_bank_coordinates)
 		self.bank_polygon = river_bank_polygon
 		self.top_bank = top_bank
 		self.bottom_bank = bottom_bank
 
@@ -60,33 +63,40 @@
 		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
 		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
 		# Voronoi Centerline Coordinates
 		self.centerlineVoronoi = shortest_path_coordinates
 
 		# Centerline length
-		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
+		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates, ellipsoid=self.ellipsoid)
 		self.equal_distance = equal_distance
 
 		# The different types of Centerline coordinates
 		self.centerlineEqualDistance = centerline_width.equalDistanceCenterline(centerline_coordinates=self.centerlineVoronoi,
-																				equal_distance=self.equal_distance)
+																				equal_distance=self.equal_distance,
+																				ellipsoid=self.ellipsoid)
 		self.centerlineEvenlySpaced = centerline_width.evenlySpacedCenterline(centerline_coordinates=self.centerlineVoronoi,
 																				number_of_fixed_points=self.interpolate_n_centerpoints)
 		self.centerlineSmoothed = centerline_width.smoothedCoordinates(river_object=self, centerline_coordinates=self.centerlineEvenlySpaced,
 																		interprolate_num=self.interpolate_n_centerpoints)
 
 
 
 	def plotCenterline(self,
+						centerline_type="Voronoi",
+						marker_type="line",
+						centerline_color="black",
 						display_all_possible_paths=False,
 						plot_title=None,
 						save_plot_name=None,
 						display_voronoi=False):
 		centerline_width.plotCenterline(river_object=self,
+										centerline_type=centerline_type,
+										marker_type=marker_type,
+										centerline_color=centerline_color,
 										display_all_possible_paths=display_all_possible_paths, 
 										plot_title=plot_title, 
 										save_plot_name=save_plot_name, 
 										display_voronoi=display_voronoi)
 
 	def plotCenterlineWidth(self,
 							plot_title=None, 
@@ -105,21 +115,19 @@
 											flag_intersections=flag_intersections,
 											remove_intersections=remove_intersections)
 
 	def riverWidthFromCenterline(self,
 								transect_span_distance=3,
 								apply_smoothing=True,
 								remove_intersections=False,
-								units="km",
 								save_to_csv=None):
 		return centerline_width.riverWidthFromCenterline(river_object=self,
 														transect_span_distance=transect_span_distance,
 														apply_smoothing=apply_smoothing,
 														remove_intersections=remove_intersections,
-														units=units,
 														save_to_csv=save_to_csv)
 
 	def saveCenterlineCSV(self, 
 						save_to_csv=None,
 						latitude_header=None,
 						longitude_header=None, 
 						centerline_type="Voronoi"):
```

### Comparing `centerline-width-0.3.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.4.0/centerline_width.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.4.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -21,30 +21,29 @@
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
-        	* saveCenterlineCSV()
-        	* saveCenterlineMAT()
         	* centerlineVoronoi
         	* centerlineEqualDistance 
         	* centerlineEvenlySpaced
         	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
+        * **Export centerline to .CSV and .MAT files**
+        	* saveCenterlineCSV()
+        	* saveCenterlineMAT()
         
         | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
         
-        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
-        
         NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.
         
         ## Install
         PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
         
         ```
         pip install centerline-width
@@ -167,22 +166,24 @@
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
         				interpolate_data=False,
         				interpolate_n=5,
         				interpolate_n_centerpoints=None,
-        				equal_distance=10)
+        				equal_distance=10,
+        				ellipsoid="WGS84")
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
+        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
         **Solutions for sparse data:**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
@@ -203,27 +204,27 @@
         **Object (class) additional atttributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
+        * ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
         * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
         * interpolate_data (bool): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
-        
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
@@ -271,36 +272,36 @@
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
-        * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
-        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
+        * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
+        * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
         saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
         ```
-        * **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
-        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
-        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
+        * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (cannot include spaces or special characters)
+        * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (cannot include spaces or special characters)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -318,19 +319,25 @@
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
-        plotCenterline(display_all_possible_paths=False, 
+        plotCenterline(centerline_type="Voronoi",
+        		marker_type="line",
+        		centerline_color="black",
+        		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False)
         ```
+        * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
+        * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
         
         ```python
         import centerline_width
@@ -394,37 +401,34 @@
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         ### Return Width of River
         
-        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width`
+        Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
-        			units="km",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] units (string): Units to measure distance, options: ["km" (kilometers), "m" (meters), "mi" (miles), "nmi" (nautical miles), "ft" (feet), "in" (inches), "rad" (radians), "deg" (degrees)], defaults to "km" (kilometers)
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
-        							units="km",
         							remove_intersections=True)
         ```
         Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
         
         ## Documentation and Algorithm to Determine Centerline
         
         The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
@@ -527,24 +531,21 @@
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
         * option to turn off verbose (no logs printed)
-        * option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
         
         ## Citations
-        Based on work written in R (Golly et al. 2017):
+        Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) with modification (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
         
-        [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
-        
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
```

### Comparing `centerline-width-0.3.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.4.0/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.3.0/setup.py` & `centerline-width-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.3.0"
+VERSION="0.4.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

