# Comparing `tmp/tfds-nightly-4.9.2.dev202306270045.tar.gz` & `tmp/tfds_nightly-4.9.2.dev202306270046-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfds-nightly-4.9.2.dev202306270045.tar", last modified: Tue Jun 27 00:46:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

