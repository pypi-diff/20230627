# Comparing `tmp/movie-rec-marking-aicore-0.1.5.tar.gz` & `tmp/movie-rec-marking-aicore-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-rec-marking-aicore-0.1.5.tar", last modified: Tue Jun 27 11:10:28 2023, max compression
+gzip compressed data, was "movie-rec-marking-aicore-0.1.6.tar", last modified: Tue Jun 27 12:34:44 2023, max compression
```

## Comparing `movie-rec-marking-aicore-0.1.5.tar` & `movie-rec-marking-aicore-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 11:10:28.941874 movie-rec-marking-aicore-0.1.5/
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-27 11:10:28.941874 movie-rec-marking-aicore-0.1.5/PKG-INFO
-drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 11:10:28.937874 movie-rec-marking-aicore-0.1.5/movie_rec_marking/
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/__init__.py
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     2099 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_1.py
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     7646 2023-06-13 15:18:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_2.py
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     5308 2023-05-12 11:04:27.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_3.py
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     6523 2023-06-27 11:07:37.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_4.py
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     9059 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_5.py
-drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 11:10:28.941874 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-27 11:10:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/PKG-INFO
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      467 2023-06-27 11:10:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/SOURCES.txt
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        1 2023-06-27 11:10:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/dependency_links.txt
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       26 2023-06-27 11:10:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/requires.txt
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       18 2023-06-27 11:10:28.000000 movie-rec-marking-aicore-0.1.5/movie_rec_marking_aicore.egg-info/top_level.txt
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       38 2023-06-27 11:10:28.941874 movie-rec-marking-aicore-0.1.5/setup.cfg
--rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      390 2023-06-27 11:10:11.000000 movie-rec-marking-aicore-0.1.5/setup.py
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 12:34:44.843926 movie-rec-marking-aicore-0.1.6/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-27 12:34:44.839926 movie-rec-marking-aicore-0.1.6/PKG-INFO
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 12:34:44.839926 movie-rec-marking-aicore-0.1.6/movie_rec_marking/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/__init__.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     2099 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_1.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     7646 2023-06-13 15:18:28.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_2.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     5308 2023-05-12 11:04:27.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_3.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     6266 2023-06-27 12:34:25.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_4.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     9059 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_5.py
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-27 12:34:44.839926 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-27 12:34:44.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/PKG-INFO
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      467 2023-06-27 12:34:44.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        1 2023-06-27 12:34:44.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       26 2023-06-27 12:34:44.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/requires.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       18 2023-06-27 12:34:44.000000 movie-rec-marking-aicore-0.1.6/movie_rec_marking_aicore.egg-info/top_level.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       38 2023-06-27 12:34:44.843926 movie-rec-marking-aicore-0.1.6/setup.cfg
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      390 2023-06-27 12:34:32.000000 movie-rec-marking-aicore-0.1.6/setup.py
```

### Comparing `movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_1.py` & `movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_1.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_2.py` & `movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_2.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_3.py` & `movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_3.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_4.py` & `movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_4.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,15 @@
         
     if not f.getvalue():
         print('The "get_user_genre_choice" function doesn\'t print anything')
         print('You have to print all the unique genres')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
     
-    source_lines = inspect.getsource(get_user_genre_choice)
-    try:
-        source_lines.index('get_unique_genres')
-    except ValueError:
-        print('The "get_user_genre_choice" function doesn\'t call the "get_unique_genres" function')
-        return False
+    
 
     print('Great! The "get_user_genre_choice" function prints the correct genre')
     print('You can continue to the next task')
     return True
 
 def check_get_movies_in_genre(first_movie, second_movie, third_movie, task_1):
     if not task_1:
```

### Comparing `movie-rec-marking-aicore-0.1.5/movie_rec_marking/test_milestone_5.py` & `movie-rec-marking-aicore-0.1.6/movie_rec_marking/test_milestone_5.py`

 * *Files identical despite different names*

