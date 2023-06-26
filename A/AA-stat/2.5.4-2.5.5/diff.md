# Comparing `tmp/AA_stat-2.5.4.tar.gz` & `tmp/AA_stat-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AA_stat-2.5.4.tar", last modified: Fri May 13 15:14:31 2022, max compression
+gzip compressed data, was "AA_stat-2.5.5.tar", last modified: Mon Jun 26 22:57:15 2023, max compression
```

## Comparing `AA_stat-2.5.4.tar` & `AA_stat-2.5.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:31.142295 AA_stat-2.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:31.138296 AA_stat-2.5.4/AA_stat/
--rw-r--r--   0 runner    (1001) docker     (121)    19447 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/AA_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7954 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/aa_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/default.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:31.142295 AA_stat-2.5.4/AA_stat/gui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9233 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     3942 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/gui/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/gui/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (121)    15745 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/html.py
--rw-r--r--   0 runner    (1001) docker     (121)    20327 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    16886 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/localization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5235 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/open_search.params
--rw-r--r--   0 runner    (1001) docker     (121)    14538 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (121)    10278 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/report.template
--rw-r--r--   0 runner    (1001) docker     (121)    19245 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    19608 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)  2386895 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/unimod.xml
--rw-r--r--   0 runner    (1001) docker     (121)    16866 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-13 15:14:21.000000 AA_stat-2.5.4/AA_stat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-13 15:14:31.142295 AA_stat-2.5.4/AA_stat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23465 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-13 15:14:31.000000 AA_stat-2.5.4/AA_stat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9346 2022-05-13 15:14:21.000000 AA_stat-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    23465 2022-05-13 15:14:31.142295 AA_stat-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-13 15:14:21.000000 AA_stat-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-13 15:14:31.142295 AA_stat-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-05-13 15:14:21.000000 AA_stat-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:15.367834 AA_stat-2.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:15.367834 AA_stat-2.5.5/AA_stat/
+-rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/AA_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/aa_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/default.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:15.367834 AA_stat-2.5.5/AA_stat/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/gui/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/gui/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/open_search.params
+-rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/report.template
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2386895 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/unimod.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 22:57:07.000000 AA_stat-2.5.5/AA_stat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:57:15.367834 AA_stat-2.5.5/AA_stat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 22:57:15.000000 AA_stat-2.5.5/AA_stat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-26 22:57:07.000000 AA_stat-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-06-26 22:57:15.367834 AA_stat-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 22:57:07.000000 AA_stat-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:57:15.367834 AA_stat-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 22:57:07.000000 AA_stat-2.5.5/setup.py
```

### Comparing `AA_stat-2.5.4/AA_stat/AA_stat.py` & `AA_stat-2.5.5/AA_stat/AA_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,23 +319,25 @@
     """
     save_directory = args.dir
 
     logger.debug('Fixed modifications: %s', params_dict['fix_mod'])
     logger.debug('Variable modifications: %s', params_dict['var_mod'])
     logger.info('Using fixed modifications: %s.', utils.format_mod_dict(utils.masses_to_mods(params_dict['fix_mod'])))
     logger.info('Variable modifications in search results: %s.', utils.format_mod_list(params_dict['var_mod']))
+    logger.debug('Enzyme specificity: %s', params_dict['enzyme'])
     data = io.read_input(args, params_dict)
     if data is None:
         sys.exit(1)
 
-    hist, popt_pvar = stats.fit_peaks(data, args, params_dict)
+    popt_pvar = stats.fit_peaks(data, args, params_dict)
     # logger.debug('popt_pvar: %s', popt_pvar)
     final_mass_shifts = filter_mass_shifts(popt_pvar, tolerance=params_dict['shift_error'] * params_dict['bin_width'])
     # logger.debug('final_mass_shifts: %s', final_mass_shifts)
     mass_shift_data_dict = utils.group_specific_filtering(data, final_mass_shifts, params_dict)
+    del data
     # logger.debug('mass_shift_data_dict: %s', mass_shift_data_dict)
     if not mass_shift_data_dict:
         html.render_html_report(None, mass_shift_data_dict, None, params_dict, {}, {}, {}, [], save_directory, [], step=step)
         return None, None, None, mass_shift_data_dict, {}
 
     reference_label, reference_mass_shift = get_zero_mass_shift(mass_shift_data_dict, params_dict)
     if abs(reference_mass_shift) < params_dict['zero bin tolerance']:
```

### Comparing `AA_stat-2.5.4/AA_stat/aa_search.py` & `AA_stat-2.5.5/AA_stat/aa_search.py`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/default.cfg` & `AA_stat-2.5.5/AA_stat/default.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -81,7 +81,9 @@
 [modifications]
 recommend variable modifications: 5
 recommend multiple modifications on residue: yes
 fixed modification intensity threshold: 3  # maximum % of peptides containing AA at zero shift to consider a fixed modification
 peptide count factor threshold: 2  # factor for peptide % threshold to justify fixed modification
 isotope error abundance threshold: 10  # minimum % of isotope error to justify recommendation of isotope error
 minimum localization count: 10  # minimum absolute localization count to recommend a variable modification
+configured fixed modifications:  # for CSV input, specify here the fixed modifications used in your search. Example: "+57.0215 @ C, +229.1629 @ K, +229.1630 @ N-term"
+configured variable modifications:  # for CSV input, specify here the variable modifications used in your search. Example: "15.9959 @ M, 42.0106 @ N-term"
```

### Comparing `AA_stat-2.5.4/AA_stat/gui/gui.py` & `AA_stat-2.5.5/AA_stat/gui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,14 @@
     edit_params_btn = tk.Button(master=params_frame, width=10, padx=4, text="Edit params",
         command=partial(edit_params, window, params_lbl))
 
     load_params_btn.pack(side=tk.LEFT, fill=tk.X, anchor=tk.E)
     edit_params_btn.pack(side=tk.LEFT, fill=tk.X, anchor=tk.E)
     params_lbl.pack(side=tk.LEFT, fill=tk.X, anchor=tk.W, padx=15)
 
-
     input_frame.pack(side=tk.TOP, fill=tk.X, expand=True)
     spectra_frame.pack(side=tk.TOP, fill=tk.X, expand=True)
     dir_frame.pack(side=tk.TOP, fill=tk.X, expand=True)
     params_frame.pack(side=tk.TOP, fill=tk.X, expand=True)
 
     top_frame.pack()
     main_frame.pack(fill=tk.BOTH, expand=True)
```

### Comparing `AA_stat-2.5.4/AA_stat/gui/logging.py` & `AA_stat-2.5.5/AA_stat/gui/logging.py`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/gui/shortcut.py` & `AA_stat-2.5.5/AA_stat/gui/shortcut.py`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/html.py` & `AA_stat-2.5.5/AA_stat/html.py`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/io.py` & `AA_stat-2.5.5/AA_stat/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 import matplotlib
 matplotlib.use('Agg')
 import pylab as plt
 from matplotlib.backends.backend_pdf import PdfPages
 
+import sys
 import ast
 import os
 import glob
 from configparser import ConfigParser
 import multiprocessing as mp
 from collections import defaultdict
 import logging
-import operator
 import re
-
 import numpy as np
 import pandas as pd
 from pyteomics import pepxml, mgf, mzml
 from . import utils, stats
 
 AA_STAT_PARAMS_DEFAULT = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'default.cfg')
 logger = logging.getLogger(__name__)
 
 
+def sanitize_df(df, params_dict):
+    # drop unneeded columns
+    column_keys = ['proteins_column', 'peptides_column', 'mass_shifts_column', 'score_column', 'measured_mass_column',
+    'calculated_mass_column', 'rt_column', 'next_aa_column', 'prev_aa_column', 'spectrum_column', 'charge_column', 'mods_column']
+    needed = {params_dict[k] for k in column_keys}
+    to_drop = [c for c in df.columns if c not in needed]
+    old_size = df.shape[1]
+    df.drop(to_drop, axis=1, inplace=True)
+    logger.debug('Kept %d and dropped %d out of %d initial columns.', df.shape[1], len(to_drop), old_size)
+
+    # TODO: simplify and sanitize columns here
+    return df
+
+
 def preprocess_df(df, filename, params_dict):
     '''
     Preprocesses DataFrame.
 
     Parameters
     ----------
     df: DataFrame
@@ -53,14 +66,15 @@
             isdddict[prefix] = isd
         prefix = max(isdddict, key=isdddict.get)
         logger.debug('Selected prefix %s for file %s (%d decoys)', prefix, filename, isdddict[prefix])
     else:
         prefix = params_dict['decoy_prefix']
 
     df['is_decoy'] = df[params_dict['proteins_column']].apply(lambda s: all(x.startswith(prefix) for x in s))
+    del df[params_dict['proteins_column']]
 
     if not df['is_decoy'].sum():
         logger.error('No decoy IDs found in %s.', filename)
         if not params_dict['decoy_prefix']:
             logger.error('Configured decoy prefixes are: %s. Check you files or config.',
                 ', '.join(params_dict['decoy_prefix_list']))
         else:
@@ -68,14 +82,15 @@
         return
     ms, filtered = utils.fdr_filter_mass_shift([None, zero_bin, window], df, params_dict)
     n = filtered.shape[0]
     logger.debug('%d filtered peptides near zero.', n)
     df[shifts] = utils.choose_correct_massdiff(
         df[shifts],
         df[params_dict['measured_mass_column']] - df[params_dict['calculated_mass_column']], params_dict)
+
     if params_dict['calibration'] == 'off':
         logger.info('Mass calibration is disabled. Skipping.')
     elif params_dict['calibration'] != 'simple':
         if n < params_dict['min_peptides_for_mass_calibration']:
             logger.warning('Skipping mass calibration: not enough peptides near zero mass shift.')
         else:
             to_fit, unit = stats.get_fittable_series(filtered, params_dict)
@@ -155,16 +170,19 @@
                     plt.hist(floc.loc[clustering.labels_ == i, shifts], label=i, alpha=0.2, bins=25, density=True)
                 plt.xlabel(shifts)
                 plt.legend()
                 pp.savefig(f)
                 plt.close()
     pp.close()
     df['file'] = os.path.splitext(os.path.basename(filename))[0]
-    df['check_composition'] = df[params_dict['peptides_column']].apply(lambda x: utils.check_composition(x, params_dict['labels']))
-    return df.loc[df['check_composition']]
+    check_composition = df[params_dict['peptides_column']].apply(lambda x: utils.check_composition(x, params_dict['labels']))
+    del df[params_dict['measured_mass_column']]
+    del df[params_dict['calculated_mass_column']]
+    del df[params_dict['rt_column']]
+    return df.loc[check_composition]
 
 
 def read_pepxml(fname, params_dict):
     '''
     Reads pepxml file and preprocess it.
     Parameters
     ----------
@@ -173,17 +191,16 @@
     params_dict: dict
         Dict with all input parameters
     Returns
     -------
     DataFrame
     '''
     logger.debug('Reading %s', fname)
-    df = pepxml.DataFrame(fname, read_schema=False, columns=operator.itemgetter(
-        'peptides_column', 'proteins_column', 'spectrum_column', 'mass_shifts_column', 'charge_column')(params_dict))
-    return preprocess_df(df, fname, params_dict)
+    df = pepxml.DataFrame(fname, read_schema=False)
+    return preprocess_df(sanitize_df(df, params_dict), fname, params_dict)
 
 
 def read_csv(fname, params_dict):
     """
     Reads csv file.
 
     Paramenters
