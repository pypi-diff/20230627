# Comparing `tmp/lognflow-0.7.4.tar.gz` & `tmp/lognflow-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.4.tar", last modified: Mon Jun 26 01:03:26 2023, max compression
+gzip compressed data, was "lognflow-0.7.5.tar", last modified: Tue Jun 27 03:29:02 2023, max compression
```

## Comparing `lognflow-0.7.4.tar` & `lognflow-0.7.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 01:03:16.000000 lognflow-0.7.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-26 01:03:16.000000 lognflow-0.7.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-26 01:03:16.000000 lognflow-0.7.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-26 01:03:16.000000 lognflow-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 01:03:16.000000 lognflow-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 01:03:26.865371 lognflow-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 01:03:16.000000 lognflow-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65639 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 01:03:26.869371 lognflow-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 01:03:16.000000 lognflow-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 03:28:52.000000 lognflow-0.7.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-27 03:28:52.000000 lognflow-0.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-27 03:28:52.000000 lognflow-0.7.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-27 03:28:52.000000 lognflow-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 03:28:52.000000 lognflow-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-27 03:29:02.686514 lognflow-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 03:28:52.000000 lognflow-0.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66489 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-27 03:29:02.686514 lognflow-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-27 03:28:52.000000 lognflow-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.4/CONTRIBUTING.rst` & `lognflow-0.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/HISTORY.rst` & `lognflow-0.7.5/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -100,8 +100,12 @@
 ------------------
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
-* critical bug fixed in log_imshow
+* critical bug fixed in log_imshow
+
+0.7.5 (2023-08-01)
+------------------
+* Added complex numbers to log_imshow
```

### Comparing `lognflow-0.7.4/LICENSE` & `lognflow-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/PKG-INFO` & `lognflow-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.4
+Version: 0.7.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -194,7 +194,11 @@
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
 * critical bug fixed in log_imshow
+
+0.7.5 (2023-08-01)
+------------------
+* Added complex numbers to log_imshow
```

### Comparing `lognflow-0.7.4/README.rst` & `lognflow-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/docs/Makefile` & `lognflow-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/docs/conf.py` & `lognflow-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/docs/installation.rst` & `lognflow-0.7.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/docs/make.bat` & `lognflow-0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/lognflow/lognflow.py` & `lognflow-0.7.5/lognflow/lognflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,14 +664,15 @@
         """ Add colobar to the current axis 
             This is specially useful in plt.subplots
             stackoverflow.com/questions/23876588/
                 matplotlib-colorbar-in-each-subplot
         """
         ax = mappable.axes
         fig = ax.figure
