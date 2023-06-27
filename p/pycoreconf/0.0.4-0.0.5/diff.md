# Comparing `tmp/pycoreconf-0.0.4.tar.gz` & `tmp/pycoreconf-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycoreconf-0.0.4.tar", last modified: Thu May  4 06:44:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