@@ -196,20 +213,24 @@
     Returns
     -------
     A DataFrame of csv file.
 
     """
     # logger.info('Reading %s', fname)
     df = pd.read_csv(fname, sep=params_dict['csv_delimiter'])
+    df[params_dict['mods_column']] = df[params_dict['mods_column']].apply(ast.literal_eval)
     protein = params_dict['proteins_column']
-    if (df[protein].str[0] == '[').all() and (df[protein].str[-1] == ']').all():
-        df[protein] = df[protein].apply(ast.literal_eval)
-    else:
-        df[protein] = df[protein].str.split(params_dict['proteins_delimeter'])
-    return preprocess_df(df, fname, params_dict)
+    prev = params_dict['prev_aa_column']
+    next_ = params_dict['next_aa_column']
+    for c in [protein, prev, next_]:
+        if (df[c].str[0] == '[').all() and (df[c].str[-1] == ']').all():
+            df[c] = df[c].apply(ast.literal_eval)
+        else:
+            df[c] = df[c].str.split(params_dict['proteins_delimeter'])
+    return preprocess_df(sanitize_df(df, params_dict), fname, params_dict)
 
 
 def read_mgf(file_path):
     return mgf.IndexedMGF(file_path)
 
 
 def read_mzml(file_path):  # write this
@@ -220,43 +241,51 @@
 
     readers = {
         'mgf': read_mgf,
         'mzml': read_mzml,
     }
     out_dict = {}
     for ftype, reader in readers.items():
-        filenames = getattr(args, ftype)
-        if filenames:
-            for filename in filenames:
-                name = os.path.split(filename)[-1].split('.')[0]  # write it in a proper way
-                out_dict[name] = reader(filename)
+        spec_filenames = getattr(args, ftype)
+        if spec_filenames:
+            break
+    else:
+        return {}
+    for inp in [args.pepxml, args.csv]:
+        if inp:
+            break
+    if len(inp) != len(spec_filenames):
+        logger.critical('Numbers of input files and spectrum files do not match (%d and %d).', len(inp), len(spec_filenames))
+        sys.exit(1)
+
+    for i, filename in zip(inp, spec_filenames):
+        name = os.path.splitext(os.path.basename(i))[0]
+        out_dict[name] = reader(filename)
     return out_dict
 
 
 def read_input(args, params_dict):
     """
     Reads open search output, assembles all data in one DataFrame.
 
     """
     logger.info('Reading input files...')
     readers = {
         'pepxml': read_pepxml,
         'csv': read_csv,
     }
-    shifts = params_dict['mass_shifts_column']
     nproc = params_dict['processes']
     if nproc == 1:
         dfs = []
         logger.debug('Reading files in one process.')
         for ftype, reader in readers.items():
             filenames = getattr(args, ftype)
             logger.debug('Filenames [%s]: %s', ftype, filenames)
             if filenames:
                 for filename in filenames:
-                    # dfs.append(reader(filename, params_dict))
                     dfs.append(reader(filename, params_dict))
     else:
         nfiles = 0
         for ftype, reader in readers.items():
             filenames = getattr(args, ftype)
             if filenames:
                 nfiles += len(filenames)
@@ -279,16 +308,17 @@
     if any(x is None for x in dfs):
         logger.critical('There were errors when reading input.')
         return
     logger.info('Starting analysis...')
     logger.debug('%d dfs collected.', len(dfs))
     data = pd.concat(dfs, axis=0)
     data.index = range(len(data))
-
-    data['bin'] = np.digitize(data[shifts], params_dict['bins'])
+    data['file'] = data['file'].astype('category')
+    logger.debug('Memory usage:')
+    logger.debug(data.memory_usage(deep=True))
     return data
 
 
 def read_config_file(fname):
     params = ConfigParser(delimiters=('=', ':'), comment_prefixes=('#'), inline_comment_prefixes=('#'))
 
     params.read(AA_STAT_PARAMS_DEFAULT)
@@ -376,14 +406,17 @@
     # modifications
     params_dict['variable_mods'] = params.getint('modifications', 'recommend variable modifications')
     params_dict['multiple_mods'] = params.getboolean('modifications', 'recommend multiple modifications on residue')
     params_dict['fix_mod_zero_thresh'] = params.getfloat('modifications', 'fixed modification intensity threshold')
     params_dict['min_fix_mod_pep_count_factor'] = params.getfloat('modifications', 'peptide count factor threshold')
     params_dict['recommend isotope threshold'] = params.getfloat('modifications', 'isotope error abundance threshold')
     params_dict['min_loc_count'] = params.getint('modifications', 'minimum localization count')
+
+    params_dict['fix_mod'] = utils.parse_mod_list(params.get('modifications', 'configured fixed modifications'), 'fixed')
+    params_dict['var_mod'] = utils.parse_mod_list(params.get('modifications', 'configured variable modifications'), 'variable')
     return params_dict
 
 
 def set_additional_params(params_dict):
     if params_dict['specific_mass_shift_flag']:
         logger.info('Custom bin: %s', params_dict['specific_window'])
         params_dict['so_range'] = params_dict['specific_window'][:]
@@ -397,27 +430,59 @@
         params_dict['window'] = int(window) + 1
     else:
         params_dict['window'] = int(window)  # should be odd
     params_dict['bins'] = np.arange(params_dict['so_range'][0],
         params_dict['so_range'][1] + params_dict['bin_width'], params_dict['bin_width'])
 
 
+_rule_to_enz = {
+    'trypsin': {'cut': 'KR', 'no_cut': 'P', 'sense': 'C'},
+}
+
 def get_params_dict(args):
     logger.debug('Received args: %s', args)
     fname = args.params
     outdir = args.dir
     params = read_config_file(fname)
     params_dict = get_parameters(params)
     set_additional_params(params_dict)
+    if args.processes is not None:
+        params_dict['processes'] = args.processes
     params_dict['output directory'] = outdir
     if args.pepxml:
         fmod, vmod = utils.get_fix_var_modifications(args.pepxml[0], params_dict['labels'])
         params_dict['fix_mod'] = fmod
         params_dict['var_mod'] = utils.format_grouped_keys(utils.group_terminal(vmod), params_dict)
         params_dict['enzyme'] = utils.get_specificity(args.pepxml[0])
+    else:
+        if args.fmods:
+            if '@' in args.fmods:
+                params_dict['fix_mod'] = utils.parse_mod_list(args.fmods, 'fixed')
+            else:
+                params_dict['fix_mod'] = ast.literal_eval(args.fmods)
+        elif not params_dict['fix_mod']:
+            logger.info('No fixed modifications specified. Use --fmods to configure them.')
+        if args.vmods:
+            if '@' in args.vmods:
+                params_dict['var_mod'] = utils.parse_mod_list(args.vmods, 'variable')
+            else:
+                params_dict['var_mod'] = ast.literal_eval(args.vmods)
+        elif not params_dict['var_mod']:
+            logger.info('No variable modifications specified. Use --vmods to configure them.')
+        if args.enzyme:
+            if '|' in args.enzyme:
+                params_dict['enzyme'] = utils.convert_tandem_cleave_rule_to_regexp(args.enzyme, params_dict)
+            else:
+                params_dict['enzyme'] = ast.literal_eval(args.enzyme)
+        elif params_dict['rule'] in _rule_to_enz:
+            params_dict['enzyme'] = _rule_to_enz[params_dict['rule']]
+            logger.info('Using standard specificity for %s.', params_dict['rule'])
+        else:
+            logger.info('Enyzme not specified. Use --enzyme to configure.')
+            params_dict['enzyme'] = None
     return params_dict
 
 
 _format_globs = {
     'pepxml': ['*.pepXML', '*.pep.xml'],
     'csv': ['*.csv'],
     'mzml': ['*.mzML'],
```

### Comparing `AA_stat-2.5.4/AA_stat/localization.py` & `AA_stat-2.5.5/AA_stat/localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,17 +375,19 @@
             if ind == 0:
                 loc_stat_dict[utils.format_localization_key('N-term', mass_dict[a[0]])] += 1
             elif ind == len(top_isoform) - 1:
                 loc_stat_dict[utils.format_localization_key('C-term', mass_dict[a[0]])] += 1
             loc_stat_dict[utils.format_localization_key(a[1], mass_dict[a[0]])] += 1
 
     scorediff = (top_score - second_score) / top_score
-    # utils.internal('Returning: %s %s %s', loc_stat_dict, ''.join(top_isoform), scorediff)
     top_i = ''.join(top_isoform)
-    return loc_stat_dict, top_i, top_terms, scorediff, utils.loc_positions(top_isoform)
+    ret = loc_stat_dict, top_i, top_terms, scorediff, utils.loc_positions(top_isoform)
+    utils.internal('Returning: %s', ret)
+
+    return ret
 
 
 def localization(df, ms, ms_label, locations_ms, params_dict, spectra_dict, mass_shift_dict):
     """
     Localizes modification or sum of modifications for mass shift and repeat localization if there are redundant candidates.
     If two peptide isoforms have the same max score, modification counts as 'non-localized'.
 
