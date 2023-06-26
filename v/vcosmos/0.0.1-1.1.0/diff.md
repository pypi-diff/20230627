# Comparing `tmp/vcosmos-0.0.1.tar.gz` & `tmp/vcosmos-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcosmos-0.0.1.tar", last modified: Thu Jun 15 00:55:10 2023, max compression
+gzip compressed data, was "vcosmos-1.1.0.tar", last modified: Mon Jun 26 23:28:49 2023, max compression
```

## Comparing `vcosmos-0.0.1.tar` & `vcosmos-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 00:55:10.256370 vcosmos-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-14 22:54:01.000000 vcosmos-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4239 2023-06-15 00:55:10.256370 vcosmos-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3690 2023-06-15 00:48:32.000000 vcosmos-0.0.1/README.md
--rw-rw-rw-   0        0        0      100 2023-06-14 22:49:59.000000 vcosmos-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      641 2023-06-15 00:55:10.259374 vcosmos-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 00:55:10.239370 vcosmos-0.0.1/spatial_domain/
--rw-rw-rw-   0        0        0        0 2023-06-14 23:06:39.000000 vcosmos-0.0.1/spatial_domain/__init__.py
--rw-rw-rw-   0        0        0     4268 2023-06-14 23:56:57.000000 vcosmos-0.0.1/spatial_domain/anomaly.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:55:10.253394 vcosmos-0.0.1/vcosmos.egg-info/
--rw-rw-rw-   0        0        0     4239 2023-06-15 00:55:10.000000 vcosmos-0.0.1/vcosmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-15 00:55:10.000000 vcosmos-0.0.1/vcosmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 00:55:10.000000 vcosmos-0.0.1/vcosmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-15 00:55:10.000000 vcosmos-0.0.1/vcosmos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 23:28:49.980865 vcosmos-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 22:54:01.000000 vcosmos-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4405 2023-06-26 23:28:49.980865 vcosmos-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3856 2023-06-26 23:12:36.000000 vcosmos-1.1.0/README.md
+-rw-rw-rw-   0        0        0      100 2023-06-14 22:49:59.000000 vcosmos-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      641 2023-06-26 23:28:49.982863 vcosmos-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 23:28:49.967452 vcosmos-1.1.0/spatial_domain/
+-rw-rw-rw-   0        0        0        0 2023-06-14 23:06:39.000000 vcosmos-1.1.0/spatial_domain/__init__.py
+-rw-rw-rw-   0        0        0     4538 2023-06-26 23:00:22.000000 vcosmos-1.1.0/spatial_domain/anomaly.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:28:49.978452 vcosmos-1.1.0/vcosmos.egg-info/
+-rw-rw-rw-   0        0        0     4405 2023-06-26 23:28:49.000000 vcosmos-1.1.0/vcosmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-26 23:28:49.000000 vcosmos-1.1.0/vcosmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 23:28:49.000000 vcosmos-1.1.0/vcosmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 23:28:49.000000 vcosmos-1.1.0/vcosmos.egg-info/top_level.txt
```

### Comparing `vcosmos-0.0.1/LICENSE.txt` & `vcosmos-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcosmos-0.0.1/PKG-INFO` & `vcosmos-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: vcosmos
-Version: 0.0.1
-Summary: This pacakge implements a 3D projection-based outlier detection algorithm using median-derived distance thresholds.
+Version: 1.1.0
+Summary: This package implements a 3D projection-based outlier detection algorithm using median-derived distance thresholds.
 Home-page: https://github.com/KarthikDevalla/vcosmos.git
 Author: Karthik Devalla
 Author-email: ihatecoding666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# __vcosmos.spatial_domain.anomaly__.O_Seive
+# __spatial_domain.anomaly__.O_Sieve
 
 ---
-## class __O_seive__(data, column, tsf=1, bsf=1)
+## class __O_Sieve__(data, column, tsf=1, bsf=1)
 ---
 
-### ___O_Seive___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
-  
-
+### ___O_Sieve___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
+--- 
+## What's new - __Version release 1.0.2__
+- Added support for __boxplots__ , `Pre and Post Cleaning` along with the `heliocentric slicing plot` to perform better cleaning. 
 ---
 ## Parameters:
 
 - __data__: _dataframe_
     - The __data__ on which the algorithm should be applied.
 
 - __column__: _str_
     - __Target column__, the filtering is done based on this column.
 
-- __tsf__: _int or float, defaul-t=1_
+- __tsf__: _int or float, default=1_
     - __Top scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
 
 - __bsf__ : _int or float, default=1_
-    - __Bottom scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
+    - __Bottom scaling factor__, the quantity with which the median distance must be multplied below the centre plane.
 ---
 ## Installation
 ```pip install vcosmos```
 
 ## Usage
 ```python
 import pandas as pd
-from spatial_domain.anomaly import O_Seive
+from spatial_domain.anomaly import O_Sieve
 # Reading a dataset using pandas.
 df=pd.read_csv('co2.csv')
 print(df.head)
 
 #   Make       Model Vehicle Class  Engine Size(L)  ...  Fuel Consumption Hwy (L/100 km) Fuel Consumption Comb (L/100 km) Fuel Consumption Comb (mpg)  CO2 Emissions(g/km)
 # 0  ACURA         ILX       COMPACT             2.0  ...                              6.7                              8.5                          33                  196
 # 1  ACURA         ILX       COMPACT             2.4  ...                              7.7                              9.6                          29                  221
```

