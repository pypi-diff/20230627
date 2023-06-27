# Comparing `tmp/learn_python_ceg_test-1.0.1.tar.gz` & `tmp/learn_python_ceg_test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learn_python_ceg_test-1.0.1.tar", last modified: Sun Jun 11 19:19:56 2023, max compression
+gzip compressed data, was "learn_python_ceg_test-1.0.2.tar", last modified: Mon Jun 12 08:46:16 2023, max compression
```

## Comparing `learn_python_ceg_test-1.0.1.tar` & `learn_python_ceg_test-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:19:55.999642 learn_python_ceg_test-1.0.1/
--rw-rw-rw-   0        0        0    35809 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1166 2023-06-11 19:19:56.000639 learn_python_ceg_test-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 19:19:55.986678 learn_python_ceg_test-1.0.1/learn_python_ceg_test/
--rw-rw-rw-   0        0        0      289 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test/__init__.py
--rw-rw-rw-   0        0        0     9568 2023-06-11 18:54:51.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test/check_answers.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:19:55.998644 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-06-11 19:19:55.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-11 19:19:55.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:19:55.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 19:19:55.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-11 19:19:55.000000 learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 19:19:56.001637 learn_python_ceg_test-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1875 2023-06-11 19:19:43.000000 learn_python_ceg_test-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:46:16.542442 learn_python_ceg_test-1.0.2/
+-rw-rw-rw-   0        0        0    35809 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1166 2023-06-12 08:46:16.542442 learn_python_ceg_test-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 08:46:16.535654 learn_python_ceg_test-1.0.2/learn_python_ceg_test/
+-rw-rw-rw-   0        0        0      289 2023-06-11 18:53:14.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test/__init__.py
+-rw-rw-rw-   0        0        0     9191 2023-06-12 08:33:13.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test/check_answers.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:46:16.541448 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-06-12 08:46:16.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-12 08:46:16.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:46:16.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 08:46:16.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-12 08:46:16.000000 learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 08:46:16.543449 learn_python_ceg_test-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1875 2023-06-12 08:45:14.000000 learn_python_ceg_test-1.0.2/setup.py
```

### Comparing `learn_python_ceg_test-1.0.1/LICENSE.txt` & `learn_python_ceg_test-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `learn_python_ceg_test-1.0.1/PKG-INFO` & `learn_python_ceg_test-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: learn_python_ceg_test
-Version: 1.0.1
+Version: 1.0.2
 Summary: learn_python check answers
 Home-page: https://github.com/mike-mendoza/learn_python_ceg_test
-Download-URL: https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.2.tar.gz
 Author: Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat
 Author-email: mendozalugo@gmail.com
 License: GNU
 Project-URL: Bug Tracker, https://github.com/mike-mendoza/learn_python_ceg_test/issues
 Keywords: pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `learn_python_ceg_test-1.0.1/learn_python_ceg_test/check_answers.py` & `learn_python_ceg_test-1.0.2/learn_python_ceg_test/check_answers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,189 +1,173 @@
 from math import pi,sqrt 
 import pandas as pd
 
-file_location = ("https://raw.githubusercontent.com/TUDelft-CITG/"
-                "learn-python/mike/book/06/Exercises/")
 
 
 ###================== NOTEBOOK 3=====================
-def notebook_3_check_answer(question_number):
+def notebook_3(question_number,arguments):
+    """This function checks the answers for notebook 3.
+    It takes two arguments:
+    - question_number: the question number to check
+    - arguments: a list of arguments to pass to the function"""
 
     if question_number == 0:
+        car_info=arguments[0]
+        message=arguments[1]
         try: 
             assert car_info[
                 'top_speed'] in message and car_info[
                     'type'] in message, 'Incorrect answer.'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 1:
+        angle=arguments[0]
+        DegToRad = arguments[1]
         try: 
             assert type(
                 DegToRad) == type(
                 lambda x:x) and abs(
                 DegToRad(
                 angle) - angle*pi/180) <= 1e-6, 'Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 2:
