# Comparing `tmp/quantops-0.1.0.tar.gz` & `tmp/quantops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantops-0.1.0.tar", last modified: Thu Jun 22 12:53:15 2023, max compression
+gzip compressed data, was "quantops-0.2.0.tar", last modified: Tue Jun 27 16:38:59 2023, max compression
```

## Comparing `quantops-0.1.0.tar` & `quantops-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:53:15.792163 quantops-0.1.0/
--rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-22 12:53:15.792029 quantops-0.1.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      514 2023-06-22 12:50:49.000000 quantops-0.1.0/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:53:15.790916 quantops-0.1.0/quantops/
--rw-r--r--   0 simon      (501) staff       (20)       42 2023-06-02 14:53:07.000000 quantops-0.1.0/quantops/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2025 2023-06-22 10:37:01.000000 quantops-0.1.0/quantops/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)    21685 2023-06-22 10:45:12.000000 quantops-0.1.0/quantops/core.py
--rw-r--r--   0 simon      (501) staff       (20)      154 2023-06-22 10:49:07.000000 quantops-0.1.0/quantops/generate.py
--rw-r--r--   0 simon      (501) staff       (20)     9729 2023-06-22 10:27:38.000000 quantops-0.1.0/quantops/parser.py
--rw-r--r--   0 simon      (501) staff       (20)     8325 2023-06-22 10:34:04.000000 quantops-0.1.0/quantops/registry.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:53:15.791838 quantops-0.1.0/quantops.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-22 12:53:15.000000 quantops-0.1.0/quantops.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      295 2023-06-22 12:53:15.000000 quantops-0.1.0/quantops.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-22 12:53:15.000000 quantops-0.1.0/quantops.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       16 2023-06-22 12:53:15.000000 quantops-0.1.0/quantops.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-22 12:53:15.000000 quantops-0.1.0/quantops.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-22 12:53:15.792200 quantops-0.1.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.337011 quantops-0.2.0/
+-rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-27 16:38:59.336883 quantops-0.2.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      514 2023-06-27 16:38:11.000000 quantops-0.2.0/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.335916 quantops-0.2.0/quantops/
+-rw-r--r--   0 simon      (501) staff       (20)       42 2023-06-02 14:53:07.000000 quantops-0.2.0/quantops/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2025 2023-06-22 10:37:01.000000 quantops-0.2.0/quantops/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)    22009 2023-06-22 15:15:32.000000 quantops-0.2.0/quantops/core.py
+-rw-r--r--   0 simon      (501) staff       (20)      154 2023-06-22 10:49:07.000000 quantops-0.2.0/quantops/generate.py
+-rw-r--r--   0 simon      (501) staff       (20)     9729 2023-06-22 10:27:38.000000 quantops-0.2.0/quantops/parser.py
+-rw-r--r--   0 simon      (501) staff       (20)     8211 2023-06-22 15:17:43.000000 quantops-0.2.0/quantops/registry.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.336699 quantops-0.2.0/quantops.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      295 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       16 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-27 16:38:59.337044 quantops-0.2.0/setup.cfg
```

### Comparing `quantops-0.1.0/pyproject.toml` & `quantops-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quantops"
-version = "0.1.0"
+version = "0.2.0"
 
 description = "Tools to define, manipulate and format physical quantities"
 readme = "readme.md"
 license = { text = "EUPL-1.2" }
 requires-python = ">=3.11"
 
 dependencies = [
```

### Comparing `quantops-0.1.0/quantops/__main__.py` & `quantops-0.2.0/quantops/__main__.py`

 * *Files identical despite different names*

### Comparing `quantops-0.1.0/quantops/core.py` & `quantops-0.2.0/quantops/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,23 @@
   def find_context(self):
     for context in self.registry._contexts.values():
       if context.dimensionality == self.dimensionality:
         return context
 
     raise RuntimeError("No matching context")
 
+  def magnitude_as(self, unit: 'AtomicUnit'):
+    if self.dimensionality != unit.dimensionality:
+      raise ValueError("Operation with different dimensionalities")
+
+    if self.registry is not unit.registry:
+      raise ValueError("Operation with different registries")
+
+    return (self.value - unit.offset) / unit.value
+
   def __hash__(self):
     return hash((frozenset(sorted(self.dimensionality.items())), self.registry, self.value))
 
   def __eq__(self, other: Self, /):
     if not isinstance(other, self.__class__):
       return NotImplemented
```

### Comparing `quantops-0.1.0/quantops/parser.py` & `quantops-0.2.0/quantops/parser.py`

 * *Files identical despite different names*

### Comparing `quantops-0.1.0/quantops/registry.toml` & `quantops-0.2.0/quantops/registry.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,14 @@
   { factor = 1e-6, label = "micro", symbol = "\u00B5", symbol_names = ["\u00B5", "\u03BC", "u"] }, # U+00B5 => micro sign, U+03BC => greek letter mu
   { factor = 1e-9, label = "nano", symbol = "n" },
   { factor = 1e-12, label = "pico", symbol = "p" },
   { factor = 1e-15, label = "femto", symbol = "f" }
 ]
 
 [[prefix_systems]]
-name = "DeciSI"
-prefixes = [
-  { factor = 1e-1, label = "deci", symbol = "d" }
-]
-
-[[prefix_systems]]
 name = "BinaryMemory"
 prefixes = [
   { factor = 1_024, label = "kibi", symbol = "Ki" },
   { factor = 1_048_576, label = "mebi", symbol = "Mi" },
   { factor = 1_073_741_824, label = "gibi", symbol = "Gi" },
   { factor = 1_099_511_627_776, label = "tebi", symbol = "Ti" },
   { factor = 1_125_899_906_842_624, label = "pebi", symbol = "Pi" }
@@ -256,17 +250,16 @@
 dimensionality = { light = 1, solid_angle = 1 }
 label = ["lumen", "lumens"]
 prefixes = ["SI"]
 symbol = "lm"
 
 [[units]]
 dimensionality = {}
-label = ["bel", "bels"]
-symbol = "B"
-prefixes = ["DeciSI"]
+label = ["decibel", "decibels"]
+symbol = "dB"
 
 [[units]]
 dimensionality = { substance = 1 }
 label = ["mole", "moles"]
 prefixes = ["SI"]
 symbol = "mol"
```

