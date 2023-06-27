# Comparing `tmp/spright-23.6.24.tar.gz` & `tmp/spright-23.6.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spright-23.6.24.tar", last modified: Sat Jun 24 18:06:56 2023, max compression
+gzip compressed data, was "spright-23.6.27.tar", last modified: Tue Jun 27 21:32:34 2023, max compression
```

## Comparing `spright-23.6.24.tar` & `spright-23.6.27.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.217131 spright-23.6.24/
--rw-r--r--   0 hannu     (1000) hannu     (1000)    35149 2022-10-08 15:41:02.000000 spright-23.6.24/LICENSE
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       19 2022-10-24 17:07:23.000000 spright-23.6.24/MANIFEST.in
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-24 18:06:56.217131 spright-23.6.24/PKG-INFO
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      544 2023-06-16 10:55:09.000000 spright-23.6.24/README.md
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      957 2023-06-24 18:05:26.000000 spright-23.6.24/pyproject.toml
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       38 2023-06-24 18:06:56.217131 spright-23.6.24/setup.cfg
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/spright/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      113 2023-06-16 11:10:55.000000 spright-23.6.24/spright/__init__.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      686 2023-06-16 11:10:55.000000 spright-23.6.24/spright/core.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     4057 2023-06-16 11:10:55.000000 spright-23.6.24/spright/distribution.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     1740 2023-06-16 11:10:55.000000 spright-23.6.24/spright/io.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3119 2023-06-16 11:10:55.000000 spright-23.6.24/spright/lpf.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)    10980 2023-06-24 18:03:22.000000 spright-23.6.24/spright/model.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3147 2023-06-16 11:10:55.000000 spright-23.6.24/spright/rdmodel.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)    11166 2023-06-16 11:10:55.000000 spright-23.6.24/spright/rmestimator.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3722 2023-06-22 14:20:14.000000 spright-23.6.24/spright/rmrelation.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       67 2023-06-16 11:10:55.000000 spright-23.6.24/spright/version.py
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/spright.egg-info/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/PKG-INFO
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      414 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/SOURCES.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        1 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/dependency_links.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       76 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/requires.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        8 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/top_level.txt
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/tests/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       58 2023-06-16 16:52:08.000000 spright-23.6.24/tests/test_installation.py
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-27 21:32:34.409185 spright-23.6.27/
+-rw-r--r--   0 hannu     (1000) hannu     (1000)    35149 2022-10-08 15:41:02.000000 spright-23.6.27/LICENSE
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       19 2022-10-24 17:07:23.000000 spright-23.6.27/MANIFEST.in
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-27 21:32:34.409185 spright-23.6.27/PKG-INFO
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     1338 2023-06-27 21:30:33.000000 spright-23.6.27/README.md
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      976 2023-06-27 21:32:19.000000 spright-23.6.27/pyproject.toml
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       38 2023-06-27 21:32:34.409185 spright-23.6.27/setup.cfg
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-27 21:32:34.409185 spright-23.6.27/spright/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      113 2023-06-16 11:10:55.000000 spright-23.6.27/spright/__init__.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      686 2023-06-16 11:10:55.000000 spright-23.6.27/spright/core.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     4221 2023-06-27 21:30:33.000000 spright-23.6.27/spright/distribution.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     1740 2023-06-16 11:10:55.000000 spright-23.6.27/spright/io.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     3119 2023-06-16 11:10:55.000000 spright-23.6.27/spright/lpf.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)    10980 2023-06-27 21:30:33.000000 spright-23.6.27/spright/model.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     3147 2023-06-16 11:10:55.000000 spright-23.6.27/spright/rdmodel.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     7543 2023-06-27 21:30:33.000000 spright-23.6.27/spright/relationmap.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)    12088 2023-06-27 21:30:33.000000 spright-23.6.27/spright/rmestimator.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     5803 2023-06-27 21:30:33.000000 spright-23.6.27/spright/rmrelation.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       67 2023-06-16 11:10:55.000000 spright-23.6.27/spright/version.py
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-27 21:32:34.409185 spright-23.6.27/spright.egg-info/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-27 21:32:33.000000 spright-23.6.27/spright.egg-info/PKG-INFO
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      437 2023-06-27 21:32:33.000000 spright-23.6.27/spright.egg-info/SOURCES.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)        1 2023-06-27 21:32:33.000000 spright-23.6.27/spright.egg-info/dependency_links.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       90 2023-06-27 21:32:33.000000 spright-23.6.27/spright.egg-info/requires.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)        8 2023-06-27 21:32:33.000000 spright-23.6.27/spright.egg-info/top_level.txt
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-27 21:32:34.409185 spright-23.6.27/tests/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       58 2023-06-16 16:52:08.000000 spright-23.6.27/tests/test_installation.py
```

### Comparing `spright-23.6.24/LICENSE` & `spright-23.6.27/LICENSE`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/PKG-INFO` & `spright-23.6.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spright
-Version: 23.6.24
+Version: 23.6.27
 Summary: Bayesian radius-density-mass relation for small planets.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
 Project-URL: homepage, https://github.com/hpparvi/spright
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `spright-23.6.24/pyproject.toml` & `spright-23.6.27/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "spright"
-version = "23.06.24"
+version = "23.06.27"
 description = 'Bayesian radius-density-mass relation for small planets.'
 authors=[{name='Hannu Parviainen', email='hpparvi@gmail.com'}]
 classifiers=[
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
 ]
 keywords = ['astronomy',  'astrophysics',  'exoplanets']
