# Comparing `tmp/rsome-1.2.0.tar.gz` & `tmp/rsome-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsome-1.2.0.tar", last modified: Sat Jun 17 16:43:27 2023, max compression
+gzip compressed data, was "rsome-1.2.1.tar", last modified: Tue Jun 27 06:47:15 2023, max compression
```

## Comparing `rsome-1.2.0.tar` & `rsome-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.169816 rsome-1.2.0/
--rw-r--r--   0 pengxiong   (501) staff       (20)    35129 2022-11-30 14:30:50.000000 rsome-1.2.0/LICENSE.md
--rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-17 16:43:27.169880 rsome-1.2.0/PKG-INFO
--rw-r--r--   0 pengxiong   (501) staff       (20)     6040 2023-06-16 07:09:38.000000 rsome-1.2.0/README.md
--rw-r--r--   0 pengxiong   (501) staff       (20)      473 2023-06-17 15:52:57.000000 rsome-1.2.0/pyproject.toml
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.168999 rsome-1.2.0/rsome/
--rw-r--r--   0 pengxiong   (501) staff       (20)      257 2023-06-07 02:43:40.000000 rsome-1.2.0/rsome/__init__.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3386 2023-06-17 09:22:45.000000 rsome-1.2.0/rsome/clp_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     4305 2023-06-17 09:24:10.000000 rsome-1.2.0/rsome/cpt_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2097 2023-06-09 02:04:06.000000 rsome-1.2.0/rsome/cpt_solver_bkp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3429 2023-06-17 09:25:07.000000 rsome-1.2.0/rsome/cpx_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    23484 2023-06-17 10:02:53.000000 rsome-1.2.0/rsome/deco.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    36908 2023-06-17 09:33:47.000000 rsome-1.2.0/rsome/dro.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3834 2023-06-17 09:34:22.000000 rsome-1.2.0/rsome/eco_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    22329 2023-06-17 10:04:18.000000 rsome-1.2.0/rsome/gcp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2972 2023-06-17 09:40:05.000000 rsome-1.2.0/rsome/grb_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)   151192 2023-06-17 10:06:04.000000 rsome-1.2.0/rsome/lp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)       33 2022-11-30 14:30:50.000000 rsome-1.2.0/rsome/lpg_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    10059 2023-06-17 10:08:04.000000 rsome-1.2.0/rsome/math.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     5379 2023-06-17 12:34:04.000000 rsome-1.2.0/rsome/msk_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2459 2023-06-09 02:08:38.000000 rsome-1.2.0/rsome/ort_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)        0 2022-11-30 14:30:50.000000 rsome-1.2.0/rsome/py.typed
--rw-r--r--   0 pengxiong   (501) staff       (20)    15521 2023-06-17 12:35:57.000000 rsome-1.2.0/rsome/ro.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    12862 2023-06-01 07:57:25.000000 rsome-1.2.0/rsome/socp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     7571 2023-06-17 10:12:56.000000 rsome-1.2.0/rsome/subroutines.py
--rw-r--r--   0 pengxiong   (501) staff       (20)      990 2023-06-17 10:13:09.000000 rsome-1.2.0/rsome/this.py
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.169703 rsome-1.2.0/rsome.egg-info/
--rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/PKG-INFO
--rw-r--r--   0 pengxiong   (501) staff       (20)      570 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/SOURCES.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/dependency_links.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/not-zip-safe
--rw-r--r--   0 pengxiong   (501) staff       (20)      115 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/requires.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        6 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/top_level.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)      823 2023-06-17 16:43:27.170163 rsome-1.2.0/setup.cfg
--rw-r--r--   0 pengxiong   (501) staff       (20)      180 2022-11-30 14:30:50.000000 rsome-1.2.0/setup.py
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-27 06:47:15.474569 rsome-1.2.1/
+-rw-r--r--   0 pengxiong   (501) staff       (20)    35129 2022-11-30 14:30:50.000000 rsome-1.2.1/LICENSE.md
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-27 06:47:15.474629 rsome-1.2.1/PKG-INFO
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6040 2023-06-27 06:35:17.000000 rsome-1.2.1/README.md
+-rw-r--r--   0 pengxiong   (501) staff       (20)      473 2023-06-17 15:52:57.000000 rsome-1.2.1/pyproject.toml
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-27 06:47:15.473727 rsome-1.2.1/rsome/
+-rw-r--r--   0 pengxiong   (501) staff       (20)      257 2023-06-07 02:43:40.000000 rsome-1.2.1/rsome/__init__.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3397 2023-06-22 08:25:27.000000 rsome-1.2.1/rsome/clp_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     4316 2023-06-26 03:27:24.000000 rsome-1.2.1/rsome/cpt_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     2097 2023-06-09 02:04:06.000000 rsome-1.2.1/rsome/cpt_solver_bkp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3464 2023-06-22 08:25:15.000000 rsome-1.2.1/rsome/cpx_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    23484 2023-06-17 10:02:53.000000 rsome-1.2.1/rsome/deco.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    37290 2023-06-27 06:23:18.000000 rsome-1.2.1/rsome/dro.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3845 2023-06-22 08:25:53.000000 rsome-1.2.1/rsome/eco_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    22329 2023-06-17 10:04:18.000000 rsome-1.2.1/rsome/gcp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3003 2023-06-22 08:24:39.000000 rsome-1.2.1/rsome/grb_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)   152565 2023-06-27 06:34:33.000000 rsome-1.2.1/rsome/lp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)       33 2022-11-30 14:30:50.000000 rsome-1.2.1/rsome/lpg_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    10059 2023-06-26 03:12:32.000000 rsome-1.2.1/rsome/math.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     5458 2023-06-22 08:23:38.000000 rsome-1.2.1/rsome/msk_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     2470 2023-06-22 08:26:07.000000 rsome-1.2.1/rsome/ort_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)        0 2022-11-30 14:30:50.000000 rsome-1.2.1/rsome/py.typed
+-rw-r--r--   0 pengxiong   (501) staff       (20)    15934 2023-06-27 06:27:27.000000 rsome-1.2.1/rsome/ro.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    12862 2023-06-01 07:57:25.000000 rsome-1.2.1/rsome/socp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     7571 2023-06-17 10:12:56.000000 rsome-1.2.1/rsome/subroutines.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)      990 2023-06-17 10:13:09.000000 rsome-1.2.1/rsome/this.py
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-27 06:47:15.474469 rsome-1.2.1/rsome.egg-info/
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/PKG-INFO
+-rw-r--r--   0 pengxiong   (501) staff       (20)      570 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/SOURCES.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/dependency_links.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/not-zip-safe
+-rw-r--r--   0 pengxiong   (501) staff       (20)      115 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/requires.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        6 2023-06-27 06:47:15.000000 rsome-1.2.1/rsome.egg-info/top_level.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)      823 2023-06-27 06:47:15.474911 rsome-1.2.1/setup.cfg
+-rw-r--r--   0 pengxiong   (501) staff       (20)      180 2022-11-30 14:30:50.000000 rsome-1.2.1/setup.py
```

### Comparing `rsome-1.2.0/LICENSE.md` & `rsome-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/PKG-INFO` & `rsome-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsome
-Version: 1.2.0
+Version: 1.2.1
 Summary: Robust Stochastic Optimization Made Easy
 Author: Peng Xiong
 License: GPL-3.0
 Platform: linux
 Platform: osx
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
@@ -27,15 +27,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.1](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
```

### Comparing `rsome-1.2.0/README.md` & `rsome-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.1](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
```

### Comparing `rsome-1.2.0/rsome/clp_solver.py` & `rsome-1.2.1/rsome/clp_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import warnings
 import time
 from .lp import Solution
 
 
-def solve(formula, display=True, params={}):
+def solve(formula, display=True, log=False, params={}):
 
     try:
         if formula.qmat:
             warnings.warn('the LP solver ignores SOC constraints.')
     except AttributeError:
         pass
```

### Comparing `rsome-1.2.0/rsome/cpt_solver.py` & `rsome-1.2.1/rsome/cpt_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 from scipy.sparse import csr_matrix
 from .socp import SOCProg
 from .gcp import GCProg
 from .lp import Solution
 
 
-def solve(form, display=True, params={}):
+def solve(form, display=True, log=False, params={}):
 
     if isinstance(form, (SOCProg, GCProg)):
         qmat = form.qmat
     else:
         qmat = []
     if isinstance(form, GCProg):
         xmat = form.xmat
```

### Comparing `rsome-1.2.0/rsome/cpt_solver_bkp.py` & `rsome-1.2.1/rsome/cpt_solver_bkp.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/cpx_solver.py` & `rsome-1.2.1/rsome/cpx_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import warnings
 import time
 from .lp import Solution
 from .socp import SOCProg
 
 
-def solve(formula, display=True, params={}):
+def solve(formula, display=True, log=False, params={}):
 
     try:
         if formula.xmat:
             warnings.warn('The SOCP solver ignores exponential cone constraints. ')
         if formula.lmi:
             warnings.warn('The SOCP solver ignores semidefinite cone constraints. ')
     except AttributeError:
@@ -50,16 +50,17 @@
             q = cplex.SparseTriple(ind1=cone, ind2=cone, val=cone_data)
             cpx.quadratic_constraints.add(quad_expr=q)
 
     if display:
         print('Being solved by CPLEX...', flush=True)
         time.sleep(0.2)
 
-    cpx.set_results_stream(None)
-    cpx.set_warning_stream(None)
+    if not log:
+        cpx.set_results_stream(None)
+        cpx.set_warning_stream(None)
     try:
         for param, value in params.items():
             text = 'cpx.parameters.' + param + '.set({0})'.format(value)
             eval(text)
     except (TypeError, ValueError, AttributeError):
         raise ValueError('Incorrect parameters or values.')
```

### Comparing `rsome-1.2.0/rsome/deco.py` & `rsome-1.2.1/rsome/deco.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/dro.py` & `rsome-1.2.1/rsome/dro.py`

 * *Files 2% similar despite different names*

```diff
@@ -763,35 +763,40 @@
                     elif isinstance(inequality, LinConstr):
                         ro_constr.append(inequality)
                     else:
                         raise TypeError('Incorrect data type.')
 
         return ro_constr
 
-    def solve(self, solver=None, display=True, params={}):
+    def solve(self, solver=None, display=True, log=False, params={}):
         """
         Solve the model with the selected solver interface.
 
         Parameters
         ----------
             solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
                       cpx_solver, grb_solver, msk_solver, cpt_solver}
                 Solver interface used for model solution. Use default solver
                 if solver=None.
             display : bool
-                Display option of the solver interface.
+                True for displaying the solution information. False for hiding
+                the solution information.
+            log : bool
+                True for printing the log information. False for hiding the log
+                information. So far the argument only applies to Gurobi, CPLEX,
+                and Mosek.
             params : dict
                 A dictionary that specifies parameters of the selected solver.
                 So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         if solver is None:
-            solution = def_sol(self.do_math(), display, params)
+            solution = def_sol(self.do_math(), display, log, params)
         else:
-            solution = solver.solve(self.do_math(), display, params)
+            solution = solver.solve(self.do_math(), display, log, params)
 
         if isinstance(solution, Solution):
             self.ro_model.solution = solution
         else:
             self.ro_model.solution = None
 
         self.ro_model.rc_model.solution = solution
@@ -816,15 +821,18 @@
             msg += f'{solution.solver} solution status: {solution.status}'
             raise RuntimeError(msg)
 
         return self.sign * self.solution.objval
 
     def optimal(self):
 
-        return self.solution is not None
+        if self.solution is None:
+            return False
+        else:
+            return not np.isnan(self.solution.objval)
 
 
 class Ambiguity:
     """
     The Ambiguity class creates an ambiguity set object
     """
```

### Comparing `rsome-1.2.0/rsome/eco_solver.py` & `rsome-1.2.1/rsome/eco_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 import scipy.sparse as sp
 from .socp import SOCProg
 from .gcp import GCProg
 from .lp import Solution
 
 
-def solve(formula, display=True, params={}):
+def solve(formula, display=True, log=False, params={}):
 
     try:
         if formula.lmi:
             warnings.warn('The solver ignores semidefinite cone constraints. ')
     except AttributeError:
         pass
```

### Comparing `rsome-1.2.0/rsome/gcp.py` & `rsome-1.2.1/rsome/gcp.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/grb_solver.py` & `rsome-1.2.1/rsome/grb_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import warnings
 import time
 from .socp import SOCProg
 from .lp import Solution
 
 
-def solve(formula, display=True, params={}):
+def solve(formula, display=True, log=False, params={}):
 
     try:
         if formula.xmat:
             warnings.warn('The SOCP solver ignores exponential cone constraints. ')
         if formula.lmi:
             warnings.warn('The SOCP solver ignores semidefinite cone constraints. ')
     except AttributeError:
@@ -47,15 +47,16 @@
             index_left = constr[1:]
             A = np.eye(len(index_left))
             grb.addConstr(x[index_left] @ A @ x[index_left] <=
                           x[index_right] @ x[index_right])
 
     grb.setObjective(formula.obj @ x)
 
-    grb.setParam('LogToConsole', 0)
+    if not log:
+        grb.setParam('LogToConsole', 0)
     try:
         for param, value in params.items():
             if eval('grb.Params.{}'.format(param)) is None:
                 raise ValueError('Unknown parameter')
             grb.setParam(param, value)
 
     except (TypeError, ValueError):
```

### Comparing `rsome-1.2.0/rsome/lp.py` & `rsome-1.2.1/rsome/lp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from numbers import Real
 from scipy.sparse import csr_matrix, coo_matrix, lil_matrix
 from scipy.linalg import sqrtm, eigh
 from collections.abc import Iterable, Sized
 # from typing import List
 
 
-def def_sol(formula, display=True, params={}):
+def def_sol(formula, display=True, log=False, params={}):
     """
     This is the default solver of RSOME.
     """
 
     try:
         if formula.qmat:
             warnings.warn('the LP solver ignores SOC constraints.')
@@ -72,20 +72,21 @@
             pi[indices_eq] = res['eqlin']['marginals']
             pi[indices_ineq] = res['ineqlin']['marginals']
             y = {'pi': pi, 'upi': upi, 'lpi': lpi}
 
             return Solution('SciPy', objval, res.x, res.status, stime, y=y)
         else:
             status = res.status
-            msg = 'The optimal solution can not be found, '
+            msg = 'Fail to find the optimal solution, '
             reasons = ('iteration limit is reached.' if status == 1 else
                        'the problem appears to be infeasible.' if status == 2 else
                        'the problem appears to be unbounded.' if status == 3 else
                        'numerical difficulties encountered.')
             msg += 'because {}'.format(reasons)
+            warnings.warn(msg)
             return Solution('Scipy', np.nan, None, status, stime)
     else:
         b_u = formula.const
         b_l = np.ones(A.shape[0]) * (-np.inf)
         bool_eq = (sense == 1)
         b_l[bool_eq] = b_u[bool_eq]
 
@@ -123,16 +124,16 @@
             print('Running time: {0:0.4f}s'.format(stime))
 
         if res.status == 0:
             objval = formula.obj @ res.x
             return Solution('SciPy', objval, res.x, res.status, stime)
         else:
             status = res.status
-            # msg = 'Fail to find the optimal solution.'
-            # warnings.warn(msg)
+            msg = 'Fail to find the optimal solution.'
+            warnings.warn(msg)
             return Solution('Scipy', np.nan, None, status, stime)
 
 
 def concat(iters, axis=0):
     """
     Join a sequence of arrays of affine expressions along an existing axis.
 
@@ -156,32 +157,49 @@
     const_each = []
     idx_each = []
     count = 0
     model = None
     event_adapt = None
     fixed = True
     ctype = None
+
     for item in iters:
+        if isinstance(item, (Real, np.ndarray)):
+            continue
+        if not isinstance(item, (Affine, Vars, VarSub)):
+            raise TypeError('Unsupported data type for concatenation')
+        if model is None:
+            model = item.model
+            num_var = model.last
+        else:
+            if model != item.model:
+                raise ValueError('Model mismatch.')
+
+    if model is None:
+        return np.concatenate(iters, axis)
+
+    for item in iters:
+        if isinstance(item, (Real, np.ndarray)):
+            item_value = np.array(item)
+            item_size = item_value.size
+            item_linear = csr_matrix(([], ([], [])), shape=(item_size, num_var))
+            item = Affine(model, item_linear, item_value)
+            if model.mtype == 'V':
+                item = DecAffine(model, item, [list(range(item.model.top.num_scen))])
         if not isinstance(item, Affine):
             item = item.to_affine()
         if isinstance(item, DecAffine):
             if event_adapt is None:
                 event_adapt = [list(range(item.model.top.num_scen))]
             if ctype is None:
                 ctype = item.ctype
             if ctype != item.ctype:
                 raise ValueError('Cannot concatenate different types of expressions.')
             event_adapt = comb_set(event_adapt, item.event_adapt)
             fixed = fixed and item.fixed
-        if model is None:
-            model = item.model
-            num_var = model.last
-        else:
-            if model != item.model:
-                raise ValueError('Model mismatch.')
 
         if item.linear.shape[1] < num_var:
             item.linear.resize(item.linear.shape[0], num_var)
         linear_each.append(item.linear)
         const_each.append(item.const)
         idx_each.append(np.arange(count, count+item.size).reshape(item.shape))
 
@@ -226,15 +244,15 @@
         package in 1) the arrays to be stacked together are presented as separate
         arguments, instead of elements in an array-like sequence; and 2) a list of
         arrays can be stacked horizontally first before being vertically stacked.
     """
 
     rows = []
     for arg in args:
-        if isinstance(arg, Iterable):
+        if isinstance(arg, Iterable) and not isinstance(arg, np.ndarray):
             rows.append(concat(arg, axis=1))
         else:
             rows.append(arg)
 
     return concat(rows, axis=0)
 
 
@@ -260,15 +278,15 @@
         package in 1) the arrays to be stacked together are presented as separate
         arguments, instead of elements in an array-like sequence; and 2) a list of
         arrays can be stacked vertically first before being horizontally stacked.
     """
 
     cols = []
     for arg in args:
-        if isinstance(arg, Iterable):
+        if isinstance(arg, Iterable) and not isinstance(arg, np.ndarray):
             cols.append(concat(arg, axis=0))
         else:
             cols.append(arg)
 
     return concat(cols, axis=1)
 
 
@@ -623,35 +641,40 @@
             formula = LinProg(dual_linear, dual_const, dual_sense,
                               np.array(['C']*ndv), dual_ub, dual_lb, dual_obj)
             self.dual = formula
             self.dupdate = False
 
             return formula
 
-    def solve(self, solver=None, display=True, params={}):
+    def solve(self, solver=None, display=True, log=False, params={}):
         """
         Solve the model with the selected solver interface.
 
         Parameters
         ----------
             solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
                       cpx_solver, grb_solver, msk_solver, cpt_solver}
                 Solver interface used for model solution. Use default solver
                 if solver=None.
             display : bool
-                Display option of the solver interface.
+                True for displaying the solution information. False for hiding
+                the solution information.
+            log : bool
+                True for printing the log information. False for hiding the log
+                information. So far the argument only applies to Gurobi, CPLEX,
+                and Mosek.
             params : dict
                 A dictionary that specifies parameters of the selected solver.
                 So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         if solver is None:
-            solution = def_sol(self.do_math(obj=True), display, params)
+            solution = def_sol(self.do_math(obj=True), display, log, params)
         else:
-            solution = solver.solve(self.do_math(obj=True), display, params)
+            solution = solver.solve(self.do_math(obj=True), display, log, params)
 
         if isinstance(solution, Solution):
             self.solution = solution
         else:
             self.solution = None
 
     def get(self):
@@ -673,15 +696,18 @@
             msg += f'{solution.solver} solution status: {solution.status}.'
             raise RuntimeError(msg)
 
         return self.sign * self.solution.objval
 
     def optimal(self):
 
-        return self.solution is not None
+        if self.solution is None:
+            return False
+        else:
+            return not np.isnan(self.solution.objval)
 
 
 class SparseVec:
 
     __array_priority__ = 200
 
     def __init__(self, index, value, nvar):
@@ -2207,14 +2233,22 @@
         if right.sign == -1:
             raise ValueError('Nonconvex constraints.')
 
         pieces = [piece <= 0 for piece in right.pieces]
 
         return PWConstr(right.model, pieces)
 
+    def __getitem__(self, item):
+
+        return self.pieces[item]
+
+    def __len__(self):
+
+        return len(self.pieces)
+
     @property
     def E(self):
 
         return ExpPiecewiseConvex(self.model, self.pieces, self.sign, self.add_sign)
 
 
 class PerspConvex(Convex):
@@ -4136,14 +4170,20 @@
         else:
             event = ' event-wise ' if len(self.event_adapt) > 1 else ' '
             ctype = ''
         expr = 'linear' if self.fixed else 'robust'
 
         return '{}{}{} constraint{}{}'.format(size, event, expr, suffix, ctype)
 
+    def forall(self, ambset):
+
+        self.ambset = ambset
+
+        return self
+
 
 class DecBounds(Bounds):
 
     def __init__(self, bounds, event_adapt=None):
 
         super().__init__(bounds.model, bounds.indices, bounds.values,
                          bounds.btype)
```

### Comparing `rsome-1.2.0/rsome/math.py` & `rsome-1.2.1/rsome/math.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/msk_solver.py` & `rsome-1.2.1/rsome/msk_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 """
 
 from mosek.fusion import *
 import numpy as np
 from scipy.sparse import coo_matrix
 from .socp import SOCProg
 from .gcp import GCProg