### Comparing `vcosmos-0.0.1/README.md` & `vcosmos-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# __vcosmos.spatial_domain.anomaly__.O_Seive
+# __spatial_domain.anomaly__.O_Sieve
 
 ---
-## class __O_seive__(data, column, tsf=1, bsf=1)
+## class __O_Sieve__(data, column, tsf=1, bsf=1)
 ---
 
-### ___O_Seive___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
-  
-
+### ___O_Sieve___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
+--- 
+## What's new - __Version release 1.0.2__
+- Added support for __boxplots__ , `Pre and Post Cleaning` along with the `heliocentric slicing plot` to perform better cleaning. 
 ---
 ## Parameters:
 
 - __data__: _dataframe_
     - The __data__ on which the algorithm should be applied.
 
 - __column__: _str_
     - __Target column__, the filtering is done based on this column.
 
-- __tsf__: _int or float, defaul-t=1_
+- __tsf__: _int or float, default=1_
     - __Top scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
 
 - __bsf__ : _int or float, default=1_
-    - __Bottom scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
+    - __Bottom scaling factor__, the quantity with which the median distance must be multplied below the centre plane.
 ---
 ## Installation
 ```pip install vcosmos```
 
 ## Usage
 ```python
 import pandas as pd
-from spatial_domain.anomaly import O_Seive
+from spatial_domain.anomaly import O_Sieve
 # Reading a dataset using pandas.
 df=pd.read_csv('co2.csv')
 print(df.head)
 
 #   Make       Model Vehicle Class  Engine Size(L)  ...  Fuel Consumption Hwy (L/100 km) Fuel Consumption Comb (L/100 km) Fuel Consumption Comb (mpg)  CO2 Emissions(g/km)
 # 0  ACURA         ILX       COMPACT             2.0  ...                              6.7                              8.5                          33                  196
 # 1  ACURA         ILX       COMPACT             2.4  ...                              7.7                              9.6                          29                  221
```

### Comparing `vcosmos-0.0.1/spatial_domain/anomaly.py` & `vcosmos-1.1.0/spatial_domain/anomaly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 import inspect
+import seaborn as sns
 import matplotlib.pyplot as plt
 
-
-class O_Seive:
+class O_Sieve:
 	def __init__(self, data, column, tsf=1, bsf=1):
 
-		if len(inspect.signature(O_Seive.__init__).parameters)-1 !=4:
+		if len(inspect.signature(O_Sieve.__init__).parameters)-1 !=4:
 			raise TypeError('Invalid number of arguments')
 
 		self.column=column # Name of the column
 		self.data=data # Dataframe
 		self.tsf=tsf # Top scaling factor.
 		self.bsf=bsf # Bottom scaling factor.
 		
@@ -26,42 +26,47 @@
 		self.ymin=self.data[self.column].min()
 		self.ymax=self.data[self.column].max()
 		self.zval=np.mean(np.square(self.data[self.column]))
 
 		print('Filtering Initiated....')
 	
 	def hcps_plot(self):
-		fig = plt.figure()
-		ax = fig.add_subplot(projection='3d')
+		fig = plt.figure(figsize=(14,6))
+		ax = fig.add_subplot(131,projection='3d')
 		ax.scatter(self.data.index, self.data[self.column], np.square(self.data[self.column]), s=0.5,color='black')
 		ax.scatter(np.mean(self.data.index),np.mean(self.data[self.column]),self.zval,color='orange',s=300)
 		ax.plot_surface([[self.xmin, self.xmax], [self.xmin, self.xmax]], [[self.ymin, self.ymin], [self.ymax, self.ymax]], np.array([[self.zval, self.zval], [self.zval, self.zval]]), alpha=0.5,color='blue')
 		ax.set_xlabel('X-axis')
 		ax.set_ylabel('Y-axis')
 		ax.set_zlabel('Z-axis')
-		z_dist_plane1, z_dist_plane2=self.learning()
+		z_dist_plane1, z_dist_plane2=self.split_learning()
 		ax.plot_surface([[self.xmin, self.xmax], [self.xmin, self.xmax]], [[self.ymin, self.ymin], [self.ymax, self.ymax]], np.array([[z_dist_plane1, z_dist_plane1], [z_dist_plane1, z_dist_plane1]]), alpha=0.5,color='red')
 		ax.plot_surface([[self.xmin, self.xmax], [self.xmin, self.xmax]], [[self.ymin, self.ymin], [self.ymax, self.ymax]], np.array([[z_dist_plane2, z_dist_plane2], [z_dist_plane2, z_dist_plane2]]), alpha=0.5,color='red')
+		
+		ax1 = fig.add_subplot(132)
+		sns.boxplot(self.data[self.column]).set_title('Pre-Cleaning')
 
