# Comparing `tmp/systemPY-0.0.8.tar.gz` & `tmp/systemPY-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemPY-0.0.8.tar", last modified: Sat Dec  3 00:49:34 2022, max compression
+gzip compressed data, was "systemPY-0.0.9.tar", last modified: Wed Dec  7 16:51:37 2022, max compression
```

## Comparing `systemPY-0.0.8.tar` & `systemPY-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.153524 systemPY-0.0.8/
--rw-r--r--   0 kai       (1000) kai       (1000)     4185 2022-12-03 00:49:34.153524 systemPY-0.0.8/PKG-INFO
--rw-r--r--   0 kai       (1000) kai       (1000)     2783 2022-08-18 19:35:06.000000 systemPY-0.0.8/README.md
--rw-r--r--   0 kai       (1000) kai       (1000)      323 2022-11-27 21:35:01.000000 systemPY-0.0.8/pyproject.toml
--rw-r--r--   0 kai       (1000) kai       (1000)       38 2022-12-03 00:49:34.153524 systemPY-0.0.8/setup.cfg
--rw-r--r--   0 kai       (1000) kai       (1000)     1752 2022-11-29 18:44:54.000000 systemPY-0.0.8/setup.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.145524 systemPY-0.0.8/systemPY.egg-info/
--rw-r--r--   0 kai       (1000) kai       (1000)     4185 2022-12-03 00:49:34.000000 systemPY-0.0.8/systemPY.egg-info/PKG-INFO
--rw-r--r--   0 kai       (1000) kai       (1000)     1010 2022-12-03 00:49:34.000000 systemPY-0.0.8/systemPY.egg-info/SOURCES.txt
--rw-r--r--   0 kai       (1000) kai       (1000)        1 2022-12-03 00:49:34.000000 systemPY-0.0.8/systemPY.egg-info/dependency_links.txt
--rw-r--r--   0 kai       (1000) kai       (1000)       16 2022-12-03 00:49:34.000000 systemPY-0.0.8/systemPY.egg-info/requires.txt
--rw-r--r--   0 kai       (1000) kai       (1000)        9 2022-12-03 00:49:34.000000 systemPY-0.0.8/systemPY.egg-info/top_level.txt
--rw-r--r--   0 kai       (1000) kai       (1000)        1 2022-11-06 14:36:29.000000 systemPY-0.0.8/systemPY.egg-info/zip-safe
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.145524 systemPY-0.0.8/systempy/
--rw-r--r--   0 kai       (1000) kai       (1000)      362 2022-12-02 12:46:41.000000 systemPY-0.0.8/systempy/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1251 2022-11-27 21:46:48.000000 systemPY-0.0.8/systempy/daemon.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.149524 systemPY-0.0.8/systempy/ext/
--rw-r--r--   0 kai       (1000) kai       (1000)        0 2022-08-08 18:09:34.000000 systemPY-0.0.8/systempy/ext/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)      608 2022-11-27 21:46:48.000000 systemPY-0.0.8/systempy/ext/celery.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1017 2022-12-02 01:10:30.000000 systemPY-0.0.8/systempy/ext/pretty_repl.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1463 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/ext/ptrepl.py
--rw-r--r--   0 kai       (1000) kai       (1000)      496 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/ext/starlette.py
--rw-r--r--   0 kai       (1000) kai       (1000)      517 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/ext/target_ext.py
--rw-r--r--   0 kai       (1000) kai       (1000)      631 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/loop.py
--rw-r--r--   0 kai       (1000) kai       (1000)     6070 2022-11-05 21:05:00.000000 systemPY-0.0.8/systempy/mypy.py
--rw-r--r--   0 kai       (1000) kai       (1000)      263 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/process.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.149524 systemPY-0.0.8/systempy/repl/
--rw-r--r--   0 kai       (1000) kai       (1000)       52 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/repl/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1627 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/repl/handle_interrupt.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1140 2022-12-02 01:09:48.000000 systemPY-0.0.8/systempy/repl/mixins.py
--rw-r--r--   0 kai       (1000) kai       (1000)     3987 2022-12-02 01:09:39.000000 systemPY-0.0.8/systempy/repl/repl.py
--rw-r--r--   0 kai       (1000) kai       (1000)      102 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/repl/typing.py
--rw-r--r--   0 kai       (1000) kai       (1000)      649 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/repl/util.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2394 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/target.py
--rw-r--r--   0 kai       (1000) kai       (1000)      213 2022-11-27 21:46:49.000000 systemPY-0.0.8/systempy/unit.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1002 2022-12-02 17:32:12.000000 systemPY-0.0.8/systempy/unit_meta.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-03 00:49:34.153524 systemPY-0.0.8/systempy/util/
--rw-r--r--   0 kai       (1000) kai       (1000)      292 2022-10-27 18:16:32.000000 systemPY-0.0.8/systempy/util/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1827 2022-12-02 01:14:30.000000 systemPY-0.0.8/systempy/util/callback_plan.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1456 2022-12-02 01:14:34.000000 systemPY-0.0.8/systempy/util/check.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1741 2022-12-02 01:14:40.000000 systemPY-0.0.8/systempy/util/configuration.py
--rw-r--r--   0 kai       (1000) kai       (1000)      684 2022-12-02 01:14:44.000000 systemPY-0.0.8/systempy/util/constants.py
--rw-r--r--   0 kai       (1000) kai       (1000)      696 2022-12-02 01:14:49.000000 systemPY-0.0.8/systempy/util/creation.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2198 2022-12-02 01:13:42.000000 systemPY-0.0.8/systempy/util/extraction.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2156 2022-12-02 01:14:38.000000 systemPY-0.0.8/systempy/util/handler_type.py
--rw-r--r--   0 kai       (1000) kai       (1000)      802 2022-12-02 01:14:59.000000 systemPY-0.0.8/systempy/util/local_dataclasses.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1469 2022-12-02 01:14:22.000000 systemPY-0.0.8/systempy/util/local_typing.py
--rw-r--r--   0 kai       (1000) kai       (1000)     3738 2022-12-02 01:13:17.000000 systemPY-0.0.8/systempy/util/misc.py
--rw-r--r--   0 kai       (1000) kai       (1000)     3082 2022-12-02 01:15:46.000000 systemPY-0.0.8/systempy/util/register.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.699932 systemPY-0.0.9/
+-rw-r--r--   0 kai       (1000) kai       (1000)     4185 2022-12-07 16:51:37.699932 systemPY-0.0.9/PKG-INFO
+-rw-r--r--   0 kai       (1000) kai       (1000)     2783 2022-08-18 19:35:06.000000 systemPY-0.0.9/README.md
+-rw-r--r--   0 kai       (1000) kai       (1000)      323 2022-11-27 21:35:01.000000 systemPY-0.0.9/pyproject.toml
+-rw-r--r--   0 kai       (1000) kai       (1000)       38 2022-12-07 16:51:37.699932 systemPY-0.0.9/setup.cfg
+-rw-r--r--   0 kai       (1000) kai       (1000)     1752 2022-11-29 18:44:54.000000 systemPY-0.0.9/setup.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.687932 systemPY-0.0.9/systemPY.egg-info/
+-rw-r--r--   0 kai       (1000) kai       (1000)     4185 2022-12-07 16:51:37.000000 systemPY-0.0.9/systemPY.egg-info/PKG-INFO
+-rw-r--r--   0 kai       (1000) kai       (1000)     1010 2022-12-07 16:51:37.000000 systemPY-0.0.9/systemPY.egg-info/SOURCES.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)        1 2022-12-07 16:51:37.000000 systemPY-0.0.9/systemPY.egg-info/dependency_links.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)       16 2022-12-07 16:51:37.000000 systemPY-0.0.9/systemPY.egg-info/requires.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)        9 2022-12-07 16:51:37.000000 systemPY-0.0.9/systemPY.egg-info/top_level.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)        1 2022-11-06 14:36:29.000000 systemPY-0.0.9/systemPY.egg-info/zip-safe
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.687932 systemPY-0.0.9/systempy/
+-rw-r--r--   0 kai       (1000) kai       (1000)      362 2022-12-02 12:46:41.000000 systemPY-0.0.9/systempy/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1251 2022-11-27 21:46:48.000000 systemPY-0.0.9/systempy/daemon.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.691932 systemPY-0.0.9/systempy/ext/
+-rw-r--r--   0 kai       (1000) kai       (1000)        0 2022-08-08 18:09:34.000000 systemPY-0.0.9/systempy/ext/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      608 2022-11-27 21:46:48.000000 systemPY-0.0.9/systempy/ext/celery.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1017 2022-12-02 01:10:30.000000 systemPY-0.0.9/systempy/ext/pretty_repl.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1463 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/ext/ptrepl.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      496 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/ext/starlette.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      517 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/ext/target_ext.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      631 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/loop.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     6119 2022-12-07 16:20:00.000000 systemPY-0.0.9/systempy/mypy.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      263 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/process.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.691932 systemPY-0.0.9/systempy/repl/
+-rw-r--r--   0 kai       (1000) kai       (1000)       52 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/repl/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1627 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/repl/handle_interrupt.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1140 2022-12-02 01:09:48.000000 systemPY-0.0.9/systempy/repl/mixins.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     3987 2022-12-02 01:09:39.000000 systemPY-0.0.9/systempy/repl/repl.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      102 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/repl/typing.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      649 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/repl/util.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     2394 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/target.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      213 2022-11-27 21:46:49.000000 systemPY-0.0.9/systempy/unit.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1002 2022-12-02 17:32:12.000000 systemPY-0.0.9/systempy/unit_meta.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2022-12-07 16:51:37.699932 systemPY-0.0.9/systempy/util/
+-rw-r--r--   0 kai       (1000) kai       (1000)      292 2022-10-27 18:16:32.000000 systemPY-0.0.9/systempy/util/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1827 2022-12-02 01:14:30.000000 systemPY-0.0.9/systempy/util/callback_plan.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1456 2022-12-02 01:14:34.000000 systemPY-0.0.9/systempy/util/check.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1741 2022-12-02 01:14:40.000000 systemPY-0.0.9/systempy/util/configuration.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      684 2022-12-02 01:14:44.000000 systemPY-0.0.9/systempy/util/constants.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      696 2022-12-02 01:14:49.000000 systemPY-0.0.9/systempy/util/creation.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     2198 2022-12-02 01:13:42.000000 systemPY-0.0.9/systempy/util/extraction.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     2156 2022-12-02 01:14:38.000000 systemPY-0.0.9/systempy/util/handler_type.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      802 2022-12-02 01:14:59.000000 systemPY-0.0.9/systempy/util/local_dataclasses.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1469 2022-12-02 01:14:22.000000 systemPY-0.0.9/systempy/util/local_typing.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     3738 2022-12-02 01:13:17.000000 systemPY-0.0.9/systempy/util/misc.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     3082 2022-12-02 01:15:46.000000 systemPY-0.0.9/systempy/util/register.py
```

### Comparing `systemPY-0.0.8/PKG-INFO` & `systemPY-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemPY
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python application component initialization system
 Home-page: https://github.com/kai3341/systemPY
 License: MIT
 Description: # systemPY
         
         ![Logo](https://raw.githubusercontent.com/kai3341/systemPY/main/docs/images/systempy-logo.png)
```

### Comparing `systemPY-0.0.8/README.md` & `systemPY-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/setup.py` & `systemPY-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systemPY.egg-info/PKG-INFO` & `systemPY-0.0.9/systemPY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemPY
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python application component initialization system
 Home-page: https://github.com/kai3341/systemPY
 License: MIT
 Description: # systemPY
         
         ![Logo](https://raw.githubusercontent.com/kai3341/systemPY/main/docs/images/systempy-logo.png)
```

### Comparing `systemPY-0.0.8/systemPY.egg-info/SOURCES.txt` & `systemPY-0.0.9/systemPY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/daemon.py` & `systemPY-0.0.9/systempy/daemon.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/ext/celery.py` & `systemPY-0.0.9/systempy/ext/celery.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/ext/pretty_repl.py` & `systemPY-0.0.9/systempy/ext/pretty_repl.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/ext/ptrepl.py` & `systemPY-0.0.9/systempy/ext/ptrepl.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/ext/target_ext.py` & `systemPY-0.0.9/systempy/ext/target_ext.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/loop.py` & `systemPY-0.0.9/systempy/loop.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/mypy.py` & `systemPY-0.0.9/systempy/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,30 +64,30 @@
     CallableType,
     # Instance,
     NoneType,
     # Overloaded,
     Type,
     TypeOfAny,
     TypeType,
-    # TypeVarType,
+    TypeVarType,
     # UnionType,
     # get_proper_type,
 )
 
 from mypy.typevars import fill_typevars
 from mypy.util import get_unique_redefinition_name
 from mypy.version import __version__ as mypy_version
 
-try:
-    from mypy.types import TypeVarDef  # type: ignore[attr-defined]
-except ImportError:  # pragma: no cover
-    # Backward-compatible with TypeVarDef from Mypy 0.910.
-    from mypy.types import TypeVarType as TypeVarDef
+# try:
+#     from mypy.types import TypeVarDef  # type: ignore[attr-defined]
+# except ImportError:  # pragma: no cover
+#     # Backward-compatible with TypeVarDef from Mypy 0.910.
+#     from mypy.types import TypeVarType as TypeVarDef
 
-UNITMETA_FULLNAME = "systempy.unit.UnitMeta"
+UNITMETA_FULLNAME = "systempy.unit_meta.UnitMeta"
 
 
 def parse_mypy_version(version: str) -> Tuple[int, ...]:
     return tuple(int(part) for part in version.split("+", 1)[0].split("."))
 
 
 MYPY_VERSION_TUPLE = parse_mypy_version(mypy_version)
@@ -120,14 +120,16 @@
 
         if not declared_metaclass:
             return None
 
         if declared_metaclass.type.fullname != UNITMETA_FULLNAME:
             return None
 
+        print(declared_metaclass)
+
         return self._on_base_class_hook
 
     def _on_base_class_hook(self, ctx: ClassDefContext) -> None:
         init_arguments = [
             Argument(Var("kwargs"), AnyType(TypeOfAny.explicit), None, ARG_STAR2)
         ]
         add_method(ctx, "__init__", init_arguments, NoneType())
@@ -139,15 +141,15 @@
 
 def add_method(
     ctx: ClassDefContext,
     name: str,
     args: List[Argument],
     return_type: Type,
     self_type: Optional[Type] = None,
-    tvar_def: Optional[TypeVarDef] = None,
+    tvar_def: Optional[TypeVarType] = None,
     is_classmethod: bool = False,
     is_new: bool = False,
     # is_staticmethod: bool = False,
 ) -> None:
     """
     Adds a new method to a class.
```

### Comparing `systemPY-0.0.8/systempy/repl/handle_interrupt.py` & `systemPY-0.0.9/systempy/repl/handle_interrupt.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/repl/mixins.py` & `systemPY-0.0.9/systempy/repl/mixins.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/repl/repl.py` & `systemPY-0.0.9/systempy/repl/repl.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/repl/util.py` & `systemPY-0.0.9/systempy/repl/util.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/target.py` & `systemPY-0.0.9/systempy/target.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/unit_meta.py` & `systemPY-0.0.9/systempy/unit_meta.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/callback_plan.py` & `systemPY-0.0.9/systempy/util/callback_plan.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/check.py` & `systemPY-0.0.9/systempy/util/check.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/configuration.py` & `systemPY-0.0.9/systempy/util/configuration.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/constants.py` & `systemPY-0.0.9/systempy/util/constants.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/creation.py` & `systemPY-0.0.9/systempy/util/creation.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/extraction.py` & `systemPY-0.0.9/systempy/util/extraction.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/handler_type.py` & `systemPY-0.0.9/systempy/util/handler_type.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/local_dataclasses.py` & `systemPY-0.0.9/systempy/util/local_dataclasses.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/local_typing.py` & `systemPY-0.0.9/systempy/util/local_typing.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/misc.py` & `systemPY-0.0.9/systempy/util/misc.py`

 * *Files identical despite different names*

### Comparing `systemPY-0.0.8/systempy/util/register.py` & `systemPY-0.0.9/systempy/util/register.py`

 * *Files identical despite different names*

