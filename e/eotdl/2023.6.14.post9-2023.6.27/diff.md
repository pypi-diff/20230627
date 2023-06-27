# Comparing `tmp/eotdl-2023.6.14.post9.tar.gz` & `tmp/eotdl-2023.6.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.6.14.post9.tar", max compression
+gzip compressed data, was "eotdl-2023.6.27.tar", max compression
```

## Comparing `eotdl-2023.6.14.post9.tar` & `eotdl-2023.6.27.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.6.14.post9/README.md
--rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.6.14.post9/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.6.14.post9/eotdl/auth/__init__.py
--rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.6.14.post9/eotdl/auth/main.py
--rw-r--r--   0        0        0      193 2023-06-14 12:17:22.982144 eotdl-2023.6.14.post9/eotdl/cli.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.14.post9/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.6.14.post9/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1491 2023-06-14 13:05:31.529532 eotdl-2023.6.14.post9/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.14.post9/eotdl/curation/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.14.post9/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.14.post9/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.14.post9/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.14.post9/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0      226 2023-06-14 12:42:18.658877 eotdl-2023.6.14.post9/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0      568 2023-06-14 13:04:46.461411 eotdl-2023.6.14.post9/eotdl/datasets/download.py
--rw-r--r--   0        0        0      846 2023-06-14 13:04:11.725320 eotdl-2023.6.14.post9/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.6.14.post9/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0      366 2023-06-14 13:05:23.913511 eotdl-2023.6.14.post9/eotdl/datasets/update.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.14.post9/eotdl/hello.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.14.post9/eotdl/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post9/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.14.post9/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0     9935 2023-06-14 12:57:49.716461 eotdl-2023.6.14.post9/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.6.14.post9/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.6.14.post9/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      788 2023-06-14 13:04:43.661404 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-06-14 10:24:20.819993 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      965 2023-06-14 13:05:23.037509 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/UpdateDataset.py
--rw-r--r--   0        0        0      270 2023-06-14 12:30:22.104262 eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0      479 2023-06-14 10:24:20.823993 eotdl-2023.6.14.post9/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.14.post9/eotdl/tools/stac.py
--rw-r--r--   0        0        0      621 2023-06-14 13:05:58.245604 eotdl-2023.6.14.post9/pyproject.toml
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post9/setup.py
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 eotdl-2023.6.14.post9/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.6.27/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.6.27/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.6.27/eotdl/auth/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.6.27/eotdl/auth/main.py
+-rw-r--r--   0        0        0      193 2023-06-14 12:17:22.982144 eotdl-2023.6.27/eotdl/cli.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.27/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.6.27/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1298 2023-06-19 14:16:48.822880 eotdl-2023.6.27/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.27/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.27/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.27/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.27/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.27/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0      159 2023-06-19 14:05:03.242426 eotdl-2023.6.27/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-16 12:06:24.332346 eotdl-2023.6.27/eotdl/datasets/download.py
+-rw-r--r--   0        0        0     1583 2023-06-16 10:46:33.504518 eotdl-2023.6.27/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.6.27/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.27/eotdl/hello.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.27/eotdl/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.27/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.27/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0    10025 2023-06-19 14:50:31.920344 eotdl-2023.6.27/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.6.27/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.6.27/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0     1908 2023-06-16 12:03:45.195900 eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      940 2023-06-16 11:34:57.062552 eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadFile.py
+-rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1943 2023-06-19 14:49:41.092104 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestFile.py
+-rw-r--r--   0        0        0     1337 2023-06-16 11:23:06.416437 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestFolder.py
+-rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.27/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      455 2023-06-16 11:29:50.861680 eotdl-2023.6.27/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      303 2023-06-16 12:06:29.796362 eotdl-2023.6.27/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-16 09:41:47.694244 eotdl-2023.6.27/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      642 2023-06-27 10:43:26.613664 eotdl-2023.6.27/pyproject.toml
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 eotdl-2023.6.27/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 eotdl-2023.6.27/PKG-INFO
```

### Comparing `eotdl-2023.6.14.post9/eotdl/__init__.py` & `eotdl-2023.6.27/eotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/access/sentinelhub/client.py` & `eotdl-2023.6.27/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.6.27/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/auth/main.py` & `eotdl-2023.6.27/eotdl/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/commands/auth.py` & `eotdl-2023.6.27/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/commands/datasets.py` & `eotdl-2023.6.27/eotdl/commands/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,57 @@
 import typer
+from pathlib import Path
+
 from ..datasets import (
     retrieve_datasets,
     download_dataset,
-    update_dataset,
-    ingest_large_dataset,
-    # ingest_large_dataset_parallel,
+    ingest_file,
+    ingest_folder,
 )