@@ -398,31 +400,38 @@
     ms_label : str
         Considered mass shift label
     locations_ms :
        locmod_df['loc candidates']
     params_dict : dict
         Dict with all paramenters.
     spectra_dict : dict
-        Keys are filenames and values file with mass spectra.
+        Keys are filenames and values are Pyteomics readers.
 
     Returns
     -------
     Counter of localizations.
     """
     logger.info('Localizing %s...', ms_label)
     logger.debug('Localizations: %s', locations_ms)
     if len(locations_ms) < 2 and list(locations_ms[0].values())[0] == set():
         df['localization_count'], df['top isoform'], df['top_terms'], df['localization score'], df['loc_position'] = None, None, None, None, None
     else:
         z = list(zip(*df.apply(lambda x: localization_of_modification(
                     ms, ms_label, x, locations_ms, params_dict, spectra_dict, mass_shift_dict), axis=1)))
+        utils.internal('z: %s', z)
         names = ['localization_count', 'top isoform', 'top_terms', 'localization score', 'loc_position']
         dt = {'localization score': np.float32}
         for c, v in zip(names, z):
-            df[c] = np.array(v, dtype=dt.get(c, np.object_))
+            t = dt.get(c, np.object_)
+            # utils.internal('Saving %s as %s...', c, t)
+            shape = (len(v), )
+            value = np.empty(shape, t)
+            value[:] = v
+            # utils.internal('Value: %s', value)
+            df[c] = value
     fname = io.table_path(params_dict['output directory'], ms_label)
     peptide = params_dict['peptides_column']
 
     mod_aa = string.ascii_lowercase
     mod_dicts = {}
     for pair in locations_ms:
         labels_mod = {}
```

### Comparing `AA_stat-2.5.4/AA_stat/main.py` & `AA_stat-2.5.5/AA_stat/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,22 @@
     input_spectra.add_argument('--mgf', nargs='+', help='MGF files to localize modifications.')
     input_spectra.add_argument('--mzml', nargs='+', help='mzML files to localize modifications.')
 
     input_file = pars.add_mutually_exclusive_group(required=True)
     input_file.add_argument('--pepxml', nargs='+', help='List of input files in pepXML format.')
     input_file.add_argument('--csv', nargs='+', help='List of input files in CSV format.')
 
+    pars.add_argument('--fmods', help='Fixed modifications specified in the search (needed with CSV input). '
+        'Example: +57.0215 @ C, +229.1630 @ N-term')
+    pars.add_argument('--vmods', help='Variable modifications specified in the search (needed with CSV input). '
+        'Example: 15.9959 @ M, 42.0106 @ N-term')
+    pars.add_argument('--enzyme', help='Enzyme specificity set in the search (needed with CSV input).')
+
+    pars.add_argument('-n', '--processes', type=int, help='Maximum number of processes to use.')
+
     args = pars.parse_args()
     levels = [logging.WARNING, logging.INFO, logging.DEBUG, utils.INTERNAL]
     logging.basicConfig(format='{levelname:>8}: {asctime} {message}',
                         datefmt='[%H:%M:%S]', level=levels[args.verbosity], style='{')
 
     # Performance optimizations as per https://docs.python.org/3/howto/logging.html#optimization
     logging._srcfile = None
```

### Comparing `AA_stat-2.5.4/AA_stat/open_search.params` & `AA_stat-2.5.5/AA_stat/open_search.params`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/recommendations.py` & `AA_stat-2.5.5/AA_stat/recommendations.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     if l10n:
         l10n.pop('non-localized', None)
         top_loc = max(l10n, key=l10n.get)
         logger.debug('Top localization label for %s: %s', mslabel, top_loc)
         return top_loc
 
 
-def get_fixed_mod_raw(aa, data_dict, choices=None):
+def get_fixed_mod_raw(aa, data_dict, params_dict, choices=None):
     dist_aa = []
     for ms, v in data_dict.items():
         if choices is None or ms in choices:
-            dist_aa.append([v[0], v[1]['peptide'].apply(lambda x: x.count(aa)).sum()])
+            dist_aa.append([v[0], v[1][params_dict['peptides_column']].apply(lambda x: x.count(aa)).sum()])
     utils.internal('Counts for %s: %s', aa, dist_aa)
     top_shift = max(dist_aa, key=lambda tup: tup[1])
     return utils.mass_format(top_shift[0])
 
 
 def determine_fixed_mods_nonzero(reference, locmod_df, data_dict):
     """Determine fixed modifications in case the reference shift is not at zero.
