# Comparing `tmp/pysigma_backend_elasticsearch-1.0.3.tar.gz` & `tmp/pysigma_backend_elasticsearch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_elasticsearch-1.0.3.tar", max compression
+gzip compressed data, was "pysigma_backend_elasticsearch-1.0.4.tar", max compression
```

## Comparing `pysigma_backend_elasticsearch-1.0.3.tar` & `pysigma_backend_elasticsearch-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7653 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/LICENSE
--rw-r--r--   0        0        0     1456 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/README.md
--rw-r--r--   0        0        0      978 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/sigma/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0    15481 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/sigma/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0      308 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/sigma/pipelines/elasticsearch/__init__.py
--rw-r--r--   0        0        0    10115 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/sigma/pipelines/elasticsearch/windows.py
--rw-r--r--   0        0        0    60963 2023-04-20 10:17:04.778373 pysigma_backend_elasticsearch-1.0.3/sigma/pipelines/elasticsearch/zeek.py
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1456 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/README.md
+-rw-r--r--   0        0        0      978 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    16130 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0      308 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    10115 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/windows.py
+-rw-r--r--   0        0        0    60963 2023-06-27 13:42:07.048584 pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/zeek.py
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.4/PKG-INFO
```

### Comparing `pysigma_backend_elasticsearch-1.0.3/LICENSE` & `pysigma_backend_elasticsearch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.3/README.md` & `pysigma_backend_elasticsearch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.3/pyproject.toml` & `pysigma_backend_elasticsearch-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-elasticsearch"
-version = "1.0.3"
+version = "1.0.4"
 description = "pySigma Elasticsearch backend"
 readme = "README.md"
 authors = ["Thomas Patzke <thomas@patzke.org>", "Hendrik Baecker <hb@process-zero.de>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-elasticsearch"
 packages = [
     { include = "sigma" }
```

### Comparing `pysigma_backend_elasticsearch-1.0.3/sigma/backends/elasticsearch/elasticsearch.py` & `pysigma_backend_elasticsearch-1.0.4/sigma/backends/elasticsearch/elasticsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import ClassVar, Dict, List, Optional, Pattern, Tuple, Union
 
 from sigma.conversion.state import ConversionState
 from sigma.rule import SigmaRule
 from sigma.conversion.base import TextQueryBackend
 from sigma.conversion.deferred import DeferredQueryExpression
 from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT, ConditionFieldEqualsValueExpression
-from sigma.types import SigmaCompareExpression
+from sigma.types import SigmaCompareExpression, SigmaNull
 import sigma
 
 
 class LuceneBackend(TextQueryBackend):
     """
     Elasticsearch query string backend. Generates query strings described here in the 
     Elasticsearch documentation:
@@ -56,16 +56,16 @@
     field_escape: ClassVar[str] = "\\"
     # All matches of this pattern are prepended with the string contained in field_escape.
     field_escape_pattern: ClassVar[Pattern] = re.compile("[\\s*]")
 
     # Values
     # string quoting character (added as escaping character)
     str_quote: ClassVar[str] = '"'
-    str_quote_pattern: ClassVar[Pattern] = re.compile(".")
-    str_quote_pattern_negation: ClassVar[bool] = True
+    str_quote_pattern: ClassVar[Pattern] = re.compile(r"^$|.*\s.*")
+    str_quote_pattern_negation: ClassVar[bool] = False
     # Escaping character for special characrers inside string
     escape_char: ClassVar[str] = "\\"
     # Character used as multi-character wildcard
     wildcard_multi: ClassVar[str] = "*"
     # Character used as single-character wildcard
     wildcard_single: ClassVar[str] = "?"
     # Characters quoted in addition to wildcards and string quote
@@ -164,20 +164,36 @@
             "INFORMATIONAL": 1,
             "LOW": 21,
             "MEDIUM": 47,
             "HIGH": 73,
             "CRITICAL": 99
         }
 
-    def convert_condition_field_eq_val_null(self, cond: ConditionFieldEqualsValueExpression, state: ConversionState) -> Union[str, DeferredQueryExpression]:
-        """Conversion of field is null expression value expressions"""
-        if cond.parent_condition_chain_contains(ConditionNOT):
-            return self.field_null_expression.format(field=self.escape_and_quote_field(cond.field)).replace(f"{self.not_token} ", "")
-        else:
-            return self.field_null_expression.format(field=self.escape_and_quote_field(cond.field))
+    @staticmethod
+    def _is_field_null_condition(cond : ConditionItem) -> bool:
+        return isinstance(cond, ConditionFieldEqualsValueExpression) and isinstance(cond.value, SigmaNull)
+
+    def convert_condition_not(self, cond : ConditionNOT, state : ConversionState) -> Union[str, DeferredQueryExpression]:
+        """When checking if a field is not null, convert "NOT NOT _exists_:field" to "_exists_:field"."""
+        if LuceneBackend._is_field_null_condition(cond.args[0]):
+            return f"_exists_:{cond.args[0].field}"
+
+        return super().convert_condition_not(cond, state)
+
+    def compare_precedence(self, outer : ConditionItem, inner : ConditionItem) -> bool:
+        """Override precedence check for null field conditions."""
+        if isinstance(inner, ConditionNOT) and LuceneBackend._is_field_null_condition(inner.args[0]):
+            # inner will turn into "_exists_:field", no parentheses needed
+            return True
+
+        if LuceneBackend._is_field_null_condition(inner):
+            # inner will turn into "NOT _exists_:field", force parentheses
+            return False
+
+        return super().compare_precedence(outer, inner)
 
     def finalize_query_dsl_lucene(
             self,
             rule: SigmaRule,
             query: str,
             index: int,
             state: ConversionState) -> Dict:
```

### Comparing `pysigma_backend_elasticsearch-1.0.3/sigma/pipelines/elasticsearch/windows.py` & `pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/windows.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.3/sigma/pipelines/elasticsearch/zeek.py` & `pysigma_backend_elasticsearch-1.0.4/sigma/pipelines/elasticsearch/zeek.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.3/PKG-INFO` & `pysigma_backend_elasticsearch-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-elasticsearch
-Version: 1.0.3
+Version: 1.0.4
 Summary: pySigma Elasticsearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-elasticsearch
 License: LGPL-3.0-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

