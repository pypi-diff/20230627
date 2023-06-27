# Comparing `tmp/signe-0.1.0.tar.gz` & `tmp/signe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.0.tar", last modified: Thu Jun 22 11:03:02 2023, max compression
+gzip compressed data, was "signe-0.1.1.tar", last modified: Tue Jun 27 15:39:01 2023, max compression
```

## Comparing `signe-0.1.0.tar` & `signe-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 11:03:02.743792 signe-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      469 2023-06-22 11:03:02.742826 signe-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-06-22 10:59:30.000000 signe-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 11:03:02.743792 signe-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1199 2023-06-22 09:28:23.000000 signe-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 11:03:02.718780 signe-0.1.0/signe/
--rw-rw-rw-   0        0        0      160 2023-06-22 09:27:52.000000 signe-0.1.0/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 11:03:02.739800 signe-0.1.0/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-14 07:24:58.000000 signe-0.1.0/signe/core/__init__.py
--rw-rw-rw-   0        0        0      537 2023-06-21 08:17:37.000000 signe-0.1.0/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-21 09:03:23.000000 signe-0.1.0/signe/core/consts.py
--rw-rw-rw-   0        0        0     4591 2023-06-21 15:29:40.000000 signe-0.1.0/signe/core/effect.py
--rw-rw-rw-   0        0        0     2493 2023-06-21 10:56:47.000000 signe-0.1.0/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2737 2023-06-21 09:03:53.000000 signe-0.1.0/signe/core/signal.py
--rw-rw-rw-   0        0        0     1102 2023-06-16 14:04:25.000000 signe-0.1.0/signe/core/transition.py
--rw-rw-rw-   0        0        0       97 2023-06-22 09:19:44.000000 signe-0.1.0/signe/types.py
--rw-rw-rw-   0        0        0     1557 2023-06-22 09:19:57.000000 signe-0.1.0/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 11:03:02.728056 signe-0.1.0/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-06-22 11:03:02.000000 signe-0.1.0/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-22 11:03:02.000000 signe-0.1.0/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 11:03:02.000000 signe-0.1.0/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 11:03:02.000000 signe-0.1.0/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-22 11:03:02.000000 signe-0.1.0/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 15:39:01.806721 signe-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-06-27 15:39:01.805703 signe-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:39:01.807697 signe-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:39:01.782763 signe-0.1.1/signe/
+-rw-rw-rw-   0        0        0      160 2023-06-27 15:38:47.000000 signe-0.1.1/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:39:01.803707 signe-0.1.1/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.1/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-06-25 12:24:57.000000 signe-0.1.1/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.1/signe/core/consts.py
+-rw-rw-rw-   0        0        0     4309 2023-06-26 14:25:04.000000 signe-0.1.1/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.1/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.1/signe/core/signal.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.1/signe/types.py
+-rw-rw-rw-   0        0        0     1571 2023-06-26 14:13:09.000000 signe-0.1.1/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:39:01.792735 signe-0.1.1/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-06-27 15:39:01.000000 signe-0.1.1/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-27 15:39:01.000000 signe-0.1.1/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:39:01.000000 signe-0.1.1/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 15:39:01.000000 signe-0.1.1/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-27 15:39:01.000000 signe-0.1.1/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.0/LICENSE` & `signe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.0/setup.py` & `signe-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 """The setup script."""
 
 from setuptools import setup, find_packages
 import signe
-from pathlib import Path
 
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = []
```

### Comparing `signe-0.1.0/signe/core/collections.py` & `signe-0.1.1/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.0/signe/core/effect.py` & `signe-0.1.1/signe/core/effect.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,38 +27,40 @@
         self._state = EffectState.CURRENT
         self.__dep_signals: Set[Signal] = set()
         self.__dep_effects: Set[Effect] = set()
         self._sub_effects: list[Effect] = []
 
         self._cleanup_callbacks: list[Callable] = []
 
-        self.__init_run_fn()
+        self.__run_fn()
+        self.__init_no_deps = (len(self.__dep_effects) + len(self.__dep_signals)) <= 0
 
     def _add_sub_effect(self, effect: Effect):
         self._sub_effects.append(effect)
 
     def add_dep_signal(self, signal: Signal):
         self.__dep_signals.add(signal)
 
     def add_dep_effect(self, effect: Effect):
         self.__dep_effects.add(effect)
 
     def getValue(self):
-        tick = self.__executor.current_execution_scheduler.tick
-        current_effect = self.__executor.effect_running_stack.get_current()
+        if not self.__init_no_deps:
+            tick = self.__executor.current_execution_scheduler.tick
+            current_effect = self.__executor.effect_running_stack.get_current()
+
+            if current_effect:
+                if self._age == tick:
+                    if self._state == EffectState.RUNNING:
+                        raise Exception("circular running")
 
-        if current_effect:
-            if self._age == tick:
-                if self._state == EffectState.RUNNING:
-                    raise Exception("circular running")
+                    self.update()
 
-                self.update()
-
-            self.__dep_effects.add(current_effect)
-            current_effect.add_dep_effect(self)
+                self.__dep_effects.add(current_effect)
+                current_effect.add_dep_effect(self)
 
         return self.value
 
     def _push_scheduler(self):
         tick = self.__executor.current_execution_scheduler.tick
 
         if self._age >= tick:
@@ -77,27 +79,14 @@
 
     def update(self):
         if self._state != EffectState.STALE:
             return
 
         self.__run_fn()
 
-    def __init_run_fn(self):
-        current_effect = self.__executor.effect_running_stack.get_current()
-
-        if current_effect is not None and current_effect is not self:
-            current_effect._add_sub_effect(self)
-
-        try:
-            self.__executor.effect_running_stack.set_current(self)
-            self.value = self.fn()
-
-        finally:
-            self.__executor.effect_running_stack.reset_current()
-
     def add_cleanup_callback(self, callback: Callable):
         self._cleanup_callbacks.append(callback)
 
     def __run_fn(self):
         self._cleanup_source_before_update()
 
         current_effect = self.__executor.effect_running_stack.get_current()
```

### Comparing `signe-0.1.0/signe/core/runtime.py` & `signe-0.1.1/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.0/signe/core/signal.py` & `signe-0.1.1/signe/core/signal.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.0/signe/utils.py` & `signe-0.1.1/signe/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         def getter():
             effect = Effect(exec, fn)
             self.getter = effect
             return effect.getValue()
 
         self.getter = getter
 
-    def __call__(self, *args: Any, **kwds: Any) -> Any:
-        return self.getter()
+    def __call__(self, *args: Any, **kwds: Any) -> T:
+        return self.getter()  # type: ignore
 
 
 def batch(fn: Callable[[], None]):
     if isinstance(exec.current_execution_scheduler, BatchExecutionScheduler):
         fn()
         return
```