-from .auth import auth
 
 app = typer.Typer()
 
 
 @app.command()
-def list():
-    """
-    List all datasets
-    """
-    datasets = retrieve_datasets()
-    typer.echo(datasets)
-
-
-@app.command()
-def get(name: str, path: str = None):
+def ingest(path: Path, dataset: str):
     """
-    Download a dataset
+    Ingest a file
 
-    name: Name of the dataset
-    path: Path to download the dataset to
+    path: Path to folder with data (limited to 10 files, not recursive!)
+    dataset: Name of the dataset
     """
     try:
-        dst_path = download_dataset(name, path, user, typer.echo)
-        typer.echo(f"Dataset {name} downloaded to {dst_path}")
+        if path.is_dir():
+            ingest_folder(path, dataset, typer.echo)
+        else:
+            ingest_file(path, dataset, typer.echo)
     except Exception as e:
         typer.echo(e)
 
 
 @app.command()
-def ingest(
-    path: str,
-    name: str,
-    # p: Optional[int] = 0,
-):
+def list():
     """
-    Ingest a dataset
-
-    path: Path to dataset to ingest
-    n: Name of the dataset
+    List all datasets and files
     """
-    try:
-        # if p:
-        #     ingest_large_dataset_parallel(name, path, user, p, typer.echo)
-        ingest_large_dataset(name, path, typer.echo)
-        typer.echo(f"Dataset {name} ingested")
-    except Exception as e:
-        typer.echo(e)
+    datasets = retrieve_datasets()
+    typer.echo(datasets)
 
 
 @app.command()
-def update(
-    name: str,
-    path: str,
-):
+def get(dataset: str, file: str = None, path: str = None):
     """
-    Update a dataset
+    Download a dataset
 
-    name: Name of the dataset
-    path: Path to dataset to ingest
+    dataset: Name of the dataset
+    file: Name of the file to download (optional, if not provided, the whole dataset will be downloaded)
+    path: Path to download the dataset to (optional, if not provided, the dataset will be downloaded to ~/.eotdl/datasets)
     """
     try:
-        update_dataset(name, path, typer.echo)
-        typer.echo(f"Dataset {name} updated")
+        dst_path = download_dataset(dataset, file, path, typer.echo)
+        typer.echo(f"Data available at {dst_path}")
     except Exception as e:
         typer.echo(e)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/formatters.py` & `eotdl-2023.6.27/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/metadata.py` & `eotdl-2023.6.27/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/stac/dataframe.py` & `eotdl-2023.6.27/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/stac/extensions.py` & `eotdl-2023.6.27/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/stac/parsers.py` & `eotdl-2023.6.27/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/stac/stac.py` & `eotdl-2023.6.27/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/curation/stac/utils.py` & `eotdl-2023.6.27/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/datasets/ingest.py` & `eotdl-2023.6.27/eotdl/datasets/ingest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 from ..src.repos import APIRepo
-from ..src.usecases.datasets import IngestDataset, IngestLargeDataset
+from ..src.usecases.datasets import IngestFile, IngestFolder
 from ..auth import with_auth
 
+allowed_extensions = [
+    ".zip",
+    ".tar",
+    ".tar.gz",
+    ".csv",
+    ".txt",
+    ".json",
+    ".pdf",
+    ".md",
+]
+
 
 @with_auth
-def ingest_dataset(name, description, path, logger=None, user=None):
+def ingest_file(file, dataset, logger=None, user=None):
     api_repo = APIRepo()