-dependencies = ["numpy", "numba", "scipy", "pandas", "astropy", "pytransit", "arviz", "corner", "tqdm", "celerite", "emcee"]
+dependencies = ["numpy", "numba", "scipy", "uncertainties", "pandas",
+  "astropy", "pytransit", "arviz", "corner", "tqdm", "celerite", "emcee"]
 
 [project.urls]
 homepage = 'https://github.com/hpparvi/spright'
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `spright-23.6.24/spright/core.py` & `spright-23.6.27/spright/core.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/spright/distribution.py` & `spright-23.6.27/spright/distribution.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
             self._minimization_result = res = minimize(minfun, array([0.5, m1, 0.5, 1.5, m2, 0.5, 1.5]),
                                                        method='powell')
             self.model, self.model_pars, self._m1, self._m2 = dmodel, res.x, res.x[1], res.x[4]
             return dmodel, res.x, res.x[1], res.x[4]
 
     def plot(self, plot_model: bool = True, plot_modes: bool = True, ax = None):
+        plot_model &= self.model is not None
         ps = percentile(self.samples, [50, 16, 84, 2.5, 97.5])
         x, y = self._fit_kde()
         il, iu = argmin(abs(x - ps[1])), argmin(abs(x - ps[2]))
         ill, iuu = argmin(abs(x - ps[3])), argmin(abs(x - ps[4]))
 
         if ax is None:
             fig, ax = subplots()
@@ -91,19 +92,21 @@
 
         ax.fill_between(x, y, alpha=0.5)
         ax.fill_between(x[ill:iuu], y[ill:iuu], lw=2, fc='k', alpha=0.25)
         ax.fill_between(x[il:iu], y[il:iu], lw=2, fc='k', alpha=0.25)
         ax.plot(x, y, 'k')
         if plot_model:
             ax.plot(x, self.model(x, self.model_pars), '--k')
-        if plot_modes:
-            ax.axvline(self._m1, c='k', ls='--')
-            if self._m2 is not None:
-                ax.axvline(self._m2, c='k', ls='--')
+            if plot_modes:
+                ax.axvline(self._m1, c='k', ls='--')
+                if self._m2 is not None:
+                    ax.axvline(self._m2, c='k', ls='--')
 
         xlabel = {'density': r'Density [g cm$^{-3}$]',
                   'relative density': r'Density [$\rho_{rocky}$]',
-                  'mass': r'Mass [M$_\oplus$]'}[self.quantity]
+                  'mass': r'Mass [M$_\oplus$]',
+                  'radius': r'Radius [R$_\oplus$]',
+                  'k': r'RV semi-amplitude [m/s]'}[self.quantity]
 
         setp(ax, ylabel='Posterior probability', xlabel=xlabel, yticks=[], xlim=percentile(self.samples, [1, 99]))
         if fig is not None:
             fig.tight_layout()
```

### Comparing `spright-23.6.24/spright/io.py` & `spright-23.6.27/spright/io.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/spright/lpf.py` & `spright-23.6.27/spright/lpf.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/spright/model.py` & `spright-23.6.27/spright/model.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/spright/rdmodel.py` & `spright-23.6.27/spright/rdmodel.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.24/spright/rmestimator.py` & `spright-23.6.27/spright/rmestimator.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     ndarray, nan
 from numpy.random import multivariate_normal, permutation, seed, normal
 from scipy.optimize import minimize
 
 from .rdmodel import RadiusDensityModel
 from .version import version
 from .core import mearth, rearth