+        distance=arguments[0]
         try: 
             assert abs(
-                Distance(
+                distance(
                 1, 1, 3, 3) - 2 * sqrt(
                 2)) <= 1e-6, '3.2.2 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
     
     elif question_number == 3:
+        get_abbreviation=arguments[0]
         try: 
             assert get_abbreviation(   
             ) == "AES", '3.4.1 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 4:
+        create_string_from_lists = arguments[0]
         try: 
             assert "B[3] = 8" in create_string_from_lists(
             ), '3.4.2 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 5:
+        factorial = arguments[0]
         try: 
             assert factorial(
                 5) == 120, '3.4.3 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')   
 
 ###==================NOTEBOOK 4=====================
-def notebook_4_check_answer(question_number):
-
+def notebook_4(question_number,arguments):
+    """This function checks the answers for notebook 4.
+    It takes two arguments:
+    - question_number: the question number to check
+    - arguments: a list of arguments to pass to the function"""
+    
     if question_number == 0:
+        get_display_temperature=arguments[0]
         try:
             assert get_display_temperature(
                 [100]) == [
                     "-173.150  °C | -279.670  °F (ID=0)"
                     ], '4.1.1 - Incorrect answer' 
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 1:
+        prepare_template=arguments[0]
         default_bands = ['B1', 'B2', 'B3', 'B4', 
                          'B5', 'B6', 'B7']
         d1 = prepare_template(default_bands, 'normal')
         d2 = prepare_template(default_bands, 'extended')
         d3 = prepare_template(default_bands, 'normal')
         try: 
             assert  d2['bands'] == ['B1', 'B2', 'B3', 'B4', 
                                    'B5', 'B6', 'B7', 'B8', 'B8A'] and \
                     d3['bands'] == ['B1', 'B2', 'B3', 'B4', 'B5', 
                         'B6', 'B7'], '4.1.2 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
-###==================SOLUTIONS TEMPLATE=====================
-
-###---------QUESTION 0 --------
-# import time
-
-# def get_display_temperature(temp_k):
-#     #copying temporarily temp_k to temp_c
-#     temp_c = temp_k.copy()
-    
-#     #converting kelvins to celsius
-#     for i in range(len(temp_c)):
-#         temp_c[i] = temp_c[i] - 273.15
-        
-#     #copying temporarily temp_k to temp_f
-#     temp_f = temp_k.copy()
-    
-#     #converting kelvins to fahrenheit
-#     for i in range(len(temp_f)):
-#         temp_f[i] = (temp_f[i] - 273.15) * (9 / 5) + 32
-    
-#     #now, creating display messages from the converted temperatures
-#     display_messages = []
-#     for i in range(len(temp_k)):
-#         msg = f"{temp_c[i]:<10.3f}°C | {temp_f[i]:<10.3f}°F (ID={i})"
-#         display_messages.append(msg)
-        
-#     return display_messages
-###------------END SOLUTION---------------------
-
-###---------QUESTION 1 --------
-# def prepare_template(default_bands, observation_mode):  
-#     #creating metadata for the upcoming observations
-#     template = {'time': time.ctime(time.time()),
-#                'observation_mode': observation_mode,
-#                'bands': default_bands.copy()}
-    
-#     #adding additional bands for the extended mode
-#     if observation_mode == 'normal':
-#         #no need to add bands
-#         pass
-#     elif observation_mode == 'extended':
-#         template['bands'] += ['B8', 'B8A']
-#     else:
-#         #if the mode is unknonw - raise a RuntimeError
-#         raise RuntimeError(f'Failed to identify observation mode: {observation_mode}')
-        
-#     return template
-###------------END SOLUTION---------------------       
-# 
-###===========================================================
 
 ###==================NOTEBOOK 6=====================
 
+file_location = ("https://raw.githubusercontent.com/TUDelft-CITG/"
+                "learn-python/mike/book/06/Exercises/")
+
 def solution_6_2_1(series):
     series_types = "Types inside series:\n"
     for i in range(len(series)):
         item_type = type(series[i])
         series_types += str(item_type) + '\n'
     return series_types
 
-def notebook_6_check_answer(question_number):
+def notebook_6(question_number,arguments):
+    """This function checks the answers for notebook 6.
+    It takes two arguments:
+    - question_number: the question number to check
+    - arguments: a list of arguments to pass to the function"""
 
     if question_number == 0:
