# Comparing `tmp/pyscicat-0.2.6.tar.gz` & `tmp/pyscicat-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscicat-0.2.6.tar", last modified: Sun Feb  5 19:50:27 2023, max compression
+gzip compressed data, was "pyscicat-0.4.1.tar", last modified: Tue Jun 27 16:12:28 2023, max compression
```

## Comparing `pyscicat-0.2.6.tar` & `pyscicat-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,36 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.423677 pyscicat-0.2.6/
--rw-r--r--   0 dylan      (501) staff       (20)      171 2022-11-08 17:36:45.000000 pyscicat-0.2.6/AUTHORS.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2463 2022-11-08 17:36:45.000000 pyscicat-0.2.6/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     2617 2022-11-08 17:36:45.000000 pyscicat-0.2.6/LICENSE.txt
--rw-r--r--   0 dylan      (501) staff       (20)      361 2022-11-08 17:36:45.000000 pyscicat-0.2.6/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)      890 2023-02-05 19:50:27.423766 pyscicat-0.2.6/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      337 2022-11-08 17:36:45.000000 pyscicat-0.2.6/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.419856 pyscicat-0.2.6/docs/
--rw-r--r--   0 dylan      (501) staff       (20)      673 2022-11-08 17:36:45.000000 pyscicat-0.2.6/docs/Makefile
--rw-r--r--   0 dylan      (501) staff       (20)      797 2022-11-08 17:36:45.000000 pyscicat-0.2.6/docs/make.bat
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.420034 pyscicat-0.2.6/docs/source/
--rw-r--r--   0 dylan      (501) staff       (20)     6442 2022-11-08 17:36:45.000000 pyscicat-0.2.6/docs/source/conf.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.417314 pyscicat-0.2.6/docs/source/reference/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.420619 pyscicat-0.2.6/docs/source/reference/generated/
--rw-r--r--   0 dylan      (501) staff       (20)      375 2022-11-08 17:36:45.000000 pyscicat-0.2.6/docs/source/reference/generated/pyscicat.client.ScicatClient.rst
--rw-r--r--   0 dylan      (501) staff       (20)      287 2022-11-08 17:36:45.000000 pyscicat-0.2.6/docs/source/reference/generated/pyscicat.model.rst
--rw-r--r--   0 dylan      (501) staff       (20)      258 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyproject.toml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.424251 pyscicat-0.2.6/pyscicat/
--rw-r--r--   0 dylan      (501) staff       (20)       93 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      497 2023-02-05 19:50:27.424288 pyscicat-0.2.6/pyscicat/_version.py
--rw-r--r--   0 dylan      (501) staff       (20)    30981 2023-02-05 19:48:31.000000 pyscicat-0.2.6/pyscicat/client.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.422700 pyscicat-0.2.6/pyscicat/hdf5/
--rw-------   0 dylan      (501) staff       (20)        0 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/hdf5/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     3472 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/hdf5/h5tools.py
--rw-r--r--   0 dylan      (501) staff       (20)     4690 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/hdf5/scientific_metadata.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.422894 pyscicat-0.2.6/pyscicat/ingest/
--rw-------   0 dylan      (501) staff       (20)        0 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/ingest/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     6108 2023-02-05 19:48:31.000000 pyscicat-0.2.6/pyscicat/model.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.423400 pyscicat-0.2.6/pyscicat/tests/
--rw-------   0 dylan      (501) staff       (20)        0 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/tests/__init__.py
--rw-------   0 dylan      (501) staff       (20)        0 2022-11-08 17:36:45.000000 pyscicat-0.2.6/pyscicat/tests/conftest.py
--rw-r--r--   0 dylan      (501) staff       (20)     7277 2023-02-05 19:48:31.000000 pyscicat-0.2.6/pyscicat/tests/test_client.py
--rw-r--r--   0 dylan      (501) staff       (20)     5379 2022-12-02 19:17:20.000000 pyscicat-0.2.6/pyscicat/tests/test_suite_2.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-02-05 19:50:27.422249 pyscicat-0.2.6/pyscicat.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)      890 2023-02-05 19:50:27.000000 pyscicat-0.2.6/pyscicat.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      751 2023-02-05 19:50:27.000000 pyscicat-0.2.6/pyscicat.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-02-05 19:50:27.000000 pyscicat-0.2.6/pyscicat.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       71 2023-02-05 19:50:27.000000 pyscicat-0.2.6/pyscicat.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        9 2023-02-05 19:50:27.000000 pyscicat-0.2.6/pyscicat.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       18 2022-11-08 17:36:45.000000 pyscicat-0.2.6/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)      180 2023-02-05 19:50:27.424074 pyscicat-0.2.6/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     2171 2022-11-08 17:36:45.000000 pyscicat-0.2.6/setup.py
--rw-r--r--   0 dylan      (501) staff       (20)    68751 2022-11-08 17:36:45.000000 pyscicat-0.2.6/versioneer.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524962 pyscicat-0.4.1/
+-rw-r--r--   0 dylan      (501) staff       (20)      171 2023-06-23 22:30:03.000000 pyscicat-0.4.1/AUTHORS.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2463 2023-06-23 22:30:03.000000 pyscicat-0.4.1/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      361 2023-06-23 22:30:03.000000 pyscicat-0.4.1/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)      888 2023-06-27 16:12:28.525047 pyscicat-0.4.1/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      337 2023-06-23 22:34:01.000000 pyscicat-0.4.1/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522247 pyscicat-0.4.1/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)      673 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/Makefile
+-rw-r--r--   0 dylan      (501) staff       (20)      797 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/make.bat
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522397 pyscicat-0.4.1/docs/source/
+-rw-r--r--   0 dylan      (501) staff       (20)     6442 2023-06-23 22:34:01.000000 pyscicat-0.4.1/docs/source/conf.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.520395 pyscicat-0.4.1/docs/source/reference/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522813 pyscicat-0.4.1/docs/source/reference/generated/
+-rw-r--r--   0 dylan      (501) staff       (20)      375 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/source/reference/generated/pyscicat.client.ScicatClient.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      287 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/source/reference/generated/pyscicat.model.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      258 2023-06-23 22:30:03.000000 pyscicat-0.4.1/pyproject.toml
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.525591 pyscicat-0.4.1/pyscicat/
+-rw-r--r--   0 dylan      (501) staff       (20)       93 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)      497 2023-06-27 16:12:28.525621 pyscicat-0.4.1/pyscicat/_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)    26331 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/client.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524740 pyscicat-0.4.1/pyscicat/hdf5/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3472 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/h5tools.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4690 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/scientific_metadata.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524853 pyscicat-0.4.1/pyscicat/ingest/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2023-06-23 22:30:03.000000 pyscicat-0.4.1/pyscicat/ingest/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6108 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/model.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524410 pyscicat-0.4.1/pyscicat.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)      888 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      607 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      245 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        9 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     1123 2023-06-27 16:12:28.525450 pyscicat-0.4.1/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)      134 2023-06-23 22:34:01.000000 pyscicat-0.4.1/setup.py
+-rw-r--r--   0 dylan      (501) staff       (20)    68751 2023-06-23 22:34:01.000000 pyscicat-0.4.1/versioneer.py
```

### Comparing `pyscicat-0.2.6/LICENSE` & `pyscicat-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/docs/Makefile` & `pyscicat-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/docs/make.bat` & `pyscicat-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/docs/source/conf.py` & `pyscicat-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/pyscicat/client.py` & `pyscicat-0.4.1/pyscicat/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 import re
 from typing import Optional
 from urllib.parse import urljoin, quote_plus
 
 from pydantic import BaseModel
 import requests
 