@@ -54,15 +54,15 @@
     fix_mod_dict = {}
     reference = utils.mass_format(0)
     aa_rel = aastat_result[reference][2]
     utils.internal('aa_rel:\n%s', aa_rel)
     candidates = aa_rel[aa_rel < fix_mod_zero_thresh].index
     logger.debug('Fixed mod candidates: %s', candidates)
     for i in candidates:
-        candidate_label = get_fixed_mod_raw(i, data_dict)
+        candidate_label = get_fixed_mod_raw(i, data_dict, params_dict)
         if candidate_label != reference:
             # number of peptides with `i` at shift `candidate label` must be higher than ...
             count_cand = data_dict[candidate_label][1][params_dict['peptides_column']].str.contains(i).sum()
             # number of peptides with `i` at shift `reference` by a factor of `min_fix_mod_pep_count_factor`
             count_ref = data_dict[reference][1][params_dict['peptides_column']].str.contains(i).sum()
             # peptide count at candidate shift over # of peptides at reference
             est_ratio = count_cand / len(data_dict[reference][1])
```

### Comparing `AA_stat-2.5.4/AA_stat/report.template` & `AA_stat-2.5.5/AA_stat/report.template`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/stats.py` & `AA_stat-2.5.5/AA_stat/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     args: argsparse
     params_dict : dict
         Parameters dict.
     """
     logger.info('Performing Gaussian fit...')
     fit_batch = params_dict['fit batch']
     half_window = int(params_dict['window'] / 2) + 1
-    hist = np.histogram(data[data['is_decoy'] == False][params_dict['mass_shifts_column']], bins=params_dict['bins'])
+    hist = np.histogram(data.loc[data['is_decoy'] == False, params_dict['mass_shifts_column']], bins=params_dict['bins'])
     hist_y = smooth(hist[0], window_size=params_dict['window'], power=5)
     hist_x = 0.5 * (hist[1][:-1] + hist[1][1:])
     loc_max_candidates_ind = argrelextrema(hist_y, np.greater_equal)[0]
     # smoothing and finding local maxima
     min_height = 2 * np.median(hist[0][hist[0] > 1])
     # minimum bin height expected to be peak approximate noise level as median of all non-negative
     loc_max_candidates_ind = loc_max_candidates_ind[hist_y[loc_max_candidates_ind] >= min_height]
@@ -327,15 +327,15 @@
                 for center in loc_max_candidates_ind])
         ys = np.concatenate([hist[0][center - half_window: center + half_window + 1]
                 for center in loc_max_candidates_ind])
         poptpvar = fit_batch_worker(os.path.join(args.dir, 'gauss_fit.pdf'),
             len(loc_max_candidates_ind), xs, ys, half_window, height_error, sigma_error)
 
     logger.debug('Returning from fit_peaks. Array size is %d.', len(poptpvar))
-    return hist, np.array(poptpvar)
+    return np.array(poptpvar)
 
 
 _Mkstyle = matplotlib.markers.MarkerStyle
 _marker_styles = [_Mkstyle('o', fillstyle='full'), (_Mkstyle('o', fillstyle='left'), _Mkstyle('o', fillstyle='right')),
     (_Mkstyle('o', fillstyle='top'), _Mkstyle('o', fillstyle='bottom')), (_Mkstyle(8), _Mkstyle(9)),
     (_Mkstyle('v'), _Mkstyle('^')), (_Mkstyle('|'), _Mkstyle('_')), (_Mkstyle('+'), _Mkstyle('x'))]
```

