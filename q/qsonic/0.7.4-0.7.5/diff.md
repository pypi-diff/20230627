# Comparing `tmp/qsonic-0.7.4.tar.gz` & `tmp/qsonic-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.7.4.tar", last modified: Sat Jun 24 15:23:28 2023, max compression
+gzip compressed data, was "qsonic-0.7.5.tar", last modified: Tue Jun 27 15:37:59 2023, max compression
```

## Comparing `qsonic-0.7.4.tar` & `qsonic-0.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-24 15:23:00.000000 qsonic-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-24 15:23:28.047543 qsonic-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-24 15:23:00.000000 qsonic-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.039543 qsonic-0.7.4/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.043543 qsonic-0.7.4/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52575 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 15:23:00.000000 qsonic-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 15:23:00.000000 qsonic-0.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-24 15:23:28.047543 qsonic-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:23:00.000000 qsonic-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.264350 qsonic-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 15:37:44.000000 qsonic-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-27 15:37:59.264350 qsonic-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-27 15:37:44.000000 qsonic-0.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.252350 qsonic-0.7.5/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.256350 qsonic-0.7.5/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53391 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.260350 qsonic-0.7.5/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30770 2023-06-27 15:37:44.000000 qsonic-0.7.5/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.260350 qsonic-0.7.5/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 15:37:59.000000 qsonic-0.7.5/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-27 15:37:44.000000 qsonic-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 15:37:44.000000 qsonic-0.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-27 15:37:59.264350 qsonic-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:37:44.000000 qsonic-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:59.264350 qsonic-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-27 15:37:44.000000 qsonic-0.7.5/tests/test_spectrum.py
```

### Comparing `qsonic-0.7.4/LICENSE` & `qsonic-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/PKG-INFO` & `qsonic-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.4
+Version: 0.7.5
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.7.4/README.rst` & `qsonic-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/calibration.py` & `qsonic-0.7.5/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/catalog.py` & `qsonic-0.7.5/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/io.py` & `qsonic-0.7.5/py/qsonic/io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/masks.py` & `qsonic-0.7.5/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/mathtools.py` & `qsonic-0.7.5/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/mpi_utils.py` & `qsonic-0.7.5/py/qsonic/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/py/qsonic/picca_continuum.py` & `qsonic-0.7.5/py/qsonic/picca_continuum.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,24 +620,24 @@
             self.eta_interp.reset(y[:, 1], ep=ep[:, 1])
 
         if self.mpi_rank != 0:
             return
 
         step = max(1, self.varlss_fitter.nwbins // 10)
         text = ("Variance fitting results:\n"
-                "wave\t| var_lss +-  error \t|   eta   +-  error \n")
+                "wave\t| var_lss +-  error \t|   eta   +-  error")
 
         for i in range(0, self.varlss_fitter.nwbins, step):
             w = self.varlss_fitter.waveobs[i]
             v = self.varlss_interp.fp[i]
             ve = self.varlss_interp.ep[i]
             n = self.eta_interp.fp[i]
             ne = self.eta_interp.ep[i]
             text += \
-                f"{w:7.2f}\t| {v:7.2e} +- {ve:7.2e}\t| {n:7.2e} +- {ne:7.2e}\n"
+                f"\n{w:7.2f}\t| {v:7.2e} +- {ve:7.2e}\t| {n:7.2e} +- {ne:7.2e}"
 
         logging_mpi(text, 0)
 
     def _normalize_flux(self, spectra_list):
         """Multiplies continuum estimates with stacked values in order to
         normalize flux in the observed grid to be 1 if
         ``--normalize-stacked-flux`` is passed.
@@ -1142,14 +1142,53 @@
 
     def _fit_array_shape_assert(self, arr):
         assert (arr.ndim == 1 or arr.ndim == 2)
         assert (arr.shape[0] == self.nwbins)
         if arr.ndim == 2:
             assert (arr.shape[1] == 2)
 
+    def _get_wave_bin_slice_params(self, iwave):
+        i1 = iwave * self.nvarbins
+        i2 = i1 + self.nvarbins
+        wave_slice = np.s_[i1:i2]
+        w = ((self.num_pixels[wave_slice] >= VarLSSFitter.min_num_pix)
+             & (self.num_qso[wave_slice] >= VarLSSFitter.min_num_qso))
+
+        if w.sum() < 5:
+            logging_mpi(
+                "Not enough statistics for VarLSSFitter at "
+                f"{self.waveobs[iwave]:.2f} A. Increasing validity range...",
+                self.mpi_rank, "warning")
+            w = ((self.num_pixels[wave_slice] >= VarLSSFitter.min_num_pix // 2)
+                 & (self.num_qso[wave_slice] >= VarLSSFitter.min_num_qso // 2))
+
+        if w.sum() < 5:
+            logging_mpi(
+                "Still not enough statistics for VarLSSFitter at "
+                f"{self.waveobs[iwave]:.2f} A.",
+                self.mpi_rank, "warning")
+            return None, None, None
+
+        if self.use_cov:
+            err2use = self.cov_var_delta[iwave][:, w][w, :]
+
+            try:
+                _ = np.linalg.cholesky(err2use)
+            except np.linalg.LinAlgError:
+                logging_mpi(
+                    "Covariance matrix is not positive-definite "
+                    f"{self.waveobs[iwave]:.2f} A. Fallback to diagonals.",
+                    self.mpi_rank, "warning")
+
+                err2use = self.e_var_delta[wave_slice][w]
+        else:
+            err2use = self.e_var_delta[wave_slice][w]
+
+        return wave_slice, w, err2use
+
     def fit(self, initial_guess, smooth=True):
         """ Syncronize all MPI processes and fit for ``var_lss`` and ``eta``.
 
         Second axis always contains ``eta`` values. Example::
 
             var_lss = initial_guess[:, 0]
             eta = initial_guess[:, 1]
