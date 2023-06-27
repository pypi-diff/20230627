# Comparing `tmp/pyidi-0.26.tar.gz` & `tmp/pyidi-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyidi-0.26.tar", last modified: Mon Dec  5 14:10:45 2022, max compression
+gzip compressed data, was "pyidi-0.27.tar", last modified: Tue Jun 27 09:36:29 2023, max compression
```

## Comparing `pyidi-0.26.tar` & `pyidi-0.27.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 14:10:45.134298 pyidi-0.26/
--rw-rw-rw-   0        0        0     1091 2019-02-22 08:54:16.000000 pyidi-0.26/LICENSE
--rw-rw-rw-   0        0        0     2426 2022-12-05 14:10:45.134298 pyidi-0.26/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2021-09-06 11:05:30.000000 pyidi-0.26/README.md
-drwxrwxrwx   0        0        0        0 2022-12-05 14:10:45.037489 pyidi-0.26/pyIDI.egg-info/
--rw-rw-rw-   0        0        0     2426 2022-12-05 14:10:44.000000 pyidi-0.26/pyIDI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2022-12-05 14:10:44.000000 pyidi-0.26/pyIDI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-05 14:10:44.000000 pyidi-0.26/pyIDI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2022-12-05 14:10:44.000000 pyidi-0.26/pyIDI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-05 14:10:44.000000 pyidi-0.26/pyIDI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-05 14:10:45.065077 pyidi-0.26/pyidi/
--rw-rw-rw-   0        0        0      139 2022-12-05 13:50:11.000000 pyidi-0.26/pyidi/__init__.py
--rw-rw-rw-   0        0        0    13426 2021-09-02 05:16:45.000000 pyidi-0.26/pyidi/gui.py
--rw-rw-rw-   0        0        0     1542 2021-03-26 05:29:39.000000 pyidi-0.26/pyidi/load_analysis.py
-drwxrwxrwx   0        0        0        0 2022-12-05 14:10:45.133381 pyidi-0.26/pyidi/methods/
--rw-rw-rw-   0        0        0      300 2021-03-26 05:29:39.000000 pyidi-0.26/pyidi/methods/__init__.py
--rw-rw-rw-   0        0        0     7249 2020-01-15 05:56:01.000000 pyidi-0.26/pyidi/methods/_gradient_based_optical_flow.py
--rw-rw-rw-   0        0        0    28623 2022-12-05 13:50:11.000000 pyidi-0.26/pyidi/methods/_lucas_kanade.py
--rw-rw-rw-   0        0        0    10092 2020-02-05 07:02:01.000000 pyidi-0.26/pyidi/methods/_lucas_kanade_scipy.py
--rw-rw-rw-   0        0        0    25982 2021-03-26 05:29:39.000000 pyidi-0.26/pyidi/methods/_lucas_kanade_scipy2.py
--rw-rw-rw-   0        0        0    15146 2021-09-02 05:16:45.000000 pyidi-0.26/pyidi/methods/_simplified_optical_flow.py
--rw-rw-rw-   0        0        0      979 2021-03-26 05:29:39.000000 pyidi-0.26/pyidi/methods/idi_method.py
--rw-rw-rw-   0        0        0    20510 2022-12-05 13:50:11.000000 pyidi-0.26/pyidi/pyidi.py
--rw-rw-rw-   0        0        0    15246 2021-09-02 05:16:45.000000 pyidi-0.26/pyidi/selection.py
--rw-rw-rw-   0        0        0    12391 2021-09-02 05:16:45.000000 pyidi-0.26/pyidi/tools.py
--rw-rw-rw-   0        0        0       42 2022-12-05 14:10:45.135294 pyidi-0.26/setup.cfg
--rw-rw-rw-   0        0        0     2086 2021-03-26 05:29:39.000000 pyidi-0.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:36:29.121538 pyidi-0.27/
+-rw-rw-rw-   0        0        0     1091 2019-02-20 08:10:56.000000 pyidi-0.27/LICENSE
+-rw-rw-rw-   0        0        0     2426 2023-06-27 09:36:29.120529 pyidi-0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2022-12-05 12:21:04.000000 pyidi-0.27/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:36:29.052770 pyidi-0.27/pyIDI.egg-info/
+-rw-rw-rw-   0        0        0     2426 2023-06-27 09:36:28.000000 pyidi-0.27/pyIDI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-06-27 09:36:28.000000 pyidi-0.27/pyIDI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:36:28.000000 pyidi-0.27/pyIDI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-06-27 09:36:28.000000 pyidi-0.27/pyIDI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 09:36:28.000000 pyidi-0.27/pyIDI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 09:36:29.079160 pyidi-0.27/pyidi/
+-rw-rw-rw-   0        0        0      139 2023-06-27 09:28:28.000000 pyidi-0.27/pyidi/__init__.py
+-rw-rw-rw-   0        0        0    13426 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/gui.py
+-rw-rw-rw-   0        0        0     1542 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/load_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:36:29.119356 pyidi-0.27/pyidi/methods/
+-rw-rw-rw-   0        0        0      300 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/methods/__init__.py
+-rw-rw-rw-   0        0        0    28718 2023-05-12 07:09:05.000000 pyidi-0.27/pyidi/methods/_dic_rigid.py
+-rw-rw-rw-   0        0        0     7249 2020-01-30 09:26:50.000000 pyidi-0.27/pyidi/methods/_gradient_based_optical_flow.py
+-rw-rw-rw-   0        0        0    28707 2023-06-27 09:22:37.000000 pyidi-0.27/pyidi/methods/_lucas_kanade.py
+-rw-rw-rw-   0        0        0    10092 2020-06-18 08:17:48.000000 pyidi-0.27/pyidi/methods/_lucas_kanade_scipy.py
+-rw-rw-rw-   0        0        0    25982 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/methods/_lucas_kanade_scipy2.py
+-rw-rw-rw-   0        0        0    15146 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/methods/_simplified_optical_flow.py
+-rw-rw-rw-   0        0        0      979 2020-06-18 08:41:54.000000 pyidi-0.27/pyidi/methods/idi_method.py
+-rw-rw-rw-   0        0        0    20562 2023-06-27 09:25:38.000000 pyidi-0.27/pyidi/pyidi.py
+-rw-rw-rw-   0        0        0    15246 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/selection.py
+-rw-rw-rw-   0        0        0    12391 2022-12-05 12:21:05.000000 pyidi-0.27/pyidi/tools.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:36:29.121538 pyidi-0.27/setup.cfg
+-rw-rw-rw-   0        0        0     2086 2020-06-18 08:41:54.000000 pyidi-0.27/setup.py
```

### Comparing `pyidi-0.26/LICENSE` & `pyidi-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/PKG-INFO` & `pyidi-0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyidi
-Version: 0.26
+Version: 0.27
 Summary: Python Image Displacement Identification.
 Home-page: https://github.com/ladisk/pyidi
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič
 Author-email: janko.slavic@fs.uni-lj.si, ladisk@gmail.com
 License: UNKNOWN
 Keywords: computer vision dic gradient-based image identification
 Platform: UNKNOWN