+		ax2 = fig.add_subplot(133)
+		sns.boxplot(self.new_data[self.column]).set_title('Post-Cleaning')
+		plt.tight_layout()
 		return plt.show()
 
-	def learning(self):
+	def split_learning(self):
 		centre = np.array([np.mean(self.data.index), np.mean(self.data[self.column]),self.zval])
 		top_distances, bottom_distances =[],[]
 		x=self.data.index
 		y=self.data[self.column]
 		z=np.square(self.data[self.column])
 		
 		for ind, val in enumerate(z):
 			if val >= self.zval:
 				top_distances.extend(np.linalg.norm(np.column_stack((x[ind], y[ind], z[ind])) - centre, axis=1).tolist())
 			else:
 				bottom_distances.extend(np.linalg.norm(np.column_stack((x[ind], y[ind], z[ind])) - centre, axis=1).tolist())
 				
-		@staticmethod
 		def median_break(data):
 			sorted_data=sorted(data)
 			if len(sorted_data) % 2 !=0:
 				return x[len(sorted_data)//2], y[len(sorted_data)//2], (z[len(sorted_data)//2], 0), sorted_data[len(sorted_data)//2]
 			else:
 				p1=sorted_data[len(sorted_data)//2]
 				p2=sorted_data[len(sorted_data)//2+1]
@@ -94,19 +99,16 @@
 	def encompassing_points(self,z,d1,d2):
 		if (z > d1)  or (z < d2):
 			return 0 # OUTLIER
 		else:
 			return 1
 		
 	def filtered_data(self):
-		z_dist_plane1, z_dist_plane2=self.learning()
+		z_dist_plane1, z_dist_plane2=self.split_learning()
 		indices=[self.encompassing_points(n, z_dist_plane1, z_dist_plane2) for n in np.square(self.data[self.column])]
 		self.data['Status']=indices
-		new_data=self.data.loc[self.data['Status'] == 1].drop(columns='Status').reset_index(drop=True)
+		self.new_data=self.data.loc[self.data['Status'] == 1].drop(columns='Status').reset_index(drop=True)
 		print('Filtering Complete.')
-		print('Ouliers Removed:',self.data.shape[0]-new_data.shape[0])
-		return new_data 
-
-
-
+		print('Ouliers Removed:',self.data.shape[0]-self.new_data.shape[0])
+		return self.new_data
```

### Comparing `vcosmos-0.0.1/vcosmos.egg-info/PKG-INFO` & `vcosmos-1.1.0/vcosmos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: vcosmos
-Version: 0.0.1
-Summary: This pacakge implements a 3D projection-based outlier detection algorithm using median-derived distance thresholds.
+Version: 1.1.0
+Summary: This package implements a 3D projection-based outlier detection algorithm using median-derived distance thresholds.
 Home-page: https://github.com/KarthikDevalla/vcosmos.git
 Author: Karthik Devalla
 Author-email: ihatecoding666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# __vcosmos.spatial_domain.anomaly__.O_Seive
+# __spatial_domain.anomaly__.O_Sieve
 
 ---
-## class __O_seive__(data, column, tsf=1, bsf=1)
+## class __O_Sieve__(data, column, tsf=1, bsf=1)
 ---
 
-### ___O_Seive___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
-  
-
+### ___O_Sieve___ is an outlier detection algorithm that utilizes a 3D projection of data points. It calculates distances of data points from a centre point in the 3D space, based on the squared values of the target column. The algorithm then determines upper and lower distance thresholds using a median-based approach. Data points that fall outside these thresholds are considered outliers. This class also provides methods for visualizing the data in the 3D space. 
+--- 
+## What's new - __Version release 1.0.2__
+- Added support for __boxplots__ , `Pre and Post Cleaning` along with the `heliocentric slicing plot` to perform better cleaning. 
 ---
 ## Parameters:
 
 - __data__: _dataframe_
     - The __data__ on which the algorithm should be applied.
 
 - __column__: _str_
     - __Target column__, the filtering is done based on this column.
 
-- __tsf__: _int or float, defaul-t=1_
+- __tsf__: _int or float, default=1_
     - __Top scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
 
 - __bsf__ : _int or float, default=1_
-    - __Bottom scaling factor__, the quantity with which the median distance must be multplied above the centre plane.
+    - __Bottom scaling factor__, the quantity with which the median distance must be multplied below the centre plane.
 ---
 ## Installation
 ```pip install vcosmos```
 
 ## Usage
 ```python
 import pandas as pd
-from spatial_domain.anomaly import O_Seive
+from spatial_domain.anomaly import O_Sieve
 # Reading a dataset using pandas.
 df=pd.read_csv('co2.csv')
 print(df.head)
 
 #   Make       Model Vehicle Class  Engine Size(L)  ...  Fuel Consumption Hwy (L/100 km) Fuel Consumption Comb (L/100 km) Fuel Consumption Comb (mpg)  CO2 Emissions(g/km)
 # 0  ACURA         ILX       COMPACT             2.0  ...                              6.7                              8.5                          33                  196
 # 1  ACURA         ILX       COMPACT             2.4  ...                              7.7                              9.6                          29                  221
```

