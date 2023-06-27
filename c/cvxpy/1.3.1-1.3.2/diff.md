# Comparing `tmp/cvxpy-1.3.1.tar.gz` & `tmp/cvxpy-1.3.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.3.1.tar", last modified: Sat Mar 18 20:40:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