+        list_types = arguments[0]
         my_list = ['begin', 2, 3/4, "end"]
         my_series = pd.Series(data=my_list)
         try: 
             assert list_types(
                 my_series) == solution_6_2_1(
                 my_series), '6.2.1 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 1:
+        count_nans = arguments[0]
+        mineral_properties=arguments[1]
         try: 
             assert count_nans(
                 mineral_properties) == 12,'Incorrect'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 2:
+        count_minerals = arguments[0]
+        mineral_properties=arguments[1]
         try: 
             assert count_minerals(
                 mineral_properties, 4) == 7, 'Incorrect'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
     
     elif question_number == 3:
+        mountains_8000 = arguments[0]
+        cols = arguments[1]
+        max_height = arguments[2]
+        index_max = arguments[3]
+        tallest_mountain = arguments[4]
+
         df_sol = pd.read_csv(file_location + 'tallest_mountains.csv')
         cols_sol = df_sol.columns
         max_height_sol = df_sol['Metres'].max() 
         indxmax_sol = df_sol['Metres'].idxmax() 
         tallest_mountain_sol = df_sol.loc[indxmax_sol,'Mountain']
         try: 
             assert df_sol.equals(
@@ -192,14 +176,16 @@
         indxmax_sol == index_max and tallest_mountain_sol == tallest_mountain, \
     '6.5.1 - Incorrect answer, did you use idxmax for the 4th problem?'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 4:
+        df_reset = arguments[0]
+
         df_sol = pd.read_csv(file_location + 'tallest_mountains.csv')
 
         df7000_sol = pd.read_csv(
             file_location + 'mountains_above_7000m.csv', encoding_errors='ignore') # 1
         df_concat_sol = pd.concat([df7000_sol,df_sol]) # 2
         df_concat_norange_sol = df_concat_sol .drop('Range', axis=1) # 3
         df_reset_sol = df_concat_norange_sol.reset_index(drop=True) # 4
@@ -221,14 +207,15 @@
             assert df_reset_sol.equals(df_reset) or \
                 or_df_reset_sol.equals(df_reset), '6.5.2 - Incorrect answer'
             print('Correct answer :D')
         except AssertionError:
             print('Incorrect answer :(')
 
     elif question_number == 5:
+        china_mountains = arguments[0]
         df_sol = pd.read_csv(file_location + 'tallest_mountains.csv')
 
         df7000_sol = pd.read_csv(
             file_location + 'mountains_above_7000m.csv', encoding_errors='ignore') # 1
         df7000_norange_sol = df7000_sol.drop('Range', axis=1) # 2
         df_concat_sol = pd.concat([df7000_norange_sol,df_sol]) # 3
         df_reset_sol = df_concat_sol.reset_index(drop=True) # 4
```

### Comparing `learn_python_ceg_test-1.0.1/learn_python_ceg_test.egg-info/PKG-INFO` & `learn_python_ceg_test-1.0.2/learn_python_ceg_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: learn-python-ceg-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: learn_python check answers
 Home-page: https://github.com/mike-mendoza/learn_python_ceg_test
-Download-URL: https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.2.tar.gz
 Author: Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat
 Author-email: mendozalugo@gmail.com
 License: GNU
 Project-URL: Bug Tracker, https://github.com/mike-mendoza/learn_python_ceg_test/issues
 Keywords: pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `learn_python_ceg_test-1.0.1/setup.py` & `learn_python_ceg_test-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='learn_python_ceg_test',                           # should match the package folder
     packages=['learn_python_ceg_test'],                   # should match the package folder
-    version='1.0.1',                              # important for updates
+    version='1.0.2',                              # important for updates
     license='GNU',                                  # should match your chosen license
     description='learn_python check answers',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat',
     author_email='mendozalugo@gmail.com',
     url='https://github.com/mike-mendoza/learn_python_ceg_test', 
@@ -27,9 +27,9 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     
-    download_url="https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.1.tar.gz",
+    download_url="https://github.com/mike-mendoza/learn_python_ceg_test/archive/refs/tags/v1.0.2.tar.gz",
 )
```

