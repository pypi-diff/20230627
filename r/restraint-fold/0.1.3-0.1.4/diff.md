# Comparing `tmp/restraint-fold-0.1.3.tar.gz` & `tmp/restraint-fold-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restraint-fold-0.1.3.tar", last modified: Sun Jun 25 01:27:25 2023, max compression
+gzip compressed data, was "restraint-fold-0.1.4.tar", last modified: Tue Jun 27 02:36:02 2023, max compression
```

## Comparing `restraint-fold-0.1.3.tar` & `restraint-fold-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1.3/LICENSE
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     4223 2023-06-25 01:23:12.000000 restraint-fold-0.1.3/README.md
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.878167 restraint-fold-0.1.3/fold/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     9540 2023-06-21 09:14:03.000000 restraint-fold-0.1.3/fold/__init__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     4074 2023-06-25 01:21:08.000000 restraint-fold-0.1.3/fold/__main__.py
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.878167 restraint-fold-0.1.3/restraint_fold.egg-info/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      249 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/SOURCES.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/dependency_links.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       18 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/requires.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/top_level.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/setup.cfg
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1984 2023-06-21 09:11:45.000000 restraint-fold-0.1.3/setup.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-27 02:36:02.409347 restraint-fold-0.1.4/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1.4/LICENSE
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-27 02:36:02.409347 restraint-fold-0.1.4/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4223 2023-06-25 01:23:12.000000 restraint-fold-0.1.4/README.md
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-27 02:36:02.409347 restraint-fold-0.1.4/fold/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    11790 2023-06-27 02:17:35.000000 restraint-fold-0.1.4/fold/__init__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4089 2023-06-27 02:30:14.000000 restraint-fold-0.1.4/fold/__main__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    19491 2023-06-26 08:37:48.000000 restraint-fold-0.1.4/fold/constants.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-27 02:36:02.409347 restraint-fold-0.1.4/restraint_fold.egg-info/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-27 02:36:02.000000 restraint-fold-0.1.4/restraint_fold.egg-info/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      267 2023-06-27 02:36:02.000000 restraint-fold-0.1.4/restraint_fold.egg-info/SOURCES.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-27 02:36:02.000000 restraint-fold-0.1.4/restraint_fold.egg-info/dependency_links.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       18 2023-06-27 02:36:02.000000 restraint-fold-0.1.4/restraint_fold.egg-info/requires.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-27 02:36:02.000000 restraint-fold-0.1.4/restraint_fold.egg-info/top_level.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-27 02:36:02.409347 restraint-fold-0.1.4/setup.cfg
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1984 2023-06-26 07:11:49.000000 restraint-fold-0.1.4/setup.py
```

### Comparing `restraint-fold-0.1.3/LICENSE` & `restraint-fold-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `restraint-fold-0.1.3/PKG-INFO` & `restraint-fold-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restraint-fold
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple Protein Structure Parser
 Home-page: https://gitee.com/dechin/restraint-fold/
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `restraint-fold-0.1.3/README.md` & `restraint-fold-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `restraint-fold-0.1.3/fold/__init__.py` & `restraint-fold-0.1.4/fold/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 import sys
 sys.setrecursionlimit(90000000)
 
 import numpy as np
 from tqdm import trange
 from hadder.parsers import read_pdb
-from hadder.constants import hnames
+from .constants import h_names, h_keys
 
-def get_hbonds(pdb_name, hbond_length=3.5, return_hbonds=False):
+def get_hbonds(pdb_name, hbond_length=3.5, return_hbonds=False, base_hlength=1.2):
     res = read_pdb(pdb_name)
     atom_names = res[5]
     group_names = res[0]
     crds = res[6]
     res_names = res[7]
     res_ids = res[8]
     n_index = []
@@ -52,15 +52,15 @@
     h_index = np.array(h_index, np.int32)
 
     n_crd = crds[n_index]
     o_crd = crds[o_index]
     h_crd = crds[h_index]
     
     dis_oh = np.linalg.norm(o_crd - h_crd[:, None, :], axis=-1)
-    mask_oh = np.where(dis_oh <= hbond_length)
+    mask_oh = np.where((dis_oh <= hbond_length) & (dis_oh >= base_hlength))
     mh_index_o = mask_oh[0]
     mo_index = mask_oh[1]
     xh_index_o = []
     for idx in mh_index_o:
         h_idx = h_index[idx]
         res_name = res_names[h_idx]
         res_id = res_ids[h_idx]
@@ -70,26 +70,23 @@
             pass
         elif res_id == 1:
             res_name = 'N' + res_name
         elif res_id == max(res_ids):
             res_name = 'C' + res_name
         else:
             pass
-        res_dict = hnames[res_name]
-        for key in res_dict:
-            if atom_names[h_idx] not in res_dict[key]:
-                continue
-            for cbk in range(50):
-                if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
-                    xh_index_o.append(h_idx - cbk - 1)
-                    break
+        key = h_keys[res_name][atom_names[h_idx]]
+        for cbk in range(50):
+            if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
+                xh_index_o.append(h_idx - cbk - 1)
+                break
     xh_index_o = np.array(xh_index_o, np.int32)
 
     dis_nh = np.linalg.norm(n_crd - h_crd[:, None, :], axis=-1)
-    mask_nh = np.where(dis_nh <= hbond_length)
+    mask_nh = np.where((dis_nh <= hbond_length) & (dis_nh >= base_hlength))
     mh_index_n = mask_nh[0]
     mn_index = mask_nh[1]
     xh_index_n = []
 
     for idx in mh_index_n:
         h_idx = h_index[idx]
         res_name = res_names[h_idx]
@@ -100,36 +97,33 @@
             pass
         elif res_id == 1:
             res_name = 'N' + res_name
         elif res_id == max(res_ids):
             res_name = 'C' + res_name
         else:
             pass
-        res_dict = hnames[res_name]
-        for key in res_dict:
-            if atom_names[h_idx] not in res_dict[key]:
-                continue
-            for cbk in range(50):
-                if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
-                    xh_index_n.append(h_idx - cbk - 1)
-                    break
+        key = h_keys[res_name][atom_names[h_idx]]
+        for cbk in range(50):
+            if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
+                xh_index_n.append(h_idx - cbk - 1)
+                break
     xh_index_n = np.array(xh_index_n, np.int32)
 
     hbonds = []
     res_bonds = []
     for i, idx in enumerate(mo_index):
         if res_ids[o_index[idx]] == res_ids[h_index[mh_index_o[i]]]:
             continue
-        hbonds.append([xh_index_o[mh_index_o[i]], h_index[mh_index_o[i]], o_index[idx]])
+        hbonds.append([xh_index_o[i], h_index[mh_index_o[i]], o_index[idx]])
         res_bonds.append([res_ids[o_index[idx]], res_ids[h_index[mh_index_o[i]]]])
 
     for i, idx in enumerate(mn_index):
         if res_ids[n_index[idx]] == res_ids[h_index[mh_index_n[i]]]:
             continue
-        hbonds.append([xh_index_n[mh_index_n[i]], h_index[mh_index_n[i]], n_index[idx]])
+        hbonds.append([xh_index_n[i], h_index[mh_index_n[i]], n_index[idx]])
         res_bonds.append([res_ids[n_index[idx]], res_ids[h_index[mh_index_n[i]]]])
 
     hbonds = np.array(hbonds, np.int32)
     res_bonds = np.array(res_bonds, np.int32)
 
     xy_vector = crds[hbonds[:, 2]] - crds[hbonds[:, 1]]
     xy = np.linalg.norm(xy_vector, axis=-1)
@@ -178,45 +172,49 @@
         #     counter += 1
         #     continue
         elif counter < min_alpha:
             counter = 0
             continue
         else:
             alpha.extend([index])
-            alpha.extend([index - 1 - i for i in range(counter)])
+            alpha.extend([index + 1])
+            alpha.extend([index - i - 1 for i in range(counter)])
             counter = 0
             continue
     alpha = np.sort(np.array(alpha, np.int32))
     return alpha
 
 tmp_beta = []
+min_res_for_beta = 4
 beta = []
 counter = 0
 counter_1 = 0
+counter_2 = 0
+counter_3 = 0
 
 def _get_beta(res_bonds, start, end):
     global beta
     global counter
     global tmp_beta
     pair = np.array([start-1, end+1])
     if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
         if start-1 not in tmp_beta:
             tmp_beta.extend([start-1])
         if end+1 not in tmp_beta:
             tmp_beta.extend([end+1])
         counter += 1
         return _get_beta(res_bonds, start-1, end+1)
-    elif counter > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
-        if start-2 not in tmp_beta:
-            tmp_beta.extend([start-2])
-        if end+2 not in tmp_beta:
-            tmp_beta.extend([end+2])
-        counter += 1
+    # elif counter > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+    #     if start-2 not in tmp_beta:
+    #         tmp_beta.extend([start-2])
+    #     if end+2 not in tmp_beta:
+    #         tmp_beta.extend([end+2])
+    #     counter += 1
     else:
-        if counter > 4:
+        if counter >= min_res_for_beta:
             beta.extend(tmp_beta)
         counter = 1
         tmp_beta = []
         return 0
 
 def _get_beta_1(res_bonds, start, end):
     global beta
@@ -225,45 +223,107 @@
     pair = np.array([start+1, end+1])
     if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
         if start-1 not in tmp_beta:
             tmp_beta.extend([start+1])
         if end+1 not in tmp_beta:
             tmp_beta.extend([end+1])
         counter_1 += 1
-        return _get_beta(res_bonds, start+1, end+1)
-    elif counter_1 > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
-        if start-2 not in tmp_beta:
-            tmp_beta.extend([start+2])
-        if end+2 not in tmp_beta:
-            tmp_beta.extend([end+2])
-        counter_1 += 1
+        return _get_beta_1(res_bonds, start+1, end+1)
+    # elif counter_1 > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+    #     if start-2 not in tmp_beta:
+    #         tmp_beta.extend([start+2])
+    #     if end+2 not in tmp_beta:
+    #         tmp_beta.extend([end+2])
+    #     counter_1 += 1
     else:
-        if counter_1 > 4:
+        if counter_1 >= min_res_for_beta:
             beta.extend(tmp_beta)
         counter_1 = 1
         tmp_beta = []
         return 0
 
-def get_beta(pdb_name, hbond_length=3.5):
+def _get_beta_2(res_bonds, start, end):
+    global beta
+    global counter_2
+    global tmp_beta
+    pair = np.array([start-1, end-1])
+    if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+        if start-1 not in tmp_beta:
+            tmp_beta.extend([start-1])
+        if end+1 not in tmp_beta:
+            tmp_beta.extend([end-1])
+        counter_2 += 1
+        return _get_beta_2(res_bonds, start-1, end-1)
+    # elif counter_2 > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+    #     if start-2 not in tmp_beta:
+    #         tmp_beta.extend([start-2])
+    #     if end+2 not in tmp_beta:
+    #         tmp_beta.extend([end+2])
+    #     counter_2 += 1
+    else:
+        if counter_2 >= min_res_for_beta:
+            beta.extend(tmp_beta)
+        counter_2 = 1
+        tmp_beta = []
+        return 0
+
+def _get_beta_3(res_bonds, start, end):
+    global beta
+    global counter_3
+    global tmp_beta
+    pair = np.array([start+1, end-1])
+    if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+        if start+1 not in tmp_beta:
+            tmp_beta.extend([start+1])
+        if end-1 not in tmp_beta:
+            tmp_beta.extend([end-1])
+        counter_3 += 1
+        return _get_beta(res_bonds, start+1, end-1)
+    # elif counter_3 > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+    #     if start+2 not in tmp_beta:
+    #         tmp_beta.extend([start+2])
+    #     if end-2 not in tmp_beta:
+    #         tmp_beta.extend([end-2])
+    #     counter_3 += 1
+    else:
+        if counter_3 >= min_res_for_beta:
+            beta.extend(tmp_beta)
+        counter_3 = 1
+        tmp_beta = []
+        return 0
+
+def get_beta(pdb_name, hbond_length=3.5, alphas=None):
     res_bonds = get_hbonds(pdb_name, hbond_length=hbond_length)
+    if alphas is not None:
+        alpha_mask = np.isin(res_bonds, alphas)
+        alpha_index = np.where(alpha_mask.sum(axis=-1)>0)
+        res_bonds = np.delete(res_bonds, alpha_index, axis=0)
     global tmp_beta
     global beta
     print ('Analysing beta:')
     for index in trange(len(res_bonds)):
         bond = res_bonds[index]
         start = bond[0]
         end = bond[1]
         pair = np.array([start-1, end+1])
         pair_1 = np.array([start+1, end+1])
+        pair_2 = np.array([start - 1, end - 1])
+        pair_3 = np.array([start + 1, end - 1])
         if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
             tmp_beta.extend([start, end])
             _ = _get_beta(res_bonds, start, end)
         elif np.sum(np.isin(res_bonds, pair_1).sum(axis=-1)==2)>0:
             tmp_beta.extend([start, end])
             _ = _get_beta_1(res_bonds, start, end)
+        elif np.sum(np.isin(res_bonds, pair_2).sum(axis=-1)==2)>0:
+            tmp_beta.extend([start, end])
+            _ = _get_beta_2(res_bonds, start, end)
+        elif np.sum(np.isin(res_bonds, pair_3).sum(axis=-1)==2)>0:
+            tmp_beta.extend([start, end])
+            _ = _get_beta_2(res_bonds, start, end)
         else:
             continue
     beta = np.array(beta, np.int32)
     beta = np.unique(beta)
     beta = np.sort(beta)
     return beta
```

