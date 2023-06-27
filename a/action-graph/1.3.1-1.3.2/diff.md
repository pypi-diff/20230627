# Comparing `tmp/action-graph-1.3.1.tar.gz` & `tmp/action-graph-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.3.1.tar", last modified: Sun Jun 25 00:50:09 2023, max compression
+gzip compressed data, was "action-graph-1.3.2.tar", last modified: Tue Jun 27 13:38:55 2023, max compression
```

## Comparing `action-graph-1.3.1.tar` & `action-graph-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.1/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.1/README.md
--rw-r--r--   0        0        0      684 2023-06-25 00:49:06.146086 action-graph-1.3.1/action_graph/__init__.py
--rw-r--r--   0        0        0     3181 2023-06-24 22:19:40.196028 action-graph-1.3.1/action_graph/action.py
--rw-r--r--   0        0        0    10818 2023-06-23 21:27:59.160761 action-graph-1.3.1/action_graph/agent.py
--rw-r--r--   0        0        0     4664 2023-06-25 00:33:36.780557 action-graph-1.3.1/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-25 00:49:10.266264 action-graph-1.3.1/pyproject.toml
--rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.1/tests/01-redundant_precon_test.py
--rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.1/tests/02-multi_feasible_test.py
--rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.1/tests/03-references_test.py
--rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.1/tests/04-loop_test.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.2/README.md
+-rw-r--r--   0        0        0      684 2023-06-27 13:37:46.128375 action-graph-1.3.2/action_graph/__init__.py
+-rw-r--r--   0        0        0     3476 2023-06-25 03:34:21.964154 action-graph-1.3.2/action_graph/action.py
+-rw-r--r--   0        0        0    10818 2023-06-23 21:27:59.160761 action-graph-1.3.2/action_graph/agent.py
+-rw-r--r--   0        0        0     4664 2023-06-25 03:02:12.179040 action-graph-1.3.2/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-27 13:37:54.104349 action-graph-1.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.2/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.2/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.2/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.2/tests/04-loop_test.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.2/PKG-INFO
```

### Comparing `action-graph-1.3.1/LICENSE` & `action-graph-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/README.md` & `action-graph-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/action_graph/__init__.py` & `action-graph-1.3.2/action_graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.3.1/action_graph/action.py` & `action-graph-1.3.2/action_graph/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,19 +75,29 @@
 
     def __hash__(self):
         return hash(self.__class__.__name__)
 
     def __eq__(self, __o: object) -> bool:
         if self.__class__.__name__ == __o.__class__.__name__ and \
                 self.cost == __o.cost and \
-                self.effects == __o.effects and \
+                self.__check_eq__(self.effects, __o.effects) and \
                 self.preconditions == __o.preconditions:
             return True
         return False
 
+    def __check_eq__(self, e1, e2):
+        for k in e1.keys():
+            if k not in e2.keys():
+                return False
+            if e1[k] != e2[k]:
+                if Ellipsis not in [e1[k], e2[k]]:
+                    return False
+            #
+        return True
+
     def __copy__(self):
         # instantiate an object of Action (or its sub-class) type
         a_copy = type(self)(self.agent)
         # shallow copy
         a_copy.cost = self.cost
         a_copy.status = self.status
         a_copy.timeout = self.timeout
```

### Comparing `action-graph-1.3.1/action_graph/agent.py` & `action-graph-1.3.2/action_graph/agent.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/action_graph/planner.py` & `action-graph-1.3.2/action_graph/planner.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/pyproject.toml` & `action-graph-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.3.1"
+version = "1.3.2"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.3.1/tests/01-redundant_precon_test.py` & `action-graph-1.3.2/tests/01-redundant_precon_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/tests/02-multi_feasible_test.py` & `action-graph-1.3.2/tests/02-multi_feasible_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/tests/03-references_test.py` & `action-graph-1.3.2/tests/03-references_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/tests/04-loop_test.py` & `action-graph-1.3.2/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.1/PKG-INFO` & `action-graph-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.3.1
+Version: 1.3.2
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

