# Comparing `tmp/markdown_it_pyrs-0.2.0.tar.gz` & `tmp/markdown_it_pyrs-0.2.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