-    ingest = IngestDataset(
-        api_repo,
-    )
-    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    ingest = IngestFile(api_repo, allowed_extensions, logger)
+    inputs = ingest.Inputs(file=file, dataset=dataset, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
 @with_auth
-def ingest_large_dataset(name, path, logger=None, user=None):
+def ingest_folder(folder, dataset, logger=None, user=None):
     api_repo = APIRepo()
-    ingest = IngestLargeDataset(api_repo, logger)
-    inputs = ingest.Inputs(name=name, path=path, user=user)
+    ingest = IngestFolder(api_repo, ingest_file, allowed_extensions, logger)
+    inputs = ingest.Inputs(folder=folder, dataset=dataset, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
-def ingest_q0(dataset, path):
-    return ingest_large_dataset(dataset, path)
-
-
-def ingest_q1(dataset, stac_catalog):
-    print("holas")
-    return
+# @with_auth
+# def ingest_dataset(name, description, path, logger=None, user=None):
+#     api_repo = APIRepo()
+#     ingest = IngestDataset(
+#         api_repo,
+#     )
+#     inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+#     outputs = ingest(inputs)
+#     return outputs.dataset
+
+
+# @with_auth
+# def ingest_large_dataset(name, path, logger=None, user=None):
+#     api_repo = APIRepo()
+#     ingest = IngestLargeDataset(api_repo, logger)
+#     inputs = ingest.Inputs(name=name, path=path, user=user)
+#     outputs = ingest(inputs)
+#     return outputs.dataset
+
+
+# def ingest_q0(dataset, path):
+#     return ingest_large_dataset(dataset, path)
+
+
+# def ingest_q1(dataset, stac_catalog):
+#     print("holas")
+#     return
```

### Comparing `eotdl-2023.6.14.post9/eotdl/datasets/retrieve.py` & `eotdl-2023.6.27/eotdl/datasets/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/src/repos/APIRepo.py` & `eotdl-2023.6.27/eotdl/src/repos/APIRepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,117 +27,121 @@
 
     def retrieve_dataset(self, name):
         response = requests.get(self.url + "datasets?name=" + name)
         if response.status_code == 200:
             return response.json(), None
         return None, response.json()["detail"]
 
-    def download_dataset(self, dataset_id, id_token, path):
-        url = self.url + "datasets/" + dataset_id + "/download"
+    def download_file(self, dataset, dataset_id, file, id_token, path):
+        url = self.url + "datasets/" + dataset_id + "/download/" + file
         headers = {"Authorization": "Bearer " + id_token}
         if path is None:
-            path = str(Path.home()) + "/.eotdl/datasets"
+            path = str(Path.home()) + "/.eotdl/datasets/" + dataset
             os.makedirs(path, exist_ok=True)
+        path = f"{path}/{file}"
+        # if os.path.exists(path):
+        #     raise Exception("File already exists")
         with requests.get(url, headers=headers, stream=True) as r:
             r.raise_for_status()
             total_size = int(r.headers.get("content-length", 0))
             block_size = 1024 * 1024 * 10
             progress_bar = tqdm(
                 total=total_size, unit="iB", unit_scale=True, unit_divisor=1024
             )
-            filename = r.headers.get("content-disposition").split("filename=")[1][1:-1]
-            path = f"{path}/{filename}"
-            if os.path.exists(path):
-                raise Exception("File already exists")
             with open(path, "wb") as f:
                 for chunk in r.iter_content(block_size):
                     progress_bar.update(len(chunk))
                     if chunk:
                         f.write(chunk)
             progress_bar.close()
             return path
 
+    def ingest_file(self, file, dataset, id_token, checksum):
+        reponse = requests.post(
+            self.url + "datasets",
+            files={"file": open(file, "rb")},
+            data={
+                "dataset": dataset,
+                "checksum": checksum,
+            },
+            headers={"Authorization": "Bearer " + id_token},
+        )
+        if reponse.status_code != 200:
+            return None, reponse.json()["detail"]
+        return reponse.json(), None
+
     def read_in_chunks(self, file_object, CHUNK_SIZE):
         while True:
             data = file_object.read(CHUNK_SIZE)
             if not data:
                 break
             yield data
 
-    def prepare_large_upload(self, name, id_token, checksum):
-        url = self.url + "datasets/chunk?name=" + name + "&checksum=" + checksum
-        response = requests.get(url, headers={"Authorization": "Bearer " + id_token})
+    def prepare_large_upload(self, file, dataset, checksum, id_token):
+        filename = Path(file).name
+        response = requests.post(
+            self.url + "datasets/uploadId",
+            json={"name": filename, "checksum": checksum, "dataset": dataset},
+            headers={"Authorization": "Bearer " + id_token},
+        )
         if response.status_code != 200:
             raise Exception(response.json()["detail"])
         data = response.json()
-        dataset_id, upload_id, parts = (
-            data["dataset_id"],
+        upload_id, parts = (
             data["upload_id"],
             data["parts"] if "parts" in data else [],
         )
-        return dataset_id, upload_id, parts
+        return upload_id, parts
 
     def get_chunk_size(self, content_size):
         # adapt chunk size to content size to avoid S3 limits (10000 parts, 500MB per part, 5TB per object)
         chunk_size = 1024 * 1024 * 10  # 10 MB (up to 100 GB, 10000 parts)
         if content_size >= 1024 * 1024 * 1024 * 100:  # 100 GB
             chunk_size = 1024 * 1024 * 100  # 100 MB (up to 1 TB, 10000 parts)
         elif content_size >= 1024 * 1024 * 1024 * 1000:  # 1 TB
             chunk_size = 1024 * 1024 * 500  # 0.5 GB (up to 5 TB, 10000 parts)
         return chunk_size
 
-    def ingest_large_dataset(self, path, upload_id, dataset_id, id_token, parts):
-        content_path = os.path.abspath(path)
+    def ingest_large_dataset(self, file, upload_id, id_token, parts):
+        content_path = os.path.abspath(file)
         content_size = os.stat(content_path).st_size
         chunk_size = self.get_chunk_size(content_size)
         total_chunks = content_size // chunk_size
-        url = self.url + "datasets/chunk"
-        headers = {
-            "Authorization": "Bearer " + id_token,
-            "Upload-Id": upload_id,
-            "Dataset-Id": dataset_id,
-        }
         # upload chunks sequentially
         pbar = tqdm(
             self.read_in_chunks(open(content_path, "rb"), chunk_size),
             total=total_chunks,
         )
         index = 0
-        parts_checkusms = []
         for chunk in pbar:
             part = index // chunk_size + 1
             offset = index + len(chunk)
             index = offset
             if part not in parts:
-                headers["Part-Number"] = str(part)
                 checksum = hashlib.md5(chunk).hexdigest()
-                parts_checkusms.append(checksum)
-                headers["Checksum"] = checksum
-                file = {"file": chunk}
-                r = requests.post(url, files=file, headers=headers)
-                if r.status_code != 200:
-                    return None, r.json()["detail"]
+                response = requests.post(
+                    self.url + "datasets/chunk/" + upload_id,
+                    files={"file": chunk},
+                    data={"part_number": part, "checksum": checksum},
+                    headers={"Authorization": "Bearer " + id_token},
+                )
+                if response.status_code != 200:
+                    raise Exception(response.json()["detail"])
             pbar.set_description(
                 "{:.2f}/{:.2f} MB".format(
                     offset / 1024 / 1024, content_size / 1024 / 1024
                 )
             )
         pbar.close()
         return
 
-    def complete_upload(self, name, id_token, upload_id, dataset_id, checksum):
-        url = self.url + "datasets/complete"
+    def complete_upload(self, id_token, upload_id):
         r = requests.post(
-            url,
-            json={"name": name, "checksum": checksum},
-            headers={
-                "Authorization": "Bearer " + id_token,
-                "Upload-Id": upload_id,
-                "Dataset-Id": dataset_id,
-            },
+            self.url + "datasets/complete/" + upload_id,
+            headers={"Authorization": "Bearer " + id_token},
         )
         if r.status_code != 200:
             return None, r.json()["detail"]
         return r.json(), None
 
     def update_dataset(self, name, path, id_token, checksum):
         # check that dataset exists
```

### Comparing `eotdl-2023.6.14.post9/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.6.27/eotdl/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.6.27/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadFile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from pydantic import BaseModel
 from ....src.utils import calculate_checksum
 
 
-class DownloadDataset:
-    def __init__(self, repo, logger):
+class DownloadFile:
+    def __init__(self, repo, retrieve_dataset, logger):
         self.repo = repo
+        self.retrieve_dataset = retrieve_dataset
         self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         dataset: str
+        file: str
         path: str = None
         user: dict
         checksum: str
 
     class Outputs(BaseModel):
         dst_path: str
 
     def __call__(self, inputs: Inputs) -> Outputs:
-        dst_path = self.repo.download_dataset(
-            inputs.dataset, inputs.user["id_token"], inputs.path
+        dataset = self.retrieve_dataset(inputs.dataset)
+        dst_path = self.repo.download_file(
+            inputs.dataset, inputs.file, inputs.user["id_token"], inputs.path
         )
         checksum = calculate_checksum(dst_path)
         self.logger(f"Checksum: {checksum}")
-        if inputs.checksum != checksum:
+        if dataset["checksum"] != checksum:
             self.logger("Checksums do not match")
         return self.Outputs(dst_path=dst_path)
```

### Comparing `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.6.27/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/eotdl/tools/stac.py` & `eotdl-2023.6.27/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.14.post9/pyproject.toml` & `eotdl-2023.6.27/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.06.14-9"
+version = "2023.06.27"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
@@ -18,11 +18,12 @@
 tqdm = "^4.65.0"
 pyjwt = "^2.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-watch = "^4.2.0"
+pytest-mock = "^3.6.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eotdl-2023.6.14.post9/setup.py` & `eotdl-2023.6.27/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.cli:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.6.14.post9',
+    'version': '2023.6.27',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library and CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.6.14.post9/PKG-INFO` & `eotdl-2023.6.27/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.6.14.post9
+Version: 2023.6.27
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

