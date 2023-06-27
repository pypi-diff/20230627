# Comparing `tmp/grgrjax-0.4.3.tar.gz` & `tmp/grgrjax-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grgrjax-0.4.3.tar", last modified: Sat Apr 15 12:22:28 2023, max compression
+gzip compressed data, was "grgrjax-0.4.4.tar", last modified: Tue Jun 27 09:11:43 2023, max compression
```

## Comparing `grgrjax-0.4.3.tar` & `grgrjax-0.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.383203 grgrjax-0.4.3/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.386536 grgrjax-0.4.3/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1221 2023-03-27 00:33:48.000000 grgrjax-0.4.3/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2023-02-17 15:12:43.000000 grgrjax-0.4.3/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2023-02-16 13:40:07.000000 grgrjax-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-18 14:43:16.000000 grgrjax-0.4.3/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-02-11 15:59:58.000000 grgrjax-0.4.3/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-04-15 12:22:28.393202 grgrjax-0.4.3/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      573 2023-03-04 11:00:53.000000 grgrjax-0.4.3/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.389869 grgrjax-0.4.3/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.383203 grgrjax-0.4.3/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.389869 grgrjax-0.4.3/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1614 2023-02-21 09:50:30.000000 grgrjax-0.4.3/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       97 2023-02-18 21:06:44.000000 grgrjax-0.4.3/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-02-18 15:27:02.000000 grgrjax-0.4.3/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/grgrjax/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      476 2023-03-27 09:28:29.000000 grgrjax-0.4.3/grgrjax/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-04-15 12:22:20.000000 grgrjax-0.4.3/grgrjax/__version__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7782 2023-03-13 19:38:38.000000 grgrjax-0.4.3/grgrjax/helpers.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6323 2023-03-28 17:15:44.000000 grgrjax-0.4.3/grgrjax/newton.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      819 2023-02-17 14:08:34.000000 grgrjax-0.4.3/grgrjax/test_all.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/grgrjax.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      502 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-02-17 14:43:43.000000 grgrjax-0.4.3/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:22:28.393202 grgrjax-0.4.3/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1033 2023-03-27 09:28:05.000000 grgrjax-0.4.3/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.738253 grgrjax-0.4.4/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.731586 grgrjax-0.4.4/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.734920 grgrjax-0.4.4/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1221 2023-03-27 00:33:48.000000 grgrjax-0.4.4/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2023-02-17 15:12:43.000000 grgrjax-0.4.4/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2023-02-16 13:40:07.000000 grgrjax-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-18 14:43:16.000000 grgrjax-0.4.4/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-02-11 15:59:58.000000 grgrjax-0.4.4/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-06-27 09:11:43.738253 grgrjax-0.4.4/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      573 2023-03-04 11:00:53.000000 grgrjax-0.4.4/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.734920 grgrjax-0.4.4/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-02-11 15:59:58.000000 grgrjax-0.4.4/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.731586 grgrjax-0.4.4/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.734920 grgrjax-0.4.4/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-02-11 15:59:58.000000 grgrjax-0.4.4/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1614 2023-02-21 09:50:30.000000 grgrjax-0.4.4/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       97 2023-02-18 21:06:44.000000 grgrjax-0.4.4/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-02-11 15:59:58.000000 grgrjax-0.4.4/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-02-18 15:27:02.000000 grgrjax-0.4.4/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.738253 grgrjax-0.4.4/grgrjax/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      476 2023-03-27 09:28:29.000000 grgrjax-0.4.4/grgrjax/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-06-27 09:11:10.000000 grgrjax-0.4.4/grgrjax/__version__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7782 2023-03-13 19:38:38.000000 grgrjax-0.4.4/grgrjax/helpers.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6464 2023-06-27 09:10:48.000000 grgrjax-0.4.4/grgrjax/newton.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      819 2023-02-17 14:08:34.000000 grgrjax-0.4.4/grgrjax/test_all.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 09:11:43.738253 grgrjax-0.4.4/grgrjax.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-06-27 09:11:43.000000 grgrjax-0.4.4/grgrjax.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      502 2023-06-27 09:11:43.000000 grgrjax-0.4.4/grgrjax.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-06-27 09:11:43.000000 grgrjax-0.4.4/grgrjax.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-06-27 09:11:43.000000 grgrjax-0.4.4/grgrjax.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2023-06-27 09:11:43.000000 grgrjax-0.4.4/grgrjax.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-02-17 14:43:43.000000 grgrjax-0.4.4/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-06-27 09:11:43.738253 grgrjax-0.4.4/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1033 2023-03-27 09:28:05.000000 grgrjax-0.4.4/setup.py
```

### Comparing `grgrjax-0.4.3/.github/workflows/continuous-integration.yml` & `grgrjax-0.4.4/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/.readthedocs.yaml` & `grgrjax-0.4.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/LICENSE` & `grgrjax-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/PKG-INFO` & `grgrjax-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grgrjax
-Version: 0.4.3
+Version: 0.4.4
 Summary: Some generic tools for JAX
 Home-page: https://github.com/gboehl/grgrjax
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grgrjax-0.4.3/README.rst` & `grgrjax-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/docs/Makefile` & `grgrjax-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/docs/conf.py` & `grgrjax-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/docs/make.bat` & `grgrjax-0.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/grgrjax/helpers.py` & `grgrjax-0.4.4/grgrjax/helpers.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/grgrjax/newton.py` & `grgrjax-0.4.4/grgrjax/newton.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 import jax
 import time
 import jax.numpy as jnp
 import scipy.sparse as ssp
 from .helpers import val_and_jacfwd, amax
 