### Comparing `AA_stat-2.5.4/AA_stat/tests.py` & `AA_stat-2.5.5/AA_stat/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
         for f in self.pepxml + self.mzml:
             if not os.path.isfile(f):
                 print(f, 'not found, skipping integrative test.')
                 return
 
         args = argparse.Namespace(dir=self.data_dir, pepxml=self.pepxml, mzml=self.mzml,
-            mgf=None, csv=None, params=None)
+            mgf=None, csv=None, params=None, processes=None)
         params_dict = io.get_params_dict(args)
         # params_dict['decoy_prefix'] = 'DECOY_'
         self.figure_data, self.table, self.locmod_df, self.mass_shift_data_dict, self.fix_mods, self.var_mods = AA_stat(params_dict, args)
 
         counts = [57, 179, 173, 540, 100, 82, 102, 279, 57, 67, 282, 52, 102, 66, 125, 60, 139, 145, 71, 2851, 341, 558, 103,
              79, 148, 128, 71, 460, 171, 277, 54, 51, 106, 197, 61, 57, 341, 397, 108, 67, 158, 78]
         # print(self.table['# peptides in bin'].tolist())
```

### Comparing `AA_stat-2.5.4/AA_stat/unimod.xml` & `AA_stat-2.5.5/AA_stat/unimod.xml`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/AA_stat/utils.py` & `AA_stat-2.5.5/AA_stat/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 def fdr_filter_mass_shift(mass_shift, data, params_dict):
     shifts = params_dict['mass_shifts_column']
     ms_shift = data.loc[np.abs(data[shifts] - mass_shift[1]) < mass_shift[2], shifts].mean()
 
     mask = np.abs(data[shifts] - mass_shift[1]) < 3 * mass_shift[2]
     internal('Mass shift %.3f +- 3 * %.3f', mass_shift[1], mass_shift[2])
-    data_slice = data.loc[mask].sort_values(by=[params_dict['score_column'], 'spectrum'],
+    data_slice = data.loc[mask].sort_values(by=[params_dict['score_column'], params_dict['spectrum_column']],
                                 ascending=params_dict['score_ascending']).drop_duplicates(subset=params_dict['peptides_column'])
     internal('%d peptide rows selected for filtering', data_slice.shape[0])
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         df = pepxml.filter_df(data_slice, key=params_dict['score_column'],
             fdr=params_dict['FDR'], reverse=not params_dict['score_ascending'], correction=params_dict['FDR_correction'], is_decoy='is_decoy')
     internal('Filtered data for %s: %d rows', mass_shift, df.shape[0])
@@ -376,14 +376,15 @@
     mass_dict_0['H-'] = 1.007825
     mass_dict_0['-OH'] = 17.00274
     mass_dict_0.update(params_dict['fix_mod'])
     mod_dict = {}
     if modifications:
         internal('Got modifications for peptide %s: %s', row[peptide], modifications)
     for m in modifications:
+        # internal('Parsing modification: %s', m)
         mmass, pos = m.split('@')
         mmass = float(mmass)
         pos = int(pos)
         if pos == 0:
             key = 'H-'
         elif pos == len(row[peptide]) + 1:
             key = '-OH'
@@ -506,7 +507,65 @@
         logger.warning('Reported mass shifts have a high calculation error (%.4f).'
         ' Using own calculations', maxdiff)
         return calculated
     else:
         logger.warning('Reported mass shifts differ from calculated values (up to %.4f).'
         ' Using the reported values. Consider reporting this to the developers.', maxdiff)
         return reported
+
+
+def convert_tandem_cleave_rule_to_regexp(cleavage_rule, params_dict):
+
+    def get_sense(c_term_rule, n_term_rule):
+        if '{' in c_term_rule:
+            return 'N'
+        elif '{' in n_term_rule:
+            return 'C'
+        else:
+            if len(c_term_rule) <= len(n_term_rule):
+                return 'C'
+            else:
+                return 'N'
+
+    def get_cut(cut, no_cut):
+        aminoacids = set(params_dict['labels'])
+        cut = ''.join(aminoacids & set(cut))
+        if '{' in no_cut:
+            no_cut = ''.join(aminoacids & set(no_cut))
+            return cut, no_cut
+        else:
+            no_cut = ''.join(set(params_dict['labels']) - set(no_cut))
+            return cut, no_cut
+
+    protease = cleavage_rule.replace('X', ''.join(params_dict['labels']))
+    c_term_rule, n_term_rule = protease.split('|')
+    sense = get_sense(c_term_rule, n_term_rule)
+    if sense == 'C':
+        cut, no_cut = get_cut(c_term_rule, n_term_rule)
+    else:
+        cut, no_cut = get_cut(n_term_rule, c_term_rule)
+    return {'sense': sense, 'cut': cut, 'no_cut': no_cut}
+
+
+def parse_mod_list(s, kind):
+    pairs = re.split(r'\s*[,;]\s*', s)
+    if kind == 'fixed':
+        out = {}
+    elif kind == 'variable':
+        out = []
+    else:
+        raise ValueError('`kind` must be "fixed" or "variable", not "{}".'.format(kind))
+
+    for p in pairs:
+        if p:
+            m, aa = re.split(r'\s*@\s*', p)
+            m = float(m)
+            if kind == 'fixed':
+                if aa == 'N-term':
+                    out['H-'] = 1.007825 + m
+                elif aa == 'C-term':
+                    out['-OH'] = 17.00274 + m
+                else:
+                    out[aa] = mass.std_aa_mass[aa] + m
+            else:
+                out.append((aa, m))
+    return out
```

