# Comparing `tmp/collapse-gtdb-tree-0.0.2.tar.gz` & `tmp/collapse-gtdb-tree-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collapse-gtdb-tree-0.0.2.tar", last modified: Thu May 19 15:31:33 2022, max compression
+gzip compressed data, was "collapse-gtdb-tree-0.0.3.tar", last modified: Tue Jun 27 09:29:39 2023, max compression
```

## Comparing `collapse-gtdb-tree-0.0.2.tar` & `collapse-gtdb-tree-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      471 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2927 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3431 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     4132 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      471 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      411 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-05-19 15:31:33.000000 collapse-gtdb-tree-0.0.2/collapse_gtdb_tree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      719 2022-05-19 15:31:33.646490 collapse-gtdb-tree-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      950 2022-05-19 15:31:27.000000 collapse-gtdb-tree-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:29:39.575782 collapse-gtdb-tree-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-27 09:29:39.575782 collapse-gtdb-tree-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:29:39.579782 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 09:29:39.579782 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:29:39.575782 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 09:29:39.000000 collapse-gtdb-tree-0.0.3/collapse_gtdb_tree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-27 09:29:39.579782 collapse-gtdb-tree-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-27 09:29:30.000000 collapse-gtdb-tree-0.0.3/setup.py
```

### Comparing `collapse-gtdb-tree-0.0.2/LICENSE` & `collapse-gtdb-tree-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `collapse-gtdb-tree-0.0.2/README.md` & `collapse-gtdb-tree-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/__main__.py` & `collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,32 +40,31 @@
     file_name = Path(file).resolve().stem.split(".")[0]
     files = {}
     for rank in ranks:
         files[rank] = f"{file_name}_{rank}.tree"
     return files
 
 
-def collapse_gtdb_tree_by_rank(tree, taxonomy, ranks, files):
+def collapse_gtdb_tree_by_rank(tree, taxonomy, ranks, files, quoted_names=False):
     for rank in ranks:
         t = tree.copy()
         df = taxonomy[["genome_id", rank]]
         df = df.groupby([rank]).agg(lambda x: x.iloc[0]).reset_index()
         ids = df.set_index(
             "genome_id",
         ).to_dict()[rank]
         t.prune(list(ids.keys()))
         logging.info(f"Pruned tree for {rank} [leaves: {len(t.get_leaves()):,}]")
         # rename leaves
         for leaf in t.iter_leaves():
             leaf.name = ids[leaf.name]
-        t.write(outfile=str(files[rank]), quoted_node_names=True, format=1)
+        t.write(outfile=str(files[rank]), quoted_node_names=quoted_names, format=1)
 
 
 def main():
-
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(levelname)s ::: %(asctime)s ::: %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     args = get_arguments()
@@ -89,13 +88,17 @@
     logging.info(f"Read tree with {len(tree.get_leaves()):,} leaves")
     tips = [x.name for x in tree.iter_leaves()]
     taxonomy_file = taxonomy_file[taxonomy_file["genome_id"].isin(tips)]
 
     files = create_collapsed_tree_files(args.tree, args.rank)
     # get list of ids by ranks
     collapse_gtdb_tree_by_rank(
-        tree=tree, taxonomy=taxonomy_file, ranks=args.rank, files=files
+        tree=tree,
+        taxonomy=taxonomy_file,
+        ranks=args.rank,
+        files=files,
+        quoted_names=args.quoted_names,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `collapse-gtdb-tree-0.0.2/collapse_gtdb_tree/utils.py` & `collapse-gtdb-tree-0.0.3/collapse_gtdb_tree/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def is_debug():
     return logging.getLogger("my_logger").getEffectiveLevel() == logging.DEBUG
 
 
 filters = ["breadth", "depth", "depth_evenness", "breadth_expected_ratio"]
 
+
 # From https://stackoverflow.com/a/59617044/15704171
 def convert_list_to_str(lst):
     n = len(lst)
     if not n:
         return ""
     if n == 1:
         return lst[0]
@@ -85,19 +86,20 @@
 
 
 defaults = {
     "rank": "all",
 }
 
 help_msg = {
-    "tree": f"GTDB tree file",
-    "taxonomy": f"GTDB taxonomy file",
-    "rank": f"Select taxonomic rank to collapse",
-    "debug": f"Print debug messages",
-    "version": f"Print program version",
+    "tree": "GTDB tree file",
+    "taxonomy": "GTDB taxonomy file",
+    "rank": "Select taxonomic rank to collapse",
+    "debug": "Print debug messages",
+    "quoted_names": "Add quotes to the node and leaf names",
+    "version": "Print program version",
 }
 
 
 def get_arguments(argv=None):
     parser = argparse.ArgumentParser(
         description="A simple tool to collapse a GTDB tree to a certain taxonomic rank",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -121,14 +123,20 @@
         "-r",
         "--rank",
         type=lambda x: get_ranks(parser, x, "--rank"),
         default=defaults["rank"],
         help=help_msg["rank"],
     )
     parser.add_argument(
+        "--quoted-names",
+        dest="quoted_names",
+        action="store_true",
+        help=help_msg["quoted_names"],
+    )
+    parser.add_argument(
         "--debug", dest="debug", action="store_true", help=help_msg["debug"]
     )
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
         help=help_msg["version"],
```

### Comparing `collapse-gtdb-tree-0.0.2/setup.cfg` & `collapse-gtdb-tree-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `collapse-gtdb-tree-0.0.2/setup.py` & `collapse-gtdb-tree-0.0.3/setup.py`

 * *Files identical despite different names*