@@ -1184,41 +1223,21 @@
         self._allreduce()
         self._calc_subsampler_stats()
 
         nfails = 0
         fit_results = np.zeros_like(initial_guess)
         std_results = np.zeros_like(initial_guess)
 
-        w_gtr_min = ((self.num_pixels > VarLSSFitter.min_num_pix)
-                     & (self.num_qso > VarLSSFitter.min_num_qso))
-
-        if self.use_cov:
-            err_base = self.cov_var_delta
-        else:
-            err_base = self.e_var_delta
-
         for iwave in range(self.nwbins):
-            i1 = iwave * self.nvarbins
-            i2 = i1 + self.nvarbins
-            wave_slice = np.s_[i1:i2]
-            w = w_gtr_min[wave_slice]
+            wave_slice, w, err2use = self._get_wave_bin_slice_params(iwave)
 
-            if w.sum() == 0:
+            if w is None:
                 nfails += 1
-                logging_mpi(
-                    "Not enough statistics for VarLSSFitter at"
-                    f" wave_obs: {self.waveobs[iwave]:.2f}.",
-                    self.mpi_rank, "warning")
                 continue
 
-            if self.use_cov:
-                err2use = err_base[iwave][:, w][w, :]
-            else:
-                err2use = err_base[wave_slice][w]
-
             try:
                 pfit, pcov = curve_fit(
                     VarLSSFitter.variance_function,
                     self.var_centers[wave_slice][w],
                     self.var_delta[wave_slice][w],
                     p0=initial_guess[iwave],
                     sigma=err2use,
```

### Comparing `qsonic-0.7.4/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.7.5/py/qsonic/scripts/qsonic_calib.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,11 +269,12 @@
     logging.basicConfig(level=logging.DEBUG)
     logging.captureWarnings(True)
 
     try:
         mpi_run_all(comm, mpi_rank, mpi_size)
     except QsonicException as e:
         logging_mpi(e, mpi_rank, "exception")
+        exit(1)
     except Exception as e:
         logging.error(f"Unexpected error on Rank{mpi_rank}. Abort.")
         logging.exception(e)
         comm.Abort()
```

### Comparing `qsonic-0.7.4/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.7.5/py/qsonic/scripts/qsonic_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,20 @@
     parser = qsonic.calibration.add_calibration_parser(parser)
 
     analysis_group = parser.add_argument_group('Analysis options')
     analysis_group.add_argument(
         "--smoothing-scale", default=16., type=float,
         help="Smoothing scale for pipeline noise in A.")
     analysis_group.add_argument(
-        "--min-rsnr", type=float, default=0.,
+        "--min-rsnr", type=float, default=0,
         help="Minium SNR <F/sigma> above Lya.")
     analysis_group.add_argument(
+        "--min-forestsnr", type=float, default=0,
+        help="Minium SNR <F/sigma> within the forest.")
+    analysis_group.add_argument(
         "--skip", type=qsonic.io._float_range(0, 1), default=0.2,
         help="Skip short spectra lower than given ratio.")
 
     parser = qsonic.spectrum.add_wave_region_parser(parser)
     parser = qsonic.masks.add_mask_parser(parser)
     parser = add_picca_continuum_parser(parser)
 
@@ -345,14 +348,18 @@
 
     apply_masks(maskers, spectra_list, mpi_rank)
 
     # remove from sample if no pixels is small
     spectra_list = remove_short_spectra(
         spectra_list, args.forest_w1, args.forest_w2, args.skip, mpi_rank)
 
+    # Remove spectra with respect to forest snr
+    spectra_list = [spec for spec in spectra_list
+                    if spec.get_effective_meansnr() >= args.min_forestsnr]
+
     # Create smoothed ivar as intermediate variable
     if args.smoothing_scale > 0:
         for spec in spectra_list:
             spec.set_smooth_forestivar(args.smoothing_scale)
 
     # Continuum fitting
     spectra_list = mpi_continuum_fitting(spectra_list, args, comm, mpi_rank)
@@ -378,14 +385,15 @@
         level=logging.DEBUG)
     logging.captureWarnings(True)
 
     try:
         mpi_run_all(comm, mpi_rank, mpi_size)
     except QsonicException as e:
         logging_mpi(e, mpi_rank, "exception")
