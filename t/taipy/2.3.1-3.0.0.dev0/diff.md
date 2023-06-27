# Comparing `tmp/taipy-2.3.1.tar.gz` & `tmp/taipy-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.3.1.tar", last modified: Tue Jun 27 08:02:12 2023, max compression
+gzip compressed data, was "taipy-3.0.0.dev0.tar", last modified: Fri Jun 23 10:47:19 2023, max compression
```

## Comparing `taipy-2.3.1.tar` & `taipy-3.0.0.dev0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-27 08:00:21.000000 taipy-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 08:00:21.000000 taipy-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-27 08:02:12.286333 taipy-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-06-27 08:00:21.000000 taipy-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 08:00:21.000000 taipy-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:02:12.286333 taipy-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-27 08:00:21.000000 taipy-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.278333 taipy-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/src/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (123)    22398 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/gui_core/GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/gui_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/gui_core/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/src/taipy/gui_core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   658126 2023-06-27 08:02:03.000000 taipy-2.3.1/src/taipy/gui_core/lib/taipy-gui-core.js
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-27 08:00:21.000000 taipy-2.3.1/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:02:03.000000 taipy-2.3.1/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 08:02:12.000000 taipy-2.3.1/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:02:12.286333 taipy-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-27 08:00:21.000000 taipy-2.3.1/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-23 10:46:09.000000 taipy-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.926101 taipy-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.930101 taipy-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    22398 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   658126 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/tests/test_run.py
```

### Comparing `taipy-2.3.1/LICENSE` & `taipy-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/PKG-INFO` & `taipy-3.0.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.1
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -25,53 +25,55 @@
 License-File: LICENSE
 
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -100,66 +102,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -200,15 +202,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -226,21 +228,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.3.1/README.md` & `taipy-3.0.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -74,66 +76,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -174,15 +176,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -200,21 +202,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.3.1/setup.py` & `taipy-3.0.0.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "cookiecutter>=2.1.1,<2.2",
-    "taipy-gui>=2.3,<2.4",
-    "taipy-rest>=2.3,<2.4",
-    "taipy-templates>=2.3,<2.4",
+    "taipy-gui==3.0.0.dev0",
+    "taipy-rest==3.0.0.dev0",
+    "taipy-templates==3.0.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "ngrok": ["pyngrok>=5.1,<6.0"],
     "image": [
```

### Comparing `taipy-2.3.1/src/taipy/__init__.py` & `taipy-3.0.0.dev0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/_cli/__init__.py` & `taipy-3.0.0.dev0/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/_cli/_help_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/_cli/_scaffold_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/_entrypoint.py` & `taipy-3.0.0.dev0/src/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/_run.py` & `taipy-3.0.0.dev0/src/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/gui_core/GuiCoreLib.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/gui_core/__init__.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/gui_core/_init.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/gui_core/lib/taipy-gui-core.js` & `taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy/version.py` & `taipy-3.0.0.dev0/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/src/taipy.egg-info/PKG-INFO` & `taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.1
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -25,53 +25,55 @@
 License-File: LICENSE
 
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -100,66 +102,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -200,15 +202,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -226,21 +228,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.3.1/src/taipy.egg-info/SOURCES.txt` & `taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-2.3.1/tests/test_run.py` & `taipy-3.0.0.dev0/tests/test_run.py`

 * *Files identical despite different names*