+
 from pyscicat.model import (
     Attachment,
-    Datablock,
     Dataset,
-    DerivedDataset,
     Instrument,
     OrigDatablock,
     Proposal,
-    RawDataset,
     Sample,
 )
 
 logger = logging.getLogger("splash_ingest")
 can_debug = logger.isEnabledFor(logging.DEBUG)
 
 
@@ -128,53 +126,14 @@
         logger.info(
             "Operation '%s' successful%s",
             operation,
             f"pid={result['pid']}" if "pid" in result else "",
         )
         return result
 
-    def datasets_replace(self, dataset: Dataset) -> str:
-        """
-        Create a new dataset or update an existing one
-        This function was renamed.
-        It is still accessible with the original name for backward compatibility
-        The original names were upload_dataset replace_datasets
-        This function is obsolete and it will be remove in next relesases
-
-
-        Parameters
-        ----------
-        dataset : Dataset
-            Dataset to create or update
-
-        Returns
-        -------
-        str
-            pid of the dataset
-        """
-
-        if isinstance(dataset, RawDataset):
-            dataset_url = "RawDataSets/replaceOrCreate"
-        elif isinstance(dataset, DerivedDataset):
-            dataset_url = "DerivedDatasets/replaceOrCreate"
-        else:
-            raise TypeError(
-                "Dataset type not recognized (not Derived or Raw dataset instances)"
-            )
-        return self._call_endpoint(
-            cmd="post", endpoint=dataset_url, data=dataset, operation="datasets_replace"
-        ).get("pid")
-
-    """
-        Upload or create a new dataset
-        Original name, kept for for backward compatibility
-    """
-    upload_dataset = datasets_replace
-    replace_dataset = datasets_replace
-
     def datasets_create(self, dataset: Dataset) -> str:
         """
         Upload a new dataset. Uses the generic dataset endpoint.
         Relies on the endpoint to sense the dataset type
         This function was renamed.
         It is still accessible with the original name for backward compatibility
         The original name were create_dataset and upload_new_dataset
@@ -201,81 +160,14 @@
     """
         Upload a new dataset
         Original name, kept for for backward compatibility
     """
     upload_new_dataset = datasets_create
     create_dataset = datasets_create
 
-    def datasets_raw_replace(self, dataset: Dataset) -> str:
-        """
-        Create a new raw dataset or update an existing one
-        This function was renamed.
-        It is still accessible with the original name for backward compatibility
-        The original names were repalce_raw_dataset and upload_raw_dataset
-        This function is obsolete and it will be removed in future releases
-
-        Parameters
-        ----------
-        dataset : Dataset
-            Dataset to load
-
-        Returns
-        -------
-        str
-            pid (or unique identifier) of the newly created dataset
-
-        Raises
-        ------
-        ScicatCommError
-            Raises if a non-20x message is returned
-        """
-        return self._call_endpoint(
-            cmd="post",
-            endpoint="RawDataSets/replaceOrCreate",
-            data=dataset,
-            operation="datasets_raw_replace",
-        ).get("pid")
-
-    """
-        Upload a raw dataset
-        Original name, kept for for backward compatibility
-    """
-    upload_raw_dataset = datasets_raw_replace
-    replace_raw_dataset = datasets_raw_replace
-
-    def datasets_derived_replace(self, dataset: Dataset) -> str:
-        """
-        Create a new derived dataset or update an existing one
-        This function was renamed.
-        It is still accessible with the original name for backward compatibility
-        The original names were replace_derived_dataset and upload_derived_dataset
-
-
-        Parameters
-        ----------
-        dataset : Dataset
-            Dataset to upload
-
-        Returns
-        -------
-        str
-            pid (or unique identifier) of the newly created dataset
-
-        Raises
-        ------
-        ScicatCommError
-            Raises if a non-20x message is returned
-        """
-        return self._call_endpoint(
-            cmd="post",
-            endpoint="DerivedDataSets/replaceOrCreate",
-            data=dataset,
-            operation="datasets_derived_replace",
-        ).get("pid")
-
     def datasets_update(self, dataset: Dataset, pid: str) -> str:
         """Updates an existing dataset
         This function was renamed.
         It is still accessible with the original name for backward compatibility
         The original name was update_dataset.
 
         Parameters