### Comparing `AA_stat-2.5.4/AA_stat.egg-info/PKG-INFO` & `AA_stat-2.5.5/AA_stat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: AA-stat
-Version: 2.5.4
+Version: 2.5.5
 Summary: A utility for validation of peptide identification results in proteomics using amino acid counting.
-Home-page: UNKNOWN
 Author: Julia Bubis & Lev Levitsky
 Author-email: julia.bubis@gmail.com
 License: License :: OSI Approved :: Apache Software License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -123,30 +121,34 @@
 ```
 
 # User manual
 
 ### Command line options
 
 ```
-usage: AA_stat [-h] [--params PARAMS] [--dir DIR] [-v {0,1,2,3}] [--mgf MGF [MGF ...] | --mzml MZML [MZML ...]] (--pepxml PEPXML [PEPXML ...] | --csv CSV [CSV ...])
+usage: AA_stat [-h] [--params PARAMS] [--dir DIR] [-v {0,1,2,3}] [--mgf MGF [MGF ...] | --mzml MZML [MZML ...]] (--pepxml PEPXML [PEPXML ...] | --csv CSV [CSV ...]) [--fmods FMODS] [--vmods VMODS]
+               [--enzyme ENZYME] [-n PROCESSES]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --params PARAMS       CFG file with parameters. If there is no file, AA_stat uses default one. An example can be found at https://github.com/SimpleNumber/aa_stat
   --dir DIR             Directory to store the results. Default value is current directory.
   -v {0,1,2,3}, --verbosity {0,1,2,3}
                         Output verbosity.
   --mgf MGF [MGF ...]   MGF files to localize modifications.
   --mzml MZML [MZML ...]
                         mzML files to localize modifications.
   --pepxml PEPXML [PEPXML ...]
                         List of input files in pepXML format.
   --csv CSV [CSV ...]   List of input files in CSV format.