### Comparing `restraint-fold-0.1.3/fold/__main__.py` & `restraint-fold-0.1.4/fold/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 if addh == '1':
     AddHydrogen(pdb_name, addh_pdb)
     print ('The new pdb file path is in: {}'.format(addh_pdb))
     pdb_name = addh_pdb
 
 alphas = get_alpha(pdb_name, hbond_length=3.5)
-betas = get_beta(pdb_name, hbond_length=3.5)
+betas = get_beta(pdb_name, hbond_length=4.0, alphas=alphas)
 
 if save_txt_name is not None:
     if use_simplified == '0':
         with open(save_txt_name, 'w') as file:
             file.write('alpha:\n')
             file.write(' '.join(list(map(str,alphas))))
             file.write('\n')
```

### Comparing `restraint-fold-0.1.3/restraint_fold.egg-info/PKG-INFO` & `restraint-fold-0.1.4/restraint_fold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restraint-fold
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple Protein Structure Parser
 Home-page: https://gitee.com/dechin/restraint-fold/
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `restraint-fold-0.1.3/setup.py` & `restraint-fold-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="restraint-fold",
-    version="0.1.3",
+    version="0.1.4",
     description="Simple Protein Structure Parser",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT License",
 
     url="https://gitee.com/dechin/restraint-fold/",
     author="Dechin CHEN",
```