-from .model import model, lnlikelihood_vp, create_radius_density_icdf
+from .model import model, create_radius_mass_map, create_radius_density_map
+from .relationmap import RMRelationMap, RDRelationMap
 from .lpf import LPF
 
 
 class RMEstimator:
     """A class that computes a numerical radius-density relation.
 
     """
     def __init__(self, nsamples: int = 50,
-                 tbl_file: Optional[Path] = None, use_tabulated_rho: bool = False, mask_bad: bool = True,
                  names: Optional[ndarray] = None,
                  radii: Optional[tuple[ndarray, ndarray]] = None,
                  masses: Optional[tuple[ndarray, ndarray]] = None,
                  densities: Optional[tuple[ndarray, ndarray]] = None):
 
         self.radius_means: Optional[ndarray] = None
         self.radius_uncertainties: Optional[ndarray] = None
@@ -57,24 +57,22 @@
 
         self.nplanets: int = 0
         self.nsamples: int = 0
 
         self._init_data(names, radii, masses, densities)
         self._create_samples(nsamples)
 
-        self.rdm = RadiusDensityModel()
-        self.lpf = LPF(self.radius_samples, self.density_samples, self.rdm)
+        self.rdmodel = RadiusDensityModel()
+        self.lpf = LPF(self.radius_samples, self.density_samples, self.rdmodel)
+
+        self.rdmap: Optional[RDRelationMap] = None
+        self.rmmap: Optional[RMRelationMap] = None
 
-        self.rdmap: Optional[ndarray] = None
-        self.icdf: Optional[ndarray] = None
         self._optimization_result = None
         self._posterior_sample = None
-        self._ra = None
-        self._da = None
-        self._pa = None
 
     def _init_data(self, names: ndarray,
                    radii: tuple[ndarray, ndarray],
                    masses: tuple[ndarray, ndarray],
                    densities: tuple[ndarray, ndarray]):
         self.planet_names = names
         self.radius_means, self.radius_uncertainties = radii
@@ -125,59 +123,76 @@
     def posterior_samples(self, burn: int = 0, thin: int = 1):
         return self.lpf.posterior_samples(burn, thin)
 
     def compute_maps(self, nsamples: int = 1500,
                      rres: int = 200, dres: int = 100, pres: int = 100,
                      rlims: tuple[float, float] = (0.5, 6.0),
                      dlims: tuple[float, float] = (0, 12),
+                     mlims: tuple[float, float] = (0, 25),
                      rseed: int = 0):
         seed(rseed)
+        rd = self.rdmodel
         df = self.lpf.posterior_samples()
-        xi = permutation(df.shape[0])[:nsamples]
-        self._posterior_sample = pvs = df.iloc[xi]
-        rd = self.lpf.rdm
-        self._ra, self._da, self._pa, self.rdmap, self.icdf = create_radius_density_icdf(pvs.values,
-                                                                                         rd._r0, rd._dr, rd.drocky, rd.dwater,
-                                                                                         pres, rlims, dlims, rres, dres)
+        self._posterior_sample = pvs = df.iloc[permutation(df.shape[0])[:nsamples]]
+        radii, densities, rdm = create_radius_density_map(pvs.values, rd._r0, rd._dr, rd.drocky, rd.dwater,
+                                                          dres=dres, rres=rres, dlims=dlims, rlims=rlims)
+        radii, masses, rmm = create_radius_mass_map(pvs.values, rd._r0, rd._dr, rd.drocky, rd.dwater,
+                                                    mres=dres, rres=rres, mlims=mlims, rlims=rlims)
+        self.rdmap = RDRelationMap(rdm, radii, densities, pres)
+        self.rmmap = RMRelationMap(rmm, radii, masses, pres)
 
     def save(self, filename: Optional[Path] = None):
-        if self.lpf.sampler is None or self.rdmap is None or self.icdf is None:
-            raise ValueError("Cannot save before computing the idcf")
+        if self.lpf.sampler is None or self.rdmap is None:
+            raise ValueError("Cannot save before computing the maps")
+
+        rdh = pf.PrimaryHDU(self.rdmap.data)
+        rdc = pf.ImageHDU(self.rdmap.xy_cdf, name='rd_cdf')
+        rdi = pf.ImageHDU(self.rdmap.xy_icdf, name='rd_icdf')
+        drc = pf.ImageHDU(self.rdmap.yx_cdf, name='dr_cdf')
+        dri = pf.ImageHDU(self.rdmap.yx_icdf, name='dr_icdf')
+
+        rmr = pf.ImageHDU(self.rmmap.data, name='rmr')
+        rmc = pf.ImageHDU(self.rmmap.xy_cdf, name='rm_cdf')
+        rmi = pf.ImageHDU(self.rmmap.xy_icdf, name='rm_icdf')
+        mrc = pf.ImageHDU(self.rmmap.yx_cdf, name='mr_cdf')
+        mri = pf.ImageHDU(self.rmmap.yx_icdf, name='mr_icdf')
 