+from .lp import Solution
 import warnings
 import time
-from .lp import Solution
+import sys
 
 
-def solve(form, display=True, params={}):
+def solve(form, display=True, log=False, params={}):
 
     if isinstance(form, (SOCProg, GCProg)):
         qmat = form.qmat
     else:
         qmat = []
     if isinstance(form, GCProg):
         xmat = form.xmat
@@ -87,14 +88,17 @@
 
             left = Expr.reshape(Expr.sub(Expr.mul(psd_linear, x), psd_const), dim, dim)
             M.constraint(left, Domain.inPSDCone(dim))
 
         for param, value in params.items():
             M.setSolverParam(param, value)
 
+        if log:
+            M.setLogHandler(sys.stdout)
+
         if display:
             print('Being solved by Mosek...', flush=True)
             time.sleep(0.2)
         t0 = time.time()
         M.solve()
         stime = time.time() - t0
         stats_string = M.getPrimalSolutionStatus().__str__()
```

### Comparing `rsome-1.2.0/rsome/ort_solver.py` & `rsome-1.2.1/rsome/ort_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import warnings
 import time
 from .lp import Solution
 from numbers import Real
 
 
-def solve(formula, display=True, params={}):
+def solve(formula, display=True, log=False, params={}):
 
     try:
         if formula.qmat:
             warnings.warn('the LP solver ignores SOC constriants.')
     except AttributeError:
         pass
