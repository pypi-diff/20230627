# Comparing `tmp/BLACKFORGE2-0.2.3.tar.gz` & `tmp/BLACKFORGE2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.2.3.tar", last modified: Fri Jun 23 04:07:31 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.2.4.tar", last modified: Tue Jun 27 04:43:46 2023, max compression
```

## Comparing `BLACKFORGE2-0.2.3.tar` & `BLACKFORGE2-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 04:07:31.014541 BLACKFORGE2-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-06-23 04:07:31.003883 BLACKFORGE2-0.2.3/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14640 2023-06-23 04:07:22.000000 BLACKFORGE2-0.2.3/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.3/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:07:31.012547 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      312 2023-06-23 04:07:30.000000 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-23 04:07:30.000000 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 04:07:30.000000 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 04:07:30.000000 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-23 04:07:30.000000 BLACKFORGE2-0.2.3/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      312 2023-06-23 04:07:31.014541 BLACKFORGE2-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-23 04:07:31.014541 BLACKFORGE2-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-06-23 04:07:26.000000 BLACKFORGE2-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:43:46.936049 BLACKFORGE2-0.2.4/
+drwxrwxrwx   0        0        0        0 2023-06-27 04:43:46.922039 BLACKFORGE2-0.2.4/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14672 2023-06-27 04:43:06.000000 BLACKFORGE2-0.2.4/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.4/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:43:46.934055 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-06-27 04:43:46.000000 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-27 04:43:46.000000 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 04:43:46.000000 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 04:43:46.000000 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 04:43:46.000000 BLACKFORGE2-0.2.4/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-06-27 04:43:46.935051 BLACKFORGE2-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-27 04:43:46.936049 BLACKFORGE2-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-06-27 04:43:32.000000 BLACKFORGE2-0.2.4/setup.py
```

### Comparing `BLACKFORGE2-0.2.3/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.2.4/BLACKFORGE2/FORGE.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,16 @@
 					self.frame_index = 0
 
 			else:
 				self.frame_index += 1
 
 			# reset the cumulative time for the next frame
 			self.current_time = 0
-
+		else:
+			self.frame_index = 0
 		# return the current frame of the animation list
 		return self.animation[self.frame_index]
 
 	def reset(self):
 		self.current_time = 0
 		self.frame_index = 0
 		self.done = False
```

### Comparing `BLACKFORGE2-0.2.3/LICENSE` & `BLACKFORGE2-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.2.3/README.rst` & `BLACKFORGE2-0.2.4/README.rst`

 * *Files identical despite different names*

