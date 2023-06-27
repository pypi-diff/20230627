# Comparing `tmp/scHPL-1.0.2.tar.gz` & `tmp/scHPL-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scHPL-1.0.2.tar", last modified: Thu Nov 17 07:36:05 2022, max compression
+gzip compressed data, was "scHPL-1.0.3.tar", last modified: Wed May  3 07:43:32 2023, max compression
```

## Comparing `scHPL-1.0.2.tar` & `scHPL-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2022-11-17 07:36:05.900133 scHPL-1.0.2/
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1091 2021-01-06 08:23:05.000000 scHPL-1.0.2/LICENSE
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     2090 2022-11-17 07:36:05.898419 scHPL-1.0.2/PKG-INFO
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1583 2021-07-09 14:18:28.000000 scHPL-1.0.2/README.md
-drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2022-11-17 07:36:05.859650 scHPL-1.0.2/scHPL/
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      437 2022-05-12 06:35:02.000000 scHPL-1.0.2/scHPL/__init__.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     6186 2022-06-17 05:51:13.000000 scHPL-1.0.2/scHPL/evaluate.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1220 2022-05-12 06:35:02.000000 scHPL-1.0.2/scHPL/faissKNeighbors.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     6474 2022-05-12 06:35:02.000000 scHPL-1.0.2/scHPL/learn.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     5010 2022-11-16 15:53:15.000000 scHPL-1.0.2/scHPL/predict.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    11324 2022-05-12 06:35:03.000000 scHPL-1.0.2/scHPL/train.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    25916 2022-05-12 06:35:03.000000 scHPL-1.0.2/scHPL/update.py
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    12105 2022-05-12 06:35:03.000000 scHPL-1.0.2/scHPL/utils.py
-drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2022-11-17 07:36:05.891661 scHPL-1.0.2/scHPL.egg-info/
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     2090 2022-11-17 07:36:05.000000 scHPL-1.0.2/scHPL.egg-info/PKG-INFO
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      309 2022-11-17 07:36:05.000000 scHPL-1.0.2/scHPL.egg-info/SOURCES.txt
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        1 2022-11-17 07:36:05.000000 scHPL-1.0.2/scHPL.egg-info/dependency_links.txt
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      125 2022-11-17 07:36:05.000000 scHPL-1.0.2/scHPL.egg-info/requires.txt
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        6 2022-11-17 07:36:05.000000 scHPL-1.0.2/scHPL.egg-info/top_level.txt
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)       38 2022-11-17 07:36:05.901441 scHPL-1.0.2/setup.cfg
--rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1177 2022-11-17 07:35:56.000000 scHPL-1.0.2/setup.py
+drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2023-05-03 07:43:32.707669 scHPL-1.0.3/
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1091 2021-01-06 08:23:05.000000 scHPL-1.0.3/LICENSE
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     2090 2023-05-03 07:43:32.705776 scHPL-1.0.3/PKG-INFO
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1583 2021-07-09 14:18:28.000000 scHPL-1.0.3/README.md
+drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2023-05-03 07:43:32.621070 scHPL-1.0.3/scHPL/
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      437 2022-04-14 12:50:33.000000 scHPL-1.0.3/scHPL/__init__.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     6186 2022-06-17 05:51:13.000000 scHPL-1.0.3/scHPL/evaluate.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1220 2022-05-12 06:35:02.000000 scHPL-1.0.3/scHPL/faissKNeighbors.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     6878 2023-05-03 06:59:43.000000 scHPL-1.0.3/scHPL/learn.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     5010 2022-11-16 15:53:15.000000 scHPL-1.0.3/scHPL/predict.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    11745 2023-05-03 06:58:18.000000 scHPL-1.0.3/scHPL/train.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    25916 2022-05-12 06:35:03.000000 scHPL-1.0.3/scHPL/update.py
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)    12105 2022-05-12 06:35:03.000000 scHPL-1.0.3/scHPL/utils.py
+drwxr-xr-x   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        0 2023-05-03 07:43:32.664179 scHPL-1.0.3/scHPL.egg-info/
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     2090 2023-05-03 07:43:32.000000 scHPL-1.0.3/scHPL.egg-info/PKG-INFO
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      309 2023-05-03 07:43:32.000000 scHPL-1.0.3/scHPL.egg-info/SOURCES.txt
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        1 2023-05-03 07:43:32.000000 scHPL-1.0.3/scHPL.egg-info/dependency_links.txt
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)      125 2023-05-03 07:43:32.000000 scHPL-1.0.3/scHPL.egg-info/requires.txt
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)        6 2023-05-03 07:43:32.000000 scHPL-1.0.3/scHPL.egg-info/top_level.txt
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)       38 2023-05-03 07:43:32.708583 scHPL-1.0.3/setup.cfg
+-rw-r--r--   0 lcmmichielsen (208942) 5-A-SHARK_hg_bioinf (100980)     1177 2023-05-03 07:39:11.000000 scHPL-1.0.3/setup.py
```

### Comparing `scHPL-1.0.2/LICENSE` & `scHPL-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/PKG-INFO` & `scHPL-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scHPL
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hierarchical progressive learning pipeline for single-cell RNA-sequencing datasets
 Home-page: https://github.com/lcmmichielsen/hierarchicalprogressivelearning
 Author: Lieke Michielsen
 Author-email: l.c.m.michielsen@tudelft.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scHPL-1.0.2/README.md` & `scHPL-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL/evaluate.py` & `scHPL-1.0.3/scHPL/evaluate.py`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL/faissKNeighbors.py` & `scHPL-1.0.3/scHPL/faissKNeighbors.py`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL/learn.py` & `scHPL-1.0.3/scHPL/learn.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                cell_type_key: str,
                tree: TreeNode = None,
                retrain: bool = False,
                batch_added: list = None,
                classifier: Literal['knn','svm','svm_occ'] = 'knn',
                n_neighbors: int = 50,
                dynamic_neighbors: bool = True,