-        rdh = pf.PrimaryHDU(self.rdmap)
-        ich = pf.ImageHDU(self.icdf, name='icdf')
         smh = pf.BinTableHDU(Table.from_pandas(self._posterior_sample), name='samples')
 
-        d = self._da
-        r = self._ra
-        p = self._pa
-
-        rdh.header['CTYPE1'] = 'density'
-        rdh.header['CRPIX1'] = 1
-        rdh.header['CRVAL1'] = d[0]
-        rdh.header['CDELT1'] = d[1] - d[0]
-
-        rdh.header['CTYPE2'] = 'radius'
-        rdh.header['CRPIX2'] = 1
-        rdh.header['CRVAL2'] = r[0]
-        rdh.header['CDELT2'] = r[1] - r[0]
+        d = self.rdmap.y
+        m = self.rmmap.y
+        r = self.rdmap.x
+        p = self.rdmap.probs
+
+        def set_axes(h, xname, yname, x, y):
+            h.header['CTYPE1'] = yname
+            h.header['CRPIX1'] = 1
+            h.header['CRVAL1'] = y[0]
+            h.header['CDELT1'] = y[1] - y[0]
+
+            h.header['CTYPE2'] = xname
+            h.header['CRPIX2'] = 1
+            h.header['CRVAL2'] = x[0]
+            h.header['CDELT2'] = x[1] - x[0]
+
+        set_axes(rdh, 'radius', 'density', r, d)
+        set_axes(rdc, 'radius', 'density', r, d)
+        set_axes(rdi, 'radius', 'icdf', r, p)
+        set_axes(drc, 'density', 'radius', d, r)
+        set_axes(dri, 'density', 'icdf', d, p)
+
+        set_axes(rmr, 'radius', 'mass', r, d)
+        set_axes(rmc, 'radius', 'mass', r, d)
+        set_axes(rmi, 'radius', 'icdf', r, p)
+        set_axes(mrc, 'mass', 'radius', m, r)
+        set_axes(mri, 'mass', 'icdf', m, p)
 
-        rdh.header['CREATOR'] = f'Moot v{str(version)} '
+        rdh.header['CREATOR'] = f'Spright v{str(version)} '
         rdh.header['CREATED'] = Time.now().to_value('fits', 'date')
 
-        ich.header['CTYPE1'] = 'icdf'
-        ich.header['CRPIX1'] = 1
-        ich.header['CRVAL1'] = p[0]
-        ich.header['CDELT1'] = p[1] - p[0]
-
-        ich.header['CTYPE2'] = 'radius'
-        ich.header['CRPIX2'] = 1
-        ich.header['CRVAL2'] = r[0]
-        ich.header['CDELT2'] = r[1] - r[0]
-
         # Catalog
         tbs = Table(data=[self.planet_names.astype('a20'),
                           self.radius_means, self.radius_uncertainties,
                           self.mass_means, self.mass_uncertainties,
                           self.density_means, self.density_uncertainties],
                     names=['name', 'radius', 'radius_e', 'mass', 'mass_e', 'density', 'density_e'],
                     units=[None, 'R_Earth', 'R_Earth', 'M_Earth', 'M_Earth', 'g cm^-3', 'g cm^-3'])
@@ -187,15 +202,15 @@
         tbs = Table(data=[self.radius_samples.ravel(),
                           self.mass_samples.ravel(),
                           self.density_samples.ravel()],
                     names=['radius', 'mass', 'density'],
                     units=['R_Earth', 'M_Earth', 'g cm^-3'])
         rms = pf.BinTableHDU(tbs, name='rmsamples')
 
-        hdul = pf.HDUList([rdh, ich, smh, cat, rms])
+        hdul = pf.HDUList([rdh, rdc, rdi, drc, dri, rmr, rmc, rmi, mrc, mri, smh, cat, rms])
         filename = filename or Path('rdmap.fits')
         hdul.writeto(filename, overwrite=True)
 
 
     def plot_radius_density(self, pv=None, rhores: int = 200, radres: int = 200, ax=None,
                             max_samples: int = 500, cmap=None, components=None, plot_contours=False):
         arho = linspace(0, 15, rhores)
```

### Comparing `spright-23.6.24/spright.egg-info/PKG-INFO` & `spright-23.6.27/spright.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spright
-Version: 23.6.24
+Version: 23.6.27
 Summary: Bayesian radius-density-mass relation for small planets.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
 Project-URL: homepage, https://github.com/hpparvi/spright
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

