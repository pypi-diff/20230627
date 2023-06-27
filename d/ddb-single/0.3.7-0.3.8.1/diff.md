# Comparing `tmp/ddb_single-0.3.7.tar.gz` & `tmp/ddb_single-0.3.8.1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddb_single-0.3.7.tar", last modified: Wed May  3 09:10:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