+               distkNN: int = 99,
                dimred: bool = False,
                useRE: bool = True,
                FN: float = 0.5,               
                rej_threshold: float = 0.5,
                match_threshold: float = 0.25,
                attach_missing: bool = False,
                print_conf: bool = False
@@ -63,14 +64,19 @@
         n_neighbors: int = 50
             Number of neighbors for the kNN classifier (only used when 
             classifier='knn').
         dynamic_neighbors: bool = True
             Number of neighbors for the kNN classifier can change when a node 
             contains a very small cell population. k is set to 
             min(n_neighbors, smallest-cell-population)
+        distkNN: int = 99
+            Used to determine the threshold for the maximum distance between a 
+            cell and it's closest neighbor of the training set. Threshold is 
+            set to the distkNN's percentile of distances within the training
+            set
         dimred: Boolean = False
             If 'True', PCA is applied before training the classifier.
         useRE: Boolean = True
             If 'True', cells are also rejected based on the reconstruction error.
         FN: Float = 0.5
             Percentage of false negatives allowed when determining the threshold
             for the reconstruction error.
@@ -122,20 +128,22 @@
         labels_2 = labels[idx_2]
         tree_2 = create_tree('root2')
         tree_2 = _construct_tree(tree_2, labels_2)
                 
         # Train the trees
         if retrain:
             tree = train_tree(data_1, labels_1, tree, classifier, 
-                              dimred, useRE, FN, n_neighbors, dynamic_neighbors)
+                              dimred, useRE, FN, n_neighbors, dynamic_neighbors,
+                              distkNN)
         else:
             retrain = True 
         
         tree_2 = train_tree(data_2, labels_2, tree_2, classifier, 
-                            dimred, useRE, FN, n_neighbors, dynamic_neighbors)
+                            dimred, useRE, FN, n_neighbors, dynamic_neighbors,
+                            distkNN)
         
         # Predict labels other dataset
         labels_2_pred = predict_labels(data_2, tree, threshold=rej_threshold)
         labels_1_pred = predict_labels(data_1, tree_2, threshold=rej_threshold)
         
         # Update first tree and labels second dataset
         tree, mis_pop = update_tree(tree, labels_1.reshape(-1,1),
@@ -154,15 +162,15 @@
         #concatenate the two datasets
         data_1 = np.concatenate((data_1, data_2), axis = 0)
         labels_1 = np.concatenate((np.squeeze(labels_1), np.squeeze(labels_2)), 
                                 axis = 0)
     
     # Train the final tree
     tree = train_tree(data_1, labels_1, tree, classifier, dimred, useRE, FN,
-                      n_neighbors, dynamic_neighbors)
+                      n_neighbors, dynamic_neighbors, distkNN)
     
     return tree, missing_pop
     
     
 
 def _construct_tree(tree, labels):
     '''
```

### Comparing `scHPL-1.0.2/scHPL/predict.py` & `scHPL-1.0.3/scHPL/predict.py`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL/train.py` & `scHPL-1.0.3/scHPL/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
                labels, 
                tree: TreeNode, 
                classifier: Literal['knn','svm','svm_occ'] = 'knn', 
                dimred: bool = False, 
                useRE: bool = True, 
                FN: float = 0.5, 
                n_neighbors: int = 50,
-               dynamic_neighbors: bool = True):
+               dynamic_neighbors: bool = True,
+               distkNN: int = 99):
     '''Train a hierarchical classifier. 
     
         Parameters
         ----------
         data: array_like 
             Training data (cells x genes)
         labels: array_like
@@ -55,14 +56,19 @@
         n_neighbors: int = 50
             Number of neighbors for the kNN classifier (only used when 
             classifier='knn').
         dynamic_neighbors: bool = True
             Number of neighbors for the kNN classifier can change when a node 
             contains a very small cell population. k is set to 
             min(n_neighbors, smallest-cell-population)
