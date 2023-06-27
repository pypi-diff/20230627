# Comparing `tmp/foundry_ml-0.6.3.tar.gz` & `tmp/foundry_ml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry_ml-0.6.3.tar", last modified: Wed May 24 21:13:23 2023, max compression
+gzip compressed data, was "foundry_ml-0.7.0.tar", last modified: Tue Jun 27 16:21:07 2023, max compression
```

## Comparing `foundry_ml-0.6.3.tar` & `foundry_ml-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    33352 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/foundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/https_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/https_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/tf_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/loaders/torch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/foundry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/foundry_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 21:13:23.000000 foundry_ml-0.6.3/foundry_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:23.451231 foundry_ml-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-24 21:13:10.000000 foundry_ml-0.6.3/tests/test_foundry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/foundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/https_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/https_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/foundry/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/loaders/tf_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/loaders/torch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/foundry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/foundry_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-27 16:21:06.000000 foundry_ml-0.7.0/foundry_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 16:21:06.000000 foundry_ml-0.7.0/foundry_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:21:06.000000 foundry_ml-0.7.0/foundry_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 16:21:06.000000 foundry_ml-0.7.0/foundry_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:21:06.000000 foundry_ml-0.7.0/foundry_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:21:07.008723 foundry_ml-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-06-27 16:20:58.000000 foundry_ml-0.7.0/tests/test_foundry.py
```

### Comparing `foundry_ml-0.6.3/LICENSE` & `foundry_ml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/PKG-INFO` & `foundry_ml-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry_ml
-Version: 0.6.3
+Version: 0.7.0
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,16 @@
 ```python
 from foundry import Foundry
 f = Foundry(index="mdf")
 
 
 f = f.load("10.18126/e73h-3w6n", globus=True)
 ```
+*NOTE*: If you run locally and don't want to install the [Globus Connect Personal endpoint](https://www.globus.org/globus-connect-personal), just set the `globus=False`.
+
 If running this code in a notebook, a table of metadata for the dataset will appear:
 
 <img width="903" alt="metadata" src="https://user-images.githubusercontent.com/16869564/197038472-0b6ae559-4a6b-4b20-88e5-679bb6eb4f5c.png">
 
 We can use the data with `f.load_data()` and specifying splits such as `train` for different segments of the dataset, then use matplotlib to visualize it.
 
 ```python
@@ -81,14 +83,17 @@
     axs[i].imshow(imgs[key_list[i]])
     axs[i].scatter(coords[key_list[i]][:,0], coords[key_list[i]][:,1], s = 20, c = 'r', alpha=0.5)
 ```
 <img width="595" alt="Screen Shot 2022-10-20 at 2 22 43 PM" src="https://user-images.githubusercontent.com/16869564/197039252-6d9c78ba-dc09-4037-aac2-d6f7e8b46851.png">
 
 [See full examples](./examples)
 
