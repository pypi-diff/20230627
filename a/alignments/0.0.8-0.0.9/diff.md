# Comparing `tmp/alignments-0.0.8.tar.gz` & `tmp/alignments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alignments-0.0.8.tar", last modified: Sun Jul 31 10:11:27 2022, max compression
+gzip compressed data, was "alignments-0.0.9.tar", last modified: Thu Sep  1 11:21:58 2022, max compression
```

## Comparing `alignments-0.0.8.tar` & `alignments-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-------   0 s1764494 (1831066) people   (10000)        0 2022-07-08 09:30:58.941881 alignments-0.0.8/alignments/__init__.py
--rw-------   0 s1764494 (1831066) people   (10000)    16268 2022-07-31 10:09:48.525618 alignments-0.0.8/alignments/dataset.py
--rw-------   0 s1764494 (1831066) people   (10000)     1118 2022-07-08 09:53:24.218206 alignments-0.0.8/alignments/datasets/libritts.py
--rw-------   0 s1764494 (1831066) people   (10000)      583 2022-07-31 10:10:27.741952 alignments-0.0.8/pyproject.toml
--rw-------   0 s1764494 (1831066) people   (10000)      218 2022-07-31 10:11:27.937930 alignments-0.0.8/PKG-INFO
+-rw-------   0 s1764494 (1831066) people   (10000)        0 2022-07-08 09:30:58.941881 alignments-0.0.9/alignments/__init__.py
+-rw-------   0 s1764494 (1831066) people   (10000)    16268 2022-07-31 10:09:48.525618 alignments-0.0.9/alignments/dataset.py
+-rw-------   0 s1764494 (1831066) people   (10000)     1183 2022-09-01 11:18:27.570492 alignments-0.0.9/alignments/datasets/libritts.py
+-rw-------   0 s1764494 (1831066) people   (10000)      583 2022-09-01 11:21:48.087006 alignments-0.0.9/pyproject.toml
+-rw-------   0 s1764494 (1831066) people   (10000)      218 2022-09-01 11:21:58.583824 alignments-0.0.9/PKG-INFO
```

### Comparing `alignments-0.0.8/alignments/dataset.py` & `alignments-0.0.9/alignments/dataset.py`

 * *Files identical despite different names*

### Comparing `alignments-0.0.8/alignments/datasets/libritts.py` & `alignments-0.0.9/alignments/datasets/libritts.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,12 +17,13 @@
     def collect_data(self, directory):
         for file in Path(directory).glob("**/*.wav"):
             transcript = open(file.with_suffix(".normalized.txt"), "r").read()
             if "illustration" in transcript.lower():
                 transcript = transcript.replace("Illustration:", " ")
             transcript = re.sub("[\[\]\(\)-]", " ", transcript)
             transcript = re.sub("\s+", " ", transcript)
+            transcript = re.sub(r"'(\w)'", "\g<1>", transcript)
             yield {
                 "path": file,
                 "speaker": file.parent.parent.name,
                 "transcript": transcript.upper(),
-            }
+            }
```

### Comparing `alignments-0.0.8/pyproject.toml` & `alignments-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alignments"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = [
     { name = "Christoph Minixhofer", email = "christoph.minixhofer@gmail.com" },
 ]
 dependencies = [
     "click>=8.0.4",
     "rich>=10.11.0",
```

