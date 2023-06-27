# Comparing `tmp/raisetool-0.1.15.tar.gz` & `tmp/raisetool-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raisetool-0.1.15.tar", max compression
+gzip compressed data, was "raisetool-1.0.0.tar", max compression
```

## Comparing `raisetool-0.1.15.tar` & `raisetool-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-05-09 11:26:38.487906 raisetool-0.1.15/LICENSE
--rw-r--r--   0        0        0     1968 2023-05-10 09:55:07.537199 raisetool-0.1.15/README.md
--rw-r--r--   0        0        0      646 2023-05-10 09:56:31.065175 raisetool-0.1.15/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 11:26:38.487906 raisetool-0.1.15/raisetool/__init__.py
--rw-r--r--   0        0        0     5239 2023-05-09 11:26:38.487906 raisetool-0.1.15/raisetool/formatter.py
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 raisetool-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 11:26:38.487906 raisetool-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1968 2023-05-10 09:55:07.537199 raisetool-1.0.0/README.md
+-rw-r--r--   0        0        0      645 2023-06-27 15:48:52.394469 raisetool-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 11:26:38.487906 raisetool-1.0.0/raisetool/__init__.py
+-rw-r--r--   0        0        0     6371 2023-06-27 15:44:13.897870 raisetool-1.0.0/raisetool/formatter.py
+-rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 raisetool-1.0.0/PKG-INFO
```

### Comparing `raisetool-0.1.15/LICENSE` & `raisetool-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raisetool-0.1.15/README.md` & `raisetool-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `raisetool-0.1.15/pyproject.toml` & `raisetool-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raisetool"
-version = "0.1.15"
+version = "1.0.0"
 description = "Rise class for formatting thrown exception messages."
 authors = ["Jacek Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Szumak75/RaiseTool"
 classifiers = [
         "Programming Language :: Python :: 3",
```

### Comparing `raisetool-0.1.15/raisetool/formatter.py` & `raisetool-1.0.0/raisetool/formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,14 +75,31 @@
         Return: ConnectionError
         """
         return ConnectionError(
             cls.message(message, class_name, currentframe)
         )
 
     @classmethod
+    def index_error(
+        cls,
+        message: str,
+        class_name: str = "",
+        currentframe: Optional[FrameType] = None,
+    ) -> IndexError:
+        """Return IndexError exception with formatted string.
+
+        message: str - message to format
+        class_name: str - caller class name (self.__class__.__name__)
+        currentframe: FrameType - object from inspect.currentframe()
+
+        Return: IndexError
+        """
+        return IndexError(cls.message(message, class_name, currentframe))
+
+    @classmethod
     def key_error(
         cls,
         message: str,
         class_name: str = "",
         currentframe: Optional[FrameType] = None,
     ) -> KeyError:
         """Return KeyError exception with formatted string.
@@ -92,14 +109,33 @@
         currentframe: FrameType - object from inspect.currentframe()
 
         Return: KeyError
         """
         return KeyError(cls.message(message, class_name, currentframe))
 
     @classmethod
+    def not_implemented_error(
+        cls,
+        message: str,
+        class_name: str = "",
+        currentframe: Optional[FrameType] = None,
+    ) -> NotImplementedError:
+        """Return NotImplementedError exception with formatted string.
+
+        message: str - message to format
+        class_name: str - caller class name (self.__class__.__name__)
+        currentframe: FrameType - object from inspect.currentframe()
+
+        Return: NotImplementedError
+        """
+        return NotImplementedError(
+            cls.message(message, class_name, currentframe)
+        )
+
+    @classmethod
     def os_error(
         cls,
         message: str,
         class_name: str = "",
         currentframe: Optional[FrameType] = None,
     ) -> OSError:
         """Return OSError exception with formatted string.
```

### Comparing `raisetool-0.1.15/PKG-INFO` & `raisetool-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raisetool
-Version: 0.1.15
+Version: 1.0.0
 Summary: Rise class for formatting thrown exception messages.
 Home-page: https://github.com/Szumak75/RaiseTool
 License: MIT
 Author: Jacek Kotlarski
 Author-email: szumak@virthost.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