+        from mpl_toolkits.axes_grid1 import make_axes_locatable
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         cbar = fig.colorbar(mappable, cax=cax)
         # cbar.ax.tick_params(size=0.01)
 
     def log_multichannel_by_subplots(self, 
         parameter_name: str, 
@@ -987,20 +988,38 @@
                 FLAG_img_ready = True
                 use_multichannel_to_square = True
         
         if(use_multichannel_to_square):
             parameter_value = self. multichannel_to_square(
                 parameter_value, borders = borders)
         if(FLAG_img_ready):
-            fig, ax = plt.subplots()
-            im = ax.imshow(parameter_value, cmap = cmap, **kwargs)
-            if(colorbar):
-                plt.colorbar(im)
-            if(remove_axis_ticks):
-                plt.setp(ax, xticks=[], yticks=[])
+
+            if(not np.iscomplexobj(parameter_value)):
+                fig, ax = plt.subplots()
+                im = ax.imshow(parameter_value, cmap = cmap, **kwargs)
+                if(colorbar):
+                    plt.colorbar(im)
+                if(remove_axis_ticks):
+                    plt.setp(ax, xticks=[], yticks=[])
+            else:
+                fig, ax = plt.subplots(1, 2)
+                im = ax[0].imshow(np.real(parameter_value), cmap = cmap, **kwargs)
+                if(colorbar):
+                    self.add_colorbar(im)
+                    # plt.colorbar(im)
+                ax[0].set_title('Real')    
+                im = ax[1].imshow(np.imag(parameter_value), cmap = cmap, **kwargs)
+                if(colorbar):
+                    self.add_colorbar(im)
+                    # plt.colorbar(im)
+                ax[1].set_title('Imag')
+                if(remove_axis_ticks):
+                    plt.setp(ax[0], xticks=[], yticks=[])
+                    plt.setp(ax[1], xticks=[], yticks=[])
+                
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
             return fpath
         else:
             self.log_text(
```

### Comparing `lognflow-0.7.4/lognflow/logviewer.py` & `lognflow-0.7.5/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/lognflow/printprogress.py` & `lognflow-0.7.5/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.5/lognflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.4
+Version: 0.7.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -194,7 +194,11 @@
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
 * critical bug fixed in log_imshow
+
+0.7.5 (2023-08-01)
+------------------
+* Added complex numbers to log_imshow
```

### Comparing `lognflow-0.7.4/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.5/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.4/setup.py` & `lognflow-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.4'
+__version__ = '0.7.5'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.4/tests/test_lognflow.py` & `lognflow-0.7.5/tests/test_lognflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,22 +268,32 @@
     logger = lognflow(temp_dir)
     logger('This is a test for test_log_single_text', flush = True)
     var = 2
     logger.log_single('text_log', 'hello\n', save_as='txt', time_tag = False)
     logger.log_single('text_log', 'bye\n', save_as='txt', time_tag = False)
     logger.log_single('text_log', var, save_as='txt', time_tag = False)
     
+def test_log_imshow_complex():
+    logger = lognflow(temp_dir)
+    logger('This is a test for test_log_imshow_complex', flush = True)
+    
+    mat = np.random.rand(100, 100) + 10 * 1j * np.random.rand(100, 100)
+    
+    logger(f'mat is complex? {np.iscomplexobj(mat)}')
+    logger.log_imshow('mat', mat)
+    
+    
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
-    
+    test_log_imshow_complex()
+    test_log_imshow()
     test_log_text()
-    exit()
     test_log_single_text()
     test_log_surface()
     test_log_single()
     test_lognflow_conflict_in_names()
     test_rename()
     test_log_plot()
     test_prepare_stack_of_images()
@@ -292,10 +302,10 @@
     test_log_var_without_time_stamp()
     test_log_var()
     test_log_animation()
     test_log_hist()
     test_log_scatter3()
     test_log_plt()
     test_log_hexbin()
-    test_log_imshow()
     test_log_canvas()
-    test_log_confusion_matrix()
+    test_log_confusion_matrix()
+    exit()
```

### Comparing `lognflow-0.7.4/tests/test_logviewer.py` & `lognflow-0.7.5/tests/test_logviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,12 +153,13 @@
     vec_out = logged.get_single('vec.npy')
     
     assert vec_out == vec
 
 if __name__ == '__main__':
     temp_dir = select_directory()
     test_get_single_specific_fname()
-    exit()
     test_get_images_as_stack()
     test_replace_time_with_index()
     test_logviewer()
-    test_text_to_object()
+    test_text_to_object()
+    exit()
+
```

### Comparing `lognflow-0.7.4/tests/test_printprogress.py` & `lognflow-0.7.5/tests/test_printprogress.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,23 +20,33 @@
 def test_content(response):
     """Sample pytest test function with the pytest fixture as an argument."""
     # from bs4 import BeautifulSoup
     # assert 'GitHub' in BeautifulSoup(response.content).title.string
 
 def test_printprogress():
     N = 15000000
-    pprog = printprogress(Ne)
+    pprog = printprogress(N)
     for _ in range(N):
         pprog()
     # assert input('Did it show you a progress bar? (y for yes)')=='y'
 
 def test_with_logger():
     logger = lognflow()
     N = 1500000
-    pprog = printprogress(Ne, print_function = logger, log_time_stamp = False)
+    pprog = printprogress(N, print_function = logger, log_time_stamp = False)
     for _ in range(N):
         pprog()
+        
+def test_ETA():
+    logger = lognflow()
+    N = 1500000
+    pprog = printprogress(N, print_function = None)
+    for _ in range(N):
+        ETA = pprog()
+        print(ETA)
+    
 
 if __name__ == '__main__':
+    test_ETA()
     test_printprogress()
     test_with_logger()
     exit()
```