+try:
+    ssp_csr_array = ssp.csr_array
+    ssp_lil_array = ssp.lil_array
+except AttributeError:
+    ssp_csr_array = ssp._arrays.csr_array
+    ssp_lil_array = ssp._arrays.lil_array
+
 
 def _newton_cond_func(carry):
     (xi, eps, cnt), (func, verbose, maxit, tol) = carry
     cond = cnt < maxit
     cond = jnp.logical_and(cond, eps > tol)
     cond = jnp.logical_and(cond, ~jnp.isnan(eps))
     verbose = jnp.logical_and(cnt, verbose)
@@ -144,41 +151,41 @@
             func = val_and_jacfwd(func)
             fout = func(xi)
 
         # unwrap results
         fval, jacval, aux = fout if len(fout) == 3 else (*fout, None)
         # check for convergence or errors
         jac_is_nan = jnp.isnan(jacval.data).any() if isinstance(
-            jacval, ssp._arrays.csr_array) else jnp.isnan(jacval).any()
+            jacval, ssp_csr_array) else jnp.isnan(jacval).any()
         eps = jnp.abs(fval).max()
         if _perform_checks_newton(res, eps, cnt, jac_is_nan, tol, rtol, maxit):
             break
 
         # be informative
         if verbose and cnt:
             ltime = time.time() - st
             info_str = f'    Iteration {cnt:3d} | max. error {eps:.2e} | lapsed {ltime:3.4f}'
             if verbose_jac:
                 jacval = jacval.toarray() if isinstance(
-                    jacval, ssp._arrays.csr_array) else jacval
+                    jacval, ssp_csr_array) else jacval
                 jacdet = jnp.linalg.det(jacval) if (
                     jacval.shape[0] == jacval.shape[1]) else 0
                 info_str += f' | det {jacdet:1.5g} | rank {jnp.linalg.matrix_rank(jacval)}/{jacval.shape[0]}'
             print(info_str)
 
         # assign suitable solver if not given
         if solver is None:
-            if isinstance(jacval, ssp._arrays.csr_array):
+            if isinstance(jacval, ssp_csr_array):
                 solver = ssp.linalg.spsolve
             else:
                 solver = jax.scipy.linalg.solve
         xi -= solver(jacval, fval)
 
     jacval = jacval.toarray() if isinstance(
-        jacval, (ssp._arrays.csr_array, ssp._arrays.lil_array)) else jacval
+        jacval, (ssp_csr_array, ssp_lil_array)) else jacval
 
     res['x'], res['niter'] = xi, cnt
     res['fun'], res['jac'] = fval, jacval
     if aux is not None:
         res['aux'] = aux
 
     if verbose_jac:
```

### Comparing `grgrjax-0.4.3/grgrjax/test_all.py` & `grgrjax-0.4.4/grgrjax/test_all.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.3/grgrjax.egg-info/PKG-INFO` & `grgrjax-0.4.4/grgrjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grgrjax
-Version: 0.4.3
+Version: 0.4.4
 Summary: Some generic tools for JAX
 Home-page: https://github.com/gboehl/grgrjax
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grgrjax-0.4.3/setup.py` & `grgrjax-0.4.4/setup.py`

 * *Files identical despite different names*

