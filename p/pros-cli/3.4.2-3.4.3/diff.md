# Comparing `tmp/pros-cli-3.4.2.tar.gz` & `tmp/pros_cli-3.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pros-cli-3.4.2.tar", last modified: Tue Apr 18 01:19:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

