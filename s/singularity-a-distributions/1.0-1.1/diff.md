# Comparing `tmp/singularity_a_distributions-1.0.tar.gz` & `tmp/singularity_a_distributions-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularity_a_distributions-1.0.tar", last modified: Tue Jun 27 12:58:08 2023, max compression
+gzip compressed data, was "singularity_a_distributions-1.1.tar", last modified: Tue Jun 27 13:24:28 2023, max compression
```

## Comparing `singularity_a_distributions-1.0.tar` & `singularity_a_distributions-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:58:08.767183 singularity_a_distributions-1.0/
--rw-rw-rw-   0        0        0      131 2023-06-27 12:58:08.767183 singularity_a_distributions-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 12:58:08.767183 singularity_a_distributions-1.0/setup.cfg
--rw-rw-rw-   0        0        0      255 2023-06-27 12:57:59.000000 singularity_a_distributions-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:58:08.759176 singularity_a_distributions-1.0/singularity_a_distributions/
--rw-rw-rw-   0        0        0    10375 2023-06-27 12:40:52.000000 singularity_a_distributions-1.0/singularity_a_distributions/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3630 2023-06-27 12:44:09.000000 singularity_a_distributions-1.0/singularity_a_distributions/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      932 2018-04-25 19:42:56.000000 singularity_a_distributions-1.0/singularity_a_distributions/Generaldistribution.py
--rw-rw-rw-   0        0        0      157 2023-06-27 12:49:06.000000 singularity_a_distributions-1.0/singularity_a_distributions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:58:08.765181 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/
--rw-rw-rw-   0        0        0      131 2023-06-27 12:58:08.000000 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-06-27 12:58:08.000000 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:58:08.000000 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-27 12:58:08.000000 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-27 12:58:08.000000 singularity_a_distributions-1.0/singularity_a_distributions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 13:24:28.240021 singularity_a_distributions-1.1/
+-rw-rw-rw-   0        0        0      131 2023-06-27 13:24:28.239019 singularity_a_distributions-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:24:28.241022 singularity_a_distributions-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-06-27 13:18:54.000000 singularity_a_distributions-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:24:28.228009 singularity_a_distributions-1.1/singularity_a_distributions/
+-rw-rw-rw-   0        0        0    10376 2023-06-27 13:17:39.000000 singularity_a_distributions-1.1/singularity_a_distributions/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3631 2023-06-27 13:17:33.000000 singularity_a_distributions-1.1/singularity_a_distributions/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      932 2018-04-25 19:42:56.000000 singularity_a_distributions-1.1/singularity_a_distributions/Generaldistribution.py
+-rw-rw-rw-   0        0        0      157 2023-06-27 12:49:06.000000 singularity_a_distributions-1.1/singularity_a_distributions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:24:28.238019 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-06-27 13:24:28.000000 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-06-27 13:24:28.000000 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:24:28.000000 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 13:24:28.000000 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-27 13:24:28.000000 singularity_a_distributions-1.1/singularity_a_distributions.egg-info/top_level.txt
```

### Comparing `singularity_a_distributions-1.0/singularity_a_distributions/Binomialdistribution.py` & `singularity_a_distributions-1.1/singularity_a_distributions/Binomialdistribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 import matplotlib.pyplot as plt
-from Generaldistribution import Distribution
+from .Generaldistribution import Distribution
 
 class Binomial(Distribution):
     """ Binomial distribution class for calculating and 
     visualizing a Binomial distribution.
     
     Attributes:
         mean (float) representing the mean value of the distribution
```

### Comparing `singularity_a_distributions-1.0/singularity_a_distributions/Gaussiandistribution.py` & `singularity_a_distributions-1.1/singularity_a_distributions/Gaussiandistribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 import matplotlib.pyplot as plt
-from Generaldistribution import Distribution
+from .Generaldistribution import Distribution
 
 class Gaussian(Distribution):
 	""" Gaussian distribution class for calculating and 
 	visualizing a Gaussian distribution.
 	
 	Attributes:
 		mean (float) representing the mean value of the distribution
```

### Comparing `singularity_a_distributions-1.0/singularity_a_distributions/Generaldistribution.py` & `singularity_a_distributions-1.1/singularity_a_distributions/Generaldistribution.py`

 * *Files identical despite different names*