+        distkNN: int = 99
+            Used to determine the threshold for the maximum distance between a 
+            cell and it's closest neighbor of the training set. Threshold is 
+            set to the distkNN's percentile of distances within the training
+            set
 
         
         Returns
         -------
         Trained classification tree
     '''
     
@@ -118,15 +124,15 @@
     if(classifier == 'knn'):
         labels_train = cp.deepcopy(labels)
         try: 
             labels_train = labels_train.values
         except:
             None
         _,_ = _train_parentnode(data, labels_train, tree[0], n_neighbors, 
-                                dynamic_neighbors)
+                                dynamic_neighbors, distkNN)
     else:
         for n in tree[0].descendants:
             _ = _train_node(data, labels, n, classifier, dimred, numgenes)
 
     return tree
 
 
@@ -164,15 +170,15 @@
     if(classifier == 'svm'):
         _train_svm(data, labels, group, n)
     else:
         _train_occ(data, labels, group, n)
         
     return group
 
-def _train_parentnode(data, labels, n, n_neighbors, dynamic_neighbors):
+def _train_parentnode(data, labels, n, n_neighbors, dynamic_neighbors, distkNN):
     '''Train a knn classifier. In contrast to the linear svm and oc svm, this 
         is trained for each parent node instead of each child node
         
         Parameters
         ----------
         data: training data
         labels: labels of the training data
@@ -191,23 +197,24 @@
     if n.is_leaf:
         group[np.squeeze(np.isin(labels, n.name))] = 1
         labels[np.squeeze(np.isin(labels, n.name))] = n.name[0]
         return group, labels
     else:
         for j in n.descendants:
             group_new, labels_new = _train_parentnode(data, labels, j, 
-                                                      n_neighbors, dynamic_neighbors)
+                                                      n_neighbors, dynamic_neighbors,
+                                                      distkNN)
             group[np.where(group_new == 1)[0]] = 1
             labels[np.where(group_new == 1)[0]] = labels_new[np.where(group_new == 1)[0]]
         if n.name != None:
             # special case; if n has only 1 child
             if len(n.descendants) == 1:
                 group[np.squeeze(np.isin(labels, n.name))] = 1
             # train_knn 
-            _train_knn(data,labels,group,n,n_neighbors,dynamic_neighbors)
+            _train_knn(data,labels,group,n,n_neighbors,dynamic_neighbors,distkNN)
             # rename all group == 1 to node.name
             group[np.squeeze(np.isin(labels, n.name))] = 1
             labels[group==1] = n.name[0]
                     
     return group, labels
 
 
@@ -259,15 +266,15 @@
     group_svm = group[idx_svm]
     
     clf = svm.LinearSVC(random_state=1).fit(data_svm, group_svm)
     
     n.set_classifier(clf) #save classifier to the node
     
 
-def _train_knn(data, labels, group, n, n_neighbors, dynamic_neighbors):
+def _train_knn(data, labels, group, n, n_neighbors, dynamic_neighbors, distkNN):
     '''Train a linear svm and attach to the node
     
         Parameters:
         -----------
         data: training data
         group: indicating which cells of the training data belong to that node
         n: node
@@ -300,15 +307,15 @@
         #print('Using KNN')
         clf = KNN(weights='distance',
                   n_neighbors=k,
                   metric='euclidean').fit(data_knn, labels_knn)
     
     if((n.name[0] == 'root') | (n.name[0] == 'root2')):
         dist,idx = clf.kneighbors(data, return_distance=True)
-        n.set_maxDist(np.percentile(np.mean(dist[:,1:],axis=1),99))
+        n.set_maxDist(np.percentile(np.mean(dist[:,1:],axis=1),distkNN))
     
     n.set_classifier(clf) #save classifier to the node
 
         
 
 def _train_occ(data, labels, group, n):
     '''Train a one-class-classifier SVM and attach to the node
```

### Comparing `scHPL-1.0.2/scHPL/update.py` & `scHPL-1.0.3/scHPL/update.py`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL/utils.py` & `scHPL-1.0.3/scHPL/utils.py`

 * *Files identical despite different names*

### Comparing `scHPL-1.0.2/scHPL.egg-info/PKG-INFO` & `scHPL-1.0.3/scHPL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scHPL
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hierarchical progressive learning pipeline for single-cell RNA-sequencing datasets
 Home-page: https://github.com/lcmmichielsen/hierarchicalprogressivelearning
 Author: Lieke Michielsen
 Author-email: l.c.m.michielsen@tudelft.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scHPL-1.0.2/setup.py` & `scHPL-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scHPL", 
-    version="1.0.2",
+    version="1.0.3",
     author="Lieke Michielsen",
     author_email="l.c.m.michielsen@tudelft.nl",
     description="Hierarchical progressive learning pipeline for single-cell RNA-sequencing datasets",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lcmmichielsen/hierarchicalprogressivelearning",
```

