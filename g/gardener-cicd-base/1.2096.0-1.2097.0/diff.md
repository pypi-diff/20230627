# Comparing `tmp/gardener-cicd-base-1.2096.0.tar.gz` & `tmp/gardener_cicd_base-1.2097.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-base-1.2096.0.tar", last modified: Mon Jun 26 14:11:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

