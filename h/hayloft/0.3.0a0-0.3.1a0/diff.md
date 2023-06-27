# Comparing `tmp/hayloft-0.3.0a0.tar.gz` & `tmp/hayloft-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.3.0a0.tar", max compression
+gzip compressed data, was "hayloft-0.3.1a0.tar", max compression
```

## Comparing `hayloft-0.3.0a0.tar` & `hayloft-0.3.1a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.3.0a0/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.3.0a0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.3.0a0/hayloft/__init__.py
--rw-r--r--   0        0        0     4265 2023-06-27 15:29:55.817527 hayloft-0.3.0a0/hayloft/app.py
--rw-r--r--   0        0        0      948 2023-06-25 12:29:19.182724 hayloft-0.3.0a0/hayloft/llama_index.py
--rw-r--r--   0        0        0      687 2023-06-25 12:29:19.182724 hayloft-0.3.0a0/hayloft/logger.py
--rw-r--r--   0        0        0   182466 2023-06-27 15:27:13.175908 hayloft-0.3.0a0/hayloft/public/assets/index-b19f38d7.js
--rw-r--r--   0        0        0    27072 2023-06-27 15:27:13.175908 hayloft-0.3.0a0/hayloft/public/assets/index-fd5275c2.css
--rw-r--r--   0        0        0      384 2023-06-27 15:27:17.012614 hayloft-0.3.0a0/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.3.0a0/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.3.0a0/hayloft/sse.py
--rw-r--r--   0        0        0      573 2023-06-27 15:31:18.854983 hayloft-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 hayloft-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.3.1a0/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.3.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.3.1a0/hayloft/__init__.py
+-rw-r--r--   0        0        0     4265 2023-06-27 17:26:34.574436 hayloft-0.3.1a0/hayloft/app.py
+-rw-r--r--   0        0        0      948 2023-06-25 12:29:19.182724 hayloft-0.3.1a0/hayloft/llama_index.py
+-rw-r--r--   0        0        0      687 2023-06-25 12:29:19.182724 hayloft-0.3.1a0/hayloft/logger.py
+-rw-r--r--   0        0        0   182480 2023-06-27 17:25:50.527648 hayloft-0.3.1a0/hayloft/public/assets/index-6f47c6c1.js
+-rw-r--r--   0        0        0    27072 2023-06-27 17:25:50.527648 hayloft-0.3.1a0/hayloft/public/assets/index-fd5275c2.css
+-rw-r--r--   0        0        0      384 2023-06-27 17:25:55.347661 hayloft-0.3.1a0/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.3.1a0/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.3.1a0/hayloft/sse.py
+-rw-r--r--   0        0        0      573 2023-06-27 17:27:48.431326 hayloft-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 hayloft-0.3.1a0/PKG-INFO
```

### Comparing `hayloft-0.3.0a0/LICENSE` & `hayloft-0.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/README.md` & `hayloft-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/app.py` & `hayloft-0.3.1a0/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/llama_index.py` & `hayloft-0.3.1a0/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/logger.py` & `hayloft-0.3.1a0/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/public/assets/index-b19f38d7.js` & `hayloft-0.3.1a0/hayloft/public/assets/index-6f47c6c1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8768,27 +8768,27 @@
         sessionId: 0,
         events: [],
         records: [],
         eagerMode: !0
     }),
     Vc = e => e.replace(/^[\n]+/, "").replace(/[\n]+$/, ""),
     ih = (e, t) => t.eagerMode && t.events.length > 0 && t.events[t.events.length - 1].title === e.title && e.message.length < 1e3 && t.events[t.events.length - 1].type === "info" && e.type === "info" ? t.records.map((n, r) => r === 0 ? {
-        indexes: [...n.indexes, r],
+        indexes: [t.events.length, ...n.indexes],
         folded: !1
     } : n) : [{
         indexes: [t.events.length],
         folded: !1
     }, ...t.records],
     Qc = (e, t) => t ? e.reduceRight((n, r, l) => {
         if (l === e.length - 1) return [{
             indexes: [l],
             folded: !0
         }]; {
             let o = e[l + 1];
-            if (o.title === r.title && r.message.length < 1e3 && o.type === "info" && r.type === "info") {
+            if (o.title === r.title && o.message.length < 1e3 && o.type === "info" && r.type === "info") {
                 let i = n[n.length - 1];
                 return n[n.length - 1] = {
                     indexes: [...i.indexes, l],
                     folded: !0
                 }, n
             } else return [...n, {
                 indexes: [l],
```

### Comparing `hayloft-0.3.0a0/hayloft/public/assets/index-fd5275c2.css` & `hayloft-0.3.1a0/hayloft/public/assets/index-fd5275c2.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/schema.py` & `hayloft-0.3.1a0/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/hayloft/sse.py` & `hayloft-0.3.1a0/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.3.0a0/pyproject.toml` & `hayloft-0.3.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.3.0a0"
+version = "0.3.1a0"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.3.0a0/PKG-INFO` & `hayloft-0.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.3.0a0
+Version: 0.3.1a0
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

