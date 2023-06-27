# Comparing `tmp/botocore-a-la-carte-osis-1.29.160.tar.gz` & `tmp/botocore_a_la_carte_osis-1.29.161-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.160.tar", last modified: Sat Jun 24 01:41:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

