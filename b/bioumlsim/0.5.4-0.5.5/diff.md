# Comparing `tmp/bioumlsim-0.5.4.tar.gz` & `tmp/bioumlsim-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.5.4.tar", last modified: Tue Jun 27 12:01:51 2023, max compression
+gzip compressed data, was "bioumlsim-0.5.5.tar", last modified: Tue Jun 27 12:25:23 2023, max compression
```

## Comparing `bioumlsim-0.5.4.tar` & `bioumlsim-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:01:51.108767 bioumlsim-0.5.4/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.5.4/LICENSE
--rw-rw-rw-   0        0        0      771 2023-06-27 12:01:51.108767 bioumlsim-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:01:50.794910 bioumlsim-0.5.4/bioumlsim/
--rw-rw-rw-   0        0        0     6320 2023-06-27 11:59:59.000000 bioumlsim-0.5.4/bioumlsim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:01:51.098803 bioumlsim-0.5.4/bioumlsim/jars/
--rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
--rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
--rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/biouml.workbench_0.9.10.jar
--rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/colt.jar
--rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
--rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
--rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
--rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
--rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
--rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/org.apache.velocity_1.6.2.jar
--rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/org.json-20170516.jar
--rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
--rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
--rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
--rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
--rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
--rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
--rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/src.jar
--rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.5.4/bioumlsim/jars/streamex-0.7.0.jar
--rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.5.4/bioumlsim/test.py
--rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.5.4/bioumlsim/test.xml
-drwxrwxrwx   0        0        0        0 2023-06-27 12:01:50.945848 bioumlsim-0.5.4/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-06-27 12:01:50.000000 bioumlsim-0.5.4/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-06-27 12:01:50.000000 bioumlsim-0.5.4/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:01:50.000000 bioumlsim-0.5.4/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-27 12:01:49.000000 bioumlsim-0.5.4/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-06-27 12:01:50.000000 bioumlsim-0.5.4/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 12:01:50.000000 bioumlsim-0.5.4/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.5.4/pyproject.toml
--rw-rw-rw-   0        0        0      895 2023-06-27 12:01:51.113796 bioumlsim-0.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 12:25:23.278155 bioumlsim-0.5.5/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-06-27 12:25:23.279154 bioumlsim-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:25:23.167197 bioumlsim-0.5.5/bioumlsim/
+-rw-rw-rw-   0        0        0     6415 2023-06-27 12:24:35.000000 bioumlsim-0.5.5/bioumlsim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:25:23.275155 bioumlsim-0.5.5/bioumlsim/jars/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.5.5/bioumlsim/jars/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.5.5/bioumlsim/test.py
+-rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.5.5/bioumlsim/test.xml
+drwxrwxrwx   0        0        0        0 2023-06-27 12:25:23.206879 bioumlsim-0.5.5/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-06-27 12:25:23.000000 bioumlsim-0.5.5/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-06-27 12:25:23.000000 bioumlsim-0.5.5/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:25:23.000000 bioumlsim-0.5.5/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 12:01:49.000000 bioumlsim-0.5.5/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-06-27 12:25:23.000000 bioumlsim-0.5.5/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 12:25:23.000000 bioumlsim-0.5.5/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0      895 2023-06-27 12:25:23.294231 bioumlsim-0.5.5/setup.cfg
```

### Comparing `bioumlsim-0.5.4/LICENSE` & `bioumlsim-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/PKG-INFO` & `bioumlsim-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.5.4/bioumlsim/__init__.py` & `bioumlsim-0.5.5/bioumlsim/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,25 +47,28 @@
             if self.checkJDKVersion(ospath.join(jdkPath,'release')):
                 if verbose:
                     print('Appropriate version detected')
                 return jdkPath
         print('Can not find appropriate JDK in '+jdkBasePath)
         return '' 
          
-    def findJVM(self, possiblePathes, jdkLocation = '', verbose=False):
+    def findJVM(self, jdkLocation = '', verbose=False):
         jdk = jdkLocation
         if jdk == '':
             jdk = self.findJDK()
         if jdk == '':
             return jdk
         if verbose:
             print('JDK found at ' + jdk)
+        possiblePaths = self.guessJVMLocations()
         for possiblePath in possiblePathes:
-            jvm = ospath.join(jdk,possiblePath)
+            jvm = ospath.join(jdk, possiblePath)
+            print ('Check JVM location: '+jvm)
             if ospath.isfile(jvm):
+                print ('JVM Found')
                 return jvm;
         print('Can not find appropriate JVM. Please install 1.8 or 11 Java')
         return '' 
     
     def guessJVMLocations(self):
         systemName = platform.system()
         if systemName == 'Windows':
@@ -93,22 +96,22 @@
         except KeyError:
             return False
      
     def __init__(self, jdk = '', verbose = False):
         path = ospath.join(ospath.dirname(__file__),'jars')
         if verbose:
             print('Path to java classes: '+path)
+            print('Path to jdk: '+jdk)
         self.bioUMLPath = path
-        possiblePathes = self.guessJVMLocations()
         if jdk != '':
-            jvmPath = self.findJVM(possiblePathes, jdkLocation = jdk)
+            jvmPath = self.findJVM(jdkLocation = jdk, verbose)
         elif self.isJavaSet() and self.isJavaHomeSet(verbose):    
             jvmPath = ''
         else:
-            jvmPath = self.findJVM(possiblePathes)
+            jvmPath = self.findJVM(verbose)
         if jvmPath == '':
            if verbose:
                print('Will try to find jvm automatically') 
            jpype.startJVM(classpath=[path+'/*'], convertStrings=True)
         else:
            if verbose:
                print ('JVM is located at '+jvmPath)
```

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/biouml.workbench_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/biouml.workbench_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/colt.jar` & `bioumlsim-0.5.5/bioumlsim/jars/colt.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar` & `bioumlsim-0.5.5/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar` & `bioumlsim-0.5.5/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar` & `bioumlsim-0.5.5/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar` & `bioumlsim-0.5.5/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/org.apache.velocity_1.6.2.jar` & `bioumlsim-0.5.5/bioumlsim/jars/org.apache.velocity_1.6.2.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/org.json-20170516.jar` & `bioumlsim-0.5.5/bioumlsim/jars/org.json-20170516.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.access_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.access_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/ru.biosoft.math_0.9.10.jar` & `bioumlsim-0.5.5/bioumlsim/jars/ru.biosoft.math_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/src.jar` & `bioumlsim-0.5.5/bioumlsim/jars/src.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/jars/streamex-0.7.0.jar` & `bioumlsim-0.5.5/bioumlsim/jars/streamex-0.7.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim/test.xml` & `bioumlsim-0.5.5/bioumlsim/test.xml`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.5.5/bioumlsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.5.4/bioumlsim.egg-info/SOURCES.txt` & `bioumlsim-0.5.5/bioumlsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.4/setup.cfg` & `bioumlsim-0.5.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 352e 340d 0a61  rsion = 0.5.4..a
+00000020: 7273 696f 6e20 3d20 302e 352e 350d 0a61  rsion = 0.5.5..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
```

