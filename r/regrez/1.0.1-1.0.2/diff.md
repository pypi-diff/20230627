# Comparing `tmp/regrez-1.0.1.tar.gz` & `tmp/regrez-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-1.0.1.tar", last modified: Tue Jun 27 18:32:02 2023, max compression
+gzip compressed data, was "regrez-1.0.2.tar", last modified: Tue Jun 27 18:37:07 2023, max compression
```

## Comparing `regrez-1.0.1.tar` & `regrez-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:32:02.550679 regrez-1.0.1/
--rw-rw-rw-   0        0        0     1407 2023-06-27 18:32:02.538034 regrez-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      953 2023-06-27 18:26:50.000000 regrez-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 18:32:02.524472 regrez-1.0.1/regrez.egg-info/
--rw-rw-rw-   0        0        0     1407 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 18:32:02.553412 regrez-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-06-27 18:31:47.000000 regrez-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:37:07.781776 regrez-1.0.2/
+-rw-rw-rw-   0        0        0     1473 2023-06-27 18:37:07.773761 regrez-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-06-27 18:36:37.000000 regrez-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:37:07.757136 regrez-1.0.2/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-06-27 18:37:07.000000 regrez-1.0.2/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-27 18:37:07.000000 regrez-1.0.2/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:37:07.000000 regrez-1.0.2/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 18:37:07.000000 regrez-1.0.2/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:37:07.000000 regrez-1.0.2/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 18:37:07.785808 regrez-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-27 18:36:46.000000 regrez-1.0.2/setup.py
```

### Comparing `regrez-1.0.1/PKG-INFO` & `regrez-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
-```
+
+``
 from regrez import Model
 m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
-```
-After that, you can train your model using m.Train() and test using m.Test(list_that_will_be_used_for_testing). Alternatively, there is a function called m.TrainAndTest() if you only want to see how good would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. Finally, you can use m.Visualize() after training if you want to see a plot showing both data points and the line to see how relative your variables are.
+``
+
+After that, you can train your model using ``m.Train()`` and test using ``m.Test(list_that_will_be_used_for_testing)``. Alternatively, there is a function called ``m.TrainAndTest()`` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use ``m.Visualize()`` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.0.1/README.md` & `regrez-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
-```
+
+``
 from regrez import Model
 m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
-```
-After that, you can train your model using m.Train() and test using m.Test(list_that_will_be_used_for_testing). Alternatively, there is a function called m.TrainAndTest() if you only want to see how good would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. Finally, you can use m.Visualize() after training if you want to see a plot showing both data points and the line to see how relative your variables are.
+``
+
+After that, you can train your model using ``m.Train()`` and test using ``m.Test(list_that_will_be_used_for_testing)``. Alternatively, there is a function called ``m.TrainAndTest()`` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use ``m.Visualize()`` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.0.1/regrez.egg-info/PKG-INFO` & `regrez-1.0.2/regrez.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
-```
+
+``
 from regrez import Model
 m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
-```
-After that, you can train your model using m.Train() and test using m.Test(list_that_will_be_used_for_testing). Alternatively, there is a function called m.TrainAndTest() if you only want to see how good would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. Finally, you can use m.Visualize() after training if you want to see a plot showing both data points and the line to see how relative your variables are.
+``
+
+After that, you can train your model using ``m.Train()`` and test using ``m.Test(list_that_will_be_used_for_testing)``. Alternatively, there is a function called ``m.TrainAndTest()`` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use ``m.Visualize()`` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.0.1/setup.py` & `regrez-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1' 
+VERSION = '1.0.2' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
         author="Mehmet Utku OZTURK",
         author_email="<contact@ælphard.tk>",
         description=DESCRIPTION,
         long_description=long,
+        long_description_content_type='text/markdown',
         packages=find_packages(),
         install_requires=["matplotlib", "sklearn", "numpy", "pandas"],
         
         keywords=['regression', 'machine learning'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Developers",
```

