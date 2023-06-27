# Comparing `tmp/ler-0.1.6.tar.gz` & `tmp/ler-0.1.7-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.1.6.tar", last modified: Mon Jun 19 08:51:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