-
-Instead of file lists, you can pass directory names. This will process all files in the directory.
+  --fmods FMODS         Fixed modifications specified in the search (needed with CSV input). Example: +57.0215 @ C, +229.1630 @ N-term
+  --vmods VMODS         Variable modifications specified in the search (needed with CSV input). Example: 15.9959 @ M, 42.0106 @ N-term
+  --enzyme ENZYME       Enzyme specificity set in the search (needed with CSV input).
+  -n PROCESSES, --processes PROCESSES
+                        Maximum number of processes to use.
 ```
 
 
 ### Configuration file
 
 Configuration parameters can be set in a **config** file (default values and comments are in [default.cfg](AA_stat/default.cfg)).
 
@@ -210,14 +212,16 @@
 | try all localizations            | no                                       | If enabled, all localizations are possible. Otherwise, localization sites are determined based on occurrence frequencies and Unimod. |
 |                                  |**[modifications]**                       |                                                                            |
 | recommend variable modifications |          5                               | Number of modifications recommended for closed search.                     |
 | recommend multiple modifications on residue  | yes                          | Allows several modifications on one AA residue.                            |
 | fixed modification intensity threshold | 3                                  | Maximum % of peptides containing AA at zero shift to consider a fixed modification. |
 | isotope error abundance threshold | 10                                      | Minimum % of isotope error to justify recommendation of isotope error.     |
 | minimum localization count       | 10                                       | Minimum absolute localization count to recommend a variable modification.  |
+| configured fixed modifications  || for CSV input, specify here the fixed modifications used in your search. Example: `+57.0215 @ C, +229.1629 @ K, +229.1630 @ N-term`. |
+| configured variable modifications || for CSV input, specify here the variable modifications used in your search. Example: `15.9959 @ M, 42.0106 @ N-term`. |
 
 
 ### Output files
 
 An example of AA_stat output can be found [here](https://gorshkovlab.github.io/aa_stat_reports/).
 
 AA_stat produces the following files:
@@ -303,15 +307,15 @@
 |localization| Localization statistics for given mass shift using MS/MS spectra provided in a format "AminoAcid_MassShift:number-of-peptides-with-this-localization". If there is no clear leader for a specific peptide's mass shift localization, it counts as 'non-localized'.
 
 
 ### AA_search option
 
 If AA_stat used in "AA_search" mode, MSFragger is run prior to AA_stat. AA_search can also optimize fixed modifications
 that are used for open search, and repeat open search if needed. This is enabled with `-x` option (or `--optimize-fixed-mods`).
-Full list of supported comman-line options:
+Full list of supported command-line options:
 
 ```
 AA_search [-h] [--params PARAMS] [--MSFragger MSFRAGGER] [--dir DIR] [-v {0,1,2,3}] (--mgf MGF [MGF ...] | --mzml MZML [MZML ...]) [-db FASTA] [--os-params OS_PARAMS] [-x] [-s [SKIP]] [-je JAVA_EXECUTABLE] [-ja JAVA_ARGS]
 
 optional arguments:
   -h, --help            show this help message and exit
   --params PARAMS       CFG file with parameters. If there is no file, AA_stat uses default one. An example can be found at https://github.com/SimpleNumber/aa_stat
@@ -341,9 +345,7 @@
 
 ```
 AA_search --MSFragger /path/to/MSFragger/MSFragger-2.4.jar -x -db fasta_file.fasta --mzml mzml_files.mzML --dir ./save_dir
 ```
 
 All searches are saved in separate folders: "step 1", "step 2", etc.
 In these folders, pepXML files and open search parameters file (os.params) are saved, together with AA_stat results.