+        exit(1)
     except Exception as e:
         logging.error(f"Unexpected error on Rank{mpi_rank}. Abort.")
         logging.exception(e)
         comm.Abort()
 
     etime = (time.time() - start_time) / 60  # min
     logging_mpi(f"Total time spent is {etime:.1f} mins.", mpi_rank)
```

### Comparing `qsonic-0.7.4/py/qsonic/spectrum.py` & `qsonic-0.7.5/py/qsonic/spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,14 +364,35 @@
         """
         size = 0
         for ivar_arm in self.forestivar.values():
             size += np.sum(ivar_arm > 0)
 
         return size
 
+    def get_effective_meansnr(self):
+        """ Calculate a weighted average of :attr:`mean_snr` over arms. Only
+        call if :meth:`set_forest_region` has been called.
+
+        .. math::
+            \\langle\\mathrm{SNR}\\rangle = \\sum_{i} \\mathrm{SNR}_i^3 \\bigg/
+            {\\sum_{i} \\mathrm{SNR}_i^2}
+
+        Returns
+        -------
+        float: Effective mean SNR.
+        """
+        msnr_eff = 0
+        norm = 1e-8
+
+        for val in self.mean_snr.values():
+            msnr_eff += val**3
+            norm += val**2
+
+        return msnr_eff / norm
+
     def is_long(self, dforest_wave, skip_ratio):
         """Determine if spectrum is long enough to be accepted.
 
         The condition is :meth:`get_real_size` > ``skip_ratio * npixels``,
         where ``npixels`` :math:`=(1 + z_\\mathrm{qso}) \\times`
         ``dforest_wave`` :math:`/ \\mathrm{d}\\lambda` and
         :math:`\\mathrm{d}\\lambda` is wavelength spacing in the observed frame
```

### Comparing `qsonic-0.7.4/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.7.5/py/qsonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.4
+Version: 0.7.5
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.7.4/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.7.5/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/setup.cfg` & `qsonic-0.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.4
+current_version = 0.7.5
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.7.4/tests/test_catalog.py` & `qsonic-0.7.5/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_io.py` & `qsonic-0.7.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_masks.py` & `qsonic-0.7.5/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_mathtools.py` & `qsonic-0.7.5/tests/test_mathtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,29 +52,34 @@
         ivar[idces] = 0
 
         ivar_sm = qsonic.mathtools.get_smooth_ivar(ivar)
         npt.assert_allclose(ivar_sm[idces], 0)
         npt.assert_allclose(ivar_sm, ivar)
 
     def test_SubsampleCov_theory(self):
-        subsampler = qsonic.mathtools.SubsampleCov(1, 100)
+        subsampler = qsonic.mathtools.SubsampleCov((2, 1), 100)
 
         randoms = np.random.default_rng().normal(size=100000)
 
         true_mean = np.mean(randoms)
         true_var = np.std(randoms)**2
         var_on_mean = true_var / randoms.size
 
         for r in randoms:
-            subsampler.add_measurement(r, 1)
+            xvec = np.empty((2, 1))
+            xvec[0] = r
+            xvec[1] = 2 * r
+            subsampler.add_measurement(xvec, 1)
 
         mean, cov = subsampler.get_mean_n_cov()
 
-        npt.assert_allclose(mean, true_mean)
+        npt.assert_allclose(mean[0], true_mean)
+        npt.assert_allclose(mean[1], 2 * true_mean)
         npt.assert_almost_equal(cov[0][0], var_on_mean, decimal=4)
+        npt.assert_almost_equal(cov[1][0], 4 * var_on_mean, decimal=4)
 
     def test_SubsampleCov_shape(self):
         subsampler = qsonic.mathtools.SubsampleCov((3, 10), 20)
         randoms = np.random.default_rng().normal(size=(100, 3, 10))
         randoms[:, 1, :] += 1
         randoms[:, 2, :] += 2
```

### Comparing `qsonic-0.7.4/tests/test_mpi_utils.py` & `qsonic-0.7.5/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_picca_continuum.py` & `qsonic-0.7.5/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_qsonic_calib.py` & `qsonic-0.7.5/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.4/tests/test_spectrum.py` & `qsonic-0.7.5/tests/test_spectrum.py`

 * *Files identical despite different names*