```

### Comparing `rsome-1.2.0/rsome/ro.py` & `rsome-1.2.1/rsome/ro.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             more_roc = []
             pw_constr = self.rc_model.vars[0] >= self.sign * self.obj
             more_roc = pw_constr.pieces
         else:
             raise TypeError('Incorrect type for the objective function.')
 
         for constr in self.all_constr + more_roc:
-            if isinstance(constr, (LinConstr, Bounds, CvxConstr,
+            if isinstance(constr, (LinConstr, Bounds, CvxConstr, ConeConstr,
                                    ExpConstr, KLConstr, LMIConstr)):
                 self.rc_model.st(constr)
             if isinstance(constr, RoConstr):
                 if constr.support:
                     rc_constrs = constr.le_to_rc()
                 else:
                     rc_constrs = constr.le_to_rc(self.obj_support)
@@ -391,44 +391,50 @@
             self.pupdate = False
         else:
             self.dual = formula
             self.dupdate = False
 
         return formula
 
-    def solve(self, solver=None, display=True, params={}):
+    def solve(self, solver=None, display=True, log=False, params={}):
         """
         Solve the model with the selected solver interface.
 
         Parameters
         ----------
         solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
                   cpx_solver, grb_solver, msk_solver, cpt_solver}
             Solver interface used for model solution. Use the default
             solver if solver=None.
         display : bool
-            Display option of the solver interface.
+            True for displaying the solution information. False for hiding
+            the solution information.
+        log : bool
+            True for printing the log information. False for hiding the log
+            information. So far the argument only applies to Gurobi, CPLEX,
+            and Mosek.
         params : dict
             A dictionary that specifies parameters of the selected solver.
             So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         if solver is None:
-            solution = def_sol(self.do_math(), display, params)
+            solution = def_sol(self.do_math(), display, log, params)
         else:
-            solution = solver.solve(self.do_math(), display, params)
+            solution = solver.solve(self.do_math(), display, log, params)
 
         if isinstance(solution, Solution):
             self.rc_model.solution = solution
         else:
             self.rc_model.solution = None
 
         self.solution = self.rc_model.solution
 
-    def soc_solve(self, solver=None, degree=4, cuts=(-30, 60), display=True, params={}):
+    def soc_solve(self, solver=None, degree=4, cuts=(-30, 60),
+                  display=True, log=False, params={}):
         """
         Solve the approximated SOC model with the selected solver interface.
 
         Parameters
         ----------
             solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
                       cpx_solver, grb_solver, msk_solver}
@@ -445,17 +451,17 @@
             params : dict
                 A dictionary that specifies parameters of the selected solver.
                 So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         formula = self.do_math().to_socp(degree, cuts)
         if solver is None:
-            solution = def_sol(formula, display, params)
+            solution = def_sol(formula, display, log, params)
         else:
-            solution = solver.solve(formula, display, params)
+            solution = solver.solve(formula, display, log, params)
 
         if isinstance(solution, Solution):
             self.rc_model.solution = solution
         else:
             self.rc_model.solution = None
 
         self.solution = self.rc_model.solution
@@ -479,8 +485,11 @@
             msg += f'{solution.solver} solution status: {solution.status}'
             raise RuntimeError(msg)
 
         return self.sign * self.rc_model.solution.objval
 
     def optimal(self):
 
-        return self.solution is not None
+        if self.solution is None:
+            return False
+        else:
+            return not np.isnan(self.solution.objval)
```

### Comparing `rsome-1.2.0/rsome/socp.py` & `rsome-1.2.1/rsome/socp.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/subroutines.py` & `rsome-1.2.1/rsome/subroutines.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome/this.py` & `rsome-1.2.1/rsome/this.py`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/rsome.egg-info/PKG-INFO` & `rsome-1.2.1/rsome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsome
-Version: 1.2.0
+Version: 1.2.1
 Summary: Robust Stochastic Optimization Made Easy
 Author: Peng Xiong
 License: GPL-3.0
 Platform: linux
 Platform: osx
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
@@ -27,15 +27,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.1](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
```

### Comparing `rsome-1.2.0/rsome.egg-info/SOURCES.txt` & `rsome-1.2.1/rsome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rsome-1.2.0/setup.cfg` & `rsome-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rsome
-version = 1.2.0
+version = 1.2.1
 description = Robust Stochastic Optimization Made Easy
 long_description = file: README.rst
 author = Peng Xiong
 license = GPL-3.0
 license_file = LICENSE.md
 platforms = linux, osx, win64
 classifiers =
```