-
-
```

### Comparing `AA_stat-2.5.4/AA_stat.egg-info/SOURCES.txt` & `AA_stat-2.5.5/AA_stat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/LICENSE` & `AA_stat-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AA_stat-2.5.4/PKG-INFO` & `AA_stat-2.5.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: AA_stat
-Version: 2.5.4
+Version: 2.5.5
 Summary: A utility for validation of peptide identification results in proteomics using amino acid counting.
-Home-page: UNKNOWN
 Author: Julia Bubis & Lev Levitsky
 Author-email: julia.bubis@gmail.com
 License: License :: OSI Approved :: Apache Software License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -123,30 +121,34 @@
 ```
 
 # User manual
 
 ### Command line options
 
 ```
-usage: AA_stat [-h] [--params PARAMS] [--dir DIR] [-v {0,1,2,3}] [--mgf MGF [MGF ...] | --mzml MZML [MZML ...]] (--pepxml PEPXML [PEPXML ...] | --csv CSV [CSV ...])
+usage: AA_stat [-h] [--params PARAMS] [--dir DIR] [-v {0,1,2,3}] [--mgf MGF [MGF ...] | --mzml MZML [MZML ...]] (--pepxml PEPXML [PEPXML ...] | --csv CSV [CSV ...]) [--fmods FMODS] [--vmods VMODS]
+               [--enzyme ENZYME] [-n PROCESSES]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --params PARAMS       CFG file with parameters. If there is no file, AA_stat uses default one. An example can be found at https://github.com/SimpleNumber/aa_stat
   --dir DIR             Directory to store the results. Default value is current directory.
   -v {0,1,2,3}, --verbosity {0,1,2,3}
                         Output verbosity.
   --mgf MGF [MGF ...]   MGF files to localize modifications.
   --mzml MZML [MZML ...]
                         mzML files to localize modifications.
   --pepxml PEPXML [PEPXML ...]
                         List of input files in pepXML format.
   --csv CSV [CSV ...]   List of input files in CSV format.
-
-Instead of file lists, you can pass directory names. This will process all files in the directory.
+  --fmods FMODS         Fixed modifications specified in the search (needed with CSV input). Example: +57.0215 @ C, +229.1630 @ N-term
+  --vmods VMODS         Variable modifications specified in the search (needed with CSV input). Example: 15.9959 @ M, 42.0106 @ N-term
+  --enzyme ENZYME       Enzyme specificity set in the search (needed with CSV input).
+  -n PROCESSES, --processes PROCESSES
+                        Maximum number of processes to use.
 ```
 
 
 ### Configuration file
 
 Configuration parameters can be set in a **config** file (default values and comments are in [default.cfg](AA_stat/default.cfg)).
 
@@ -210,14 +212,16 @@
 | try all localizations            | no                                       | If enabled, all localizations are possible. Otherwise, localization sites are determined based on occurrence frequencies and Unimod. |
 |                                  |**[modifications]**                       |                                                                            |
 | recommend variable modifications |          5                               | Number of modifications recommended for closed search.                     |
 | recommend multiple modifications on residue  | yes                          | Allows several modifications on one AA residue.                            |
 | fixed modification intensity threshold | 3                                  | Maximum % of peptides containing AA at zero shift to consider a fixed modification. |
 | isotope error abundance threshold | 10                                      | Minimum % of isotope error to justify recommendation of isotope error.     |
 | minimum localization count       | 10                                       | Minimum absolute localization count to recommend a variable modification.  |
+| configured fixed modifications  || for CSV input, specify here the fixed modifications used in your search. Example: `+57.0215 @ C, +229.1629 @ K, +229.1630 @ N-term`. |
+| configured variable modifications || for CSV input, specify here the variable modifications used in your search. Example: `15.9959 @ M, 42.0106 @ N-term`. |
 
 
 ### Output files
 
 An example of AA_stat output can be found [here](https://gorshkovlab.github.io/aa_stat_reports/).
 
 AA_stat produces the following files:
@@ -303,15 +307,15 @@
 |localization| Localization statistics for given mass shift using MS/MS spectra provided in a format "AminoAcid_MassShift:number-of-peptides-with-this-localization". If there is no clear leader for a specific peptide's mass shift localization, it counts as 'non-localized'.
 
 
 ### AA_search option
 
 If AA_stat used in "AA_search" mode, MSFragger is run prior to AA_stat. AA_search can also optimize fixed modifications
 that are used for open search, and repeat open search if needed. This is enabled with `-x` option (or `--optimize-fixed-mods`).
-Full list of supported comman-line options:
+Full list of supported command-line options:
 
 ```
 AA_search [-h] [--params PARAMS] [--MSFragger MSFRAGGER] [--dir DIR] [-v {0,1,2,3}] (--mgf MGF [MGF ...] | --mzml MZML [MZML ...]) [-db FASTA] [--os-params OS_PARAMS] [-x] [-s [SKIP]] [-je JAVA_EXECUTABLE] [-ja JAVA_ARGS]
 
 optional arguments:
   -h, --help            show this help message and exit
   --params PARAMS       CFG file with parameters. If there is no file, AA_stat uses default one. An example can be found at https://github.com/SimpleNumber/aa_stat
@@ -341,9 +345,7 @@
 
 ```
 AA_search --MSFragger /path/to/MSFragger/MSFragger-2.4.jar -x -db fasta_file.fasta --mzml mzml_files.mzML --dir ./save_dir
 ```
 
 All searches are saved in separate folders: "step 1", "step 2", etc.
 In these folders, pepXML files and open search parameters file (os.params) are saved, together with AA_stat results.
-
-
```

### Comparing `AA_stat-2.5.4/setup.py` & `AA_stat-2.5.5/setup.py`

 * *Files identical despite different names*

