# Comparing `tmp/gtfs_segments-0.0.7.tar.gz` & `tmp/gtfs_segments-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_segments-0.0.7.tar", last modified: Wed Dec 21 02:26:36 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