@@ -304,55 +196,14 @@
 
     """
         Update a dataset
         Original name, kept for for backward compatibility
     """
     update_dataset = datasets_update
 
-    def datasets_datablock_create(
-        self, datablock: Datablock, datasetType: str = "RawDatasets"
-    ) -> dict:
-        """
-        Create a new datablock for a dataset.
-        The dataset can be both Raw or Derived.
-        It is still accessible with the original name for backward compatibility
-        The original names were create_dataset_datablock and upload_datablock
-        This function is obsolete and will be removed in future releases
-        Function datasets_origdatablock_create should be used.
-
-        Parameters
-        ----------
-        datablock : Datablock
-            Datablock to upload
-
-        Returns
-        -------
-        datablock : Datablock
-            The created Datablock with id
-
-        Raises
-        ------
-        ScicatCommError
-            Raises if a non-20x message is returned
-        """
-        endpoint = f"{datasetType}/{quote_plus(datablock.datasetId)}/origdatablocks"
-        return self._call_endpoint(
-            cmd="post",
-            endpoint=endpoint,
-            data=datablock,
-            operation="datasets_datablock_create",
-        )
-
-    """
-        Upload a Datablock
-        Original name, kept for for backward compatibility
-    """
-    upload_datablock = datasets_datablock_create
-    create_dataset_datablock = datasets_datablock_create
-
     def datasets_origdatablock_create(self, origdatablock: OrigDatablock) -> dict:
         """
         Create a new SciCat Dataset OrigDatablock
         This function has been renamed.
         It is still accessible with the original name for backward compatibility
         The original names were create_dataset_origdatablock and upload_dataset_origdatablock
 
@@ -384,15 +235,15 @@
         Create a new SciCat Dataset OrigDatablock
         Original name, kept for for backward compatibility
     """
     upload_dataset_origdatablock = datasets_origdatablock_create
     create_dataset_origdatablock = datasets_origdatablock_create
 
     def datasets_attachment_create(
-        self, attachment: Attachment, datasetType: str = "RawDatasets"
+        self, attachment: Attachment, datasetType: str = "Datasets"
     ) -> dict:
         """
         Create a new Attachment for a dataset.
         Note that datasetType can be provided to determine the type of dataset
         that this attachment is attached to. This is required for creating the url that SciCat uses.
         This function has been renamed.
         It is still accessible with the original name for backward compatibility
@@ -702,15 +553,15 @@
         ----------
         filter_fields : dict
             Dictionary of filtering fields. Must be json serializable.
         """
         if not filter_fields:
             filter_fields = {}
         filter_fields = json.dumps(filter_fields)
