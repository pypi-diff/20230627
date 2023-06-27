# Comparing `tmp/spectralnet-0.0.2.tar.gz` & `tmp/spectralnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.2.tar", last modified: Tue Jun 27 10:45:19 2023, max compression
+gzip compressed data, was "spectralnet-0.0.3.tar", last modified: Tue Jun 27 12:06:39 2023, max compression
```

## Comparing `spectralnet-0.0.2.tar` & `spectralnet-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.996915 spectralnet-0.0.2/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-25 12:12:14.000000 spectralnet-0.0.2/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)      806 2023-06-27 10:45:19.997006 spectralnet-0.0.2/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      308 2023-06-27 10:18:33.000000 spectralnet-0.0.2/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-27 10:10:06.000000 spectralnet-0.0.2/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-27 10:45:19.997274 spectralnet-0.0.2/setup.cfg
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.989452 spectralnet-0.0.2/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.991772 spectralnet-0.0.2/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      114 2023-06-27 09:56:19.000000 spectralnet-0.0.2/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.993461 spectralnet-0.0.2/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-25 13:45:07.000000 spectralnet-0.0.2/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-25 17:02:04.000000 spectralnet-0.0.2/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-25 13:27:35.000000 spectralnet-0.0.2/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-25 17:05:52.000000 spectralnet-0.0.2/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.994991 spectralnet-0.0.2/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-25 13:44:44.000000 spectralnet-0.0.2/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-27 09:25:21.000000 spectralnet-0.0.2/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-25 17:56:01.000000 spectralnet-0.0.2/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2897 2023-06-25 18:01:13.000000 spectralnet-0.0.2/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-26 12:24:44.000000 spectralnet-0.0.2/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.996582 spectralnet-0.0.2/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-25 17:49:01.000000 spectralnet-0.0.2/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3733 2023-06-25 18:43:37.000000 spectralnet-0.0.2/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9437 2023-06-25 18:58:20.000000 spectralnet-0.0.2/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7972 2023-06-26 12:27:24.000000 spectralnet-0.0.2/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-25 17:43:03.000000 spectralnet-0.0.2/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-25 17:04:22.000000 spectralnet-0.0.2/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 10:45:19.992592 spectralnet-0.0.2/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)      806 2023-06-27 10:45:19.000000 spectralnet-0.0.2/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      814 2023-06-27 10:45:19.000000 spectralnet-0.0.2/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-27 10:45:19.000000 spectralnet-0.0.2/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       12 2023-06-27 10:45:19.000000 spectralnet-0.0.2/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.273912 spectralnet-0.0.3/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-25 12:12:14.000000 spectralnet-0.0.3/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-27 12:06:39.273998 spectralnet-0.0.3/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-27 12:05:58.000000 spectralnet-0.0.3/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-27 10:10:06.000000 spectralnet-0.0.3/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-27 12:06:39.274305 spectralnet-0.0.3/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-27 11:38:50.000000 spectralnet-0.0.3/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.269049 spectralnet-0.0.3/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.270830 spectralnet-0.0.3/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      114 2023-06-27 09:56:19.000000 spectralnet-0.0.3/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.271770 spectralnet-0.0.3/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-25 13:45:07.000000 spectralnet-0.0.3/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-25 17:02:04.000000 spectralnet-0.0.3/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-25 13:27:35.000000 spectralnet-0.0.3/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-25 17:05:52.000000 spectralnet-0.0.3/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.272797 spectralnet-0.0.3/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-25 13:44:44.000000 spectralnet-0.0.3/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-27 09:25:21.000000 spectralnet-0.0.3/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-25 17:56:01.000000 spectralnet-0.0.3/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2897 2023-06-25 18:01:13.000000 spectralnet-0.0.3/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-26 12:24:44.000000 spectralnet-0.0.3/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.273767 spectralnet-0.0.3/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-25 17:49:01.000000 spectralnet-0.0.3/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3733 2023-06-25 18:43:37.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9437 2023-06-25 18:58:20.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7892 2023-06-27 11:52:09.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-25 17:43:03.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-25 17:04:22.000000 spectralnet-0.0.3/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.271409 spectralnet-0.0.3/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      823 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       12 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/top_level.txt
```

### Comparing `spectralnet-0.0.2/LICENSE.md` & `spectralnet-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/setup.cfg` & `spectralnet-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.0.2
+version = 0.0.3
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AmitaiYacobi/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/AmitaiYacobi/SpectralNet/issues
```

### Comparing `spectralnet-0.0.2/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.3/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.3/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_metrics.py` & `spectralnet-0.0.3/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.3/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.3/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.3/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_spectral.py` & `spectralnet-0.0.3/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.3/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.3/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.3/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         )
 
         train_loader, ortho_loader, valid_loader = self._get_data_loader()
 
         print("Training SpectralNet:")
         for epoch in range(self.epochs):
             train_loss = 0.0
-            for (X_grad, y_grad), (X_orth, _) in zip(train_loader, ortho_loader):
+            for (X_grad, _), (X_orth, _) in zip(train_loader, ortho_loader):
                 X_grad = X_grad.to(device=self.device)
                 X_grad = X_grad.view(X_grad.size(0), -1)
                 X_orth = X_orth.to(device=self.device)
                 X_orth = X_orth.view(X_orth.size(0), -1)
 
                 if self.is_sparse:
                     X_grad = make_batch_for_sparse_grapsh(X_grad)
@@ -159,16 +159,14 @@
                         X = self.siamese_net.forward_once(X)
 
                 W = self._get_affinity_matrix(X)
 
                 loss = self.criterion(W, Y)
                 valid_loss += loss.item()
 
-        if self.counter % 10 == 0:
-            plot_sorted_laplacian(W, y)
         self.counter += 1
 
         valid_loss /= len(valid_loader)
         return valid_loss
 
     def _get_affinity_matrix(self, X: torch.Tensor) -> torch.Tensor:
         """
```

### Comparing `spectralnet-0.0.2/src/spectralnet/_utils.py` & `spectralnet-0.0.3/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.2/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.3/src/spectralnet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/spectralnet/__init__.py
 src/spectralnet/_metrics.py
 src/spectralnet/_spectral.py
 src/spectralnet/_utils.py
 src/spectralnet.egg-info/PKG-INFO
 src/spectralnet.egg-info/SOURCES.txt
 src/spectralnet.egg-info/dependency_links.txt
```