+# Contributing
+Foundry is an Open Source project and we encourage contributions from the community. To contribute, please fork from the `main` branch and open a Pull Request on the `main` branch. A member of our team will review your PR shortly.
+
 # Primary Support
 This work was supported by the National Science Foundation under NSF Award Number: 1931306 "Collaborative Research: Framework: Machine Learning Materials Innovation Infrastructure".
 
 # Other Support
 Foundry-ML brings together many components in the materials data ecosystem. Including [MAST-ML](https://mastmldocs.readthedocs.io/en/latest/), the [Data and Learning Hub for Science](https://www.dlhub.org) (DLHub), and the [Materials Data Facility](https://materialsdatafacility.org) (MDF).
 
 ## MAST-ML
```

### Comparing `foundry_ml-0.6.3/README.md` & `foundry_ml-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 ```python
 from foundry import Foundry
 f = Foundry(index="mdf")
 
 
 f = f.load("10.18126/e73h-3w6n", globus=True)
 ```
+*NOTE*: If you run locally and don't want to install the [Globus Connect Personal endpoint](https://www.globus.org/globus-connect-personal), just set the `globus=False`.
+
 If running this code in a notebook, a table of metadata for the dataset will appear:
 
 <img width="903" alt="metadata" src="https://user-images.githubusercontent.com/16869564/197038472-0b6ae559-4a6b-4b20-88e5-679bb6eb4f5c.png">
 
 We can use the data with `f.load_data()` and specifying splits such as `train` for different segments of the dataset, then use matplotlib to visualize it.
 
 ```python
@@ -61,14 +63,17 @@
     axs[i].imshow(imgs[key_list[i]])
     axs[i].scatter(coords[key_list[i]][:,0], coords[key_list[i]][:,1], s = 20, c = 'r', alpha=0.5)
 ```
 <img width="595" alt="Screen Shot 2022-10-20 at 2 22 43 PM" src="https://user-images.githubusercontent.com/16869564/197039252-6d9c78ba-dc09-4037-aac2-d6f7e8b46851.png">
 
 [See full examples](./examples)
 
+# Contributing
+Foundry is an Open Source project and we encourage contributions from the community. To contribute, please fork from the `main` branch and open a Pull Request on the `main` branch. A member of our team will review your PR shortly.
+
 # Primary Support
 This work was supported by the National Science Foundation under NSF Award Number: 1931306 "Collaborative Research: Framework: Machine Learning Materials Innovation Infrastructure".
 
 # Other Support
 Foundry-ML brings together many components in the materials data ecosystem. Including [MAST-ML](https://mastmldocs.readthedocs.io/en/latest/), the [Data and Learning Hub for Science](https://www.dlhub.org) (DLHub), and the [Materials Data Facility](https://materialsdatafacility.org) (MDF).
 
 ## MAST-ML
```

### Comparing `foundry_ml-0.6.3/foundry/auth.py` & `foundry_ml-0.7.0/foundry/auth.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry/foundry.py` & `foundry_ml-0.7.0/foundry/foundry.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,31 +43,36 @@
     forge_client: Any
     connect_client: Any
     transfer_client: Any
     auth_client: Any
     index = ""
     auths: Any
 
-    xtract_tokens: Any
-
     def __init__(
-            self, no_browser=False, no_local_server=False, index="mdf", authorizers=None, **data
+            self, name=None, no_browser=False, no_local_server=False, index="mdf", authorizers=None,
+            download=True, globus=True, verbose=False, metadata=None, interval=10, **data
     ):
         """Initialize a Foundry client
         Args:
+            name (str): Name of the foundry dataset. If not supplied, metadata will not be loaded into
+                    the Foundry object
             no_browser (bool):  Whether to open the browser for the Globus Auth URL.
             no_local_server (bool): Whether a local server is available.
                     This should be `False` when on remote server (e.g., Google Colab ).
             index (str): Index to use for search and data publication. Choices `mdf` or `mdf-test`
             authorizers (dict): A dictionary of authorizers to use, following the `mdf_toolbox` format
+            download (bool): If True, download the data associated with the package (default is True)
+            globus (bool): If True, download using Globus, otherwise https
+            verbose (bool): If True print additional debug information
+            metadata (dict): **For debug purposes.** A search result analog to prepopulate metadata.
+            interval (int): How often to poll Globus to check if transfers are complete
             data (dict): Other arguments, e.g., results from an MDF search result that are used
                     to populate Foundry metadata fields
 
-        Returns
-        -------
+        Returns:
             an initialized and authenticated Foundry client
         """
         super().__init__(**data)
         self.index = index
         self.auths = None
 
         if authorizers:
@@ -136,36 +141,34 @@
             openid_authorizer=self.auths['openid'],
             sl_authorizer=self.auths[
                 "https://auth.globus.org/scopes/d31d4f5d-be37-4adc-a761-2f716b7af105/action_all"
             ],
             force_login=False,
         )
 
-        self.xtract_tokens = {
-            "auth_token": self.auths["petrel"].access_token,
-            "transfer_token": self.auths["transfer"].authorizer.access_token,
-            "funcx_token": self.auths[
-                "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all"
-            ].access_token,
-        }
+        if name is not None:
+            self._load(name=name,
+                       download=download,
+                       globus=globus,
+                       verbose=verbose,
+                       metadata=metadata,
+                       authorizers=authorizers,
+                       interval=interval)
 
-    def load(self, name, download=True, globus=False, verbose=False, metadata=None, authorizers=None, **kwargs):
+    def _load(self, name, download=True, globus=True, verbose=False, metadata=None, authorizers=None, interval=None):
         """Load the metadata for a Foundry dataset into the client
         Args:
             name (str): Name of the foundry dataset
             download (bool): If True, download the data associated with the package (default is True)
             globus (bool): If True, download using Globus, otherwise https
             verbose (bool): If True print additional debug information
             metadata (dict): **For debug purposes.** A search result analog to prepopulate metadata.
-
-        Keyword Args:
             interval (int): How often to poll Globus to check if transfers are complete
 
-        Returns
-        -------
+        Returns:
             self
         """
 
         # handle empty dataset name (was returning all the datasets)
         if not name:
             raise ValueError("load: No dataset name is given")
 
@@ -204,15 +207,15 @@
 
         self.dc = res['dc']
         self.mdf = res['mdf']
         self.dataset = FoundryDataset(**res['dataset'])
 
         if download:  # Add check for package existence
             self.download(
-                interval=kwargs.get("interval", 10), globus=globus, verbose=verbose
+                interval=interval, globus=globus, verbose=verbose
             )
 
         return self
 
     def search(self, q=None, limit=None):
         """Search available Foundry datasets
         q (str): query string to match
@@ -255,23 +258,22 @@
         """Run a model on data
 
         Args:
            name (str): DLHub model name
            inputs: Data to send to DLHub as inputs (should be JSON serializable)
            funcx_endpoint (optional): UUID for the funcx endpoint to run the model on, if not the default (eg River)
 
-        Returns
-        -------
+        Returns:
              Returns results after invocation via the DLHub service
         """
         if funcx_endpoint is not None:
             self.dlhub_client.fx_endpoint = funcx_endpoint
         return self.dlhub_client.run(name, inputs=inputs, **kwargs)
 
-    def load_data(self, source_id=None, globus=True, as_hdf5=False):
+    def load_data(self, source_id=None, globus=True, as_hdf5=False, splits=[]):
         """Load in the data associated with the prescribed dataset
 
         Tabular Data Type: Data are arranged in a standard data frame
         stored in self.dataframe_file. The contents are read, and
 
         File Data Type: <<Add desc>>
 
@@ -279,29 +281,41 @@
         subclass Foundry and override the load_data function
 
         Args:
            inputs (list): List of strings for input columns
            targets (list): List of strings for output columns
            source_id (string): Relative path to the source file
            as_hdf5 (bool): If True and dataset is in hdf5 format, keep data in hdf5 format
+           splits (list): Labels of splits to be loaded
 
-        Returns
-        -------
-             (tuple): Tuple of X, y values
+        Returns:
+             (dict): a labeled dictionary of tuples
         """
         data = {}
 
         # Handle splits if they exist. Return as a labeled dictionary of tuples
         try:
             if self.dataset.splits:
-                for split in self.dataset.splits:
-                    data[split.label] = self._load_data(file=split.path, source_id=source_id, globus=globus,
-                                                        as_hdf5=as_hdf5)
+                if not splits:
+                    for split in self.dataset.splits:
+                        data[split.label] = self._load_data(file=split.path, source_id=source_id, globus=globus,
+                                                            as_hdf5=as_hdf5)
+                else:
+                    for split in self.dataset.splits:
+                        if split.label in splits:
+                            splits.remove(split.label)
+                            data[split.label] = self._load_data(file=split.path, source_id=source_id, globus=globus,
+                                                                as_hdf5=as_hdf5)
+                    if len(splits) > 0:
+                        raise ValueError(f'The split(s) {splits} were not found in the dataset!')
                 return data
             else:
+                # raise an error if splits are specified but not present in the dataset
+                if len(splits) > 0:
+                    raise ValueError(f"Splits to load were specified as {splits}, but no splits are present in dataset")
                 return {"data": self._load_data(source_id=source_id, globus=globus, as_hdf5=as_hdf5)}
         except Exception as e:
             raise Exception(
                 "Metadata not loaded into Foundry object, make sure to call load()") from e
 
     def _repr_html_(self) -> str:
         if not self.dc:
```

### Comparing `foundry_ml-0.6.3/foundry/https_download.py` & `foundry_ml-0.7.0/foundry/https_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Methods to download files from a Globus endpoint using Xtract (HTTPS). Now deprecated as of Aug 2022
+"""Methods to download files from a Globus endpoint
 """
 
 
 import os
 from collections import deque
 
 import requests
```

### Comparing `foundry_ml-0.6.3/foundry/https_upload.py` & `foundry_ml-0.7.0/foundry/https_upload.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry/loaders/tf_wrapper.py` & `foundry_ml-0.7.0/foundry/loaders/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry/loaders/torch_wrapper.py` & `foundry_ml-0.7.0/foundry/loaders/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry/models.py` & `foundry_ml-0.7.0/foundry/models.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry/utils.py` & `foundry_ml-0.7.0/foundry/utils.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.6.3/foundry_ml.egg-info/PKG-INFO` & `foundry_ml-0.7.0/foundry_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-ml
-Version: 0.6.3
+Version: 0.7.0
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,16 @@
 ```python
 from foundry import Foundry
 f = Foundry(index="mdf")
 
 
 f = f.load("10.18126/e73h-3w6n", globus=True)
 ```
+*NOTE*: If you run locally and don't want to install the [Globus Connect Personal endpoint](https://www.globus.org/globus-connect-personal), just set the `globus=False`.
+
 If running this code in a notebook, a table of metadata for the dataset will appear:
 
 <img width="903" alt="metadata" src="https://user-images.githubusercontent.com/16869564/197038472-0b6ae559-4a6b-4b20-88e5-679bb6eb4f5c.png">
 
 We can use the data with `f.load_data()` and specifying splits such as `train` for different segments of the dataset, then use matplotlib to visualize it.
 
 ```python
@@ -81,14 +83,17 @@
     axs[i].imshow(imgs[key_list[i]])
     axs[i].scatter(coords[key_list[i]][:,0], coords[key_list[i]][:,1], s = 20, c = 'r', alpha=0.5)
 ```
 <img width="595" alt="Screen Shot 2022-10-20 at 2 22 43 PM" src="https://user-images.githubusercontent.com/16869564/197039252-6d9c78ba-dc09-4037-aac2-d6f7e8b46851.png">
 
 [See full examples](./examples)
 
+# Contributing
+Foundry is an Open Source project and we encourage contributions from the community. To contribute, please fork from the `main` branch and open a Pull Request on the `main` branch. A member of our team will review your PR shortly.
+
 # Primary Support
 This work was supported by the National Science Foundation under NSF Award Number: 1931306 "Collaborative Research: Framework: Machine Learning Materials Innovation Infrastructure".
 
 # Other Support
 Foundry-ML brings together many components in the materials data ecosystem. Including [MAST-ML](https://mastmldocs.readthedocs.io/en/latest/), the [Data and Learning Hub for Science](https://www.dlhub.org) (DLHub), and the [Materials Data Facility](https://materialsdatafacility.org) (MDF).
 
 ## MAST-ML
```

### Comparing `foundry_ml-0.6.3/setup.py` & `foundry_ml-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 packages = (setuptools.find_packages(),)
 setuptools.setup(
     name="foundry_ml",
-    version="0.6.3",
+    version="0.7.0",
     author="""Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik""",
     author_email="blaiszik@uchicago.edu",
     packages=setuptools.find_packages(),
     description="Package to support simplified application of machine learning models to datasets in materials science",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `foundry_ml-0.6.3/tests/test_foundry.py` & `foundry_ml-0.7.0/tests/test_foundry.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,113 +142,137 @@
 def _delete_test_data(foundry_obj):
     path = os.path.join(foundry_obj.config.local_cache_dir, test_dataset)
     if os.path.isdir(path):
         shutil.rmtree(path)
 
 
 def test_foundry_init():
-    f = Foundry(authorizers=auths)
+    f = Foundry(test_dataset, download=False, authorizers=auths)
     assert isinstance(f.forge_client, Forge)
     assert isinstance(f.connect_client, MDFConnectClient)
 
     if not is_gha:
         assert isinstance(f.dlhub_client, DLHubClient)
 
-        f2 = Foundry(authorizers=auths, no_browser=False, no_local_server=True)
+        f2 = Foundry(test_dataset, download=False, authorizers=auths, no_browser=False, no_local_server=True)
         assert isinstance(f2.dlhub_client, DLHubClient)
         assert isinstance(f2.forge_client, Forge)
         assert isinstance(f2.connect_client, MDFConnectClient)
 
-        f3 = Foundry(authorizers=auths, no_browser=True, no_local_server=False)
+        f3 = Foundry(test_dataset, download=False, authorizers=auths, no_browser=True, no_local_server=False)
         assert isinstance(f3.dlhub_client, DLHubClient)
         assert isinstance(f3.forge_client, Forge)
         assert isinstance(f3.connect_client, MDFConnectClient)
 
 
 def test_list():
-    f = Foundry(authorizers=auths)
+    f = Foundry(test_dataset, download=False, authorizers=auths)
     ds = f.list()
     assert isinstance(ds, pd.DataFrame)
     assert len(ds) > 0
 
 
 def test_search():
-    f = Foundry(authorizers=auths)
+    f = Foundry(test_dataset, download=False, authorizers=auths)
     q = "Elwood"
     ds = f.search(q)
 
     assert isinstance(ds, pd.DataFrame)
     assert len(ds) > 0
     assert ds.iloc[0]['name'] is not None
     assert ds.iloc[0]['source_id'] is not None
     assert ds.iloc[0]['year'] is not None
 
 
 def test_metadata_pull():
-    f = Foundry(authorizers=auths)
-    assert f.dc == {}
-    f = f.load(test_dataset, download=False, authorizers=auths)
+    f = Foundry(test_dataset, download=False, authorizers=auths)
     assert f.dc["titles"][0]["title"] == expected_title
 
 
 def test_download_https():
-    f = Foundry(authorizers=auths)
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths)
     _delete_test_data(f)
 
-    f = f.load(test_dataset, download=True, globus=False, authorizers=auths)
     assert f.dc["titles"][0]["title"] == expected_title
     _delete_test_data(f)
 
 
 def test_dataframe_load():
-    f = Foundry(authorizers=auths)
-    _delete_test_data(f)
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths)
 
-    f = f.load(test_dataset, download=True, globus=False, authorizers=auths)
     res = f.load_data()
     X, y = res['train']
 
     assert len(X) > 1
     assert isinstance(X, pd.DataFrame)
     assert len(y) > 1
     assert isinstance(y, pd.DataFrame)
     _delete_test_data(f)
 
 
-def test_dataframe_load_doi():
-    f = Foundry(authorizers=auths)
+def test_dataframe_load_split():
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths)
+
+    res = f.load_data(splits=['train'])
+    X, y = res['train']
+
+    assert len(X) > 1
+    assert isinstance(X, pd.DataFrame)
+    assert len(y) > 1
+    assert isinstance(y, pd.DataFrame)
     _delete_test_data(f)
 
-    f = f.load(test_doi, download=True, globus=False, authorizers=auths)
+
+def test_dataframe_load_split_wrong_split_name():
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths)
+
+    with pytest.raises(Exception) as exc_info:
+        f.load_data(splits=['chewbacca'])
+
+    err = exc_info.value
+    assert hasattr(err, '__cause__')
+    assert isinstance(err.__cause__, ValueError)
+    _delete_test_data(f)
+
+
+@pytest.mark.skip(reason='No clear examples of datasets without splits - likely to be protected against soon.')
+def test_dataframe_load_split_but_no_splits():
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths)
+
+    with pytest.raises(ValueError):
+        f.load_data(splits=['train'])
+    _delete_test_data(f)
+
+
+def test_dataframe_load_doi():
+    f = Foundry(test_doi, download=True, globus=False, authorizers=auths)
+
     res = f.load_data()
     X, y = res['train']
 
     assert len(X) > 1
     assert isinstance(X, pd.DataFrame)
     assert len(y) > 1
     assert isinstance(y, pd.DataFrame)
     _delete_test_data(f)
 
 
 @pytest.mark.skipif(bool(is_gha), reason="Test does not succeed on GHA - no Globus endpoint")
 def test_download_globus():
-    f = Foundry(authorizers=auths, no_browser=True, no_local_server=True)
+    f = Foundry(test_dataset, download=True, authorizers=auths, no_browser=True, no_local_server=True)
     _delete_test_data(f)
 
-    f = f .load(test_dataset, download=True)
     assert f.dc["titles"][0]["title"] == expected_title
     _delete_test_data(f)
 
 
 @pytest.mark.skipif(bool(is_gha), reason="Test does not succeed on GHA - no Globus endpoint")
 def test_globus_dataframe_load():
-    f = Foundry(authorizers=auths, no_browser=True, no_local_server=True)
-    _delete_test_data(f)
+    f = Foundry(test_dataset, download=True, authorizers=auths, no_browser=True, no_local_server=True)
 
-    f = f.load(test_dataset, download=True)
     res = f.load_data()
     X, y = res['train']
 
     assert len(X) > 1
     assert isinstance(X, pd.DataFrame)
     assert len(y) > 1
     assert isinstance(y, pd.DataFrame)
@@ -375,34 +399,29 @@
 
 def test_check_status():
     # TODO: the 'active messages' in MDF CC's check_status() don't appear to do anything? need to determine how to test
     pass
 
 
 def test_to_pytorch():
-    f = Foundry(authorizers=auths, no_browser=True, no_local_server=True)
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths, no_browser=True, no_local_server=True)
 
-    _delete_test_data(f)
-
-    f = f.load(test_dataset, download=True, globus=False, authorizers=auths)
     raw = f.load_data()
 
     ds = f.to_torch(split='train')
 
     assert raw['train'][0].iloc[0][0] == ds[0]['input'][0]
     assert len(raw['train'][0]) == len(ds)
 
     _delete_test_data(f)
 
 
 def test_to_tensorflow():
-    f = Foundry(authorizers=auths, no_browser=True, no_local_server=True)
+    f = Foundry(test_dataset, download=True, globus=False, authorizers=auths, no_browser=True, no_local_server=True)
 
-    _delete_test_data(f)
-    f = f.load(test_dataset, download=True, globus=False, authorizers=auths)
     raw = f.load_data()
 
     ds = f.to_tensorflow(split='train')
 
     assert raw['train'][0].iloc[0][0] == ds[0]['input'][0]
     assert len(raw['train'][0]) == len(ds)
```

