# Comparing `tmp/zhon-2.0.1.tar.gz` & `tmp/zhon-2.0.2.tar.gz`

## Comparing `zhon-2.0.1.tar` & `zhon-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/__init__.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/hanzi.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/pinyin.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/zhuyin.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/__init__.py
--rw-r--r--   0        0        0    39182 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/all.py
--rw-r--r--   0        0        0    32332 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/simplified.py
--rw-r--r--   0        0        0    32327 2020-02-02 00:00:00.000000 zhon-2.0.1/src/zhon/cedict/traditional.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 zhon-2.0.1/AUTHORS.rst
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhon-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 zhon-2.0.1/README.rst
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 zhon-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 zhon-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/__init__.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/hanzi.py
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/pinyin.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/zhuyin.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/cedict/__init__.py
+-rw-r--r--   0        0        0    39182 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/cedict/all.py
+-rw-r--r--   0        0        0    32332 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/cedict/simplified.py
+-rw-r--r--   0        0        0    32327 2020-02-02 00:00:00.000000 zhon-2.0.2/src/zhon/cedict/traditional.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 zhon-2.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhon-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 zhon-2.0.2/README.rst
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 zhon-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 zhon-2.0.2/PKG-INFO
```

### Comparing `zhon-2.0.1/src/zhon/hanzi.py` & `zhon-2.0.2/src/zhon/hanzi.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/src/zhon/pinyin.py` & `zhon-2.0.2/src/zhon/pinyin.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/src/zhon/zhuyin.py` & `zhon-2.0.2/src/zhon/zhuyin.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/src/zhon/cedict/all.py` & `zhon-2.0.2/src/zhon/cedict/all.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/src/zhon/cedict/simplified.py` & `zhon-2.0.2/src/zhon/cedict/simplified.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/src/zhon/cedict/traditional.py` & `zhon-2.0.2/src/zhon/cedict/traditional.py`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/LICENSE.txt` & `zhon-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zhon-2.0.1/README.rst` & `zhon-2.0.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 
     >>> re.findall(zhon.pinyin.sentence, 'Yuànzi lǐ tíngzhe yí liàng chē.', re.I)
     ['Yuànzi lǐ tíngzhe yí liàng chē.']
 
 Features
 --------
 
-* Includes commonly-used constants:
-    - CJK characters and radicals
-    - Chinese punctuation marks
-    - Chinese sentence regular expression pattern
-    - Pinyin vowels, consonants, lowercase, uppercase, and punctuation
-    - Pinyin syllable, word, and sentence regular expression patterns
-    - Zhuyin characters and marks
-    - Zhuyin syllable regular expression pattern
-    - CC-CEDICT characters
+Zhon includes the following commonly-used constants:
+
+* CJK characters and radicals
+* Chinese punctuation marks
+* Chinese sentence regular expression pattern
+* Pinyin vowels, consonants, lowercase, uppercase, and punctuation
+* Pinyin syllable, word, and sentence regular expression patterns
+* Zhuyin characters and marks
+* Zhuyin syllable regular expression pattern
+* CC-CEDICT characters
 
 Getting Started
 ---------------
 
-* `Install Zhon <https://tsroten.github.io/zhon/#installation>`_
-* Read `Zhon's introduction <https://tsroten.github.io/zhon/#using-zhon>`_
-* Learn from the `API documentation <https://tsroten.github.io/zhon/#module-zhon.hanzi>`_
+* `Install Zhon <https://tsroten.github.io/zhon/installation.html>`_
+* `Learn how to use Zhon <https://tsroten.github.io/zhon/api.html>`_
 * `Contribute <https://github.com/tsroten/zhon/blob/develop/CONTRIBUTING.rst>`_ documentation, code, or feedback
```

### Comparing `zhon-2.0.1/pyproject.toml` & `zhon-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Linguistic",
 ]
 
 [project.urls]
-Documentation = "https://tsroten.github.io/fcache"
-"Source code" = "https://github.com/tsroten/zhon"
+Documentation = "https://tsroten.github.io/zhon"
+Changes = "https://tsroten.github.io/zhon/history.html"
+"Issue Tracker" = "https://github.com/tsroten/zhon/issues"
+"Source Code" = "https://github.com/tsroten/zhon"
 
 [tool.hatch.version]
 path = "src/zhon/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/src",
```

### Comparing `zhon-2.0.1/PKG-INFO` & `zhon-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: zhon
-Version: 2.0.1
+Version: 2.0.2
 Summary: Zhon provides constants used in Chinese text processing.
-Project-URL: Documentation, https://tsroten.github.io/fcache
-Project-URL: Source code, https://github.com/tsroten/zhon
+Project-URL: Documentation, https://tsroten.github.io/zhon
+Project-URL: Changes, https://tsroten.github.io/zhon/history.html
+Project-URL: Issue Tracker, https://github.com/tsroten/zhon/issues
+Project-URL: Source Code, https://github.com/tsroten/zhon
 Author-email: Thomas Roten <thomas@roten.us>
 License-Expression: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE.txt
 Keywords: cc-cedict,cedict,characters,chinese,cjk,han,hanzi,mandarin,pinyin,punctuation,radicals,segmentation,simplified,tokenization,traditional,unicode,zhuyin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -67,24 +69,24 @@
 
     >>> re.findall(zhon.pinyin.sentence, 'Yuànzi lǐ tíngzhe yí liàng chē.', re.I)
     ['Yuànzi lǐ tíngzhe yí liàng chē.']
 
 Features
 --------
 
-* Includes commonly-used constants:
-    - CJK characters and radicals
-    - Chinese punctuation marks
-    - Chinese sentence regular expression pattern
-    - Pinyin vowels, consonants, lowercase, uppercase, and punctuation
-    - Pinyin syllable, word, and sentence regular expression patterns
-    - Zhuyin characters and marks
-    - Zhuyin syllable regular expression pattern
-    - CC-CEDICT characters
+Zhon includes the following commonly-used constants:
+
+* CJK characters and radicals
+* Chinese punctuation marks
+* Chinese sentence regular expression pattern
+* Pinyin vowels, consonants, lowercase, uppercase, and punctuation
+* Pinyin syllable, word, and sentence regular expression patterns
+* Zhuyin characters and marks
+* Zhuyin syllable regular expression pattern
+* CC-CEDICT characters
 
 Getting Started
 ---------------
 
-* `Install Zhon <https://tsroten.github.io/zhon/#installation>`_
-* Read `Zhon's introduction <https://tsroten.github.io/zhon/#using-zhon>`_
-* Learn from the `API documentation <https://tsroten.github.io/zhon/#module-zhon.hanzi>`_
+* `Install Zhon <https://tsroten.github.io/zhon/installation.html>`_
+* `Learn how to use Zhon <https://tsroten.github.io/zhon/api.html>`_
 * `Contribute <https://github.com/tsroten/zhon/blob/develop/CONTRIBUTING.rst>`_ documentation, code, or feedback
```