-        endpoint = f'/Datasets/?filter={{"where":{filter_fields}}}'
+        endpoint = f'Datasets?filter={{"where":{filter_fields}}}'
         return self._call_endpoint(
             cmd="get", endpoint=endpoint, operation="datasets_get_many", allow_404=True
         )
 
     """
         find a set of datasets according to the simple filter provided
         Original name, kept for for backward compatibility
@@ -875,15 +726,15 @@
         Returns
         -------
         dict
             The orig_datablocks of the dataset with the requested pid
         """
         return self._call_endpoint(
             cmd="get",
-            endpoint=f"/Datasets/{quote_plus(pid)}/origdatablocks",
+            endpoint=f"Datasets/{quote_plus(pid)}/origdatablocks",
             operation="datasets_origdatablocks_get_one",
             allow_404=True,
         )
 
     get_dataset_origdatablocks = datasets_origdatablocks_get_one
 
     def datasets_delete(self, pid: str) -> Optional[dict]:
@@ -900,15 +751,15 @@
         Returns
         -------
         dict
             response from SciCat backend
         """
         return self._call_endpoint(
             cmd="delete",
-            endpoint=f"/Datasets/{quote_plus(pid)}",
+            endpoint=f"Datasets/{quote_plus(pid)}",
             operation="datasets_delete",
             allow_404=True,
         )
 
     delete_dataset = datasets_delete
```

### Comparing `pyscicat-0.2.6/pyscicat/hdf5/h5tools.py` & `pyscicat-0.4.1/pyscicat/hdf5/h5tools.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/pyscicat/hdf5/scientific_metadata.py` & `pyscicat-0.4.1/pyscicat/hdf5/scientific_metadata.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/pyscicat/model.py` & `pyscicat-0.4.1/pyscicat/model.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.2.6/pyscicat.egg-info/SOURCES.txt` & `pyscicat-0.4.1/pyscicat.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 AUTHORS.rst
 LICENSE
-LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/reference/generated/pyscicat.client.ScicatClient.rst
@@ -21,12 +19,8 @@
 pyscicat.egg-info/SOURCES.txt
 pyscicat.egg-info/dependency_links.txt
 pyscicat.egg-info/requires.txt
 pyscicat.egg-info/top_level.txt
 pyscicat/hdf5/__init__.py
 pyscicat/hdf5/h5tools.py
 pyscicat/hdf5/scientific_metadata.py
-pyscicat/ingest/__init__.py
-pyscicat/tests/__init__.py
-pyscicat/tests/conftest.py
-pyscicat/tests/test_client.py
-pyscicat/tests/test_suite_2.py
+pyscicat/ingest/__init__.py
```

### Comparing `pyscicat-0.2.6/versioneer.py` & `pyscicat-0.4.1/versioneer.py`

 * *Files identical despite different names*