```

### Comparing `pyidi-0.26/README.md` & `pyidi-0.27/README.md`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyIDI.egg-info/PKG-INFO` & `pyidi-0.27/pyIDI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyidi
-Version: 0.26
+Version: 0.27
 Summary: Python Image Displacement Identification.
 Home-page: https://github.com/ladisk/pyidi
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič
 Author-email: janko.slavic@fs.uni-lj.si, ladisk@gmail.com
 License: UNKNOWN
 Keywords: computer vision dic gradient-based image identification
 Platform: UNKNOWN
```

### Comparing `pyidi-0.26/pyIDI.egg-info/SOURCES.txt` & `pyidi-0.27/pyIDI.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 pyidi/tools.py
 pyidi.egg-info/PKG-INFO
 pyidi.egg-info/SOURCES.txt
 pyidi.egg-info/dependency_links.txt
 pyidi.egg-info/requires.txt
 pyidi.egg-info/top_level.txt
 pyidi/methods/__init__.py
+pyidi/methods/_dic_rigid.py
 pyidi/methods/_gradient_based_optical_flow.py
 pyidi/methods/_lucas_kanade.py
 pyidi/methods/_lucas_kanade_scipy.py
 pyidi/methods/_lucas_kanade_scipy2.py
 pyidi/methods/_simplified_optical_flow.py
 pyidi/methods/idi_method.py
```

### Comparing `pyidi-0.26/pyidi/gui.py` & `pyidi-0.27/pyidi/gui.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/load_analysis.py` & `pyidi-0.27/pyidi/load_analysis.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/methods/_gradient_based_optical_flow.py` & `pyidi-0.27/pyidi/methods/_gradient_based_optical_flow.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/methods/_lucas_kanade.py` & `pyidi-0.27/pyidi/methods/_lucas_kanade.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,15 +428,15 @@
 
         fig, ax = plt.subplots(figsize=figsize)
         ax.imshow(video.mraw[0].astype(float), cmap=cmap)
         ax.scatter(video.points[:, 1],
                    video.points[:, 0], marker='.', color=color)
 
         for point in video.points:
-            roi_border = patches.Rectangle((point - self.roi_size//2)[::-1], self.roi_size[1], self.roi_size[0],
+            roi_border = patches.Rectangle((point - self.roi_size//2 - 0.5)[::-1], self.roi_size[1], self.roi_size[0],
                                             linewidth=1, edgecolor=color, facecolor='none')
             ax.add_patch(roi_border)
 
         plt.grid(False)
         plt.show()
 
 
@@ -457,17 +457,20 @@
             if self.process_number == 0:
                 shutil.rmtree(temp_dir)
                 os.mkdir(temp_dir)
         
         if self.process_number == 0:
             # Write all the settings of the analysis
             settings = self._make_comparison_dict()
-            pickle.dump(settings, open(self.settings_filename, 'wb'))
+            with open(self.settings_filename, 'wb') as f:
+                pickle.dump(settings, f)
+            
             self.points_filename = os.path.join(temp_dir, 'points.pkl')
-            pickle.dump(self.video.points, open(self.points_filename, 'wb'))
+            with open(self.points_filename, 'wb') as f:
+                pickle.dump(self.video.points, f)
 
         if not init_multi:
             token = f'{self.process_number:0>3.0f}'
 
             self.process_log = os.path.join(temp_dir, 'process_log_' + token + '.txt')
             self.points_filename = os.path.join(temp_dir, 'points.pkl')
             self.disp_filename = os.path.join(temp_dir, 'disp_' + token + '.pkl')
@@ -478,15 +481,15 @@
                     f'token: {token}\n',
                     f'points_filename: {self.points_filename}\n',
                     f'disp_filename: {self.disp_filename}\n',
                     f'disp_shape: {(self.video.points.shape[0], self.N_time_points, 2)}\n',
                     f'analysis_run <{self.analysis_run}>:'
                 ])
 
-            self.temp_disp = np.memmap(self.disp_filename, dtype=np.float, mode='w+', shape=(self.video.points.shape[0], self.N_time_points, 2))
+            self.temp_disp = np.memmap(self.disp_filename, dtype=np.float64, mode='w+', shape=(self.video.points.shape[0], self.N_time_points, 2))
             
 
     def clear_temp_files(self):
         """Clearing the temporary files.
         """
         shutil.rmtree(self.temp_dir)
 
@@ -526,15 +529,15 @@
         self.disp_filename = os.path.join(temp_dir, 'disp_' + token + '.pkl')
 
         with open(self.process_log, 'r', encoding='utf-8') as f:
             log = f.readlines()
 
         shape = tuple([int(_) for _ in log[4].replace(' ', '').split(':')[1].replace('(', '').replace(')', '').split(',')])
  
-        self.temp_disp = np.memmap(self.disp_filename, dtype=np.float, mode='r+', shape=shape)
+        self.temp_disp = np.memmap(self.disp_filename, dtype=np.float64, mode='r+', shape=shape)
         self.displacements = np.array(self.temp_disp).copy()
 
         self.start_time = int(log[-1].replace(' ', '').rstrip().split('\t')[1].split(':')[1]) + 1
         self.analysis_run = int(log[-1].split('<')[1].split('>')[0]) + 1
 
 
     def temp_files_check(self):
```

### Comparing `pyidi-0.26/pyidi/methods/_lucas_kanade_scipy.py` & `pyidi-0.27/pyidi/methods/_lucas_kanade_scipy.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/methods/_lucas_kanade_scipy2.py` & `pyidi-0.27/pyidi/methods/_lucas_kanade_scipy2.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/methods/_simplified_optical_flow.py` & `pyidi-0.27/pyidi/methods/_simplified_optical_flow.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/methods/idi_method.py` & `pyidi-0.27/pyidi/methods/idi_method.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/pyidi.py` & `pyidi-0.27/pyidi/pyidi.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,18 @@
             n = 0
         self.root_this_analysis = os.path.join(self.root_analysis, f'analysis_{n+1:0>3.0f}')
         
         os.mkdir(self.root_this_analysis)
 
     
     def save(self, root=''):
-        pickle.dump(self.displacements, open(os.path.join(root, 'results.pkl'), 'wb'), protocol=-1)
-        pickle.dump(self.points, open(os.path.join(root, 'points.pkl'), 'wb'), protocol=-1)
+        with open(os.path.join(root, 'results.pkl'), 'wb') as f:
+            pickle.dump(self.displacements, f, protocol=-1)
+        with open(os.path.join(root, 'points.pkl'), 'wb') as f:
+            pickle.dump(self.points, f, protocol=-1)
 
         out = {
             'info': self.info,
             'createdate': datetime.datetime.now().strftime("%Y %m %d    %H:%M:%S"),
             'cih_file': self.cih_file,
             'settings': self.method.create_settings_dict(),
             'method': self.method_name
```

### Comparing `pyidi-0.26/pyidi/selection.py` & `pyidi-0.27/pyidi/selection.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/pyidi/tools.py` & `pyidi-0.27/pyidi/tools.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.26/setup.py` & `pyidi-0.27/setup.py`

 * *Files identical despite different names*

